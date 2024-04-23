# Comparing `tmp/django_sql_explorer-4.1b5.tar.gz` & `tmp/django_sql_explorer-4.1b6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_sql_explorer-4.1b5.tar", last modified: Fri Apr 19 00:21:16 2024, max compression
+gzip compressed data, was "django_sql_explorer-4.1b6.tar", last modified: Tue Apr 23 02:38:17 2024, max compression
```

## Comparing `django_sql_explorer-4.1b5.tar` & `django_sql_explorer-4.1b6.tar`

### file list

```diff
@@ -1,159 +1,158 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:21:16.029594 django_sql_explorer-4.1b5/
--rw-r--r--   0 runner    (1001) docker     (127)      523 2024-04-19 00:20:56.000000 django_sql_explorer-4.1b5/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-04-19 00:20:56.000000 django_sql_explorer-4.1b5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-19 00:20:56.000000 django_sql_explorer-4.1b5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5231 2024-04-19 00:21:16.029594 django_sql_explorer-4.1b5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3349 2024-04-19 00:20:56.000000 django_sql_explorer-4.1b5/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:21:16.029594 django_sql_explorer-4.1b5/django_sql_explorer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5231 2024-04-19 00:21:15.000000 django_sql_explorer-4.1b5/django_sql_explorer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4381 2024-04-19 00:21:15.000000 django_sql_explorer-4.1b5/django_sql_explorer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 00:21:15.000000 django_sql_explorer-4.1b5/django_sql_explorer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 00:21:15.000000 django_sql_explorer-4.1b5/django_sql_explorer.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-19 00:21:15.000000 django_sql_explorer-4.1b5/django_sql_explorer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-19 00:21:15.000000 django_sql_explorer-4.1b5/django_sql_explorer.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:21:16.005593 django_sql_explorer-4.1b5/explorer/
--rw-r--r--   0 runner    (1001) docker     (127)      636 2024-04-19 00:20:56.000000 django_sql_explorer-4.1b5/explorer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1741 2024-04-19 00:20:56.000000 django_sql_explorer-4.1b5/explorer/actions.py
--rw-r--r--   0 runner    (1001) docker     (127)      356 2024-04-19 00:20:56.000000 django_sql_explorer-4.1b5/explorer/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)     4948 2024-04-19 00:20:56.000000 django_sql_explorer-4.1b5/explorer/app_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     2659 2024-04-19 00:20:56.000000 django_sql_explorer-4.1b5/explorer/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:21:16.005593 django_sql_explorer-4.1b5/explorer/assistant/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 00:20:56.000000 django_sql_explorer-4.1b5/explorer/assistant/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      620 2024-04-19 00:20:56.000000 django_sql_explorer-4.1b5/explorer/assistant/models.py
--rw-r--r--   0 runner    (1001) docker     (127)      538 2024-04-19 00:20:56.000000 django_sql_explorer-4.1b5/explorer/assistant/prompts.py
--rw-r--r--   0 runner    (1001) docker     (127)     4329 2024-04-19 00:20:56.000000 django_sql_explorer-4.1b5/explorer/assistant/tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     2747 2024-04-19 00:20:56.000000 django_sql_explorer-4.1b5/explorer/assistant/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2934 2024-04-19 00:20:56.000000 django_sql_explorer-4.1b5/explorer/assistant/views.py
--rw-r--r--   0 runner    (1001) docker     (127)     3313 2024-04-19 00:20:56.000000 django_sql_explorer-4.1b5/explorer/charts.py
--rw-r--r--   0 runner    (1001) docker     (127)      754 2024-04-19 00:20:56.000000 django_sql_explorer-4.1b5/explorer/connections.py
--rw-r--r--   0 runner    (1001) docker     (127)     3861 2024-04-19 00:20:56.000000 django_sql_explorer-4.1b5/explorer/exporters.py
--rw-r--r--   0 runner    (1001) docker     (127)     2050 2024-04-19 00:20:56.000000 django_sql_explorer-4.1b5/explorer/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:21:15.997593 django_sql_explorer-4.1b5/explorer/locale/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:21:15.997593 django_sql_explorer-4.1b5/explorer/locale/ru/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:21:16.009593 django_sql_explorer-4.1b5/explorer/locale/ru/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     5335 2024-04-19 00:20:56.000000 django_sql_explorer-4.1b5/explorer/locale/ru/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)    10091 2024-04-19 00:20:56.000000 django_sql_explorer-4.1b5/explorer/locale/ru/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:21:15.997593 django_sql_explorer-4.1b5/explorer/locale/zh_Hans/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:21:16.009593 django_sql_explorer-4.1b5/explorer/locale/zh_Hans/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     2549 2024-04-19 00:20:56.000000 django_sql_explorer-4.1b5/explorer/locale/zh_Hans/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     4863 2024-04-19 00:20:56.000000 django_sql_explorer-4.1b5/explorer/locale/zh_Hans/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:21:16.009593 django_sql_explorer-4.1b5/explorer/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)     1905 2024-04-19 00:20:56.000000 django_sql_explorer-4.1b5/explorer/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)      435 2024-04-19 00:20:56.000000 django_sql_explorer-4.1b5/explorer/migrations/0002_auto_20150501_1515.py
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-04-19 00:20:56.000000 django_sql_explorer-4.1b5/explorer/migrations/0003_query_snapshot.py
--rw-r--r--   0 runner    (1001) docker     (127)      345 2024-04-19 00:20:56.000000 django_sql_explorer-4.1b5/explorer/migrations/0004_querylog_duration.py
--rw-r--r--   0 runner    (1001) docker     (127)      439 2024-04-19 00:20:56.000000 django_sql_explorer-4.1b5/explorer/migrations/0005_auto_20160105_2052.py
--rw-r--r--   0 runner    (1001) docker     (127)      500 2024-04-19 00:20:56.000000 django_sql_explorer-4.1b5/explorer/migrations/0006_query_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)      364 2024-04-19 00:20:56.000000 django_sql_explorer-4.1b5/explorer/migrations/0007_querylog_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)      502 2024-04-19 00:20:56.000000 django_sql_explorer-4.1b5/explorer/migrations/0008_auto_20190308_1642.py
--rw-r--r--   0 runner    (1001) docker     (127)      913 2024-04-19 00:20:56.000000 django_sql_explorer-4.1b5/explorer/migrations/0009_auto_20201009_0547.py
--rw-r--r--   0 runner    (1001) docker     (127)      370 2024-04-19 00:20:56.000000 django_sql_explorer-4.1b5/explorer/migrations/0010_sql_required.py
--rw-r--r--   0 runner    (1001) docker     (127)      914 2024-04-19 00:20:56.000000 django_sql_explorer-4.1b5/explorer/migrations/0011_query_favorites.py
--rw-r--r--   0 runner    (1001) docker     (127)      971 2024-04-19 00:20:56.000000 django_sql_explorer-4.1b5/explorer/migrations/0012_alter_queryfavorite_query_alter_queryfavorite_user.py
--rw-r--r--   0 runner    (1001) docker     (127)      582 2024-04-19 00:20:56.000000 django_sql_explorer-4.1b5/explorer/migrations/0013_querylog_error_querylog_success.py
--rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-04-19 00:20:56.000000 django_sql_explorer-4.1b5/explorer/migrations/0014_promptlog.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 00:20:56.000000 django_sql_explorer-4.1b5/explorer/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11007 2024-04-19 00:20:56.000000 django_sql_explorer-4.1b5/explorer/models.py
--rw-r--r--   0 runner    (1001) docker     (127)      954 2024-04-19 00:20:56.000000 django_sql_explorer-4.1b5/explorer/permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3478 2024-04-19 00:20:56.000000 django_sql_explorer-4.1b5/explorer/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:21:16.001593 django_sql_explorer-4.1b5/explorer/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:21:16.013594 django_sql_explorer-4.1b5/explorer/src/js/
--rw-r--r--   0 runner    (1001) docker     (127)     6182 2024-04-19 00:20:56.000000 django_sql_explorer-4.1b5/explorer/src/js/assistant.js
--rw-r--r--   0 runner    (1001) docker     (127)     2189 2024-04-19 00:20:56.000000 django_sql_explorer-4.1b5/explorer/src/js/codemirror-config.js
--rw-r--r--   0 runner    (1001) docker     (127)      442 2024-04-19 00:20:56.000000 django_sql_explorer-4.1b5/explorer/src/js/csrf.js
--rw-r--r--   0 runner    (1001) docker     (127)    13060 2024-04-19 00:20:56.000000 django_sql_explorer-4.1b5/explorer/src/js/explorer.js
--rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-04-19 00:20:56.000000 django_sql_explorer-4.1b5/explorer/src/js/favorites.js
--rw-r--r--   0 runner    (1001) docker     (127)     1389 2024-04-19 00:20:56.000000 django_sql_explorer-4.1b5/explorer/src/js/main.js
--rw-r--r--   0 runner    (1001) docker     (127)     1281 2024-04-19 00:20:56.000000 django_sql_explorer-4.1b5/explorer/src/js/pivot-setup.js
--rw-r--r--   0 runner    (1001) docker     (127)    77235 2024-04-19 00:20:56.000000 django_sql_explorer-4.1b5/explorer/src/js/pivot.js
--rw-r--r--   0 runner    (1001) docker     (127)     3393 2024-04-19 00:20:56.000000 django_sql_explorer-4.1b5/explorer/src/js/query-list.js
--rw-r--r--   0 runner    (1001) docker     (127)     1351 2024-04-19 00:20:56.000000 django_sql_explorer-4.1b5/explorer/src/js/schema.js
--rw-r--r--   0 runner    (1001) docker     (127)      884 2024-04-19 00:20:56.000000 django_sql_explorer-4.1b5/explorer/src/js/table-to-csv.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:21:16.013594 django_sql_explorer-4.1b5/explorer/src/scss/
--rw-r--r--   0 runner    (1001) docker     (127)      620 2024-04-19 00:20:56.000000 django_sql_explorer-4.1b5/explorer/src/scss/assistant.scss
--rw-r--r--   0 runner    (1001) docker     (127)     1837 2024-04-19 00:20:56.000000 django_sql_explorer-4.1b5/explorer/src/scss/explorer.scss
--rw-r--r--   0 runner    (1001) docker     (127)     2597 2024-04-19 00:20:56.000000 django_sql_explorer-4.1b5/explorer/src/scss/pivot.css
--rw-r--r--   0 runner    (1001) docker     (127)      255 2024-04-19 00:20:56.000000 django_sql_explorer-4.1b5/explorer/src/scss/styles.scss
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-19 00:20:56.000000 django_sql_explorer-4.1b5/explorer/src/scss/variables.scss
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:21:16.001593 django_sql_explorer-4.1b5/explorer/static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:21:16.017593 django_sql_explorer-4.1b5/explorer/static/explorer/
--rw-r--r--   0 runner    (1001) docker     (127)   176088 2024-04-19 00:21:09.000000 django_sql_explorer-4.1b5/explorer/static/explorer/bootstrap-icons.woff
--rw-r--r--   0 runner    (1001) docker     (127)   130648 2024-04-19 00:21:09.000000 django_sql_explorer-4.1b5/explorer/static/explorer/bootstrap-icons.woff2
--rw-r--r--   0 runner    (1001) docker     (127)   546668 2024-04-19 00:21:09.000000 django_sql_explorer-4.1b5/explorer/static/explorer/explorer.js
--rw-r--r--   0 runner    (1001) docker     (127)     2704 2024-04-19 00:21:09.000000 django_sql_explorer-4.1b5/explorer/static/explorer/favorites.js
--rw-r--r--   0 runner    (1001) docker     (127)    18658 2024-04-19 00:21:09.000000 django_sql_explorer-4.1b5/explorer/static/explorer/index.js
--rw-r--r--   0 runner    (1001) docker     (127)    84338 2024-04-19 00:21:09.000000 django_sql_explorer-4.1b5/explorer/static/explorer/main.js
--rw-r--r--   0 runner    (1001) docker     (127)    66999 2024-04-19 00:21:09.000000 django_sql_explorer-4.1b5/explorer/static/explorer/pivot-setup.js
--rw-r--r--   0 runner    (1001) docker     (127)     1778 2024-04-19 00:21:09.000000 django_sql_explorer-4.1b5/explorer/static/explorer/query-list.js
--rw-r--r--   0 runner    (1001) docker     (127)      879 2024-04-19 00:21:09.000000 django_sql_explorer-4.1b5/explorer/static/explorer/schema.js
--rw-r--r--   0 runner    (1001) docker     (127)   308829 2024-04-19 00:21:09.000000 django_sql_explorer-4.1b5/explorer/static/explorer/styles.css
--rw-r--r--   0 runner    (1001) docker     (127)     3705 2024-04-19 00:20:56.000000 django_sql_explorer-4.1b5/explorer/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:21:16.001593 django_sql_explorer-4.1b5/explorer/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:21:16.021593 django_sql_explorer-4.1b5/explorer/templates/explorer/
--rw-r--r--   0 runner    (1001) docker     (127)     3028 2024-04-19 00:20:56.000000 django_sql_explorer-4.1b5/explorer/templates/explorer/assistant.html
--rw-r--r--   0 runner    (1001) docker     (127)     3524 2024-04-19 00:20:56.000000 django_sql_explorer-4.1b5/explorer/templates/explorer/base.html
--rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-04-19 00:20:56.000000 django_sql_explorer-4.1b5/explorer/templates/explorer/export_buttons.html
--rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-04-19 00:20:56.000000 django_sql_explorer-4.1b5/explorer/templates/explorer/fullscreen.html
--rw-r--r--   0 runner    (1001) docker     (127)      571 2024-04-19 00:20:56.000000 django_sql_explorer-4.1b5/explorer/templates/explorer/params.html
--rw-r--r--   0 runner    (1001) docker     (127)      548 2024-04-19 00:20:56.000000 django_sql_explorer-4.1b5/explorer/templates/explorer/pdf_template.html
--rw-r--r--   0 runner    (1001) docker     (127)     3708 2024-04-19 00:20:56.000000 django_sql_explorer-4.1b5/explorer/templates/explorer/play.html
--rw-r--r--   0 runner    (1001) docker     (127)    12827 2024-04-19 00:20:56.000000 django_sql_explorer-4.1b5/explorer/templates/explorer/preview_pane.html
--rw-r--r--   0 runner    (1001) docker     (127)     7987 2024-04-19 00:20:56.000000 django_sql_explorer-4.1b5/explorer/templates/explorer/query.html
--rw-r--r--   0 runner    (1001) docker     (127)      552 2024-04-19 00:20:56.000000 django_sql_explorer-4.1b5/explorer/templates/explorer/query_confirm_delete.html
--rw-r--r--   0 runner    (1001) docker     (127)      314 2024-04-19 00:20:56.000000 django_sql_explorer-4.1b5/explorer/templates/explorer/query_favorite_button.html
--rw-r--r--   0 runner    (1001) docker     (127)      885 2024-04-19 00:20:56.000000 django_sql_explorer-4.1b5/explorer/templates/explorer/query_favorites.html
--rw-r--r--   0 runner    (1001) docker     (127)     7641 2024-04-19 00:20:56.000000 django_sql_explorer-4.1b5/explorer/templates/explorer/query_list.html
--rw-r--r--   0 runner    (1001) docker     (127)     2915 2024-04-19 00:20:56.000000 django_sql_explorer-4.1b5/explorer/templates/explorer/querylog_list.html
--rw-r--r--   0 runner    (1001) docker     (127)     1686 2024-04-19 00:20:56.000000 django_sql_explorer-4.1b5/explorer/templates/explorer/schema.html
--rw-r--r--   0 runner    (1001) docker     (127)      294 2024-04-19 00:20:56.000000 django_sql_explorer-4.1b5/explorer/templates/explorer/schema_building.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:21:16.021593 django_sql_explorer-4.1b5/explorer/templatetags/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 00:20:56.000000 django_sql_explorer-4.1b5/explorer/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      756 2024-04-19 00:20:56.000000 django_sql_explorer-4.1b5/explorer/templatetags/explorer_tags.py
--rw-r--r--   0 runner    (1001) docker     (127)     1588 2024-04-19 00:20:56.000000 django_sql_explorer-4.1b5/explorer/templatetags/vite.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:21:16.025594 django_sql_explorer-4.1b5/explorer/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 00:20:56.000000 django_sql_explorer-4.1b5/explorer/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      771 2024-04-19 00:20:56.000000 django_sql_explorer-4.1b5/explorer/tests/factories.py
--rw-r--r--   0 runner    (1001) docker     (127)      767 2024-04-19 00:20:56.000000 django_sql_explorer-4.1b5/explorer/tests/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     1433 2024-04-19 00:20:56.000000 django_sql_explorer-4.1b5/explorer/tests/test_actions.py
--rw-r--r--   0 runner    (1001) docker     (127)      704 2024-04-19 00:20:56.000000 django_sql_explorer-4.1b5/explorer/tests/test_apps.py
--rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-04-19 00:20:56.000000 django_sql_explorer-4.1b5/explorer/tests/test_csrf_cookie_name.py
--rw-r--r--   0 runner    (1001) docker     (127)     4235 2024-04-19 00:20:56.000000 django_sql_explorer-4.1b5/explorer/tests/test_exporters.py
--rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-04-19 00:20:56.000000 django_sql_explorer-4.1b5/explorer/tests/test_forms.py
--rw-r--r--   0 runner    (1001) docker     (127)     8449 2024-04-19 00:20:56.000000 django_sql_explorer-4.1b5/explorer/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     3947 2024-04-19 00:20:56.000000 django_sql_explorer-4.1b5/explorer/tests/test_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     3414 2024-04-19 00:20:56.000000 django_sql_explorer-4.1b5/explorer/tests/test_tasks.py
--rw-r--r--   0 runner    (1001) docker     (127)      637 2024-04-19 00:20:56.000000 django_sql_explorer-4.1b5/explorer/tests/test_tracker.py
--rw-r--r--   0 runner    (1001) docker     (127)    10140 2024-04-19 00:20:56.000000 django_sql_explorer-4.1b5/explorer/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    32207 2024-04-19 00:20:56.000000 django_sql_explorer-4.1b5/explorer/tests/test_views.py
--rw-r--r--   0 runner    (1001) docker     (127)      291 2024-04-19 00:20:56.000000 django_sql_explorer-4.1b5/explorer/tests/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)     3744 2024-04-19 00:20:56.000000 django_sql_explorer-4.1b5/explorer/tracker.py
--rw-r--r--   0 runner    (1001) docker     (127)     1736 2024-04-19 00:20:56.000000 django_sql_explorer-4.1b5/explorer/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)     6197 2024-04-19 00:20:56.000000 django_sql_explorer-4.1b5/explorer/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:21:16.025594 django_sql_explorer-4.1b5/explorer/views/
--rw-r--r--   0 runner    (1001) docker     (127)      911 2024-04-19 00:20:56.000000 django_sql_explorer-4.1b5/explorer/views/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1625 2024-04-19 00:20:56.000000 django_sql_explorer-4.1b5/explorer/views/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)      546 2024-04-19 00:20:56.000000 django_sql_explorer-4.1b5/explorer/views/create.py
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-04-19 00:20:56.000000 django_sql_explorer-4.1b5/explorer/views/delete.py
--rw-r--r--   0 runner    (1001) docker     (127)      909 2024-04-19 00:20:56.000000 django_sql_explorer-4.1b5/explorer/views/download.py
--rw-r--r--   0 runner    (1001) docker     (127)      688 2024-04-19 00:20:56.000000 django_sql_explorer-4.1b5/explorer/views/email.py
--rw-r--r--   0 runner    (1001) docker     (127)      874 2024-04-19 00:20:56.000000 django_sql_explorer-4.1b5/explorer/views/export.py
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-19 00:20:56.000000 django_sql_explorer-4.1b5/explorer/views/format_sql.py
--rw-r--r--   0 runner    (1001) docker     (127)     5375 2024-04-19 00:20:56.000000 django_sql_explorer-4.1b5/explorer/views/list.py
--rw-r--r--   0 runner    (1001) docker     (127)      951 2024-04-19 00:20:56.000000 django_sql_explorer-4.1b5/explorer/views/mixins.py
--rw-r--r--   0 runner    (1001) docker     (127)     5038 2024-04-19 00:20:56.000000 django_sql_explorer-4.1b5/explorer/views/query.py
--rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-04-19 00:20:56.000000 django_sql_explorer-4.1b5/explorer/views/query_favorite.py
--rw-r--r--   0 runner    (1001) docker     (127)     1426 2024-04-19 00:20:56.000000 django_sql_explorer-4.1b5/explorer/views/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)      632 2024-04-19 00:20:56.000000 django_sql_explorer-4.1b5/explorer/views/stream.py
--rw-r--r--   0 runner    (1001) docker     (127)     2750 2024-04-19 00:20:56.000000 django_sql_explorer-4.1b5/explorer/views/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      970 2024-04-19 00:20:56.000000 django_sql_explorer-4.1b5/package.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:21:16.025594 django_sql_explorer-4.1b5/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-19 00:20:56.000000 django_sql_explorer-4.1b5/requirements/base.txt
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-04-19 00:20:56.000000 django_sql_explorer-4.1b5/requirements/dev.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:21:16.029594 django_sql_explorer-4.1b5/requirements/extra/
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-19 00:20:56.000000 django_sql_explorer-4.1b5/requirements/extra/assistant.txt
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-19 00:20:56.000000 django_sql_explorer-4.1b5/requirements/extra/charts.txt
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-19 00:20:56.000000 django_sql_explorer-4.1b5/requirements/extra/snapshots.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-19 00:20:56.000000 django_sql_explorer-4.1b5/requirements/extra/xls.txt
--rw-r--r--   0 runner    (1001) docker     (127)      814 2024-04-19 00:21:16.029594 django_sql_explorer-4.1b5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3111 2024-04-19 00:20:56.000000 django_sql_explorer-4.1b5/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-04-19 00:20:56.000000 django_sql_explorer-4.1b5/vite.config.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 02:38:17.521280 django_sql_explorer-4.1b6/
+-rw-r--r--   0 runner    (1001) docker     (127)      523 2024-04-23 02:37:58.000000 django_sql_explorer-4.1b6/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-04-23 02:37:58.000000 django_sql_explorer-4.1b6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-23 02:37:58.000000 django_sql_explorer-4.1b6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5240 2024-04-23 02:38:17.521280 django_sql_explorer-4.1b6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3358 2024-04-23 02:37:58.000000 django_sql_explorer-4.1b6/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 02:38:17.521280 django_sql_explorer-4.1b6/django_sql_explorer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5240 2024-04-23 02:38:17.000000 django_sql_explorer-4.1b6/django_sql_explorer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4358 2024-04-23 02:38:17.000000 django_sql_explorer-4.1b6/django_sql_explorer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 02:38:17.000000 django_sql_explorer-4.1b6/django_sql_explorer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 02:38:17.000000 django_sql_explorer-4.1b6/django_sql_explorer.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-23 02:38:17.000000 django_sql_explorer-4.1b6/django_sql_explorer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-23 02:38:17.000000 django_sql_explorer-4.1b6/django_sql_explorer.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 02:38:17.501280 django_sql_explorer-4.1b6/explorer/
+-rw-r--r--   0 runner    (1001) docker     (127)      636 2024-04-23 02:37:58.000000 django_sql_explorer-4.1b6/explorer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1741 2024-04-23 02:37:58.000000 django_sql_explorer-4.1b6/explorer/actions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      356 2024-04-23 02:37:58.000000 django_sql_explorer-4.1b6/explorer/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4948 2024-04-23 02:37:58.000000 django_sql_explorer-4.1b6/explorer/app_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2659 2024-04-23 02:37:58.000000 django_sql_explorer-4.1b6/explorer/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 02:38:17.501280 django_sql_explorer-4.1b6/explorer/assistant/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 02:37:58.000000 django_sql_explorer-4.1b6/explorer/assistant/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      620 2024-04-23 02:37:58.000000 django_sql_explorer-4.1b6/explorer/assistant/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      538 2024-04-23 02:37:58.000000 django_sql_explorer-4.1b6/explorer/assistant/prompts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4329 2024-04-23 02:37:58.000000 django_sql_explorer-4.1b6/explorer/assistant/tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2747 2024-04-23 02:37:58.000000 django_sql_explorer-4.1b6/explorer/assistant/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2934 2024-04-23 02:37:58.000000 django_sql_explorer-4.1b6/explorer/assistant/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3313 2024-04-23 02:37:58.000000 django_sql_explorer-4.1b6/explorer/charts.py
+-rw-r--r--   0 runner    (1001) docker     (127)      754 2024-04-23 02:37:58.000000 django_sql_explorer-4.1b6/explorer/connections.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3861 2024-04-23 02:37:58.000000 django_sql_explorer-4.1b6/explorer/exporters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-04-23 02:37:58.000000 django_sql_explorer-4.1b6/explorer/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 02:38:17.497280 django_sql_explorer-4.1b6/explorer/locale/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 02:38:17.497280 django_sql_explorer-4.1b6/explorer/locale/ru/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 02:38:17.501280 django_sql_explorer-4.1b6/explorer/locale/ru/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     5335 2024-04-23 02:37:58.000000 django_sql_explorer-4.1b6/explorer/locale/ru/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    10091 2024-04-23 02:37:58.000000 django_sql_explorer-4.1b6/explorer/locale/ru/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 02:38:17.497280 django_sql_explorer-4.1b6/explorer/locale/zh_Hans/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 02:38:17.505280 django_sql_explorer-4.1b6/explorer/locale/zh_Hans/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     2549 2024-04-23 02:37:58.000000 django_sql_explorer-4.1b6/explorer/locale/zh_Hans/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     4863 2024-04-23 02:37:58.000000 django_sql_explorer-4.1b6/explorer/locale/zh_Hans/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 02:38:17.505280 django_sql_explorer-4.1b6/explorer/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     1905 2024-04-23 02:37:58.000000 django_sql_explorer-4.1b6/explorer/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)      435 2024-04-23 02:37:58.000000 django_sql_explorer-4.1b6/explorer/migrations/0002_auto_20150501_1515.py
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-04-23 02:37:58.000000 django_sql_explorer-4.1b6/explorer/migrations/0003_query_snapshot.py
+-rw-r--r--   0 runner    (1001) docker     (127)      345 2024-04-23 02:37:58.000000 django_sql_explorer-4.1b6/explorer/migrations/0004_querylog_duration.py
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-04-23 02:37:58.000000 django_sql_explorer-4.1b6/explorer/migrations/0005_auto_20160105_2052.py
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-04-23 02:37:58.000000 django_sql_explorer-4.1b6/explorer/migrations/0006_query_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      364 2024-04-23 02:37:58.000000 django_sql_explorer-4.1b6/explorer/migrations/0007_querylog_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      502 2024-04-23 02:37:58.000000 django_sql_explorer-4.1b6/explorer/migrations/0008_auto_20190308_1642.py
+-rw-r--r--   0 runner    (1001) docker     (127)      913 2024-04-23 02:37:58.000000 django_sql_explorer-4.1b6/explorer/migrations/0009_auto_20201009_0547.py
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2024-04-23 02:37:58.000000 django_sql_explorer-4.1b6/explorer/migrations/0010_sql_required.py
+-rw-r--r--   0 runner    (1001) docker     (127)      914 2024-04-23 02:37:58.000000 django_sql_explorer-4.1b6/explorer/migrations/0011_query_favorites.py
+-rw-r--r--   0 runner    (1001) docker     (127)      971 2024-04-23 02:37:58.000000 django_sql_explorer-4.1b6/explorer/migrations/0012_alter_queryfavorite_query_alter_queryfavorite_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-04-23 02:37:58.000000 django_sql_explorer-4.1b6/explorer/migrations/0013_querylog_error_querylog_success.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-04-23 02:37:58.000000 django_sql_explorer-4.1b6/explorer/migrations/0014_promptlog.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 02:37:58.000000 django_sql_explorer-4.1b6/explorer/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11007 2024-04-23 02:37:58.000000 django_sql_explorer-4.1b6/explorer/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      954 2024-04-23 02:37:58.000000 django_sql_explorer-4.1b6/explorer/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3478 2024-04-23 02:37:58.000000 django_sql_explorer-4.1b6/explorer/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 02:38:17.497280 django_sql_explorer-4.1b6/explorer/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 02:38:17.509280 django_sql_explorer-4.1b6/explorer/src/js/
+-rw-r--r--   0 runner    (1001) docker     (127)     5807 2024-04-23 02:37:58.000000 django_sql_explorer-4.1b6/explorer/src/js/assistant.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2189 2024-04-23 02:37:58.000000 django_sql_explorer-4.1b6/explorer/src/js/codemirror-config.js
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2024-04-23 02:37:58.000000 django_sql_explorer-4.1b6/explorer/src/js/csrf.js
+-rw-r--r--   0 runner    (1001) docker     (127)    13023 2024-04-23 02:37:58.000000 django_sql_explorer-4.1b6/explorer/src/js/explorer.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-04-23 02:37:58.000000 django_sql_explorer-4.1b6/explorer/src/js/favorites.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1389 2024-04-23 02:37:58.000000 django_sql_explorer-4.1b6/explorer/src/js/main.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1281 2024-04-23 02:37:58.000000 django_sql_explorer-4.1b6/explorer/src/js/pivot-setup.js
+-rw-r--r--   0 runner    (1001) docker     (127)    77235 2024-04-23 02:37:58.000000 django_sql_explorer-4.1b6/explorer/src/js/pivot.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3393 2024-04-23 02:37:58.000000 django_sql_explorer-4.1b6/explorer/src/js/query-list.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1351 2024-04-23 02:37:58.000000 django_sql_explorer-4.1b6/explorer/src/js/schema.js
+-rw-r--r--   0 runner    (1001) docker     (127)      884 2024-04-23 02:37:58.000000 django_sql_explorer-4.1b6/explorer/src/js/table-to-csv.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 02:38:17.509280 django_sql_explorer-4.1b6/explorer/src/scss/
+-rw-r--r--   0 runner    (1001) docker     (127)      620 2024-04-23 02:37:58.000000 django_sql_explorer-4.1b6/explorer/src/scss/assistant.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     1837 2024-04-23 02:37:58.000000 django_sql_explorer-4.1b6/explorer/src/scss/explorer.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     2597 2024-04-23 02:37:58.000000 django_sql_explorer-4.1b6/explorer/src/scss/pivot.css
+-rw-r--r--   0 runner    (1001) docker     (127)      255 2024-04-23 02:37:58.000000 django_sql_explorer-4.1b6/explorer/src/scss/styles.scss
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-23 02:37:58.000000 django_sql_explorer-4.1b6/explorer/src/scss/variables.scss
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 02:38:17.497280 django_sql_explorer-4.1b6/explorer/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 02:38:17.509280 django_sql_explorer-4.1b6/explorer/static/explorer/
+-rw-r--r--   0 runner    (1001) docker     (127)   176088 2024-04-23 02:38:14.000000 django_sql_explorer-4.1b6/explorer/static/explorer/bootstrap-icons.woff
+-rw-r--r--   0 runner    (1001) docker     (127)   130648 2024-04-23 02:38:14.000000 django_sql_explorer-4.1b6/explorer/static/explorer/bootstrap-icons.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)   546399 2024-04-23 02:38:14.000000 django_sql_explorer-4.1b6/explorer/static/explorer/explorer.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2704 2024-04-23 02:38:14.000000 django_sql_explorer-4.1b6/explorer/static/explorer/favorites.js
+-rw-r--r--   0 runner    (1001) docker     (127)    18658 2024-04-23 02:38:14.000000 django_sql_explorer-4.1b6/explorer/static/explorer/index.js
+-rw-r--r--   0 runner    (1001) docker     (127)    84338 2024-04-23 02:38:14.000000 django_sql_explorer-4.1b6/explorer/static/explorer/main.js
+-rw-r--r--   0 runner    (1001) docker     (127)    66999 2024-04-23 02:38:14.000000 django_sql_explorer-4.1b6/explorer/static/explorer/pivot-setup.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1778 2024-04-23 02:38:14.000000 django_sql_explorer-4.1b6/explorer/static/explorer/query-list.js
+-rw-r--r--   0 runner    (1001) docker     (127)      879 2024-04-23 02:38:14.000000 django_sql_explorer-4.1b6/explorer/static/explorer/schema.js
+-rw-r--r--   0 runner    (1001) docker     (127)   308829 2024-04-23 02:38:14.000000 django_sql_explorer-4.1b6/explorer/static/explorer/styles.css
+-rw-r--r--   0 runner    (1001) docker     (127)     3705 2024-04-23 02:37:58.000000 django_sql_explorer-4.1b6/explorer/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 02:38:17.497280 django_sql_explorer-4.1b6/explorer/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 02:38:17.513280 django_sql_explorer-4.1b6/explorer/templates/explorer/
+-rw-r--r--   0 runner    (1001) docker     (127)     3499 2024-04-23 02:37:58.000000 django_sql_explorer-4.1b6/explorer/templates/explorer/assistant.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3524 2024-04-23 02:37:58.000000 django_sql_explorer-4.1b6/explorer/templates/explorer/base.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-04-23 02:37:58.000000 django_sql_explorer-4.1b6/explorer/templates/explorer/export_buttons.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-04-23 02:37:58.000000 django_sql_explorer-4.1b6/explorer/templates/explorer/fullscreen.html
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-04-23 02:37:58.000000 django_sql_explorer-4.1b6/explorer/templates/explorer/params.html
+-rw-r--r--   0 runner    (1001) docker     (127)      548 2024-04-23 02:37:58.000000 django_sql_explorer-4.1b6/explorer/templates/explorer/pdf_template.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3708 2024-04-23 02:37:58.000000 django_sql_explorer-4.1b6/explorer/templates/explorer/play.html
+-rw-r--r--   0 runner    (1001) docker     (127)    12827 2024-04-23 02:37:58.000000 django_sql_explorer-4.1b6/explorer/templates/explorer/preview_pane.html
+-rw-r--r--   0 runner    (1001) docker     (127)     7844 2024-04-23 02:37:58.000000 django_sql_explorer-4.1b6/explorer/templates/explorer/query.html
+-rw-r--r--   0 runner    (1001) docker     (127)      552 2024-04-23 02:37:58.000000 django_sql_explorer-4.1b6/explorer/templates/explorer/query_confirm_delete.html
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-04-23 02:37:58.000000 django_sql_explorer-4.1b6/explorer/templates/explorer/query_favorite_button.html
+-rw-r--r--   0 runner    (1001) docker     (127)      885 2024-04-23 02:37:58.000000 django_sql_explorer-4.1b6/explorer/templates/explorer/query_favorites.html
+-rw-r--r--   0 runner    (1001) docker     (127)     7641 2024-04-23 02:37:58.000000 django_sql_explorer-4.1b6/explorer/templates/explorer/query_list.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2915 2024-04-23 02:37:58.000000 django_sql_explorer-4.1b6/explorer/templates/explorer/querylog_list.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1686 2024-04-23 02:37:58.000000 django_sql_explorer-4.1b6/explorer/templates/explorer/schema.html
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-04-23 02:37:58.000000 django_sql_explorer-4.1b6/explorer/templates/explorer/schema_building.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 02:38:17.513280 django_sql_explorer-4.1b6/explorer/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 02:37:58.000000 django_sql_explorer-4.1b6/explorer/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      756 2024-04-23 02:37:58.000000 django_sql_explorer-4.1b6/explorer/templatetags/explorer_tags.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1588 2024-04-23 02:37:58.000000 django_sql_explorer-4.1b6/explorer/templatetags/vite.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 02:38:17.517280 django_sql_explorer-4.1b6/explorer/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 02:37:58.000000 django_sql_explorer-4.1b6/explorer/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      771 2024-04-23 02:37:58.000000 django_sql_explorer-4.1b6/explorer/tests/factories.py
+-rw-r--r--   0 runner    (1001) docker     (127)      767 2024-04-23 02:37:58.000000 django_sql_explorer-4.1b6/explorer/tests/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1433 2024-04-23 02:37:58.000000 django_sql_explorer-4.1b6/explorer/tests/test_actions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      704 2024-04-23 02:37:58.000000 django_sql_explorer-4.1b6/explorer/tests/test_apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-04-23 02:37:58.000000 django_sql_explorer-4.1b6/explorer/tests/test_csrf_cookie_name.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4235 2024-04-23 02:37:58.000000 django_sql_explorer-4.1b6/explorer/tests/test_exporters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-04-23 02:37:58.000000 django_sql_explorer-4.1b6/explorer/tests/test_forms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8449 2024-04-23 02:37:58.000000 django_sql_explorer-4.1b6/explorer/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3947 2024-04-23 02:37:58.000000 django_sql_explorer-4.1b6/explorer/tests/test_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3414 2024-04-23 02:37:58.000000 django_sql_explorer-4.1b6/explorer/tests/test_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)      637 2024-04-23 02:37:58.000000 django_sql_explorer-4.1b6/explorer/tests/test_tracker.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10140 2024-04-23 02:37:58.000000 django_sql_explorer-4.1b6/explorer/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32207 2024-04-23 02:37:58.000000 django_sql_explorer-4.1b6/explorer/tests/test_views.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3805 2024-04-23 02:37:58.000000 django_sql_explorer-4.1b6/explorer/tracker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1736 2024-04-23 02:37:58.000000 django_sql_explorer-4.1b6/explorer/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6197 2024-04-23 02:37:58.000000 django_sql_explorer-4.1b6/explorer/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 02:38:17.517280 django_sql_explorer-4.1b6/explorer/views/
+-rw-r--r--   0 runner    (1001) docker     (127)      911 2024-04-23 02:37:58.000000 django_sql_explorer-4.1b6/explorer/views/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1625 2024-04-23 02:37:58.000000 django_sql_explorer-4.1b6/explorer/views/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)      546 2024-04-23 02:37:58.000000 django_sql_explorer-4.1b6/explorer/views/create.py
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-04-23 02:37:58.000000 django_sql_explorer-4.1b6/explorer/views/delete.py
+-rw-r--r--   0 runner    (1001) docker     (127)      909 2024-04-23 02:37:58.000000 django_sql_explorer-4.1b6/explorer/views/download.py
+-rw-r--r--   0 runner    (1001) docker     (127)      688 2024-04-23 02:37:58.000000 django_sql_explorer-4.1b6/explorer/views/email.py
+-rw-r--r--   0 runner    (1001) docker     (127)      874 2024-04-23 02:37:58.000000 django_sql_explorer-4.1b6/explorer/views/export.py
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-23 02:37:58.000000 django_sql_explorer-4.1b6/explorer/views/format_sql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5375 2024-04-23 02:37:58.000000 django_sql_explorer-4.1b6/explorer/views/list.py
+-rw-r--r--   0 runner    (1001) docker     (127)      951 2024-04-23 02:37:58.000000 django_sql_explorer-4.1b6/explorer/views/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5038 2024-04-23 02:37:58.000000 django_sql_explorer-4.1b6/explorer/views/query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-04-23 02:37:58.000000 django_sql_explorer-4.1b6/explorer/views/query_favorite.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1426 2024-04-23 02:37:58.000000 django_sql_explorer-4.1b6/explorer/views/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2024-04-23 02:37:58.000000 django_sql_explorer-4.1b6/explorer/views/stream.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2750 2024-04-23 02:37:58.000000 django_sql_explorer-4.1b6/explorer/views/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      970 2024-04-23 02:37:58.000000 django_sql_explorer-4.1b6/package.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 02:38:17.517280 django_sql_explorer-4.1b6/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-23 02:37:58.000000 django_sql_explorer-4.1b6/requirements/base.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-04-23 02:37:58.000000 django_sql_explorer-4.1b6/requirements/dev.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 02:38:17.521280 django_sql_explorer-4.1b6/requirements/extra/
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-23 02:37:58.000000 django_sql_explorer-4.1b6/requirements/extra/assistant.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-23 02:37:58.000000 django_sql_explorer-4.1b6/requirements/extra/charts.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-23 02:37:58.000000 django_sql_explorer-4.1b6/requirements/extra/snapshots.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-23 02:37:58.000000 django_sql_explorer-4.1b6/requirements/extra/xls.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      814 2024-04-23 02:38:17.521280 django_sql_explorer-4.1b6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3111 2024-04-23 02:37:58.000000 django_sql_explorer-4.1b6/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-04-23 02:37:58.000000 django_sql_explorer-4.1b6/vite.config.js
```

### Comparing `django_sql_explorer-4.1b5/AUTHORS` & `django_sql_explorer-4.1b6/AUTHORS`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b5/LICENSE` & `django_sql_explorer-4.1b6/LICENSE`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b5/PKG-INFO` & `django_sql_explorer-4.1b6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-sql-explorer
-Version: 4.1b5
+Version: 4.1b6
 Summary: A pluggable app that allows users (admins) to execute SQL, view, and export the results.
 Home-page: https://www.sqlexplorer.io
 Author: Chris Clark
 Author-email: chris@untrod.com
 Maintainer: Mark Walker
 Maintainer-email: theshow@gmail.com
 License: MIT
@@ -132,8 +132,8 @@
 ------------
 
 Included is a test_project that you can use to kick the tires. Just
 create a new virtualenv, cd into ``test_project`` and run ``start.sh`` (or
 walk through the steps yourself) to get a test instance of the app up
 and running.
 
-You can now navigate to 127.0.0.1:8000/ and begin exploring!
+You can now navigate to 127.0.0.1:8000/explorer/ and begin exploring!
```

### Comparing `django_sql_explorer-4.1b5/README.rst` & `django_sql_explorer-4.1b6/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -86,8 +86,8 @@
 ------------
 
 Included is a test_project that you can use to kick the tires. Just
 create a new virtualenv, cd into ``test_project`` and run ``start.sh`` (or
 walk through the steps yourself) to get a test instance of the app up
 and running.
 
-You can now navigate to 127.0.0.1:8000/ and begin exploring!
+You can now navigate to 127.0.0.1:8000/explorer/ and begin exploring!
```

### Comparing `django_sql_explorer-4.1b5/django_sql_explorer.egg-info/PKG-INFO` & `django_sql_explorer-4.1b6/django_sql_explorer.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-sql-explorer
-Version: 4.1b5
+Version: 4.1b6
 Summary: A pluggable app that allows users (admins) to execute SQL, view, and export the results.
 Home-page: https://www.sqlexplorer.io
 Author: Chris Clark
 Author-email: chris@untrod.com
 Maintainer: Mark Walker
 Maintainer-email: theshow@gmail.com
 License: MIT
@@ -132,8 +132,8 @@
 ------------
 
 Included is a test_project that you can use to kick the tires. Just
 create a new virtualenv, cd into ``test_project`` and run ``start.sh`` (or
 walk through the steps yourself) to get a test instance of the app up
 and running.
 
-You can now navigate to 127.0.0.1:8000/ and begin exploring!
+You can now navigate to 127.0.0.1:8000/explorer/ and begin exploring!
```

### Comparing `django_sql_explorer-4.1b5/django_sql_explorer.egg-info/SOURCES.txt` & `django_sql_explorer-4.1b6/django_sql_explorer.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -108,15 +108,14 @@
 explorer/tests/test_forms.py
 explorer/tests/test_models.py
 explorer/tests/test_schema.py
 explorer/tests/test_tasks.py
 explorer/tests/test_tracker.py
 explorer/tests/test_utils.py
 explorer/tests/test_views.py
-explorer/tests/urls.py
 explorer/views/__init__.py
 explorer/views/auth.py
 explorer/views/create.py
 explorer/views/delete.py
 explorer/views/download.py
 explorer/views/email.py
 explorer/views/export.py
```

### Comparing `django_sql_explorer-4.1b5/explorer/__init__.py` & `django_sql_explorer-4.1b6/explorer/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 __version_info__ = {
     "major": 4,
     "minor": 1,
     "patch": 0,
     "releaselevel": "beta",
-    "serial": 5
+    "serial": 6
 }
 
 
 def get_version(short=False):
     assert __version_info__["releaselevel"] in ("alpha", "beta", "final")
     vers = ["%(major)i.%(minor)i" % __version_info__, ]
     if __version_info__["patch"]:
```

### Comparing `django_sql_explorer-4.1b5/explorer/actions.py` & `django_sql_explorer-4.1b6/explorer/actions.py`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b5/explorer/app_settings.py` & `django_sql_explorer-4.1b6/explorer/app_settings.py`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b5/explorer/apps.py` & `django_sql_explorer-4.1b6/explorer/apps.py`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b5/explorer/assistant/models.py` & `django_sql_explorer-4.1b6/explorer/assistant/models.py`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b5/explorer/assistant/prompts.py` & `django_sql_explorer-4.1b6/explorer/assistant/prompts.py`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b5/explorer/assistant/tests.py` & `django_sql_explorer-4.1b6/explorer/assistant/tests.py`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b5/explorer/assistant/utils.py` & `django_sql_explorer-4.1b6/explorer/assistant/utils.py`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b5/explorer/assistant/views.py` & `django_sql_explorer-4.1b6/explorer/assistant/views.py`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b5/explorer/charts.py` & `django_sql_explorer-4.1b6/explorer/charts.py`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b5/explorer/connections.py` & `django_sql_explorer-4.1b6/explorer/connections.py`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b5/explorer/exporters.py` & `django_sql_explorer-4.1b6/explorer/exporters.py`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b5/explorer/forms.py` & `django_sql_explorer-4.1b6/explorer/forms.py`

 * *Files 8% similar despite different names*

```diff
@@ -38,25 +38,21 @@
         super().__init__(*args, **kwargs)
         self.fields["connection"].widget.choices = self.connections
         if not self.instance.connection:
             self.initial["connection"] = EXPLORER_DEFAULT_CONNECTION
         self.fields["connection"].widget.attrs["class"] = "form-select"
 
     def clean(self):
-        if self.instance and self.data.get("created_by_user", None):
+        # Don't overwrite created_by_user
+        if self.instance and self.instance.created_by_user:
             self.cleaned_data["created_by_user"] = \
                 self.instance.created_by_user
         return super().clean()
 
     @property
-    def created_by_user_email(self):
-        return self.instance.created_by_user.email if \
-            self.instance.created_by_user else "--"
-
-    @property
     def created_at_time(self):
         return self.instance.created_at.strftime("%Y-%m-%d")
 
     @property
     def connections(self):
         return [(v, k) for k, v in EXPLORER_CONNECTIONS.items()]
```

### Comparing `django_sql_explorer-4.1b5/explorer/locale/ru/LC_MESSAGES/django.mo` & `django_sql_explorer-4.1b6/explorer/locale/ru/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b5/explorer/locale/ru/LC_MESSAGES/django.po` & `django_sql_explorer-4.1b6/explorer/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b5/explorer/locale/zh_Hans/LC_MESSAGES/django.mo` & `django_sql_explorer-4.1b6/explorer/locale/zh_Hans/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b5/explorer/locale/zh_Hans/LC_MESSAGES/django.po` & `django_sql_explorer-4.1b6/explorer/locale/zh_Hans/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b5/explorer/migrations/0001_initial.py` & `django_sql_explorer-4.1b6/explorer/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b5/explorer/migrations/0009_auto_20201009_0547.py` & `django_sql_explorer-4.1b6/explorer/migrations/0009_auto_20201009_0547.py`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b5/explorer/migrations/0011_query_favorites.py` & `django_sql_explorer-4.1b6/explorer/migrations/0011_query_favorites.py`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b5/explorer/migrations/0012_alter_queryfavorite_query_alter_queryfavorite_user.py` & `django_sql_explorer-4.1b6/explorer/migrations/0012_alter_queryfavorite_query_alter_queryfavorite_user.py`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b5/explorer/migrations/0013_querylog_error_querylog_success.py` & `django_sql_explorer-4.1b6/explorer/migrations/0013_querylog_error_querylog_success.py`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b5/explorer/migrations/0014_promptlog.py` & `django_sql_explorer-4.1b6/explorer/migrations/0014_promptlog.py`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b5/explorer/models.py` & `django_sql_explorer-4.1b6/explorer/models.py`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b5/explorer/permissions.py` & `django_sql_explorer-4.1b6/explorer/permissions.py`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b5/explorer/schema.py` & `django_sql_explorer-4.1b6/explorer/schema.py`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b5/explorer/src/js/assistant.js` & `django_sql_explorer-4.1b6/explorer/src/js/assistant.js`

 * *Files 13% similar despite different names*

#### js-beautify {}

```diff
@@ -5,38 +5,35 @@
     marked
 } from "marked";
 import DOMPurify from "dompurify";
 import * as bootstrap from 'bootstrap';
 import $ from "jquery";
 import List from "list.js";
 
-const spinner = "<div class=\"spinner-border text-primary\" role=\"status\"><span class=\"visually-hidden\">Loading...</span></div>";
-
 function getErrorMessage() {
     const errorElement = document.querySelector('.alert-danger.db-error');
     return errorElement ? errorElement.textContent.trim() : null;
 }
 
+function assistantSearchFocus() {
+    document.getElementById("search_assistant_tables").focus();
+}
+
 export function setUpAssistant(expand = false) {
 
     const error = getErrorMessage();
 
     if (expand || error) {
         const myCollapseElement = document.getElementById('assistant_collapse');
         const bsCollapse = new bootstrap.Collapse(myCollapseElement, {
             toggle: false
         });
         bsCollapse.show();
         if (error) {
-            const textarea = document.getElementById('id_assistant_input');
-            textarea.value = "Please help me fix the error(s) in this query.";
-            const newDiv = document.createElement('div');
-            newDiv.textContent = 'Error messages are automatically included in the prompt. Just hit "Ask Assistant" and all relevant context will be injected to the LLM request.'; // Add any text or HTML content
-            newDiv.className = 'text-secondary small';
-            textarea.parentNode.insertBefore(newDiv, textarea.nextSibling);
+            document.getElementById('id_error_help_message').classList.remove('d-none');
         }
     }
 
     const tooltipTriggerList = document.querySelectorAll('[data-bs-toggle="tooltip"]');
     [...tooltipTriggerList].map(tooltipTriggerEl => new bootstrap.Tooltip(tooltipTriggerEl));
 
     fetch('../schema.json/' + $("#id_connection").val())
@@ -83,66 +80,75 @@
     const assistantInputWrapper = document.getElementById('assistant_input_wrapper');
 
     function showHideExtraTables(checked) {
         if (checked) {
             additionalTableContainer.classList.remove('d-none');
             assistantInputWrapper.classList.remove('col-12');
             assistantInputWrapper.classList.add('col-9');
+            assistantSearchFocus();
         } else {
             additionalTableContainer.classList.add('d-none');
             assistantInputWrapper.classList.remove('col-9');
             assistantInputWrapper.classList.add('col-12');
         }
     }
     checkbox.addEventListener('change', function() {
         showHideExtraTables(this.checked);
     });
     showHideExtraTables(checkbox.checked);
 
-    document.getElementById('ask_assistant_btn').addEventListener('click', function() {
-
-        const selectedTables = Array.from(
-            document.querySelectorAll('.table-checkbox:checked')
-        ).map(cb => cb.value);
-
-        const data = {
-            sql: window.editor?.state.doc.toString() ?? null,
-            connection: document.getElementById("id_connection")?.value ?? null,
-            assistant_request: document.getElementById("id_assistant_input")?.value ?? null,
-            selected_tables: selectedTables,
-            db_error: getErrorMessage()
-        };
-
-        document.getElementById("response_block").style.display = "block";
-        document.getElementById("assistant_response").innerHTML = spinner;
-
-        fetch('/assistant/', {
-                method: 'POST',
-                headers: {
-                    'Content-Type': 'application/json',
-                    'X-CSRFToken': getCsrfToken()
-                },
-                body: JSON.stringify(data)
-            })
-            .then(response => {
-                if (!response.ok) {
-                    throw new Error('Network response was not ok');
-                }
-                return response.json();
-            })
-            .then(data => {
-                const output = DOMPurify.sanitize(marked.parse(data.message));
-                document.getElementById("response_block").style.display = "block";
-                document.getElementById("assistant_response").innerHTML = output;
-                setUpCopyButtons();
-            })
-            .catch(error => {
-                console.error('Error:', error);
-            });
+    document.getElementById('id_assistant_input').addEventListener('keydown', function(event) {
+        if ((event.ctrlKey || event.metaKey) && (event.key === 'Enter')) {
+            event.preventDefault();
+            submitAssistantAsk();
+        }
     });
+
+    document.getElementById('ask_assistant_btn').addEventListener('click', submitAssistantAsk);
+}
+
+function submitAssistantAsk() {
+
+    const selectedTables = Array.from(
+        document.querySelectorAll('.table-checkbox:checked')
+    ).map(cb => cb.value);
+
+    const data = {
+        sql: window.editor?.state.doc.toString() ?? null,
+        connection: document.getElementById("id_connection")?.value ?? null,
+        assistant_request: document.getElementById("id_assistant_input")?.value ?? null,
+        selected_tables: selectedTables,
+        db_error: getErrorMessage()
+    };
+
+    document.getElementById("response_block").classList.remove('d-none');
+    document.getElementById("assistant_spinner").classList.remove('d-none');
+
+    fetch('../assistant/', {
+            method: 'POST',
+            headers: {
+                'Content-Type': 'application/json',
+                'X-CSRFToken': getCsrfToken()
+            },
+            body: JSON.stringify(data)
+        })
+        .then(response => {
+            if (!response.ok) {
+                throw new Error('Network response was not ok');
+            }
+            return response.json();
+        })
+        .then(data => {
+            const output = DOMPurify.sanitize(marked.parse(data.message));
+            document.getElementById("assistant_response").innerHTML = output;
+            setUpCopyButtons();
+        })
+        .catch(error => {
+            console.error('Error:', error);
+        });
 }
 
 function setUpCopyButtons() {
     document.querySelectorAll('#assistant_response pre').forEach(pre => {
 
         const btn = document.createElement('i');
         btn.classList.add('copy-btn');
```

### Comparing `django_sql_explorer-4.1b5/explorer/src/js/codemirror-config.js` & `django_sql_explorer-4.1b6/explorer/src/js/codemirror-config.js`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b5/explorer/src/js/explorer.js` & `django_sql_explorer-4.1b6/explorer/src/js/explorer.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -52,15 +52,14 @@
             // Expand the assistant only if a new query is being created
             // and no results are yet being shown
             const expand = !pa && queryId === 'new';
             setUpAssistant(expand);
         }
 
         this.queryId = queryId;
-        this.$table = $("#preview");
         this.$rows = $("#rows");
         this.$form = $("form");
         this.$snapshotField = $("#id_snapshot");
         this.docChanged = false;
 
         this.$submit = $("#refresh_play_button, #save_button");
         if (!this.$submit.length) {
```

### Comparing `django_sql_explorer-4.1b5/explorer/src/js/favorites.js` & `django_sql_explorer-4.1b6/explorer/src/js/favorites.js`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b5/explorer/src/js/main.js` & `django_sql_explorer-4.1b6/explorer/src/js/main.js`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b5/explorer/src/js/pivot-setup.js` & `django_sql_explorer-4.1b6/explorer/src/js/pivot-setup.js`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b5/explorer/src/js/pivot.js` & `django_sql_explorer-4.1b6/explorer/src/js/pivot.js`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b5/explorer/src/js/query-list.js` & `django_sql_explorer-4.1b6/explorer/src/js/query-list.js`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b5/explorer/src/js/schema.js` & `django_sql_explorer-4.1b6/explorer/src/js/schema.js`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b5/explorer/src/js/table-to-csv.js` & `django_sql_explorer-4.1b6/explorer/src/js/table-to-csv.js`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b5/explorer/src/scss/assistant.scss` & `django_sql_explorer-4.1b6/explorer/src/scss/assistant.scss`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b5/explorer/src/scss/explorer.scss` & `django_sql_explorer-4.1b6/explorer/src/scss/explorer.scss`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b5/explorer/src/scss/pivot.css` & `django_sql_explorer-4.1b6/explorer/src/scss/pivot.css`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b5/explorer/static/explorer/bootstrap-icons.woff` & `django_sql_explorer-4.1b6/explorer/static/explorer/bootstrap-icons.woff`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b5/explorer/static/explorer/bootstrap-icons.woff2` & `django_sql_explorer-4.1b6/explorer/static/explorer/bootstrap-icons.woff2`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b5/explorer/static/explorer/explorer.js` & `django_sql_explorer-4.1b6/explorer/static/explorer/explorer.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -1,49 +1,49 @@
-var Um = Object.defineProperty,
-    Qm = Object.defineProperties;
-var Gm = Object.getOwnPropertyDescriptors;
+var Qm = Object.defineProperty,
+    Gm = Object.defineProperties;
+var Km = Object.getOwnPropertyDescriptors;
 var Ic = Object.getOwnPropertySymbols;
-var Km = Object.prototype.hasOwnProperty,
-    Xm = Object.prototype.propertyIsEnumerable;
-var Xl = (n, e, t) => e in n ? Um(n, e, {
+var Xm = Object.prototype.hasOwnProperty,
+    Ym = Object.prototype.propertyIsEnumerable;
+var Xl = (n, e, t) => e in n ? Qm(n, e, {
         enumerable: !0,
         configurable: !0,
         writable: !0,
         value: t
     }) : n[e] = t,
     It = (n, e) => {
-        for (var t in e || (e = {})) Km.call(e, t) && Xl(n, t, e[t]);
+        for (var t in e || (e = {})) Xm.call(e, t) && Xl(n, t, e[t]);
         if (Ic)
-            for (var t of Ic(e)) Xm.call(e, t) && Xl(n, t, e[t]);
+            for (var t of Ic(e)) Ym.call(e, t) && Xl(n, t, e[t]);
         return n
     },
-    lr = (n, e) => Qm(n, Gm(e));
+    lr = (n, e) => Gm(n, Km(e));
 var ze = (n, e, t) => (Xl(n, typeof e != "symbol" ? e + "" : e, t), t),
-    Ym = (n, e, t) => {
+    Jm = (n, e, t) => {
         if (!e.has(n)) throw TypeError("Cannot " + t)
     };
 var Yl = (n, e, t) => {
     if (e.has(n)) throw TypeError("Cannot add the same private member more than once");
     e instanceof WeakSet ? e.add(n) : e.set(n, t)
 };
-var Js = (n, e, t) => (Ym(n, e, "access private method"), t);
+var Js = (n, e, t) => (Jm(n, e, "access private method"), t);
 import {
-    C as Jm,
-    T as Zm,
-    _ as e0
+    C as Zm,
+    T as e0,
+    _ as t0
 } from "./main.js";
 import {
-    c as t0,
-    g as i0,
+    c as i0,
+    g as n0,
     L as Vu
 } from "./index.js";
 import {
     g as Uu,
     c as Jl,
-    t as n0
+    t as r0
 } from "./favorites.js";
 var Qu = {
     exports: {}
 };
 /*!
  * jQuery JavaScript Library v3.7.1
  * https://jquery.com/
@@ -56,32 +56,32 @@
  */
 (function(n) {
     (function(e, t) {
         n.exports = e.document ? t(e, !0) : function(i) {
             if (!i.document) throw new Error("jQuery requires a window with a document");
             return t(i)
         }
-    })(typeof window != "undefined" ? window : t0, function(e, t) {
+    })(typeof window != "undefined" ? window : i0, function(e, t) {
         var i = [],
             r = Object.getPrototypeOf,
             s = i.slice,
             o = i.flat ? function(a) {
                 return i.flat.call(a)
             } : function(a) {
                 return i.concat.apply([], a)
             },
             l = i.push,
             h = i.indexOf,
             f = {},
             u = f.toString,
-            g = f.hasOwnProperty,
-            y = g.toString,
+            m = f.hasOwnProperty,
+            y = m.toString,
             k = y.call(Object),
             v = {},
-            C = function(c) {
+            A = function(c) {
                 return typeof c == "function" && typeof c.nodeType != "number" && typeof c.item != "function"
             },
             O = function(c) {
                 return c != null && c === c.window
             },
             D = e.document,
             F = {
@@ -89,17 +89,17 @@
                 src: !0,
                 nonce: !0,
                 noModule: !0
             };
 
         function $(a, c, d) {
             d = d || D;
-            var m, b, x = d.createElement("script");
+            var g, b, x = d.createElement("script");
             if (x.text = a, c)
-                for (m in F) b = c[m] || c.getAttribute && c.getAttribute(m), b && x.setAttribute(m, b);
+                for (g in F) b = c[g] || c.getAttribute && c.getAttribute(g), b && x.setAttribute(g, b);
             d.head.appendChild(x).parentNode.removeChild(x)
         }
 
         function j(a) {
             return a == null ? a + "" : typeof a == "object" || typeof a == "function" ? f[u.call(a)] || "object" : typeof a
         }
         var z = "3.7.1",
@@ -156,58 +156,58 @@
             end: function() {
                 return this.prevObject || this.constructor()
             },
             push: l,
             sort: i.sort,
             splice: i.splice
         }, p.extend = p.fn.extend = function() {
-            var a, c, d, m, b, x, w = arguments[0] || {},
+            var a, c, d, g, b, x, w = arguments[0] || {},
                 T = 1,
-                A = arguments.length,
+                C = arguments.length,
                 E = !1;
-            for (typeof w == "boolean" && (E = w, w = arguments[T] || {}, T++), typeof w != "object" && !C(w) && (w = {}), T === A && (w = this, T--); T < A; T++)
+            for (typeof w == "boolean" && (E = w, w = arguments[T] || {}, T++), typeof w != "object" && !A(w) && (w = {}), T === C && (w = this, T--); T < C; T++)
                 if ((a = arguments[T]) != null)
-                    for (c in a) m = a[c], !(c === "__proto__" || w === m) && (E && m && (p.isPlainObject(m) || (b = Array.isArray(m))) ? (d = w[c], b && !Array.isArray(d) ? x = [] : !b && !p.isPlainObject(d) ? x = {} : x = d, b = !1, w[c] = p.extend(E, x, m)) : m !== void 0 && (w[c] = m));
+                    for (c in a) g = a[c], !(c === "__proto__" || w === g) && (E && g && (p.isPlainObject(g) || (b = Array.isArray(g))) ? (d = w[c], b && !Array.isArray(d) ? x = [] : !b && !p.isPlainObject(d) ? x = {} : x = d, b = !1, w[c] = p.extend(E, x, g)) : g !== void 0 && (w[c] = g));
             return w
         }, p.extend({
             expando: "jQuery" + (z + Math.random()).replace(/\D/g, ""),
             isReady: !0,
             error: function(a) {
                 throw new Error(a)
             },
             noop: function() {},
             isPlainObject: function(a) {
                 var c, d;
-                return !a || u.call(a) !== "[object Object]" ? !1 : (c = r(a), c ? (d = g.call(c, "constructor") && c.constructor, typeof d == "function" && y.call(d) === k) : !0)
+                return !a || u.call(a) !== "[object Object]" ? !1 : (c = r(a), c ? (d = m.call(c, "constructor") && c.constructor, typeof d == "function" && y.call(d) === k) : !0)
             },
             isEmptyObject: function(a) {
                 var c;
                 for (c in a) return !1;
                 return !0
             },
             globalEval: function(a, c, d) {
                 $(a, {
                     nonce: c && c.nonce
                 }, d)
             },
             each: function(a, c) {
-                var d, m = 0;
+                var d, g = 0;
                 if (he(a))
-                    for (d = a.length; m < d && c.call(a[m], m, a[m]) !== !1; m++);
+                    for (d = a.length; g < d && c.call(a[g], g, a[g]) !== !1; g++);
                 else
-                    for (m in a)
-                        if (c.call(a[m], m, a[m]) === !1) break;
+                    for (g in a)
+                        if (c.call(a[g], g, a[g]) === !1) break;
                 return a
             },
             text: function(a) {
                 var c, d = "",
-                    m = 0,
+                    g = 0,
                     b = a.nodeType;
                 if (!b)
-                    for (; c = a[m++];) d += p.text(c);
+                    for (; c = a[g++];) d += p.text(c);
                 return b === 1 || b === 11 ? a.textContent : b === 9 ? a.documentElement.textContent : b === 3 || b === 4 ? a.nodeValue : d
             },
             makeArray: function(a, c) {
                 var d = c || [];
                 return a != null && (he(Object(a)) ? p.merge(d, typeof a == "string" ? [a] : a) : l.call(d, a)), d
             },
             inArray: function(a, c, d) {
@@ -215,40 +215,40 @@
             },
             isXMLDoc: function(a) {
                 var c = a && a.namespaceURI,
                     d = a && (a.ownerDocument || a).documentElement;
                 return !G.test(c || d && d.nodeName || "HTML")
             },
             merge: function(a, c) {
-                for (var d = +c.length, m = 0, b = a.length; m < d; m++) a[b++] = c[m];
+                for (var d = +c.length, g = 0, b = a.length; g < d; g++) a[b++] = c[g];
                 return a.length = b, a
             },
             grep: function(a, c, d) {
-                for (var m, b = [], x = 0, w = a.length, T = !d; x < w; x++) m = !c(a[x], x), m !== T && b.push(a[x]);
+                for (var g, b = [], x = 0, w = a.length, T = !d; x < w; x++) g = !c(a[x], x), g !== T && b.push(a[x]);
                 return b
             },
             map: function(a, c, d) {
-                var m, b, x = 0,
+                var g, b, x = 0,
                     w = [];
                 if (he(a))
-                    for (m = a.length; x < m; x++) b = c(a[x], x, d), b != null && w.push(b);
+                    for (g = a.length; x < g; x++) b = c(a[x], x, d), b != null && w.push(b);
                 else
                     for (x in a) b = c(a[x], x, d), b != null && w.push(b);
                 return o(w)
             },
             guid: 1,
             support: v
         }), typeof Symbol == "function" && (p.fn[Symbol.iterator] = i[Symbol.iterator]), p.each("Boolean Number String Function Array Date RegExp Object Error Symbol".split(" "), function(a, c) {
             f["[object " + c + "]"] = c.toLowerCase()
         });
 
         function he(a) {
             var c = !!a && "length" in a && a.length,
                 d = j(a);
-            return C(a) || O(a) ? !1 : d === "array" || c === 0 || typeof c == "number" && c > 0 && c - 1 in a
+            return A(a) || O(a) ? !1 : d === "array" || c === 0 || typeof c == "number" && c > 0 && c - 1 in a
         }
 
         function J(a, c) {
             return a.nodeName && a.nodeName.toLowerCase() === c.toLowerCase()
         }
         var ae = i.pop,
             pe = i.sort,
@@ -266,20 +266,20 @@
         }
         p.escapeSelector = function(a) {
             return (a + "").replace(Be, st)
         };
         var _e = D,
             Ye = l;
         (function() {
-            var a, c, d, m, b, x = Ye,
-                w, T, A, E, I, _ = p.expando,
+            var a, c, d, g, b, x = Ye,
+                w, T, C, E, I, _ = p.expando,
                 P = 0,
                 W = 0,
                 ce = Gs(),
-                Te = Gs(),
+                Ae = Gs(),
                 ge = Gs(),
                 ut = Gs(),
                 et = function(S, M) {
                     return S === M && (b = !0), 0
                 },
                 wi = "checked|selected|async|autofocus|autoplay|controls|defer|disabled|hidden|ismap|loop|multiple|open|readonly|required|scoped",
                 vi = "(?:\\\\[\\da-fA-F]{1,6}" + ie + "?|\\\\[^\\r\\n\\f]|[\\w-]|[^\0-\\x7f])+",
@@ -306,25 +306,25 @@
                 Zt = /^(?:#([\w-]+)|(\w+)|\.([\w-]+))$/,
                 jl = /[+~]/,
                 qi = new RegExp("\\\\[\\da-fA-F]{1,6}" + ie + "?|\\\\([^\\r\\n\\f])", "g"),
                 ji = function(S, M) {
                     var L = "0x" + S.slice(1) - 65536;
                     return M || (L < 0 ? String.fromCharCode(L + 65536) : String.fromCharCode(L >> 10 | 55296, L & 1023 | 56320))
                 },
-                Fm = function() {
+                zm = function() {
                     an()
                 },
-                zm = Xs(function(S) {
+                $m = Xs(function(S) {
                     return S.disabled === !0 && J(S, "fieldset")
                 }, {
                     dir: "parentNode",
                     next: "legend"
                 });
 
-            function $m() {
+            function Wm() {
                 try {
                     return w.activeElement
                 } catch (S) {}
             }
             try {
                 x.apply(i = s.call(_e.childNodes), _e.childNodes), i[_e.childNodes.length].nodeType
             } catch (S) {
@@ -338,15 +338,15 @@
                 }
             }
 
             function Le(S, M, L, N) {
                 var B, U, K, re, X, xe, le, ue = M && M.ownerDocument,
                     ke = M ? M.nodeType : 9;
                 if (L = L || [], typeof S != "string" || !S || ke !== 1 && ke !== 9 && ke !== 11) return L;
-                if (!N && (an(M), M = M || w, A)) {
+                if (!N && (an(M), M = M || w, C)) {
                     if (ke !== 11 && (X = Zt.exec(S)))
                         if (B = X[1]) {
                             if (ke === 9)
                                 if (K = M.getElementById(B)) {
                                     if (K.id === B) return x.call(L, K), L
                                 } else return L;
                             else if (ue && (K = ue.getElementById(B)) && Le.contains(M, K) && K.id === B) return x.call(L, K), L
@@ -390,29 +390,29 @@
                 } catch (L) {
                     return !1
                 } finally {
                     M.parentNode && M.parentNode.removeChild(M), M = null
                 }
             }
 
-            function Wm(S) {
+            function qm(S) {
                 return function(M) {
                     return J(M, "input") && M.type === S
                 }
             }
 
-            function qm(S) {
+            function jm(S) {
                 return function(M) {
                     return (J(M, "input") || J(M, "button")) && M.type === S
                 }
             }
 
             function Lc(S) {
                 return function(M) {
-                    return "form" in M ? M.parentNode && M.disabled === !1 ? "label" in M ? "label" in M.parentNode ? M.parentNode.disabled === S : M.disabled === S : M.isDisabled === S || M.isDisabled !== !S && zm(M) === S : M.disabled === S : "label" in M ? M.disabled === S : !1
+                    return "form" in M ? M.parentNode && M.disabled === !1 ? "label" in M ? "label" in M.parentNode ? M.parentNode.disabled === S : M.disabled === S : M.isDisabled === S || M.isDisabled !== !S && $m(M) === S : M.disabled === S : "label" in M ? M.disabled === S : !1
                 }
             }
 
             function In(S) {
                 return fi(function(M) {
                     return M = +M, fi(function(L, N) {
                         for (var B, U = S([], L.length, M), K = U.length; K--;) L[B = U[K]] && (L[B] = !(N[B] = L[B]))
@@ -422,15 +422,15 @@
 
             function Vl(S) {
                 return S && typeof S.getElementsByTagName != "undefined" && S
             }
 
             function an(S) {
                 var M, L = S ? S.ownerDocument || S : _e;
-                return L == w || L.nodeType !== 9 || !L.documentElement || (w = L, T = w.documentElement, A = !p.isXMLDoc(w), I = T.matches || T.webkitMatchesSelector || T.msMatchesSelector, T.msMatchesSelector && _e != w && (M = w.defaultView) && M.top !== M && M.addEventListener("unload", Fm), v.getById = sr(function(N) {
+                return L == w || L.nodeType !== 9 || !L.documentElement || (w = L, T = w.documentElement, C = !p.isXMLDoc(w), I = T.matches || T.webkitMatchesSelector || T.msMatchesSelector, T.msMatchesSelector && _e != w && (M = w.defaultView) && M.top !== M && M.addEventListener("unload", zm), v.getById = sr(function(N) {
                     return T.appendChild(N).id = p.expando, !w.getElementsByName || !w.getElementsByName(p.expando).length
                 }), v.disconnectedMatch = sr(function(N) {
                     return I.call(N, "*")
                 }), v.scope = sr(function() {
                     return w.querySelectorAll(":scope")
                 }), v.cssHas = sr(function() {
                     try {
@@ -440,75 +440,75 @@
                     }
                 }), v.getById ? (c.filter.ID = function(N) {
                     var B = N.replace(qi, ji);
                     return function(U) {
                         return U.getAttribute("id") === B
                     }
                 }, c.find.ID = function(N, B) {
-                    if (typeof B.getElementById != "undefined" && A) {
+                    if (typeof B.getElementById != "undefined" && C) {
                         var U = B.getElementById(N);
                         return U ? [U] : []
                     }
                 }) : (c.filter.ID = function(N) {
                     var B = N.replace(qi, ji);
                     return function(U) {
                         var K = typeof U.getAttributeNode != "undefined" && U.getAttributeNode("id");
                         return K && K.value === B
                     }
                 }, c.find.ID = function(N, B) {
-                    if (typeof B.getElementById != "undefined" && A) {
+                    if (typeof B.getElementById != "undefined" && C) {
                         var U, K, re, X = B.getElementById(N);
                         if (X) {
                             if (U = X.getAttributeNode("id"), U && U.value === N) return [X];
                             for (re = B.getElementsByName(N), K = 0; X = re[K++];)
                                 if (U = X.getAttributeNode("id"), U && U.value === N) return [X]
                         }
                         return []
                     }
                 }), c.find.TAG = function(N, B) {
                     return typeof B.getElementsByTagName != "undefined" ? B.getElementsByTagName(N) : B.querySelectorAll(N)
                 }, c.find.CLASS = function(N, B) {
-                    if (typeof B.getElementsByClassName != "undefined" && A) return B.getElementsByClassName(N)
+                    if (typeof B.getElementsByClassName != "undefined" && C) return B.getElementsByClassName(N)
                 }, E = [], sr(function(N) {
                     var B;
                     T.appendChild(N).innerHTML = "<a id='" + _ + "' href='' disabled='disabled'></a><select id='" + _ + "-\r\\' disabled='disabled'><option selected=''></option></select>", N.querySelectorAll("[selected]").length || E.push("\\[" + ie + "*(?:value|" + wi + ")"), N.querySelectorAll("[id~=" + _ + "-]").length || E.push("~="), N.querySelectorAll("a#" + _ + "+*").length || E.push(".#.+[+~]"), N.querySelectorAll(":checked").length || E.push(":checked"), B = w.createElement("input"), B.setAttribute("type", "hidden"), N.appendChild(B).setAttribute("name", "D"), T.appendChild(N).disabled = !0, N.querySelectorAll(":disabled").length !== 2 && E.push(":enabled", ":disabled"), B = w.createElement("input"), B.setAttribute("name", ""), N.appendChild(B), N.querySelectorAll("[name='']").length || E.push("\\[" + ie + "*name" + ie + "*=" + ie + `*(?:''|"")`)
                 }), v.cssHas || E.push(":has"), E = E.length && new RegExp(E.join("|")), et = function(N, B) {
                     if (N === B) return b = !0, 0;
                     var U = !N.compareDocumentPosition - !B.compareDocumentPosition;
-                    return U || (U = (N.ownerDocument || N) == (B.ownerDocument || B) ? N.compareDocumentPosition(B) : 1, U & 1 || !v.sortDetached && B.compareDocumentPosition(N) === U ? N === w || N.ownerDocument == _e && Le.contains(_e, N) ? -1 : B === w || B.ownerDocument == _e && Le.contains(_e, B) ? 1 : m ? h.call(m, N) - h.call(m, B) : 0 : U & 4 ? -1 : 1)
+                    return U || (U = (N.ownerDocument || N) == (B.ownerDocument || B) ? N.compareDocumentPosition(B) : 1, U & 1 || !v.sortDetached && B.compareDocumentPosition(N) === U ? N === w || N.ownerDocument == _e && Le.contains(_e, N) ? -1 : B === w || B.ownerDocument == _e && Le.contains(_e, B) ? 1 : g ? h.call(g, N) - h.call(g, B) : 0 : U & 4 ? -1 : 1)
                 }), w
             }
             Le.matches = function(S, M) {
                 return Le(S, null, null, M)
             }, Le.matchesSelector = function(S, M) {
-                if (an(S), A && !ut[M + " "] && (!E || !E.test(M))) try {
+                if (an(S), C && !ut[M + " "] && (!E || !E.test(M))) try {
                     var L = I.call(S, M);
                     if (L || v.disconnectedMatch || S.document && S.document.nodeType !== 11) return L
                 } catch (N) {
                     ut(M, !0)
                 }
                 return Le(M, w, null, [S]).length > 0
             }, Le.contains = function(S, M) {
                 return (S.ownerDocument || S) != w && an(S), p.contains(S, M)
             }, Le.attr = function(S, M) {
                 (S.ownerDocument || S) != w && an(S);
                 var L = c.attrHandle[M.toLowerCase()],
-                    N = L && g.call(c.attrHandle, M.toLowerCase()) ? L(S, M, !A) : void 0;
+                    N = L && m.call(c.attrHandle, M.toLowerCase()) ? L(S, M, !C) : void 0;
                 return N !== void 0 ? N : S.getAttribute(M)
             }, Le.error = function(S) {
                 throw new Error("Syntax error, unrecognized expression: " + S)
             }, p.uniqueSort = function(S) {
                 var M, L = [],
                     N = 0,
                     B = 0;
-                if (b = !v.sortStable, m = !v.sortStable && s.call(S, 0), pe.call(S, et), b) {
+                if (b = !v.sortStable, g = !v.sortStable && s.call(S, 0), pe.call(S, et), b) {
                     for (; M = S[B++];) M === S[B] && (N = L.push(B));
                     for (; N--;) fe.call(S, L[N], 1)
                 }
-                return m = null, S
+                return g = null, S
             }, p.fn.uniqueSort = function() {
                 return this.pushStack(p.uniqueSort(s.apply(this)))
             }, c = p.expr = {
                 cacheLength: 50,
                 createPseudo: fi,
                 match: Ci,
                 attrHandle: {},
@@ -628,27 +628,27 @@
                             }
                     }),
                     lang: fi(function(S) {
                         return zr.test(S || "") || Le.error("unsupported lang: " + S), S = S.replace(qi, ji).toLowerCase(),
                             function(M) {
                                 var L;
                                 do
-                                    if (L = A ? M.lang : M.getAttribute("xml:lang") || M.getAttribute("lang")) return L = L.toLowerCase(), L === S || L.indexOf(S + "-") === 0; while ((M = M.parentNode) && M.nodeType === 1);
+                                    if (L = C ? M.lang : M.getAttribute("xml:lang") || M.getAttribute("lang")) return L = L.toLowerCase(), L === S || L.indexOf(S + "-") === 0; while ((M = M.parentNode) && M.nodeType === 1);
                                 return !1
                             }
                     }),
                     target: function(S) {
                         var M = e.location && e.location.hash;
                         return M && M.slice(1) === S.id
                     },
                     root: function(S) {
                         return S === T
                     },
                     focus: function(S) {
-                        return S === $m() && w.hasFocus() && !!(S.type || S.href || ~S.tabIndex)
+                        return S === Wm() && w.hasFocus() && !!(S.type || S.href || ~S.tabIndex)
                     },
                     enabled: Lc(!1),
                     disabled: Lc(!0),
                     checked: function(S) {
                         return J(S, "input") && !!S.checked || J(S, "option") && !!S.selected
                     },
                     selected: function(S) {
@@ -705,39 +705,39 @@
             }, c.pseudos.nth = c.pseudos.eq;
             for (a in {
                     radio: !0,
                     checkbox: !0,
                     file: !0,
                     password: !0,
                     image: !0
-                }) c.pseudos[a] = Wm(a);
+                }) c.pseudos[a] = qm(a);
             for (a in {
                     submit: !0,
                     reset: !0
-                }) c.pseudos[a] = qm(a);
+                }) c.pseudos[a] = jm(a);
 
             function Pc() {}
             Pc.prototype = c.filters = c.pseudos, c.setFilters = new Pc;
 
             function $r(S, M) {
-                var L, N, B, U, K, re, X, xe = Te[S + " "];
+                var L, N, B, U, K, re, X, xe = Ae[S + " "];
                 if (xe) return M ? 0 : xe.slice(0);
                 for (K = S, re = [], X = c.preFilter; K;) {
                     (!L || (N = Qe.exec(K))) && (N && (K = K.slice(N[0].length) || K), re.push(B = [])), L = !1, (N = Fr.exec(K)) && (L = N.shift(), B.push({
                         value: L,
                         type: N[0].replace(ye, " ")
                     }), K = K.slice(L.length));
                     for (U in c.filter)(N = Ci[U].exec(K)) && (!X[U] || (N = X[U](N))) && (L = N.shift(), B.push({
                         value: L,
                         type: U,
                         matches: N
                     }), K = K.slice(L.length));
                     if (!L) break
                 }
-                return M ? K.length : K ? Le.error(S) : Te(S, re).slice(0)
+                return M ? K.length : K ? Le.error(S) : Ae(S, re).slice(0)
             }
 
             function Ks(S) {
                 for (var M = 0, L = S.length, N = ""; M < L; M++) N += S[M].value;
                 return N
             }
 
@@ -771,30 +771,30 @@
                 return S.length > 1 ? function(M, L, N) {
                     for (var B = S.length; B--;)
                         if (!S[B](M, L, N)) return !1;
                     return !0
                 } : S[0]
             }
 
-            function jm(S, M, L) {
+            function Vm(S, M, L) {
                 for (var N = 0, B = M.length; N < B; N++) Le(S, M[N], L);
                 return L
             }
 
             function Ys(S, M, L, N, B) {
                 for (var U, K = [], re = 0, X = S.length, xe = M != null; re < X; re++)(U = S[re]) && (!L || L(U, N, B)) && (K.push(U), xe && M.push(re));
                 return K
             }
 
             function Ql(S, M, L, N, B, U) {
                 return N && !N[_] && (N = Ql(N)), B && !B[_] && (B = Ql(B, U)), fi(function(K, re, X, xe) {
                     var le, ue, ke, oe, Fe = [],
                         Nt = [],
                         wt = re.length,
-                        ei = K || jm(M || "*", X.nodeType ? [X] : X, []),
+                        ei = K || Vm(M || "*", X.nodeType ? [X] : X, []),
                         Ai = S && (K || !M) ? Ys(ei, Fe, S, X, xe) : ei;
                     if (L ? (oe = B || (K ? S : wt || N) ? [] : re, L(Ai, oe, X, xe)) : oe = Ai, N)
                         for (le = Ys(oe, Nt), N(le, [], X, xe), ue = le.length; ue--;)(ke = le[ue]) && (oe[Nt[ue]] = !(Ai[Nt[ue]] = ke));
                     if (K) {
                         if (B || S) {
                             if (B) {
                                 for (le = [], ue = oe.length; ue--;)(ke = oe[ue]) && le.push(Ai[ue] = ke);
@@ -823,29 +823,29 @@
                                 value: S[re - 2].type === " " ? "*" : ""
                             })).replace(ye, "$1"), L, re < N && Gl(S.slice(re, N)), N < B && Gl(S = S.slice(N)), N < B && Ks(S))
                         }
                         le.push(L)
                     } return Ul(le)
             }
 
-            function Vm(S, M) {
+            function Um(S, M) {
                 var L = M.length > 0,
                     N = S.length > 0,
                     B = function(U, K, re, X, xe) {
                         var le, ue, ke, oe = 0,
                             Fe = "0",
                             Nt = U && [],
                             wt = [],
                             ei = d,
                             Ai = U || N && c.find.TAG("*", xe),
                             or = P += ei == null ? 1 : Math.random() || .1,
                             Mt = Ai.length;
                         for (xe && (d = K == w || K || xe); Fe !== Mt && (le = Ai[Fe]) != null; Fe++) {
                             if (N && le) {
-                                for (ue = 0, !K && le.ownerDocument != w && (an(le), re = !A); ke = S[ue++];)
+                                for (ue = 0, !K && le.ownerDocument != w && (an(le), re = !C); ke = S[ue++];)
                                     if (ke(le, K || w, re)) {
                                         x.call(X, le);
                                         break
                                     } xe && (P = or)
                             }
                             L && ((le = !ke && le) && oe--, U && Nt.push(le))
                         }
@@ -865,105 +865,105 @@
 
             function Kl(S, M) {
                 var L, N = [],
                     B = [],
                     U = ge[S + " "];
                 if (!U) {
                     for (M || (M = $r(S)), L = M.length; L--;) U = Gl(M[L]), U[_] ? N.push(U) : B.push(U);
-                    U = ge(S, Vm(B, N)), U.selector = S
+                    U = ge(S, Um(B, N)), U.selector = S
                 }
                 return U
             }
 
             function Nc(S, M, L, N) {
                 var B, U, K, re, X, xe = typeof S == "function" && S,
                     le = !N && $r(S = xe.selector || S);
                 if (L = L || [], le.length === 1) {
-                    if (U = le[0] = le[0].slice(0), U.length > 2 && (K = U[0]).type === "ID" && M.nodeType === 9 && A && c.relative[U[1].type]) {
+                    if (U = le[0] = le[0].slice(0), U.length > 2 && (K = U[0]).type === "ID" && M.nodeType === 9 && C && c.relative[U[1].type]) {
                         if (M = (c.find.ID(K.matches[0].replace(qi, ji), M) || [])[0], M) xe && (M = M.parentNode);
                         else return L;
                         S = S.slice(U.shift().value.length)
                     }
                     for (B = Ci.needsContext.test(S) ? 0 : U.length; B-- && (K = U[B], !c.relative[re = K.type]);)
                         if ((X = c.find[re]) && (N = X(K.matches[0].replace(qi, ji), jl.test(U[0].type) && Vl(M.parentNode) || M))) {
                             if (U.splice(B, 1), S = N.length && Ks(U), !S) return x.apply(L, N), L;
                             break
                         }
                 }
-                return (xe || Kl(S, le))(N, M, !A, L, !M || jl.test(S) && Vl(M.parentNode) || M), L
+                return (xe || Kl(S, le))(N, M, !C, L, !M || jl.test(S) && Vl(M.parentNode) || M), L
             }
             v.sortStable = _.split("").sort(et).join("") === _, an(), v.sortDetached = sr(function(S) {
                 return S.compareDocumentPosition(w.createElement("fieldset")) & 1
             }), p.find = Le, p.expr[":"] = p.expr.pseudos, p.unique = p.uniqueSort, Le.compile = Kl, Le.select = Nc, Le.setDocument = an, Le.tokenize = $r, Le.escape = p.escapeSelector, Le.getText = p.text, Le.isXML = p.isXMLDoc, Le.selectors = p.expr, Le.support = p.support, Le.uniqueSort = p.uniqueSort
         })();
         var be = function(a, c, d) {
-                for (var m = [], b = d !== void 0;
+                for (var g = [], b = d !== void 0;
                     (a = a[c]) && a.nodeType !== 9;)
                     if (a.nodeType === 1) {
                         if (b && p(a).is(d)) break;
-                        m.push(a)
-                    } return m
+                        g.push(a)
+                    } return g
             },
             We = function(a, c) {
                 for (var d = []; a; a = a.nextSibling) a.nodeType === 1 && a !== c && d.push(a);
                 return d
             },
-            Ae = p.expr.match.needsContext,
+            Ce = p.expr.match.needsContext,
             bt = /^<([a-z][^\/\0>:\x20\t\r\n\f]*)[\x20\t\r\n\f]*\/?>(?:<\/\1>|)$/i;
 
         function Oe(a, c, d) {
-            return C(c) ? p.grep(a, function(m, b) {
-                return !!c.call(m, b, m) !== d
-            }) : c.nodeType ? p.grep(a, function(m) {
-                return m === c !== d
-            }) : typeof c != "string" ? p.grep(a, function(m) {
-                return h.call(c, m) > -1 !== d
+            return A(c) ? p.grep(a, function(g, b) {
+                return !!c.call(g, b, g) !== d
+            }) : c.nodeType ? p.grep(a, function(g) {
+                return g === c !== d
+            }) : typeof c != "string" ? p.grep(a, function(g) {
+                return h.call(c, g) > -1 !== d
             }) : p.filter(c, a, d)
         }
         p.filter = function(a, c, d) {
-            var m = c[0];
-            return d && (a = ":not(" + a + ")"), c.length === 1 && m.nodeType === 1 ? p.find.matchesSelector(m, a) ? [m] : [] : p.find.matches(a, p.grep(c, function(b) {
+            var g = c[0];
+            return d && (a = ":not(" + a + ")"), c.length === 1 && g.nodeType === 1 ? p.find.matchesSelector(g, a) ? [g] : [] : p.find.matches(a, p.grep(c, function(b) {
                 return b.nodeType === 1
             }))
         }, p.fn.extend({
             find: function(a) {
-                var c, d, m = this.length,
+                var c, d, g = this.length,
                     b = this;
                 if (typeof a != "string") return this.pushStack(p(a).filter(function() {
-                    for (c = 0; c < m; c++)
+                    for (c = 0; c < g; c++)
                         if (p.contains(b[c], this)) return !0
                 }));
-                for (d = this.pushStack([]), c = 0; c < m; c++) p.find(a, b[c], d);
-                return m > 1 ? p.uniqueSort(d) : d
+                for (d = this.pushStack([]), c = 0; c < g; c++) p.find(a, b[c], d);
+                return g > 1 ? p.uniqueSort(d) : d
             },
             filter: function(a) {
                 return this.pushStack(Oe(this, a || [], !1))
             },
             not: function(a) {
                 return this.pushStack(Oe(this, a || [], !0))
             },
             is: function(a) {
-                return !!Oe(this, typeof a == "string" && Ae.test(a) ? p(a) : a || [], !1).length
+                return !!Oe(this, typeof a == "string" && Ce.test(a) ? p(a) : a || [], !1).length
             }
         });
         var Tt, yi = /^(?:\s*(<[\w\W]+>)[^>]*|#([\w-]+))$/,
             On = p.fn.init = function(a, c, d) {
-                var m, b;
+                var g, b;
                 if (!a) return this;
                 if (d = d || Tt, typeof a == "string")
-                    if (a[0] === "<" && a[a.length - 1] === ">" && a.length >= 3 ? m = [null, a, null] : m = yi.exec(a), m && (m[1] || !c))
-                        if (m[1]) {
-                            if (c = c instanceof p ? c[0] : c, p.merge(this, p.parseHTML(m[1], c && c.nodeType ? c.ownerDocument || c : D, !0)), bt.test(m[1]) && p.isPlainObject(c))
-                                for (m in c) C(this[m]) ? this[m](c[m]) : this.attr(m, c[m]);
+                    if (a[0] === "<" && a[a.length - 1] === ">" && a.length >= 3 ? g = [null, a, null] : g = yi.exec(a), g && (g[1] || !c))
+                        if (g[1]) {
+                            if (c = c instanceof p ? c[0] : c, p.merge(this, p.parseHTML(g[1], c && c.nodeType ? c.ownerDocument || c : D, !0)), bt.test(g[1]) && p.isPlainObject(c))
+                                for (g in c) A(this[g]) ? this[g](c[g]) : this.attr(g, c[g]);
                             return this
-                        } else return b = D.getElementById(m[2]), b && (this[0] = b, this.length = 1), this;
+                        } else return b = D.getElementById(g[2]), b && (this[0] = b, this.length = 1), this;
                 else return !c || c.jquery ? (c || d).find(a) : this.constructor(c).find(a);
                 else {
                     if (a.nodeType) return this[0] = a, this.length = 1, this;
-                    if (C(a)) return d.ready !== void 0 ? d.ready(a) : a(p)
+                    if (A(a)) return d.ready !== void 0 ? d.ready(a) : a(p)
                 }
                 return p.makeArray(a, this)
             };
         On.prototype = p.fn, Tt = p(D);
         var Mr = /^(?:parents|prev(?:Until|All))/,
             Bs = {
                 children: !0,
@@ -972,26 +972,26 @@
                 prev: !0
             };
         p.fn.extend({
             has: function(a) {
                 var c = p(a, this),
                     d = c.length;
                 return this.filter(function() {
-                    for (var m = 0; m < d; m++)
-                        if (p.contains(this, c[m])) return !0
+                    for (var g = 0; g < d; g++)
+                        if (p.contains(this, c[g])) return !0
                 })
             },
             closest: function(a, c) {
-                var d, m = 0,
+                var d, g = 0,
                     b = this.length,
                     x = [],
                     w = typeof a != "string" && p(a);
-                if (!Ae.test(a)) {
-                    for (; m < b; m++)
-                        for (d = this[m]; d && d !== c; d = d.parentNode)
+                if (!Ce.test(a)) {
+                    for (; g < b; g++)
+                        for (d = this[g]; d && d !== c; d = d.parentNode)
                             if (d.nodeType < 11 && (w ? w.index(d) > -1 : d.nodeType === 1 && p.find.matchesSelector(d, a))) {
                                 x.push(d);
                                 break
                             }
                 }
                 return this.pushStack(x.length > 1 ? p.uniqueSort(x) : x)
             },
@@ -1046,44 +1046,44 @@
             children: function(a) {
                 return We(a.firstChild)
             },
             contents: function(a) {
                 return a.contentDocument != null && r(a.contentDocument) ? a.contentDocument : (J(a, "template") && (a = a.content || a), p.merge([], a.childNodes))
             }
         }, function(a, c) {
-            p.fn[a] = function(d, m) {
+            p.fn[a] = function(d, g) {
                 var b = p.map(this, c, d);
-                return a.slice(-5) !== "Until" && (m = d), m && typeof m == "string" && (b = p.filter(m, b)), this.length > 1 && (Bs[a] || p.uniqueSort(b), Mr.test(a) && b.reverse()), this.pushStack(b)
+                return a.slice(-5) !== "Until" && (g = d), g && typeof g == "string" && (b = p.filter(g, b)), this.length > 1 && (Bs[a] || p.uniqueSort(b), Mr.test(a) && b.reverse()), this.pushStack(b)
             }
         });
         var at = /[^\x20\t\r\n\f]+/g;
 
         function zi(a) {
             var c = {};
-            return p.each(a.match(at) || [], function(d, m) {
-                c[m] = !0
+            return p.each(a.match(at) || [], function(d, g) {
+                c[g] = !0
             }), c
         }
         p.Callbacks = function(a) {
             a = typeof a == "string" ? zi(a) : p.extend({}, a);
-            var c, d, m, b, x = [],
+            var c, d, g, b, x = [],
                 w = [],
                 T = -1,
-                A = function() {
-                    for (b = b || a.once, m = c = !0; w.length; T = -1)
+                C = function() {
+                    for (b = b || a.once, g = c = !0; w.length; T = -1)
                         for (d = w.shift(); ++T < x.length;) x[T].apply(d[0], d[1]) === !1 && a.stopOnFalse && (T = x.length, d = !1);
                     a.memory || (d = !1), c = !1, b && (d ? x = [] : x = "")
                 },
                 E = {
                     add: function() {
                         return x && (d && !c && (T = x.length - 1, w.push(d)), function I(_) {
                             p.each(_, function(P, W) {
-                                C(W) ? (!a.unique || !E.has(W)) && x.push(W) : W && W.length && j(W) !== "string" && I(W)
+                                A(W) ? (!a.unique || !E.has(W)) && x.push(W) : W && W.length && j(W) !== "string" && I(W)
                             })
-                        }(arguments), d && !c && A()), this
+                        }(arguments), d && !c && C()), this
                     },
                     remove: function() {
                         return p.each(arguments, function(I, _) {
                             for (var P;
                                 (P = p.inArray(_, x, P)) > -1;) x.splice(P, 1), P <= T && T--
                         }), this
                     },
@@ -1102,127 +1102,127 @@
                     lock: function() {
                         return b = w = [], !d && !c && (x = d = ""), this
                     },
                     locked: function() {
                         return !!b
                     },
                     fireWith: function(I, _) {
-                        return b || (_ = _ || [], _ = [I, _.slice ? _.slice() : _], w.push(_), c || A()), this
+                        return b || (_ = _ || [], _ = [I, _.slice ? _.slice() : _], w.push(_), c || C()), this
                     },
                     fire: function() {
                         return E.fireWith(this, arguments), this
                     },
                     fired: function() {
-                        return !!m
+                        return !!g
                     }
                 };
             return E
         };
 
         function bi(a) {
             return a
         }
 
         function Yi(a) {
             throw a
         }
 
-        function $i(a, c, d, m) {
+        function $i(a, c, d, g) {
             var b;
             try {
-                a && C(b = a.promise) ? b.call(a).done(c).fail(d) : a && C(b = a.then) ? b.call(a, c, d) : c.apply(void 0, [a].slice(m))
+                a && A(b = a.promise) ? b.call(a).done(c).fail(d) : a && A(b = a.then) ? b.call(a, c, d) : c.apply(void 0, [a].slice(g))
             } catch (x) {
                 d.apply(void 0, [x])
             }
         }
         p.extend({
             Deferred: function(a) {
                 var c = [
                         ["notify", "progress", p.Callbacks("memory"), p.Callbacks("memory"), 2],
                         ["resolve", "done", p.Callbacks("once memory"), p.Callbacks("once memory"), 0, "resolved"],
                         ["reject", "fail", p.Callbacks("once memory"), p.Callbacks("once memory"), 1, "rejected"]
                     ],
                     d = "pending",
-                    m = {
+                    g = {
                         state: function() {
                             return d
                         },
                         always: function() {
                             return b.done(arguments).fail(arguments), this
                         },
                         catch: function(x) {
-                            return m.then(null, x)
+                            return g.then(null, x)
                         },
                         pipe: function() {
                             var x = arguments;
                             return p.Deferred(function(w) {
-                                p.each(c, function(T, A) {
-                                    var E = C(x[A[4]]) && x[A[4]];
-                                    b[A[1]](function() {
+                                p.each(c, function(T, C) {
+                                    var E = A(x[C[4]]) && x[C[4]];
+                                    b[C[1]](function() {
                                         var I = E && E.apply(this, arguments);
-                                        I && C(I.promise) ? I.promise().progress(w.notify).done(w.resolve).fail(w.reject) : w[A[0] + "With"](this, E ? [I] : arguments)
+                                        I && A(I.promise) ? I.promise().progress(w.notify).done(w.resolve).fail(w.reject) : w[C[0] + "With"](this, E ? [I] : arguments)
                                     })
                                 }), x = null
                             }).promise()
                         },
                         then: function(x, w, T) {
-                            var A = 0;
+                            var C = 0;
 
                             function E(I, _, P, W) {
                                 return function() {
                                     var ce = this,
-                                        Te = arguments,
+                                        Ae = arguments,
                                         ge = function() {
                                             var et, wi;
-                                            if (!(I < A)) {
-                                                if (et = P.apply(ce, Te), et === _.promise()) throw new TypeError("Thenable self-resolution");
-                                                wi = et && (typeof et == "object" || typeof et == "function") && et.then, C(wi) ? W ? wi.call(et, E(A, _, bi, W), E(A, _, Yi, W)) : (A++, wi.call(et, E(A, _, bi, W), E(A, _, Yi, W), E(A, _, bi, _.notifyWith))) : (P !== bi && (ce = void 0, Te = [et]), (W || _.resolveWith)(ce, Te))
+                                            if (!(I < C)) {
+                                                if (et = P.apply(ce, Ae), et === _.promise()) throw new TypeError("Thenable self-resolution");
+                                                wi = et && (typeof et == "object" || typeof et == "function") && et.then, A(wi) ? W ? wi.call(et, E(C, _, bi, W), E(C, _, Yi, W)) : (C++, wi.call(et, E(C, _, bi, W), E(C, _, Yi, W), E(C, _, bi, _.notifyWith))) : (P !== bi && (ce = void 0, Ae = [et]), (W || _.resolveWith)(ce, Ae))
                                             }
                                         },
                                         ut = W ? ge : function() {
                                             try {
                                                 ge()
                                             } catch (et) {
-                                                p.Deferred.exceptionHook && p.Deferred.exceptionHook(et, ut.error), I + 1 >= A && (P !== Yi && (ce = void 0, Te = [et]), _.rejectWith(ce, Te))
+                                                p.Deferred.exceptionHook && p.Deferred.exceptionHook(et, ut.error), I + 1 >= C && (P !== Yi && (ce = void 0, Ae = [et]), _.rejectWith(ce, Ae))
                                             }
                                         };
                                     I ? ut() : (p.Deferred.getErrorHook ? ut.error = p.Deferred.getErrorHook() : p.Deferred.getStackHook && (ut.error = p.Deferred.getStackHook()), e.setTimeout(ut))
                                 }
                             }
                             return p.Deferred(function(I) {
-                                c[0][3].add(E(0, I, C(T) ? T : bi, I.notifyWith)), c[1][3].add(E(0, I, C(x) ? x : bi)), c[2][3].add(E(0, I, C(w) ? w : Yi))
+                                c[0][3].add(E(0, I, A(T) ? T : bi, I.notifyWith)), c[1][3].add(E(0, I, A(x) ? x : bi)), c[2][3].add(E(0, I, A(w) ? w : Yi))
                             }).promise()
                         },
                         promise: function(x) {
-                            return x != null ? p.extend(x, m) : m
+                            return x != null ? p.extend(x, g) : g
                         }
                     },
                     b = {};
                 return p.each(c, function(x, w) {
                     var T = w[2],
-                        A = w[5];
-                    m[w[1]] = T.add, A && T.add(function() {
-                        d = A
+                        C = w[5];
+                    g[w[1]] = T.add, C && T.add(function() {
+                        d = C
                     }, c[3 - x][2].disable, c[3 - x][3].disable, c[0][2].lock, c[0][3].lock), T.add(w[3].fire), b[w[0]] = function() {
                         return b[w[0] + "With"](this === b ? void 0 : this, arguments), this
                     }, b[w[0] + "With"] = T.fireWith
-                }), m.promise(b), a && a.call(b, b), b
+                }), g.promise(b), a && a.call(b, b), b
             },
             when: function(a) {
                 var c = arguments.length,
                     d = c,
-                    m = Array(d),
+                    g = Array(d),
                     b = s.call(arguments),
                     x = p.Deferred(),
                     w = function(T) {
-                        return function(A) {
-                            m[T] = this, b[T] = arguments.length > 1 ? s.call(arguments) : A, --c || x.resolveWith(m, b)
+                        return function(C) {
+                            g[T] = this, b[T] = arguments.length > 1 ? s.call(arguments) : C, --c || x.resolveWith(g, b)
                         }
                     };
-                if (c <= 1 && ($i(a, x.done(w(d)).resolve, x.reject, !c), x.state() === "pending" || C(b[d] && b[d].then))) return x.then();
+                if (c <= 1 && ($i(a, x.done(w(d)).resolve, x.reject, !c), x.state() === "pending" || A(b[d] && b[d].then))) return x.then();
                 for (; d--;) $i(b[d], w(d), x.reject);
                 return x.promise()
             }
         });
         var Yn = /^(Eval|Internal|Range|Reference|Syntax|Type|URI)Error$/;
         p.Deferred.exceptionHook = function(a, c) {
             e.console && e.console.warn && a && Yn.test(a.name) && e.console.warn("jQuery.Deferred exception: " + a.message, a.stack, c)
@@ -1244,26 +1244,26 @@
             }
         }), p.ready.then = Ji.then;
 
         function Mn() {
             D.removeEventListener("DOMContentLoaded", Mn), e.removeEventListener("load", Mn), p.ready()
         }
         D.readyState === "complete" || D.readyState !== "loading" && !D.documentElement.doScroll ? e.setTimeout(p.ready) : (D.addEventListener("DOMContentLoaded", Mn), e.addEventListener("load", Mn));
-        var Kt = function(a, c, d, m, b, x, w) {
+        var Kt = function(a, c, d, g, b, x, w) {
                 var T = 0,
-                    A = a.length,
+                    C = a.length,
                     E = d == null;
                 if (j(d) === "object") {
                     b = !0;
                     for (T in d) Kt(a, c, T, d[T], !0, x, w)
-                } else if (m !== void 0 && (b = !0, C(m) || (w = !0), E && (w ? (c.call(a, m), c = null) : (E = c, c = function(I, _, P) {
+                } else if (g !== void 0 && (b = !0, A(g) || (w = !0), E && (w ? (c.call(a, g), c = null) : (E = c, c = function(I, _, P) {
                         return E.call(p(I), P)
                     })), c))
-                    for (; T < A; T++) c(a[T], d, w ? m : m.call(a[T], T, c(a[T], d)));
-                return b ? a : E ? c.call(a) : A ? c(a[0], d) : x
+                    for (; T < C; T++) c(a[T], d, w ? g : g.call(a[T], T, c(a[T], d)));
+                return b ? a : E ? c.call(a) : C ? c(a[0], d) : x
             },
             Ll = /^-ms-/,
             Dr = /-([a-z])/g;
 
         function En(a, c) {
             return c.toUpperCase()
         }
@@ -1283,32 +1283,32 @@
                 var c = a[this.expando];
                 return c || (c = {}, Xt(a) && (a.nodeType ? a[this.expando] = c : Object.defineProperty(a, this.expando, {
                     value: c,
                     configurable: !0
                 }))), c
             },
             set: function(a, c, d) {
-                var m, b = this.cache(a);
+                var g, b = this.cache(a);
                 if (typeof c == "string") b[ht(c)] = d;
                 else
-                    for (m in c) b[ht(m)] = c[m];
+                    for (g in c) b[ht(g)] = c[g];
                 return b
             },
             get: function(a, c) {
                 return c === void 0 ? this.cache(a) : a[this.expando] && a[this.expando][ht(c)]
             },
             access: function(a, c, d) {
                 return c === void 0 || c && typeof c == "string" && d === void 0 ? this.get(a, c) : (this.set(a, c, d), d !== void 0 ? d : c)
             },
             remove: function(a, c) {
-                var d, m = a[this.expando];
-                if (m !== void 0) {
+                var d, g = a[this.expando];
+                if (g !== void 0) {
                     if (c !== void 0)
-                        for (Array.isArray(c) ? c = c.map(ht) : (c = ht(c), c = c in m ? [c] : c.match(at) || []), d = c.length; d--;) delete m[c[d]];
-                    (c === void 0 || p.isEmptyObject(m)) && (a.nodeType ? a[this.expando] = void 0 : delete a[this.expando])
+                        for (Array.isArray(c) ? c = c.map(ht) : (c = ht(c), c = c in g ? [c] : c.match(at) || []), d = c.length; d--;) delete g[c[d]];
+                    (c === void 0 || p.isEmptyObject(g)) && (a.nodeType ? a[this.expando] = void 0 : delete a[this.expando])
                 }
             },
             hasData: function(a) {
                 var c = a[this.expando];
                 return c !== void 0 && !p.isEmptyObject(c)
             }
         };
@@ -1318,17 +1318,17 @@
             _s = /[A-Z]/g;
 
         function Jn(a) {
             return a === "true" ? !0 : a === "false" ? !1 : a === "null" ? null : a === +a + "" ? +a : Rr.test(a) ? JSON.parse(a) : a
         }
 
         function Dn(a, c, d) {
-            var m;
+            var g;
             if (d === void 0 && a.nodeType === 1)
-                if (m = "data-" + c.replace(_s, "-$&").toLowerCase(), d = a.getAttribute(m), typeof d == "string") {
+                if (g = "data-" + c.replace(_s, "-$&").toLowerCase(), d = a.getAttribute(g), typeof d == "string") {
                     try {
                         d = Jn(d)
                     } catch (b) {}
                     ct.set(a, c, d)
                 } else d = void 0;
             return d
         }
@@ -1346,87 +1346,87 @@
                 return ne.access(a, c, d)
             },
             _removeData: function(a, c) {
                 ne.remove(a, c)
             }
         }), p.fn.extend({
             data: function(a, c) {
-                var d, m, b, x = this[0],
+                var d, g, b, x = this[0],
                     w = x && x.attributes;
                 if (a === void 0) {
                     if (this.length && (b = ct.get(x), x.nodeType === 1 && !ne.get(x, "hasDataAttrs"))) {
-                        for (d = w.length; d--;) w[d] && (m = w[d].name, m.indexOf("data-") === 0 && (m = ht(m.slice(5)), Dn(x, m, b[m])));
+                        for (d = w.length; d--;) w[d] && (g = w[d].name, g.indexOf("data-") === 0 && (g = ht(g.slice(5)), Dn(x, g, b[g])));
                         ne.set(x, "hasDataAttrs", !0)
                     }
                     return b
                 }
                 return typeof a == "object" ? this.each(function() {
                     ct.set(this, a)
                 }) : Kt(this, function(T) {
-                    var A;
-                    if (x && T === void 0) return A = ct.get(x, a), A !== void 0 || (A = Dn(x, a), A !== void 0) ? A : void 0;
+                    var C;
+                    if (x && T === void 0) return C = ct.get(x, a), C !== void 0 || (C = Dn(x, a), C !== void 0) ? C : void 0;
                     this.each(function() {
                         ct.set(this, a, T)
                     })
                 }, null, c, arguments.length > 1, null, !0)
             },
             removeData: function(a) {
                 return this.each(function() {
                     ct.remove(this, a)
                 })
             }
         }), p.extend({
             queue: function(a, c, d) {
-                var m;
-                if (a) return c = (c || "fx") + "queue", m = ne.get(a, c), d && (!m || Array.isArray(d) ? m = ne.access(a, c, p.makeArray(d)) : m.push(d)), m || []
+                var g;
+                if (a) return c = (c || "fx") + "queue", g = ne.get(a, c), d && (!g || Array.isArray(d) ? g = ne.access(a, c, p.makeArray(d)) : g.push(d)), g || []
             },
             dequeue: function(a, c) {
                 c = c || "fx";
                 var d = p.queue(a, c),
-                    m = d.length,
+                    g = d.length,
                     b = d.shift(),
                     x = p._queueHooks(a, c),
                     w = function() {
                         p.dequeue(a, c)
                     };
-                b === "inprogress" && (b = d.shift(), m--), b && (c === "fx" && d.unshift("inprogress"), delete x.stop, b.call(a, w, x)), !m && x && x.empty.fire()
+                b === "inprogress" && (b = d.shift(), g--), b && (c === "fx" && d.unshift("inprogress"), delete x.stop, b.call(a, w, x)), !g && x && x.empty.fire()
             },
             _queueHooks: function(a, c) {
                 var d = c + "queueHooks";
                 return ne.get(a, d) || ne.access(a, d, {
                     empty: p.Callbacks("once memory").add(function() {
                         ne.remove(a, [c + "queue", d])
                     })
                 })
             }
         }), p.fn.extend({
             queue: function(a, c) {
                 var d = 2;
                 return typeof a != "string" && (c = a, a = "fx", d--), arguments.length < d ? p.queue(this[0], a) : c === void 0 ? this : this.each(function() {
-                    var m = p.queue(this, a, c);
-                    p._queueHooks(this, a), a === "fx" && m[0] !== "inprogress" && p.dequeue(this, a)
+                    var g = p.queue(this, a, c);
+                    p._queueHooks(this, a), a === "fx" && g[0] !== "inprogress" && p.dequeue(this, a)
                 })
             },
             dequeue: function(a) {
                 return this.each(function() {
                     p.dequeue(this, a)
                 })
             },
             clearQueue: function(a) {
                 return this.queue(a || "fx", [])
             },
             promise: function(a, c) {
-                var d, m = 1,
+                var d, g = 1,
                     b = p.Deferred(),
                     x = this,
                     w = this.length,
                     T = function() {
-                        --m || b.resolveWith(x, [x])
+                        --g || b.resolveWith(x, [x])
                     };
-                for (typeof a != "string" && (c = a, a = void 0), a = a || "fx"; w--;) d = ne.get(x[w], a + "queueHooks"), d && d.empty && (m++, d.empty.add(T));
+                for (typeof a != "string" && (c = a, a = void 0), a = a || "fx"; w--;) d = ne.get(x[w], a + "queueHooks"), d && d.empty && (g++, d.empty.add(T));
                 return T(), b.promise(c)
             }
         });
         var Yt = /[+-]?(?:\d*\.|)\d+(?:[eE][+-]?\d+|)/.source,
             Jt = new RegExp("^(?:([+-])=|)(" + Yt + ")([a-z%]*)$", "i"),
             Ft = ["Top", "Right", "Bottom", "Left"],
             ai = D.documentElement,
@@ -1439,41 +1439,41 @@
         ai.getRootNode && (en = function(a) {
             return p.contains(a.ownerDocument, a) || a.getRootNode(Rn) === a.ownerDocument
         });
         var Zn = function(a, c) {
             return a = c || a, a.style.display === "none" || a.style.display === "" && en(a) && p.css(a, "display") === "none"
         };
 
-        function Hs(a, c, d, m) {
+        function Hs(a, c, d, g) {
             var b, x, w = 20,
-                T = m ? function() {
-                    return m.cur()
+                T = g ? function() {
+                    return g.cur()
                 } : function() {
                     return p.css(a, c, "")
                 },
-                A = T(),
+                C = T(),
                 E = d && d[3] || (p.cssNumber[c] ? "" : "px"),
-                I = a.nodeType && (p.cssNumber[c] || E !== "px" && +A) && Jt.exec(p.css(a, c));
+                I = a.nodeType && (p.cssNumber[c] || E !== "px" && +C) && Jt.exec(p.css(a, c));
             if (I && I[3] !== E) {
-                for (A = A / 2, E = E || I[3], I = +A || 1; w--;) p.style(a, c, I + E), (1 - x) * (1 - (x = T() / A || .5)) <= 0 && (w = 0), I = I / x;
+                for (C = C / 2, E = E || I[3], I = +C || 1; w--;) p.style(a, c, I + E), (1 - x) * (1 - (x = T() / C || .5)) <= 0 && (w = 0), I = I / x;
                 I = I * 2, p.style(a, c, I + E), d = d || []
             }
-            return d && (I = +I || +A || 0, b = d[1] ? I + (d[1] + 1) * d[2] : +d[2], m && (m.unit = E, m.start = I, m.end = b)), b
+            return d && (I = +I || +C || 0, b = d[1] ? I + (d[1] + 1) * d[2] : +d[2], g && (g.unit = E, g.start = I, g.end = b)), b
         }
         var Ge = {};
 
         function tn(a) {
             var c, d = a.ownerDocument,
-                m = a.nodeName,
-                b = Ge[m];
-            return b || (c = d.body.appendChild(d.createElement(m)), b = p.css(c, "display"), c.parentNode.removeChild(c), b === "none" && (b = "block"), Ge[m] = b, b)
+                g = a.nodeName,
+                b = Ge[g];
+            return b || (c = d.body.appendChild(d.createElement(g)), b = p.css(c, "display"), c.parentNode.removeChild(c), b === "none" && (b = "block"), Ge[g] = b, b)
         }
 
         function nn(a, c) {
-            for (var d, m, b = [], x = 0, w = a.length; x < w; x++) m = a[x], m.style && (d = m.style.display, c ? (d === "none" && (b[x] = ne.get(m, "display") || null, b[x] || (m.style.display = "")), m.style.display === "" && Zn(m) && (b[x] = tn(m))) : d !== "none" && (b[x] = "none", ne.set(m, "display", d)));
+            for (var d, g, b = [], x = 0, w = a.length; x < w; x++) g = a[x], g.style && (d = g.style.display, c ? (d === "none" && (b[x] = ne.get(g, "display") || null, b[x] || (g.style.display = "")), g.style.display === "" && Zn(g) && (b[x] = tn(g))) : d !== "none" && (b[x] = "none", ne.set(g, "display", d)));
             for (x = 0; x < w; x++) b[x] != null && (a[x].style.display = b[x]);
             return a
         }
         p.fn.extend({
             show: function() {
                 return nn(this, !0)
             },
@@ -1506,29 +1506,29 @@
 
         function xt(a, c) {
             var d;
             return typeof a.getElementsByTagName != "undefined" ? d = a.getElementsByTagName(c || "*") : typeof a.querySelectorAll != "undefined" ? d = a.querySelectorAll(c || "*") : d = [], c === void 0 || c && J(a, c) ? p.merge([a], d) : d
         }
 
         function tr(a, c) {
-            for (var d = 0, m = a.length; d < m; d++) ne.set(a[d], "globalEval", !c || ne.get(c[d], "globalEval"))
+            for (var d = 0, g = a.length; d < g; d++) ne.set(a[d], "globalEval", !c || ne.get(c[d], "globalEval"))
         }
         var Fs = /<|&#?\w+;/;
 
-        function zs(a, c, d, m, b) {
-            for (var x, w, T, A, E, I, _ = c.createDocumentFragment(), P = [], W = 0, ce = a.length; W < ce; W++)
+        function zs(a, c, d, g, b) {
+            for (var x, w, T, C, E, I, _ = c.createDocumentFragment(), P = [], W = 0, ce = a.length; W < ce; W++)
                 if (x = a[W], x || x === 0)
                     if (j(x) === "object") p.merge(P, x.nodeType ? [x] : x);
                     else if (!Fs.test(x)) P.push(c.createTextNode(x));
             else {
-                for (w = w || _.appendChild(c.createElement("div")), T = (er.exec(x) || ["", ""])[1].toLowerCase(), A = Ot[T] || Ot._default, w.innerHTML = A[1] + p.htmlPrefilter(x) + A[2], I = A[0]; I--;) w = w.lastChild;
+                for (w = w || _.appendChild(c.createElement("div")), T = (er.exec(x) || ["", ""])[1].toLowerCase(), C = Ot[T] || Ot._default, w.innerHTML = C[1] + p.htmlPrefilter(x) + C[2], I = C[0]; I--;) w = w.lastChild;
                 p.merge(P, w.childNodes), w = _.firstChild, w.textContent = ""
             }
             for (_.textContent = "", W = 0; x = P[W++];) {
-                if (m && p.inArray(x, m) > -1) {
+                if (g && p.inArray(x, g) > -1) {
                     b && b.push(x);
                     continue
                 }
                 if (E = en(x), w = xt(_.appendChild(x), "script"), E && tr(w), d)
                     for (I = 0; x = w[I++];) Lr.test(x.type || "") && d.push(x)
             }
             return _
@@ -1539,99 +1539,99 @@
             return !0
         }
 
         function Wi() {
             return !1
         }
 
-        function ir(a, c, d, m, b, x) {
+        function ir(a, c, d, g, b, x) {
             var w, T;
             if (typeof c == "object") {
-                typeof d != "string" && (m = m || d, d = void 0);
-                for (T in c) ir(a, T, d, m, c[T], x);
+                typeof d != "string" && (g = g || d, d = void 0);
+                for (T in c) ir(a, T, d, g, c[T], x);
                 return a
             }
-            if (m == null && b == null ? (b = d, m = d = void 0) : b == null && (typeof d == "string" ? (b = m, m = void 0) : (b = m, m = d, d = void 0)), b === !1) b = Wi;
+            if (g == null && b == null ? (b = d, g = d = void 0) : b == null && (typeof d == "string" ? (b = g, g = void 0) : (b = g, g = d, d = void 0)), b === !1) b = Wi;
             else if (!b) return a;
-            return x === 1 && (w = b, b = function(A) {
-                return p().off(A), w.apply(this, arguments)
+            return x === 1 && (w = b, b = function(C) {
+                return p().off(C), w.apply(this, arguments)
             }, b.guid = w.guid || (w.guid = p.guid++)), a.each(function() {
-                p.event.add(this, c, b, m, d)
+                p.event.add(this, c, b, g, d)
             })
         }
         p.event = {
             global: {},
-            add: function(a, c, d, m, b) {
-                var x, w, T, A, E, I, _, P, W, ce, Te, ge = ne.get(a);
+            add: function(a, c, d, g, b) {
+                var x, w, T, C, E, I, _, P, W, ce, Ae, ge = ne.get(a);
                 if (Xt(a))
-                    for (d.handler && (x = d, d = x.handler, b = x.selector), b && p.find.matchesSelector(ai, b), d.guid || (d.guid = p.guid++), (A = ge.events) || (A = ge.events = Object.create(null)), (w = ge.handle) || (w = ge.handle = function(ut) {
+                    for (d.handler && (x = d, d = x.handler, b = x.selector), b && p.find.matchesSelector(ai, b), d.guid || (d.guid = p.guid++), (C = ge.events) || (C = ge.events = Object.create(null)), (w = ge.handle) || (w = ge.handle = function(ut) {
                             return typeof p != "undefined" && p.event.triggered !== ut.type ? p.event.dispatch.apply(a, arguments) : void 0
-                        }), c = (c || "").match(at) || [""], E = c.length; E--;) T = xi.exec(c[E]) || [], W = Te = T[1], ce = (T[2] || "").split(".").sort(), W && (_ = p.event.special[W] || {}, W = (b ? _.delegateType : _.bindType) || W, _ = p.event.special[W] || {}, I = p.extend({
+                        }), c = (c || "").match(at) || [""], E = c.length; E--;) T = xi.exec(c[E]) || [], W = Ae = T[1], ce = (T[2] || "").split(".").sort(), W && (_ = p.event.special[W] || {}, W = (b ? _.delegateType : _.bindType) || W, _ = p.event.special[W] || {}, I = p.extend({
                         type: W,
-                        origType: Te,
-                        data: m,
+                        origType: Ae,
+                        data: g,
                         handler: d,
                         guid: d.guid,
                         selector: b,
                         needsContext: b && p.expr.match.needsContext.test(b),
                         namespace: ce.join(".")
-                    }, x), (P = A[W]) || (P = A[W] = [], P.delegateCount = 0, (!_.setup || _.setup.call(a, m, ce, w) === !1) && a.addEventListener && a.addEventListener(W, w)), _.add && (_.add.call(a, I), I.handler.guid || (I.handler.guid = d.guid)), b ? P.splice(P.delegateCount++, 0, I) : P.push(I), p.event.global[W] = !0)
+                    }, x), (P = C[W]) || (P = C[W] = [], P.delegateCount = 0, (!_.setup || _.setup.call(a, g, ce, w) === !1) && a.addEventListener && a.addEventListener(W, w)), _.add && (_.add.call(a, I), I.handler.guid || (I.handler.guid = d.guid)), b ? P.splice(P.delegateCount++, 0, I) : P.push(I), p.event.global[W] = !0)
             },
-            remove: function(a, c, d, m, b) {
-                var x, w, T, A, E, I, _, P, W, ce, Te, ge = ne.hasData(a) && ne.get(a);
-                if (!(!ge || !(A = ge.events))) {
+            remove: function(a, c, d, g, b) {
+                var x, w, T, C, E, I, _, P, W, ce, Ae, ge = ne.hasData(a) && ne.get(a);
+                if (!(!ge || !(C = ge.events))) {
                     for (c = (c || "").match(at) || [""], E = c.length; E--;) {
-                        if (T = xi.exec(c[E]) || [], W = Te = T[1], ce = (T[2] || "").split(".").sort(), !W) {
-                            for (W in A) p.event.remove(a, W + c[E], d, m, !0);
+                        if (T = xi.exec(c[E]) || [], W = Ae = T[1], ce = (T[2] || "").split(".").sort(), !W) {
+                            for (W in C) p.event.remove(a, W + c[E], d, g, !0);
                             continue
                         }
-                        for (_ = p.event.special[W] || {}, W = (m ? _.delegateType : _.bindType) || W, P = A[W] || [], T = T[2] && new RegExp("(^|\\.)" + ce.join("\\.(?:.*\\.|)") + "(\\.|$)"), w = x = P.length; x--;) I = P[x], (b || Te === I.origType) && (!d || d.guid === I.guid) && (!T || T.test(I.namespace)) && (!m || m === I.selector || m === "**" && I.selector) && (P.splice(x, 1), I.selector && P.delegateCount--, _.remove && _.remove.call(a, I));
-                        w && !P.length && ((!_.teardown || _.teardown.call(a, ce, ge.handle) === !1) && p.removeEvent(a, W, ge.handle), delete A[W])
+                        for (_ = p.event.special[W] || {}, W = (g ? _.delegateType : _.bindType) || W, P = C[W] || [], T = T[2] && new RegExp("(^|\\.)" + ce.join("\\.(?:.*\\.|)") + "(\\.|$)"), w = x = P.length; x--;) I = P[x], (b || Ae === I.origType) && (!d || d.guid === I.guid) && (!T || T.test(I.namespace)) && (!g || g === I.selector || g === "**" && I.selector) && (P.splice(x, 1), I.selector && P.delegateCount--, _.remove && _.remove.call(a, I));
+                        w && !P.length && ((!_.teardown || _.teardown.call(a, ce, ge.handle) === !1) && p.removeEvent(a, W, ge.handle), delete C[W])
                     }
-                    p.isEmptyObject(A) && ne.remove(a, "handle events")
+                    p.isEmptyObject(C) && ne.remove(a, "handle events")
                 }
             },
             dispatch: function(a) {
-                var c, d, m, b, x, w, T = new Array(arguments.length),
-                    A = p.event.fix(a),
-                    E = (ne.get(this, "events") || Object.create(null))[A.type] || [],
-                    I = p.event.special[A.type] || {};
-                for (T[0] = A, c = 1; c < arguments.length; c++) T[c] = arguments[c];
-                if (A.delegateTarget = this, !(I.preDispatch && I.preDispatch.call(this, A) === !1)) {
-                    for (w = p.event.handlers.call(this, A, E), c = 0;
-                        (b = w[c++]) && !A.isPropagationStopped();)
-                        for (A.currentTarget = b.elem, d = 0;
-                            (x = b.handlers[d++]) && !A.isImmediatePropagationStopped();)(!A.rnamespace || x.namespace === !1 || A.rnamespace.test(x.namespace)) && (A.handleObj = x, A.data = x.data, m = ((p.event.special[x.origType] || {}).handle || x.handler).apply(b.elem, T), m !== void 0 && (A.result = m) === !1 && (A.preventDefault(), A.stopPropagation()));
-                    return I.postDispatch && I.postDispatch.call(this, A), A.result
+                var c, d, g, b, x, w, T = new Array(arguments.length),
+                    C = p.event.fix(a),
+                    E = (ne.get(this, "events") || Object.create(null))[C.type] || [],
+                    I = p.event.special[C.type] || {};
+                for (T[0] = C, c = 1; c < arguments.length; c++) T[c] = arguments[c];
+                if (C.delegateTarget = this, !(I.preDispatch && I.preDispatch.call(this, C) === !1)) {
+                    for (w = p.event.handlers.call(this, C, E), c = 0;
+                        (b = w[c++]) && !C.isPropagationStopped();)
+                        for (C.currentTarget = b.elem, d = 0;
+                            (x = b.handlers[d++]) && !C.isImmediatePropagationStopped();)(!C.rnamespace || x.namespace === !1 || C.rnamespace.test(x.namespace)) && (C.handleObj = x, C.data = x.data, g = ((p.event.special[x.origType] || {}).handle || x.handler).apply(b.elem, T), g !== void 0 && (C.result = g) === !1 && (C.preventDefault(), C.stopPropagation()));
+                    return I.postDispatch && I.postDispatch.call(this, C), C.result
                 }
             },
             handlers: function(a, c) {
-                var d, m, b, x, w, T = [],
-                    A = c.delegateCount,
+                var d, g, b, x, w, T = [],
+                    C = c.delegateCount,
                     E = a.target;
-                if (A && E.nodeType && !(a.type === "click" && a.button >= 1)) {
+                if (C && E.nodeType && !(a.type === "click" && a.button >= 1)) {
                     for (; E !== this; E = E.parentNode || this)
                         if (E.nodeType === 1 && !(a.type === "click" && E.disabled === !0)) {
-                            for (x = [], w = {}, d = 0; d < A; d++) m = c[d], b = m.selector + " ", w[b] === void 0 && (w[b] = m.needsContext ? p(b, this).index(E) > -1 : p.find(b, this, null, [E]).length), w[b] && x.push(m);
+                            for (x = [], w = {}, d = 0; d < C; d++) g = c[d], b = g.selector + " ", w[b] === void 0 && (w[b] = g.needsContext ? p(b, this).index(E) > -1 : p.find(b, this, null, [E]).length), w[b] && x.push(g);
                             x.length && T.push({
                                 elem: E,
                                 handlers: x
                             })
                         }
                 }
-                return E = this, A < c.length && T.push({
+                return E = this, C < c.length && T.push({
                     elem: E,
-                    handlers: c.slice(A)
+                    handlers: c.slice(C)
                 }), T
             },
             addProp: function(a, c) {
                 Object.defineProperty(p.Event.prototype, a, {
                     enumerable: !0,
                     configurable: !0,
-                    get: C(c) ? function() {
+                    get: A(c) ? function() {
                         if (this.originalEvent) return c(this.originalEvent)
                     } : function() {
                         if (this.originalEvent) return this.originalEvent[a]
                     },
                     set: function(d) {
                         Object.defineProperty(this, a, {
                             enumerable: !0,
@@ -1674,20 +1674,20 @@
         function nr(a, c, d) {
             if (!d) {
                 ne.get(a, c) === void 0 && p.event.add(a, c, ki);
                 return
             }
             ne.set(a, c, !1), p.event.add(a, c, {
                 namespace: !1,
-                handler: function(m) {
+                handler: function(g) {
                     var b, x = ne.get(this, c);
-                    if (m.isTrigger & 1 && this[c]) {
-                        if (x)(p.event.special[c] || {}).delegateType && m.stopPropagation();
-                        else if (x = s.call(arguments), ne.set(this, c, x), this[c](), b = ne.get(this, c), ne.set(this, c, !1), x !== b) return m.stopImmediatePropagation(), m.preventDefault(), b
-                    } else x && (ne.set(this, c, p.event.trigger(x[0], x.slice(1), this)), m.stopPropagation(), m.isImmediatePropagationStopped = ki)
+                    if (g.isTrigger & 1 && this[c]) {
+                        if (x)(p.event.special[c] || {}).delegateType && g.stopPropagation();
+                        else if (x = s.call(arguments), ne.set(this, c, x), this[c](), b = ne.get(this, c), ne.set(this, c, !1), x !== b) return g.stopImmediatePropagation(), g.preventDefault(), b
+                    } else x && (ne.set(this, c, p.event.trigger(x[0], x.slice(1), this)), g.stopPropagation(), g.isImmediatePropagationStopped = ki)
                 }
             })
         }
         p.removeEvent = function(a, c, d) {
             a.removeEventListener && a.removeEventListener(c, d)
         }, p.Event = function(a, c) {
             if (!(this instanceof p.Event)) return new p.Event(a, c);
@@ -1742,79 +1742,79 @@
             toElement: !0,
             touches: !0,
             which: !0
         }, p.event.addProp), p.each({
             focus: "focusin",
             blur: "focusout"
         }, function(a, c) {
-            function d(m) {
+            function d(g) {
                 if (D.documentMode) {
                     var b = ne.get(this, "handle"),
-                        x = p.event.fix(m);
-                    x.type = m.type === "focusin" ? "focus" : "blur", x.isSimulated = !0, b(m), x.target === x.currentTarget && b(x)
-                } else p.event.simulate(c, m.target, p.event.fix(m))
+                        x = p.event.fix(g);
+                    x.type = g.type === "focusin" ? "focus" : "blur", x.isSimulated = !0, b(g), x.target === x.currentTarget && b(x)
+                } else p.event.simulate(c, g.target, p.event.fix(g))
             }
             p.event.special[a] = {
                 setup: function() {
-                    var m;
-                    if (nr(this, a, !0), D.documentMode) m = ne.get(this, c), m || this.addEventListener(c, d), ne.set(this, c, (m || 0) + 1);
+                    var g;
+                    if (nr(this, a, !0), D.documentMode) g = ne.get(this, c), g || this.addEventListener(c, d), ne.set(this, c, (g || 0) + 1);
                     else return !1
                 },
                 trigger: function() {
                     return nr(this, a), !0
                 },
                 teardown: function() {
-                    var m;
-                    if (D.documentMode) m = ne.get(this, c) - 1, m ? ne.set(this, c, m) : (this.removeEventListener(c, d), ne.remove(this, c));
+                    var g;
+                    if (D.documentMode) g = ne.get(this, c) - 1, g ? ne.set(this, c, g) : (this.removeEventListener(c, d), ne.remove(this, c));
                     else return !1
                 },
-                _default: function(m) {
-                    return ne.get(m.target, a)
+                _default: function(g) {
+                    return ne.get(g.target, a)
                 },
                 delegateType: c
             }, p.event.special[c] = {
                 setup: function() {
-                    var m = this.ownerDocument || this.document || this,
-                        b = D.documentMode ? this : m,
+                    var g = this.ownerDocument || this.document || this,
+                        b = D.documentMode ? this : g,
                         x = ne.get(b, c);
-                    x || (D.documentMode ? this.addEventListener(c, d) : m.addEventListener(a, d, !0)), ne.set(b, c, (x || 0) + 1)
+                    x || (D.documentMode ? this.addEventListener(c, d) : g.addEventListener(a, d, !0)), ne.set(b, c, (x || 0) + 1)
                 },
                 teardown: function() {
-                    var m = this.ownerDocument || this.document || this,
-                        b = D.documentMode ? this : m,
+                    var g = this.ownerDocument || this.document || this,
+                        b = D.documentMode ? this : g,
                         x = ne.get(b, c) - 1;
-                    x ? ne.set(b, c, x) : (D.documentMode ? this.removeEventListener(c, d) : m.removeEventListener(a, d, !0), ne.remove(b, c))
+                    x ? ne.set(b, c, x) : (D.documentMode ? this.removeEventListener(c, d) : g.removeEventListener(a, d, !0), ne.remove(b, c))
                 }
             }
         }), p.each({
             mouseenter: "mouseover",
             mouseleave: "mouseout",
             pointerenter: "pointerover",
             pointerleave: "pointerout"
         }, function(a, c) {
             p.event.special[a] = {
                 delegateType: c,
                 bindType: c,
                 handle: function(d) {
-                    var m, b = this,
+                    var g, b = this,
                         x = d.relatedTarget,
                         w = d.handleObj;
-                    return (!x || x !== b && !p.contains(b, x)) && (d.type = w.origType, m = w.handler.apply(this, arguments), d.type = c), m
+                    return (!x || x !== b && !p.contains(b, x)) && (d.type = w.origType, g = w.handler.apply(this, arguments), d.type = c), g
                 }
             }
         }), p.fn.extend({
-            on: function(a, c, d, m) {
-                return ir(this, a, c, d, m)
+            on: function(a, c, d, g) {
+                return ir(this, a, c, d, g)
             },
-            one: function(a, c, d, m) {
-                return ir(this, a, c, d, m, 1)
+            one: function(a, c, d, g) {
+                return ir(this, a, c, d, g, 1)
             },
             off: function(a, c, d) {
-                var m, b;
-                if (a && a.preventDefault && a.handleObj) return m = a.handleObj, p(a.delegateTarget).off(m.namespace ? m.origType + "." + m.namespace : m.origType, m.selector, m.handler), this;
+                var g, b;
+                if (a && a.preventDefault && a.handleObj) return g = a.handleObj, p(a.delegateTarget).off(g.namespace ? g.origType + "." + g.namespace : g.origType, g.selector, g.handler), this;
                 if (typeof a == "object") {
                     for (b in a) this.off(b, c, a[b]);
                     return this
                 }
                 return (c === !1 || typeof c == "function") && (d = c, c = void 0), d === !1 && (d = Wi), this.each(function() {
                     p.event.remove(this, a, d, c)
                 })
@@ -1833,78 +1833,78 @@
         }
 
         function js(a) {
             return (a.type || "").slice(0, 5) === "true/" ? a.type = a.type.slice(5) : a.removeAttribute("type"), a
         }
 
         function Vs(a, c) {
-            var d, m, b, x, w, T, A;
+            var d, g, b, x, w, T, C;
             if (c.nodeType === 1) {
-                if (ne.hasData(a) && (x = ne.get(a), A = x.events, A)) {
+                if (ne.hasData(a) && (x = ne.get(a), C = x.events, C)) {
                     ne.remove(c, "handle events");
-                    for (b in A)
-                        for (d = 0, m = A[b].length; d < m; d++) p.event.add(c, b, A[b][d])
+                    for (b in C)
+                        for (d = 0, g = C[b].length; d < g; d++) p.event.add(c, b, C[b][d])
                 }
                 ct.hasData(a) && (w = ct.access(a), T = p.extend({}, w), ct.set(c, T))
             }
         }
 
         function se(a, c) {
             var d = c.nodeName.toLowerCase();
             d === "input" && rn.test(a.type) ? c.checked = a.checked : (d === "input" || d === "textarea") && (c.defaultValue = a.defaultValue)
         }
 
-        function R(a, c, d, m) {
+        function R(a, c, d, g) {
             c = o(c);
-            var b, x, w, T, A, E, I = 0,
+            var b, x, w, T, C, E, I = 0,
                 _ = a.length,
                 P = _ - 1,
                 W = c[0],
-                ce = C(W);
-            if (ce || _ > 1 && typeof W == "string" && !v.checkClone && hi.test(W)) return a.each(function(Te) {
-                var ge = a.eq(Te);
-                ce && (c[0] = W.call(this, Te, ge.html())), R(ge, c, d, m)
+                ce = A(W);
+            if (ce || _ > 1 && typeof W == "string" && !v.checkClone && hi.test(W)) return a.each(function(Ae) {
+                var ge = a.eq(Ae);
+                ce && (c[0] = W.call(this, Ae, ge.html())), R(ge, c, d, g)
             });
-            if (_ && (b = zs(c, a[0].ownerDocument, !1, a, m), x = b.firstChild, b.childNodes.length === 1 && (b = x), x || m)) {
-                for (w = p.map(xt(b, "script"), qs), T = w.length; I < _; I++) A = b, I !== P && (A = p.clone(A, !0, !0), T && p.merge(w, xt(A, "script"))), d.call(a[I], A, I);
+            if (_ && (b = zs(c, a[0].ownerDocument, !1, a, g), x = b.firstChild, b.childNodes.length === 1 && (b = x), x || g)) {
+                for (w = p.map(xt(b, "script"), qs), T = w.length; I < _; I++) C = b, I !== P && (C = p.clone(C, !0, !0), T && p.merge(w, xt(C, "script"))), d.call(a[I], C, I);
                 if (T)
-                    for (E = w[w.length - 1].ownerDocument, p.map(w, js), I = 0; I < T; I++) A = w[I], Lr.test(A.type || "") && !ne.access(A, "globalEval") && p.contains(E, A) && (A.src && (A.type || "").toLowerCase() !== "module" ? p._evalUrl && !A.noModule && p._evalUrl(A.src, {
-                        nonce: A.nonce || A.getAttribute("nonce")
-                    }, E) : $(A.textContent.replace(Ws, ""), A, E))
+                    for (E = w[w.length - 1].ownerDocument, p.map(w, js), I = 0; I < T; I++) C = w[I], Lr.test(C.type || "") && !ne.access(C, "globalEval") && p.contains(E, C) && (C.src && (C.type || "").toLowerCase() !== "module" ? p._evalUrl && !C.noModule && p._evalUrl(C.src, {
+                        nonce: C.nonce || C.getAttribute("nonce")
+                    }, E) : $(C.textContent.replace(Ws, ""), C, E))
             }
             return a
         }
 
         function V(a, c, d) {
-            for (var m, b = c ? p.filter(c, a) : a, x = 0;
-                (m = b[x]) != null; x++) !d && m.nodeType === 1 && p.cleanData(xt(m)), m.parentNode && (d && en(m) && tr(xt(m, "script")), m.parentNode.removeChild(m));
+            for (var g, b = c ? p.filter(c, a) : a, x = 0;
+                (g = b[x]) != null; x++) !d && g.nodeType === 1 && p.cleanData(xt(g)), g.parentNode && (d && en(g) && tr(xt(g, "script")), g.parentNode.removeChild(g));
             return a
         }
         p.extend({
             htmlPrefilter: function(a) {
                 return a
             },
             clone: function(a, c, d) {
-                var m, b, x, w, T = a.cloneNode(!0),
-                    A = en(a);
+                var g, b, x, w, T = a.cloneNode(!0),
+                    C = en(a);
                 if (!v.noCloneChecked && (a.nodeType === 1 || a.nodeType === 11) && !p.isXMLDoc(a))
-                    for (w = xt(T), x = xt(a), m = 0, b = x.length; m < b; m++) se(x[m], w[m]);
+                    for (w = xt(T), x = xt(a), g = 0, b = x.length; g < b; g++) se(x[g], w[g]);
                 if (c)
                     if (d)
-                        for (x = x || xt(a), w = w || xt(T), m = 0, b = x.length; m < b; m++) Vs(x[m], w[m]);
+                        for (x = x || xt(a), w = w || xt(T), g = 0, b = x.length; g < b; g++) Vs(x[g], w[g]);
                     else Vs(a, T);
-                return w = xt(T, "script"), w.length > 0 && tr(w, !A && xt(a, "script")), T
+                return w = xt(T, "script"), w.length > 0 && tr(w, !C && xt(a, "script")), T
             },
             cleanData: function(a) {
-                for (var c, d, m, b = p.event.special, x = 0;
+                for (var c, d, g, b = p.event.special, x = 0;
                     (d = a[x]) !== void 0; x++)
                     if (Xt(d)) {
                         if (c = d[ne.expando]) {
                             if (c.events)
-                                for (m in c.events) b[m] ? p.event.remove(d, m) : p.removeEvent(d, m, c.handle);
+                                for (g in c.events) b[g] ? p.event.remove(d, g) : p.removeEvent(d, g, c.handle);
                             d[ne.expando] = void 0
                         }
                         d[ct.expando] && (d[ct.expando] = void 0)
                     }
             }
         }), p.fn.extend({
             detach: function(a) {
@@ -1955,21 +1955,21 @@
                 return a = a == null ? !1 : a, c = c == null ? a : c, this.map(function() {
                     return p.clone(this, a, c)
                 })
             },
             html: function(a) {
                 return Kt(this, function(c) {
                     var d = this[0] || {},
-                        m = 0,
+                        g = 0,
                         b = this.length;
                     if (c === void 0 && d.nodeType === 1) return d.innerHTML;
                     if (typeof c == "string" && !$s.test(c) && !Ot[(er.exec(c) || ["", ""])[1].toLowerCase()]) {
                         c = p.htmlPrefilter(c);
                         try {
-                            for (; m < b; m++) d = this[m] || {}, d.nodeType === 1 && (p.cleanData(xt(d, !1)), d.innerHTML = c);
+                            for (; g < b; g++) d = this[g] || {}, d.nodeType === 1 && (p.cleanData(xt(d, !1)), d.innerHTML = c);
                             d = 0
                         } catch (x) {}
                     }
                     d && this.empty().append(c)
                 }, null, a, arguments.length)
             },
             replaceWith: function() {
@@ -1983,49 +1983,49 @@
             appendTo: "append",
             prependTo: "prepend",
             insertBefore: "before",
             insertAfter: "after",
             replaceAll: "replaceWith"
         }, function(a, c) {
             p.fn[a] = function(d) {
-                for (var m, b = [], x = p(d), w = x.length - 1, T = 0; T <= w; T++) m = T === w ? this : this.clone(!0), p(x[T])[c](m), l.apply(b, m.get());
+                for (var g, b = [], x = p(d), w = x.length - 1, T = 0; T <= w; T++) g = T === w ? this : this.clone(!0), p(x[T])[c](g), l.apply(b, g.get());
                 return this.pushStack(b)
             }
         });
         var Y = new RegExp("^(" + Yt + ")(?!px)[a-z%]+$", "i"),
             Re = /^--/,
             Ke = function(a) {
                 var c = a.ownerDocument.defaultView;
                 return (!c || !c.opener) && (c = e), c.getComputedStyle(a)
             },
             Ze = function(a, c, d) {
-                var m, b, x = {};
+                var g, b, x = {};
                 for (b in c) x[b] = a.style[b], a.style[b] = c[b];
-                m = d.call(a);
+                g = d.call(a);
                 for (b in c) a.style[b] = x[b];
-                return m
+                return g
             },
             kt = new RegExp(Ft.join("|"), "i");
         (function() {
             function a() {
                 if (E) {
-                    A.style.cssText = "position:absolute;left:-11111px;width:60px;margin-top:1px;padding:0;border:0", E.style.cssText = "position:relative;display:block;box-sizing:border-box;overflow:scroll;margin:auto;border:1px;padding:1px;width:60%;top:1%", ai.appendChild(A).appendChild(E);
+                    C.style.cssText = "position:absolute;left:-11111px;width:60px;margin-top:1px;padding:0;border:0", E.style.cssText = "position:relative;display:block;box-sizing:border-box;overflow:scroll;margin:auto;border:1px;padding:1px;width:60%;top:1%", ai.appendChild(C).appendChild(E);
                     var I = e.getComputedStyle(E);
-                    d = I.top !== "1%", T = c(I.marginLeft) === 12, E.style.right = "60%", x = c(I.right) === 36, m = c(I.width) === 36, E.style.position = "absolute", b = c(E.offsetWidth / 3) === 12, ai.removeChild(A), E = null
+                    d = I.top !== "1%", T = c(I.marginLeft) === 12, E.style.right = "60%", x = c(I.right) === 36, g = c(I.width) === 36, E.style.position = "absolute", b = c(E.offsetWidth / 3) === 12, ai.removeChild(C), E = null
                 }
             }
 
             function c(I) {
                 return Math.round(parseFloat(I))
             }
-            var d, m, b, x, w, T, A = D.createElement("div"),
+            var d, g, b, x, w, T, C = D.createElement("div"),
                 E = D.createElement("div");
             E.style && (E.style.backgroundClip = "content-box", E.cloneNode(!0).style.backgroundClip = "", v.clearCloneStyle = E.style.backgroundClip === "content-box", p.extend(v, {
                 boxSizingReliable: function() {
-                    return a(), m
+                    return a(), g
                 },
                 pixelBoxStyles: function() {
                     return a(), x
                 },
                 pixelPosition: function() {
                     return a(), d
                 },
@@ -2039,17 +2039,17 @@
                     var I, _, P, W;
                     return w == null && (I = D.createElement("table"), _ = D.createElement("tr"), P = D.createElement("div"), I.style.cssText = "position:absolute;left:-11111px;border-collapse:separate", _.style.cssText = "box-sizing:content-box;border:1px solid", _.style.height = "1px", P.style.height = "9px", P.style.display = "block", ai.appendChild(I).appendChild(_).appendChild(P), W = e.getComputedStyle(_), w = parseInt(W.height, 10) + parseInt(W.borderTopWidth, 10) + parseInt(W.borderBottomWidth, 10) === _.offsetHeight, ai.removeChild(I)), w
                 }
             }))
         })();
 
         function zt(a, c, d) {
-            var m, b, x, w, T = Re.test(c),
-                A = a.style;
-            return d = d || Ke(a), d && (w = d.getPropertyValue(c) || d[c], T && w && (w = w.replace(ye, "$1") || void 0), w === "" && !en(a) && (w = p.style(a, c)), !v.pixelBoxStyles() && Y.test(w) && kt.test(c) && (m = A.width, b = A.minWidth, x = A.maxWidth, A.minWidth = A.maxWidth = A.width = w, w = d.width, A.width = m, A.minWidth = b, A.maxWidth = x)), w !== void 0 ? w + "" : w
+            var g, b, x, w, T = Re.test(c),
+                C = a.style;
+            return d = d || Ke(a), d && (w = d.getPropertyValue(c) || d[c], T && w && (w = w.replace(ye, "$1") || void 0), w === "" && !en(a) && (w = p.style(a, c)), !v.pixelBoxStyles() && Y.test(w) && kt.test(c) && (g = C.width, b = C.minWidth, x = C.maxWidth, C.minWidth = C.maxWidth = C.width = w, w = d.width, C.width = g, C.minWidth = b, C.maxWidth = x)), w !== void 0 ? w + "" : w
         }
 
         function sn(a, c) {
             return {
                 get: function() {
                     if (a()) {
                         delete this.get;
@@ -2059,61 +2059,61 @@
                 }
             }
         }
         var ft = ["Webkit", "Moz", "ms"],
             Nr = D.createElement("div").style,
             Ir = {};
 
-        function dm(a) {
+        function pm(a) {
             for (var c = a[0].toUpperCase() + a.slice(1), d = ft.length; d--;)
                 if (a = ft[d] + c, a in Nr) return a
         }
 
         function Pl(a) {
             var c = p.cssProps[a] || Ir[a];
-            return c || (a in Nr ? a : Ir[a] = dm(a) || a)
+            return c || (a in Nr ? a : Ir[a] = pm(a) || a)
         }
-        var pm = /^(none|table(?!-c[ea]).+)/,
-            gm = {
+        var gm = /^(none|table(?!-c[ea]).+)/,
+            mm = {
                 position: "absolute",
                 visibility: "hidden",
                 display: "block"
             },
             yc = {
                 letterSpacing: "0",
                 fontWeight: "400"
             };
 
         function bc(a, c, d) {
-            var m = Jt.exec(c);
-            return m ? Math.max(0, m[2] - (d || 0)) + (m[3] || "px") : c
+            var g = Jt.exec(c);
+            return g ? Math.max(0, g[2] - (d || 0)) + (g[3] || "px") : c
         }
 
-        function Nl(a, c, d, m, b, x) {
+        function Nl(a, c, d, g, b, x) {
             var w = c === "width" ? 1 : 0,
                 T = 0,
-                A = 0,
+                C = 0,
                 E = 0;
-            if (d === (m ? "border" : "content")) return 0;
-            for (; w < 4; w += 2) d === "margin" && (E += p.css(a, d + Ft[w], !0, b)), m ? (d === "content" && (A -= p.css(a, "padding" + Ft[w], !0, b)), d !== "margin" && (A -= p.css(a, "border" + Ft[w] + "Width", !0, b))) : (A += p.css(a, "padding" + Ft[w], !0, b), d !== "padding" ? A += p.css(a, "border" + Ft[w] + "Width", !0, b) : T += p.css(a, "border" + Ft[w] + "Width", !0, b));
-            return !m && x >= 0 && (A += Math.max(0, Math.ceil(a["offset" + c[0].toUpperCase() + c.slice(1)] - x - A - T - .5)) || 0), A + E
+            if (d === (g ? "border" : "content")) return 0;
+            for (; w < 4; w += 2) d === "margin" && (E += p.css(a, d + Ft[w], !0, b)), g ? (d === "content" && (C -= p.css(a, "padding" + Ft[w], !0, b)), d !== "margin" && (C -= p.css(a, "border" + Ft[w] + "Width", !0, b))) : (C += p.css(a, "padding" + Ft[w], !0, b), d !== "padding" ? C += p.css(a, "border" + Ft[w] + "Width", !0, b) : T += p.css(a, "border" + Ft[w] + "Width", !0, b));
+            return !g && x >= 0 && (C += Math.max(0, Math.ceil(a["offset" + c[0].toUpperCase() + c.slice(1)] - x - C - T - .5)) || 0), C + E
         }
 
         function xc(a, c, d) {
-            var m = Ke(a),
+            var g = Ke(a),
                 b = !v.boxSizingReliable() || d,
-                x = b && p.css(a, "boxSizing", !1, m) === "border-box",
+                x = b && p.css(a, "boxSizing", !1, g) === "border-box",
                 w = x,
-                T = zt(a, c, m),
-                A = "offset" + c[0].toUpperCase() + c.slice(1);
+                T = zt(a, c, g),
+                C = "offset" + c[0].toUpperCase() + c.slice(1);
             if (Y.test(T)) {
                 if (!d) return T;
                 T = "auto"
             }
-            return (!v.boxSizingReliable() && x || !v.reliableTrDimensions() && J(a, "tr") || T === "auto" || !parseFloat(T) && p.css(a, "display", !1, m) === "inline") && a.getClientRects().length && (x = p.css(a, "boxSizing", !1, m) === "border-box", w = A in a, w && (T = a[A])), T = parseFloat(T) || 0, T + Nl(a, c, d || (x ? "border" : "content"), w, m, T) + "px"
+            return (!v.boxSizingReliable() && x || !v.reliableTrDimensions() && J(a, "tr") || T === "auto" || !parseFloat(T) && p.css(a, "display", !1, g) === "inline") && a.getClientRects().length && (x = p.css(a, "boxSizing", !1, g) === "border-box", w = C in a, w && (T = a[C])), T = parseFloat(T) || 0, T + Nl(a, c, d || (x ? "border" : "content"), w, g, T) + "px"
         }
         p.extend({
             cssHooks: {
                 opacity: {
                     get: function(a, c) {
                         if (c) {
                             var d = zt(a, "opacity");
@@ -2148,44 +2148,44 @@
                 fillOpacity: !0,
                 floodOpacity: !0,
                 stopOpacity: !0,
                 strokeMiterlimit: !0,
                 strokeOpacity: !0
             },
             cssProps: {},
-            style: function(a, c, d, m) {
+            style: function(a, c, d, g) {
                 if (!(!a || a.nodeType === 3 || a.nodeType === 8 || !a.style)) {
                     var b, x, w, T = ht(c),
-                        A = Re.test(c),
+                        C = Re.test(c),
                         E = a.style;
-                    if (A || (c = Pl(T)), w = p.cssHooks[c] || p.cssHooks[T], d !== void 0) {
+                    if (C || (c = Pl(T)), w = p.cssHooks[c] || p.cssHooks[T], d !== void 0) {
                         if (x = typeof d, x === "string" && (b = Jt.exec(d)) && b[1] && (d = Hs(a, c, b), x = "number"), d == null || d !== d) return;
-                        x === "number" && !A && (d += b && b[3] || (p.cssNumber[T] ? "" : "px")), !v.clearCloneStyle && d === "" && c.indexOf("background") === 0 && (E[c] = "inherit"), (!w || !("set" in w) || (d = w.set(a, d, m)) !== void 0) && (A ? E.setProperty(c, d) : E[c] = d)
-                    } else return w && "get" in w && (b = w.get(a, !1, m)) !== void 0 ? b : E[c]
+                        x === "number" && !C && (d += b && b[3] || (p.cssNumber[T] ? "" : "px")), !v.clearCloneStyle && d === "" && c.indexOf("background") === 0 && (E[c] = "inherit"), (!w || !("set" in w) || (d = w.set(a, d, g)) !== void 0) && (C ? E.setProperty(c, d) : E[c] = d)
+                    } else return w && "get" in w && (b = w.get(a, !1, g)) !== void 0 ? b : E[c]
                 }
             },
-            css: function(a, c, d, m) {
+            css: function(a, c, d, g) {
                 var b, x, w, T = ht(c),
-                    A = Re.test(c);
-                return A || (c = Pl(T)), w = p.cssHooks[c] || p.cssHooks[T], w && "get" in w && (b = w.get(a, !0, d)), b === void 0 && (b = zt(a, c, m)), b === "normal" && c in yc && (b = yc[c]), d === "" || d ? (x = parseFloat(b), d === !0 || isFinite(x) ? x || 0 : b) : b
+                    C = Re.test(c);
+                return C || (c = Pl(T)), w = p.cssHooks[c] || p.cssHooks[T], w && "get" in w && (b = w.get(a, !0, d)), b === void 0 && (b = zt(a, c, g)), b === "normal" && c in yc && (b = yc[c]), d === "" || d ? (x = parseFloat(b), d === !0 || isFinite(x) ? x || 0 : b) : b
             }
         }), p.each(["height", "width"], function(a, c) {
             p.cssHooks[c] = {
-                get: function(d, m, b) {
-                    if (m) return pm.test(p.css(d, "display")) && (!d.getClientRects().length || !d.getBoundingClientRect().width) ? Ze(d, gm, function() {
+                get: function(d, g, b) {
+                    if (g) return gm.test(p.css(d, "display")) && (!d.getClientRects().length || !d.getBoundingClientRect().width) ? Ze(d, mm, function() {
                         return xc(d, c, b)
                     }) : xc(d, c, b)
                 },
-                set: function(d, m, b) {
+                set: function(d, g, b) {
                     var x, w = Ke(d),
                         T = !v.scrollboxSize() && w.position === "absolute",
-                        A = T || b,
-                        E = A && p.css(d, "boxSizing", !1, w) === "border-box",
+                        C = T || b,
+                        E = C && p.css(d, "boxSizing", !1, w) === "border-box",
                         I = b ? Nl(d, c, b, E, w) : 0;
-                    return E && T && (I -= Math.ceil(d["offset" + c[0].toUpperCase() + c.slice(1)] - parseFloat(w[c]) - Nl(d, c, "border", !1, w) - .5)), I && (x = Jt.exec(m)) && (x[3] || "px") !== "px" && (d.style[c] = m, m = p.css(d, c)), bc(d, m, I)
+                    return E && T && (I -= Math.ceil(d["offset" + c[0].toUpperCase() + c.slice(1)] - parseFloat(w[c]) - Nl(d, c, "border", !1, w) - .5)), I && (x = Jt.exec(g)) && (x[3] || "px") !== "px" && (d.style[c] = g, g = p.css(d, c)), bc(d, g, I)
                 }
             }
         }), p.cssHooks.marginLeft = sn(v.reliableMarginLeft, function(a, c) {
             if (c) return (parseFloat(zt(a, "marginLeft")) || a.getBoundingClientRect().left - Ze(a, {
                 marginLeft: 0
             }, function() {
                 return a.getBoundingClientRect().left
@@ -2193,39 +2193,39 @@
         }), p.each({
             margin: "",
             padding: "",
             border: "Width"
         }, function(a, c) {
             p.cssHooks[a + c] = {
                 expand: function(d) {
-                    for (var m = 0, b = {}, x = typeof d == "string" ? d.split(" ") : [d]; m < 4; m++) b[a + Ft[m] + c] = x[m] || x[m - 2] || x[0];
+                    for (var g = 0, b = {}, x = typeof d == "string" ? d.split(" ") : [d]; g < 4; g++) b[a + Ft[g] + c] = x[g] || x[g - 2] || x[0];
                     return b
                 }
             }, a !== "margin" && (p.cssHooks[a + c].set = bc)
         }), p.fn.extend({
             css: function(a, c) {
-                return Kt(this, function(d, m, b) {
+                return Kt(this, function(d, g, b) {
                     var x, w, T = {},
-                        A = 0;
-                    if (Array.isArray(m)) {
-                        for (x = Ke(d), w = m.length; A < w; A++) T[m[A]] = p.css(d, m[A], !1, x);
+                        C = 0;
+                    if (Array.isArray(g)) {
+                        for (x = Ke(d), w = g.length; C < w; C++) T[g[C]] = p.css(d, g[C], !1, x);
                         return T
                     }
-                    return b !== void 0 ? p.style(d, m, b) : p.css(d, m)
+                    return b !== void 0 ? p.style(d, g, b) : p.css(d, g)
                 }, a, c, arguments.length > 1)
             }
         });
 
-        function Pt(a, c, d, m, b) {
-            return new Pt.prototype.init(a, c, d, m, b)
+        function Pt(a, c, d, g, b) {
+            return new Pt.prototype.init(a, c, d, g, b)
         }
         p.Tween = Pt, Pt.prototype = {
             constructor: Pt,
-            init: function(a, c, d, m, b, x) {
-                this.elem = a, this.prop = d, this.easing = b || p.easing._default, this.options = c, this.start = this.now = this.cur(), this.end = m, this.unit = x || (p.cssNumber[d] ? "" : "px")
+            init: function(a, c, d, g, b, x) {
+                this.elem = a, this.prop = d, this.easing = b || p.easing._default, this.options = c, this.start = this.now = this.cur(), this.end = g, this.unit = x || (p.cssNumber[d] ? "" : "px")
             },
             cur: function() {
                 var a = Pt.propHooks[this.prop];
                 return a && a.get ? a.get(this) : Pt.propHooks._default.get(this)
             },
             run: function(a) {
                 var c, d = Pt.propHooks[this.prop];
@@ -2250,94 +2250,94 @@
                 return a
             },
             swing: function(a) {
                 return .5 - Math.cos(a * Math.PI) / 2
             },
             _default: "swing"
         }, p.fx = Pt.prototype.init, p.fx.step = {};
-        var rr, Us, mm = /^(?:toggle|show|hide)$/,
-            ym = /queueHooks$/;
+        var rr, Us, ym = /^(?:toggle|show|hide)$/,
+            bm = /queueHooks$/;
 
         function Il() {
             Us && (D.hidden === !1 && e.requestAnimationFrame ? e.requestAnimationFrame(Il) : e.setTimeout(Il, p.fx.interval), p.fx.tick())
         }
 
         function kc() {
             return e.setTimeout(function() {
                 rr = void 0
             }), rr = Date.now()
         }
 
         function Qs(a, c) {
-            var d, m = 0,
+            var d, g = 0,
                 b = {
                     height: a
                 };
-            for (c = c ? 1 : 0; m < 4; m += 2 - c) d = Ft[m], b["margin" + d] = b["padding" + d] = a;
+            for (c = c ? 1 : 0; g < 4; g += 2 - c) d = Ft[g], b["margin" + d] = b["padding" + d] = a;
             return c && (b.opacity = b.width = a), b
         }
 
         function wc(a, c, d) {
-            for (var m, b = (ci.tweeners[c] || []).concat(ci.tweeners["*"]), x = 0, w = b.length; x < w; x++)
-                if (m = b[x].call(d, c, a)) return m
+            for (var g, b = (ci.tweeners[c] || []).concat(ci.tweeners["*"]), x = 0, w = b.length; x < w; x++)
+                if (g = b[x].call(d, c, a)) return g
         }
 
-        function bm(a, c, d) {
-            var m, b, x, w, T, A, E, I, _ = "width" in c || "height" in c,
+        function xm(a, c, d) {
+            var g, b, x, w, T, C, E, I, _ = "width" in c || "height" in c,
                 P = this,
                 W = {},
                 ce = a.style,
-                Te = a.nodeType && Zn(a),
+                Ae = a.nodeType && Zn(a),
                 ge = ne.get(a, "fxshow");
             d.queue || (w = p._queueHooks(a, "fx"), w.unqueued == null && (w.unqueued = 0, T = w.empty.fire, w.empty.fire = function() {
                 w.unqueued || T()
             }), w.unqueued++, P.always(function() {
                 P.always(function() {
                     w.unqueued--, p.queue(a, "fx").length || w.empty.fire()
                 })
             }));
-            for (m in c)
-                if (b = c[m], mm.test(b)) {
-                    if (delete c[m], x = x || b === "toggle", b === (Te ? "hide" : "show"))
-                        if (b === "show" && ge && ge[m] !== void 0) Te = !0;
+            for (g in c)
+                if (b = c[g], ym.test(b)) {
+                    if (delete c[g], x = x || b === "toggle", b === (Ae ? "hide" : "show"))
+                        if (b === "show" && ge && ge[g] !== void 0) Ae = !0;
                         else continue;
-                    W[m] = ge && ge[m] || p.style(a, m)
-                } if (A = !p.isEmptyObject(c), !(!A && p.isEmptyObject(W))) {
-                _ && a.nodeType === 1 && (d.overflow = [ce.overflow, ce.overflowX, ce.overflowY], E = ge && ge.display, E == null && (E = ne.get(a, "display")), I = p.css(a, "display"), I === "none" && (E ? I = E : (nn([a], !0), E = a.style.display || E, I = p.css(a, "display"), nn([a]))), (I === "inline" || I === "inline-block" && E != null) && p.css(a, "float") === "none" && (A || (P.done(function() {
+                    W[g] = ge && ge[g] || p.style(a, g)
+                } if (C = !p.isEmptyObject(c), !(!C && p.isEmptyObject(W))) {
+                _ && a.nodeType === 1 && (d.overflow = [ce.overflow, ce.overflowX, ce.overflowY], E = ge && ge.display, E == null && (E = ne.get(a, "display")), I = p.css(a, "display"), I === "none" && (E ? I = E : (nn([a], !0), E = a.style.display || E, I = p.css(a, "display"), nn([a]))), (I === "inline" || I === "inline-block" && E != null) && p.css(a, "float") === "none" && (C || (P.done(function() {
                     ce.display = E
                 }), E == null && (I = ce.display, E = I === "none" ? "" : I)), ce.display = "inline-block")), d.overflow && (ce.overflow = "hidden", P.always(function() {
                     ce.overflow = d.overflow[0], ce.overflowX = d.overflow[1], ce.overflowY = d.overflow[2]
-                })), A = !1;
-                for (m in W) A || (ge ? "hidden" in ge && (Te = ge.hidden) : ge = ne.access(a, "fxshow", {
+                })), C = !1;
+                for (g in W) C || (ge ? "hidden" in ge && (Ae = ge.hidden) : ge = ne.access(a, "fxshow", {
                     display: E
-                }), x && (ge.hidden = !Te), Te && nn([a], !0), P.done(function() {
-                    Te || nn([a]), ne.remove(a, "fxshow");
-                    for (m in W) p.style(a, m, W[m])
-                })), A = wc(Te ? ge[m] : 0, m, P), m in ge || (ge[m] = A.start, Te && (A.end = A.start, A.start = 0))
+                }), x && (ge.hidden = !Ae), Ae && nn([a], !0), P.done(function() {
+                    Ae || nn([a]), ne.remove(a, "fxshow");
+                    for (g in W) p.style(a, g, W[g])
+                })), C = wc(Ae ? ge[g] : 0, g, P), g in ge || (ge[g] = C.start, Ae && (C.end = C.start, C.start = 0))
             }
         }
 
-        function xm(a, c) {
-            var d, m, b, x, w;
+        function km(a, c) {
+            var d, g, b, x, w;
             for (d in a)
-                if (m = ht(d), b = c[m], x = a[d], Array.isArray(x) && (b = x[1], x = a[d] = x[0]), d !== m && (a[m] = x, delete a[d]), w = p.cssHooks[m], w && "expand" in w) {
-                    x = w.expand(x), delete a[m];
+                if (g = ht(d), b = c[g], x = a[d], Array.isArray(x) && (b = x[1], x = a[d] = x[0]), d !== g && (a[g] = x, delete a[d]), w = p.cssHooks[g], w && "expand" in w) {
+                    x = w.expand(x), delete a[g];
                     for (d in x) d in a || (a[d] = x[d], c[d] = b)
-                } else c[m] = b
+                } else c[g] = b
         }
 
         function ci(a, c, d) {
-            var m, b, x = 0,
+            var g, b, x = 0,
                 w = ci.prefilters.length,
                 T = p.Deferred().always(function() {
-                    delete A.elem
+                    delete C.elem
                 }),
-                A = function() {
+                C = function() {
                     if (b) return !1;
-                    for (var _ = rr || kc(), P = Math.max(0, E.startTime + E.duration - _), W = P / E.duration || 0, ce = 1 - W, Te = 0, ge = E.tweens.length; Te < ge; Te++) E.tweens[Te].run(ce);
+                    for (var _ = rr || kc(), P = Math.max(0, E.startTime + E.duration - _), W = P / E.duration || 0, ce = 1 - W, Ae = 0, ge = E.tweens.length; Ae < ge; Ae++) E.tweens[Ae].run(ce);
                     return T.notifyWith(a, [E, ce, P]), ce < 1 && ge ? P : (ge || T.notifyWith(a, [E, 1, 0]), T.resolveWith(a, [E]), !1)
                 },
                 E = T.promise({
                     elem: a,
                     props: p.extend({}, c),
                     opts: p.extend(!0, {
                         specialEasing: {},
@@ -2357,94 +2357,94 @@
                             W = _ ? E.tweens.length : 0;
                         if (b) return this;
                         for (b = !0; P < W; P++) E.tweens[P].run(1);
                         return _ ? (T.notifyWith(a, [E, 1, 0]), T.resolveWith(a, [E, _])) : T.rejectWith(a, [E, _]), this
                     }
                 }),
                 I = E.props;
-            for (xm(I, E.opts.specialEasing); x < w; x++)
-                if (m = ci.prefilters[x].call(E, a, I, E.opts), m) return C(m.stop) && (p._queueHooks(E.elem, E.opts.queue).stop = m.stop.bind(m)), m;
-            return p.map(I, wc, E), C(E.opts.start) && E.opts.start.call(a, E), E.progress(E.opts.progress).done(E.opts.done, E.opts.complete).fail(E.opts.fail).always(E.opts.always), p.fx.timer(p.extend(A, {
+            for (km(I, E.opts.specialEasing); x < w; x++)
+                if (g = ci.prefilters[x].call(E, a, I, E.opts), g) return A(g.stop) && (p._queueHooks(E.elem, E.opts.queue).stop = g.stop.bind(g)), g;
+            return p.map(I, wc, E), A(E.opts.start) && E.opts.start.call(a, E), E.progress(E.opts.progress).done(E.opts.done, E.opts.complete).fail(E.opts.fail).always(E.opts.always), p.fx.timer(p.extend(C, {
                 elem: a,
                 anim: E,
                 queue: E.opts.queue
             })), E
         }
         p.Animation = p.extend(ci, {
                 tweeners: {
                     "*": [function(a, c) {
                         var d = this.createTween(a, c);
                         return Hs(d.elem, a, Jt.exec(c), d), d
                     }]
                 },
                 tweener: function(a, c) {
-                    C(a) ? (c = a, a = ["*"]) : a = a.match(at);
-                    for (var d, m = 0, b = a.length; m < b; m++) d = a[m], ci.tweeners[d] = ci.tweeners[d] || [], ci.tweeners[d].unshift(c)
+                    A(a) ? (c = a, a = ["*"]) : a = a.match(at);
+                    for (var d, g = 0, b = a.length; g < b; g++) d = a[g], ci.tweeners[d] = ci.tweeners[d] || [], ci.tweeners[d].unshift(c)
                 },
-                prefilters: [bm],
+                prefilters: [xm],
                 prefilter: function(a, c) {
                     c ? ci.prefilters.unshift(a) : ci.prefilters.push(a)
                 }
             }), p.speed = function(a, c, d) {
-                var m = a && typeof a == "object" ? p.extend({}, a) : {
-                    complete: d || !d && c || C(a) && a,
+                var g = a && typeof a == "object" ? p.extend({}, a) : {
+                    complete: d || !d && c || A(a) && a,
                     duration: a,
-                    easing: d && c || c && !C(c) && c
+                    easing: d && c || c && !A(c) && c
                 };
-                return p.fx.off ? m.duration = 0 : typeof m.duration != "number" && (m.duration in p.fx.speeds ? m.duration = p.fx.speeds[m.duration] : m.duration = p.fx.speeds._default), (m.queue == null || m.queue === !0) && (m.queue = "fx"), m.old = m.complete, m.complete = function() {
-                    C(m.old) && m.old.call(this), m.queue && p.dequeue(this, m.queue)
-                }, m
+                return p.fx.off ? g.duration = 0 : typeof g.duration != "number" && (g.duration in p.fx.speeds ? g.duration = p.fx.speeds[g.duration] : g.duration = p.fx.speeds._default), (g.queue == null || g.queue === !0) && (g.queue = "fx"), g.old = g.complete, g.complete = function() {
+                    A(g.old) && g.old.call(this), g.queue && p.dequeue(this, g.queue)
+                }, g
             }, p.fn.extend({
-                fadeTo: function(a, c, d, m) {
+                fadeTo: function(a, c, d, g) {
                     return this.filter(Zn).css("opacity", 0).show().end().animate({
                         opacity: c
-                    }, a, d, m)
+                    }, a, d, g)
                 },
-                animate: function(a, c, d, m) {
+                animate: function(a, c, d, g) {
                     var b = p.isEmptyObject(a),
-                        x = p.speed(c, d, m),
+                        x = p.speed(c, d, g),
                         w = function() {
                             var T = ci(this, p.extend({}, a), x);
                             (b || ne.get(this, "finish")) && T.stop(!0)
                         };
                     return w.finish = w, b || x.queue === !1 ? this.each(w) : this.queue(x.queue, w)
                 },
                 stop: function(a, c, d) {
-                    var m = function(b) {
+                    var g = function(b) {
                         var x = b.stop;
                         delete b.stop, x(d)
                     };
                     return typeof a != "string" && (d = c, c = a, a = void 0), c && this.queue(a || "fx", []), this.each(function() {
                         var b = !0,
                             x = a != null && a + "queueHooks",
                             w = p.timers,
                             T = ne.get(this);
-                        if (x) T[x] && T[x].stop && m(T[x]);
+                        if (x) T[x] && T[x].stop && g(T[x]);
                         else
-                            for (x in T) T[x] && T[x].stop && ym.test(x) && m(T[x]);
+                            for (x in T) T[x] && T[x].stop && bm.test(x) && g(T[x]);
                         for (x = w.length; x--;) w[x].elem === this && (a == null || w[x].queue === a) && (w[x].anim.stop(d), b = !1, w.splice(x, 1));
                         (b || !d) && p.dequeue(this, a)
                     })
                 },
                 finish: function(a) {
                     return a !== !1 && (a = a || "fx"), this.each(function() {
                         var c, d = ne.get(this),
-                            m = d[a + "queue"],
+                            g = d[a + "queue"],
                             b = d[a + "queueHooks"],
                             x = p.timers,
-                            w = m ? m.length : 0;
+                            w = g ? g.length : 0;
                         for (d.finish = !0, p.queue(this, a, []), b && b.stop && b.stop.call(this, !0), c = x.length; c--;) x[c].elem === this && x[c].queue === a && (x[c].anim.stop(!0), x.splice(c, 1));
-                        for (c = 0; c < w; c++) m[c] && m[c].finish && m[c].finish.call(this);
+                        for (c = 0; c < w; c++) g[c] && g[c].finish && g[c].finish.call(this);
                         delete d.finish
                     })
                 }
             }), p.each(["toggle", "show", "hide"], function(a, c) {
                 var d = p.fn[c];
-                p.fn[c] = function(m, b, x) {
-                    return m == null || typeof m == "boolean" ? d.apply(this, arguments) : this.animate(Qs(c, !0), m, b, x)
+                p.fn[c] = function(g, b, x) {
+                    return g == null || typeof g == "boolean" ? d.apply(this, arguments) : this.animate(Qs(c, !0), g, b, x)
                 }
             }), p.each({
                 slideDown: Qs("show"),
                 slideUp: Qs("hide"),
                 slideToggle: Qs("toggle"),
                 fadeIn: {
                     opacity: "show"
@@ -2452,16 +2452,16 @@
                 fadeOut: {
                     opacity: "hide"
                 },
                 fadeToggle: {
                     opacity: "toggle"
                 }
             }, function(a, c) {
-                p.fn[a] = function(d, m, b) {
-                    return this.animate(c, d, m, b)
+                p.fn[a] = function(d, g, b) {
+                    return this.animate(c, d, g, b)
                 }
             }), p.timers = [], p.fx.tick = function() {
                 var a, c = 0,
                     d = p.timers;
                 for (rr = Date.now(); c < d.length; c++) a = d[c], !a() && d[c] === a && d.splice(c--, 1);
                 d.length || p.fx.stop(), rr = void 0
             }, p.fx.timer = function(a) {
@@ -2471,17 +2471,17 @@
             }, p.fx.stop = function() {
                 Us = null
             }, p.fx.speeds = {
                 slow: 600,
                 fast: 200,
                 _default: 400
             }, p.fn.delay = function(a, c) {
-                return a = p.fx && p.fx.speeds[a] || a, c = c || "fx", this.queue(c, function(d, m) {
+                return a = p.fx && p.fx.speeds[a] || a, c = c || "fx", this.queue(c, function(d, g) {
                     var b = e.setTimeout(d, a);
-                    m.stop = function() {
+                    g.stop = function() {
                         e.clearTimeout(b)
                     }
                 })
             },
             function() {
                 var a = D.createElement("input"),
                     c = D.createElement("select"),
@@ -2496,75 +2496,75 @@
             removeAttr: function(a) {
                 return this.each(function() {
                     p.removeAttr(this, a)
                 })
             }
         }), p.extend({
             attr: function(a, c, d) {
-                var m, b, x = a.nodeType;
+                var g, b, x = a.nodeType;
                 if (!(x === 3 || x === 8 || x === 2)) {
                     if (typeof a.getAttribute == "undefined") return p.prop(a, c, d);
                     if ((x !== 1 || !p.isXMLDoc(a)) && (b = p.attrHooks[c.toLowerCase()] || (p.expr.match.bool.test(c) ? vc : void 0)), d !== void 0) {
                         if (d === null) {
                             p.removeAttr(a, c);
                             return
                         }
-                        return b && "set" in b && (m = b.set(a, d, c)) !== void 0 ? m : (a.setAttribute(c, d + ""), d)
+                        return b && "set" in b && (g = b.set(a, d, c)) !== void 0 ? g : (a.setAttribute(c, d + ""), d)
                     }
-                    return b && "get" in b && (m = b.get(a, c)) !== null ? m : (m = p.find.attr(a, c), m == null ? void 0 : m)
+                    return b && "get" in b && (g = b.get(a, c)) !== null ? g : (g = p.find.attr(a, c), g == null ? void 0 : g)
                 }
             },
             attrHooks: {
                 type: {
                     set: function(a, c) {
                         if (!v.radioValue && c === "radio" && J(a, "input")) {
                             var d = a.value;
                             return a.setAttribute("type", c), d && (a.value = d), c
                         }
                     }
                 }
             },
             removeAttr: function(a, c) {
-                var d, m = 0,
+                var d, g = 0,
                     b = c && c.match(at);
                 if (b && a.nodeType === 1)
-                    for (; d = b[m++];) a.removeAttribute(d)
+                    for (; d = b[g++];) a.removeAttribute(d)
             }
         }), vc = {
             set: function(a, c, d) {
                 return c === !1 ? p.removeAttr(a, d) : a.setAttribute(d, d), d
             }
         }, p.each(p.expr.match.bool.source.match(/\w+/g), function(a, c) {
             var d = Br[c] || p.find.attr;
-            Br[c] = function(m, b, x) {
-                var w, T, A = b.toLowerCase();
-                return x || (T = Br[A], Br[A] = w, w = d(m, b, x) != null ? A : null, Br[A] = T), w
+            Br[c] = function(g, b, x) {
+                var w, T, C = b.toLowerCase();
+                return x || (T = Br[C], Br[C] = w, w = d(g, b, x) != null ? C : null, Br[C] = T), w
             }
         });
-        var km = /^(?:input|select|textarea|button)$/i,
-            wm = /^(?:a|area)$/i;
+        var wm = /^(?:input|select|textarea|button)$/i,
+            vm = /^(?:a|area)$/i;
         p.fn.extend({
             prop: function(a, c) {
                 return Kt(this, p.prop, a, c, arguments.length > 1)
             },
             removeProp: function(a) {
                 return this.each(function() {
                     delete this[p.propFix[a] || a]
                 })
             }
         }), p.extend({
             prop: function(a, c, d) {
-                var m, b, x = a.nodeType;
-                if (!(x === 3 || x === 8 || x === 2)) return (x !== 1 || !p.isXMLDoc(a)) && (c = p.propFix[c] || c, b = p.propHooks[c]), d !== void 0 ? b && "set" in b && (m = b.set(a, d, c)) !== void 0 ? m : a[c] = d : b && "get" in b && (m = b.get(a, c)) !== null ? m : a[c]
+                var g, b, x = a.nodeType;
+                if (!(x === 3 || x === 8 || x === 2)) return (x !== 1 || !p.isXMLDoc(a)) && (c = p.propFix[c] || c, b = p.propHooks[c]), d !== void 0 ? b && "set" in b && (g = b.set(a, d, c)) !== void 0 ? g : a[c] = d : b && "get" in b && (g = b.get(a, c)) !== null ? g : a[c]
             },
             propHooks: {
                 tabIndex: {
                     get: function(a) {
                         var c = p.find.attr(a, "tabindex");
-                        return c ? parseInt(c, 10) : km.test(a.nodeName) || wm.test(a.nodeName) && a.href ? 0 : -1
+                        return c ? parseInt(c, 10) : wm.test(a.nodeName) || vm.test(a.nodeName) && a.href ? 0 : -1
                     }
                 }
             },
             propFix: {
                 for: "htmlFor",
                 class: "className"
             }
@@ -2591,88 +2591,88 @@
         }
 
         function Bl(a) {
             return Array.isArray(a) ? a : typeof a == "string" ? a.match(at) || [] : []
         }
         p.fn.extend({
             addClass: function(a) {
-                var c, d, m, b, x, w;
-                return C(a) ? this.each(function(T) {
+                var c, d, g, b, x, w;
+                return A(a) ? this.each(function(T) {
                     p(this).addClass(a.call(this, T, Pn(this)))
                 }) : (c = Bl(a), c.length ? this.each(function() {
-                    if (m = Pn(this), d = this.nodeType === 1 && " " + Ln(m) + " ", d) {
+                    if (g = Pn(this), d = this.nodeType === 1 && " " + Ln(g) + " ", d) {
                         for (x = 0; x < c.length; x++) b = c[x], d.indexOf(" " + b + " ") < 0 && (d += b + " ");
-                        w = Ln(d), m !== w && this.setAttribute("class", w)
+                        w = Ln(d), g !== w && this.setAttribute("class", w)
                     }
                 }) : this)
             },
             removeClass: function(a) {
-                var c, d, m, b, x, w;
-                return C(a) ? this.each(function(T) {
+                var c, d, g, b, x, w;
+                return A(a) ? this.each(function(T) {
                     p(this).removeClass(a.call(this, T, Pn(this)))
                 }) : arguments.length ? (c = Bl(a), c.length ? this.each(function() {
-                    if (m = Pn(this), d = this.nodeType === 1 && " " + Ln(m) + " ", d) {
+                    if (g = Pn(this), d = this.nodeType === 1 && " " + Ln(g) + " ", d) {
                         for (x = 0; x < c.length; x++)
                             for (b = c[x]; d.indexOf(" " + b + " ") > -1;) d = d.replace(" " + b + " ", " ");
-                        w = Ln(d), m !== w && this.setAttribute("class", w)
+                        w = Ln(d), g !== w && this.setAttribute("class", w)
                     }
                 }) : this) : this.attr("class", "")
             },
             toggleClass: function(a, c) {
-                var d, m, b, x, w = typeof a,
+                var d, g, b, x, w = typeof a,
                     T = w === "string" || Array.isArray(a);
-                return C(a) ? this.each(function(A) {
-                    p(this).toggleClass(a.call(this, A, Pn(this), c), c)
+                return A(a) ? this.each(function(C) {
+                    p(this).toggleClass(a.call(this, C, Pn(this), c), c)
                 }) : typeof c == "boolean" && T ? c ? this.addClass(a) : this.removeClass(a) : (d = Bl(a), this.each(function() {
                     if (T)
-                        for (x = p(this), b = 0; b < d.length; b++) m = d[b], x.hasClass(m) ? x.removeClass(m) : x.addClass(m);
-                    else(a === void 0 || w === "boolean") && (m = Pn(this), m && ne.set(this, "__className__", m), this.setAttribute && this.setAttribute("class", m || a === !1 ? "" : ne.get(this, "__className__") || ""))
+                        for (x = p(this), b = 0; b < d.length; b++) g = d[b], x.hasClass(g) ? x.removeClass(g) : x.addClass(g);
+                    else(a === void 0 || w === "boolean") && (g = Pn(this), g && ne.set(this, "__className__", g), this.setAttribute && this.setAttribute("class", g || a === !1 ? "" : ne.get(this, "__className__") || ""))
                 }))
             },
             hasClass: function(a) {
-                var c, d, m = 0;
-                for (c = " " + a + " "; d = this[m++];)
+                var c, d, g = 0;
+                for (c = " " + a + " "; d = this[g++];)
                     if (d.nodeType === 1 && (" " + Ln(Pn(d)) + " ").indexOf(c) > -1) return !0;
                 return !1
             }
         });
-        var vm = /\r/g;
+        var Sm = /\r/g;
         p.fn.extend({
             val: function(a) {
-                var c, d, m, b = this[0];
-                return arguments.length ? (m = C(a), this.each(function(x) {
+                var c, d, g, b = this[0];
+                return arguments.length ? (g = A(a), this.each(function(x) {
                     var w;
-                    this.nodeType === 1 && (m ? w = a.call(this, x, p(this).val()) : w = a, w == null ? w = "" : typeof w == "number" ? w += "" : Array.isArray(w) && (w = p.map(w, function(T) {
+                    this.nodeType === 1 && (g ? w = a.call(this, x, p(this).val()) : w = a, w == null ? w = "" : typeof w == "number" ? w += "" : Array.isArray(w) && (w = p.map(w, function(T) {
                         return T == null ? "" : T + ""
                     })), c = p.valHooks[this.type] || p.valHooks[this.nodeName.toLowerCase()], (!c || !("set" in c) || c.set(this, w, "value") === void 0) && (this.value = w))
-                })) : b ? (c = p.valHooks[b.type] || p.valHooks[b.nodeName.toLowerCase()], c && "get" in c && (d = c.get(b, "value")) !== void 0 ? d : (d = b.value, typeof d == "string" ? d.replace(vm, "") : d == null ? "" : d)) : void 0
+                })) : b ? (c = p.valHooks[b.type] || p.valHooks[b.nodeName.toLowerCase()], c && "get" in c && (d = c.get(b, "value")) !== void 0 ? d : (d = b.value, typeof d == "string" ? d.replace(Sm, "") : d == null ? "" : d)) : void 0
             }
         }), p.extend({
             valHooks: {
                 option: {
                     get: function(a) {
                         var c = p.find.attr(a, "value");
                         return c != null ? c : Ln(p.text(a))
                     }
                 },
                 select: {
                     get: function(a) {
-                        var c, d, m, b = a.options,
+                        var c, d, g, b = a.options,
                             x = a.selectedIndex,
                             w = a.type === "select-one",
                             T = w ? null : [],
-                            A = w ? x + 1 : b.length;
-                        for (x < 0 ? m = A : m = w ? x : 0; m < A; m++)
-                            if (d = b[m], (d.selected || m === x) && !d.disabled && (!d.parentNode.disabled || !J(d.parentNode, "optgroup"))) {
+                            C = w ? x + 1 : b.length;
+                        for (x < 0 ? g = C : g = w ? x : 0; g < C; g++)
+                            if (d = b[g], (d.selected || g === x) && !d.disabled && (!d.parentNode.disabled || !J(d.parentNode, "optgroup"))) {
                                 if (c = p(d).val(), w) return c;
                                 T.push(c)
                             } return T
                     },
                     set: function(a, c) {
-                        for (var d, m, b = a.options, x = p.makeArray(c), w = b.length; w--;) m = b[w], (m.selected = p.inArray(p.valHooks.option.get(m), x) > -1) && (d = !0);
+                        for (var d, g, b = a.options, x = p.makeArray(c), w = b.length; w--;) g = b[w], (g.selected = p.inArray(p.valHooks.option.get(g), x) > -1) && (d = !0);
                         return d || (a.selectedIndex = -1), x
                     }
                 }
             }
         }), p.each(["radio", "checkbox"], function() {
             p.valHooks[this] = {
                 set: function(a, c) {
@@ -2688,202 +2688,202 @@
             },
             _l = /\?/;
         p.parseXML = function(a) {
             var c, d;
             if (!a || typeof a != "string") return null;
             try {
                 c = new e.DOMParser().parseFromString(a, "text/xml")
-            } catch (m) {}
-            return d = c && c.getElementsByTagName("parsererror")[0], (!c || d) && p.error("Invalid XML: " + (d ? p.map(d.childNodes, function(m) {
-                return m.textContent
+            } catch (g) {}
+            return d = c && c.getElementsByTagName("parsererror")[0], (!c || d) && p.error("Invalid XML: " + (d ? p.map(d.childNodes, function(g) {
+                return g.textContent
             }).join(`
 `) : a)), c
         };
         var Cc = /^(?:focusinfocus|focusoutblur)$/,
             Ac = function(a) {
                 a.stopPropagation()
             };
         p.extend(p.event, {
-            trigger: function(a, c, d, m) {
-                var b, x, w, T, A, E, I, _, P = [d || D],
-                    W = g.call(a, "type") ? a.type : a,
-                    ce = g.call(a, "namespace") ? a.namespace.split(".") : [];
-                if (x = _ = w = d = d || D, !(d.nodeType === 3 || d.nodeType === 8) && !Cc.test(W + p.event.triggered) && (W.indexOf(".") > -1 && (ce = W.split("."), W = ce.shift(), ce.sort()), A = W.indexOf(":") < 0 && "on" + W, a = a[p.expando] ? a : new p.Event(W, typeof a == "object" && a), a.isTrigger = m ? 2 : 3, a.namespace = ce.join("."), a.rnamespace = a.namespace ? new RegExp("(^|\\.)" + ce.join("\\.(?:.*\\.|)") + "(\\.|$)") : null, a.result = void 0, a.target || (a.target = d), c = c == null ? [a] : p.makeArray(c, [a]), I = p.event.special[W] || {}, !(!m && I.trigger && I.trigger.apply(d, c) === !1))) {
-                    if (!m && !I.noBubble && !O(d)) {
+            trigger: function(a, c, d, g) {
+                var b, x, w, T, C, E, I, _, P = [d || D],
+                    W = m.call(a, "type") ? a.type : a,
+                    ce = m.call(a, "namespace") ? a.namespace.split(".") : [];
+                if (x = _ = w = d = d || D, !(d.nodeType === 3 || d.nodeType === 8) && !Cc.test(W + p.event.triggered) && (W.indexOf(".") > -1 && (ce = W.split("."), W = ce.shift(), ce.sort()), C = W.indexOf(":") < 0 && "on" + W, a = a[p.expando] ? a : new p.Event(W, typeof a == "object" && a), a.isTrigger = g ? 2 : 3, a.namespace = ce.join("."), a.rnamespace = a.namespace ? new RegExp("(^|\\.)" + ce.join("\\.(?:.*\\.|)") + "(\\.|$)") : null, a.result = void 0, a.target || (a.target = d), c = c == null ? [a] : p.makeArray(c, [a]), I = p.event.special[W] || {}, !(!g && I.trigger && I.trigger.apply(d, c) === !1))) {
+                    if (!g && !I.noBubble && !O(d)) {
                         for (T = I.delegateType || W, Cc.test(T + W) || (x = x.parentNode); x; x = x.parentNode) P.push(x), w = x;
                         w === (d.ownerDocument || D) && P.push(w.defaultView || w.parentWindow || e)
                     }
                     for (b = 0;
-                        (x = P[b++]) && !a.isPropagationStopped();) _ = x, a.type = b > 1 ? T : I.bindType || W, E = (ne.get(x, "events") || Object.create(null))[a.type] && ne.get(x, "handle"), E && E.apply(x, c), E = A && x[A], E && E.apply && Xt(x) && (a.result = E.apply(x, c), a.result === !1 && a.preventDefault());
-                    return a.type = W, !m && !a.isDefaultPrevented() && (!I._default || I._default.apply(P.pop(), c) === !1) && Xt(d) && A && C(d[W]) && !O(d) && (w = d[A], w && (d[A] = null), p.event.triggered = W, a.isPropagationStopped() && _.addEventListener(W, Ac), d[W](), a.isPropagationStopped() && _.removeEventListener(W, Ac), p.event.triggered = void 0, w && (d[A] = w)), a.result
+                        (x = P[b++]) && !a.isPropagationStopped();) _ = x, a.type = b > 1 ? T : I.bindType || W, E = (ne.get(x, "events") || Object.create(null))[a.type] && ne.get(x, "handle"), E && E.apply(x, c), E = C && x[C], E && E.apply && Xt(x) && (a.result = E.apply(x, c), a.result === !1 && a.preventDefault());
+                    return a.type = W, !g && !a.isDefaultPrevented() && (!I._default || I._default.apply(P.pop(), c) === !1) && Xt(d) && C && A(d[W]) && !O(d) && (w = d[C], w && (d[C] = null), p.event.triggered = W, a.isPropagationStopped() && _.addEventListener(W, Ac), d[W](), a.isPropagationStopped() && _.removeEventListener(W, Ac), p.event.triggered = void 0, w && (d[C] = w)), a.result
                 }
             },
             simulate: function(a, c, d) {
-                var m = p.extend(new p.Event, d, {
+                var g = p.extend(new p.Event, d, {
                     type: a,
                     isSimulated: !0
                 });
-                p.event.trigger(m, null, c)
+                p.event.trigger(g, null, c)
             }
         }), p.fn.extend({
             trigger: function(a, c) {
                 return this.each(function() {
                     p.event.trigger(a, c, this)
                 })
             },
             triggerHandler: function(a, c) {
                 var d = this[0];
                 if (d) return p.event.trigger(a, c, d, !0)
             }
         });
-        var Sm = /\[\]$/,
+        var Cm = /\[\]$/,
             Tc = /\r?\n/g,
-            Cm = /^(?:submit|button|image|reset|file)$/i,
-            Am = /^(?:input|select|textarea|keygen)/i;
+            Am = /^(?:submit|button|image|reset|file)$/i,
+            Tm = /^(?:input|select|textarea|keygen)/i;
 
-        function Hl(a, c, d, m) {
+        function Hl(a, c, d, g) {
             var b;
             if (Array.isArray(c)) p.each(c, function(x, w) {
-                d || Sm.test(a) ? m(a, w) : Hl(a + "[" + (typeof w == "object" && w != null ? x : "") + "]", w, d, m)
+                d || Cm.test(a) ? g(a, w) : Hl(a + "[" + (typeof w == "object" && w != null ? x : "") + "]", w, d, g)
             });
             else if (!d && j(c) === "object")
-                for (b in c) Hl(a + "[" + b + "]", c[b], d, m);
-            else m(a, c)
+                for (b in c) Hl(a + "[" + b + "]", c[b], d, g);
+            else g(a, c)
         }
         p.param = function(a, c) {
-            var d, m = [],
+            var d, g = [],
                 b = function(x, w) {
-                    var T = C(w) ? w() : w;
-                    m[m.length] = encodeURIComponent(x) + "=" + encodeURIComponent(T == null ? "" : T)
+                    var T = A(w) ? w() : w;
+                    g[g.length] = encodeURIComponent(x) + "=" + encodeURIComponent(T == null ? "" : T)
                 };
             if (a == null) return "";
             if (Array.isArray(a) || a.jquery && !p.isPlainObject(a)) p.each(a, function() {
                 b(this.name, this.value)
             });
             else
                 for (d in a) Hl(d, a[d], c, b);
-            return m.join("&")
+            return g.join("&")
         }, p.fn.extend({
             serialize: function() {
                 return p.param(this.serializeArray())
             },
             serializeArray: function() {
                 return this.map(function() {
                     var a = p.prop(this, "elements");
                     return a ? p.makeArray(a) : this
                 }).filter(function() {
                     var a = this.type;
-                    return this.name && !p(this).is(":disabled") && Am.test(this.nodeName) && !Cm.test(a) && (this.checked || !rn.test(a))
+                    return this.name && !p(this).is(":disabled") && Tm.test(this.nodeName) && !Am.test(a) && (this.checked || !rn.test(a))
                 }).map(function(a, c) {
                     var d = p(this).val();
-                    return d == null ? null : Array.isArray(d) ? p.map(d, function(m) {
+                    return d == null ? null : Array.isArray(d) ? p.map(d, function(g) {
                         return {
                             name: c.name,
-                            value: m.replace(Tc, `\r
+                            value: g.replace(Tc, `\r
 `)
                         }
                     }) : {
                         name: c.name,
                         value: d.replace(Tc, `\r
 `)
                     }
                 }).get()
             }
         });
-        var Tm = /%20/g,
-            Om = /#.*$/,
-            Mm = /([?&])_=[^&]*/,
-            Em = /^(.*?):[ \t]*([^\r\n]*)$/mg,
-            Dm = /^(?:about|app|app-storage|.+-extension|file|res|widget):$/,
-            Rm = /^(?:GET|HEAD)$/,
-            Lm = /^\/\//,
+        var Om = /%20/g,
+            Mm = /#.*$/,
+            Em = /([?&])_=[^&]*/,
+            Dm = /^(.*?):[ \t]*([^\r\n]*)$/mg,
+            Rm = /^(?:about|app|app-storage|.+-extension|file|res|widget):$/,
+            Lm = /^(?:GET|HEAD)$/,
+            Pm = /^\/\//,
             Oc = {},
             Fl = {},
             Mc = "*/".concat("*"),
             zl = D.createElement("a");
         zl.href = _r.href;
 
         function Ec(a) {
             return function(c, d) {
                 typeof c != "string" && (d = c, c = "*");
-                var m, b = 0,
+                var g, b = 0,
                     x = c.toLowerCase().match(at) || [];
-                if (C(d))
-                    for (; m = x[b++];) m[0] === "+" ? (m = m.slice(1) || "*", (a[m] = a[m] || []).unshift(d)) : (a[m] = a[m] || []).push(d)
+                if (A(d))
+                    for (; g = x[b++];) g[0] === "+" ? (g = g.slice(1) || "*", (a[g] = a[g] || []).unshift(d)) : (a[g] = a[g] || []).push(d)
             }
         }
 
-        function Dc(a, c, d, m) {
+        function Dc(a, c, d, g) {
             var b = {},
                 x = a === Fl;
 
             function w(T) {
-                var A;
+                var C;
                 return b[T] = !0, p.each(a[T] || [], function(E, I) {
-                    var _ = I(c, d, m);
+                    var _ = I(c, d, g);
                     if (typeof _ == "string" && !x && !b[_]) return c.dataTypes.unshift(_), w(_), !1;
-                    if (x) return !(A = _)
-                }), A
+                    if (x) return !(C = _)
+                }), C
             }
             return w(c.dataTypes[0]) || !b["*"] && w("*")
         }
 
         function $l(a, c) {
-            var d, m, b = p.ajaxSettings.flatOptions || {};
-            for (d in c) c[d] !== void 0 && ((b[d] ? a : m || (m = {}))[d] = c[d]);
-            return m && p.extend(!0, a, m), a
+            var d, g, b = p.ajaxSettings.flatOptions || {};
+            for (d in c) c[d] !== void 0 && ((b[d] ? a : g || (g = {}))[d] = c[d]);
+            return g && p.extend(!0, a, g), a
         }
 
-        function Pm(a, c, d) {
-            for (var m, b, x, w, T = a.contents, A = a.dataTypes; A[0] === "*";) A.shift(), m === void 0 && (m = a.mimeType || c.getResponseHeader("Content-Type"));
-            if (m) {
+        function Nm(a, c, d) {
+            for (var g, b, x, w, T = a.contents, C = a.dataTypes; C[0] === "*";) C.shift(), g === void 0 && (g = a.mimeType || c.getResponseHeader("Content-Type"));
+            if (g) {
                 for (b in T)
-                    if (T[b] && T[b].test(m)) {
-                        A.unshift(b);
+                    if (T[b] && T[b].test(g)) {
+                        C.unshift(b);
                         break
                     }
             }
-            if (A[0] in d) x = A[0];
+            if (C[0] in d) x = C[0];
             else {
                 for (b in d) {
-                    if (!A[0] || a.converters[b + " " + A[0]]) {
+                    if (!C[0] || a.converters[b + " " + C[0]]) {
                         x = b;
                         break
                     }
                     w || (w = b)
                 }
                 x = x || w
             }
-            if (x) return x !== A[0] && A.unshift(x), d[x]
+            if (x) return x !== C[0] && C.unshift(x), d[x]
         }
 
-        function Nm(a, c, d, m) {
-            var b, x, w, T, A, E = {},
+        function Im(a, c, d, g) {
+            var b, x, w, T, C, E = {},
                 I = a.dataTypes.slice();
             if (I[1])
                 for (w in a.converters) E[w.toLowerCase()] = a.converters[w];
             for (x = I.shift(); x;)
-                if (a.responseFields[x] && (d[a.responseFields[x]] = c), !A && m && a.dataFilter && (c = a.dataFilter(c, a.dataType)), A = x, x = I.shift(), x) {
-                    if (x === "*") x = A;
-                    else if (A !== "*" && A !== x) {
-                        if (w = E[A + " " + x] || E["* " + x], !w) {
+                if (a.responseFields[x] && (d[a.responseFields[x]] = c), !C && g && a.dataFilter && (c = a.dataFilter(c, a.dataType)), C = x, x = I.shift(), x) {
+                    if (x === "*") x = C;
+                    else if (C !== "*" && C !== x) {
+                        if (w = E[C + " " + x] || E["* " + x], !w) {
                             for (b in E)
-                                if (T = b.split(" "), T[1] === x && (w = E[A + " " + T[0]] || E["* " + T[0]], w)) {
+                                if (T = b.split(" "), T[1] === x && (w = E[C + " " + T[0]] || E["* " + T[0]], w)) {
                                     w === !0 ? w = E[b] : E[b] !== !0 && (x = T[0], I.unshift(T[1]));
                                     break
                                 }
                         }
                         if (w !== !0)
                             if (w && a.throws) c = w(c);
                             else try {
                                 c = w(c)
                             } catch (_) {
                                 return {
                                     state: "parsererror",
-                                    error: w ? _ : "No conversion from " + A + " to " + x
+                                    error: w ? _ : "No conversion from " + C + " to " + x
                                 }
                             }
                     }
                 } return {
                 state: "success",
                 data: c
             }
@@ -2891,15 +2891,15 @@
         p.extend({
             active: 0,
             lastModified: {},
             etag: {},
             ajaxSettings: {
                 url: _r.href,
                 type: "GET",
-                isLocal: Dm.test(_r.protocol),
+                isLocal: Rm.test(_r.protocol),
                 global: !0,
                 processData: !0,
                 async: !0,
                 contentType: "application/x-www-form-urlencoded; charset=UTF-8",
                 accepts: {
                     "*": Mc,
                     text: "text/plain",
@@ -2931,101 +2931,101 @@
             ajaxSetup: function(a, c) {
                 return c ? $l($l(a, p.ajaxSettings), c) : $l(p.ajaxSettings, a)
             },
             ajaxPrefilter: Ec(Oc),
             ajaxTransport: Ec(Fl),
             ajax: function(a, c) {
                 typeof a == "object" && (c = a, a = void 0), c = c || {};
-                var d, m, b, x, w, T, A, E, I, _, P = p.ajaxSetup({}, c),
+                var d, g, b, x, w, T, C, E, I, _, P = p.ajaxSetup({}, c),
                     W = P.context || P,
                     ce = P.context && (W.nodeType || W.jquery) ? p(W) : p.event,
-                    Te = p.Deferred(),
+                    Ae = p.Deferred(),
                     ge = p.Callbacks("once memory"),
                     ut = P.statusCode || {},
                     et = {},
                     wi = {},
                     vi = "canceled",
                     ve = {
                         readyState: 0,
                         getResponseHeader: function(Me) {
                             var Qe;
-                            if (A) {
+                            if (C) {
                                 if (!x)
-                                    for (x = {}; Qe = Em.exec(b);) x[Qe[1].toLowerCase() + " "] = (x[Qe[1].toLowerCase() + " "] || []).concat(Qe[2]);
+                                    for (x = {}; Qe = Dm.exec(b);) x[Qe[1].toLowerCase() + " "] = (x[Qe[1].toLowerCase() + " "] || []).concat(Qe[2]);
                                 Qe = x[Me.toLowerCase() + " "]
                             }
                             return Qe == null ? null : Qe.join(", ")
                         },
                         getAllResponseHeaders: function() {
-                            return A ? b : null
+                            return C ? b : null
                         },
                         setRequestHeader: function(Me, Qe) {
-                            return A == null && (Me = wi[Me.toLowerCase()] = wi[Me.toLowerCase()] || Me, et[Me] = Qe), this
+                            return C == null && (Me = wi[Me.toLowerCase()] = wi[Me.toLowerCase()] || Me, et[Me] = Qe), this
                         },
                         overrideMimeType: function(Me) {
-                            return A == null && (P.mimeType = Me), this
+                            return C == null && (P.mimeType = Me), this
                         },
                         statusCode: function(Me) {
                             var Qe;
                             if (Me)
-                                if (A) ve.always(Me[ve.status]);
+                                if (C) ve.always(Me[ve.status]);
                                 else
                                     for (Qe in Me) ut[Qe] = [ut[Qe], Me[Qe]];
                             return this
                         },
                         abort: function(Me) {
                             var Qe = Me || vi;
                             return d && d.abort(Qe), Nn(0, Qe), this
                         }
                     };
-                if (Te.promise(ve), P.url = ((a || P.url || _r.href) + "").replace(Lm, _r.protocol + "//"), P.type = c.method || c.type || P.method || P.type, P.dataTypes = (P.dataType || "*").toLowerCase().match(at) || [""], P.crossDomain == null) {
+                if (Ae.promise(ve), P.url = ((a || P.url || _r.href) + "").replace(Pm, _r.protocol + "//"), P.type = c.method || c.type || P.method || P.type, P.dataTypes = (P.dataType || "*").toLowerCase().match(at) || [""], P.crossDomain == null) {
                     T = D.createElement("a");
                     try {
                         T.href = P.url, T.href = T.href, P.crossDomain = zl.protocol + "//" + zl.host != T.protocol + "//" + T.host
                     } catch (Me) {
                         P.crossDomain = !0
                     }
                 }
-                if (P.data && P.processData && typeof P.data != "string" && (P.data = p.param(P.data, P.traditional)), Dc(Oc, P, c, ve), A) return ve;
-                E = p.event && P.global, E && p.active++ === 0 && p.event.trigger("ajaxStart"), P.type = P.type.toUpperCase(), P.hasContent = !Rm.test(P.type), m = P.url.replace(Om, ""), P.hasContent ? P.data && P.processData && (P.contentType || "").indexOf("application/x-www-form-urlencoded") === 0 && (P.data = P.data.replace(Tm, "+")) : (_ = P.url.slice(m.length), P.data && (P.processData || typeof P.data == "string") && (m += (_l.test(m) ? "&" : "?") + P.data, delete P.data), P.cache === !1 && (m = m.replace(Mm, "$1"), _ = (_l.test(m) ? "&" : "?") + "_=" + Sc.guid++ + _), P.url = m + _), P.ifModified && (p.lastModified[m] && ve.setRequestHeader("If-Modified-Since", p.lastModified[m]), p.etag[m] && ve.setRequestHeader("If-None-Match", p.etag[m])), (P.data && P.hasContent && P.contentType !== !1 || c.contentType) && ve.setRequestHeader("Content-Type", P.contentType), ve.setRequestHeader("Accept", P.dataTypes[0] && P.accepts[P.dataTypes[0]] ? P.accepts[P.dataTypes[0]] + (P.dataTypes[0] !== "*" ? ", " + Mc + "; q=0.01" : "") : P.accepts["*"]);
+                if (P.data && P.processData && typeof P.data != "string" && (P.data = p.param(P.data, P.traditional)), Dc(Oc, P, c, ve), C) return ve;
+                E = p.event && P.global, E && p.active++ === 0 && p.event.trigger("ajaxStart"), P.type = P.type.toUpperCase(), P.hasContent = !Lm.test(P.type), g = P.url.replace(Mm, ""), P.hasContent ? P.data && P.processData && (P.contentType || "").indexOf("application/x-www-form-urlencoded") === 0 && (P.data = P.data.replace(Om, "+")) : (_ = P.url.slice(g.length), P.data && (P.processData || typeof P.data == "string") && (g += (_l.test(g) ? "&" : "?") + P.data, delete P.data), P.cache === !1 && (g = g.replace(Em, "$1"), _ = (_l.test(g) ? "&" : "?") + "_=" + Sc.guid++ + _), P.url = g + _), P.ifModified && (p.lastModified[g] && ve.setRequestHeader("If-Modified-Since", p.lastModified[g]), p.etag[g] && ve.setRequestHeader("If-None-Match", p.etag[g])), (P.data && P.hasContent && P.contentType !== !1 || c.contentType) && ve.setRequestHeader("Content-Type", P.contentType), ve.setRequestHeader("Accept", P.dataTypes[0] && P.accepts[P.dataTypes[0]] ? P.accepts[P.dataTypes[0]] + (P.dataTypes[0] !== "*" ? ", " + Mc + "; q=0.01" : "") : P.accepts["*"]);
                 for (I in P.headers) ve.setRequestHeader(I, P.headers[I]);
-                if (P.beforeSend && (P.beforeSend.call(W, ve, P) === !1 || A)) return ve.abort();
+                if (P.beforeSend && (P.beforeSend.call(W, ve, P) === !1 || C)) return ve.abort();
                 if (vi = "abort", ge.add(P.complete), ve.done(P.success), ve.fail(P.error), d = Dc(Fl, P, c, ve), !d) Nn(-1, "No Transport");
                 else {
-                    if (ve.readyState = 1, E && ce.trigger("ajaxSend", [ve, P]), A) return ve;
+                    if (ve.readyState = 1, E && ce.trigger("ajaxSend", [ve, P]), C) return ve;
                     P.async && P.timeout > 0 && (w = e.setTimeout(function() {
                         ve.abort("timeout")
                     }, P.timeout));
                     try {
-                        A = !1, d.send(et, Nn)
+                        C = !1, d.send(et, Nn)
                     } catch (Me) {
-                        if (A) throw Me;
+                        if (C) throw Me;
                         Nn(-1, Me)
                     }
                 }
 
                 function Nn(Me, Qe, Fr, ql) {
                     var Si, zr, Ci, on, ln, Zt = Qe;
-                    A || (A = !0, w && e.clearTimeout(w), d = void 0, b = ql || "", ve.readyState = Me > 0 ? 4 : 0, Si = Me >= 200 && Me < 300 || Me === 304, Fr && (on = Pm(P, ve, Fr)), !Si && p.inArray("script", P.dataTypes) > -1 && p.inArray("json", P.dataTypes) < 0 && (P.converters["text script"] = function() {}), on = Nm(P, on, ve, Si), Si ? (P.ifModified && (ln = ve.getResponseHeader("Last-Modified"), ln && (p.lastModified[m] = ln), ln = ve.getResponseHeader("etag"), ln && (p.etag[m] = ln)), Me === 204 || P.type === "HEAD" ? Zt = "nocontent" : Me === 304 ? Zt = "notmodified" : (Zt = on.state, zr = on.data, Ci = on.error, Si = !Ci)) : (Ci = Zt, (Me || !Zt) && (Zt = "error", Me < 0 && (Me = 0))), ve.status = Me, ve.statusText = (Qe || Zt) + "", Si ? Te.resolveWith(W, [zr, Zt, ve]) : Te.rejectWith(W, [ve, Zt, Ci]), ve.statusCode(ut), ut = void 0, E && ce.trigger(Si ? "ajaxSuccess" : "ajaxError", [ve, P, Si ? zr : Ci]), ge.fireWith(W, [ve, Zt]), E && (ce.trigger("ajaxComplete", [ve, P]), --p.active || p.event.trigger("ajaxStop")))
+                    C || (C = !0, w && e.clearTimeout(w), d = void 0, b = ql || "", ve.readyState = Me > 0 ? 4 : 0, Si = Me >= 200 && Me < 300 || Me === 304, Fr && (on = Nm(P, ve, Fr)), !Si && p.inArray("script", P.dataTypes) > -1 && p.inArray("json", P.dataTypes) < 0 && (P.converters["text script"] = function() {}), on = Im(P, on, ve, Si), Si ? (P.ifModified && (ln = ve.getResponseHeader("Last-Modified"), ln && (p.lastModified[g] = ln), ln = ve.getResponseHeader("etag"), ln && (p.etag[g] = ln)), Me === 204 || P.type === "HEAD" ? Zt = "nocontent" : Me === 304 ? Zt = "notmodified" : (Zt = on.state, zr = on.data, Ci = on.error, Si = !Ci)) : (Ci = Zt, (Me || !Zt) && (Zt = "error", Me < 0 && (Me = 0))), ve.status = Me, ve.statusText = (Qe || Zt) + "", Si ? Ae.resolveWith(W, [zr, Zt, ve]) : Ae.rejectWith(W, [ve, Zt, Ci]), ve.statusCode(ut), ut = void 0, E && ce.trigger(Si ? "ajaxSuccess" : "ajaxError", [ve, P, Si ? zr : Ci]), ge.fireWith(W, [ve, Zt]), E && (ce.trigger("ajaxComplete", [ve, P]), --p.active || p.event.trigger("ajaxStop")))
                 }
                 return ve
             },
             getJSON: function(a, c, d) {
                 return p.get(a, c, d, "json")
             },
             getScript: function(a, c) {
                 return p.get(a, void 0, c, "script")
             }
         }), p.each(["get", "post"], function(a, c) {
-            p[c] = function(d, m, b, x) {
-                return C(m) && (x = x || b, b = m, m = void 0), p.ajax(p.extend({
+            p[c] = function(d, g, b, x) {
+                return A(g) && (x = x || b, b = g, g = void 0), p.ajax(p.extend({
                     url: d,
                     type: c,
                     dataType: x,
-                    data: m,
+                    data: g,
                     success: b
                 }, p.isPlainObject(d) && d))
             }
         }), p.ajaxPrefilter(function(a) {
             var c;
             for (c in a.headers) c.toLowerCase() === "content-type" && (a.contentType = a.headers[c] || "")
         }), p._evalUrl = function(a, c, d) {
@@ -3035,37 +3035,37 @@
                 dataType: "script",
                 cache: !0,
                 async: !1,
                 global: !1,
                 converters: {
                     "text script": function() {}
                 },
-                dataFilter: function(m) {
-                    p.globalEval(m, c, d)
+                dataFilter: function(g) {
+                    p.globalEval(g, c, d)
                 }
             })
         }, p.fn.extend({
             wrapAll: function(a) {
                 var c;
-                return this[0] && (C(a) && (a = a.call(this[0])), c = p(a, this[0].ownerDocument).eq(0).clone(!0), this[0].parentNode && c.insertBefore(this[0]), c.map(function() {
+                return this[0] && (A(a) && (a = a.call(this[0])), c = p(a, this[0].ownerDocument).eq(0).clone(!0), this[0].parentNode && c.insertBefore(this[0]), c.map(function() {
                     for (var d = this; d.firstElementChild;) d = d.firstElementChild;
                     return d
                 }).append(this)), this
             },
             wrapInner: function(a) {
-                return C(a) ? this.each(function(c) {
+                return A(a) ? this.each(function(c) {
                     p(this).wrapInner(a.call(this, c))
                 }) : this.each(function() {
                     var c = p(this),
                         d = c.contents();
                     d.length ? d.wrapAll(a) : c.append(a)
                 })
             },
             wrap: function(a) {
-                var c = C(a);
+                var c = A(a);
                 return this.each(function(d) {
                     p(this).wrapAll(c ? a.call(this, d) : a)
                 })
             },
             unwrap: function(a) {
                 return this.parent(a).not("body").each(function() {
                     p(this).replaceWith(this.childNodes)
@@ -3076,31 +3076,31 @@
         }, p.expr.pseudos.visible = function(a) {
             return !!(a.offsetWidth || a.offsetHeight || a.getClientRects().length)
         }, p.ajaxSettings.xhr = function() {
             try {
                 return new e.XMLHttpRequest
             } catch (a) {}
         };
-        var Im = {
+        var Bm = {
                 0: 200,
                 1223: 204
             },
             Hr = p.ajaxSettings.xhr();
         v.cors = !!Hr && "withCredentials" in Hr, v.ajax = Hr = !!Hr, p.ajaxTransport(function(a) {
             var c, d;
             if (v.cors || Hr && !a.crossDomain) return {
-                send: function(m, b) {
+                send: function(g, b) {
                     var x, w = a.xhr();
                     if (w.open(a.type, a.url, a.async, a.username, a.password), a.xhrFields)
                         for (x in a.xhrFields) w[x] = a.xhrFields[x];
-                    a.mimeType && w.overrideMimeType && w.overrideMimeType(a.mimeType), !a.crossDomain && !m["X-Requested-With"] && (m["X-Requested-With"] = "XMLHttpRequest");
-                    for (x in m) w.setRequestHeader(x, m[x]);
+                    a.mimeType && w.overrideMimeType && w.overrideMimeType(a.mimeType), !a.crossDomain && !g["X-Requested-With"] && (g["X-Requested-With"] = "XMLHttpRequest");
+                    for (x in g) w.setRequestHeader(x, g[x]);
                     c = function(T) {
                         return function() {
-                            c && (c = d = w.onload = w.onerror = w.onabort = w.ontimeout = w.onreadystatechange = null, T === "abort" ? w.abort() : T === "error" ? typeof w.status != "number" ? b(0, "error") : b(w.status, w.statusText) : b(Im[w.status] || w.status, w.statusText, (w.responseType || "text") !== "text" || typeof w.responseText != "string" ? {
+                            c && (c = d = w.onload = w.onerror = w.onabort = w.ontimeout = w.onreadystatechange = null, T === "abort" ? w.abort() : T === "error" ? typeof w.status != "number" ? b(0, "error") : b(w.status, w.statusText) : b(Bm[w.status] || w.status, w.statusText, (w.responseType || "text") !== "text" || typeof w.responseText != "string" ? {
                                 binary: w.response
                             } : {
                                 text: w.responseText
                             }, w.getAllResponseHeaders()))
                         }
                     }, w.onload = c(), d = w.onerror = w.ontimeout = c("error"), w.onabort !== void 0 ? w.onabort = d : w.onreadystatechange = function() {
                         w.readyState === 4 && e.setTimeout(function() {
@@ -3133,15 +3133,15 @@
             }
         }), p.ajaxPrefilter("script", function(a) {
             a.cache === void 0 && (a.cache = !1), a.crossDomain && (a.type = "GET")
         }), p.ajaxTransport("script", function(a) {
             if (a.crossDomain || a.scriptAttrs) {
                 var c, d;
                 return {
-                    send: function(m, b) {
+                    send: function(g, b) {
                         c = p("<script>").attr(a.scriptAttrs || {}).prop({
                             charset: a.scriptCharset,
                             src: a.url
                         }).on("load error", d = function(x) {
                             c.remove(), d = null, x && b(x.type === "error" ? 404 : 200, x.type)
                         }), D.head.appendChild(c[0])
                     },
@@ -3156,176 +3156,176 @@
         p.ajaxSetup({
             jsonp: "callback",
             jsonpCallback: function() {
                 var a = Rc.pop() || p.expando + "_" + Sc.guid++;
                 return this[a] = !0, a
             }
         }), p.ajaxPrefilter("json jsonp", function(a, c, d) {
-            var m, b, x, w = a.jsonp !== !1 && (Wl.test(a.url) ? "url" : typeof a.data == "string" && (a.contentType || "").indexOf("application/x-www-form-urlencoded") === 0 && Wl.test(a.data) && "data");
-            if (w || a.dataTypes[0] === "jsonp") return m = a.jsonpCallback = C(a.jsonpCallback) ? a.jsonpCallback() : a.jsonpCallback, w ? a[w] = a[w].replace(Wl, "$1" + m) : a.jsonp !== !1 && (a.url += (_l.test(a.url) ? "&" : "?") + a.jsonp + "=" + m), a.converters["script json"] = function() {
-                return x || p.error(m + " was not called"), x[0]
-            }, a.dataTypes[0] = "json", b = e[m], e[m] = function() {
+            var g, b, x, w = a.jsonp !== !1 && (Wl.test(a.url) ? "url" : typeof a.data == "string" && (a.contentType || "").indexOf("application/x-www-form-urlencoded") === 0 && Wl.test(a.data) && "data");
+            if (w || a.dataTypes[0] === "jsonp") return g = a.jsonpCallback = A(a.jsonpCallback) ? a.jsonpCallback() : a.jsonpCallback, w ? a[w] = a[w].replace(Wl, "$1" + g) : a.jsonp !== !1 && (a.url += (_l.test(a.url) ? "&" : "?") + a.jsonp + "=" + g), a.converters["script json"] = function() {
+                return x || p.error(g + " was not called"), x[0]
+            }, a.dataTypes[0] = "json", b = e[g], e[g] = function() {
                 x = arguments
             }, d.always(function() {
-                b === void 0 ? p(e).removeProp(m) : e[m] = b, a[m] && (a.jsonpCallback = c.jsonpCallback, Rc.push(m)), x && C(b) && b(x[0]), x = b = void 0
+                b === void 0 ? p(e).removeProp(g) : e[g] = b, a[g] && (a.jsonpCallback = c.jsonpCallback, Rc.push(g)), x && A(b) && b(x[0]), x = b = void 0
             }), "script"
         }), v.createHTMLDocument = function() {
             var a = D.implementation.createHTMLDocument("").body;
             return a.innerHTML = "<form></form><form></form>", a.childNodes.length === 2
         }(), p.parseHTML = function(a, c, d) {
             if (typeof a != "string") return [];
             typeof c == "boolean" && (d = c, c = !1);
-            var m, b, x;
-            return c || (v.createHTMLDocument ? (c = D.implementation.createHTMLDocument(""), m = c.createElement("base"), m.href = D.location.href, c.head.appendChild(m)) : c = D), b = bt.exec(a), x = !d && [], b ? [c.createElement(b[1])] : (b = zs([a], c, x), x && x.length && p(x).remove(), p.merge([], b.childNodes))
+            var g, b, x;
+            return c || (v.createHTMLDocument ? (c = D.implementation.createHTMLDocument(""), g = c.createElement("base"), g.href = D.location.href, c.head.appendChild(g)) : c = D), b = bt.exec(a), x = !d && [], b ? [c.createElement(b[1])] : (b = zs([a], c, x), x && x.length && p(x).remove(), p.merge([], b.childNodes))
         }, p.fn.load = function(a, c, d) {
-            var m, b, x, w = this,
+            var g, b, x, w = this,
                 T = a.indexOf(" ");
-            return T > -1 && (m = Ln(a.slice(T)), a = a.slice(0, T)), C(c) ? (d = c, c = void 0) : c && typeof c == "object" && (b = "POST"), w.length > 0 && p.ajax({
+            return T > -1 && (g = Ln(a.slice(T)), a = a.slice(0, T)), A(c) ? (d = c, c = void 0) : c && typeof c == "object" && (b = "POST"), w.length > 0 && p.ajax({
                 url: a,
                 type: b || "GET",
                 dataType: "html",
                 data: c
-            }).done(function(A) {
-                x = arguments, w.html(m ? p("<div>").append(p.parseHTML(A)).find(m) : A)
-            }).always(d && function(A, E) {
+            }).done(function(C) {
+                x = arguments, w.html(g ? p("<div>").append(p.parseHTML(C)).find(g) : C)
+            }).always(d && function(C, E) {
                 w.each(function() {
-                    d.apply(this, x || [A.responseText, E, A])
+                    d.apply(this, x || [C.responseText, E, C])
                 })
             }), this
         }, p.expr.pseudos.animated = function(a) {
             return p.grep(p.timers, function(c) {
                 return a === c.elem
             }).length
         }, p.offset = {
             setOffset: function(a, c, d) {
-                var m, b, x, w, T, A, E, I = p.css(a, "position"),
+                var g, b, x, w, T, C, E, I = p.css(a, "position"),
                     _ = p(a),
                     P = {};
-                I === "static" && (a.style.position = "relative"), T = _.offset(), x = p.css(a, "top"), A = p.css(a, "left"), E = (I === "absolute" || I === "fixed") && (x + A).indexOf("auto") > -1, E ? (m = _.position(), w = m.top, b = m.left) : (w = parseFloat(x) || 0, b = parseFloat(A) || 0), C(c) && (c = c.call(a, d, p.extend({}, T))), c.top != null && (P.top = c.top - T.top + w), c.left != null && (P.left = c.left - T.left + b), "using" in c ? c.using.call(a, P) : _.css(P)
+                I === "static" && (a.style.position = "relative"), T = _.offset(), x = p.css(a, "top"), C = p.css(a, "left"), E = (I === "absolute" || I === "fixed") && (x + C).indexOf("auto") > -1, E ? (g = _.position(), w = g.top, b = g.left) : (w = parseFloat(x) || 0, b = parseFloat(C) || 0), A(c) && (c = c.call(a, d, p.extend({}, T))), c.top != null && (P.top = c.top - T.top + w), c.left != null && (P.left = c.left - T.left + b), "using" in c ? c.using.call(a, P) : _.css(P)
             }
         }, p.fn.extend({
             offset: function(a) {
                 if (arguments.length) return a === void 0 ? this : this.each(function(b) {
                     p.offset.setOffset(this, a, b)
                 });
-                var c, d, m = this[0];
-                if (m) return m.getClientRects().length ? (c = m.getBoundingClientRect(), d = m.ownerDocument.defaultView, {
+                var c, d, g = this[0];
+                if (g) return g.getClientRects().length ? (c = g.getBoundingClientRect(), d = g.ownerDocument.defaultView, {
                     top: c.top + d.pageYOffset,
                     left: c.left + d.pageXOffset
                 }) : {
                     top: 0,
                     left: 0
                 }
             },
             position: function() {
                 if (this[0]) {
-                    var a, c, d, m = this[0],
+                    var a, c, d, g = this[0],
                         b = {
                             top: 0,
                             left: 0
                         };
-                    if (p.css(m, "position") === "fixed") c = m.getBoundingClientRect();
+                    if (p.css(g, "position") === "fixed") c = g.getBoundingClientRect();
                     else {
-                        for (c = this.offset(), d = m.ownerDocument, a = m.offsetParent || d.documentElement; a && (a === d.body || a === d.documentElement) && p.css(a, "position") === "static";) a = a.parentNode;
-                        a && a !== m && a.nodeType === 1 && (b = p(a).offset(), b.top += p.css(a, "borderTopWidth", !0), b.left += p.css(a, "borderLeftWidth", !0))
+                        for (c = this.offset(), d = g.ownerDocument, a = g.offsetParent || d.documentElement; a && (a === d.body || a === d.documentElement) && p.css(a, "position") === "static";) a = a.parentNode;
+                        a && a !== g && a.nodeType === 1 && (b = p(a).offset(), b.top += p.css(a, "borderTopWidth", !0), b.left += p.css(a, "borderLeftWidth", !0))
                     }
                     return {
-                        top: c.top - b.top - p.css(m, "marginTop", !0),
-                        left: c.left - b.left - p.css(m, "marginLeft", !0)
+                        top: c.top - b.top - p.css(g, "marginTop", !0),
+                        left: c.left - b.left - p.css(g, "marginLeft", !0)
                     }
                 }
             },
             offsetParent: function() {
                 return this.map(function() {
                     for (var a = this.offsetParent; a && p.css(a, "position") === "static";) a = a.offsetParent;
                     return a || ai
                 })
             }
         }), p.each({
             scrollLeft: "pageXOffset",
             scrollTop: "pageYOffset"
         }, function(a, c) {
             var d = c === "pageYOffset";
-            p.fn[a] = function(m) {
+            p.fn[a] = function(g) {
                 return Kt(this, function(b, x, w) {
                     var T;
                     if (O(b) ? T = b : b.nodeType === 9 && (T = b.defaultView), w === void 0) return T ? T[c] : b[x];
                     T ? T.scrollTo(d ? T.pageXOffset : w, d ? w : T.pageYOffset) : b[x] = w
-                }, a, m, arguments.length)
+                }, a, g, arguments.length)
             }
         }), p.each(["top", "left"], function(a, c) {
-            p.cssHooks[c] = sn(v.pixelPosition, function(d, m) {
-                if (m) return m = zt(d, c), Y.test(m) ? p(d).position()[c] + "px" : m
+            p.cssHooks[c] = sn(v.pixelPosition, function(d, g) {
+                if (g) return g = zt(d, c), Y.test(g) ? p(d).position()[c] + "px" : g
             })
         }), p.each({
             Height: "height",
             Width: "width"
         }, function(a, c) {
             p.each({
                 padding: "inner" + a,
                 content: c,
                 "": "outer" + a
-            }, function(d, m) {
-                p.fn[m] = function(b, x) {
+            }, function(d, g) {
+                p.fn[g] = function(b, x) {
                     var w = arguments.length && (d || typeof b != "boolean"),
                         T = d || (b === !0 || x === !0 ? "margin" : "border");
-                    return Kt(this, function(A, E, I) {
+                    return Kt(this, function(C, E, I) {
                         var _;
-                        return O(A) ? m.indexOf("outer") === 0 ? A["inner" + a] : A.document.documentElement["client" + a] : A.nodeType === 9 ? (_ = A.documentElement, Math.max(A.body["scroll" + a], _["scroll" + a], A.body["offset" + a], _["offset" + a], _["client" + a])) : I === void 0 ? p.css(A, E, T) : p.style(A, E, I, T)
+                        return O(C) ? g.indexOf("outer") === 0 ? C["inner" + a] : C.document.documentElement["client" + a] : C.nodeType === 9 ? (_ = C.documentElement, Math.max(C.body["scroll" + a], _["scroll" + a], C.body["offset" + a], _["offset" + a], _["client" + a])) : I === void 0 ? p.css(C, E, T) : p.style(C, E, I, T)
                     }, c, w ? b : void 0, w)
                 }
             })
         }), p.each(["ajaxStart", "ajaxStop", "ajaxComplete", "ajaxError", "ajaxSuccess", "ajaxSend"], function(a, c) {
             p.fn[c] = function(d) {
                 return this.on(c, d)
             }
         }), p.fn.extend({
             bind: function(a, c, d) {
                 return this.on(a, null, c, d)
             },
             unbind: function(a, c) {
                 return this.off(a, null, c)
             },
-            delegate: function(a, c, d, m) {
-                return this.on(c, a, d, m)
+            delegate: function(a, c, d, g) {
+                return this.on(c, a, d, g)
             },
             undelegate: function(a, c, d) {
                 return arguments.length === 1 ? this.off(a, "**") : this.off(c, a || "**", d)
             },
             hover: function(a, c) {
                 return this.on("mouseenter", a).on("mouseleave", c || a)
             }
         }), p.each("blur focus focusin focusout resize scroll click dblclick mousedown mouseup mousemove mouseover mouseout mouseenter mouseleave change select submit keydown keypress keyup contextmenu".split(" "), function(a, c) {
-            p.fn[c] = function(d, m) {
-                return arguments.length > 0 ? this.on(c, null, d, m) : this.trigger(c)
+            p.fn[c] = function(d, g) {
+                return arguments.length > 0 ? this.on(c, null, d, g) : this.trigger(c)
             }
         });
-        var Bm = /^[\s\uFEFF\xA0]+|([^\s\uFEFF\xA0])[\s\uFEFF\xA0]+$/g;
+        var _m = /^[\s\uFEFF\xA0]+|([^\s\uFEFF\xA0])[\s\uFEFF\xA0]+$/g;
         p.proxy = function(a, c) {
-            var d, m, b;
-            if (typeof c == "string" && (d = a[c], c = a, a = d), !!C(a)) return m = s.call(arguments, 2), b = function() {
-                return a.apply(c || this, m.concat(s.call(arguments)))
+            var d, g, b;
+            if (typeof c == "string" && (d = a[c], c = a, a = d), !!A(a)) return g = s.call(arguments, 2), b = function() {
+                return a.apply(c || this, g.concat(s.call(arguments)))
             }, b.guid = a.guid = a.guid || p.guid++, b
         }, p.holdReady = function(a) {
             a ? p.readyWait++ : p.ready(!0)
-        }, p.isArray = Array.isArray, p.parseJSON = JSON.parse, p.nodeName = J, p.isFunction = C, p.isWindow = O, p.camelCase = ht, p.type = j, p.now = Date.now, p.isNumeric = function(a) {
+        }, p.isArray = Array.isArray, p.parseJSON = JSON.parse, p.nodeName = J, p.isFunction = A, p.isWindow = O, p.camelCase = ht, p.type = j, p.now = Date.now, p.isNumeric = function(a) {
             var c = p.type(a);
             return (c === "number" || c === "string") && !isNaN(a - parseFloat(a))
         }, p.trim = function(a) {
-            return a == null ? "" : (a + "").replace(Bm, "$1")
+            return a == null ? "" : (a + "").replace(_m, "$1")
         };
-        var _m = e.jQuery,
-            Hm = e.$;
+        var Hm = e.jQuery,
+            Fm = e.$;
         return p.noConflict = function(a) {
-            return e.$ === p && (e.$ = Hm), a && e.jQuery === p && (e.jQuery = _m), p
+            return e.$ === p && (e.$ = Fm), a && e.jQuery === p && (e.jQuery = Hm), p
         }, typeof t == "undefined" && (e.jQuery = e.$ = p), p
     })
 })(Qu);
-var r0 = Qu.exports;
-const Ce = i0(r0);
+var s0 = Qu.exports;
+const Te = n0(s0);
 class De {
     lineAt(e) {
         if (e < 0 || e > this.length) throw new RangeError(`Invalid position ${e} in document of length ${this.length}`);
         return this.lineInner(e, !1, 1, 0)
     }
     line(e) {
         if (e < 1 || e > this.lines) throw new RangeError(`Invalid line number ${e} in ${this.lines}-line document`);
@@ -3382,28 +3382,28 @@
     constructor() {}
     static of (e) {
         if (e.length == 0) throw new RangeError("A document must have at least one line");
         return e.length == 1 && !e[0] ? De.empty : e.length <= 32 ? new Xe(e) : Ri.from(Xe.split(e, []))
     }
 }
 class Xe extends De {
-    constructor(e, t = s0(e)) {
+    constructor(e, t = o0(e)) {
         super(), this.text = e, this.length = t
     }
     get lines() {
         return this.text.length
     }
     get children() {
         return null
     }
     lineInner(e, t, i, r) {
         for (let s = 0;; s++) {
             let o = this.text[s],
                 l = r + o.length;
-            if ((t ? i : l) >= e) return new o0(r, l, i, o);
+            if ((t ? i : l) >= e) return new l0(r, l, i, o);
             r = l + 1, i++
         }
     }
     decompose(e, t, i, r) {
         let s = e <= 0 && t >= this.length ? this : new Xe(Bc(this.text, e, t), Math.min(t, this.length) - Math.max(0, e));
         if (r & 1) {
             let o = i.pop(),
@@ -3527,31 +3527,31 @@
             s = r << 1,
             o = r >> 1,
             l = [],
             h = 0,
             f = -1,
             u = [];
 
-        function g(k) {
+        function m(k) {
             let v;
             if (k.lines > s && k instanceof Ri)
-                for (let C of k.children) g(C);
+                for (let A of k.children) m(A);
             else k.lines > o && (h > o || !h) ? (y(), l.push(k)) : k instanceof Xe && h && (v = u[u.length - 1]) instanceof Xe && k.lines + v.lines <= 32 ? (h += k.lines, f += k.length + 1, u[u.length - 1] = new Xe(v.text.concat(k.text), v.length + 1 + k.length)) : (h + k.lines > r && y(), h += k.lines, f += k.length + 1, u.push(k))
         }
 
         function y() {
             h != 0 && (l.push(u.length == 1 ? u[0] : Ri.from(u, f)), f = -1, h = u.length = 0)
         }
-        for (let k of e) g(k);
+        for (let k of e) m(k);
         return y(), l.length == 1 ? l[0] : new Ri(l, t)
     }
 }
 De.empty = new Xe([""], 0);
 
-function s0(n) {
+function o0(n) {
     let e = -1;
     for (let t of n) e += t.length + 1;
     return e
 }
 
 function Mo(n, e, t = 0, i = 1e9) {
     for (let r = 0, s = 0, o = !0; s < n.length && r <= i; s++) {
@@ -3635,63 +3635,63 @@
     }
 }
 typeof Symbol != "undefined" && (De.prototype[Symbol.iterator] = function() {
     return this.iter()
 }, rs.prototype[Symbol.iterator] = Gu.prototype[Symbol.iterator] = Ku.prototype[Symbol.iterator] = function() {
     return this
 });
-class o0 {
+class l0 {
     constructor(e, t, i, r) {
         this.from = e, this.to = t, this.number = i, this.text = r
     }
     get length() {
         return this.to - this.from
     }
 }
 
 function wr(n, e, t) {
     return e = Math.max(0, Math.min(n.length, e)), [e, Math.max(e, Math.min(n.length, t))]
 }
 let pr = "lc,34,7n,7,7b,19,,,,2,,2,,,20,b,1c,l,g,,2t,7,2,6,2,2,,4,z,,u,r,2j,b,1m,9,9,,o,4,,9,,3,,5,17,3,3b,f,,w,1j,,,,4,8,4,,3,7,a,2,t,,1m,,,,2,4,8,,9,,a,2,q,,2,2,1l,,4,2,4,2,2,3,3,,u,2,3,,b,2,1l,,4,5,,2,4,,k,2,m,6,,,1m,,,2,,4,8,,7,3,a,2,u,,1n,,,,c,,9,,14,,3,,1l,3,5,3,,4,7,2,b,2,t,,1m,,2,,2,,3,,5,2,7,2,b,2,s,2,1l,2,,,2,4,8,,9,,a,2,t,,20,,4,,2,3,,,8,,29,,2,7,c,8,2q,,2,9,b,6,22,2,r,,,,,,1j,e,,5,,2,5,b,,10,9,,2u,4,,6,,2,2,2,p,2,4,3,g,4,d,,2,2,6,,f,,jj,3,qa,3,t,3,t,2,u,2,1s,2,,7,8,,2,b,9,,19,3,3b,2,y,,3a,3,4,2,9,,6,3,63,2,2,,1m,,,7,,,,,2,8,6,a,2,,1c,h,1r,4,1c,7,,,5,,14,9,c,2,w,4,2,2,,3,1k,,,2,3,,,3,1m,8,2,2,48,3,,d,,7,4,,6,,3,2,5i,1m,,5,ek,,5f,x,2da,3,3x,,2o,w,fe,6,2x,2,n9w,4,,a,w,2,28,2,7k,,3,,4,,p,2,5,,47,2,q,i,d,,12,8,p,b,1a,3,1c,,2,4,2,2,13,,1v,6,2,2,2,2,c,,8,,1b,,1f,,,3,2,2,5,2,,,16,2,8,,6m,,2,,4,,fn4,,kh,g,g,g,a6,2,gt,,6a,,45,5,1ae,3,,2,5,4,14,3,4,,4l,2,fx,4,ar,2,49,b,4w,,1i,f,1k,3,1d,4,2,2,1x,3,10,5,,8,1q,,c,2,1g,9,a,4,2,,2n,3,2,,,2,6,,4g,,3,8,l,2,1l,2,,,,,m,,e,7,3,5,5f,8,2,3,,,n,,29,,2,6,,,2,,,2,,2,6j,,2,4,6,2,,2,r,2,2d,8,2,,,2,2y,,,,2,6,,,2t,3,2,4,,5,77,9,,2,6t,,a,2,,,4,,40,4,2,2,4,,w,a,14,6,2,4,8,,9,6,2,3,1a,d,,2,ba,7,,6,,,2a,m,2,7,,2,,2,3e,6,3,,,2,,7,,,20,2,3,,,,9n,2,f0b,5,1n,7,t4,,1r,4,29,,f5k,2,43q,,,3,4,5,8,8,2,7,u,4,44,3,1iz,1j,4,1e,8,,e,,m,5,,f,11s,7,,h,2,7,,2,,5,79,7,c5,4,15s,7,31,7,240,5,gx7k,2o,3k,6o".split(",").map(n => n ? parseInt(n, 36) : 1);
 for (let n = 1; n < pr.length; n++) pr[n] += pr[n - 1];
 
-function l0(n) {
+function a0(n) {
     for (let e = 1; e < pr.length; e += 2)
         if (pr[e] > n) return pr[e - 1] <= n;
     return !1
 }
 
 function _c(n) {
     return n >= 127462 && n <= 127487
 }
 const Hc = 8205;
 
 function mt(n, e, t = !0, i = !0) {
-    return (t ? Xu : a0)(n, e, i)
+    return (t ? Xu : h0)(n, e, i)
 }
 
 function Xu(n, e, t) {
     if (e == n.length) return e;
     e && Yu(n.charCodeAt(e)) && Ju(n.charCodeAt(e - 1)) && e--;
     let i = pt(n, e);
     for (e += ti(i); e < n.length;) {
         let r = pt(n, e);
-        if (i == Hc || r == Hc || t && l0(r)) e += ti(r), i = r;
+        if (i == Hc || r == Hc || t && a0(r)) e += ti(r), i = r;
         else if (_c(r)) {
             let s = 0,
                 o = e - 2;
             for (; o >= 0 && _c(pt(n, o));) s++, o -= 2;
             if (s % 2 == 0) break;
             e += 2
         } else break
     }
     return e
 }
 
-function a0(n, e, t) {
+function h0(n, e, t) {
     for (; e > 0;) {
         let i = Xu(n, e - 2, t);
         if (i < e) return i;
         e--
     }
     return 0
 }
@@ -3863,16 +3863,16 @@
             s = new cs(this);
         e: for (let o = 0, l = 0;;) {
             let h = o == e.length ? 1e9 : e[o++];
             for (; l < h || l == h && s.len == 0;) {
                 if (s.done) break e;
                 let u = Math.min(s.len, h - l);
                 vt(r, u, -1);
-                let g = s.ins == -1 ? -1 : s.off == 0 ? s.ins : 0;
-                vt(t, u, g), g > 0 && un(i, t, s.text), s.forward(u), l += u
+                let m = s.ins == -1 ? -1 : s.off == 0 ? s.ins : 0;
+                vt(t, u, m), m > 0 && un(i, t, s.text), s.forward(u), l += u
             }
             let f = e[o++];
             for (; l < f;) {
                 if (s.done) break e;
                 let u = Math.min(s.len, f - l);
                 vt(t, u, -1), vt(r, u, s.ins == -1 ? -1 : s.off == 0 ? s.ins : 0), s.forward(u), l += u
             }
@@ -3896,35 +3896,35 @@
             s = [],
             o = 0,
             l = null;
 
         function h(u = !1) {
             if (!u && !r.length) return;
             o < t && vt(r, t - o, -1);
-            let g = new it(r, s);
-            l = l ? l.compose(g.map(l)) : g, r = [], s = [], o = 0
+            let m = new it(r, s);
+            l = l ? l.compose(m.map(l)) : m, r = [], s = [], o = 0
         }
 
         function f(u) {
             if (Array.isArray(u))
-                for (let g of u) f(g);
+                for (let m of u) f(m);
             else if (u instanceof it) {
                 if (u.length != t) throw new RangeError(`Mismatched change set length (got ${u.length}, expected ${t})`);
                 h(), l = l ? l.compose(u.map(l)) : u
             } else {
                 let {
-                    from: g,
-                    to: y = g,
+                    from: m,
+                    to: y = m,
                     insert: k
                 } = u;
-                if (g > y || g < 0 || y > t) throw new RangeError(`Invalid change range ${g} to ${y} (in doc of length ${t})`);
+                if (m > y || m < 0 || y > t) throw new RangeError(`Invalid change range ${m} to ${y} (in doc of length ${t})`);
                 let v = k ? typeof k == "string" ? De.of(k.split(i || Ra)) : k : De.empty,
-                    C = v.length;
-                if (g == y && C == 0) return;
-                g < o && h(), g > o && vt(r, g - o, -1), vt(r, y - g, C), un(s, r, v), o = y
+                    A = v.length;
+                if (m == y && A == 0) return;
+                m < o && h(), m > o && vt(r, m - o, -1), vt(r, y - m, A), un(s, r, v), o = y
             }
         }
         return f(e), h(!l), l
     }
     static empty(e) {
         return new it(e ? [e, -1] : [], [])
     }
@@ -3972,17 +3972,17 @@
     for (let r = 0, s = 0, o = 0; o < n.sections.length;) {
         let l = n.sections[o++],
             h = n.sections[o++];
         if (h < 0) r += l, s += l;
         else {
             let f = r,
                 u = s,
-                g = De.empty;
-            for (; f += l, u += h, h && i && (g = g.append(i[o - 2 >> 1])), !(t || o == n.sections.length || n.sections[o + 1] < 0);) l = n.sections[o++], h = n.sections[o++];
-            e(r, f, s, u, g), r = f, s = u
+                m = De.empty;
+            for (; f += l, u += h, h && i && (m = m.append(i[o - 2 >> 1])), !(t || o == n.sections.length || n.sections[o + 1] < 0);) l = n.sections[o++], h = n.sections[o++];
+            e(r, f, s, u, m), r = f, s = u
         }
     }
 }
 
 function Pa(n, e, t, i = !1) {
     let r = [],
         s = i ? [] : null,
@@ -4000,16 +4000,16 @@
         }
         l.next()
     } else if (o.ins >= 0) {
         let f = 0,
             u = o.len;
         for (; u;)
             if (l.ins == -1) {
-                let g = Math.min(u, l.len);
-                f += g, u -= g, l.forward(g)
+                let m = Math.min(u, l.len);
+                f += m, u -= m, l.forward(m)
             } else if (l.ins == 0 && l.len < u) u -= l.len, l.next();
         else break;
         vt(r, f, h < o.i ? o.ins : 0), s && h < o.i && un(s, r, o.text), h = o.i, o.forward(o.len - u)
     } else {
         if (o.done && l.done) return s ? it.createSet(r, s) : _i.create(r);
         throw new Error("Mismatched change set lengths")
     }
@@ -4238,33 +4238,33 @@
             r = this.facet.compareInput,
             s = this.id,
             o = e[s] >> 1,
             l = this.type == 2,
             h = !1,
             f = !1,
             u = [];
-        for (let g of this.dependencies) g == "doc" ? h = !0 : g == "selection" ? f = !0 : ((t = e[g.id]) !== null && t !== void 0 ? t : 1) & 1 || u.push(e[g.id]);
+        for (let m of this.dependencies) m == "doc" ? h = !0 : m == "selection" ? f = !0 : ((t = e[m.id]) !== null && t !== void 0 ? t : 1) & 1 || u.push(e[m.id]);
         return {
-            create(g) {
-                return g.values[o] = i(g), 1
+            create(m) {
+                return m.values[o] = i(m), 1
             },
-            update(g, y) {
-                if (h && y.docChanged || f && (y.docChanged || y.selection) || Na(g, u)) {
-                    let k = i(g);
-                    if (l ? !Fc(k, g.values[o], r) : !r(k, g.values[o])) return g.values[o] = k, 1
+            update(m, y) {
+                if (h && y.docChanged || f && (y.docChanged || y.selection) || Na(m, u)) {
+                    let k = i(m);
+                    if (l ? !Fc(k, m.values[o], r) : !r(k, m.values[o])) return m.values[o] = k, 1
                 }
                 return 0
             },
-            reconfigure: (g, y) => {
+            reconfigure: (m, y) => {
                 let k, v = y.config.address[s];
                 if (v != null) {
-                    let C = zo(y, v);
-                    if (this.dependencies.every(O => O instanceof Z ? y.facet(O) === g.facet(O) : O instanceof yt ? y.field(O, !1) == g.field(O, !1) : !0) || (l ? Fc(k = i(g), C, r) : r(k = i(g), C))) return g.values[o] = C, 0
-                } else k = i(g);
-                return g.values[o] = k, 1
+                    let A = zo(y, v);
+                    if (this.dependencies.every(O => O instanceof Z ? y.facet(O) === m.facet(O) : O instanceof yt ? y.field(O, !1) == m.field(O, !1) : !0) || (l ? Fc(k = i(m), A, r) : r(k = i(m), A))) return m.values[o] = A, 0
+                } else k = i(m);
+                return m.values[o] = k, 1
             }
         }
     }
 }
 
 function Fc(n, e, t) {
     if (n.length != e.length) return !1;
@@ -4275,27 +4275,27 @@
 
 function Na(n, e) {
     let t = !1;
     for (let i of e) ss(n, i) & 1 && (t = !0);
     return t
 }
 
-function h0(n, e, t) {
+function c0(n, e, t) {
     let i = t.map(h => n[h.id]),
         r = t.map(h => h.type),
         s = i.filter(h => !(h & 1)),
         o = n[e.id] >> 1;
 
     function l(h) {
         let f = [];
         for (let u = 0; u < i.length; u++) {
-            let g = zo(h, i[u]);
+            let m = zo(h, i[u]);
             if (r[u] == 2)
-                for (let y of g) f.push(y);
-            else f.push(g)
+                for (let y of m) f.push(y);
+            else f.push(m)
         }
         return e.combine(f)
     }
     return {
         create(h) {
             for (let f of i) ss(h, f);
             return h.values[o] = l(h), 1
@@ -4303,17 +4303,17 @@
         update(h, f) {
             if (!Na(h, s)) return 0;
             let u = l(h);
             return e.compare(u, h.values[o]) ? 0 : (h.values[o] = u, 1)
         },
         reconfigure(h, f) {
             let u = Na(h, i),
-                g = f.config.facets[e.id],
+                m = f.config.facets[e.id],
                 y = f.facet(e);
-            if (g && !u && Ph(t, g)) return h.values[o] = y, 0;
+            if (m && !u && Ph(t, m)) return h.values[o] = y, 0;
             let k = l(h);
             return e.compare(k, y) ? (h.values[o] = y, 0) : (h.values[o] = k, 1)
         }
     }
 }
 const zc = Z.define({
     static: !0
@@ -4402,41 +4402,41 @@
         let t = this.address[e.id];
         return t == null ? e.default : this.staticValues[t >> 1]
     }
     static resolve(e, t, i) {
         let r = [],
             s = Object.create(null),
             o = new Map;
-        for (let y of c0(e, t, o)) y instanceof yt ? r.push(y) : (s[y.facet.id] || (s[y.facet.id] = [])).push(y);
+        for (let y of f0(e, t, o)) y instanceof yt ? r.push(y) : (s[y.facet.id] || (s[y.facet.id] = [])).push(y);
         let l = Object.create(null),
             h = [],
             f = [];
         for (let y of r) l[y.id] = f.length << 1, f.push(k => y.slot(k));
         let u = i == null ? void 0 : i.config.facets;
         for (let y in s) {
             let k = s[y],
                 v = k[0].facet,
-                C = u && u[y] || [];
+                A = u && u[y] || [];
             if (k.every(O => O.type == 0))
-                if (l[v.id] = h.length << 1 | 1, Ph(C, k)) h.push(i.facet(v));
+                if (l[v.id] = h.length << 1 | 1, Ph(A, k)) h.push(i.facet(v));
                 else {
                     let O = v.combine(k.map(D => D.value));
                     h.push(i && v.compare(O, i.facet(v)) ? i.facet(v) : O)
                 }
             else {
                 for (let O of k) O.type == 0 ? (l[O.id] = h.length << 1 | 1, h.push(O.value)) : (l[O.id] = f.length << 1, f.push(D => O.dynamicSlot(D)));
-                l[v.id] = f.length << 1, f.push(O => h0(O, v, k))
+                l[v.id] = f.length << 1, f.push(O => c0(O, v, k))
             }
         }
-        let g = f.map(y => y(l));
-        return new Fo(e, o, g, l, h, s)
+        let m = f.map(y => y(l));
+        return new Fo(e, o, m, l, h, s)
     }
 }
 
-function c0(n, e, t) {
+function f0(n, e, t) {
     let i = [
             [],
             [],
             [],
             [],
             []
         ],
@@ -4497,23 +4497,23 @@
         combine: n => n.length ? n[0] : !1
     });
 class Xi {
     constructor(e, t) {
         this.type = e, this.value = t
     }
     static define() {
-        return new f0
+        return new u0
     }
 }
-class f0 {
+class u0 {
     of(e) {
         return new Xi(this, e)
     }
 }
-class u0 {
+class d0 {
     constructor(e) {
         this.map = e
     }
     of(e) {
         return new me(this, e)
     }
 }
@@ -4525,15 +4525,15 @@
         let t = this.type.map(this.value, e);
         return t === void 0 ? void 0 : t == this.value ? this : new me(this.type, t)
     }
     is(e) {
         return this.type == e
     }
     static define(e = {}) {
-        return new u0(e.map || (t => t))
+        return new d0(e.map || (t => t))
     }
     static mapEffects(e, t) {
         if (!e.length) return e;
         let i = [];
         for (let r of e) {
             let s = r.map(t);
             s && i.push(s)
@@ -4575,15 +4575,15 @@
     }
 }
 nt.time = Xi.define();
 nt.userEvent = Xi.define();
 nt.addToHistory = Xi.define();
 nt.remote = Xi.define();
 
-function d0(n, e) {
+function p0(n, e) {
     let t = [];
     for (let i = 0, r = 0;;) {
         let s, o;
         if (i < n.length && (r == e.length || e[r] >= n[i])) s = n[i++], o = n[i++];
         else if (r < e.length) s = e[r++], o = e[r++];
         else return t;
         !t.length || t[t.length - 1] < s ? t.push(s, o) : t[t.length - 1] < o && (t[t.length - 1] = o)
@@ -4619,27 +4619,27 @@
     e.length && e[0].filter === !1 && (t = !1);
     for (let s = 1; s < e.length; s++) {
         e[s].filter === !1 && (t = !1);
         let o = !!e[s].sequential;
         i = ad(i, _a(n, e[s], o ? i.changes.newLength : n.doc.length), o)
     }
     let r = nt.create(n, i.changes, i.selection, i.effects, i.annotations, i.scrollIntoView);
-    return g0(t ? p0(r) : r)
+    return m0(t ? g0(r) : r)
 }
 
-function p0(n) {
+function g0(n) {
     let e = n.startState,
         t = !0;
     for (let r of e.facet(rd)) {
         let s = r(n);
         if (s === !1) {
             t = !1;
             break
         }
-        Array.isArray(s) && (t = t === !0 ? s : d0(t, s))
+        Array.isArray(s) && (t = t === !0 ? s : p0(t, s))
     }
     if (t !== !0) {
         let r, s;
         if (t === !1) s = n.changes.invertedDesc, r = it.empty(e.doc.length);
         else {
             let o = n.changes.filter(t);
             r = o.changes, s = o.filtered.mapDesc(o.changes).invertedDesc
@@ -4650,51 +4650,51 @@
     for (let r = i.length - 1; r >= 0; r--) {
         let s = i[r](n);
         s instanceof nt ? n = s : Array.isArray(s) && s.length == 1 && s[0] instanceof nt ? n = s[0] : n = hd(e, gr(s), !1)
     }
     return n
 }
 
-function g0(n) {
+function m0(n) {
     let e = n.startState,
         t = e.facet(od),
         i = n;
     for (let r = t.length - 1; r >= 0; r--) {
         let s = t[r](n);
         s && Object.keys(s).length && (i = ad(i, _a(e, s, n.changes.newLength), !0))
     }
     return i == n ? n : nt.create(e, n.changes, n.selection, i.effects, i.annotations, i.scrollIntoView)
 }
-const m0 = [];
+const y0 = [];
 
 function gr(n) {
-    return n == null ? m0 : Array.isArray(n) ? n : [n]
+    return n == null ? y0 : Array.isArray(n) ? n : [n]
 }
 var Ve = function(n) {
     return n[n.Word = 0] = "Word", n[n.Space = 1] = "Space", n[n.Other = 2] = "Other", n
 }(Ve || (Ve = {}));
-const y0 = /[\u00df\u0587\u0590-\u05f4\u0600-\u06ff\u3040-\u309f\u30a0-\u30ff\u3400-\u4db5\u4e00-\u9fcc\uac00-\ud7af]/;
+const b0 = /[\u00df\u0587\u0590-\u05f4\u0600-\u06ff\u3040-\u309f\u30a0-\u30ff\u3400-\u4db5\u4e00-\u9fcc\uac00-\ud7af]/;
 let Ha;
 try {
     Ha = new RegExp("[\\p{Alphabetic}\\p{Number}_]", "u")
 } catch (n) {}
 
-function b0(n) {
+function x0(n) {
     if (Ha) return Ha.test(n);
     for (let e = 0; e < n.length; e++) {
         let t = n[e];
-        if (/\w/.test(t) || t > "" && (t.toUpperCase() != t.toLowerCase() || y0.test(t))) return !0
+        if (/\w/.test(t) || t > "" && (t.toUpperCase() != t.toLowerCase() || b0.test(t))) return !0
     }
     return !1
 }
 
-function x0(n) {
+function k0(n) {
     return e => {
         if (!/\S/.test(e)) return Ve.Space;
-        if (b0(e)) return Ve.Word;
+        if (x0(e)) return Ve.Word;
         for (let t = 0; t < n.length; t++)
             if (e.indexOf(n[t]) > -1) return Ve.Word;
         return Ve.Other
     }
 }
 class Ee {
     constructor(e, t, i, r, s, o) {
@@ -4742,16 +4742,16 @@
             s = [i.range],
             o = gr(i.effects);
         for (let l = 1; l < t.ranges.length; l++) {
             let h = e(t.ranges[l]),
                 f = this.changes(h.changes),
                 u = f.map(r);
             for (let y = 0; y < l; y++) s[y] = s[y].map(u);
-            let g = r.mapDesc(f, !0);
-            s.push(h.range.map(g)), r = r.compose(u), o = me.mapEffects(o, u).concat(me.mapEffects(gr(h.effects), g))
+            let m = r.mapDesc(f, !0);
+            s.push(h.range.map(m)), r = r.compose(u), o = me.mapEffects(o, u).concat(me.mapEffects(gr(h.effects), m))
         }
         return {
             changes: r,
             selection: H.create(s, t.mainIndex),
             effects: o
         }
     }
@@ -4827,15 +4827,15 @@
     languageDataAt(e, t, i = -1) {
         let r = [];
         for (let s of this.facet(id))
             for (let o of s(this, t, i)) Object.prototype.hasOwnProperty.call(o, e) && r.push(o[e]);
         return r
     }
     charCategorizer(e) {
-        return x0(this.languageDataAt("wordChars", e).join(""))
+        return k0(this.languageDataAt("wordChars", e).join(""))
     }
     wordAt(e) {
         let {
             text: t,
             from: i,
             length: r
         } = this.doc.lineAt(e), s = this.charCategorizer(e), o = e - i, l = e - i;
@@ -4934,20 +4934,20 @@
             r = [],
             s = [],
             o = -1,
             l = -1;
         for (let h = 0; h < this.value.length; h++) {
             let f = this.value[h],
                 u = this.from[h] + e,
-                g = this.to[h] + e,
+                m = this.to[h] + e,
                 y, k;
-            if (u == g) {
+            if (u == m) {
                 let v = t.mapPos(u, f.startSide, f.mapMode);
                 if (v == null || (y = k = v, f.startSide != f.endSide && (k = t.mapPos(u, f.endSide), k < y))) continue
-            } else if (y = t.mapPos(u, f.startSide), k = t.mapPos(g, f.endSide), y > k || y == k && f.startSide > 0 && f.endSide <= 0) continue;
+            } else if (y = t.mapPos(u, f.startSide), k = t.mapPos(m, f.endSide), y > k || y == k && f.startSide > 0 && f.endSide <= 0) continue;
             (k - y || f.endSide - f.startSide) < 0 || (o < 0 && (o = y), f.point && (l = Math.max(l, k - y)), i.push(f), r.push(y - o), s.push(k - o))
         }
         return {
             mapped: i.length ? new Nh(r, s, i, l) : null,
             pos: o
         }
     }
@@ -4983,16 +4983,16 @@
         if (i && (t = t.slice().sort(za)), this.isEmpty) return t.length ? Pe.of(t) : this;
         let l = new fd(this, null, -1).goto(0),
             h = 0,
             f = [],
             u = new xn;
         for (; l.value || h < t.length;)
             if (h < t.length && (l.from - t[h].from || l.startSide - t[h].value.startSide) >= 0) {
-                let g = t[h++];
-                u.addInner(g.from, g.to, g.value) || f.push(g)
+                let m = t[h++];
+                u.addInner(m.from, m.to, m.value) || f.push(m)
             } else l.rangeIndex == 1 && l.chunkIndex < this.chunk.length && (h == t.length || this.chunkEnd(l.chunkIndex) < t[h].from) && (!o || r > this.chunkEnd(l.chunkIndex) || s < this.chunkPos[l.chunkIndex]) && u.addChunk(this.chunkPos[l.chunkIndex], this.chunk[l.chunkIndex]) ? l.nextChunk() : ((!o || r > l.to || s < l.from || o(l.from, l.to, l.value)) && (u.addInner(l.from, l.to, l.value) || f.push(Fa.create(l.from, l.to, l.value))), l.next());
         return u.finishInner(this.nextLayer.isEmpty && !f.length ? Pe.empty : this.nextLayer.update({
             add: f,
             filter: o,
             filterFrom: r,
             filterTo: s
         }))
@@ -5006,17 +5006,17 @@
             let l = this.chunkPos[o],
                 h = this.chunk[o],
                 f = e.touchesRange(l, l + h.length);
             if (f === !1) r = Math.max(r, h.maxPoint), t.push(h), i.push(e.mapPos(l));
             else if (f === !0) {
                 let {
                     mapped: u,
-                    pos: g
+                    pos: m
                 } = h.map(l, e);
-                u && (r = Math.max(r, u.maxPoint), t.push(u), i.push(g))
+                u && (r = Math.max(r, u.maxPoint), t.push(u), i.push(m))
             }
         }
         let s = this.nextLayer.map(e);
         return t.length == 0 ? s : new Pe(i, t, s || Pe.empty, r)
     }
     between(e, t, i) {
         if (!this.isEmpty) {
@@ -5034,20 +5034,20 @@
     get isEmpty() {
         return this.nextLayer == this
     }
     static iter(e, t = 0) {
         return fs.from(e).goto(t)
     }
     static compare(e, t, i, r, s = -1) {
-        let o = e.filter(g => g.maxPoint > 0 || !g.isEmpty && g.maxPoint >= s),
-            l = t.filter(g => g.maxPoint > 0 || !g.isEmpty && g.maxPoint >= s),
+        let o = e.filter(m => m.maxPoint > 0 || !m.isEmpty && m.maxPoint >= s),
+            l = t.filter(m => m.maxPoint > 0 || !m.isEmpty && m.maxPoint >= s),
             h = $c(o, l, i),
             f = new qr(o, h, s),
             u = new qr(l, h, s);
-        i.iterGaps((g, y, k) => Wc(f, g, u, y, k, r)), i.empty && i.length == 0 && Wc(f, 0, u, 0, 0, r)
+        i.iterGaps((m, y, k) => Wc(f, m, u, y, k, r)), i.empty && i.length == 0 && Wc(f, 0, u, 0, 0, r)
     }
     static eq(e, t, i = 0, r) {
         r == null && (r = 999999999);
         let s = e.filter(u => !u.isEmpty && t.indexOf(u) < 0),
             o = t.filter(u => !u.isEmpty && e.indexOf(u) < 0);
         if (s.length != o.length) return !1;
         if (!s.length) return !0;
@@ -5064,30 +5064,30 @@
         let o = new qr(e, null, s).goto(t),
             l = t,
             h = o.openStart;
         for (;;) {
             let f = Math.min(o.to, i);
             if (o.point) {
                 let u = o.activeForPoint(o.to),
-                    g = o.pointFrom < t ? u.length + 1 : Math.min(u.length, h);
-                r.point(l, f, o.point, u, g, o.pointRank), h = Math.min(o.openEnd(f), u.length)
+                    m = o.pointFrom < t ? u.length + 1 : Math.min(u.length, h);
+                r.point(l, f, o.point, u, m, o.pointRank), h = Math.min(o.openEnd(f), u.length)
             } else f > l && (r.span(l, f, o.active, h), h = o.openEnd(f));
             if (o.to > i) return h + (o.point && o.to > i ? 1 : 0);
             l = o.to, o.next()
         }
     }
     static of (e, t = !1) {
         let i = new xn;
-        for (let r of e instanceof Fa ? [e] : t ? k0(e) : e) i.add(r.from, r.to, r.value);
+        for (let r of e instanceof Fa ? [e] : t ? w0(e) : e) i.add(r.from, r.to, r.value);
         return i.finish()
     }
 }
 Pe.empty = new Pe([], [], null, -1);
 
-function k0(n) {
+function w0(n) {
     if (n.length > 1)
         for (let e = n[0], t = 1; t < n.length; t++) {
             let i = n[t];
             if (za(e, i) > 0) return n.slice().sort(za);
             e = i
         }
     return n
@@ -5308,16 +5308,16 @@
     n.goto(e), t.goto(i);
     let o = i + r,
         l = i,
         h = i - e;
     for (;;) {
         let f = n.to + h - t.to || n.endSide - t.endSide,
             u = f < 0 ? n.to + h : t.to,
-            g = Math.min(u, o);
-        if (n.point || t.point ? n.point && t.point && (n.point == t.point || n.point.eq(t.point)) && $a(n.activeForPoint(n.to), t.activeForPoint(t.to)) || s.comparePoint(l, g, n.point, t.point) : g > l && !$a(n.active, t.active) && s.compareRange(l, g, n.active, t.active), u > o) break;
+            m = Math.min(u, o);
+        if (n.point || t.point ? n.point && t.point && (n.point == t.point || n.point.eq(t.point)) && $a(n.activeForPoint(n.to), t.activeForPoint(t.to)) || s.comparePoint(l, m, n.point, t.point) : m > l && !$a(n.active, t.active) && s.compareRange(l, m, n.active, t.active), u > o) break;
         l = u, f <= 0 && n.next(), f >= 0 && t.next()
     }
 }
 
 function $a(n, e) {
     if (n.length != e.length) return !1;
     for (let t = 0; t < n.length; t++)
@@ -5344,15 +5344,15 @@
 
 function Os(n, e, t = n.length) {
     let i = 0;
     for (let r = 0; r < t;) n.charCodeAt(r) == 9 ? (i += e - i % e, r++) : (i++, r = mt(n, r));
     return i
 }
 
-function w0(n, e, t, i) {
+function v0(n, e, t, i) {
     for (let r = 0, s = 0;;) {
         if (s >= e) return r;
         if (r == n.length) break;
         s += n.charCodeAt(r) == 9 ? t - s % t : 1, r = mt(n, r)
     }
     return i === !0 ? -1 : n.length
 }
@@ -5369,44 +5369,44 @@
 
         function r(o) {
             return /^@/.test(o) ? [o] : o.split(/,\s*/)
         }
 
         function s(o, l, h, f) {
             let u = [],
-                g = /^@(\w+)\b/.exec(o[0]),
-                y = g && g[1] == "keyframes";
-            if (g && l == null) return h.push(o[0] + ";");
+                m = /^@(\w+)\b/.exec(o[0]),
+                y = m && m[1] == "keyframes";
+            if (m && l == null) return h.push(o[0] + ";");
             for (let k in l) {
                 let v = l[k];
-                if (/&/.test(k)) s(k.split(/,\s*/).map(C => o.map(O => C.replace(/&/, O))).reduce((C, O) => C.concat(O)), v, h);
+                if (/&/.test(k)) s(k.split(/,\s*/).map(A => o.map(O => A.replace(/&/, O))).reduce((A, O) => A.concat(O)), v, h);
                 else if (v && typeof v == "object") {
-                    if (!g) throw new RangeError("The value of a property (" + k + ") should be a primitive value.");
+                    if (!m) throw new RangeError("The value of a property (" + k + ") should be a primitive value.");
                     s(r(k), v, u, y)
-                } else v != null && u.push(k.replace(/_.*/, "").replace(/[A-Z]/g, C => "-" + C.toLowerCase()) + ": " + v + ";")
-            }(u.length || y) && h.push((i && !g && !f ? o.map(i) : o).join(", ") + " {" + u.join(" ") + "}")
+                } else v != null && u.push(k.replace(/_.*/, "").replace(/[A-Z]/g, A => "-" + A.toLowerCase()) + ": " + v + ";")
+            }(u.length || y) && h.push((i && !m && !f ? o.map(i) : o).join(", ") + " {" + u.join(" ") + "}")
         }
         for (let o in e) s(r(o), e[o], this.rules)
     }
     getRules() {
         return this.rules.join(`
 `)
     }
     static newName() {
         let e = Vc[jc] || 1;
         return Vc[jc] = e + 1, Wa + e.toString(36)
     }
     static mount(e, t, i) {
         let r = e[qa],
             s = i && i.nonce;
-        r ? s && r.setNonce(s) : r = new v0(e, s), r.mount(Array.isArray(t) ? t : [t])
+        r ? s && r.setNonce(s) : r = new S0(e, s), r.mount(Array.isArray(t) ? t : [t])
     }
 }
 let Uc = new Map;
-class v0 {
+class S0 {
     constructor(e, t) {
         let i = e.ownerDocument || e,
             r = i.defaultView;
         if (!e.head && e.adoptedStyleSheets && r.CSSStyleSheet) {
             let s = Uc.get(i);
             if (s) return e.adoptedStyleSheets = [s.sheet, ...e.adoptedStyleSheets], e[qa] = s;
             this.sheet = new r.CSSStyleSheet, e.adoptedStyleSheets = [this.sheet, ...e.adoptedStyleSheets], Uc.set(i, this)
@@ -5519,37 +5519,37 @@
         191: "?",
         192: "~",
         219: "{",
         220: "|",
         221: "}",
         222: '"'
     },
-    S0 = typeof navigator != "undefined" && /Mac/.test(navigator.platform),
-    C0 = typeof navigator != "undefined" && /MSIE \d|Trident\/(?:[7-9]|\d{2,})\..*rv:(\d+)/.exec(navigator.userAgent);
+    C0 = typeof navigator != "undefined" && /Mac/.test(navigator.platform),
+    A0 = typeof navigator != "undefined" && /MSIE \d|Trident\/(?:[7-9]|\d{2,})\..*rv:(\d+)/.exec(navigator.userAgent);
 for (var gt = 0; gt < 10; gt++) wn[48 + gt] = wn[96 + gt] = String(gt);
 for (var gt = 1; gt <= 24; gt++) wn[gt + 111] = "F" + gt;
 for (var gt = 65; gt <= 90; gt++) wn[gt] = String.fromCharCode(gt + 32), us[gt] = String.fromCharCode(gt);
 for (var ea in wn) us.hasOwnProperty(ea) || (us[ea] = wn[ea]);
 
-function A0(n) {
-    var e = S0 && n.metaKey && n.shiftKey && !n.ctrlKey && !n.altKey || C0 && n.shiftKey && n.key && n.key.length == 1 || n.key == "Unidentified",
+function T0(n) {
+    var e = C0 && n.metaKey && n.shiftKey && !n.ctrlKey && !n.altKey || A0 && n.shiftKey && n.key && n.key.length == 1 || n.key == "Unidentified",
         t = !e && n.key || (n.shiftKey ? us : wn)[n.keyCode] || n.key || "Unidentified";
     return t == "Esc" && (t = "Escape"), t == "Del" && (t = "Delete"), t == "Left" && (t = "ArrowLeft"), t == "Up" && (t = "ArrowUp"), t == "Right" && (t = "ArrowRight"), t == "Down" && (t = "ArrowDown"), t
 }
 
 function $o(n) {
     let e;
     return n.nodeType == 11 ? e = n.getSelection ? n : n.ownerDocument : e = n, e.getSelection()
 }
 
 function ja(n, e) {
     return e ? n == e || n.contains(e.nodeType != 1 ? e.parentNode : e) : !1
 }
 
-function T0(n) {
+function O0(n) {
     let e = n.activeElement;
     for (; e && e.shadowRoot;) e = e.shadowRoot.activeElement;
     return e
 }
 
 function Do(n, e) {
     if (!e.anchorNode) return !1;
@@ -5598,15 +5598,15 @@
         left: t,
         right: t,
         top: n.top,
         bottom: n.bottom
     }
 }
 
-function O0(n) {
+function M0(n) {
     return {
         left: 0,
         right: n.innerWidth,
         top: 0,
         bottom: n.innerHeight
     }
 }
@@ -5616,37 +5616,37 @@
         i = e.height / n.offsetHeight;
     return (t > .995 && t < 1.005 || !isFinite(t) || Math.abs(e.width - n.offsetWidth) < 1) && (t = 1), (i > .995 && i < 1.005 || !isFinite(i) || Math.abs(e.height - n.offsetHeight) < 1) && (i = 1), {
         scaleX: t,
         scaleY: i
     }
 }
 
-function M0(n, e, t, i, r, s, o, l) {
+function E0(n, e, t, i, r, s, o, l) {
     let h = n.ownerDocument,
         f = h.defaultView || window;
-    for (let u = n, g = !1; u && !g;)
+    for (let u = n, m = !1; u && !m;)
         if (u.nodeType == 1) {
             let y, k = u == h.body,
                 v = 1,
-                C = 1;
-            if (k) y = O0(f);
+                A = 1;
+            if (k) y = M0(f);
             else {
-                if (/^(fixed|sticky)$/.test(getComputedStyle(u).position) && (g = !0), u.scrollHeight <= u.clientHeight && u.scrollWidth <= u.clientWidth) {
+                if (/^(fixed|sticky)$/.test(getComputedStyle(u).position) && (m = !0), u.scrollHeight <= u.clientHeight && u.scrollWidth <= u.clientWidth) {
                     u = u.assignedSlot || u.parentNode;
                     continue
                 }
                 let F = u.getBoundingClientRect();
                 ({
                     scaleX: v,
-                    scaleY: C
+                    scaleY: A
                 } = ud(u, F)), y = {
                     left: F.left,
                     right: F.left + u.clientWidth * v,
                     top: F.top,
-                    bottom: F.top + u.clientHeight * C
+                    bottom: F.top + u.clientHeight * A
                 }
             }
             let O = 0,
                 D = 0;
             if (r == "nearest") e.top < y.top ? (D = -(y.top - e.top + o), t > 0 && e.bottom > y.bottom + D && (D = e.bottom - y.bottom + D + o)) : e.bottom > y.bottom && (D = e.bottom - y.bottom + o, t < 0 && e.top - D < y.top && (D = -(y.top + D - e.top + o)));
             else {
                 let F = e.bottom - e.top,
@@ -5656,15 +5656,15 @@
             if (i == "nearest" ? e.left < y.left ? (O = -(y.left - e.left + s), t > 0 && e.right > y.right + O && (O = e.right - y.right + O + s)) : e.right > y.right && (O = e.right - y.right + s, t < 0 && e.left < y.left + O && (O = -(y.left + O - e.left + s))) : O = (i == "center" ? e.left + (e.right - e.left) / 2 - (y.right - y.left) / 2 : i == "start" == l ? e.left - s : e.right - (y.right - y.left) + s) - y.left, O || D)
                 if (k) f.scrollBy(O, D);
                 else {
                     let F = 0,
                         $ = 0;
                     if (D) {
                         let j = u.scrollTop;
-                        u.scrollTop += D / C, $ = (u.scrollTop - j) * C
+                        u.scrollTop += D / A, $ = (u.scrollTop - j) * A
                     }
                     if (O) {
                         let j = u.scrollLeft;
                         u.scrollLeft += O / v, F = (u.scrollLeft - j) * v
                     }
                     e = {
                         left: e.left - F,
@@ -5674,25 +5674,25 @@
                     }, F && Math.abs(F - O) < 1 && (i = "nearest"), $ && Math.abs($ - D) < 1 && (r = "nearest")
                 } if (k) break;
             u = u.assignedSlot || u.parentNode
         } else if (u.nodeType == 11) u = u.host;
     else break
 }
 
-function E0(n) {
+function D0(n) {
     let e = n.ownerDocument;
     for (let t = n.parentNode; t && t != e.body;)
         if (t.nodeType == 1) {
             if (t.scrollHeight > t.clientHeight || t.scrollWidth > t.clientWidth) return t;
             t = t.assignedSlot || t.parentNode
         } else if (t.nodeType == 11) t = t.host;
     else break;
     return null
 }
-class D0 {
+class R0 {
     constructor() {
         this.anchorNode = null, this.anchorOffset = 0, this.focusNode = null, this.focusOffset = 0
     }
     eq(e) {
         return this.anchorNode == e.anchorNode && this.anchorOffset == e.anchorOffset && this.focusNode == e.focusNode && this.focusOffset == e.focusOffset
     }
     setRange(e) {
@@ -5746,27 +5746,27 @@
         },
         r = new KeyboardEvent("keydown", i);
     r.synthetic = !0, n.dispatchEvent(r);
     let s = new KeyboardEvent("keyup", i);
     return s.synthetic = !0, n.dispatchEvent(s), r.defaultPrevented || s.defaultPrevented
 }
 
-function R0(n) {
+function L0(n) {
     for (; n;) {
         if (n && (n.nodeType == 9 || n.nodeType == 11 && n.host)) return n;
         n = n.assignedSlot || n.parentNode
     }
     return null
 }
 
 function pd(n) {
     for (; n.attributes.length;) n.removeAttributeNode(n.attributes[0])
 }
 
-function L0(n, e) {
+function P0(n, e) {
     let t = e.focusNode,
         i = e.focusOffset;
     if (!t || e.anchorNode != t || e.anchorOffset != i) return !1;
     for (i = Math.min(i, Ui(t));;)
         if (i) {
             if (t.nodeType != 1) return !1;
             let r = t.childNodes[i - 1];
@@ -5862,22 +5862,22 @@
     }
     domBoundsAround(e, t, i = 0) {
         let r = -1,
             s = -1,
             o = -1,
             l = -1;
         for (let h = 0, f = i, u = i; h < this.children.length; h++) {
-            let g = this.children[h],
-                y = f + g.length;
-            if (f < e && y > t) return g.domBoundsAround(e, t, f);
-            if (y >= e && r == -1 && (r = h, s = f), f > t && g.dom.parentNode == this.dom) {
+            let m = this.children[h],
+                y = f + m.length;
+            if (f < e && y > t) return m.domBoundsAround(e, t, f);
+            if (y >= e && r == -1 && (r = h, s = f), f > t && m.dom.parentNode == this.dom) {
                 o = h, l = u;
                 break
             }
-            u = y, f = y + g.breakAfter
+            u = y, f = y + m.breakAfter
         }
         return {
             from: s,
             to: l < 0 ? i + this.length : l,
             startDOM: (r ? this.children[r - 1].dom.nextSibling : null) || this.dom.firstChild,
             endDOM: o < this.children.length && o >= 0 ? this.children[o].dom : null
         }
@@ -5976,19 +5976,19 @@
         }
     }
 }
 
 function yd(n, e, t, i, r, s, o, l, h) {
     let {
         children: f
-    } = n, u = f.length ? f[e] : null, g = s.length ? s[s.length - 1] : null, y = g ? g.breakAfter : o;
-    if (!(e == i && u && !o && !y && s.length < 2 && u.merge(t, r, s.length ? g : null, t == 0, l, h))) {
+    } = n, u = f.length ? f[e] : null, m = s.length ? s[s.length - 1] : null, y = m ? m.breakAfter : o;
+    if (!(e == i && u && !o && !y && s.length < 2 && u.merge(t, r, s.length ? m : null, t == 0, l, h))) {
         if (i < f.length) {
             let k = f[i];
-            k && (r < k.length || k.breakAfter && (g != null && g.breakAfter)) ? (e == i && (k = k.split(r), r = 0), !y && g && k.merge(0, r, g, !0, 0, h) ? s[s.length - 1] = k : ((r || k.children.length && !k.children[0].length) && k.merge(0, r, null, !1, 0, h), s.push(k))) : k != null && k.breakAfter && (g ? g.breakAfter = 1 : o = 1), i++
+            k && (r < k.length || k.breakAfter && (m != null && m.breakAfter)) ? (e == i && (k = k.split(r), r = 0), !y && m && k.merge(0, r, m, !0, 0, h) ? s[s.length - 1] = k : ((r || k.children.length && !k.children[0].length) && k.merge(0, r, null, !1, 0, h), s.push(k))) : k != null && k.breakAfter && (m ? m.breakAfter = 1 : o = 1), i++
         }
         for (u && (u.breakAfter = o, t > 0 && (!o && s.length && u.merge(t, u.length, s[0], !1, l, 0) ? u.breakAfter = s.shift().breakAfter : (t < u.length || u.children.length && u.children[u.children.length - 1].length == 0) && u.merge(t, u.length, null, !1, l, 0), e++)); e < i && s.length;)
             if (f[i - 1].become(s[s.length - 1])) i--, s.pop(), h = s.length ? 0 : l;
             else if (f[e].become(s[0])) e++, s.shift(), l = s.length ? 0 : h;
         else break;
         !s.length && e && i < f.length && !f[e - 1].breakAfter && f[i].merge(0, 0, f[e - 1], !1, l, h) && e--, (e < i || s.length) && n.replaceChildren(e, i, s)
     }
@@ -6000,17 +6000,17 @@
             i: l,
             off: h
         } = o.findPos(t, 1),
         {
             i: f,
             off: u
         } = o.findPos(e, -1),
-        g = e - t;
-    for (let y of i) g += y.length;
-    n.length += g, yd(n, f, u, l, h, i, 0, r, s)
+        m = e - t;
+    for (let y of i) m += y.length;
+    n.length += m, yd(n, f, u, l, h, i, 0, r, s)
 }
 let Qt = typeof navigator != "undefined" ? navigator : {
         userAgent: "",
         vendor: "",
         platform: ""
     },
     Va = typeof document != "undefined" ? document : {
@@ -6040,15 +6040,15 @@
     ios: Jc,
     android: /Android\b/.test(Qt.userAgent),
     webkit: Yc,
     safari: kd,
     webkit_version: Yc ? +(/\bAppleWebKit\/(\d+)/.exec(navigator.userAgent) || [0, 0])[1] : 0,
     tabSize: Va.documentElement.style.tabSize != null ? "tab-size" : "-moz-tab-size"
 };
-const P0 = 256;
+const N0 = 256;
 class Qi extends je {
     constructor(e) {
         super(), this.text = e
     }
     get length() {
         return this.text.length
     }
@@ -6058,15 +6058,15 @@
     sync(e, t) {
         this.dom || this.createDOM(), this.dom.nodeValue != this.text && (t && t.node == this.dom && (t.written = !0), this.dom.nodeValue = this.text)
     }
     reuseDOM(e) {
         e.nodeType == 3 && this.createDOM(e)
     }
     merge(e, t, i) {
-        return this.flags & 8 || i && (!(i instanceof Qi) || this.length - (t - e) + i.length > P0 || i.flags & 8) ? !1 : (this.text = this.text.slice(0, e) + (i ? i.text : "") + this.text.slice(t), this.markDirty(), !0)
+        return this.flags & 8 || i && (!(i instanceof Qi) || this.length - (t - e) + i.length > N0 || i.flags & 8) ? !1 : (this.text = this.text.slice(0, e) + (i ? i.text : "") + this.text.slice(t), this.markDirty(), !0)
     }
     split(e) {
         let t = new Qi(this.text.slice(e));
         return this.text = this.text.slice(0, e), this.markDirty(), t.flags |= this.flags & 8, t
     }
     localPosFromDOM(e, t) {
         return e == this.dom ? t : t ? this.text.length : 0
@@ -6079,15 +6079,15 @@
             from: i,
             to: i + this.length,
             startDOM: this.dom,
             endDOM: this.dom.nextSibling
         }
     }
     coordsAt(e, t) {
-        return N0(this.dom, e, t)
+        return I0(this.dom, e, t)
     }
 }
 class Gi extends je {
     constructor(e, t = [], i = 0) {
         super(), this.mark = e, this.children = t, this.length = i;
         for (let r of t) r.setParent(this)
     }
@@ -6124,15 +6124,15 @@
         return wd(this, e)
     }
     coordsAt(e, t) {
         return Sd(this, e, t)
     }
 }
 
-function N0(n, e, t) {
+function I0(n, e, t) {
     let i = n.nodeValue.length;
     e > i && (e = i);
     let r = e,
         s = e,
         o = 0;
     e == 0 && t < 0 || e == i && t >= 0 ? ee.chrome || ee.gecko || (e ? (r--, o = 1) : s < i && (s++, o = -1)) : t < 0 ? r-- : s < i && s++;
     let l = Un(n, r, s).getClientRects();
@@ -6289,26 +6289,26 @@
 function Sd(n, e, t) {
     let i = null,
         r = -1,
         s = null,
         o = -1;
 
     function l(f, u) {
-        for (let g = 0, y = 0; g < f.children.length && y <= u; g++) {
-            let k = f.children[g],
+        for (let m = 0, y = 0; m < f.children.length && y <= u; m++) {
+            let k = f.children[m],
                 v = y + k.length;
             v >= u && (k.children.length ? l(k, u - y) : (!s || s.isHidden && t > 0) && (v > u || y == v && k.getSide() > 0) ? (s = k, o = u - y) : (y < u || y == v && k.getSide() < 0 && !k.isHidden) && (i = k, r = u - y)), y = v
         }
     }
     l(n, e);
     let h = (t < 0 ? i : s) || i || s;
-    return h ? h.coordsAt(Math.max(0, h == i ? r : o), t) : I0(n)
+    return h ? h.coordsAt(Math.max(0, h == i ? r : o), t) : B0(n)
 }
 
-function I0(n) {
+function B0(n) {
     let e = n.dom.lastChild;
     if (!e) return n.dom.getBoundingClientRect();
     let t = ds(e);
     return t[t.length - 1] || null
 }
 
 function Ga(n, e) {
@@ -6333,15 +6333,15 @@
     if (e)
         for (let r in e) t && r in t || (i = !0, r == "style" ? n.style.cssText = "" : n.removeAttribute(r));
     if (t)
         for (let r in t) e && e[r] == t[r] || (i = !0, r == "style" ? n.style.cssText = t[r] : n.setAttribute(r, t[r]));
     return i
 }
 
-function B0(n) {
+function _0(n) {
     let e = Object.create(null);
     for (let t = 0; t < n.attributes.length; t++) {
         let i = n.attributes[t];
         e[i.name] = i.value
     }
     return e
 }
@@ -6618,15 +6618,15 @@
     get type() {
         return this.startSide != this.endSide ? Dt.WidgetRange : this.startSide <= 0 ? Dt.WidgetBefore : Dt.WidgetAfter
     }
     get heightRelevant() {
         return this.block || !!this.widget && (this.widget.estimatedHeight >= 5 || this.widget.lineBreaks > 0)
     }
     eq(e) {
-        return e instanceof vn && _0(this.widget, e.widget) && this.block == e.block && this.startSide == e.startSide && this.endSide == e.endSide
+        return e instanceof vn && H0(this.widget, e.widget) && this.block == e.block && this.startSide == e.startSide && this.endSide == e.endSide
     }
     range(e, t = e) {
         if (this.isReplace && (e > t || e == t && this.startSide > 0 && this.endSide <= 0)) throw new RangeError("Invalid range for replacement decoration");
         if (!this.isReplace && t != e) throw new RangeError("Widget decorations can only have zero-length ranges");
         return super.range(e, t)
     }
 }
@@ -6639,15 +6639,15 @@
     } = n;
     return t == null && (t = n.inclusive), i == null && (i = n.inclusive), {
         start: t != null ? t : e,
         end: i != null ? i : e
     }
 }
 
-function _0(n, e) {
+function H0(n, e) {
     return n == e || !!(n && e && n.compare(e))
 }
 
 function Xa(n, e, t, i = 0) {
     let r = t.length - 1;
     r >= 0 && t[r] + i >= n ? t[r] = Math.max(t[r], e) : t.push(n, e)
 }
@@ -6701,16 +6701,16 @@
         let l = t - e;
         if (i instanceof vn)
             if (i.block) i.startSide > 0 && !this.posCovered() && this.getLine(), this.addBlockWidget(new mn(i.widget || new ef("div"), l, i));
             else {
                 let h = dn.create(i.widget || new ef("span"), l, l ? 0 : i.startSide),
                     f = this.atCursorPos && !h.isEditable && s <= r.length && (e < t || i.startSide > 0),
                     u = !h.isEditable && (e < t || s > r.length || i.startSide <= 0),
-                    g = this.getLine();
-                this.pendingBuffer == 2 && !f && !h.isEditable && (this.pendingBuffer = 0), this.flushBuffer(r), f && (g.append(to(new vr(1), r), s), s = r.length + Math.max(0, s - r.length)), g.append(to(h, r), s), this.atCursorPos = u, this.pendingBuffer = u ? e < t || s > r.length ? 1 : 2 : 0, this.pendingBuffer && (this.bufferMarks = r.slice())
+                    m = this.getLine();
+                this.pendingBuffer == 2 && !f && !h.isEditable && (this.pendingBuffer = 0), this.flushBuffer(r), f && (m.append(to(new vr(1), r), s), s = r.length + Math.max(0, s - r.length)), m.append(to(h, r), s), this.atCursorPos = u, this.pendingBuffer = u ? e < t || s > r.length ? 1 : 2 : 0, this.pendingBuffer && (this.bufferMarks = r.slice())
             }
         else this.doc.lineAt(this.pos).from == this.pos && this.getLine().addLineDeco(i);
         l && (this.textOff + l <= this.text.length ? this.textOff += l : (this.skip += l - (this.text.length - this.textOff), this.text = "", this.textOff = 0), this.pos = t), this.openStart < 0 && (this.openStart = s)
     }
     static build(e, t, i, r, s) {
         let o = new os(e, t, i, s);
         return o.openEnd = Pe.spans(r, t, i, o), o.openStart < 0 && (o.openStart = o.openEnd), o.finish(o.openEnd), o
@@ -6769,28 +6769,28 @@
 function ni(n, e, t) {
     let i = n.facet(Md);
     i.length ? i[0](e) : window.onerror ? window.onerror(String(e), t, void 0, void 0, e) : t ? console.error(t + ":", e) : console.error(e)
 }
 const bl = Z.define({
     combine: n => n.length ? n[0] : !0
 });
-let H0 = 0;
+let F0 = 0;
 const Zr = Z.define();
 class rt {
     constructor(e, t, i, r, s) {
         this.id = e, this.create = t, this.domEventHandlers = i, this.domEventObservers = r, this.extension = s(this)
     }
     static define(e, t) {
         const {
             eventHandlers: i,
             eventObservers: r,
             provide: s,
             decorations: o
         } = t || {};
-        return new rt(H0++, e, i, r, l => {
+        return new rt(F0++, e, i, r, l => {
             let h = [Zr.of(l)];
             return o && h.push(gs.of(f => {
                 let u = f.plugin(l);
                 return u ? o(u) : de.none
             })), s && h.push(s(l)), h
         })
     }
@@ -6845,16 +6845,16 @@
     if (!i.length) return i;
     let r = i.map(o => o instanceof Function ? o(n) : o),
         s = [];
     return Pe.spans(r, e, t, {
         point() {},
         span(o, l, h, f) {
             let u = s;
-            for (let g = h.length - 1; g >= 0; g--, f--) {
-                let y = h[g].spec.bidiIsolate,
+            for (let m = h.length - 1; m >= 0; m--, f--) {
+                let y = h[m].spec.bidiIsolate,
                     k;
                 if (y != null)
                     if (f > 0 && u.length && (k = u[u.length - 1]).to == o && k.direction == y) k.to = l, u = k.inner;
                     else {
                         let v = {
                             from: o,
                             to: l,
@@ -6909,17 +6909,17 @@
         if (t.length == 0) return e;
         let i = [];
         for (let r = 0, s = 0, o = 0, l = 0;; r++) {
             let h = r == e.length ? null : e[r],
                 f = o - l,
                 u = h ? h.fromB : 1e9;
             for (; s < t.length && t[s] < u;) {
-                let g = t[s],
+                let m = t[s],
                     y = t[s + 1],
-                    k = Math.max(l, g),
+                    k = Math.max(l, m),
                     v = Math.min(u, y);
                 if (k <= v && new ri(k + f, v + f, k, v).addToSet(i), y > u) break;
                 s += 2
             }
             if (!h) return i;
             new ri(h.fromA, h.toA, h.fromB, h.toB).addToSet(i), o = h.toA, l = h.toB
         }
@@ -6964,28 +6964,28 @@
     _d = Ue.RTL;
 
 function Hd(n) {
     let e = [];
     for (let t = 0; t < n.length; t++) e.push(1 << +n[t]);
     return e
 }
-const F0 = Hd("88888888888888888888888888888888888666888888787833333333337888888000000000000000000000000008888880000000000000000000000000088888888888888888888888888888888888887866668888088888663380888308888800000000000000000000000800000000000000000000000000000008"),
-    z0 = Hd("4444448826627288999999999992222222222222222222222222222222222222222222222229999999999999999999994444444444644222822222222222222222222222222222222222222222222222222222222222222222222222222222222222222222222222222222999999949999999229989999223333333333"),
+const z0 = Hd("88888888888888888888888888888888888666888888787833333333337888888000000000000000000000000008888880000000000000000000000000088888888888888888888888888888888888887866668888088888663380888308888800000000000000000000000800000000000000000000000000000008"),
+    $0 = Hd("4444448826627288999999999992222222222222222222222222222222222222222222222229999999999999999999994444444444644222822222222222222222222222222222222222222222222222222222222222222222222222222222222222222222222222222222999999949999999229989999223333333333"),
     Ja = Object.create(null),
     Ti = [];
 for (let n of ["()", "[]", "{}"]) {
     let e = n.charCodeAt(0),
         t = n.charCodeAt(1);
     Ja[e] = t, Ja[t] = -e
 }
 
-function $0(n) {
-    return n <= 247 ? F0[n] : 1424 <= n && n <= 1524 ? 2 : 1536 <= n && n <= 1785 ? z0[n - 1536] : 1774 <= n && n <= 2220 ? 4 : 8192 <= n && n <= 8204 ? 256 : 64336 <= n && n <= 65023 ? 4 : 1
+function W0(n) {
+    return n <= 247 ? z0[n] : 1424 <= n && n <= 1524 ? 2 : 1536 <= n && n <= 1785 ? $0[n - 1536] : 1774 <= n && n <= 2220 ? 4 : 8192 <= n && n <= 8204 ? 256 : 64336 <= n && n <= 65023 ? 4 : 1
 }
-const W0 = /[\u0590-\u05f4\u0600-\u06ff\u0700-\u08ac\ufb50-\ufdff]/;
+const q0 = /[\u0590-\u05f4\u0600-\u06ff\u0700-\u08ac\ufb50-\ufdff]/;
 class pn {
     get dir() {
         return this.level % 2 ? _d : ms
     }
     constructor(e, t, i) {
         this.from = e, this.to = t, this.level = i
     }
@@ -7013,193 +7013,193 @@
             r = e[t];
         if (i.from != r.from || i.to != r.to || i.direction != r.direction || !Fd(i.inner, r.inner)) return !1
     }
     return !0
 }
 const He = [];
 
-function q0(n, e, t, i, r) {
+function j0(n, e, t, i, r) {
     for (let s = 0; s <= i.length; s++) {
         let o = s ? i[s - 1].to : e,
             l = s < i.length ? i[s].from : t,
             h = s ? 256 : r;
-        for (let f = o, u = h, g = h; f < l; f++) {
-            let y = $0(n.charCodeAt(f));
-            y == 512 ? y = u : y == 8 && g == 4 && (y = 16), He[f] = y == 4 ? 2 : y, y & 7 && (g = y), u = y
+        for (let f = o, u = h, m = h; f < l; f++) {
+            let y = W0(n.charCodeAt(f));
+            y == 512 ? y = u : y == 8 && m == 4 && (y = 16), He[f] = y == 4 ? 2 : y, y & 7 && (m = y), u = y
         }
-        for (let f = o, u = h, g = h; f < l; f++) {
+        for (let f = o, u = h, m = h; f < l; f++) {
             let y = He[f];
             if (y == 128) f < l - 1 && u == He[f + 1] && u & 24 ? y = He[f] = u : He[f] = 256;
             else if (y == 64) {
                 let k = f + 1;
                 for (; k < l && He[k] == 64;) k++;
-                let v = f && u == 8 || k < t && He[k] == 8 ? g == 1 ? 1 : 8 : 256;
-                for (let C = f; C < k; C++) He[C] = v;
+                let v = f && u == 8 || k < t && He[k] == 8 ? m == 1 ? 1 : 8 : 256;
+                for (let A = f; A < k; A++) He[A] = v;
                 f = k - 1
-            } else y == 8 && g == 1 && (He[f] = 1);
-            u = y, y & 7 && (g = y)
+            } else y == 8 && m == 1 && (He[f] = 1);
+            u = y, y & 7 && (m = y)
         }
     }
 }
 
-function j0(n, e, t, i, r) {
+function V0(n, e, t, i, r) {
     let s = r == 1 ? 2 : 1;
     for (let o = 0, l = 0, h = 0; o <= i.length; o++) {
         let f = o ? i[o - 1].to : e,
             u = o < i.length ? i[o].from : t;
-        for (let g = f, y, k, v; g < u; g++)
-            if (k = Ja[y = n.charCodeAt(g)])
+        for (let m = f, y, k, v; m < u; m++)
+            if (k = Ja[y = n.charCodeAt(m)])
                 if (k < 0) {
-                    for (let C = l - 3; C >= 0; C -= 3)
-                        if (Ti[C + 1] == -k) {
-                            let O = Ti[C + 2],
+                    for (let A = l - 3; A >= 0; A -= 3)
+                        if (Ti[A + 1] == -k) {
+                            let O = Ti[A + 2],
                                 D = O & 2 ? r : O & 4 ? O & 1 ? s : r : 0;
-                            D && (He[g] = He[Ti[C]] = D), l = C;
+                            D && (He[m] = He[Ti[A]] = D), l = A;
                             break
                         }
                 } else {
                     if (Ti.length == 189) break;
-                    Ti[l++] = g, Ti[l++] = y, Ti[l++] = h
+                    Ti[l++] = m, Ti[l++] = y, Ti[l++] = h
                 }
-        else if ((v = He[g]) == 2 || v == 1) {
-            let C = v == r;
-            h = C ? 0 : 1;
+        else if ((v = He[m]) == 2 || v == 1) {
+            let A = v == r;
+            h = A ? 0 : 1;
             for (let O = l - 3; O >= 0; O -= 3) {
                 let D = Ti[O + 2];
                 if (D & 2) break;
-                if (C) Ti[O + 2] |= 2;
+                if (A) Ti[O + 2] |= 2;
                 else {
                     if (D & 4) break;
                     Ti[O + 2] |= 4
                 }
             }
         }
     }
 }
 
-function V0(n, e, t, i) {
+function U0(n, e, t, i) {
     for (let r = 0, s = i; r <= t.length; r++) {
         let o = r ? t[r - 1].to : n,
             l = r < t.length ? t[r].from : e;
         for (let h = o; h < l;) {
             let f = He[h];
             if (f == 256) {
                 let u = h + 1;
                 for (;;)
                     if (u == l) {
                         if (r == t.length) break;
                         u = t[r++].to, l = r < t.length ? t[r].from : e
                     } else if (He[u] == 256) u++;
                 else break;
-                let g = s == 1,
+                let m = s == 1,
                     y = (u < e ? He[u] : i) == 1,
-                    k = g == y ? g ? 1 : 2 : i;
-                for (let v = u, C = r, O = C ? t[C - 1].to : n; v > h;) v == O && (v = t[--C].from, O = C ? t[C - 1].to : n), He[--v] = k;
+                    k = m == y ? m ? 1 : 2 : i;
+                for (let v = u, A = r, O = A ? t[A - 1].to : n; v > h;) v == O && (v = t[--A].from, O = A ? t[A - 1].to : n), He[--v] = k;
                 h = u
             } else s = f, h++
         }
     }
 }
 
 function Za(n, e, t, i, r, s, o) {
     let l = i % 2 ? 2 : 1;
     if (i % 2 == r % 2)
         for (let h = e, f = 0; h < t;) {
             let u = !0,
-                g = !1;
+                m = !1;
             if (f == s.length || h < s[f].from) {
-                let C = He[h];
-                C != l && (u = !1, g = C == 16)
+                let A = He[h];
+                A != l && (u = !1, m = A == 16)
             }
             let y = !u && l == 1 ? [] : null,
                 k = u ? i : i + 1,
                 v = h;
             e: for (;;)
                 if (f < s.length && v == s[f].from) {
-                    if (g) break e;
-                    let C = s[f];
+                    if (m) break e;
+                    let A = s[f];
                     if (!u)
-                        for (let O = C.to, D = f + 1;;) {
+                        for (let O = A.to, D = f + 1;;) {
                             if (O == t) break e;
                             if (D < s.length && s[D].from == O) O = s[D++].to;
                             else {
                                 if (He[O] == l) break e;
                                 break
                             }
                         }
-                    if (f++, y) y.push(C);
+                    if (f++, y) y.push(A);
                     else {
-                        C.from > h && o.push(new pn(h, C.from, k));
-                        let O = C.direction == ms != !(k % 2);
-                        eh(n, O ? i + 1 : i, r, C.inner, C.from, C.to, o), h = C.to
+                        A.from > h && o.push(new pn(h, A.from, k));
+                        let O = A.direction == ms != !(k % 2);
+                        eh(n, O ? i + 1 : i, r, A.inner, A.from, A.to, o), h = A.to
                     }
-                    v = C.to
+                    v = A.to
                 } else {
                     if (v == t || (u ? He[v] != l : He[v] == l)) break;
                     v++
                 } y ? Za(n, h, v, i + 1, r, y, o) : h < v && o.push(new pn(h, v, k)), h = v
         } else
             for (let h = t, f = s.length; h > e;) {
                 let u = !0,
-                    g = !1;
+                    m = !1;
                 if (!f || h > s[f - 1].to) {
-                    let C = He[h - 1];
-                    C != l && (u = !1, g = C == 16)
+                    let A = He[h - 1];
+                    A != l && (u = !1, m = A == 16)
                 }
                 let y = !u && l == 1 ? [] : null,
                     k = u ? i : i + 1,
                     v = h;
                 e: for (;;)
                     if (f && v == s[f - 1].to) {
-                        if (g) break e;
-                        let C = s[--f];
+                        if (m) break e;
+                        let A = s[--f];
                         if (!u)
-                            for (let O = C.from, D = f;;) {
+                            for (let O = A.from, D = f;;) {
                                 if (O == e) break e;
                                 if (D && s[D - 1].to == O) O = s[--D].from;
                                 else {
                                     if (He[O - 1] == l) break e;
                                     break
                                 }
                             }
-                        if (y) y.push(C);
+                        if (y) y.push(A);
                         else {
-                            C.to < h && o.push(new pn(C.to, h, k));
-                            let O = C.direction == ms != !(k % 2);
-                            eh(n, O ? i + 1 : i, r, C.inner, C.from, C.to, o), h = C.from
+                            A.to < h && o.push(new pn(A.to, h, k));
+                            let O = A.direction == ms != !(k % 2);
+                            eh(n, O ? i + 1 : i, r, A.inner, A.from, A.to, o), h = A.from
                         }
-                        v = C.from
+                        v = A.from
                     } else {
                         if (v == e || (u ? He[v - 1] != l : He[v - 1] == l)) break;
                         v--
                     } y ? Za(n, v, h, i + 1, r, y, o) : v < h && o.push(new pn(v, h, k)), h = v
             }
 }
 
 function eh(n, e, t, i, r, s, o) {
     let l = e % 2 ? 2 : 1;
-    q0(n, r, s, i, l), j0(n, r, s, i, l), V0(r, s, i, l), Za(n, r, s, e, t, i, o)
+    j0(n, r, s, i, l), V0(n, r, s, i, l), U0(r, s, i, l), Za(n, r, s, e, t, i, o)
 }
 
-function U0(n, e, t) {
+function Q0(n, e, t) {
     if (!n) return [new pn(0, 0, e == _d ? 1 : 0)];
-    if (e == ms && !t.length && !W0.test(n)) return zd(n.length);
+    if (e == ms && !t.length && !q0.test(n)) return zd(n.length);
     if (t.length)
         for (; n.length > He.length;) He[He.length] = 256;
     let i = [],
         r = e == ms ? 0 : 1;
     return eh(n, r, r, t, 0, n.length, i), i
 }
 
 function zd(n) {
     return [new pn(0, n, 0)]
 }
 let $d = "";
 
-function Q0(n, e, t, i, r) {
+function G0(n, e, t, i, r) {
     var s;
     let o = i.head - n.from,
         l = -1;
     if (o == 0) {
         if (!r || !n.length) return null;
         e[0].level != t && (o = e[0].side(!1, t), l = 0)
     } else if (o == n.length) {
@@ -7209,16 +7209,16 @@
     }
     l < 0 && (l = pn.find(e, o, (s = i.bidiLevel) !== null && s !== void 0 ? s : -1, i.assoc));
     let h = e[l];
     o == h.side(r, t) && (h = e[l += r ? 1 : -1], o = h.side(!r, t));
     let f = r == (h.dir == t),
         u = mt(n.text, o, f);
     if ($d = n.text.slice(Math.min(o, u), Math.max(o, u)), u > h.from && u < h.to) return H.cursor(u + n.from, f ? -1 : 1, h.level);
-    let g = l == (r ? e.length - 1 : 0) ? null : e[l + (r ? 1 : -1)];
-    return !g && h.level != t ? H.cursor(r ? n.to : n.from, r ? -1 : 1, t) : g && g.level < h.level ? H.cursor(g.side(!r, t) + n.from, r ? 1 : -1, g.level) : H.cursor(u + n.from, r ? -1 : 1, h.level)
+    let m = l == (r ? e.length - 1 : 0) ? null : e[l + (r ? 1 : -1)];
+    return !m && h.level != t ? H.cursor(r ? n.to : n.from, r ? -1 : 1, t) : m && m.level < h.level ? H.cursor(m.side(!r, t) + n.from, r ? 1 : -1, m.level) : H.cursor(u + n.from, r ? -1 : 1, h.level)
 }
 class nf extends je {
     get length() {
         return this.view.state.doc.length
     }
     constructor(e) {
         super(), this.view = e, this.decorations = [], this.dynamicDecorationMap = [], this.domChanged = null, this.hasComposition = null, this.markedForComposition = new Set, this.minWidth = 0, this.minWidthFrom = 0, this.minWidthTo = 0, this.impreciseAnchor = null, this.impreciseHead = null, this.forceSelection = !1, this.lastUpdate = Date.now(), this.setDOM(e.contentDOM), this.children = [new tt], this.children[0].setParent(this), this.updateDeco(), this.updateInner([new ri(0, 0, 0, e.state.doc.length)], 0, null)
@@ -7227,31 +7227,31 @@
         var t;
         let i = e.changedRanges;
         this.minWidth > 0 && i.length && (i.every(({
             fromA: f,
             toA: u
         }) => u < this.minWidthFrom || f > this.minWidthTo) ? (this.minWidthFrom = e.changes.mapPos(this.minWidthFrom, 1), this.minWidthTo = e.changes.mapPos(this.minWidthTo, 1)) : this.minWidth = this.minWidthFrom = this.minWidthTo = 0);
         let r = -1;
-        this.view.inputState.composing >= 0 && (!((t = this.domChanged) === null || t === void 0) && t.newSel ? r = this.domChanged.newSel.head : !ey(e.changes, this.hasComposition) && !e.selectionSet && (r = e.state.selection.main.head));
-        let s = r > -1 ? K0(this.view, e.changes, r) : null;
+        this.view.inputState.composing >= 0 && (!((t = this.domChanged) === null || t === void 0) && t.newSel ? r = this.domChanged.newSel.head : !ty(e.changes, this.hasComposition) && !e.selectionSet && (r = e.state.selection.main.head));
+        let s = r > -1 ? X0(this.view, e.changes, r) : null;
         if (this.domChanged = null, this.hasComposition) {
             this.markedForComposition.clear();
             let {
                 from: f,
                 to: u
             } = this.hasComposition;
             i = new ri(f, u, e.changes.mapPos(f, -1), e.changes.mapPos(u, 1)).addToSet(i.slice())
         }
         this.hasComposition = s ? {
             from: s.range.fromB,
             to: s.range.toB
         } : null, (ee.ie || ee.chrome) && !s && e && e.state.doc.lines != e.startState.doc.lines && (this.forceSelection = !0);
         let o = this.decorations,
             l = this.updateDeco(),
-            h = J0(o, l, e.changes);
+            h = Z0(o, l, e.changes);
         return i = ri.extendWithRanges(i, h), !(this.flags & 7) && i.length == 0 ? !1 : (this.updateInner(i, e.startState.doc.length, s), e.transactions.length && (this.lastUpdate = Date.now()), !0)
     }
     updateInner(e, t, i) {
         this.view.viewState.mustMeasureContent = !0, this.updateChildren(e, t, i);
         let {
             observer: r
         } = this.view;
@@ -7274,36 +7274,36 @@
         for (let o = r.length - 1;; o--) {
             let l = o >= 0 ? r[o] : null;
             if (!l) break;
             let {
                 fromA: h,
                 toA: f,
                 fromB: u,
-                toB: g
-            } = l, y, k, v, C;
-            if (i && i.range.fromB < g && i.range.toB > u) {
+                toB: m
+            } = l, y, k, v, A;
+            if (i && i.range.fromB < m && i.range.toB > u) {
                 let j = os.build(this.view.state.doc, u, i.range.fromB, this.decorations, this.dynamicDecorationMap),
-                    z = os.build(this.view.state.doc, i.range.toB, g, this.decorations, this.dynamicDecorationMap);
-                k = j.breakAtStart, v = j.openStart, C = z.openEnd;
+                    z = os.build(this.view.state.doc, i.range.toB, m, this.decorations, this.dynamicDecorationMap);
+                k = j.breakAtStart, v = j.openStart, A = z.openEnd;
                 let G = this.compositionView(i);
                 z.breakAtStart ? G.breakAfter = 1 : z.content.length && G.merge(G.length, G.length, z.content[0], !1, z.openStart, 0) && (G.breakAfter = z.content[0].breakAfter, z.content.shift()), j.content.length && G.merge(0, 0, j.content[j.content.length - 1], !0, 0, j.openEnd) && j.content.pop(), y = j.content.concat(G).concat(z.content)
             } else({
                 content: y,
                 breakAtStart: k,
                 openStart: v,
-                openEnd: C
-            } = os.build(this.view.state.doc, u, g, this.decorations, this.dynamicDecorationMap));
+                openEnd: A
+            } = os.build(this.view.state.doc, u, m, this.decorations, this.dynamicDecorationMap));
             let {
                 i: O,
                 off: D
             } = s.findPos(f, 1), {
                 i: F,
                 off: $
             } = s.findPos(h, -1);
-            yd(this, F, $, O, D, y, k, v, C)
+            yd(this, F, $, O, D, y, k, v, A)
         }
         i && this.fixCompositionDOM(i)
     }
     compositionView(e) {
         let t = new Qi(e.text.nodeValue);
         t.flags |= 8;
         for (let {
@@ -7331,42 +7331,42 @@
             s = !r && Do(this.dom, this.view.observer.selectionRange) && !(i && this.dom.contains(i));
         if (!(r || t || s)) return;
         let o = this.forceSelection;
         this.forceSelection = !1;
         let l = this.view.state.selection.main,
             h = this.moveToLine(this.domAtPos(l.anchor)),
             f = l.empty ? h : this.moveToLine(this.domAtPos(l.head));
-        if (ee.gecko && l.empty && !this.hasComposition && G0(h)) {
-            let g = document.createTextNode("");
-            this.view.observer.ignore(() => h.node.insertBefore(g, h.node.childNodes[h.offset] || null)), h = f = new St(g, 0), o = !0
+        if (ee.gecko && l.empty && !this.hasComposition && K0(h)) {
+            let m = document.createTextNode("");
+            this.view.observer.ignore(() => h.node.insertBefore(m, h.node.childNodes[h.offset] || null)), h = f = new St(m, 0), o = !0
         }
         let u = this.view.observer.selectionRange;
         (o || !u.focusNode || !Wo(h.node, h.offset, u.anchorNode, u.anchorOffset) || !Wo(f.node, f.offset, u.focusNode, u.focusOffset)) && (this.view.observer.ignore(() => {
-            ee.android && ee.chrome && this.dom.contains(u.focusNode) && Z0(u.focusNode, this.dom) && (this.dom.blur(), this.dom.focus({
+            ee.android && ee.chrome && this.dom.contains(u.focusNode) && ey(u.focusNode, this.dom) && (this.dom.blur(), this.dom.focus({
                 preventScroll: !0
             }));
-            let g = $o(this.view.root);
-            if (g)
+            let m = $o(this.view.root);
+            if (m)
                 if (l.empty) {
                     if (ee.gecko) {
-                        let y = X0(h.node, h.offset);
+                        let y = Y0(h.node, h.offset);
                         if (y && y != 3) {
                             let k = qd(h.node, h.offset, y == 1 ? 1 : -1);
                             k && (h = new St(k.node, k.offset))
                         }
                     }
-                    g.collapse(h.node, h.offset), l.bidiLevel != null && g.caretBidiLevel !== void 0 && (g.caretBidiLevel = l.bidiLevel)
-                } else if (g.extend) {
-                g.collapse(h.node, h.offset);
+                    m.collapse(h.node, h.offset), l.bidiLevel != null && m.caretBidiLevel !== void 0 && (m.caretBidiLevel = l.bidiLevel)
+                } else if (m.extend) {
+                m.collapse(h.node, h.offset);
                 try {
-                    g.extend(f.node, f.offset)
+                    m.extend(f.node, f.offset)
                 } catch (y) {}
             } else {
                 let y = document.createRange();
-                l.anchor > l.head && ([h, f] = [f, h]), y.setEnd(f.node, f.offset), y.setStart(h.node, h.offset), g.removeAllRanges(), g.addRange(y)
+                l.anchor > l.head && ([h, f] = [f, h]), y.setEnd(f.node, f.offset), y.setStart(h.node, h.offset), m.removeAllRanges(), m.addRange(y)
             }
             s && this.view.root.activeElement == this.dom && (this.dom.blur(), i && i.focus())
         }), this.view.observer.setSelectionRange(h, f)), this.impreciseAnchor = h.precise ? null : new St(u.anchorNode, u.anchorOffset), this.impreciseHead = f.precise ? null : new St(u.focusNode, u.focusOffset)
     }
     enforceCursorAssoc() {
         if (this.hasComposition) return;
         let {
@@ -7381,16 +7381,16 @@
         let l = o.posAtStart;
         if (t.head == l || t.head == l + o.length) return;
         let h = this.coordsAt(t.head, -1),
             f = this.coordsAt(t.head, 1);
         if (!h || !f || h.bottom > f.top) return;
         let u = this.domAtPos(t.head + t.assoc);
         i.collapse(u.node, u.offset), i.modify("move", t.assoc < 0 ? "forward" : "backward", "lineboundary"), e.observer.readSelectionRange();
-        let g = e.observer.selectionRange;
-        e.docView.posFromDOM(g.anchorNode, g.anchorOffset) != t.from && i.collapse(r, s)
+        let m = e.observer.selectionRange;
+        e.docView.posFromDOM(m.anchorNode, m.anchorOffset) != t.from && i.collapse(r, s)
     }
     moveToLine(e) {
         let t = this.dom,
             i;
         if (e.node != t) return e;
         for (let r = e.offset; !i && r < t.childNodes.length; r++) {
             let s = je.get(t.childNodes[r]);
@@ -7473,30 +7473,30 @@
                 to: r
             } = e,
             s = this.view.contentDOM.clientWidth,
             o = s > Math.max(this.view.scrollDOM.clientWidth, this.minWidth) + 1,
             l = -1,
             h = this.view.textDirection == Ue.LTR;
         for (let f = 0, u = 0; u < this.children.length; u++) {
-            let g = this.children[u],
-                y = f + g.length;
+            let m = this.children[u],
+                y = f + m.length;
             if (y > r) break;
             if (f >= i) {
-                let k = g.dom.getBoundingClientRect();
+                let k = m.dom.getBoundingClientRect();
                 if (t.push(k.height), o) {
-                    let v = g.dom.lastChild,
-                        C = v ? ds(v) : [];
-                    if (C.length) {
-                        let O = C[C.length - 1],
+                    let v = m.dom.lastChild,
+                        A = v ? ds(v) : [];
+                    if (A.length) {
+                        let O = A[A.length - 1],
                             D = h ? O.right - k.left : k.right - O.left;
                         D > l && (l = D, this.minWidth = s, this.minWidthFrom = f, this.minWidthTo = y)
                     }
                 }
             }
-            f = y + g.breakAfter
+            f = y + m.breakAfter
         }
         return t
     }
     textDirectionAt(e) {
         let {
             i: t
         } = this.childPos(e, 1);
@@ -7571,19 +7571,19 @@
                 right: i.right + s.right,
                 bottom: i.bottom + s.bottom
             },
             {
                 offsetWidth: l,
                 offsetHeight: h
             } = this.view.scrollDOM;
-        M0(this.view.scrollDOM, o, t.head < t.anchor ? -1 : 1, e.x, e.y, Math.max(Math.min(e.xMargin, l), -l), Math.max(Math.min(e.yMargin, h), -h), this.view.textDirection == Ue.LTR)
+        E0(this.view.scrollDOM, o, t.head < t.anchor ? -1 : 1, e.x, e.y, Math.max(Math.min(e.xMargin, l), -l), Math.max(Math.min(e.yMargin, h), -h), this.view.textDirection == Ue.LTR)
     }
 }
 
-function G0(n) {
+function K0(n) {
     return n.node.nodeType == 1 && n.node.firstChild && (n.offset == 0 || n.node.childNodes[n.offset - 1].contentEditable == "false") && (n.offset == n.node.childNodes.length || n.node.childNodes[n.offset].contentEditable == "false")
 }
 class rf extends An {
     constructor(e) {
         super(), this.height = e
     }
     toDOM() {
@@ -7609,45 +7609,45 @@
     return {
         from: r,
         to: r + i.node.nodeValue.length,
         node: i.node
     }
 }
 
-function K0(n, e, t) {
+function X0(n, e, t) {
     let i = Wd(n, t);
     if (!i) return null;
     let {
         node: r,
         from: s,
         to: o
     } = i, l = r.nodeValue;
     if (/[\n\r]/.test(l) || n.state.doc.sliceString(i.from, i.to) != l) return null;
     let h = e.invertedDesc,
         f = new ri(h.mapPos(s), h.mapPos(o), s, o),
         u = [];
-    for (let g = r.parentNode;; g = g.parentNode) {
-        let y = je.get(g);
+    for (let m = r.parentNode;; m = m.parentNode) {
+        let y = je.get(m);
         if (y instanceof Gi) u.push({
-            node: g,
+            node: m,
             deco: y.mark
         });
         else {
-            if (y instanceof tt || g.nodeName == "DIV" && g.parentNode == n.contentDOM) return {
+            if (y instanceof tt || m.nodeName == "DIV" && m.parentNode == n.contentDOM) return {
                 range: f,
                 text: r,
                 marks: u,
-                line: g
+                line: m
             };
-            if (g != n.contentDOM) u.push({
-                node: g,
+            if (m != n.contentDOM) u.push({
+                node: m,
                 deco: new Ms({
                     inclusive: !0,
-                    attributes: B0(g),
-                    tagName: g.tagName.toLowerCase()
+                    attributes: _0(m),
+                    tagName: m.tagName.toLowerCase()
                 })
             });
             else return null
         }
     }
 }
 
@@ -7669,48 +7669,48 @@
             };
             if (i.nodeType == 1 && r < i.childNodes.length && t >= 0) i = i.childNodes[r], r = 0;
             else break
         }
     return null
 }
 
-function X0(n, e) {
+function Y0(n, e) {
     return n.nodeType != 1 ? 0 : (e && n.childNodes[e - 1].contentEditable == "false" ? 1 : 0) | (e < n.childNodes.length && n.childNodes[e].contentEditable == "false" ? 2 : 0)
 }
-let Y0 = class {
+let J0 = class {
     constructor() {
         this.changes = []
     }
     compareRange(e, t) {
         Xa(e, t, this.changes)
     }
     comparePoint(e, t) {
         Xa(e, t, this.changes)
     }
 };
 
-function J0(n, e, t) {
-    let i = new Y0;
+function Z0(n, e, t) {
+    let i = new J0;
     return Pe.compare(n, e, t, i), i.changes
 }
 
-function Z0(n, e) {
+function ey(n, e) {
     for (let t = n; t && t != e; t = t.assignedSlot || t.parentNode)
         if (t.nodeType == 1 && t.contentEditable == "false") return !0;
     return !1
 }
 
-function ey(n, e) {
+function ty(n, e) {
     let t = !1;
     return e && n.iterChangedRanges((i, r) => {
         i < e.to && r > e.from && (t = !0)
     }), t
 }
 
-function ty(n, e, t = 1) {
+function iy(n, e, t = 1) {
     let i = n.charCategorizer(e),
         r = n.doc.lineAt(e),
         s = e - r.from;
     if (r.length == 0) return H.cursor(e);
     s == 0 ? t = 1 : s == r.length && (t = -1);
     let o = s,
         l = s;
@@ -7725,19 +7725,19 @@
         let f = mt(r.text, l);
         if (i(r.text.slice(l, f)) != h) break;
         l = f
     }
     return H.range(o + r.from, l + r.from)
 }
 
-function iy(n, e) {
+function ny(n, e) {
     return e.left > n ? e.left - n : Math.max(0, n - e.right)
 }
 
-function ny(n, e) {
+function ry(n, e) {
     return e.top > n ? e.top - n : Math.max(0, n - e.bottom)
 }
 
 function na(n, e) {
     return n.top < e.bottom - 1 && n.bottom > e.top + 1
 }
 
@@ -7757,32 +7757,32 @@
         right: n.right,
         bottom: e
     } : n
 }
 
 function th(n, e, t) {
     let i, r, s, o, l = !1,
-        h, f, u, g;
+        h, f, u, m;
     for (let v = n.firstChild; v; v = v.nextSibling) {
-        let C = ds(v);
-        for (let O = 0; O < C.length; O++) {
-            let D = C[O];
+        let A = ds(v);
+        for (let O = 0; O < A.length; O++) {
+            let D = A[O];
             r && na(r, D) && (D = sf(of(D, r.bottom), r.top));
-            let F = iy(e, D),
-                $ = ny(t, D);
+            let F = ny(e, D),
+                $ = ry(t, D);
             if (F == 0 && $ == 0) return v.nodeType == 3 ? lf(v, e, t) : th(v, e, t);
             if (!i || o > $ || o == $ && s > F) {
                 i = v, r = D, s = F, o = $;
                 let j = $ ? t < D.top ? -1 : 1 : F ? e < D.left ? -1 : 1 : 0;
-                l = !j || (j > 0 ? O < C.length - 1 : O > 0)
+                l = !j || (j > 0 ? O < A.length - 1 : O > 0)
             }
-            F == 0 ? t > D.bottom && (!u || u.bottom < D.bottom) ? (h = v, u = D) : t < D.top && (!g || g.top > D.top) && (f = v, g = D) : u && na(u, D) ? u = of(u, D.bottom) : g && na(g, D) && (g = sf(g, D.top))
+            F == 0 ? t > D.bottom && (!u || u.bottom < D.bottom) ? (h = v, u = D) : t < D.top && (!m || m.top > D.top) && (f = v, m = D) : u && na(u, D) ? u = of(u, D.bottom) : m && na(m, D) && (m = sf(m, D.top))
         }
     }
-    if (u && u.bottom >= t ? (i = h, r = u) : g && g.top <= t && (i = f, r = g), !i) return {
+    if (u && u.bottom >= t ? (i = h, r = u) : m && m.top <= t && (i = f, r = m), !i) return {
         node: n,
         offset: 0
     };
     let y = Math.max(r.left, Math.min(r.right, e));
     if (i.nodeType == 3) return lf(i, y, t);
     if (l && i.contentEditable != "false") return th(i, y, t);
     let k = Array.prototype.indexOf.call(n.childNodes, i) + (e >= (r.left + r.right) / 2 ? 1 : 0);
@@ -7799,23 +7799,23 @@
         o = 0;
     for (let l = 0; l < i; l++) {
         let h = Un(n, l, l + 1).getClientRects();
         for (let f = 0; f < h.length; f++) {
             let u = h[f];
             if (u.top == u.bottom) continue;
             o || (o = e - u.left);
-            let g = (u.top > t ? u.top - t : t - u.bottom) - 1;
-            if (u.left - 1 <= e && u.right + 1 >= e && g < s) {
+            let m = (u.top > t ? u.top - t : t - u.bottom) - 1;
+            if (u.left - 1 <= e && u.right + 1 >= e && m < s) {
                 let y = e >= (u.left + u.right) / 2,
                     k = y;
-                if ((ee.chrome || ee.gecko) && Un(n, l).getBoundingClientRect().left == u.right && (k = !y), g <= 0) return {
+                if ((ee.chrome || ee.gecko) && Un(n, l).getBoundingClientRect().left == u.right && (k = !y), m <= 0) return {
                     node: n,
                     offset: l + (k ? 1 : 0)
                 };
-                r = l + (k ? 1 : 0), s = g
+                r = l + (k ? 1 : 0), s = m
             }
         }
     }
     return {
         node: n,
         offset: r > -1 ? r : o > 0 ? n.nodeValue.length : 0
     }
@@ -7826,55 +7826,55 @@
     let o = n.contentDOM.getBoundingClientRect(),
         l = o.top + n.viewState.paddingTop,
         h, {
             docHeight: f
         } = n.viewState,
         {
             x: u,
-            y: g
+            y: m
         } = e,
-        y = g - l;
+        y = m - l;
     if (y < 0) return 0;
     if (y > f) return n.state.doc.length;
     for (let j = n.viewState.heightOracle.textHeight / 2, z = !1; h = n.elementAtHeight(y), h.type != Dt.Text;)
         for (; y = i > 0 ? h.bottom + j : h.top - j, !(y >= 0 && y <= f);) {
             if (z) return t ? null : 0;
             z = !0, i = -i
         }
-    g = l + y;
+    m = l + y;
     let k = h.from;
-    if (k < n.viewport.from) return n.viewport.from == 0 ? 0 : t ? null : af(n, o, h, u, g);
-    if (k > n.viewport.to) return n.viewport.to == n.state.doc.length ? n.state.doc.length : t ? null : af(n, o, h, u, g);
+    if (k < n.viewport.from) return n.viewport.from == 0 ? 0 : t ? null : af(n, o, h, u, m);
+    if (k > n.viewport.to) return n.viewport.to == n.state.doc.length ? n.state.doc.length : t ? null : af(n, o, h, u, m);
     let v = n.dom.ownerDocument,
-        C = n.root.elementFromPoint ? n.root : v,
-        O = C.elementFromPoint(u, g);
-    O && !n.contentDOM.contains(O) && (O = null), O || (u = Math.max(o.left + 1, Math.min(o.right - 1, u)), O = C.elementFromPoint(u, g), O && !n.contentDOM.contains(O) && (O = null));
+        A = n.root.elementFromPoint ? n.root : v,
+        O = A.elementFromPoint(u, m);
+    O && !n.contentDOM.contains(O) && (O = null), O || (u = Math.max(o.left + 1, Math.min(o.right - 1, u)), O = A.elementFromPoint(u, m), O && !n.contentDOM.contains(O) && (O = null));
     let D, F = -1;
     if (O && ((r = n.docView.nearest(O)) === null || r === void 0 ? void 0 : r.isEditable) != !1) {
         if (v.caretPositionFromPoint) {
-            let j = v.caretPositionFromPoint(u, g);
+            let j = v.caretPositionFromPoint(u, m);
             j && ({
                 offsetNode: D,
                 offset: F
             } = j)
         } else if (v.caretRangeFromPoint) {
-            let j = v.caretRangeFromPoint(u, g);
+            let j = v.caretRangeFromPoint(u, m);
             j && ({
                 startContainer: D,
                 startOffset: F
-            } = j, (!n.contentDOM.contains(D) || ee.safari && ry(D, F, u) || ee.chrome && sy(D, F, u)) && (D = void 0))
+            } = j, (!n.contentDOM.contains(D) || ee.safari && sy(D, F, u) || ee.chrome && oy(D, F, u)) && (D = void 0))
         }
     }
     if (!D || !n.docView.dom.contains(D)) {
         let j = tt.find(n.docView, k);
         if (!j) return y > h.top + h.height / 2 ? h.to : h.from;
         ({
             node: D,
             offset: F
-        } = th(j.dom, u, g))
+        } = th(j.dom, u, m))
     }
     let $ = n.docView.nearest(D);
     if (!$) return null;
     if ($.isWidget && ((s = $.dom) === null || s === void 0 ? void 0 : s.nodeType) == 1) {
         let j = $.dom.getBoundingClientRect();
         return e.y < j.top || e.y <= j.bottom && e.x <= (j.left + j.right) / 2 ? $.posAtStart : $.posAtEnd
     } else return $.localPosFromDOM(D, F) + $.posAtStart
@@ -7884,26 +7884,26 @@
     let s = Math.round((i - e.left) * n.defaultCharacterWidth);
     if (n.lineWrapping && t.height > n.defaultLineHeight * 1.5) {
         let l = n.viewState.heightOracle.textHeight,
             h = Math.floor((r - t.top - (n.defaultLineHeight - l) * .5) / l);
         s += h * n.viewState.heightOracle.lineLength
     }
     let o = n.state.sliceDoc(t.from, t.to);
-    return t.from + w0(o, s, n.state.tabSize)
+    return t.from + v0(o, s, n.state.tabSize)
 }
 
-function ry(n, e, t) {
+function sy(n, e, t) {
     let i;
     if (n.nodeType != 3 || e != (i = n.nodeValue.length)) return !1;
     for (let r = n.nextSibling; r; r = r.nextSibling)
         if (r.nodeType != 1 || r.nodeName != "BR") return !1;
     return Un(n, i - 1, i).getBoundingClientRect().left > t
 }
 
-function sy(n, e, t) {
+function oy(n, e, t) {
     if (e != 0) return !1;
     for (let r = n;;) {
         let s = r.parentNode;
         if (!s || s.nodeType != 1 || s.firstChild != r) return !1;
         if (s.classList.contains("cm-line")) break;
         r = s
     }
@@ -7916,15 +7916,15 @@
     if (Array.isArray(t.type)) {
         for (let i of t.type)
             if (i.to > e || i.to == e && (i.to == t.to || i.type == Dt.Text)) return i
     }
     return t
 }
 
-function oy(n, e, t, i) {
+function ly(n, e, t, i) {
     let r = ih(n, e.head),
         s = !i || r.type != Dt.Text || !(n.lineWrapping || r.widgetLineBreaks) ? null : n.coordsAtPos(e.assoc < 0 && e.head > r.from ? e.head - 1 : e.head);
     if (s) {
         let o = n.dom.getBoundingClientRect(),
             l = n.textDirectionAt(r.from),
             h = n.posAtCoords({
                 x: t == (l == Ue.LTR) ? o.right - 1 : o.left + 1,
@@ -7936,15 +7936,15 @@
 }
 
 function hf(n, e, t, i) {
     let r = n.state.doc.lineAt(e.head),
         s = n.bidiSpans(r),
         o = n.textDirectionAt(r.from);
     for (let l = e, h = null;;) {
-        let f = Q0(r, s, o, l, t),
+        let f = G0(r, s, o, l, t),
             u = $d;
         if (!f) {
             if (r.number == (t ? n.state.doc.lines : 1)) return l;
             u = `
 `, r = n.state.doc.line(r.number + (t ? 1 : -1)), s = n.bidiSpans(r), f = H.cursor(t ? r.from : r.to)
         }
         if (h) {
@@ -7953,48 +7953,48 @@
             if (!i) return f;
             h = i(u)
         }
         l = f
     }
 }
 
-function ly(n, e, t) {
+function ay(n, e, t) {
     let i = n.state.charCategorizer(e),
         r = i(t);
     return s => {
         let o = i(s);
         return r == Ve.Space && (r = o), r == o
     }
 }
 
-function ay(n, e, t, i) {
+function hy(n, e, t, i) {
     let r = e.head,
         s = t ? 1 : -1;
     if (r == (t ? n.state.doc.length : 0)) return H.cursor(r, e.assoc);
     let o = e.goalColumn,
         l, h = n.contentDOM.getBoundingClientRect(),
         f = n.coordsAtPos(r, e.assoc || -1),
         u = n.documentTop;
     if (f) o == null && (o = f.left - h.left), l = s < 0 ? f.top : f.bottom;
     else {
         let k = n.viewState.lineBlockAt(r);
         o == null && (o = Math.min(h.right - h.left, n.defaultCharacterWidth * (r - k.from))), l = (s < 0 ? k.top : k.bottom) + u
     }
-    let g = h.left + o,
+    let m = h.left + o,
         y = i != null ? i : n.viewState.heightOracle.textHeight >> 1;
     for (let k = 0;; k += 10) {
         let v = l + (y + k) * s,
-            C = jd(n, {
-                x: g,
+            A = jd(n, {
+                x: m,
                 y: v
             }, !1, s);
-        if (v < h.top || v > h.bottom || (s < 0 ? C < r : C > r)) {
-            let O = n.docView.coordsForChar(C),
+        if (v < h.top || v > h.bottom || (s < 0 ? A < r : A > r)) {
+            let O = n.docView.coordsForChar(A),
                 D = !O || v < O.top ? -1 : 1;
-            return H.cursor(C, D, void 0, o)
+            return H.cursor(A, D, void 0, o)
         }
     }
 }
 
 function Ro(n, e, t) {
     for (;;) {
         let i = 0;
@@ -8008,23 +8008,23 @@
     }
 }
 
 function ra(n, e, t) {
     let i = Ro(n.state.facet(Fh).map(r => r(n)), t.from, e.head > t.from ? -1 : 1);
     return i == t.from ? t : H.cursor(i, i < t.from ? 1 : -1)
 }
-class hy {
+class cy {
     setSelectionOrigin(e) {
         this.lastSelectionOrigin = e, this.lastSelectionTime = Date.now()
     }
     constructor(e) {
-        this.view = e, this.lastKeyCode = 0, this.lastKeyTime = 0, this.lastTouchTime = 0, this.lastFocusTime = 0, this.lastScrollTop = 0, this.lastScrollLeft = 0, this.pendingIOSKey = void 0, this.lastSelectionOrigin = null, this.lastSelectionTime = 0, this.lastEscPress = 0, this.lastContextMenu = 0, this.scrollHandlers = [], this.handlers = Object.create(null), this.composing = -1, this.compositionFirstChange = null, this.compositionEndedAt = 0, this.compositionPendingKey = !1, this.compositionPendingChange = !1, this.mouseSelection = null, this.draggedContent = null, this.handleEvent = this.handleEvent.bind(this), this.notifiedFocused = e.hasFocus, ee.safari && e.contentDOM.addEventListener("input", () => null), ee.gecko && Ay(e.contentDOM.ownerDocument)
+        this.view = e, this.lastKeyCode = 0, this.lastKeyTime = 0, this.lastTouchTime = 0, this.lastFocusTime = 0, this.lastScrollTop = 0, this.lastScrollLeft = 0, this.pendingIOSKey = void 0, this.lastSelectionOrigin = null, this.lastSelectionTime = 0, this.lastEscPress = 0, this.lastContextMenu = 0, this.scrollHandlers = [], this.handlers = Object.create(null), this.composing = -1, this.compositionFirstChange = null, this.compositionEndedAt = 0, this.compositionPendingKey = !1, this.compositionPendingChange = !1, this.mouseSelection = null, this.draggedContent = null, this.handleEvent = this.handleEvent.bind(this), this.notifiedFocused = e.hasFocus, ee.safari && e.contentDOM.addEventListener("input", () => null), ee.gecko && Ty(e.contentDOM.ownerDocument)
     }
     handleEvent(e) {
-        !yy(this.view, e) || this.ignoreDuringComposition(e) || e.type == "keydown" && this.keydown(e) || this.runHandlers(e.type, e)
+        !by(this.view, e) || this.ignoreDuringComposition(e) || e.type == "keydown" && this.keydown(e) || this.runHandlers(e.type, e)
     }
     runHandlers(e, t) {
         let i = this.handlers[e];
         if (i) {
             for (let r of i.observers) r(this.view, t);
             for (let r of i.handlers) {
                 if (t.defaultPrevented) break;
@@ -8032,15 +8032,15 @@
                     t.preventDefault();
                     break
                 }
             }
         }
     }
     ensureHandlers(e) {
-        let t = cy(e),
+        let t = fy(e),
             i = this.handlers,
             r = this.view.contentDOM;
         for (let s in t)
             if (s != "scroll") {
                 let o = !t[s].handlers.length,
                     l = i[s];
                 l && o != !l.handlers.length && (r.removeEventListener(s, this.handleEvent), l = null), l || r.addEventListener(s, this.handleEvent, {
@@ -8049,15 +8049,15 @@
             } for (let s in i) s != "scroll" && !t[s] && r.removeEventListener(s, this.handleEvent);
         this.handlers = t
     }
     keydown(e) {
         if (this.lastKeyCode = e.keyCode, this.lastKeyTime = Date.now(), e.keyCode == 9 && Date.now() < this.lastEscPress + 2e3) return !0;
         if (e.keyCode != 27 && Ud.indexOf(e.keyCode) < 0 && (this.view.inputState.lastEscPress = 0), ee.android && ee.chrome && !e.synthetic && (e.keyCode == 13 || e.keyCode == 8)) return this.view.observer.delayAndroidKey(e.key, e.keyCode), !0;
         let t;
-        return ee.ios && !e.synthetic && !e.altKey && !e.metaKey && ((t = Vd.find(i => i.keyCode == e.keyCode)) && !e.ctrlKey || fy.indexOf(e.key) > -1 && e.ctrlKey && !e.shiftKey) ? (this.pendingIOSKey = t || e, setTimeout(() => this.flushIOSKey(), 250), !0) : (e.keyCode != 229 && this.view.observer.forceFlush(), !1)
+        return ee.ios && !e.synthetic && !e.altKey && !e.metaKey && ((t = Vd.find(i => i.keyCode == e.keyCode)) && !e.ctrlKey || uy.indexOf(e.key) > -1 && e.ctrlKey && !e.shiftKey) ? (this.pendingIOSKey = t || e, setTimeout(() => this.flushIOSKey(), 250), !0) : (e.keyCode != 229 && this.view.observer.forceFlush(), !1)
     }
     flushIOSKey() {
         let e = this.pendingIOSKey;
         return e ? (this.pendingIOSKey = void 0, mr(this.view.contentDOM, e.key, e.keyCode)) : !1
     }
     ignoreDuringComposition(e) {
         return /^key/.test(e.type) ? this.composing > 0 ? !0 : ee.safari && !ee.ios && this.compositionPendingKey && Date.now() - this.compositionEndedAt < 100 ? (this.compositionPendingKey = !1, !0) : !1 : !1
@@ -8079,15 +8079,15 @@
             return e.call(n, i, t)
         } catch (r) {
             ni(t.state, r)
         }
     }
 }
 
-function cy(n) {
+function fy(n) {
     let e = Object.create(null);
 
     function t(i) {
         return e[i] || (e[i] = {
             observers: [],
             handlers: []
         })
@@ -8122,41 +8122,41 @@
         keyCode: 13,
         inputType: "insertLineBreak"
     }, {
         key: "Delete",
         keyCode: 46,
         inputType: "deleteContentForward"
     }],
-    fy = "dthko",
+    uy = "dthko",
     Ud = [16, 17, 18, 20, 91, 92, 224, 225],
     no = 6;
 
 function ro(n) {
     return Math.max(0, n) * .7 + 8
 }
 
-function uy(n, e) {
+function dy(n, e) {
     return Math.max(Math.abs(n.clientX - e.clientX), Math.abs(n.clientY - e.clientY))
 }
-class dy {
+class py {
     constructor(e, t, i, r) {
         this.view = e, this.startEvent = t, this.style = i, this.mustSelect = r, this.scrollSpeed = {
             x: 0,
             y: 0
-        }, this.scrolling = -1, this.lastEvent = t, this.scrollParent = E0(e.contentDOM), this.atoms = e.state.facet(Fh).map(o => o(e));
+        }, this.scrolling = -1, this.lastEvent = t, this.scrollParent = D0(e.contentDOM), this.atoms = e.state.facet(Fh).map(o => o(e));
         let s = e.contentDOM.ownerDocument;
-        s.addEventListener("mousemove", this.move = this.move.bind(this)), s.addEventListener("mouseup", this.up = this.up.bind(this)), this.extend = t.shiftKey, this.multiple = e.state.facet(Ee.allowMultipleSelections) && py(e, t), this.dragging = my(e, t) && Xd(t) == 1 ? null : !1
+        s.addEventListener("mousemove", this.move = this.move.bind(this)), s.addEventListener("mouseup", this.up = this.up.bind(this)), this.extend = t.shiftKey, this.multiple = e.state.facet(Ee.allowMultipleSelections) && gy(e, t), this.dragging = yy(e, t) && Xd(t) == 1 ? null : !1
     }
     start(e) {
         this.dragging === !1 && this.select(e)
     }
     move(e) {
         var t;
         if (e.buttons == 0) return this.destroy();
-        if (this.dragging || this.dragging == null && uy(this.startEvent, e) < 10) return;
+        if (this.dragging || this.dragging == null && dy(this.startEvent, e) < 10) return;
         this.select(this.lastEvent = e);
         let i = 0,
             r = 0,
             s = ((t = this.scrollParent) === null || t === void 0 ? void 0 : t.getBoundingClientRect()) || {
                 left: 0,
                 top: 0,
                 right: this.view.win.innerWidth,
@@ -8209,51 +8209,51 @@
         }), this.mustSelect = !1
     }
     update(e) {
         this.style.update(e) && setTimeout(() => this.select(this.lastEvent), 20)
     }
 }
 
-function py(n, e) {
+function gy(n, e) {
     let t = n.state.facet(Ad);
     return t.length ? t[0](e) : ee.mac ? e.metaKey : e.ctrlKey
 }
 
-function gy(n, e) {
+function my(n, e) {
     let t = n.state.facet(Td);
     return t.length ? t[0](e) : ee.mac ? !e.altKey : !e.ctrlKey
 }
 
-function my(n, e) {
+function yy(n, e) {
     let {
         main: t
     } = n.state.selection;
     if (t.empty) return !1;
     let i = $o(n.root);
     if (!i || i.rangeCount == 0) return !0;
     let r = i.getRangeAt(0).getClientRects();
     for (let s = 0; s < r.length; s++) {
         let o = r[s];
         if (o.left <= e.clientX && o.right >= e.clientX && o.top <= e.clientY && o.bottom >= e.clientY) return !0
     }
     return !1
 }
 
-function yy(n, e) {
+function by(n, e) {
     if (!e.bubbles) return !0;
     if (e.defaultPrevented) return !1;
     for (let t = e.target, i; t != n.contentDOM; t = t.parentNode)
         if (!t || t.nodeType == 11 || (i = je.get(t)) && i.ignoreEvent(e)) return !1;
     return !0
 }
 const di = Object.create(null),
     pi = Object.create(null),
     Qd = ee.ie && ee.ie_version < 15 || ee.ios && ee.webkit_version < 604;
 
-function by(n) {
+function xy(n) {
     let e = n.dom.parentNode;
     if (!e) return;
     let t = e.appendChild(document.createElement("textarea"));
     t.style.cssText = "position: fixed; left: -10000px; top: 10px", t.focus(), setTimeout(() => {
         n.focus(), t.remove(), Gd(n, t.value)
     }, 50)
 }
@@ -8266,21 +8266,21 @@
         let h = -1;
         i = t.changeByRange(f => {
             let u = t.doc.lineAt(f.from);
             if (u.from == h) return {
                 range: f
             };
             h = u.from;
-            let g = t.toText((o ? s.line(r++).text : e) + t.lineBreak);
+            let m = t.toText((o ? s.line(r++).text : e) + t.lineBreak);
             return {
                 changes: {
                     from: u.from,
-                    insert: g
+                    insert: m
                 },
-                range: H.cursor(f.from + g.length)
+                range: H.cursor(f.from + m.length)
             }
         })
     } else o ? i = t.changeByRange(h => {
         let f = s.line(r++);
         return {
             changes: {
                 from: h.from,
@@ -8306,38 +8306,38 @@
     n.inputState.setSelectionOrigin("select.pointer")
 };
 di.mousedown = (n, e) => {
     if (n.observer.flush(), n.inputState.lastTouchTime > Date.now() - 2e3) return !1;
     let t = null;
     for (let i of n.state.facet(Od))
         if (t = i(n, e), t) break;
-    if (!t && e.button == 0 && (t = wy(n, e)), t) {
+    if (!t && e.button == 0 && (t = vy(n, e)), t) {
         let i = !n.hasFocus;
-        n.inputState.startMouseSelection(new dy(n, e, t, i)), i && n.observer.ignore(() => dd(n.contentDOM));
+        n.inputState.startMouseSelection(new py(n, e, t, i)), i && n.observer.ignore(() => dd(n.contentDOM));
         let r = n.inputState.mouseSelection;
         if (r) return r.start(e), r.dragging === !1
     }
     return !1
 };
 
 function ff(n, e, t, i) {
     if (i == 1) return H.cursor(e, t);
-    if (i == 2) return ty(n.state, e, t);
+    if (i == 2) return iy(n.state, e, t);
     {
         let r = tt.find(n.docView, e),
             s = n.state.doc.lineAt(r ? r.posAtEnd : e),
             o = r ? r.posAtStart : s.from,
             l = r ? r.posAtEnd : s.to;
         return l < n.state.doc.length && l == s.to && l++, H.range(o, l)
     }
 }
 let Kd = (n, e) => n >= e.top && n <= e.bottom,
     uf = (n, e, t) => Kd(e, t) && n >= t.left && n <= t.right;
 
-function xy(n, e, t, i) {
+function ky(n, e, t, i) {
     let r = tt.find(n.docView, e);
     if (!r) return 1;
     let s = e - r.posAtStart;
     if (s == 0) return 1;
     if (s == r.length) return -1;
     let o = r.coordsAt(s, -1);
     if (o && uf(t, i, o)) return -1;
@@ -8348,52 +8348,52 @@
 function df(n, e) {
     let t = n.posAtCoords({
         x: e.clientX,
         y: e.clientY
     }, !1);
     return {
         pos: t,
-        bias: xy(n, t, e.clientX, e.clientY)
+        bias: ky(n, t, e.clientX, e.clientY)
     }
 }
-const ky = ee.ie && ee.ie_version <= 11;
+const wy = ee.ie && ee.ie_version <= 11;
 let pf = null,
     gf = 0,
     mf = 0;
 
 function Xd(n) {
-    if (!ky) return n.detail;
+    if (!wy) return n.detail;
     let e = pf,
         t = mf;
     return pf = n, mf = Date.now(), gf = !e || t > Date.now() - 400 && Math.abs(e.clientX - n.clientX) < 2 && Math.abs(e.clientY - n.clientY) < 2 ? (gf + 1) % 3 : 1
 }
 
-function wy(n, e) {
+function vy(n, e) {
     let t = df(n, e),
         i = Xd(e),
         r = n.state.selection;
     return {
         update(s) {
             s.docChanged && (t.pos = s.changes.mapPos(t.pos), r = r.map(s.changes))
         },
         get(s, o, l) {
             let h = df(n, s),
                 f, u = ff(n, h.pos, h.bias, i);
             if (t.pos != h.pos && !o) {
-                let g = ff(n, t.pos, t.bias, i),
-                    y = Math.min(g.from, u.from),
-                    k = Math.max(g.to, u.to);
+                let m = ff(n, t.pos, t.bias, i),
+                    y = Math.min(m.from, u.from),
+                    k = Math.max(m.to, u.to);
                 u = y < u.from ? H.range(y, k) : H.range(k, y)
             }
-            return o ? r.replaceRange(r.main.extend(u.from, u.to)) : l && i == 1 && r.ranges.length > 1 && (f = vy(r, h.pos)) ? f : l ? r.addRange(u) : H.create([u])
+            return o ? r.replaceRange(r.main.extend(u.from, u.to)) : l && i == 1 && r.ranges.length > 1 && (f = Sy(r, h.pos)) ? f : l ? r.addRange(u) : H.create([u])
         }
     }
 }
 
-function vy(n, e) {
+function Sy(n, e) {
     for (let t = 0; t < n.ranges.length; t++) {
         let {
             from: i,
             to: r
         } = n.ranges[t];
         if (i <= e && r >= e) return H.create(n.ranges.slice(0, t).concat(n.ranges.slice(t + 1)), n.mainIndex == t ? 0 : n.mainIndex - (n.mainIndex > t ? 1 : 0))
     }
@@ -8425,15 +8425,15 @@
     let r = n.posAtCoords({
             x: e.clientX,
             y: e.clientY
         }, !1),
         {
             draggedContent: s
         } = n.inputState,
-        o = i && s && gy(n, e) ? {
+        o = i && s && my(n, e) ? {
             from: s.from,
             to: s.to
         } : null,
         l = {
             from: r,
             insert: t
         },
@@ -8470,27 +8470,27 @@
     }
     return !1
 };
 di.paste = (n, e) => {
     if (n.state.readOnly) return !0;
     n.observer.flush();
     let t = Qd ? null : e.clipboardData;
-    return t ? (Gd(n, t.getData("text/plain") || t.getData("text/uri-text")), !0) : (by(n), !1)
+    return t ? (Gd(n, t.getData("text/plain") || t.getData("text/uri-text")), !0) : (xy(n), !1)
 };
 
-function Sy(n, e) {
+function Cy(n, e) {
     let t = n.dom.parentNode;
     if (!t) return;
     let i = t.appendChild(document.createElement("textarea"));
     i.style.cssText = "position: fixed; left: -10000px; top: 10px", i.value = e, i.focus(), i.selectionEnd = e.length, i.selectionStart = 0, setTimeout(() => {
         i.remove(), n.focus()
     }, 50)
 }
 
-function Cy(n) {
+function Ay(n) {
     let e = [],
         t = [],
         i = !1;
     for (let r of n.selection.ranges) r.empty || (e.push(n.sliceDoc(r.from, r.to)), t.push(r));
     if (!e.length) {
         let r = -1;
         for (let {
@@ -8513,23 +8513,23 @@
 }
 let nh = null;
 di.copy = di.cut = (n, e) => {
     let {
         text: t,
         ranges: i,
         linewise: r
-    } = Cy(n.state);
+    } = Ay(n.state);
     if (!t && !r) return !1;
     nh = r ? t : null, e.type == "cut" && !n.state.readOnly && n.dispatch({
         changes: i,
         scrollIntoView: !0,
         userEvent: "delete.cut"
     });
     let s = Qd ? null : e.clipboardData;
-    return s ? (s.clearData(), s.setData("text/plain", t), !0) : (Sy(n, t), !1)
+    return s ? (s.clearData(), s.setData("text/plain", t), !0) : (Cy(n, t), !1)
 };
 const Yd = Xi.define();
 
 function Jd(n, e) {
     let t = [];
     for (let i of n.facet(Dd)) {
         let r = i(n, e);
@@ -8577,19 +8577,19 @@
             (((s = window.visualViewport) === null || s === void 0 ? void 0 : s.height) || 0) > r + 10 && n.hasFocus && (n.contentDOM.blur(), n.focus())
         }, 100)
     }
     return !1
 };
 const bf = new Set;
 
-function Ay(n) {
+function Ty(n) {
     bf.has(n) || (bf.add(n), n.addEventListener("copy", () => {}), n.addEventListener("cut", () => {}))
 }
 const xf = ["pre-wrap", "normal", "pre-line", "break-spaces"];
-class Ty {
+class Oy {
     constructor(e) {
         this.lineWrapping = e, this.doc = De.empty, this.heightSamples = {}, this.lineHeight = 14, this.charWidth = 7, this.textHeight = 14, this.lineLength = 30, this.heightChanged = !1
     }
     heightForGap(e, t) {
         let i = this.doc.lineAt(t).number - this.doc.lineAt(e).number + 1;
         return this.lineWrapping && (i += Math.max(0, Math.ceil((t - e - i * this.lineLength * .5) / this.lineLength))), this.lineHeight * i
     }
@@ -8619,15 +8619,15 @@
                 let u = o[f];
                 u < 0 ? f++ : this.heightSamples[Math.floor(u * 10)] = !0
             }
         }
         return h
     }
 }
-class Oy {
+class My {
     constructor(e, t) {
         this.from = e, this.heights = t, this.index = 0
     }
     get more() {
         return this.index < this.heights.length
     }
 }
@@ -8685,19 +8685,19 @@
         let s = this,
             o = i.doc;
         for (let l = r.length - 1; l >= 0; l--) {
             let {
                 fromA: h,
                 toA: f,
                 fromB: u,
-                toB: g
+                toB: m
             } = r[l], y = s.lineAt(h, qe.ByPosNoHeight, i.setDoc(t), 0, 0), k = y.to >= f ? y : s.lineAt(f, qe.ByPosNoHeight, i, 0, 0);
-            for (g += k.to - f, f = k.to; l > 0 && y.from <= r[l - 1].toA;) h = r[l - 1].fromA, u = r[l - 1].fromB, l--, h < y.from && (y = s.lineAt(h, qe.ByPosNoHeight, i, 0, 0));
+            for (m += k.to - f, f = k.to; l > 0 && y.from <= r[l - 1].toA;) h = r[l - 1].fromA, u = r[l - 1].fromB, l--, h < y.from && (y = s.lineAt(h, qe.ByPosNoHeight, i, 0, 0));
             u += y.from - h, h = y.from;
-            let v = zh.build(i.setDoc(o), e, u, g);
+            let v = zh.build(i.setDoc(o), e, u, m);
             s = s.replace(h, f, v)
         }
         return s.updateHeight(i, 0)
     }
     static empty() {
         return new jt(0, 0)
     }
@@ -8720,15 +8720,15 @@
             let l = e[t++];
             l && (r += l.size)
         } else {
             let l = e[--i];
             l && (s += l.size)
         }
         let o = 0;
-        return e[t - 1] == null ? (o = 1, t--) : e[t] == null && (o = 1, i++), new My(Rt.of(e.slice(0, t)), o, Rt.of(e.slice(i)))
+        return e[t - 1] == null ? (o = 1, t--) : e[t] == null && (o = 1, i++), new Ey(Rt.of(e.slice(0, t)), o, Rt.of(e.slice(i)))
     }
 }
 Rt.prototype.size = 1;
 class ep extends Rt {
     constructor(e, t, i) {
         super(e, t), this.deco = i
     }
@@ -8792,24 +8792,24 @@
             lastLine: o,
             perLine: l,
             perChar: h
         } = this.heightMetrics(t, r);
         if (t.lineWrapping) {
             let f = r + Math.round(Math.max(0, Math.min(1, (e - i) / this.height)) * this.length),
                 u = t.doc.lineAt(f),
-                g = l + u.length * h,
-                y = Math.max(i, e - g / 2);
-            return new Li(u.from, u.length, y, g, 0)
+                m = l + u.length * h,
+                y = Math.max(i, e - m / 2);
+            return new Li(u.from, u.length, y, m, 0)
         } else {
             let f = Math.max(0, Math.min(o - s, Math.floor((e - i) / l))),
                 {
                     from: u,
-                    length: g
+                    length: m
                 } = t.doc.line(s + f);
-            return new Li(u, g, i + l * f, l, 0)
+            return new Li(u, m, i + l * f, l, 0)
         }
     }
     lineAt(e, t, i, r, s) {
         if (t == qe.ByHeight) return this.blockAt(e, i, r, s);
         if (t == qe.ByPosNoHeight) {
             let {
                 from: k,
@@ -8817,32 +8817,32 @@
             } = i.doc.lineAt(e);
             return new Li(k, v - k, 0, 0, 0)
         }
         let {
             firstLine: o,
             perLine: l,
             perChar: h
-        } = this.heightMetrics(i, s), f = i.doc.lineAt(e), u = l + f.length * h, g = f.number - o, y = r + l * g + h * (f.from - s - g);
+        } = this.heightMetrics(i, s), f = i.doc.lineAt(e), u = l + f.length * h, m = f.number - o, y = r + l * m + h * (f.from - s - m);
         return new Li(f.from, f.length, Math.max(r, Math.min(y, r + this.height - u)), u, 0)
     }
     forEachLine(e, t, i, r, s, o) {
         e = Math.max(e, s), t = Math.min(t, s + this.length);
         let {
             firstLine: l,
             perLine: h,
             perChar: f
         } = this.heightMetrics(i, s);
-        for (let u = e, g = r; u <= t;) {
+        for (let u = e, m = r; u <= t;) {
             let y = i.doc.lineAt(u);
             if (u == e) {
                 let v = y.number - l;
-                g += h * v + f * (e - s - v)
+                m += h * v + f * (e - s - v)
             }
             let k = h + f * y.length;
-            o(new Li(y.from, y.length, g, k, 0)), g += k, u = y.to + 1
+            o(new Li(y.from, y.length, m, k, 0)), m += k, u = y.to + 1
         }
     }
     replace(e, t, i) {
         let r = this.length - t;
         if (r > 0) {
             let s = i[i.length - 1];
             s instanceof dt ? i[i.length - 1] = new dt(s.length + r) : i.push(null, new dt(r - 1))
@@ -8864,30 +8864,30 @@
         if (r && r.from <= t + this.length && r.more) {
             let o = [],
                 l = Math.max(t, r.from),
                 h = -1;
             for (r.from > t && o.push(new dt(r.from - t - 1).updateHeight(e, t)); l <= s && r.more;) {
                 let u = e.doc.lineAt(l).length;
                 o.length && o.push(null);
-                let g = r.heights[r.index++];
-                h == -1 ? h = g : Math.abs(g - h) >= Lo && (h = -2);
-                let y = new jt(u, g);
+                let m = r.heights[r.index++];
+                h == -1 ? h = m : Math.abs(m - h) >= Lo && (h = -2);
+                let y = new jt(u, m);
                 y.outdated = !1, o.push(y), l += u + 1
             }
             l <= s && o.push(null, new dt(s - l).updateHeight(e, l));
             let f = Rt.of(o);
             return (h < 0 || Math.abs(f.height - this.height) >= Lo || Math.abs(h - this.heightMetrics(e, t).perLine) >= Lo) && (e.heightChanged = !0), f
         } else(i || this.outdated) && (this.setHeight(e, e.heightForGap(t, t + this.length)), this.outdated = !1);
         return this
     }
     toString() {
         return `gap(${this.length})`
     }
 }
-class My extends Rt {
+class Ey extends Rt {
     constructor(e, t, i) {
         super(e.length + t + i.length, e.height + i.height, t | (e.outdated || i.outdated ? 2 : 0)), this.left = e, this.right = i, this.size = e.size + i.size
     }
     get break() {
         return this.flags & 1
     }
     blockAt(e, t, i, r) {
@@ -8952,15 +8952,15 @@
     }
 }
 
 function kf(n, e) {
     let t, i;
     n[e] == null && (t = n[e - 1]) instanceof dt && (i = n[e + 1]) instanceof dt && n.splice(e - 1, 3, new dt(t.length + 1 + i.length))
 }
-const Ey = 5;
+const Dy = 5;
 class zh {
     constructor(e, t) {
         this.pos = e, this.oracle = t, this.nodes = [], this.lineStart = -1, this.lineEnd = -1, this.covering = null, this.writtenTo = e
     }
     get isCovered() {
         return this.covering && this.nodes[this.nodes.length - 1] == this.covering
     }
@@ -8974,15 +8974,15 @@
     }
     point(e, t, i) {
         if (e < t || i.heightRelevant) {
             let r = i.widget ? i.widget.estimatedHeight : 0,
                 s = i.widget ? i.widget.lineBreaks : 0;
             r < 0 && (r = this.oracle.lineHeight);
             let o = t - e;
-            i.block ? this.addBlock(new ep(o, r, i)) : (o || s || r >= Ey) && this.addLineDeco(r, s, o)
+            i.block ? this.addBlock(new ep(o, r, i)) : (o || s || r >= Dy) && this.addLineDeco(r, s, o)
         } else t > e && this.span(e, t);
         this.lineEnd > -1 && this.lineEnd < this.pos && (this.lineEnd = this.oracle.doc.lineAt(this.pos).to)
     }
     enterLine() {
         if (this.lineStart > -1) return;
         let {
             from: e,
@@ -9019,56 +9019,56 @@
     }
     static build(e, t, i, r) {
         let s = new zh(i, e);
         return Pe.spans(t, i, r, s, 0), s.finish(i)
     }
 }
 
-function Dy(n, e, t) {
-    let i = new Ry;
+function Ry(n, e, t) {
+    let i = new Ly;
     return Pe.compare(n, e, t, i, 0), i.changes
 }
-class Ry {
+class Ly {
     constructor() {
         this.changes = []
     }
     compareRange() {}
     comparePoint(e, t, i, r) {
         (e < t || i && i.heightRelevant || r && r.heightRelevant) && Xa(e, t, this.changes, 5)
     }
 }
 
-function Ly(n, e) {
+function Py(n, e) {
     let t = n.getBoundingClientRect(),
         i = n.ownerDocument,
         r = i.defaultView || window,
         s = Math.max(0, t.left),
         o = Math.min(r.innerWidth, t.right),
         l = Math.max(0, t.top),
         h = Math.min(r.innerHeight, t.bottom);
     for (let f = n.parentNode; f && f != i.body;)
         if (f.nodeType == 1) {
             let u = f,
-                g = window.getComputedStyle(u);
-            if ((u.scrollHeight > u.clientHeight || u.scrollWidth > u.clientWidth) && g.overflow != "visible") {
+                m = window.getComputedStyle(u);
+            if ((u.scrollHeight > u.clientHeight || u.scrollWidth > u.clientWidth) && m.overflow != "visible") {
                 let y = u.getBoundingClientRect();
                 s = Math.max(s, y.left), o = Math.min(o, y.right), l = Math.max(l, y.top), h = f == n.parentNode ? y.bottom : Math.min(h, y.bottom)
             }
-            f = g.position == "absolute" || g.position == "fixed" ? u.offsetParent : u.parentNode
+            f = m.position == "absolute" || m.position == "fixed" ? u.offsetParent : u.parentNode
         } else if (f.nodeType == 11) f = f.host;
     else break;
     return {
         left: s - t.left,
         right: Math.max(s, o) - t.left,
         top: l - (t.top + e),
         bottom: Math.max(l, h) - (t.top + e)
     }
 }
 
-function Py(n, e) {
+function Ny(n, e) {
     let t = n.getBoundingClientRect();
     return {
         left: 0,
         right: t.right - t.left,
         top: e,
         bottom: t.bottom - (t.top + e)
     }
@@ -9084,19 +9084,19 @@
                 s = t[i];
             if (r.from != s.from || r.to != s.to || r.size != s.size) return !1
         }
         return !0
     }
     draw(e, t) {
         return de.replace({
-            widget: new Ny(this.size * (t ? e.scaleY : e.scaleX), t)
+            widget: new Iy(this.size * (t ? e.scaleY : e.scaleX), t)
         }).range(this.from, this.to)
     }
 }
-class Ny extends An {
+class Iy extends An {
     constructor(e, t) {
         super(), this.size = e, this.vertical = t
     }
     eq(e) {
         return e.size == this.size && e.vertical == this.vertical
     }
     toDOM() {
@@ -9112,15 +9112,15 @@
         this.state = e, this.pixelViewport = {
             left: 0,
             right: window.innerWidth,
             top: 0,
             bottom: 0
         }, this.inView = !0, this.paddingTop = 0, this.paddingBottom = 0, this.contentDOMWidth = 0, this.contentDOMHeight = 0, this.editorHeight = 0, this.editorWidth = 0, this.scrollTop = 0, this.scrolledToBottom = !0, this.scaleX = 1, this.scaleY = 1, this.scrollAnchorPos = 0, this.scrollAnchorHeight = -1, this.scaler = vf, this.scrollTarget = null, this.printing = !1, this.mustMeasureContent = !0, this.defaultTextDirection = Ue.LTR, this.visibleRanges = [], this.mustEnforceCursorAssoc = !1;
         let t = e.facet(Hh).some(i => typeof i != "function" && i.class == "cm-lineWrapping");
-        this.heightOracle = new Ty(t), this.stateDeco = e.facet(gs).filter(i => typeof i != "function"), this.heightMap = Rt.empty().applyChanges(this.stateDeco, De.empty, this.heightOracle.setDoc(e.doc), [new ri(0, 0, 0, e.doc.length)]), this.viewport = this.getViewport(0, null), this.updateViewportLines(), this.updateForViewport(), this.lineGaps = this.ensureLineGaps([]), this.lineGapDeco = de.set(this.lineGaps.map(i => i.draw(this, !1))), this.computeVisibleRanges()
+        this.heightOracle = new Oy(t), this.stateDeco = e.facet(gs).filter(i => typeof i != "function"), this.heightMap = Rt.empty().applyChanges(this.stateDeco, De.empty, this.heightOracle.setDoc(e.doc), [new ri(0, 0, 0, e.doc.length)]), this.viewport = this.getViewport(0, null), this.updateViewportLines(), this.updateForViewport(), this.lineGaps = this.ensureLineGaps([]), this.lineGapDeco = de.set(this.lineGaps.map(i => i.draw(this, !1))), this.computeVisibleRanges()
     }
     updateForViewport() {
         let e = [this.viewport],
             {
                 main: t
             } = this.state.selection;
         for (let i = 0; i <= 1; i++) {
@@ -9132,27 +9132,27 @@
                 let {
                     from: s,
                     to: o
                 } = this.lineBlockAt(r);
                 e.push(new so(s, o))
             }
         }
-        this.viewports = e.sort((i, r) => i.from - r.from), this.scaler = this.heightMap.height <= 7e6 ? vf : new _y(this.heightOracle, this.heightMap, this.viewports)
+        this.viewports = e.sort((i, r) => i.from - r.from), this.scaler = this.heightMap.height <= 7e6 ? vf : new Hy(this.heightOracle, this.heightMap, this.viewports)
     }
     updateViewportLines() {
         this.viewportLines = [], this.heightMap.forEachLine(this.viewport.from, this.viewport.to, this.heightOracle.setDoc(this.state.doc), 0, 0, e => {
             this.viewportLines.push(this.scaler.scale == 1 ? e : ts(e, this.scaler))
         })
     }
     update(e, t = null) {
         this.state = e.state;
         let i = this.stateDeco;
         this.stateDeco = this.state.facet(gs).filter(u => typeof u != "function");
         let r = e.changedRanges,
-            s = ri.extendWithRanges(r, Dy(i, this.stateDeco, e ? e.changes : it.empty(this.state.doc.length))),
+            s = ri.extendWithRanges(r, Ry(i, this.stateDeco, e ? e.changes : it.empty(this.state.doc.length))),
             o = this.heightMap.height,
             l = this.scrolledToBottom ? null : this.scrollAnchorAt(this.scrollTop);
         this.heightMap = this.heightMap.applyChanges(this.stateDeco, e.startState.doc, this.heightOracle.setDoc(this.state.doc), s), this.heightMap.height != o && (e.flags |= 2), l ? (this.scrollAnchorPos = e.changes.mapPos(l.from, -1), this.scrollAnchorHeight = l.top) : (this.scrollAnchorPos = -1, this.scrollAnchorHeight = this.heightMap.height);
         let h = s.length ? this.mapViewport(this.viewport, e.changes) : this.viewport;
         (t && (t.range.head < h.from || t.range.head > h.to) || !this.viewportIsAppropriate(h)) && (h = this.getViewport(0, t));
         let f = !e.changes.empty || e.flags & 2 || h.from != this.viewport.from || h.to != this.viewport.to;
         this.viewport = h, this.updateForViewport(), f && this.updateViewportLines(), (this.lineGaps.length || this.viewport.to - this.viewport.from > 4e3) && this.updateLineGaps(this.ensureLineGaps(this.mapLineGaps(this.lineGaps, e.changes))), e.flags |= this.computeVisibleRanges(), t && (this.scrollTarget = t), !this.mustEnforceCursorAssoc && e.selectionSet && e.view.lineWrapping && e.state.selection.main.empty && e.state.selection.main.assoc && !e.state.facet(Ld) && (this.mustEnforceCursorAssoc = !0)
@@ -9172,21 +9172,21 @@
         if (l.width && l.height) {
             let {
                 scaleX: j,
                 scaleY: z
             } = ud(t, l);
             (this.scaleX != j || this.scaleY != z) && (this.scaleX = j, this.scaleY = z, f |= 8, o = h = !0)
         }
-        let g = (parseInt(i.paddingTop) || 0) * this.scaleY,
+        let m = (parseInt(i.paddingTop) || 0) * this.scaleY,
             y = (parseInt(i.paddingBottom) || 0) * this.scaleY;
-        (this.paddingTop != g || this.paddingBottom != y) && (this.paddingTop = g, this.paddingBottom = y, f |= 10), this.editorWidth != e.scrollDOM.clientWidth && (r.lineWrapping && (h = !0), this.editorWidth = e.scrollDOM.clientWidth, f |= 8);
+        (this.paddingTop != m || this.paddingBottom != y) && (this.paddingTop = m, this.paddingBottom = y, f |= 10), this.editorWidth != e.scrollDOM.clientWidth && (r.lineWrapping && (h = !0), this.editorWidth = e.scrollDOM.clientWidth, f |= 8);
         let k = e.scrollDOM.scrollTop * this.scaleY;
         this.scrollTop != k && (this.scrollAnchorHeight = -1, this.scrollTop = k), this.scrolledToBottom = gd(e.scrollDOM);
-        let v = (this.printing ? Py : Ly)(t, this.paddingTop),
-            C = v.top - this.pixelViewport.top,
+        let v = (this.printing ? Ny : Py)(t, this.paddingTop),
+            A = v.top - this.pixelViewport.top,
             O = v.bottom - this.pixelViewport.bottom;
         this.pixelViewport = v;
         let D = this.pixelViewport.bottom > this.pixelViewport.top && this.pixelViewport.right > this.pixelViewport.left;
         if (D != this.inView && (this.inView = D, D && (h = !0)), !this.inView && !this.scrollTarget) return 0;
         let F = l.width;
         if ((this.contentDOMWidth != F || this.editorHeight != e.scrollDOM.clientHeight) && (this.contentDOMWidth = l.width, this.editorHeight = e.scrollDOM.clientHeight, f |= 8), h) {
             let j = e.docView.measureVisibleLineHeights(this.viewport);
@@ -9194,18 +9194,18 @@
                 let {
                     lineHeight: z,
                     charWidth: G,
                     textHeight: p
                 } = e.docView.measureTextSize();
                 o = z > 0 && r.refresh(s, z, G, p, F / G, j), o && (e.docView.minWidth = 0, f |= 8)
             }
-            C > 0 && O > 0 ? u = Math.max(C, O) : C < 0 && O < 0 && (u = Math.min(C, O)), r.heightChanged = !1;
+            A > 0 && O > 0 ? u = Math.max(A, O) : A < 0 && O < 0 && (u = Math.min(A, O)), r.heightChanged = !1;
             for (let z of this.viewports) {
                 let G = z.from == this.viewport.from ? j : e.docView.measureVisibleLineHeights(z);
-                this.heightMap = (o ? Rt.empty().applyChanges(this.stateDeco, De.empty, this.heightOracle, [new ri(0, 0, 0, e.state.doc.length)]) : this.heightMap).updateHeight(r, 0, o, new Oy(z.from, G))
+                this.heightMap = (o ? Rt.empty().applyChanges(this.stateDeco, De.empty, this.heightOracle, [new ri(0, 0, 0, e.state.doc.length)]) : this.heightMap).updateHeight(r, 0, o, new My(z.from, G))
             }
             r.heightChanged && (f |= 2)
         }
         let $ = !this.viewportIsAppropriate(this.viewport, u) || this.scrollTarget && (this.scrollTarget.range.head < this.viewport.from || this.scrollTarget.range.head > this.viewport.to);
         return $ && (this.viewport = this.getViewport(u, this.scrollTarget)), this.updateForViewport(), (f & 2 || $) && this.updateViewportLines(), (this.lineGaps.length || this.viewport.to - this.viewport.from > 4e3) && this.updateLineGaps(this.ensureLineGaps(o ? [] : this.lineGaps, e)), f |= this.computeVisibleRanges(), this.mustEnforceCursorAssoc && (this.mustEnforceCursorAssoc = !1, e.docView.enforceCursorAssoc()), f
     }
     get visibleTop() {
@@ -9225,17 +9225,17 @@
             h = new so(r.lineAt(o - i * 1e3, qe.ByHeight, s, 0, 0).from, r.lineAt(l + (1 - i) * 1e3, qe.ByHeight, s, 0, 0).to);
         if (t) {
             let {
                 head: f
             } = t.range;
             if (f < h.from || f > h.to) {
                 let u = Math.min(this.editorHeight, this.pixelViewport.bottom - this.pixelViewport.top),
-                    g = r.lineAt(f, qe.ByPos, s, 0, 0),
+                    m = r.lineAt(f, qe.ByPos, s, 0, 0),
                     y;
-                t.y == "center" ? y = (g.top + g.bottom) / 2 - u / 2 : t.y == "start" || t.y == "nearest" && f < h.from ? y = g.top : y = g.bottom - u, h = new so(r.lineAt(y - 1e3 / 2, qe.ByHeight, s, 0, 0).from, r.lineAt(y + u + 1e3 / 2, qe.ByHeight, s, 0, 0).to)
+                t.y == "center" ? y = (m.top + m.bottom) / 2 - u / 2 : t.y == "start" || t.y == "nearest" && f < h.from ? y = m.top : y = m.bottom - u, h = new so(r.lineAt(y - 1e3 / 2, qe.ByHeight, s, 0, 0).from, r.lineAt(y + u + 1e3 / 2, qe.ByHeight, s, 0, 0).to)
             }
         }
         return h
     }
     mapViewport(e, t) {
         let i = t.mapPos(e.from, -1),
             r = t.mapPos(e.to, 1);
@@ -9265,57 +9265,57 @@
     ensureLineGaps(e, t) {
         let i = this.heightOracle.lineWrapping,
             r = i ? 1e4 : 2e3,
             s = r >> 1,
             o = r << 1;
         if (this.defaultTextDirection != Ue.LTR && !i) return [];
         let l = [],
-            h = (f, u, g, y) => {
+            h = (f, u, m, y) => {
                 if (u - f < s) return;
                 let k = this.state.selection.main,
                     v = [k.from];
                 k.empty || v.push(k.to);
                 for (let O of v)
                     if (O > f && O < u) {
-                        h(f, O - 10, g, y), h(O + 10, u, g, y);
+                        h(f, O - 10, m, y), h(O + 10, u, m, y);
                         return
-                    } let C = By(e, O => O.from >= g.from && O.to <= g.to && Math.abs(O.from - f) < s && Math.abs(O.to - u) < s && !v.some(D => O.from < D && O.to > D));
-                if (!C) {
-                    if (u < g.to && t && i && t.visibleRanges.some(O => O.from <= u && O.to >= u)) {
+                    } let A = _y(e, O => O.from >= m.from && O.to <= m.to && Math.abs(O.from - f) < s && Math.abs(O.to - u) < s && !v.some(D => O.from < D && O.to > D));
+                if (!A) {
+                    if (u < m.to && t && i && t.visibleRanges.some(O => O.from <= u && O.to >= u)) {
                         let O = t.moveToLineBoundary(H.cursor(u), !1, !0).head;
                         O > f && (u = O)
                     }
-                    C = new sa(f, u, this.gapSize(g, f, u, y))
+                    A = new sa(f, u, this.gapSize(m, f, u, y))
                 }
-                l.push(C)
+                l.push(A)
             };
         for (let f of this.viewportLines) {
             if (f.length < o) continue;
-            let u = Iy(f.from, f.to, this.stateDeco);
+            let u = By(f.from, f.to, this.stateDeco);
             if (u.total < o) continue;
-            let g = this.scrollTarget ? this.scrollTarget.range.head : null,
+            let m = this.scrollTarget ? this.scrollTarget.range.head : null,
                 y, k;
             if (i) {
                 let v = r / this.heightOracle.lineLength * this.heightOracle.lineHeight,
-                    C, O;
-                if (g != null) {
-                    let D = lo(u, g),
+                    A, O;
+                if (m != null) {
+                    let D = lo(u, m),
                         F = ((this.visibleBottom - this.visibleTop) / 2 + v) / f.height;
-                    C = D - F, O = D + F
-                } else C = (this.visibleTop - f.top - v) / f.height, O = (this.visibleBottom - f.top + v) / f.height;
-                y = oo(u, C), k = oo(u, O)
+                    A = D - F, O = D + F
+                } else A = (this.visibleTop - f.top - v) / f.height, O = (this.visibleBottom - f.top + v) / f.height;
+                y = oo(u, A), k = oo(u, O)
             } else {
                 let v = u.total * this.heightOracle.charWidth,
-                    C = r * this.heightOracle.charWidth,
+                    A = r * this.heightOracle.charWidth,
                     O, D;
-                if (g != null) {
-                    let F = lo(u, g),
-                        $ = ((this.pixelViewport.right - this.pixelViewport.left) / 2 + C) / v;
+                if (m != null) {
+                    let F = lo(u, m),
+                        $ = ((this.pixelViewport.right - this.pixelViewport.left) / 2 + A) / v;
                     O = F - $, D = F + $
-                } else O = (this.pixelViewport.left - C) / v, D = (this.pixelViewport.right + C) / v;
+                } else O = (this.pixelViewport.left - A) / v, D = (this.pixelViewport.right + A) / v;
                 y = oo(u, O), k = oo(u, D)
             }
             y > f.from && h(f.from, y, f, u), k < f.to && h(k, f.to, f, u)
         }
         return l
     }
     gapSize(e, t, i, r) {
@@ -9363,15 +9363,15 @@
 }
 class so {
     constructor(e, t) {
         this.from = e, this.to = t
     }
 }
 
-function Iy(n, e, t) {
+function By(n, e, t) {
     let i = [],
         r = n,
         s = 0;
     return Pe.spans(t, n, e, {
         span() {},
         point(o, l) {
             o > r && (i.push({
@@ -9417,28 +9417,28 @@
             break
         }
         t += r - i
     }
     return t / n.total
 }
 
-function By(n, e) {
+function _y(n, e) {
     for (let t of n)
         if (e(t)) return t
 }
 const vf = {
     toDOM(n) {
         return n
     },
     fromDOM(n) {
         return n
     },
     scale: 1
 };
-class _y {
+class Hy {
     constructor(e, t, i) {
         let r = 0,
             s = 0,
             o = 0;
         this.viewports = i.map(({
             from: l,
             to: h
@@ -9501,15 +9501,15 @@
                 if (r == "&") return n;
                 if (!t || !t[r]) throw new RangeError(`Unsupported selector: ${r}`);
                 return t[r]
             }) : n + " " + i
         }
     })
 }
-const Hy = oh("." + sh, {
+const Fy = oh("." + sh, {
         "&": {
             position: "relative !important",
             boxSizing: "border-box",
             "&.cm-focused": {
                 outline: "1px dotted #212121"
             },
             display: "flex !important",
@@ -9760,15 +9760,15 @@
         },
         "&dark .cm-textfield": {
             border: "1px solid #555",
             backgroundColor: "inherit"
         }
     }, np),
     is = "￿";
-class Fy {
+class zy {
     constructor(e, t) {
         this.points = e, this.text = "", this.lineSeparator = t.facet(Ee.lineSeparator)
     }
     append(e) {
         this.text += e
     }
     lineBreak() {
@@ -9811,19 +9811,19 @@
             for (let r = i.iter(); !r.next().done;) r.lineBreak ? this.lineBreak() : this.append(r.value)
         } else e.nodeType == 3 ? this.readTextNode(e) : e.nodeName == "BR" ? e.nextSibling && this.lineBreak() : e.nodeType == 1 && this.readRange(e.firstChild, null)
     }
     findPointBefore(e, t) {
         for (let i of this.points) i.node == e && e.childNodes[i.offset] == t && (i.pos = this.text.length)
     }
     findPointInside(e, t) {
-        for (let i of this.points)(e.nodeType == 3 ? i.node == e : e.contains(i.node)) && (i.pos = this.text.length + (zy(e, i.node, i.offset) ? t : 0))
+        for (let i of this.points)(e.nodeType == 3 ? i.node == e : e.contains(i.node)) && (i.pos = this.text.length + ($y(e, i.node, i.offset) ? t : 0))
     }
 }
 
-function zy(n, e, t) {
+function $y(n, e, t) {
     for (;;) {
         if (!e || t < Ui(e)) return !1;
         if (e == n) return !0;
         t = ps(e) + 1, e = e.parentNode
     }
 }
 
@@ -9831,26 +9831,26 @@
     return n.nodeType == 1 && /^(DIV|P|LI|UL|OL|BLOCKQUOTE|DD|DT|H\d|SECTION|PRE)$/.test(n.nodeName)
 }
 class Cf {
     constructor(e, t) {
         this.node = e, this.offset = t, this.pos = -1
     }
 }
-class $y {
+class Wy {
     constructor(e, t, i, r) {
         this.typeOver = r, this.bounds = null, this.text = "";
         let {
             impreciseHead: s,
             impreciseAnchor: o
         } = e.docView;
         if (e.state.readOnly && t > -1) this.newSel = null;
         else if (t > -1 && (this.bounds = e.docView.domBoundsAround(t, i, 0))) {
-            let l = s || o ? [] : jy(e),
-                h = new Fy(l, e.state);
-            h.readRange(this.bounds.startDOM, this.bounds.endDOM), this.text = h.text, this.newSel = Vy(l, this.bounds.from)
+            let l = s || o ? [] : Vy(e),
+                h = new zy(l, e.state);
+            h.readRange(this.bounds.startDOM, this.bounds.endDOM), this.text = h.text, this.newSel = Uy(l, this.bounds.from)
         } else {
             let l = e.observer.selectionRange,
                 h = s && s.node == l.focusNode && s.offset == l.focusOffset || !ja(e.contentDOM, l.focusNode) ? e.state.selection.main.head : e.docView.posFromDOM(l.focusNode, l.focusOffset),
                 f = o && o.node == l.anchorNode && o.offset == l.anchorOffset || !ja(e.contentDOM, l.anchorNode) ? e.state.selection.main.anchor : e.docView.posFromDOM(l.anchorNode, l.anchorOffset);
             this.newSel = H.single(f, h)
         }
     }
@@ -9864,15 +9864,15 @@
         s = n.inputState.lastKeyTime > Date.now() - 100 ? n.inputState.lastKeyCode : -1;
     if (e.bounds) {
         let {
             from: o,
             to: l
         } = e.bounds, h = r.from, f = null;
         (s === 8 || ee.android && e.text.length < l - o) && (h = r.to, f = "end");
-        let u = qy(n.state.doc.sliceString(o, l, is), e.text, h - o, f);
+        let u = jy(n.state.doc.sliceString(o, l, is), e.text, h - o, f);
         u && (ee.chrome && s == 13 && u.toB == u.from + 2 && e.text.slice(u.from, u.toB) == is + is && u.toB--, t = {
             from: o + u.from,
             to: o + u.toA,
             insert: De.of(e.text.slice(u.from, u.toB).split(is))
         })
     } else i && (!n.hasFocus && n.state.facet(bl) || i.main.eq(r)) && (i = null);
     if (!t && !i) return !1;
@@ -9893,62 +9893,62 @@
             from: r.from,
             to: r.to,
             insert: De.of([" "])
         }), t) {
         if (ee.ios && n.inputState.flushIOSKey() || ee.android && (t.from == r.from && t.to == r.to && t.insert.length == 1 && t.insert.lines == 2 && mr(n.contentDOM, "Enter", 13) || (t.from == r.from - 1 && t.to == r.to && t.insert.length == 0 || s == 8 && t.insert.length < t.to - t.from && t.to > r.head) && mr(n.contentDOM, "Backspace", 8) || t.from == r.from && t.to == r.to + 1 && t.insert.length == 0 && mr(n.contentDOM, "Delete", 46))) return !0;
         let o = t.insert.toString();
         n.inputState.composing >= 0 && n.inputState.composing++;
-        let l, h = () => l || (l = Wy(n, t, i));
+        let l, h = () => l || (l = qy(n, t, i));
         return n.state.facet(Ed).some(f => f(n, t.from, t.to, o, h)) || n.dispatch(h()), !0
     } else if (i && !i.main.eq(r)) {
         let o = !1,
             l = "select";
         return n.inputState.lastSelectionTime > Date.now() - 50 && (n.inputState.lastSelectionOrigin == "select" && (o = !0), l = n.inputState.lastSelectionOrigin), n.dispatch({
             selection: i,
             scrollIntoView: o,
             userEvent: l
         }), !0
     } else return !1
 }
 
-function Wy(n, e, t) {
+function qy(n, e, t) {
     let i, r = n.state,
         s = r.selection.main;
     if (e.from >= s.from && e.to <= s.to && e.to - e.from >= (s.to - s.from) / 3 && (!t || t.main.empty && t.main.from == e.from + e.insert.length) && n.inputState.composing < 0) {
         let l = s.from < e.from ? r.sliceDoc(s.from, e.from) : "",
             h = s.to > e.to ? r.sliceDoc(e.to, s.to) : "";
         i = r.replaceSelection(n.state.toText(l + e.insert.sliceString(0, void 0, n.state.lineBreak) + h))
     } else {
         let l = r.changes(e),
             h = t && t.main.to <= l.newLength ? t.main : void 0;
         if (r.selection.ranges.length > 1 && n.inputState.composing >= 0 && e.to <= s.to && e.to >= s.to - 10) {
             let f = n.state.sliceDoc(e.from, e.to),
-                u, g = t && Wd(n, t.main.head);
-            if (g) {
+                u, m = t && Wd(n, t.main.head);
+            if (m) {
                 let v = e.insert.length - (e.to - e.from);
                 u = {
-                    from: g.from,
-                    to: g.to - v
+                    from: m.from,
+                    to: m.to - v
                 }
             } else u = n.state.doc.lineAt(s.head);
             let y = s.to - e.to,
                 k = s.to - s.from;
             i = r.changeByRange(v => {
                 if (v.from == s.from && v.to == s.to) return {
                     changes: l,
                     range: h || v.map(l)
                 };
-                let C = v.to - y,
-                    O = C - f.length;
-                if (v.to - v.from != k || n.state.sliceDoc(O, C) != f || v.to >= u.from && v.from <= u.to) return {
+                let A = v.to - y,
+                    O = A - f.length;
+                if (v.to - v.from != k || n.state.sliceDoc(O, A) != f || v.to >= u.from && v.from <= u.to) return {
                     range: v
                 };
                 let D = r.changes({
                         from: O,
-                        to: C,
+                        to: A,
                         insert: e.insert
                     }),
                     F = v.to - s.to;
                 return {
                     changes: D,
                     range: h ? H.range(Math.max(0, h.anchor + F), Math.max(0, h.head + F)) : v.map(D)
                 }
@@ -9961,15 +9961,15 @@
     let o = "input.type";
     return (n.composing || n.inputState.compositionPendingChange && n.inputState.compositionEndedAt > Date.now() - 50) && (n.inputState.compositionPendingChange = !1, o += ".compose", n.inputState.compositionFirstChange && (o += ".start", n.inputState.compositionFirstChange = !1)), r.update(i, {
         userEvent: o,
         scrollIntoView: !0
     })
 }
 
-function qy(n, e, t, i) {
+function jy(n, e, t, i) {
     let r = Math.min(n.length, e.length),
         s = 0;
     for (; s < r && n.charCodeAt(s) == e.charCodeAt(s);) s++;
     if (s == r && n.length == e.length) return null;
     let o = n.length,
         l = e.length;
     for (; o > 0 && l > 0 && n.charCodeAt(o - 1) == e.charCodeAt(l - 1);) o--, l--;
@@ -9987,43 +9987,43 @@
     return {
         from: s,
         toA: o,
         toB: l
     }
 }
 
-function jy(n) {
+function Vy(n) {
     let e = [];
     if (n.root.activeElement != n.contentDOM) return e;
     let {
         anchorNode: t,
         anchorOffset: i,
         focusNode: r,
         focusOffset: s
     } = n.observer.selectionRange;
     return t && (e.push(new Cf(t, i)), (r != t || s != i) && e.push(new Cf(r, s))), e
 }
 
-function Vy(n, e) {
+function Uy(n, e) {
     if (n.length == 0) return null;
     let t = n[0].pos,
         i = n.length == 2 ? n[1].pos : t;
     return t > -1 && i > -1 ? H.single(t + e, i + e) : null
 }
-const Uy = {
+const Qy = {
         childList: !0,
         characterData: !0,
         subtree: !0,
         attributes: !0,
         characterDataOldValue: !0
     },
     oa = ee.ie && ee.ie_version <= 11;
-class Qy {
+class Gy {
     constructor(e) {
-        this.view = e, this.active = !1, this.selectionRange = new D0, this.selectionChanged = !1, this.delayedFlush = -1, this.resizeTimeout = -1, this.queue = [], this.delayedAndroidKey = null, this.flushingAndroidKey = -1, this.lastChange = 0, this.scrollTargets = [], this.intersection = null, this.resizeScroll = null, this.intersecting = !1, this.gapIntersection = null, this.gaps = [], this.parentCheck = -1, this.dom = e.contentDOM, this.observer = new MutationObserver(t => {
+        this.view = e, this.active = !1, this.selectionRange = new R0, this.selectionChanged = !1, this.delayedFlush = -1, this.resizeTimeout = -1, this.queue = [], this.delayedAndroidKey = null, this.flushingAndroidKey = -1, this.lastChange = 0, this.scrollTargets = [], this.intersection = null, this.resizeScroll = null, this.intersecting = !1, this.gapIntersection = null, this.gaps = [], this.parentCheck = -1, this.dom = e.contentDOM, this.observer = new MutationObserver(t => {
             for (let i of t) this.queue.push(i);
             (ee.ie && ee.ie_version <= 11 || ee.ios && e.composing) && t.some(i => i.type == "childList" && i.removedNodes.length || i.type == "characterData" && i.oldValue.length > i.target.nodeValue.length) ? this.flushSoon() : this.flush()
         }), oa && (this.onCharData = t => {
             this.queue.push({
                 target: t.target,
                 type: "characterData",
                 oldValue: t.prevValue
@@ -10074,18 +10074,18 @@
             t || (this.selectionChanged = !1);
             return
         }(ee.ie && ee.ie_version <= 11 || ee.android && ee.chrome) && !i.state.selection.main.empty && r.focusNode && Wo(r.focusNode, r.focusOffset, r.anchorNode, r.anchorOffset) ? this.flushSoon() : this.flush(!1)
     }
     readSelectionRange() {
         let {
             view: e
-        } = this, t = ee.safari && e.root.nodeType == 11 && T0(this.dom.ownerDocument) == this.dom && Gy(this.view) || $o(e.root);
+        } = this, t = ee.safari && e.root.nodeType == 11 && O0(this.dom.ownerDocument) == this.dom && Ky(this.view) || $o(e.root);
         if (!t || this.selectionRange.eq(t)) return !1;
         let i = Do(this.dom, t);
-        return i && !this.selectionChanged && e.inputState.lastFocusTime > Date.now() - 200 && e.inputState.lastTouchTime < Date.now() - 300 && L0(this.dom, t) ? (this.view.inputState.lastFocusTime = 0, e.docView.updateSelection(), !1) : (this.selectionRange.setRange(t), i && (this.selectionChanged = !0), !0)
+        return i && !this.selectionChanged && e.inputState.lastFocusTime > Date.now() - 200 && e.inputState.lastTouchTime < Date.now() - 300 && P0(this.dom, t) ? (this.view.inputState.lastFocusTime = 0, e.docView.updateSelection(), !1) : (this.selectionRange.setRange(t), i && (this.selectionChanged = !0), !0)
     }
     setSelectionRange(e, t) {
         this.selectionRange.set(e.node, e.offset, t.node, t.offset), this.selectionChanged = !1
     }
     clearSelectionRange() {
         this.selectionRange.set(null, 0, null, 0)
     }
@@ -10107,15 +10107,15 @@
         try {
             return this.stop(), e()
         } finally {
             this.start(), this.clear()
         }
     }
     start() {
-        this.active || (this.observer.observe(this.dom, Uy), oa && this.dom.addEventListener("DOMCharacterDataModified", this.onCharData), this.active = !0)
+        this.active || (this.observer.observe(this.dom, Qy), oa && this.dom.addEventListener("DOMCharacterDataModified", this.onCharData), this.active = !0)
     }
     stop() {
         this.active && (this.active = !1, this.observer.disconnect(), oa && this.dom.removeEventListener("DOMCharacterDataModified", this.onCharData))
     }
     clear() {
         this.processRecords(), this.queue.length = 0, this.selectionChanged = !1
     }
@@ -10171,15 +10171,15 @@
         let {
             from: e,
             to: t,
             typeOver: i
         } = this.processRecords(), r = this.selectionChanged && Do(this.dom, this.selectionRange);
         if (e < 0 && !r) return null;
         e > -1 && (this.lastChange = Date.now()), this.view.inputState.lastFocusTime = 0, this.selectionChanged = !1;
-        let s = new $y(this.view, e, t, i);
+        let s = new Wy(this.view, e, t, i);
         return this.view.docView.domChanged = {
             newSel: s.newSel ? s.newSel.main : null
         }, s
     }
     flush(e = !0) {
         if (this.delayedFlush >= 0 || this.delayedAndroidKey) return !1;
         e && this.readSelectionRange();
@@ -10229,15 +10229,15 @@
         if (i && i.parent == n) return i;
         let r = e.parentNode;
         e = r != n.dom ? r : t > 0 ? e.nextSibling : e.previousSibling
     }
     return null
 }
 
-function Gy(n) {
+function Ky(n) {
     let e = null;
 
     function t(h) {
         h.preventDefault(), h.stopImmediatePropagation(), e = h.getTargetRanges()[0]
     }
     if (n.contentDOM.addEventListener("beforeinput", t, !0), n.dom.ownerDocument.execCommand("indent"), n.contentDOM.removeEventListener("beforeinput", t, !0), !e) return null;
     let i = e.startContainer,
@@ -10278,17 +10278,17 @@
         return this.dom.ownerDocument.defaultView || window
     }
     constructor(e = {}) {
         this.plugins = [], this.pluginMap = new Map, this.editorAttrs = {}, this.contentAttrs = {}, this.bidiCache = [], this.destroyed = !1, this.updateState = 2, this.measureScheduled = -1, this.measureRequests = [], this.contentDOM = document.createElement("div"), this.scrollDOM = document.createElement("div"), this.scrollDOM.tabIndex = -1, this.scrollDOM.className = "cm-scroller", this.scrollDOM.appendChild(this.contentDOM), this.announceDOM = document.createElement("div"), this.announceDOM.className = "cm-announced", this.announceDOM.setAttribute("aria-live", "polite"), this.dom = document.createElement("div"), this.dom.appendChild(this.announceDOM), this.dom.appendChild(this.scrollDOM), e.parent && e.parent.appendChild(this.dom);
         let {
             dispatch: t
         } = e;
-        this.dispatchTransactions = e.dispatchTransactions || t && (i => i.forEach(r => t(r, this))) || (i => this.update(i)), this.dispatch = this.dispatch.bind(this), this._root = e.root || R0(e.parent) || document, this.viewState = new wf(e.state || Ee.create(e)), e.scrollTo && e.scrollTo.is(io) && (this.viewState.scrollTarget = e.scrollTo.value.clip(this.viewState.state)), this.plugins = this.state.facet(Zr).map(i => new ia(i));
+        this.dispatchTransactions = e.dispatchTransactions || t && (i => i.forEach(r => t(r, this))) || (i => this.update(i)), this.dispatch = this.dispatch.bind(this), this._root = e.root || L0(e.parent) || document, this.viewState = new wf(e.state || Ee.create(e)), e.scrollTo && e.scrollTo.is(io) && (this.viewState.scrollTarget = e.scrollTo.value.clip(this.viewState.state)), this.plugins = this.state.facet(Zr).map(i => new ia(i));
         for (let i of this.plugins) i.update(this);
-        this.observer = new Qy(this), this.inputState = new hy(this), this.inputState.ensureHandlers(this.plugins), this.docView = new nf(this), this.mountStyles(), this.updateAttrs(), this.updateState = 0, this.requestMeasure()
+        this.observer = new Gy(this), this.inputState = new cy(this), this.inputState.ensureHandlers(this.plugins), this.docView = new nf(this), this.mountStyles(), this.updateAttrs(), this.updateState = 0, this.requestMeasure()
     }
     dispatch(...e) {
         let t = e.length == 1 && e[0] instanceof nt ? e : e.length == 1 && Array.isArray(e[0]) ? e[0] : [this.state.update(...e)];
         this.dispatchTransactions(t, this)
     }
     update(e) {
         if (this.updateState != 0) throw new Error("Calls to EditorView.update are not allowed while an update is in progress");
@@ -10307,31 +10307,31 @@
             l = 0,
             h = null;
         e.some(y => y.annotation(Yd)) ? (this.inputState.notifiedFocused = o, l = 1) : o != this.inputState.notifiedFocused && (this.inputState.notifiedFocused = o, h = Jd(s, o), h || (l = 1));
         let f = this.observer.delayedAndroidKey,
             u = null;
         if (f ? (this.observer.clearDelayedAndroidKey(), u = this.observer.readChange(), (u && !this.state.doc.eq(s.doc) || !this.state.selection.eq(s.selection)) && (u = null)) : this.observer.clear(), s.facet(Ee.phrases) != this.state.facet(Ee.phrases)) return this.setState(s);
         r = qo.create(this, s, e), r.flags |= l;
-        let g = this.viewState.scrollTarget;
+        let m = this.viewState.scrollTarget;
         try {
             this.updateState = 2;
             for (let y of e) {
-                if (g && (g = g.map(y.changes)), y.scrollIntoView) {
+                if (m && (m = m.map(y.changes)), y.scrollIntoView) {
                     let {
                         main: k
                     } = y.state.selection;
-                    g = new yr(k.empty ? k : H.cursor(k.head, k.head > k.anchor ? -1 : 1))
+                    m = new yr(k.empty ? k : H.cursor(k.head, k.head > k.anchor ? -1 : 1))
                 }
-                for (let k of y.effects) k.is(io) && (g = k.value.clip(this.state))
+                for (let k of y.effects) k.is(io) && (m = k.value.clip(this.state))
             }
-            this.viewState.update(r, g), this.bidiCache = jo.update(this.bidiCache, r.changes), r.empty || (this.updatePlugins(r), this.inputState.update(r)), t = this.docView.update(r), this.state.facet(es) != this.styleModules && this.mountStyles(), i = this.updateAttrs(), this.showAnnouncements(e), this.docView.updateSelection(t, e.some(y => y.isUserEvent("select.pointer")))
+            this.viewState.update(r, m), this.bidiCache = jo.update(this.bidiCache, r.changes), r.empty || (this.updatePlugins(r), this.inputState.update(r)), t = this.docView.update(r), this.state.facet(es) != this.styleModules && this.mountStyles(), i = this.updateAttrs(), this.showAnnouncements(e), this.docView.updateSelection(t, e.some(y => y.isUserEvent("select.pointer")))
         } finally {
             this.updateState = 0
         }
-        if (r.startState.facet(ao) != r.state.facet(ao) && (this.viewState.mustMeasureContent = !0), (t || i || g || this.viewState.mustEnforceCursorAssoc || this.viewState.mustMeasureContent) && this.requestMeasure(), !r.empty)
+        if (r.startState.facet(ao) != r.state.facet(ao) && (this.viewState.mustMeasureContent = !0), (t || i || m || this.viewState.mustEnforceCursorAssoc || this.viewState.mustMeasureContent) && this.requestMeasure(), !r.empty)
             for (let y of this.state.facet(Ya)) try {
                 y(r)
             } catch (k) {
                 ni(this.state, k, "update listener")
             }(h || u) && Promise.resolve().then(() => {
                 h && this.state == h.startState && this.dispatch(h), u && !rp(this, u) && f.force && mr(this.contentDOM, f.key, f.keyCode)
             })
@@ -10408,25 +10408,25 @@
                 let u = f.map(k => {
                         try {
                             return k.read(this)
                         } catch (v) {
                             return ni(this.state, v), Tf
                         }
                     }),
-                    g = qo.create(this, this.state, []),
+                    m = qo.create(this, this.state, []),
                     y = !1;
-                g.flags |= h, t ? t.flags |= h : t = g, this.updateState = 2, g.empty || (this.updatePlugins(g), this.inputState.update(g), this.updateAttrs(), y = this.docView.update(g));
+                m.flags |= h, t ? t.flags |= h : t = m, this.updateState = 2, m.empty || (this.updatePlugins(m), this.inputState.update(m), this.updateAttrs(), y = this.docView.update(m));
                 for (let k = 0; k < f.length; k++)
                     if (u[k] != Tf) try {
                         let v = f[k];
                         v.write && v.write(u[k], this)
                     } catch (v) {
                         ni(this.state, v)
                     }
-                if (y && this.docView.updateSelection(!0), !g.viewportChanged && this.measureRequests.length == 0) {
+                if (y && this.docView.updateSelection(!0), !m.viewportChanged && this.measureRequests.length == 0) {
                     if (this.viewState.editorHeight)
                         if (this.viewState.scrollTarget) {
                             this.docView.scrollIntoView(this.viewState.scrollTarget), this.viewState.scrollTarget = null, o = -1;
                             continue
                         } else {
                             let v = (s < 0 ? this.viewState.heightMap.height : this.viewState.lineBlockAt(s).top) - o;
                             if (v > 1 || v < -1) {
@@ -10477,15 +10477,15 @@
                     let s = this.announceDOM.appendChild(document.createElement("div"));
                     s.textContent = r.value
                 }
     }
     mountStyles() {
         this.styleModules = this.state.facet(es);
         let e = this.state.facet(te.cspNonce);
-        kn.mount(this.root, this.styleModules.concat(Hy).reverse(), e ? {
+        kn.mount(this.root, this.styleModules.concat(Fy).reverse(), e ? {
             nonce: e
         } : void 0)
     }
     readMeasured() {
         if (this.updateState == 2) throw new Error("Reading the editor layout isn't allowed during an update");
         this.updateState == 0 && this.measureScheduled > -1 && this.measure(!1)
     }
@@ -10536,21 +10536,21 @@
     get contentHeight() {
         return this.viewState.contentHeight
     }
     moveByChar(e, t, i) {
         return ra(this, e, hf(this, e, t, i))
     }
     moveByGroup(e, t) {
-        return ra(this, e, hf(this, e, t, i => ly(this, e.head, i)))
+        return ra(this, e, hf(this, e, t, i => ay(this, e.head, i)))
     }
     moveToLineBoundary(e, t, i = !0) {
-        return oy(this, e, t, i)
+        return ly(this, e, t, i)
     }
     moveVertically(e, t, i) {
-        return ra(this, e, ay(this, e, t, i))
+        return ra(this, e, hy(this, e, t, i))
     }
     domAtPos(e) {
         return this.docView.domAtPos(e)
     }
     posAtDOM(e, t = 0) {
         return this.docView.posFromDOM(e, t)
     }
@@ -10581,21 +10581,21 @@
     textDirectionAt(e) {
         return !this.state.facet(Rd) || e < this.viewport.from || e > this.viewport.to ? this.textDirection : (this.readMeasured(), this.docView.textDirectionAt(e))
     }
     get lineWrapping() {
         return this.viewState.heightOracle.lineWrapping
     }
     bidiSpans(e) {
-        if (e.length > Ky) return zd(e.length);
+        if (e.length > Xy) return zd(e.length);
         let t = this.textDirectionAt(e.from),
             i;
         for (let s of this.bidiCache)
             if (s.from == e.from && s.dir == t && (s.fresh || Fd(s.isolates, i = tf(this, e.from, e.to)))) return s.order;
         i || (i = tf(this, e.from, e.to));
-        let r = U0(e.text, t, i);
+        let r = Q0(e.text, t, i);
         return this.bidiCache.push(new jo(e.from, e.to, t, i, !0, r)), r
     }
     get hasFocus() {
         var e;
         return (this.dom.ownerDocument.hasFocus() || ee.safari && ((e = this.inputState) === null || e === void 0 ? void 0 : e.lastContextMenu) > Date.now() - 3e4) && this.root.activeElement == this.contentDOM
     }
     focus() {
@@ -10665,15 +10665,15 @@
 });
 te.contentAttributes = Hh;
 te.editorAttributes = Pd;
 te.lineWrapping = te.contentAttributes.of({
     class: "cm-lineWrapping"
 });
 te.announce = me.define();
-const Ky = 4096,
+const Xy = 4096,
     Tf = {};
 class jo {
     constructor(e, t, i, r, s, o) {
         this.from = e, this.to = t, this.dir = i, this.isolates = r, this.fresh = s, this.order = o
     }
     static update(e, t) {
         if (t.empty && !e.some(s => s.fresh)) return e;
@@ -10691,17 +10691,17 @@
     for (let i = n.state.facet(e), r = i.length - 1; r >= 0; r--) {
         let s = i[r],
             o = typeof s == "function" ? s(n) : s;
         o && Ga(o, t)
     }
     return t
 }
-const Xy = ee.mac ? "mac" : ee.windows ? "win" : ee.linux ? "linux" : "key";
+const Yy = ee.mac ? "mac" : ee.windows ? "win" : ee.linux ? "linux" : "key";
 
-function Yy(n, e) {
+function Jy(n, e) {
     const t = n.split(/-(?!$)/);
     let i = t[t.length - 1];
     i == "Space" && (i = " ");
     let r, s, o, l;
     for (let h = 0; h < t.length - 1; ++h) {
         const f = t[h];
         if (/^(cmd|meta|m)$/i.test(f)) l = !0;
@@ -10713,114 +10713,114 @@
     }
     return r && (i = "Alt-" + i), s && (i = "Ctrl-" + i), l && (i = "Meta-" + i), o && (i = "Shift-" + i), i
 }
 
 function ho(n, e, t) {
     return e.altKey && (n = "Alt-" + n), e.ctrlKey && (n = "Ctrl-" + n), e.metaKey && (n = "Meta-" + n), t !== !1 && e.shiftKey && (n = "Shift-" + n), n
 }
-const Jy = Kn.default(te.domEventHandlers({
+const Zy = Kn.default(te.domEventHandlers({
         keydown(n, e) {
             return op(sp(e.state), n, e, "editor")
         }
     })),
     xl = Z.define({
-        enables: Jy
+        enables: Zy
     }),
     Mf = new WeakMap;
 
 function sp(n) {
     let e = n.facet(xl),
         t = Mf.get(e);
-    return t || Mf.set(e, t = tb(e.reduce((i, r) => i.concat(r), []))), t
+    return t || Mf.set(e, t = ib(e.reduce((i, r) => i.concat(r), []))), t
 }
 
-function Zy(n, e, t) {
+function eb(n, e, t) {
     return op(sp(n.state), e, n, t)
 }
 let fn = null;
-const eb = 4e3;
+const tb = 4e3;
 
-function tb(n, e = Xy) {
+function ib(n, e = Yy) {
     let t = Object.create(null),
         i = Object.create(null),
         r = (o, l) => {
             let h = i[o];
             if (h == null) i[o] = l;
             else if (h != l) throw new Error("Key binding " + o + " is used both as a regular binding and as a multi-stroke prefix")
         },
         s = (o, l, h, f, u) => {
-            var g, y;
+            var m, y;
             let k = t[o] || (t[o] = Object.create(null)),
-                v = l.split(/ (?!$)/).map(D => Yy(D, e));
+                v = l.split(/ (?!$)/).map(D => Jy(D, e));
             for (let D = 1; D < v.length; D++) {
                 let F = v.slice(0, D).join(" ");
                 r(F, !0), k[F] || (k[F] = {
                     preventDefault: !0,
                     stopPropagation: !1,
                     run: [$ => {
                         let j = fn = {
                             view: $,
                             prefix: F,
                             scope: o
                         };
                         return setTimeout(() => {
                             fn == j && (fn = null)
-                        }, eb), !0
+                        }, tb), !0
                     }]
                 })
             }
-            let C = v.join(" ");
-            r(C, !1);
-            let O = k[C] || (k[C] = {
+            let A = v.join(" ");
+            r(A, !1);
+            let O = k[A] || (k[A] = {
                 preventDefault: !1,
                 stopPropagation: !1,
-                run: ((y = (g = k._any) === null || g === void 0 ? void 0 : g.run) === null || y === void 0 ? void 0 : y.slice()) || []
+                run: ((y = (m = k._any) === null || m === void 0 ? void 0 : m.run) === null || y === void 0 ? void 0 : y.slice()) || []
             });
             h && O.run.push(h), f && (O.preventDefault = !0), u && (O.stopPropagation = !0)
         };
     for (let o of n) {
         let l = o.scope ? o.scope.split(" ") : ["editor"];
         if (o.any)
             for (let f of l) {
                 let u = t[f] || (t[f] = Object.create(null));
                 u._any || (u._any = {
                     preventDefault: !1,
                     stopPropagation: !1,
                     run: []
                 });
-                for (let g in u) u[g].run.push(o.any)
+                for (let m in u) u[m].run.push(o.any)
             }
         let h = o[e] || o.key;
         if (h)
             for (let f of l) s(f, h, o.run, o.preventDefault, o.stopPropagation), o.shift && s(f, "Shift-" + h, o.shift, o.preventDefault, o.stopPropagation)
     }
     return t
 }
 
 function op(n, e, t, i) {
-    let r = A0(e),
+    let r = T0(e),
         s = pt(r, 0),
         o = ti(s) == r.length && r != " ",
         l = "",
         h = !1,
         f = !1,
         u = !1;
     fn && fn.view == t && fn.scope == i && (l = fn.prefix + " ", Ud.indexOf(e.keyCode) < 0 && (f = !0, fn = null));
-    let g = new Set,
+    let m = new Set,
         y = O => {
             if (O) {
                 for (let D of O.run)
-                    if (!g.has(D) && (g.add(D), D(t, e))) return O.stopPropagation && (u = !0), !0;
+                    if (!m.has(D) && (m.add(D), D(t, e))) return O.stopPropagation && (u = !0), !0;
                 O.preventDefault && (O.stopPropagation && (u = !0), f = !0)
             }
             return !1
         },
         k = n[i],
-        v, C;
-    return k && (y(k[l + ho(r, e, !o)]) ? h = !0 : o && (e.altKey || e.metaKey || e.ctrlKey) && !(ee.windows && e.ctrlKey && e.altKey) && (v = wn[e.keyCode]) && v != r ? (y(k[l + ho(v, e, !0)]) || e.shiftKey && (C = us[e.keyCode]) != r && C != v && y(k[l + ho(C, e, !1)])) && (h = !0) : o && e.shiftKey && y(k[l + ho(r, e, !0)]) && (h = !0), !h && y(k._any) && (h = !0)), f && (h = !0), h && u && e.stopPropagation(), h
+        v, A;
+    return k && (y(k[l + ho(r, e, !o)]) ? h = !0 : o && (e.altKey || e.metaKey || e.ctrlKey) && !(ee.windows && e.ctrlKey && e.altKey) && (v = wn[e.keyCode]) && v != r ? (y(k[l + ho(v, e, !0)]) || e.shiftKey && (A = us[e.keyCode]) != r && A != v && y(k[l + ho(A, e, !1)])) && (h = !0) : o && e.shiftKey && y(k[l + ho(r, e, !0)]) && (h = !0), !h && y(k._any) && (h = !0)), f && (h = !0), h && u && e.stopPropagation(), h
 }
 class Ds {
     constructor(e, t, i, r, s) {
         this.className = e, this.left = t, this.top = i, this.width = r, this.height = s
     }
     draw() {
         let e = document.createElement("div");
@@ -10837,15 +10837,15 @@
     }
     static forRange(e, t, i) {
         if (i.empty) {
             let r = e.coordsAtPos(i.head, i.assoc || 1);
             if (!r) return [];
             let s = lp(e);
             return [new Ds(t, r.left - s.left, r.top - s.top, null, r.bottom - r.top)]
-        } else return ib(e, t, i)
+        } else return nb(e, t, i)
     }
 }
 
 function lp(n) {
     let e = n.scrollDOM.getBoundingClientRect();
     return {
         left: (n.textDirection == Ue.LTR ? e.left : e.right - n.scrollDOM.clientWidth * n.scaleX) - n.scrollDOM.scrollLeft * n.scaleX,
@@ -10858,36 +10858,36 @@
     return {
         from: Math.max(t.from, n.moveToLineBoundary(i, !1, !0).from),
         to: Math.min(t.to, n.moveToLineBoundary(i, !0, !0).from),
         type: Dt.Text
     }
 }
 
-function ib(n, e, t) {
+function nb(n, e, t) {
     if (t.to <= n.viewport.from || t.from >= n.viewport.to) return [];
     let i = Math.max(t.from, n.viewport.from),
         r = Math.min(t.to, n.viewport.to),
         s = n.textDirection == Ue.LTR,
         o = n.contentDOM,
         l = o.getBoundingClientRect(),
         h = lp(n),
         f = o.querySelector(".cm-line"),
         u = f && window.getComputedStyle(f),
-        g = l.left + (u ? parseInt(u.paddingLeft) + Math.min(0, parseInt(u.textIndent)) : 0),
+        m = l.left + (u ? parseInt(u.paddingLeft) + Math.min(0, parseInt(u.textIndent)) : 0),
         y = l.right - (u ? parseInt(u.paddingRight) : 0),
         k = ih(n, i),
         v = ih(n, r),
-        C = k.type == Dt.Text ? k : null,
+        A = k.type == Dt.Text ? k : null,
         O = v.type == Dt.Text ? v : null;
-    if (C && (n.lineWrapping || k.widgetLineBreaks) && (C = Ef(n, i, C)), O && (n.lineWrapping || v.widgetLineBreaks) && (O = Ef(n, r, O)), C && O && C.from == O.from) return F($(t.from, t.to, C));
+    if (A && (n.lineWrapping || k.widgetLineBreaks) && (A = Ef(n, i, A)), O && (n.lineWrapping || v.widgetLineBreaks) && (O = Ef(n, r, O)), A && O && A.from == O.from) return F($(t.from, t.to, A));
     {
-        let z = C ? $(t.from, null, C) : j(k, !1),
+        let z = A ? $(t.from, null, A) : j(k, !1),
             G = O ? $(null, t.to, O) : j(v, !0),
             p = [];
-        return (C || k).to < (O || v).from - (C && O ? 1 : 0) || k.widgetLineBreaks > 1 && z.bottom + n.defaultLineHeight / 2 < G.top ? p.push(D(g, z.bottom, y, G.top)) : z.bottom < G.top && n.elementAtHeight((z.bottom + G.top) / 2).type == Dt.Text && (z.bottom = G.top = (z.bottom + G.top) / 2), F(z).concat(p).concat(F(G))
+        return (A || k).to < (O || v).from - (A && O ? 1 : 0) || k.widgetLineBreaks > 1 && z.bottom + n.defaultLineHeight / 2 < G.top ? p.push(D(m, z.bottom, y, G.top)) : z.bottom < G.top && n.elementAtHeight((z.bottom + G.top) / 2).type == Dt.Text && (z.bottom = G.top = (z.bottom + G.top) / 2), F(z).concat(p).concat(F(G))
     }
 
     function D(z, G, p, he) {
         return new Ds(e, z - h.left, G - h.top - .01, p - z, he - G + .01)
     }
 
     function F({
@@ -10904,15 +10904,15 @@
         let he = 1e9,
             J = -1e9,
             ae = [];
 
         function pe(ye, Be, st, _e, Ye) {
             let be = n.coordsAtPos(ye, ye == p.to ? -2 : 2),
                 We = n.coordsAtPos(st, st == p.from ? 2 : -2);
-            !be || !We || (he = Math.min(be.top, We.top, he), J = Math.max(be.bottom, We.bottom, J), Ye == Ue.LTR ? ae.push(s && Be ? g : be.left, s && _e ? y : We.right) : ae.push(!s && _e ? g : We.left, !s && Be ? y : be.right))
+            !be || !We || (he = Math.min(be.top, We.top, he), J = Math.max(be.bottom, We.bottom, J), Ye == Ue.LTR ? ae.push(s && Be ? m : be.left, s && _e ? y : We.right) : ae.push(!s && _e ? m : We.left, !s && Be ? y : be.right))
         }
         let fe = z != null ? z : p.from,
             ie = G != null ? G : p.to;
         for (let ye of n.visibleRanges)
             if (ye.to > fe && ye.from < ie)
                 for (let Be = Math.max(ye.from, fe), st = Math.min(ye.to, ie);;) {
                     let _e = n.state.doc.lineAt(Be);
@@ -10937,18 +10937,18 @@
             top: p,
             bottom: p,
             horizontal: []
         }
     }
 }
 
-function nb(n, e) {
+function rb(n, e) {
     return n.constructor == e.constructor && n.eq(e)
 }
-class rb {
+class sb {
     constructor(e, t) {
         this.view = e, this.layer = t, this.drawn = [], this.scaleX = 1, this.scaleY = 1, this.measureReq = {
             read: this.measure.bind(this),
             write: this.draw.bind(this)
         }, this.dom = e.scrollDOM.appendChild(document.createElement("div")), this.dom.classList.add("cm-layer"), t.above && this.dom.classList.add("cm-layer-above"), t.class && this.dom.classList.add(t.class), this.scale(), this.dom.setAttribute("aria-hidden", "true"), this.setOrder(e.state), e.requestMeasure(this.measureReq), t.mount && t.mount(this.dom, e)
     }
     update(e) {
@@ -10967,15 +10967,15 @@
         let {
             scaleX: e,
             scaleY: t
         } = this.view;
         (e != this.scaleX || t != this.scaleY) && (this.scaleX = e, this.scaleY = t, this.dom.style.transform = `scale(${1/e}, ${1/t})`)
     }
     draw(e) {
-        if (e.length != this.drawn.length || e.some((t, i) => !nb(t, this.drawn[i]))) {
+        if (e.length != this.drawn.length || e.some((t, i) => !rb(t, this.drawn[i]))) {
             let t = this.dom.firstChild,
                 i = 0;
             for (let r of e) r.update && t && r.constructor && this.drawn[i].constructor && r.update(t, this.drawn[i]) ? (t = t.nextSibling, i++) : this.dom.insertBefore(r.draw(), t);
             for (; t;) {
                 let r = t.nextSibling;
                 t.remove(), t = r
             }
@@ -10985,37 +10985,37 @@
     destroy() {
         this.layer.destroy && this.layer.destroy(this.dom, this.view), this.dom.remove()
     }
 }
 const Po = Z.define();
 
 function ap(n) {
-    return [rt.define(e => new rb(e, n)), Po.of(n)]
+    return [rt.define(e => new sb(e, n)), Po.of(n)]
 }
 const hp = !ee.ios,
     ys = Z.define({
         combine(n) {
             return Hi(n, {
                 cursorBlinkRate: 1200,
                 drawRangeCursor: !0
             }, {
                 cursorBlinkRate: (e, t) => Math.min(e, t),
                 drawRangeCursor: (e, t) => e || t
             })
         }
     });
 
-function sb(n = {}) {
-    return [ys.of(n), ob, lb, ab, Ld.of(!0)]
+function ob(n = {}) {
+    return [ys.of(n), lb, ab, hb, Ld.of(!0)]
 }
 
 function cp(n) {
     return n.startState.facet(ys) != n.state.facet(ys)
 }
-const ob = ap({
+const lb = ap({
     above: !0,
     markers(n) {
         let {
             state: e
         } = n, t = e.facet(ys), i = [];
         for (let r of e.selection.ranges) {
             let s = r == e.selection.main;
@@ -11037,15 +11037,15 @@
     },
     class: "cm-cursorLayer"
 });
 
 function Df(n, e) {
     e.style.animationDuration = n.facet(ys).cursorBlinkRate + "ms"
 }
-const lb = ap({
+const ab = ap({
         above: !1,
         markers(n) {
             return n.state.selection.ranges.map(e => e.empty ? [] : Ds.forRange(n, "cm-selectionBackground", e)).reduce((e, t) => e.concat(t))
         },
         update(n, e) {
             return n.docChanged || n.selectionSet || n.viewportChanged || cp(n)
         },
@@ -11060,29 +11060,29 @@
                 backgroundColor: "transparent !important"
             }
         }
     };
 hp && (lh[".cm-line"].caretColor = "transparent !important", lh[".cm-content"] = {
     caretColor: "transparent !important"
 });
-const ab = Kn.highest(te.theme(lh)),
+const hb = Kn.highest(te.theme(lh)),
     fp = me.define({
         map(n, e) {
             return n == null ? null : e.mapPos(n)
         }
     }),
     ns = yt.define({
         create() {
             return null
         },
         update(n, e) {
             return n != null && (n = e.changes.mapPos(n)), e.effects.reduce((t, i) => i.is(fp) ? i.value : t, n)
         }
     }),
-    hb = rt.fromClass(class {
+    cb = rt.fromClass(class {
         constructor(n) {
             this.view = n, this.cursor = null, this.measureReq = {
                 read: this.readPos.bind(this),
                 write: this.drawCursor.bind(this)
             }
         }
         update(n) {
@@ -11135,66 +11135,66 @@
             },
             drop() {
                 this.setDropPos(null)
             }
         }
     });
 
-function cb() {
-    return [ns, hb]
+function fb() {
+    return [ns, cb]
 }
 
 function Rf(n, e, t, i, r) {
     e.lastIndex = 0;
     for (let s = n.iterRange(t, i), o = t, l; !s.next().done; o += s.value.length)
         if (!s.lineBreak)
             for (; l = e.exec(s.value);) r(o + l.index, l)
 }
 
-function fb(n, e) {
+function ub(n, e) {
     let t = n.visibleRanges;
     if (t.length == 1 && t[0].from == n.viewport.from && t[0].to == n.viewport.to) return t;
     let i = [];
     for (let {
             from: r,
             to: s
         }
         of t) r = Math.max(n.state.doc.lineAt(r).from, r - e), s = Math.min(n.state.doc.lineAt(s).to, s + e), i.length && i[i.length - 1].to >= r ? i[i.length - 1].to = s : i.push({
         from: r,
         to: s
     });
     return i
 }
-class ub {
+class db {
     constructor(e) {
         const {
             regexp: t,
             decoration: i,
             decorate: r,
             boundary: s,
             maxLength: o = 1e3
         } = e;
         if (!t.global) throw new RangeError("The regular expression given to MatchDecorator should have its 'g' flag set");
         if (this.regexp = t, r) this.addMatch = (l, h, f, u) => r(u, f, f + l[0].length, l, h);
         else if (typeof i == "function") this.addMatch = (l, h, f, u) => {
-            let g = i(l, h, f);
-            g && u(f, f + l[0].length, g)
+            let m = i(l, h, f);
+            m && u(f, f + l[0].length, m)
         };
         else if (i) this.addMatch = (l, h, f, u) => u(f, f + l[0].length, i);
         else throw new RangeError("Either 'decorate' or 'decoration' should be provided to MatchDecorator");
         this.boundary = s, this.maxLength = o
     }
     createDeco(e) {
         let t = new xn,
             i = t.add.bind(t);
         for (let {
                 from: r,
                 to: s
             }
-            of fb(e, this.maxLength)) Rf(e.state.doc, this.regexp, r, s, (o, l) => this.addMatch(l, e, o, i));
+            of ub(e, this.maxLength)) Rf(e.state.doc, this.regexp, r, s, (o, l) => this.addMatch(l, e, o, i));
         return t.finish()
     }
     updateDeco(e, t) {
         let i = 1e9,
             r = -1;
         return e.docChanged && e.changes.iterChanges((s, o, l, h) => {
             h > e.view.viewport.from && l < e.view.viewport.to && (i = Math.min(l, i), r = Math.max(h, r))
@@ -11204,47 +11204,47 @@
         for (let s of e.visibleRanges) {
             let o = Math.max(s.from, i),
                 l = Math.min(s.to, r);
             if (l > o) {
                 let h = e.state.doc.lineAt(o),
                     f = h.to < l ? e.state.doc.lineAt(l) : h,
                     u = Math.max(s.from, h.from),
-                    g = Math.min(s.to, f.to);
+                    m = Math.min(s.to, f.to);
                 if (this.boundary) {
                     for (; o > h.from; o--)
                         if (this.boundary.test(h.text[o - 1 - h.from])) {
                             u = o;
                             break
                         } for (; l < f.to; l++)
                         if (this.boundary.test(f.text[l - f.from])) {
-                            g = l;
+                            m = l;
                             break
                         }
                 }
                 let y = [],
-                    k, v = (C, O, D) => y.push(D.range(C, O));
+                    k, v = (A, O, D) => y.push(D.range(A, O));
                 if (h == f)
                     for (this.regexp.lastIndex = u - h.from;
-                        (k = this.regexp.exec(h.text)) && k.index < g - h.from;) this.addMatch(k, e, k.index + h.from, v);
-                else Rf(e.state.doc, this.regexp, u, g, (C, O) => this.addMatch(O, e, C, v));
+                        (k = this.regexp.exec(h.text)) && k.index < m - h.from;) this.addMatch(k, e, k.index + h.from, v);
+                else Rf(e.state.doc, this.regexp, u, m, (A, O) => this.addMatch(O, e, A, v));
                 t = t.update({
                     filterFrom: u,
-                    filterTo: g,
-                    filter: (C, O) => C < u || O > g,
+                    filterTo: m,
+                    filter: (A, O) => A < u || O > m,
                     add: y
                 })
             }
         }
         return t
     }
 }
 const ah = /x/.unicode != null ? "gu" : "g",
-    db = new RegExp(`[\0-\b
+    pb = new RegExp(`[\0-\b
 --­؜​‎‏\u2028\u2029‭‮⁦⁧⁩\uFEFF￹-￼]`, ah),
-    pb = {
+    gb = {
         0: "null",
         7: "bell",
         8: "backspace",
         10: "newline",
         11: "vertical tab",
         13: "carriage return",
         27: "escape",
@@ -11261,98 +11261,98 @@
         8297: "pop directional isolate",
         8233: "paragraph separator",
         65279: "zero width no-break space",
         65532: "object replacement"
     };
 let la = null;
 
-function gb() {
+function mb() {
     var n;
     if (la == null && typeof document != "undefined" && document.body) {
         let e = document.body.style;
         la = ((n = e.tabSize) !== null && n !== void 0 ? n : e.MozTabSize) != null
     }
     return la || !1
 }
 const No = Z.define({
     combine(n) {
         let e = Hi(n, {
             render: null,
-            specialChars: db,
+            specialChars: pb,
             addSpecialChars: null
         });
-        return (e.replaceTabs = !gb()) && (e.specialChars = new RegExp("	|" + e.specialChars.source, ah)), e.addSpecialChars && (e.specialChars = new RegExp(e.specialChars.source + "|" + e.addSpecialChars.source, ah)), e
+        return (e.replaceTabs = !mb()) && (e.specialChars = new RegExp("	|" + e.specialChars.source, ah)), e.addSpecialChars && (e.specialChars = new RegExp(e.specialChars.source + "|" + e.addSpecialChars.source, ah)), e
     }
 });
 
-function mb(n = {}) {
-    return [No.of(n), yb()]
+function yb(n = {}) {
+    return [No.of(n), bb()]
 }
 let Lf = null;
 
-function yb() {
+function bb() {
     return Lf || (Lf = rt.fromClass(class {
         constructor(n) {
             this.view = n, this.decorations = de.none, this.decorationCache = Object.create(null), this.decorator = this.makeDecorator(n.state.facet(No)), this.decorations = this.decorator.createDeco(n)
         }
         makeDecorator(n) {
-            return new ub({
+            return new db({
                 regexp: n.specialChars,
                 decoration: (e, t, i) => {
                     let {
                         doc: r
                     } = t.state, s = pt(e[0], 0);
                     if (s == 9) {
                         let o = r.lineAt(i),
                             l = t.state.tabSize,
                             h = Os(o.text, l, i - o.from);
                         return de.replace({
-                            widget: new wb((l - h % l) * this.view.defaultCharacterWidth / this.view.scaleX)
+                            widget: new vb((l - h % l) * this.view.defaultCharacterWidth / this.view.scaleX)
                         })
                     }
                     return this.decorationCache[s] || (this.decorationCache[s] = de.replace({
-                        widget: new kb(n, s)
+                        widget: new wb(n, s)
                     }))
                 },
                 boundary: n.replaceTabs ? void 0 : /[^]/
             })
         }
         update(n) {
             let e = n.state.facet(No);
             n.startState.facet(No) != e ? (this.decorator = this.makeDecorator(e), this.decorations = this.decorator.createDeco(n.view)) : this.decorations = this.decorator.updateDeco(n, this.decorations)
         }
     }, {
         decorations: n => n.decorations
     }))
 }
-const bb = "•";
+const xb = "•";
 
-function xb(n) {
-    return n >= 32 ? bb : n == 10 ? "␤" : String.fromCharCode(9216 + n)
+function kb(n) {
+    return n >= 32 ? xb : n == 10 ? "␤" : String.fromCharCode(9216 + n)
 }
-class kb extends An {
+class wb extends An {
     constructor(e, t) {
         super(), this.options = e, this.code = t
     }
     eq(e) {
         return e.code == this.code
     }
     toDOM(e) {
-        let t = xb(this.code),
-            i = e.state.phrase("Control character") + " " + (pb[this.code] || "0x" + this.code.toString(16)),
+        let t = kb(this.code),
+            i = e.state.phrase("Control character") + " " + (gb[this.code] || "0x" + this.code.toString(16)),
             r = this.options.render && this.options.render(this.code, i, t);
         if (r) return r;
         let s = document.createElement("span");
         return s.textContent = t, s.title = i, s.setAttribute("aria-label", i), s.className = "cm-specialChar", s
     }
     ignoreEvent() {
         return !1
     }
 }
-class wb extends An {
+class vb extends An {
     constructor(e) {
         super(), this.width = e
     }
     eq(e) {
         return e.width == this.width
     }
     toDOM() {
@@ -11360,33 +11360,33 @@
         return e.textContent = "	", e.className = "cm-tab", e.style.width = this.width + "px", e
     }
     ignoreEvent() {
         return !1
     }
 }
 
-function vb() {
-    return Cb
+function Sb() {
+    return Ab
 }
-const Sb = de.line({
+const Cb = de.line({
         class: "cm-activeLine"
     }),
-    Cb = rt.fromClass(class {
+    Ab = rt.fromClass(class {
         constructor(n) {
             this.decorations = this.getDeco(n)
         }
         update(n) {
             (n.docChanged || n.selectionSet) && (this.decorations = this.getDeco(n.view))
         }
         getDeco(n) {
             let e = -1,
                 t = [];
             for (let i of n.state.selection.ranges) {
                 let r = n.lineBlockAt(i.head);
-                r.from > e && (t.push(Sb.range(r.from)), e = r.from)
+                r.from > e && (t.push(Cb.range(r.from)), e = r.from)
             }
             return de.set(t)
         }
     }, {
         decorations: n => n.decorations
     }),
     jr = "-10000px";
@@ -11404,31 +11404,31 @@
         }
         let o = [],
             l = t ? [] : null;
         for (let h = 0; h < s.length; h++) {
             let f = s[h],
                 u = -1;
             if (f) {
-                for (let g = 0; g < this.tooltips.length; g++) {
-                    let y = this.tooltips[g];
-                    y && y.create == f.create && (u = g)
+                for (let m = 0; m < this.tooltips.length; m++) {
+                    let y = this.tooltips[m];
+                    y && y.create == f.create && (u = m)
                 }
                 if (u < 0) o[h] = this.createTooltipView(f), l && (l[h] = !!f.above);
                 else {
-                    let g = o[h] = this.tooltipViews[u];
-                    l && (l[h] = t[u]), g.update && g.update(e)
+                    let m = o[h] = this.tooltipViews[u];
+                    l && (l[h] = t[u]), m.update && m.update(e)
                 }
             }
         }
         for (let h of this.tooltipViews) o.indexOf(h) < 0 && (h.dom.remove(), (i = h.destroy) === null || i === void 0 || i.call(h));
         return t && (l.forEach((h, f) => t[f] = h), t.length = l.length), this.input = r, this.tooltips = s, this.tooltipViews = o, !0
     }
 }
 
-function Ab(n) {
+function Tb(n) {
     let {
         win: e
     } = n;
     return {
         top: 0,
         left: 0,
         bottom: e.innerHeight,
@@ -11437,15 +11437,15 @@
 }
 const aa = Z.define({
         combine: n => {
             var e, t, i;
             return {
                 position: ee.ios ? "absolute" : ((e = n.find(r => r.position)) === null || e === void 0 ? void 0 : e.position) || "fixed",
                 parent: ((t = n.find(r => r.parent)) === null || t === void 0 ? void 0 : t.parent) || null,
-                tooltipSpace: ((i = n.find(r => r.tooltipSpace)) === null || i === void 0 ? void 0 : i.tooltipSpace) || Ab
+                tooltipSpace: ((i = n.find(r => r.tooltipSpace)) === null || i === void 0 ? void 0 : i.tooltipSpace) || Tb
             }
         }
     }),
     Pf = new WeakMap,
     $h = rt.fromClass(class {
         constructor(n) {
             this.view = n, this.above = [], this.inView = !0, this.madeAbsolute = !1, this.lastTransaction = 0, this.measureTimeout = -1;
@@ -11559,43 +11559,43 @@
             } = n, o = [];
             for (let l = 0; l < this.manager.tooltips.length; l++) {
                 let h = this.manager.tooltips[l],
                     f = this.manager.tooltipViews[l],
                     {
                         dom: u
                     } = f,
-                    g = n.pos[l],
+                    m = n.pos[l],
                     y = n.size[l];
-                if (!g || g.bottom <= Math.max(t.top, i.top) || g.top >= Math.min(t.bottom, i.bottom) || g.right < Math.max(t.left, i.left) - .1 || g.left > Math.min(t.right, i.right) + .1) {
+                if (!m || m.bottom <= Math.max(t.top, i.top) || m.top >= Math.min(t.bottom, i.bottom) || m.right < Math.max(t.left, i.left) - .1 || m.left > Math.min(t.right, i.right) + .1) {
                     u.style.top = jr;
                     continue
                 }
                 let k = h.arrow ? f.dom.querySelector(".cm-tooltip-arrow") : null,
                     v = k ? 7 : 0,
-                    C = y.right - y.left,
+                    A = y.right - y.left,
                     O = (e = Pf.get(f)) !== null && e !== void 0 ? e : y.bottom - y.top,
-                    D = f.offset || Ob,
+                    D = f.offset || Mb,
                     F = this.view.textDirection == Ue.LTR,
-                    $ = y.width > i.right - i.left ? F ? i.left : i.right - y.width : F ? Math.min(g.left - (k ? 14 : 0) + D.x, i.right - C) : Math.max(i.left, g.left - C + (k ? 14 : 0) - D.x),
+                    $ = y.width > i.right - i.left ? F ? i.left : i.right - y.width : F ? Math.min(m.left - (k ? 14 : 0) + D.x, i.right - A) : Math.max(i.left, m.left - A + (k ? 14 : 0) - D.x),
                     j = this.above[l];
-                !h.strictSide && (j ? g.top - (y.bottom - y.top) - D.y < i.top : g.bottom + (y.bottom - y.top) + D.y > i.bottom) && j == i.bottom - g.bottom > g.top - i.top && (j = this.above[l] = !j);
-                let z = (j ? g.top - i.top : i.bottom - g.bottom) - v;
+                !h.strictSide && (j ? m.top - (y.bottom - y.top) - D.y < i.top : m.bottom + (y.bottom - y.top) + D.y > i.bottom) && j == i.bottom - m.bottom > m.top - i.top && (j = this.above[l] = !j);
+                let z = (j ? m.top - i.top : i.bottom - m.bottom) - v;
                 if (z < O && f.resize !== !1) {
                     if (z < this.view.defaultLineHeight) {
                         u.style.top = jr;
                         continue
                     }
                     Pf.set(f, O), u.style.height = (O = z) / s + "px"
                 } else u.style.height && (u.style.height = "");
-                let G = j ? g.top - O - v - D.y : g.bottom + v + D.y,
-                    p = $ + C;
+                let G = j ? m.top - O - v - D.y : m.bottom + v + D.y,
+                    p = $ + A;
                 if (f.overlap !== !0)
                     for (let he of o) he.left < p && he.right > $ && he.top < G + O && he.bottom > G && (G = j ? he.top - O - 2 - v : he.bottom + v + 2);
                 if (this.position == "absolute" ? (u.style.top = (G - n.parent.top) / s + "px", u.style.left = ($ - n.parent.left) / r + "px") : (u.style.top = G / s + "px", u.style.left = $ / r + "px"), k) {
-                    let he = g.left + (F ? D.x : -D.x) - ($ + 14 - 7);
+                    let he = m.left + (F ? D.x : -D.x) - ($ + 14 - 7);
                     k.style.left = he / r + "px"
                 }
                 f.overlap !== !0 && o.push({
                     left: $,
                     top: G,
                     right: p,
                     bottom: G + O
@@ -11609,15 +11609,15 @@
     }, {
         eventObservers: {
             scroll() {
                 this.maybeMeasure()
             }
         }
     }),
-    Tb = te.baseTheme({
+    Ob = te.baseTheme({
         ".cm-tooltip": {
             zIndex: 100,
             boxSizing: "border-box"
         },
         "&light .cm-tooltip": {
             border: "1px solid #bbb",
             backgroundColor: "#f5f5f5"
@@ -11671,20 +11671,20 @@
             },
             "&:after": {
                 borderTopColor: "transparent",
                 borderBottomColor: "transparent"
             }
         }
     }),
-    Ob = {
+    Mb = {
         x: 0,
         y: 0
     },
     Wh = Z.define({
-        enables: [$h, Tb]
+        enables: [$h, Ob]
     }),
     Vo = Z.define();
 class kl {
     static create(e) {
         return new kl(e)
     }
     constructor(e) {
@@ -11728,28 +11728,28 @@
     get overlap() {
         return this.passProp("overlap")
     }
     get resize() {
         return this.passProp("resize")
     }
 }
-const Mb = Wh.compute([Vo], n => {
+const Eb = Wh.compute([Vo], n => {
     let e = n.facet(Vo).filter(t => t);
     return e.length === 0 ? null : {
         pos: Math.min(...e.map(t => t.pos)),
         end: Math.max(...e.map(t => {
             var i;
             return (i = t.end) !== null && i !== void 0 ? i : t.pos
         })),
         create: kl.create,
         above: e[0].above,
         arrow: e.some(t => t.arrow)
     }
 });
-class Eb {
+class Db {
     constructor(e, t, i, r, s) {
         this.view = e, this.source = t, this.field = i, this.setHover = r, this.hoverTime = s, this.hoverTimeout = -1, this.restartTimeout = -1, this.pending = null, this.lastMove = {
             x: 0,
             y: 0,
             target: e.dom,
             time: 0
         }, this.checkHover = this.checkHover.bind(this), e.dom.addEventListener("mouseleave", this.mouseleave = this.mouseleave.bind(this)), e.dom.addEventListener("mousemove", this.mousemove = this.mousemove.bind(this))
@@ -11809,19 +11809,19 @@
             target: e.target,
             time: Date.now()
         }, this.hoverTimeout < 0 && (this.hoverTimeout = setTimeout(this.checkHover, this.hoverTime));
         let {
             active: i,
             tooltip: r
         } = this;
-        if (i && r && !Db(r.dom, e) || this.pending) {
+        if (i && r && !Rb(r.dom, e) || this.pending) {
             let {
                 pos: s
             } = i || this.pending, o = (t = i == null ? void 0 : i.end) !== null && t !== void 0 ? t : s;
-            (s == o ? this.view.posAtCoords(this.lastMove) != s : !Rb(this.view, s, o, e.clientX, e.clientY)) && (this.view.dispatch({
+            (s == o ? this.view.posAtCoords(this.lastMove) != s : !Lb(this.view, s, o, e.clientX, e.clientY)) && (this.view.dispatch({
                 effects: this.setHover.of(null)
             }), this.pending = null)
         }
     }
     mouseleave(e) {
         clearTimeout(this.hoverTimeout), this.hoverTimeout = -1;
         let {
@@ -11846,59 +11846,59 @@
     }
     destroy() {
         clearTimeout(this.hoverTimeout), this.view.dom.removeEventListener("mouseleave", this.mouseleave), this.view.dom.removeEventListener("mousemove", this.mousemove)
     }
 }
 const co = 4;
 
-function Db(n, e) {
+function Rb(n, e) {
     let t = n.getBoundingClientRect();
     return e.clientX >= t.left - co && e.clientX <= t.right + co && e.clientY >= t.top - co && e.clientY <= t.bottom + co
 }
 
-function Rb(n, e, t, i, r, s) {
+function Lb(n, e, t, i, r, s) {
     let o = n.scrollDOM.getBoundingClientRect(),
         l = n.documentTop + n.documentPadding.top + n.contentHeight;
     if (o.left > i || o.right < i || o.top > r || Math.min(o.bottom, l) < r) return !1;
     let h = n.posAtCoords({
         x: i,
         y: r
     }, !1);
     return h >= e && h <= t
 }
 
-function Lb(n, e = {}) {
+function Pb(n, e = {}) {
     let t = me.define(),
         i = yt.define({
             create() {
                 return null
             },
             update(r, s) {
                 if (r && (e.hideOnChange && (s.docChanged || s.selection) || e.hideOn && e.hideOn(s, r))) return null;
                 if (r && s.docChanged) {
                     let o = s.changes.mapPos(r.pos, -1, Et.TrackDel);
                     if (o == null) return null;
                     let l = Object.assign(Object.create(null), r);
                     l.pos = o, r.end != null && (l.end = s.changes.mapPos(r.end)), r = l
                 }
-                for (let o of s.effects) o.is(t) && (r = o.value), o.is(Pb) && (r = null);
+                for (let o of s.effects) o.is(t) && (r = o.value), o.is(Nb) && (r = null);
                 return r
             },
             provide: r => Vo.from(r)
         });
-    return [i, rt.define(r => new Eb(r, n, i, t, e.hoverTime || 300)), Mb]
+    return [i, rt.define(r => new Db(r, n, i, t, e.hoverTime || 300)), Eb]
 }
 
 function dp(n, e) {
     let t = n.plugin($h);
     if (!t) return null;
     let i = t.manager.tooltips.indexOf(e);
     return i < 0 ? null : t.manager.tooltipViews[i]
 }
-const Pb = me.define(),
+const Nb = me.define(),
     Nf = Z.define({
         combine(n) {
             let e, t;
             for (let i of n) e = e || i.topContainer, t = t || i.bottomContainer;
             return {
                 topContainer: e,
                 bottomContainer: t
@@ -12005,40 +12005,40 @@
 }
 Ki.prototype.elementClass = "";
 Ki.prototype.toDOM = void 0;
 Ki.prototype.mapMode = Et.TrackBefore;
 Ki.prototype.startSide = Ki.prototype.endSide = -1;
 Ki.prototype.point = !0;
 const Io = Z.define(),
-    Nb = {
+    Ib = {
         class: "",
         renderEmptyElements: !1,
         elementStyle: "",
         markers: () => Pe.empty,
         lineMarker: () => null,
         widgetMarker: () => null,
         lineMarkerChange: null,
         initialSpacer: null,
         updateSpacer: null,
         domEventHandlers: {}
     },
     ls = Z.define();
 
-function Ib(n) {
-    return [gp(), ls.of(Object.assign(Object.assign({}, Nb), n))]
+function Bb(n) {
+    return [gp(), ls.of(Object.assign(Object.assign({}, Ib), n))]
 }
 const hh = Z.define({
     combine: n => n.some(e => e)
 });
 
 function gp(n) {
-    let e = [Bb];
+    let e = [_b];
     return n && n.fixed === !1 && e.push(hh.of(!0)), e
 }
-const Bb = rt.fromClass(class {
+const _b = rt.fromClass(class {
     constructor(n) {
         this.view = n, this.prevViewport = n.viewport, this.dom = document.createElement("div"), this.dom.className = "cm-gutters", this.dom.setAttribute("aria-hidden", "true"), this.dom.style.minHeight = this.view.contentHeight / this.view.scaleY + "px", this.gutters = n.state.facet(ls).map(e => new _f(n, e));
         for (let e of this.gutters) this.dom.appendChild(e.dom);
         this.fixed = !n.state.facet(hh), this.fixed && (this.dom.style.position = "sticky"), this.syncGutters(!1), n.scrollDOM.insertBefore(this.dom, n.contentDOM)
     }
     update(n) {
         if (this.updateGutters(n)) {
@@ -12050,15 +12050,15 @@
         n.geometryChanged && (this.dom.style.minHeight = this.view.contentHeight + "px"), this.view.state.facet(hh) != !this.fixed && (this.fixed = !this.fixed, this.dom.style.position = this.fixed ? "sticky" : ""), this.prevViewport = n.view.viewport
     }
     syncGutters(n) {
         let e = this.dom.nextSibling;
         n && this.dom.remove();
         let t = Pe.iter(this.view.state.facet(Io), this.view.viewport.from),
             i = [],
-            r = this.gutters.map(s => new _b(s, this.view.viewport, -this.view.documentPadding.top));
+            r = this.gutters.map(s => new Hb(s, this.view.viewport, -this.view.documentPadding.top));
         for (let s of this.view.viewportLineBlocks)
             if (i.length && (i = []), Array.isArray(s.type)) {
                 let o = !0;
                 for (let l of s.type)
                     if (l.type == Dt.Text && o) {
                         ch(t, i, l.from);
                         for (let h of r) h.line(this.view, l, i);
@@ -12110,15 +12110,15 @@
 function Bf(n) {
     return Array.isArray(n) ? n : [n]
 }
 
 function ch(n, e, t) {
     for (; n.value && n.from <= t;) n.from == t && e.push(n.value), n.next()
 }
-class _b {
+class Hb {
     constructor(e, t, i) {
         this.gutter = e, this.height = i, this.i = 0, this.cursor = Pe.iter(e.markers, t.from)
     }
     addElement(e, t, i) {
         let {
             gutter: r
         } = this, s = (t.top - this.height) / e.scaleY, o = t.height / e.scaleY;
@@ -12178,57 +12178,57 @@
     }
 }
 class mp {
     constructor(e, t, i, r) {
         this.height = -1, this.above = 0, this.markers = [], this.dom = document.createElement("div"), this.dom.className = "cm-gutterElement", this.update(e, t, i, r)
     }
     update(e, t, i, r) {
-        this.height != t && (this.height = t, this.dom.style.height = t + "px"), this.above != i && (this.dom.style.marginTop = (this.above = i) ? i + "px" : ""), Hb(this.markers, r) || this.setMarkers(e, r)
+        this.height != t && (this.height = t, this.dom.style.height = t + "px"), this.above != i && (this.dom.style.marginTop = (this.above = i) ? i + "px" : ""), Fb(this.markers, r) || this.setMarkers(e, r)
     }
     setMarkers(e, t) {
         let i = "cm-gutterElement",
             r = this.dom.firstChild;
         for (let s = 0, o = 0;;) {
             let l = o,
                 h = s < t.length ? t[s++] : null,
                 f = !1;
             if (h) {
                 let u = h.elementClass;
                 u && (i += " " + u);
-                for (let g = o; g < this.markers.length; g++)
-                    if (this.markers[g].compare(h)) {
-                        l = g, f = !0;
+                for (let m = o; m < this.markers.length; m++)
+                    if (this.markers[m].compare(h)) {
+                        l = m, f = !0;
                         break
                     }
             } else l = this.markers.length;
             for (; o < l;) {
                 let u = this.markers[o++];
                 if (u.toDOM) {
                     u.destroy(r);
-                    let g = r.nextSibling;
-                    r.remove(), r = g
+                    let m = r.nextSibling;
+                    r.remove(), r = m
                 }
             }
             if (!h) break;
             h.toDOM && (f ? r = r.nextSibling : this.dom.insertBefore(h.toDOM(e), r)), f && o++
         }
         this.dom.className = i, this.markers = t
     }
     destroy() {
         this.setMarkers(null, [])
     }
 }
 
-function Hb(n, e) {
+function Fb(n, e) {
     if (n.length != e.length) return !1;
     for (let t = 0; t < n.length; t++)
         if (!n[t].compare(e[t])) return !1;
     return !0
 }
-const Fb = Z.define(),
+const zb = Z.define(),
     fr = Z.define({
         combine(n) {
             return Hi(n, {
                 formatNumber: String,
                 domEventHandlers: {}
             }, {
                 domEventHandlers(e, t) {
@@ -12254,19 +12254,19 @@
         return document.createTextNode(this.number)
     }
 }
 
 function ca(n, e) {
     return n.state.facet(fr).formatNumber(e, n.state)
 }
-const zb = ls.compute([fr], n => ({
+const $b = ls.compute([fr], n => ({
     class: "cm-lineNumbers",
     renderEmptyElements: !1,
     markers(e) {
-        return e.state.facet(Fb)
+        return e.state.facet(zb)
     },
     lineMarker(e, t, i) {
         return i.some(r => r.toDOM) ? null : new ha(ca(e, e.state.doc.lineAt(t.from).number))
     },
     widgetMarker: () => null,
     lineMarkerChange: e => e.startState.facet(fr) != e.state.facet(fr),
     initialSpacer(e) {
@@ -12275,51 +12275,51 @@
     updateSpacer(e, t) {
         let i = ca(t.view, Hf(t.view.state.doc.lines));
         return i == e.number ? e : new ha(i)
     },
     domEventHandlers: n.facet(fr).domEventHandlers
 }));
 
-function $b(n = {}) {
-    return [fr.of(n), gp(), zb]
+function Wb(n = {}) {
+    return [fr.of(n), gp(), $b]
 }
 
 function Hf(n) {
     let e = 9;
     for (; e < n;) e = e * 10 + 9;
     return e
 }
-const Wb = new class extends Ki {
+const qb = new class extends Ki {
         constructor() {
             super(...arguments), this.elementClass = "cm-activeLineGutter"
         }
     },
-    qb = Io.compute(["selection"], n => {
+    jb = Io.compute(["selection"], n => {
         let e = [],
             t = -1;
         for (let i of n.selection.ranges) {
             let r = n.doc.lineAt(i.head).from;
-            r > t && (t = r, e.push(Wb.range(r)))
+            r > t && (t = r, e.push(qb.range(r)))
         }
         return Pe.of(e)
     });
 
-function jb() {
-    return qb
+function Vb() {
+    return jb
 }
 const yp = 1024;
-let Vb = 0;
+let Ub = 0;
 class fa {
     constructor(e, t) {
         this.from = e, this.to = t
     }
 }
 class Se {
     constructor(e = {}) {
-        this.id = Vb++, this.perNode = !!e.perNode, this.deserialize = e.deserialize || (() => {
+        this.id = Ub++, this.perNode = !!e.perNode, this.deserialize = e.deserialize || (() => {
             throw new Error("This node type doesn't define a deserialize function")
         })
     }
     add(e) {
         if (this.perNode) throw new RangeError("Can't add per-node props to node types");
         return typeof e != "function" && (e = Ht.match(e)), t => {
             let i = e(t);
@@ -12349,21 +12349,21 @@
     constructor(e, t, i) {
         this.tree = e, this.overlay = t, this.parser = i
     }
     static get(e) {
         return e && e.props && e.props[Se.mounted.id]
     }
 }
-const Ub = Object.create(null);
+const Qb = Object.create(null);
 class Ht {
     constructor(e, t, i, r = 0) {
         this.name = e, this.props = t, this.id = i, this.flags = r
     }
     static define(e) {
-        let t = e.props && e.props.length ? Object.create(null) : Ub,
+        let t = e.props && e.props.length ? Object.create(null) : Qb,
             i = (e.top ? 1 : 0) | (e.skipped ? 2 : 0) | (e.error ? 4 : 0) | (e.name == null ? 8 : 0),
             r = new Ht(e.name || "", t, e.id, i);
         if (e.props) {
             for (let s of e.props)
                 if (Array.isArray(s) || (s = s(r)), s) {
                     if (s[0].perNode) throw new RangeError("Can't store a per-node prop on a node type");
                     t[s[0].id] = s[1]
@@ -12465,15 +12465,15 @@
         return uo.set(this, i), i
     }
     resolveInner(e, t = 0) {
         let i = ks(Ff.get(this) || this.topNode, e, t, !0);
         return Ff.set(this, i), i
     }
     resolveStack(e, t = 0) {
-        return Kb(this, e, t)
+        return Xb(this, e, t)
     }
     iterate(e) {
         let {
             enter: t,
             leave: i,
             from: r = 0,
             to: s = this.length
@@ -12499,15 +12499,15 @@
             for (let t in this.props) e.push([+t, this.props[t]]);
         return e
     }
     balance(e = {}) {
         return this.children.length <= 8 ? this : Uh(Ht.none, this.children, this.positions, 0, this.children.length, 0, this.length, (t, i, r) => new Je(this.type, t, i, r, this.propValues), e.makeTree || ((t, i, r) => new Je(Ht.none, t, i, r)))
     }
     static build(e) {
-        return Xb(e)
+        return Yb(e)
     }
 }
 Je.empty = new Je(Ht.none, [], [], 0);
 class jh {
     constructor(e, t) {
         this.buffer = e, this.index = t
     }
@@ -12660,24 +12660,24 @@
     nextChild(e, t, i, r, s = 0) {
         for (let o = this;;) {
             for (let {
                     children: l,
                     positions: h
                 } = o._tree, f = t > 0 ? l.length : -1; e != f; e += t) {
                 let u = l[e],
-                    g = h[e] + o.from;
-                if (bp(r, i, g, g + u.length)) {
+                    m = h[e] + o.from;
+                if (bp(r, i, m, m + u.length)) {
                     if (u instanceof Sn) {
                         if (s & ot.ExcludeBuffers) continue;
-                        let y = u.findChild(0, u.buffer.length, t, i - g, r);
-                        if (y > -1) return new gn(new Qb(o, u, e, g), null, y)
+                        let y = u.findChild(0, u.buffer.length, t, i - m, r);
+                        if (y > -1) return new gn(new Gb(o, u, e, m), null, y)
                     } else if (s & ot.IncludeAnonymous || !u.type.isAnonymous || Vh(u)) {
                         let y;
-                        if (!(s & ot.IgnoreMounts) && (y = Uo.get(u)) && !y.overlay) return new si(y.tree, g, e, o);
-                        let k = new si(u, g, e, o);
+                        if (!(s & ot.IgnoreMounts) && (y = Uo.get(u)) && !y.overlay) return new si(y.tree, m, e, o);
+                        let k = new si(u, m, e, o);
                         return s & ot.IncludeAnonymous || !k.type.isAnonymous ? k : k.nextChild(t < 0 ? u.children.length - 1 : 0, t, i, r)
                     }
                 }
             }
             if (s & ot.IncludeAnonymous || !o.type.isAnonymous || (o.index >= 0 ? e = o.index + t : e = t < 0 ? -1 : o._parent._tree.children.length, o = o._parent, !o)) return null
         }
     }
@@ -12751,15 +12751,15 @@
         if (!i.type.isAnonymous) {
             if (e[t] && e[t] != i.name) return !1;
             t--
         }
     }
     return !0
 }
-class Qb {
+class Gb {
     constructor(e, t, i, r) {
         this.parent = e, this.buffer = t, this.index = i, this.start = r
     }
 }
 class gn extends xp {
     get name() {
         return this.type.name
@@ -12844,26 +12844,26 @@
         t = n[0];
     for (let s = 1; s < n.length; s++) {
         let o = n[s];
         (o.from > t.from || o.to < t.to) && (t = o, e = s)
     }
     let i = t instanceof si && t.index < 0 ? null : t.parent,
         r = n.slice();
-    return i ? r[e] = i : r.splice(e, 1), new Gb(r, t)
+    return i ? r[e] = i : r.splice(e, 1), new Kb(r, t)
 }
-class Gb {
+class Kb {
     constructor(e, t) {
         this.heads = e, this.node = t
     }
     get next() {
         return kp(this.heads)
     }
 }
 
-function Kb(n, e, t) {
+function Xb(n, e, t) {
     let i = n.resolveInner(e, t),
         r = null;
     for (let s = i instanceof si ? i : i.context.parent; s; s = s.parent)
         if (s.index < 0) {
             let o = s.parent;
             (r || (r = [i])).push(o.resolve(e, t)), s = o
         } else {
@@ -13054,25 +13054,25 @@
     }
 }
 
 function Vh(n) {
     return n.children.some(e => e instanceof Sn || !e.type.isAnonymous || Vh(e))
 }
 
-function Xb(n) {
+function Yb(n) {
     var e;
     let {
         buffer: t,
         nodeSet: i,
         maxBufferLength: r = yp,
         reused: s = [],
         minRepeatType: o = i.types.length
     } = n, l = Array.isArray(t) ? new jh(t, t.length) : t, h = i.types, f = 0, u = 0;
 
-    function g(z, G, p, he, J, ae) {
+    function m(z, G, p, he, J, ae) {
         let {
             id: pe,
             start: fe,
             end: ie,
             size: ye
         } = l, Be = u;
         for (; ye < 0;)
@@ -13087,31 +13087,31 @@
             u = pe;
             return
         } else throw new RangeError(`Unrecognized record size: ${ye}`);
         let st = h[pe],
             _e, Ye, be = fe - z;
         if (ie - fe <= r && (Ye = O(l.pos - G, J))) {
             let We = new Uint16Array(Ye.size - Ye.skip),
-                Ae = l.pos - Ye.size,
+                Ce = l.pos - Ye.size,
                 bt = We.length;
-            for (; l.pos > Ae;) bt = D(Ye.start, We, bt);
+            for (; l.pos > Ce;) bt = D(Ye.start, We, bt);
             _e = new Sn(We, ie - Ye.start, i), be = Ye.start - z
         } else {
             let We = l.pos - ye;
             l.next();
-            let Ae = [],
+            let Ce = [],
                 bt = [],
                 Oe = pe >= o ? pe : -1,
                 Tt = 0,
                 yi = ie;
-            for (; l.pos > We;) Oe >= 0 && l.id == Oe && l.size >= 0 ? (l.end <= yi - r && (v(Ae, bt, fe, Tt, l.end, yi, Oe, Be), Tt = Ae.length, yi = l.end), l.next()) : ae > 2500 ? y(fe, We, Ae, bt) : g(fe, We, Ae, bt, Oe, ae + 1);
-            if (Oe >= 0 && Tt > 0 && Tt < Ae.length && v(Ae, bt, fe, Tt, fe, yi, Oe, Be), Ae.reverse(), bt.reverse(), Oe > -1 && Tt > 0) {
+            for (; l.pos > We;) Oe >= 0 && l.id == Oe && l.size >= 0 ? (l.end <= yi - r && (v(Ce, bt, fe, Tt, l.end, yi, Oe, Be), Tt = Ce.length, yi = l.end), l.next()) : ae > 2500 ? y(fe, We, Ce, bt) : m(fe, We, Ce, bt, Oe, ae + 1);
+            if (Oe >= 0 && Tt > 0 && Tt < Ce.length && v(Ce, bt, fe, Tt, fe, yi, Oe, Be), Ce.reverse(), bt.reverse(), Oe > -1 && Tt > 0) {
                 let On = k(st);
-                _e = Uh(st, Ae, bt, 0, Ae.length, 0, ie - fe, On, On)
-            } else _e = C(st, Ae, bt, ie - fe, Be - ie)
+                _e = Uh(st, Ce, bt, 0, Ce.length, 0, ie - fe, On, On)
+            } else _e = A(st, Ce, bt, ie - fe, Be - ie)
         }
         p.push(_e), he.push(be)
     }
 
     function y(z, G, p, he) {
         let J = [],
             ae = 0,
@@ -13142,26 +13142,26 @@
             let J = 0,
                 ae = G.length - 1,
                 pe, fe;
             if (ae >= 0 && (pe = G[ae]) instanceof Je) {
                 if (!ae && pe.type == z && pe.length == he) return pe;
                 (fe = pe.prop(Se.lookAhead)) && (J = p[ae] + pe.length + fe)
             }
-            return C(z, G, p, he, J)
+            return A(z, G, p, he, J)
         }
     }
 
     function v(z, G, p, he, J, ae, pe, fe) {
         let ie = [],
             ye = [];
         for (; z.length > he;) ie.push(z.pop()), ye.push(G.pop() + p - J);
-        z.push(C(i.types[pe], ie, ye, ae - J, fe - ae)), G.push(J - p)
+        z.push(A(i.types[pe], ie, ye, ae - J, fe - ae)), G.push(J - p)
     }
 
-    function C(z, G, p, he, J = 0, ae) {
+    function A(z, G, p, he, J = 0, ae) {
         if (f) {
             let pe = [Se.contextHash, f];
             ae = ae ? [pe].concat(ae) : [pe]
         }
         if (J > 25) {
             let pe = [Se.lookAhead, J];
             ae = ae ? [pe].concat(ae) : [pe]
@@ -13217,15 +13217,15 @@
             }
             G[--p] = fe, G[--p] = ae - z, G[--p] = J - z, G[--p] = he
         } else pe == -3 ? f = he : pe == -4 && (u = he);
         return p
     }
     let F = [],
         $ = [];
-    for (; l.pos > 0;) g(n.start || 0, n.bufferStart || 0, F, $, -1, 0);
+    for (; l.pos > 0;) m(n.start || 0, n.bufferStart || 0, F, $, -1, 0);
     let j = (e = n.length) !== null && e !== void 0 ? e : F.length ? $[0] + F[0].length : 0;
     return new Je(h[n.topID], F.reverse(), $.reverse(), j)
 }
 const $f = new WeakMap;
 
 function Bo(n, e) {
     if (!n.isAnonymous || e instanceof Sn || e.type != n) return 1;
@@ -13244,42 +13244,42 @@
     return t
 }
 
 function Uh(n, e, t, i, r, s, o, l, h) {
     let f = 0;
     for (let v = i; v < r; v++) f += Bo(n, e[v]);
     let u = Math.ceil(f * 1.5 / 8),
-        g = [],
+        m = [],
         y = [];
 
-    function k(v, C, O, D, F) {
+    function k(v, A, O, D, F) {
         for (let $ = O; $ < D;) {
             let j = $,
-                z = C[$],
+                z = A[$],
                 G = Bo(n, v[$]);
             for ($++; $ < D; $++) {
                 let p = Bo(n, v[$]);
                 if (G + p >= u) break;
                 G += p
             }
             if ($ == j + 1) {
                 if (G > u) {
                     let p = v[j];
-                    k(p.children, p.positions, 0, p.children.length, C[j] + F);
+                    k(p.children, p.positions, 0, p.children.length, A[j] + F);
                     continue
                 }
-                g.push(v[j])
+                m.push(v[j])
             } else {
-                let p = C[$ - 1] + v[$ - 1].length - z;
-                g.push(Uh(n, v, C, j, $, z, p, null, h))
+                let p = A[$ - 1] + v[$ - 1].length - z;
+                m.push(Uh(n, v, A, j, $, z, p, null, h))
             }
             y.push(z + F - s)
         }
     }
-    return k(e, t, i, r, 0), (l || h)(g, y, o)
+    return k(e, t, i, r, 0), (l || h)(m, y, o)
 }
 class jn {
     constructor(e, t, i, r, s = !1, o = !1) {
         this.from = e, this.to = t, this.tree = i, this.offset = r, this.open = (s ? 1 : 0) | (o ? 2 : 0)
     }
     get openStart() {
         return (this.open & 1) > 0
@@ -13295,45 +13295,45 @@
     static applyChanges(e, t, i = 128) {
         if (!t.length) return e;
         let r = [],
             s = 1,
             o = e.length ? e[0] : null;
         for (let l = 0, h = 0, f = 0;; l++) {
             let u = l < t.length ? t[l] : null,
-                g = u ? u.fromA : 1e9;
-            if (g - h >= i)
-                for (; o && o.from < g;) {
+                m = u ? u.fromA : 1e9;
+            if (m - h >= i)
+                for (; o && o.from < m;) {
                     let y = o;
-                    if (h >= y.from || g <= y.to || f) {
+                    if (h >= y.from || m <= y.to || f) {
                         let k = Math.max(y.from, h) - f,
-                            v = Math.min(y.to, g) - f;
+                            v = Math.min(y.to, m) - f;
                         y = k >= v ? null : new jn(k, v, y.tree, y.offset + f, l > 0, !!u)
                     }
-                    if (y && r.push(y), o.to > g) break;
+                    if (y && r.push(y), o.to > m) break;
                     o = s < e.length ? e[s++] : null
                 }
             if (!u) break;
             h = u.toA, f = u.toA - u.toB
         }
         return r
     }
 }
 class wp {
     startParse(e, t, i) {
-        return typeof e == "string" && (e = new Yb(e)), i = i ? i.length ? i.map(r => new fa(r.from, r.to)) : [new fa(0, 0)] : [new fa(0, e.length)], this.createParse(e, t || [], i)
+        return typeof e == "string" && (e = new Jb(e)), i = i ? i.length ? i.map(r => new fa(r.from, r.to)) : [new fa(0, 0)] : [new fa(0, e.length)], this.createParse(e, t || [], i)
     }
     parse(e, t, i) {
         let r = this.startParse(e, t, i);
         for (;;) {
             let s = r.advance();
             if (s) return s
         }
     }
 }
-class Yb {
+class Jb {
     constructor(e) {
         this.string = e
     }
     get length() {
         return this.string.length
     }
     chunk(e) {
@@ -13345,56 +13345,56 @@
     read(e, t) {
         return this.string.slice(e, t)
     }
 }
 new Se({
     perNode: !0
 });
-let Jb = 0;
+let Zb = 0;
 class Di {
     constructor(e, t, i) {
-        this.set = e, this.base = t, this.modified = i, this.id = Jb++
+        this.set = e, this.base = t, this.modified = i, this.id = Zb++
     }
     static define(e) {
         if (e != null && e.base) throw new Error("Can not derive from a modified tag");
         let t = new Di([], null, []);
         if (t.set.push(t), e)
             for (let i of e.set) t.set.push(i);
         return t
     }
     static defineModifier() {
         let e = new Qo;
         return t => t.modified.indexOf(e) > -1 ? t : Qo.get(t.base || t, t.modified.concat(e).sort((i, r) => i.id - r.id))
     }
 }
-let Zb = 0;
+let ex = 0;
 class Qo {
     constructor() {
-        this.instances = [], this.id = Zb++
+        this.instances = [], this.id = ex++
     }
     static get(e, t) {
         if (!t.length) return e;
-        let i = t[0].instances.find(l => l.base == e && ex(t, l.modified));
+        let i = t[0].instances.find(l => l.base == e && tx(t, l.modified));
         if (i) return i;
         let r = [],
             s = new Di(r, e, t);
         for (let l of t) l.instances.push(s);
-        let o = tx(t);
+        let o = ix(t);
         for (let l of e.set)
             if (!l.modified.length)
                 for (let h of o) r.push(Qo.get(l, h));
         return s
     }
 }
 
-function ex(n, e) {
+function tx(n, e) {
     return n.length == e.length && n.every((t, i) => t == e[i])
 }
 
-function tx(n) {
+function ix(n) {
     let e = [
         []
     ];
     for (let t = 0; t < n.length; t++)
         for (let i = 0, r = e.length; i < r; i++) e.push(e[i].concat(n[t]));
     return e.sort((t, i) => i.length - t.length)
 }
@@ -13405,29 +13405,29 @@
         let i = n[t];
         Array.isArray(i) || (i = [i]);
         for (let r of t.split(" "))
             if (r) {
                 let s = [],
                     o = 2,
                     l = r;
-                for (let g = 0;;) {
-                    if (l == "..." && g > 0 && g + 3 == r.length) {
+                for (let m = 0;;) {
+                    if (l == "..." && m > 0 && m + 3 == r.length) {
                         o = 1;
                         break
                     }
                     let y = /^"(?:[^"\\]|\\.)*?"|[^\/!]+/.exec(l);
                     if (!y) throw new RangeError("Invalid path: " + r);
-                    if (s.push(y[0] == "*" ? "" : y[0][0] == '"' ? JSON.parse(y[0]) : y[0]), g += y[0].length, g == r.length) break;
-                    let k = r[g++];
-                    if (g == r.length && k == "!") {
+                    if (s.push(y[0] == "*" ? "" : y[0][0] == '"' ? JSON.parse(y[0]) : y[0]), m += y[0].length, m == r.length) break;
+                    let k = r[m++];
+                    if (m == r.length && k == "!") {
                         o = 0;
                         break
                     }
                     if (k != "/") throw new RangeError("Invalid path: " + r);
-                    l = r.slice(g)
+                    l = r.slice(m)
                 }
                 let h = s.length - 1,
                     f = s[h];
                 if (!f) throw new RangeError("Invalid path: " + r);
                 let u = new Go(i, o, h > 0 ? s.slice(0, h) : null);
                 e[f] = u.sort(e[f])
             }
@@ -13477,28 +13477,28 @@
                 }
             return o
         },
         scope: i
     }
 }
 
-function ix(n, e) {
+function nx(n, e) {
     let t = null;
     for (let i of n) {
         let r = i.style(e);
         r && (t = t ? t + " " + r : r)
     }
     return t
 }
 
-function nx(n, e, t, i = 0, r = n.length) {
-    let s = new rx(i, Array.isArray(e) ? e : [e], t);
+function rx(n, e, t, i = 0, r = n.length) {
+    let s = new sx(i, Array.isArray(e) ? e : [e], t);
     s.highlightRange(n.cursor(), i, r, "", s.highlighters), s.flush(r)
 }
-class rx {
+class sx {
     constructor(e, t, i) {
         this.at = e, this.highlighters = t, this.span = i, this.class = ""
     }
     startSpan(e, t) {
         t != this.class && (this.flush(e), e > this.at && (this.at = e), this.class = t)
     }
     flush(e) {
@@ -13509,46 +13509,46 @@
             type: o,
             from: l,
             to: h
         } = e;
         if (l >= i || h <= t) return;
         o.isTop && (s = this.highlighters.filter(k => !k.scope || k.scope(o)));
         let f = r,
-            u = sx(e) || Go.empty,
-            g = ix(s, u.tags);
-        if (g && (f && (f += " "), f += g, u.mode == 1 && (r += (r ? " " : "") + g)), this.startSpan(Math.max(t, l), f), u.opaque) return;
+            u = ox(e) || Go.empty,
+            m = nx(s, u.tags);
+        if (m && (f && (f += " "), f += m, u.mode == 1 && (r += (r ? " " : "") + m)), this.startSpan(Math.max(t, l), f), u.opaque) return;
         let y = e.tree && e.tree.prop(Se.mounted);
         if (y && y.overlay) {
             let k = e.node.enter(y.overlay[0].from + l, 1),
                 v = this.highlighters.filter(O => !O.scope || O.scope(y.tree.type)),
-                C = e.firstChild();
+                A = e.firstChild();
             for (let O = 0, D = l;; O++) {
                 let F = O < y.overlay.length ? y.overlay[O] : null,
                     $ = F ? F.from + l : h,
                     j = Math.max(t, D),
                     z = Math.min(i, $);
-                if (j < z && C)
+                if (j < z && A)
                     for (; e.from < z && (this.highlightRange(e, j, z, r, s), this.startSpan(Math.min(z, e.to), f), !(e.to >= $ || !e.nextSibling())););
                 if (!F || $ > i) break;
                 D = F.to + l, D > t && (this.highlightRange(k.cursor(), Math.max(t, F.from + l), Math.min(i, D), "", v), this.startSpan(Math.min(i, D), f))
             }
-            C && e.parent()
+            A && e.parent()
         } else if (e.firstChild()) {
             y && (r = "");
             do
                 if (!(e.to <= t)) {
                     if (e.from >= i) break;
                     this.highlightRange(e, t, i, r, s), this.startSpan(Math.min(i, e.to), f)
                 } while (e.nextSibling());
             e.parent()
         }
     }
 }
 
-function sx(n) {
+function ox(n) {
     let e = n.type.prop(Sp);
     for (; e && e.context && !n.matchContext(e.context);) e = e.next;
     return e || null
 }
 const Q = Di.define,
     po = Q(),
     hn = Q(),
@@ -13740,35 +13740,35 @@
 }, {
     tag: q.punctuation,
     class: "tok-punctuation"
 }]);
 var da;
 const ur = new Se;
 
-function ox(n) {
+function lx(n) {
     return Z.define({
         combine: n ? e => e.concat(n) : void 0
     })
 }
-const lx = new Se;
+const ax = new Se;
 class ui {
     constructor(e, t, i = [], r = "") {
         this.data = e, this.name = r, Ee.prototype.hasOwnProperty("tree") || Object.defineProperty(Ee.prototype, "tree", {
             get() {
                 return lt(this)
             }
         }), this.parser = t, this.extension = [Cn.of(this), Ee.languageData.of((s, o, l) => {
             let h = jf(s, o, l),
                 f = h.type.prop(ur);
             if (!f) return [];
             let u = s.facet(f),
-                g = h.type.prop(lx);
-            if (g) {
+                m = h.type.prop(ax);
+            if (m) {
                 let y = h.resolve(o - h.from, l);
-                for (let k of g)
+                for (let k of m)
                     if (k.test(y, s)) {
                         let v = s.facet(k.facet);
                         return k.type == "replace" ? v : v.concat(u)
                     }
             }
             return u
         })].concat(i)
@@ -13831,15 +13831,15 @@
     return r
 }
 class Ko extends ui {
     constructor(e, t, i) {
         super(e, t, [], i), this.parser = t
     }
     static define(e) {
-        let t = ox(e.languageData);
+        let t = lx(e.languageData);
         return new Ko(t, e.parser.configure({
             props: [ur.add(i => i.isTop ? t : void 0)]
         }), e.name)
     }
     configure(e, t) {
         return new Ko(this.data, this.parser.configure(e), t || this.name)
     }
@@ -13848,15 +13848,15 @@
     }
 }
 
 function lt(n) {
     let e = n.field(ui.state, !1);
     return e ? e.tree : Je.empty
 }
-class ax {
+class hx {
     constructor(e) {
         this.doc = e, this.cursorPos = 0, this.string = "", this.cursor = e.iter()
     }
     get length() {
         return this.doc.length
     }
     syncTo(e) {
@@ -13878,15 +13878,15 @@
     constructor(e, t, i = [], r, s, o, l, h) {
         this.parser = e, this.state = t, this.fragments = i, this.tree = r, this.treeLen = s, this.viewport = o, this.skipped = l, this.scheduleOn = h, this.parse = null, this.tempSkipped = []
     }
     static create(e, t, i) {
         return new Xo(e, t, [], Je.empty, 0, i, [], null)
     }
     startParse() {
-        return this.parser.startParse(new ax(this.state.doc), this.fragments)
+        return this.parser.startParse(new hx(this.state.doc), this.fragments)
     }
     work(e, t) {
         return t != null && t >= this.state.doc.length && (t = void 0), this.tree != Je.empty && this.isDone(t != null ? t : this.state.doc.length) ? (this.takeTree(), !0) : this.withContext(() => {
             var i;
             if (typeof e == "number") {
                 let r = Date.now() + e;
                 e = () => Date.now() > r
@@ -13925,30 +13925,30 @@
             tree: r,
             treeLen: s,
             viewport: o,
             skipped: l
         } = this;
         if (this.takeTree(), !e.empty) {
             let h = [];
-            if (e.iterChangedRanges((f, u, g, y) => h.push({
+            if (e.iterChangedRanges((f, u, m, y) => h.push({
                     fromA: f,
                     toA: u,
-                    fromB: g,
+                    fromB: m,
                     toB: y
                 })), i = jn.applyChanges(i, h), r = Je.empty, s = 0, o = {
                     from: e.mapPos(o.from, -1),
                     to: e.mapPos(o.to, 1)
                 }, this.skipped.length) {
                 l = [];
                 for (let f of this.skipped) {
                     let u = e.mapPos(f.from, 1),
-                        g = e.mapPos(f.to, -1);
-                    u < g && l.push({
+                        m = e.mapPos(f.to, -1);
+                    u < m && l.push({
                         from: u,
-                        to: g
+                        to: m
                     })
                 }
             }
         }
         return new Xo(this.parser, t, i, r, s, o, l, this.scheduleOn)
     }
     updateViewport(e) {
@@ -14049,15 +14049,15 @@
             e = requestIdleCallback(n, {
                 timeout: 400
             })
         }, 100);
     return () => e < 0 ? clearTimeout(t) : cancelIdleCallback(e)
 });
 const pa = typeof navigator != "undefined" && (!((da = navigator.scheduling) === null || da === void 0) && da.isInputPending) ? () => navigator.scheduling.isInputPending() : null,
-    hx = rt.fromClass(class {
+    cx = rt.fromClass(class {
         constructor(e) {
             this.view = e, this.working = null, this.workScheduled = 0, this.chunkEnd = -1, this.chunkBudget = -1, this.work = this.work.bind(this), this.scheduleWork()
         }
         update(e) {
             let t = this.view.state.field(ui.state).context;
             (t.updateViewport(e.view.viewport) || this.view.viewport.to > t.treeLen) && this.scheduleWork(), (e.docChanged || e.selectionSet) && (this.view.hasFocus && (this.chunkBudget += 50), this.scheduleWork()), this.checkAsyncSchedule(t)
         }
@@ -14102,27 +14102,27 @@
             }
         }
     }),
     Cn = Z.define({
         combine(n) {
             return n.length ? n[0] : null
         },
-        enables: n => [ui.state, hx, te.contentAttributes.compute([n], e => {
+        enables: n => [ui.state, cx, te.contentAttributes.compute([n], e => {
             let t = e.facet(n);
             return t && t.name ? {
                 "data-language": t.name
             } : {}
         })]
     });
-class cx {
+class fx {
     constructor(e, t = []) {
         this.language = e, this.support = t, this.extension = [e, t]
     }
 }
-const fx = Z.define(),
+const ux = Z.define(),
     Qh = Z.define({
         combine: n => {
             if (!n.length) return "  ";
             let e = n[0];
             if (!e || /\S/.test(e) || Array.from(e).some(t => t != e[0])) throw new Error("Invalid indent unit: " + JSON.stringify(n[0]));
             return e
         }
@@ -14143,20 +14143,20 @@
     }
     for (let s = 0; s < e; s++) t += r;
     return t
 }
 
 function Gh(n, e) {
     n instanceof Ee && (n = new wl(n));
-    for (let i of n.state.facet(fx)) {
+    for (let i of n.state.facet(ux)) {
         let r = i(n, e);
         if (r !== void 0) return r
     }
     let t = lt(n.state);
-    return t.length >= e ? ux(n, t, e) : null
+    return t.length >= e ? dx(n, t, e) : null
 }
 class wl {
     constructor(e, t = {}) {
         this.state = e, this.options = t, this.unit = Yo(e)
     }
     lineAt(e, t = 1) {
         let i = this.state.doc.lineAt(e),
@@ -14206,15 +14206,15 @@
     }
     get simulatedBreak() {
         return this.options.simulateBreak || null
     }
 }
 const Tp = new Se;
 
-function ux(n, e, t) {
+function dx(n, e, t) {
     let i = e.resolveStack(t),
         r = i.node.enterUnfinishedNodesBefore(t);
     if (r != i.node) {
         let s = [];
         for (let o = r; o != i.node; o = o.parent) s.push(o);
         for (let o = s.length - 1; o >= 0; o--) i = {
             node: s[o],
@@ -14222,38 +14222,38 @@
         }
     }
     return Op(i, n, t)
 }
 
 function Op(n, e, t) {
     for (let i = n; i; i = i.next) {
-        let r = px(i.node);
+        let r = gx(i.node);
         if (r) return r(Kh.create(e, t, i))
     }
     return 0
 }
 
-function dx(n) {
+function px(n) {
     return n.pos == n.options.simulateBreak && n.options.simulateDoubleBreak
 }
 
-function px(n) {
+function gx(n) {
     let e = n.type.prop(Tp);
     if (e) return e;
     let t = n.firstChild,
         i;
     if (t && (i = t.type.prop(Se.closedBy))) {
         let r = n.lastChild,
             s = r && i.indexOf(r.name) > -1;
-        return o => bx(o, !0, 1, void 0, s && !dx(o) ? r.from : void 0)
+        return o => xx(o, !0, 1, void 0, s && !px(o) ? r.from : void 0)
     }
-    return n.parent == null ? gx : null
+    return n.parent == null ? mx : null
 }
 
-function gx() {
+function mx() {
     return 0
 }
 class Kh extends wl {
     constructor(e, t, i) {
         super(e.state, e.options), this.base = e, this.pos = t, this.context = i
     }
     get node() {
@@ -14269,31 +14269,31 @@
         return this.baseIndentFor(this.node)
     }
     baseIndentFor(e) {
         let t = this.state.doc.lineAt(e.from);
         for (;;) {
             let i = e.resolve(t.from);
             for (; i.parent && i.parent.from == i.from;) i = i.parent;
-            if (mx(i, e)) break;
+            if (yx(i, e)) break;
             t = this.state.doc.lineAt(i.from)
         }
         return this.lineIndent(t.from)
     }
     continue () {
         return Op(this.context.next, this.base, this.pos)
     }
 }
 
-function mx(n, e) {
+function yx(n, e) {
     for (let t = e; t; t = t.parent)
         if (n == t) return !0;
     return !1
 }
 
-function yx(n) {
+function bx(n) {
     let e = n.node,
         t = e.childAfter(e.from),
         i = e.lastChild;
     if (!t) return null;
     let r = n.options.simulateBreak,
         s = n.state.doc.lineAt(t.from),
         o = r == null || r <= s.from ? s.to : Math.min(s.to, r);
@@ -14301,104 +14301,104 @@
         let h = e.childAfter(l);
         if (!h || h == i) return null;
         if (!h.type.isSkipped) return h.from < o ? t : null;
         l = h.to
     }
 }
 
-function bx(n, e, t, i, r) {
+function xx(n, e, t, i, r) {
     let s = n.textAfter,
         o = s.match(/^\s*/)[0].length,
         l = i && s.slice(o, o + i.length) == i || r == n.pos + o,
-        h = e ? yx(n) : null;
+        h = e ? bx(n) : null;
     return h ? l ? n.column(h.from) : n.column(h.to) : n.baseIndent + (l ? 0 : n.unit * t)
 }
 
-function xx({
+function kx({
     except: n,
     units: e = 1
 } = {}) {
     return t => {
         let i = n && n.test(t.textAfter);
         return t.baseIndent + (i ? 0 : e * t.unit)
     }
 }
-const kx = 200;
+const wx = 200;
 
-function wx() {
+function vx() {
     return Ee.transactionFilter.of(n => {
         if (!n.docChanged || !n.isUserEvent("input.type") && !n.isUserEvent("input.complete")) return n;
         let e = n.startState.languageDataAt("indentOnInput", n.startState.selection.main.head);
         if (!e.length) return n;
         let t = n.newDoc,
             {
                 head: i
             } = n.newSelection.main,
             r = t.lineAt(i);
-        if (i > r.from + kx) return n;
+        if (i > r.from + wx) return n;
         let s = t.sliceString(r.from, i);
         if (!e.some(f => f.test(s))) return n;
         let {
             state: o
         } = n, l = -1, h = [];
         for (let {
                 head: f
             }
             of o.selection.ranges) {
             let u = o.doc.lineAt(f);
             if (u.from == l) continue;
             l = u.from;
-            let g = Gh(o, u.from);
-            if (g == null) continue;
+            let m = Gh(o, u.from);
+            if (m == null) continue;
             let y = /^\s*/.exec(u.text)[0],
-                k = ws(o, g);
+                k = ws(o, m);
             y != k && h.push({
                 from: u.from,
                 to: u.from + y.length,
                 insert: k
             })
         }
         return h.length ? [n, {
             changes: h,
             sequential: !0
         }] : n
     })
 }
-const vx = Z.define(),
+const Sx = Z.define(),
     Mp = new Se;
 
-function Sx(n, e, t) {
+function Cx(n, e, t) {
     let i = lt(n);
     if (i.length < t) return null;
     let r = i.resolveStack(t, 1),
         s = null;
     for (let o = r; o; o = o.next) {
         let l = o.node;
         if (l.to <= t || l.from > t) continue;
         if (s && l.from < e) break;
         let h = l.type.prop(Mp);
-        if (h && (l.to < i.length - 50 || i.length == n.doc.length || !Cx(l))) {
+        if (h && (l.to < i.length - 50 || i.length == n.doc.length || !Ax(l))) {
             let f = h(l, n);
             f && f.from <= t && f.from >= e && f.to > t && (s = f)
         }
     }
     return s
 }
 
-function Cx(n) {
+function Ax(n) {
     let e = n.lastChild;
     return e && e.to == n.to && e.type.isError
 }
 
 function Jo(n, e, t) {
-    for (let i of n.facet(vx)) {
+    for (let i of n.facet(Sx)) {
         let r = i(n, e, t);
         if (r) return r
     }
-    return Sx(n, e, t)
+    return Cx(n, e, t)
 }
 
 function Ep(n, e) {
     let t = e.mapPos(n.from, 1),
         i = e.mapPos(n.to, -1);
     return t >= i ? void 0 : {
         from: t,
@@ -14423,19 +14423,19 @@
 const Qn = yt.define({
     create() {
         return de.none
     },
     update(n, e) {
         n = n.map(e.changes);
         for (let t of e.effects)
-            if (t.is(vl) && !Ax(n, t.value.from, t.value.to)) {
+            if (t.is(vl) && !Tx(n, t.value.from, t.value.to)) {
                 let {
                     preparePlaceholder: i
                 } = e.state.facet(Xh), r = i ? de.replace({
-                    widget: new Lx(i(e.state, t.value))
+                    widget: new Px(i(e.state, t.value))
                 }) : Uf;
                 n = n.update({
                     add: [r.range(t.value.from, t.value.to)]
                 })
             } else t.is(Rs) && (n = n.update({
                 filter: (i, r) => t.value.from != i || t.value.to != r,
                 filterFrom: t.value.from,
@@ -14483,34 +14483,34 @@
         (!r || r.from > s) && (r = {
             from: s,
             to: o
         })
     }), r
 }
 
-function Ax(n, e, t) {
+function Tx(n, e, t) {
     let i = !1;
     return n.between(e, e, (r, s) => {
         r == e && s == t && (i = !0)
     }), i
 }
 
 function Rp(n, e) {
     return n.field(Qn, !1) ? e : e.concat(me.appendConfig.of(Pp()))
 }
-const Tx = n => {
+const Ox = n => {
         for (let e of Dp(n)) {
             let t = Jo(n.state, e.from, e.to);
             if (t) return n.dispatch({
                 effects: Rp(n.state, [vl.of(t), Lp(n, t)])
             }), !0
         }
         return !1
     },
-    Ox = n => {
+    Mx = n => {
         if (!n.state.field(Qn, !1)) return !1;
         let e = [];
         for (let t of Dp(n)) {
             let i = Zo(n.state, t.from, t.to);
             i && e.push(Rs.of(i), Lp(n, i, !1))
         }
         return e.length && n.dispatch({
@@ -14519,68 +14519,68 @@
     };
 
 function Lp(n, e, t = !0) {
     let i = n.state.doc.lineAt(e.from).number,
         r = n.state.doc.lineAt(e.to).number;
     return te.announce.of(`${n.state.phrase(t?"Folded lines":"Unfolded lines")} ${i} ${n.state.phrase("to")} ${r}.`)
 }
-const Mx = n => {
+const Ex = n => {
         let {
             state: e
         } = n, t = [];
         for (let i = 0; i < e.doc.length;) {
             let r = n.lineBlockAt(i),
                 s = Jo(e, r.from, r.to);
             s && t.push(vl.of(s)), i = (s ? n.lineBlockAt(s.to) : r).to + 1
         }
         return t.length && n.dispatch({
             effects: Rp(n.state, t)
         }), !!t.length
     },
-    Ex = n => {
+    Dx = n => {
         let e = n.state.field(Qn, !1);
         if (!e || !e.size) return !1;
         let t = [];
         return e.between(0, n.state.doc.length, (i, r) => {
             t.push(Rs.of({
                 from: i,
                 to: r
             }))
         }), n.dispatch({
             effects: t
         }), !0
     },
-    Dx = [{
+    Rx = [{
         key: "Ctrl-Shift-[",
         mac: "Cmd-Alt-[",
-        run: Tx
+        run: Ox
     }, {
         key: "Ctrl-Shift-]",
         mac: "Cmd-Alt-]",
-        run: Ox
+        run: Mx
     }, {
         key: "Ctrl-Alt-[",
-        run: Mx
+        run: Ex
     }, {
         key: "Ctrl-Alt-]",
-        run: Ex
+        run: Dx
     }],
-    Rx = {
+    Lx = {
         placeholderDOM: null,
         preparePlaceholder: null,
         placeholderText: "…"
     },
     Xh = Z.define({
         combine(n) {
-            return Hi(n, Rx)
+            return Hi(n, Lx)
         }
     });
 
 function Pp(n) {
-    let e = [Qn, Ix];
+    let e = [Qn, Bx];
     return n && e.push(Xh.of(n)), e
 }
 
 function Np(n, e) {
     let {
         state: t
     } = n, i = t.facet(Xh), r = o => {
@@ -14597,26 +14597,26 @@
 const Uf = de.replace({
     widget: new class extends An {
         toDOM(n) {
             return Np(n, null)
         }
     }
 });
-class Lx extends An {
+class Px extends An {
     constructor(e) {
         super(), this.value = e
     }
     eq(e) {
         return this.value == e.value
     }
     toDOM(e) {
         return Np(e, this.value)
     }
 }
-const Px = {
+const Nx = {
     openText: "⌄",
     closedText: "›",
     markerDOM: null,
     domEventHandlers: {},
     foldingChanged: () => !1
 };
 class ga extends Ki {
@@ -14629,16 +14629,16 @@
     toDOM(e) {
         if (this.config.markerDOM) return this.config.markerDOM(this.open);
         let t = document.createElement("span");
         return t.textContent = this.open ? this.config.openText : this.config.closedText, t.title = e.state.phrase(this.open ? "Fold line" : "Unfold line"), t
     }
 }
 
-function Nx(n = {}) {
-    let e = Object.assign(Object.assign({}, Px), n),
+function Ix(n = {}) {
+    let e = Object.assign(Object.assign({}, Nx), n),
         t = new ga(e, !0),
         i = new ga(e, !1),
         r = rt.fromClass(class {
             constructor(o) {
                 this.from = o.viewport.from, this.markers = this.buildMarkers(o)
             }
             update(o) {
@@ -14652,15 +14652,15 @@
                 }
                 return l.finish()
             }
         }),
         {
             domEventHandlers: s
         } = e;
-    return [r, Ib({
+    return [r, Bb({
         class: "cm-foldGutter",
         markers(o) {
             var l;
             return ((l = o.plugin(r)) === null || l === void 0 ? void 0 : l.markers) || Pe.empty
         },
         initialSpacer() {
             return new ga(e, !1)
@@ -14676,15 +14676,15 @@
                 return u ? (o.dispatch({
                     effects: vl.of(u)
                 }), !0) : !1
             }
         })
     }), Pp()]
 }
-const Ix = te.baseTheme({
+const Bx = te.baseTheme({
     ".cm-foldPlaceholder": {
         backgroundColor: "#eee",
         border: "1px solid #ddd",
         color: "#888",
         borderRadius: ".2em",
         margin: "0 1px",
         padding: "0 1px",
@@ -14727,20 +14727,20 @@
     });
 
 function ma(n) {
     let e = n.facet(ph);
     return e.length ? e : n.facet(Ip)
 }
 
-function Bx(n, e) {
-    let t = [Hx],
+function _x(n, e) {
+    let t = [Fx],
         i;
     return n instanceof Sl && (n.module && t.push(te.styleModule.of(n.module)), i = n.themeType), e != null && e.fallback ? t.push(Ip.of(n)) : i ? t.push(ph.computeN([te.darkTheme], r => r.facet(te.darkTheme) == (i == "dark") ? [n] : [])) : t.push(ph.of(n)), t
 }
-class _x {
+class Hx {
     constructor(e) {
         this.markCache = Object.create(null), this.tree = lt(e.state), this.decorations = this.buildDeco(e, ma(e.state))
     }
     update(e) {
         let t = lt(e.state),
             i = ma(e.state),
             r = i != ma(e.startState);
@@ -14749,26 +14749,26 @@
     buildDeco(e, t) {
         if (!t || !this.tree.length) return de.none;
         let i = new xn;
         for (let {
                 from: r,
                 to: s
             }
-            of e.visibleRanges) nx(this.tree, t, (o, l, h) => {
+            of e.visibleRanges) rx(this.tree, t, (o, l, h) => {
             i.add(o, l, this.markCache[h] || (this.markCache[h] = de.mark({
                 class: h
             })))
         }, r, s);
         return i.finish()
     }
 }
-const Hx = Kn.high(rt.fromClass(_x, {
+const Fx = Kn.high(rt.fromClass(Hx, {
         decorations: n => n.decorations
     })),
-    Fx = Sl.define([{
+    zx = Sl.define([{
         tag: q.meta,
         color: "#404740"
     }, {
         tag: q.link,
         textDecoration: "underline"
     }, {
         tag: q.heading,
@@ -14819,15 +14819,15 @@
     }, {
         tag: q.comment,
         color: "#940"
     }, {
         tag: q.invalid,
         color: "#f00"
     }]),
-    zx = te.baseTheme({
+    $x = te.baseTheme({
         "&.cm-focused .cm-matchingBracket": {
             backgroundColor: "#328c8252"
         },
         "&.cm-focused .cm-nonmatchingBracket": {
             backgroundColor: "#bb555544"
         }
     }),
@@ -14835,31 +14835,31 @@
     _p = "()[]{}",
     Hp = Z.define({
         combine(n) {
             return Hi(n, {
                 afterCursor: !0,
                 brackets: _p,
                 maxScanDistance: Bp,
-                renderMatch: qx
+                renderMatch: jx
             })
         }
     }),
-    $x = de.mark({
+    Wx = de.mark({
         class: "cm-matchingBracket"
     }),
-    Wx = de.mark({
+    qx = de.mark({
         class: "cm-nonmatchingBracket"
     });
 
-function qx(n) {
+function jx(n) {
     let e = [],
-        t = n.matched ? $x : Wx;
+        t = n.matched ? Wx : qx;
     return e.push(t.range(n.start.from, n.start.to)), n.end && e.push(t.range(n.end.from, n.end.to)), e
 }
-const jx = yt.define({
+const Vx = yt.define({
         create() {
             return de.none
         },
         update(n, e) {
             if (!e.docChanged && !e.selection) return n;
             let t = [],
                 i = e.state.facet(Hp);
@@ -14868,156 +14868,156 @@
                 let s = Pi(e.state, r.head, -1, i) || r.head > 0 && Pi(e.state, r.head - 1, 1, i) || i.afterCursor && (Pi(e.state, r.head, 1, i) || r.head < e.state.doc.length && Pi(e.state, r.head + 1, -1, i));
                 s && (t = t.concat(i.renderMatch(s, e.state)))
             }
             return de.set(t, !0)
         },
         provide: n => te.decorations.from(n)
     }),
-    Vx = [jx, zx];
+    Ux = [Vx, $x];
 
-function Ux(n = {}) {
-    return [Hp.of(n), Vx]
+function Qx(n = {}) {
+    return [Hp.of(n), Ux]
 }
-const Qx = new Se;
+const Gx = new Se;
 
 function gh(n, e, t) {
     let i = n.prop(e < 0 ? Se.openedBy : Se.closedBy);
     if (i) return i;
     if (n.name.length == 1) {
         let r = t.indexOf(n.name);
         if (r > -1 && r % 2 == (e < 0 ? 1 : 0)) return [t[r + e]]
     }
     return null
 }
 
 function mh(n) {
-    let e = n.type.prop(Qx);
+    let e = n.type.prop(Gx);
     return e ? e(n.node) : n
 }
 
 function Pi(n, e, t, i = {}) {
     let r = i.maxScanDistance || Bp,
         s = i.brackets || _p,
         o = lt(n),
         l = o.resolveInner(e, t);
     for (let h = l; h; h = h.parent) {
         let f = gh(h.type, t, s);
         if (f && h.from < h.to) {
             let u = mh(h);
-            if (u && (t > 0 ? e >= u.from && e < u.to : e > u.from && e <= u.to)) return Gx(n, e, t, h, u, f, s)
+            if (u && (t > 0 ? e >= u.from && e < u.to : e > u.from && e <= u.to)) return Kx(n, e, t, h, u, f, s)
         }
     }
-    return Kx(n, e, t, o, l.type, r, s)
+    return Xx(n, e, t, o, l.type, r, s)
 }
 
-function Gx(n, e, t, i, r, s, o) {
+function Kx(n, e, t, i, r, s, o) {
     let l = i.parent,
         h = {
             from: r.from,
             to: r.to
         },
         f = 0,
         u = l == null ? void 0 : l.cursor();
     if (u && (t < 0 ? u.childBefore(i.from) : u.childAfter(i.to)))
         do
             if (t < 0 ? u.to <= i.from : u.from >= i.to) {
                 if (f == 0 && s.indexOf(u.type.name) > -1 && u.from < u.to) {
-                    let g = mh(u);
+                    let m = mh(u);
                     return {
                         start: h,
-                        end: g ? {
-                            from: g.from,
-                            to: g.to
+                        end: m ? {
+                            from: m.from,
+                            to: m.to
                         } : void 0,
                         matched: !0
                     }
                 } else if (gh(u.type, t, o)) f++;
                 else if (gh(u.type, -t, o)) {
                     if (f == 0) {
-                        let g = mh(u);
+                        let m = mh(u);
                         return {
                             start: h,
-                            end: g && g.from < g.to ? {
-                                from: g.from,
-                                to: g.to
+                            end: m && m.from < m.to ? {
+                                from: m.from,
+                                to: m.to
                             } : void 0,
                             matched: !1
                         }
                     }
                     f--
                 }
             } while (t < 0 ? u.prevSibling() : u.nextSibling());
     return {
         start: h,
         matched: !1
     }
 }
 
-function Kx(n, e, t, i, r, s, o) {
+function Xx(n, e, t, i, r, s, o) {
     let l = t < 0 ? n.sliceDoc(e - 1, e) : n.sliceDoc(e, e + 1),
         h = o.indexOf(l);
     if (h < 0 || h % 2 == 0 != t > 0) return null;
     let f = {
             from: t < 0 ? e - 1 : e,
             to: t > 0 ? e + 1 : e
         },
         u = n.doc.iterRange(e, t > 0 ? n.doc.length : 0),
-        g = 0;
+        m = 0;
     for (let y = 0; !u.next().done && y <= s;) {
         let k = u.value;
         t < 0 && (y += k.length);
         let v = e + y * t;
-        for (let C = t > 0 ? 0 : k.length - 1, O = t > 0 ? k.length : -1; C != O; C += t) {
-            let D = o.indexOf(k[C]);
-            if (!(D < 0 || i.resolveInner(v + C, 1).type != r))
-                if (D % 2 == 0 == t > 0) g++;
+        for (let A = t > 0 ? 0 : k.length - 1, O = t > 0 ? k.length : -1; A != O; A += t) {
+            let D = o.indexOf(k[A]);
+            if (!(D < 0 || i.resolveInner(v + A, 1).type != r))
+                if (D % 2 == 0 == t > 0) m++;
                 else {
-                    if (g == 1) return {
+                    if (m == 1) return {
                         start: f,
                         end: {
-                            from: v + C,
-                            to: v + C + 1
+                            from: v + A,
+                            to: v + A + 1
                         },
                         matched: D >> 1 == h >> 1
                     };
-                    g--
+                    m--
                 }
         }
         t > 0 && (y += k.length)
     }
     return u.done ? {
         start: f,
         matched: !1
     } : null
 }
-const Xx = Object.create(null),
+const Yx = Object.create(null),
     Qf = [Ht.none],
     Gf = [],
     Kf = Object.create(null),
-    Yx = Object.create(null);
+    Jx = Object.create(null);
 for (let [n, e] of [
         ["variable", "variableName"],
         ["variable-2", "variableName.special"],
         ["string-2", "string.special"],
         ["def", "variableName.definition"],
         ["tag", "tagName"],
         ["attribute", "attributeName"],
         ["type", "typeName"],
         ["builtin", "variableName.standard"],
         ["qualifier", "modifier"],
         ["error", "invalid"],
         ["header", "heading"],
         ["property", "propertyName"]
-    ]) Yx[n] = Jx(Xx, e);
+    ]) Jx[n] = Zx(Yx, e);
 
 function ya(n, e) {
     Gf.indexOf(n) > -1 || (Gf.push(n), console.warn(e))
 }
 
-function Jx(n, e) {
+function Zx(n, e) {
     let t = [];
     for (let l of e.split(" ")) {
         let h = [];
         for (let f of l.split(".")) {
             let u = n[f] || q[f];
             u ? typeof u == "function" ? h.length ? h = h.map(u) : ya(f, `Modifier ${f} used at start of tag`) : h.length ? ya(f, `Tag ${f} used as modifier`) : h = Array.isArray(u) ? u : [u] : ya(f, `Unknown highlighting tag ${f}`)
         }
@@ -15033,42 +15033,42 @@
         name: i,
         props: [vp({
             [i]: t
         })]
     });
     return Qf.push(o), o.id
 }
-const Zx = n => {
+const e1 = n => {
     let {
         state: e
     } = n, t = e.doc.lineAt(e.selection.main.from), i = Jh(n.state, t.from);
-    return i.line ? e1(n) : i.block ? i1(n) : !1
+    return i.line ? t1(n) : i.block ? n1(n) : !1
 };
 
 function Yh(n, e) {
     return ({
         state: t,
         dispatch: i
     }) => {
         if (t.readOnly) return !1;
         let r = n(e, t);
         return r ? (i(t.update(r)), !0) : !1
     }
 }
-const e1 = Yh(s1, 0),
-    t1 = Yh(Fp, 0),
-    i1 = Yh((n, e) => Fp(n, e, r1(e)), 0);
+const t1 = Yh(o1, 0),
+    i1 = Yh(Fp, 0),
+    n1 = Yh((n, e) => Fp(n, e, s1(e)), 0);
 
 function Jh(n, e) {
     let t = n.languageDataAt("commentTokens", e);
     return t.length ? t[0] : {}
 }
 const Qr = 50;
 
-function n1(n, {
+function r1(n, {
     open: e,
     close: t
 }, i, r) {
     let s = n.sliceDoc(i - Qr, i),
         o = n.sliceDoc(r, r + Qr),
         l = /\s*$/.exec(s)[0].length,
         h = /^\s*/.exec(o)[0].length,
@@ -15079,32 +15079,32 @@
             margin: l && 1
         },
         close: {
             pos: r + h,
             margin: h && 1
         }
     };
-    let u, g;
-    r - i <= 2 * Qr ? u = g = n.sliceDoc(i, r) : (u = n.sliceDoc(i, i + Qr), g = n.sliceDoc(r - Qr, r));
+    let u, m;
+    r - i <= 2 * Qr ? u = m = n.sliceDoc(i, r) : (u = n.sliceDoc(i, i + Qr), m = n.sliceDoc(r - Qr, r));
     let y = /^\s*/.exec(u)[0].length,
-        k = /\s*$/.exec(g)[0].length,
-        v = g.length - k - t.length;
-    return u.slice(y, y + e.length) == e && g.slice(v, v + t.length) == t ? {
+        k = /\s*$/.exec(m)[0].length,
+        v = m.length - k - t.length;
+    return u.slice(y, y + e.length) == e && m.slice(v, v + t.length) == t ? {
         open: {
             pos: i + y + e.length,
             margin: /\s/.test(u.charAt(y + e.length)) ? 1 : 0
         },
         close: {
             pos: r - k - t.length,
-            margin: /\s/.test(g.charAt(v - 1)) ? 1 : 0
+            margin: /\s/.test(m.charAt(v - 1)) ? 1 : 0
         }
     } : null
 }
 
-function r1(n) {
+function s1(n) {
     let e = [];
     for (let t of n.selection.ranges) {
         let i = n.doc.lineAt(t.from),
             r = t.to <= i.to ? i : n.doc.lineAt(t.to),
             s = e.length - 1;
         s >= 0 && e[s].to > i.from ? e[s].to = r.to : e.push({
             from: i.from + /^\s*/.exec(i.text)[0].length,
@@ -15113,15 +15113,15 @@
     }
     return e
 }
 
 function Fp(n, e, t = e.selection.ranges) {
     let i = t.map(s => Jh(e, s.from).block);
     if (!i.every(s => s)) return null;
-    let r = t.map((s, o) => n1(e, i[o], s.from, s.to));
+    let r = t.map((s, o) => r1(e, i[o], s.from, s.to));
     if (n != 2 && !r.every(s => s)) return {
         changes: e.changes(t.map((s, o) => r[o] ? [] : [{
             from: s.from,
             insert: i[o].open + " "
         }, {
             from: s.to,
             insert: " " + i[o].close
@@ -15146,59 +15146,59 @@
             } return {
             changes: s
         }
     }
     return null
 }
 
-function s1(n, e, t = e.selection.ranges) {
+function o1(n, e, t = e.selection.ranges) {
     let i = [],
         r = -1;
     for (let {
             from: s,
             to: o
         }
         of t) {
         let l = i.length,
             h = 1e9,
             f = Jh(e, s).line;
         if (f) {
             for (let u = s; u <= o;) {
-                let g = e.doc.lineAt(u);
-                if (g.from > r && (s == o || o > g.from)) {
-                    r = g.from;
-                    let y = /^\s*/.exec(g.text)[0].length,
-                        k = y == g.length,
-                        v = g.text.slice(y, y + f.length) == f ? y : -1;
-                    y < g.text.length && y < h && (h = y), i.push({
-                        line: g,
+                let m = e.doc.lineAt(u);
+                if (m.from > r && (s == o || o > m.from)) {
+                    r = m.from;
+                    let y = /^\s*/.exec(m.text)[0].length,
+                        k = y == m.length,
+                        v = m.text.slice(y, y + f.length) == f ? y : -1;
+                    y < m.text.length && y < h && (h = y), i.push({
+                        line: m,
                         comment: v,
                         token: f,
                         indent: y,
                         empty: k,
                         single: !1
                     })
                 }
-                u = g.to + 1
+                u = m.to + 1
             }
             if (h < 1e9)
                 for (let u = l; u < i.length; u++) i[u].indent < i[u].line.text.length && (i[u].indent = h);
             i.length == l + 1 && (i[l].single = !0)
         }
     }
     if (n != 2 && i.some(s => s.comment < 0 && (!s.empty || s.single))) {
         let s = [];
         for (let {
                 line: l,
                 token: h,
                 indent: f,
                 empty: u,
-                single: g
+                single: m
             }
-            of i)(g || !u) && s.push({
+            of i)(m || !u) && s.push({
             from: l.from + f,
             insert: h + " "
         });
         let o = e.changes(s);
         return {
             changes: o,
             selection: e.selection.map(o, 1)
@@ -15221,16 +15221,16 @@
             } return {
             changes: s
         }
     }
     return null
 }
 const yh = Xi.define(),
-    o1 = Xi.define(),
-    l1 = Z.define(),
+    l1 = Xi.define(),
+    a1 = Z.define(),
     zp = Z.define({
         combine(n) {
             return Hi(n, {
                 minDepth: 100,
                 newGroupDelay: 500,
                 joinToEvent: (e, t) => t
             }, {
@@ -15249,15 +15249,15 @@
                 i = e.annotation(yh);
             if (i) {
                 let h = _t.fromTransaction(e, i.selection),
                     f = i.side,
                     u = f == 0 ? n.undone : n.done;
                 return h ? u = el(u, u.length, t.minDepth, h) : u = jp(u, e.startState.selection), new Ni(f == 0 ? i.rest : u, f == 0 ? u : i.rest)
             }
-            let r = e.annotation(o1);
+            let r = e.annotation(l1);
             if ((r == "full" || r == "before") && (n = n.isolate()), e.annotation(nt.addToHistory) === !1) return e.changes.empty ? n : n.addMapping(e.changes.desc);
             let s = _t.fromTransaction(e),
                 o = e.annotation(nt.time),
                 l = e.annotation(nt.userEvent);
             return s ? n = n.addChanges(s, o, l, t, e) : e.selection && (n = n.addSelection(e.startState.selection, o, l, t.newGroupDelay)), (r == "full" || r == "after") && (n = n.isolate()), n
         },
         toJSON(n) {
@@ -15267,15 +15267,15 @@
             }
         },
         fromJSON(n) {
             return new Ni(n.done.map(_t.fromJSON), n.undone.map(_t.fromJSON))
         }
     });
 
-function a1(n = {}) {
+function h1(n = {}) {
     return [$p, zp.of(n), te.domEventHandlers({
         beforeinput(e, t) {
             let i = e.inputType == "historyUndo" ? Wp : e.inputType == "historyRedo" ? bh : null;
             return i ? (e.preventDefault(), i(t)) : !1
         }
     })]
 }
@@ -15290,16 +15290,16 @@
         if (!r) return !1;
         let s = r.pop(n, t, e);
         return s ? (i(s), !0) : !1
     }
 }
 const Wp = Cl(0, !1),
     bh = Cl(1, !1),
-    h1 = Cl(0, !0),
-    c1 = Cl(1, !0);
+    c1 = Cl(0, !0),
+    f1 = Cl(1, !0);
 class _t {
     constructor(e, t, i, r, s) {
         this.changes = e, this.effects = t, this.mapped = i, this.startSelection = r, this.selectionsAfter = s
     }
     setSelAfter(e) {
         return new _t(this.changes, this.effects, this.mapped, this.startSelection, e)
     }
@@ -15313,15 +15313,15 @@
         }
     }
     static fromJSON(e) {
         return new _t(e.changes && it.fromJSON(e.changes), [], e.mapped && _i.fromJSON(e.mapped), e.startSelection && H.fromJSON(e.startSelection), e.selectionsAfter.map(H.fromJSON))
     }
     static fromTransaction(e, t) {
         let i = ii;
-        for (let r of e.startState.facet(l1)) {
+        for (let r of e.startState.facet(a1)) {
             let s = r(e);
             s.length && (i = i.concat(s))
         }
         return !i.length && e.changes.empty ? null : new _t(e.changes.invert(e.startState.doc), i, void 0, t || e.startState.selection, ii)
     }
     static selection(e) {
         return new _t(void 0, ii, void 0, void 0, e)
@@ -15330,102 +15330,102 @@
 
 function el(n, e, t, i) {
     let r = e + 1 > t + 20 ? e - t - 1 : 0,
         s = n.slice(r, e);
     return s.push(i), s
 }
 
-function f1(n, e) {
+function u1(n, e) {
     let t = [],
         i = !1;
     return n.iterChangedRanges((r, s) => t.push(r, s)), e.iterChangedRanges((r, s, o, l) => {
         for (let h = 0; h < t.length;) {
             let f = t[h++],
                 u = t[h++];
             l >= f && o <= u && (i = !0)
         }
     }), i
 }
 
-function u1(n, e) {
+function d1(n, e) {
     return n.ranges.length == e.ranges.length && n.ranges.filter((t, i) => t.empty != e.ranges[i].empty).length === 0
 }
 
 function qp(n, e) {
     return n.length ? e.length ? n.concat(e) : n : e
 }
 const ii = [],
-    d1 = 200;
+    p1 = 200;
 
 function jp(n, e) {
     if (n.length) {
         let t = n[n.length - 1],
-            i = t.selectionsAfter.slice(Math.max(0, t.selectionsAfter.length - d1));
+            i = t.selectionsAfter.slice(Math.max(0, t.selectionsAfter.length - p1));
         return i.length && i[i.length - 1].eq(e) ? n : (i.push(e), el(n, n.length - 1, 1e9, t.setSelAfter(i)))
     } else return [_t.selection([e])]
 }
 
-function p1(n) {
+function g1(n) {
     let e = n[n.length - 1],
         t = n.slice();
     return t[n.length - 1] = e.setSelAfter(e.selectionsAfter.slice(0, e.selectionsAfter.length - 1)), t
 }
 
 function ba(n, e) {
     if (!n.length) return n;
     let t = n.length,
         i = ii;
     for (; t;) {
-        let r = g1(n[t - 1], e, i);
+        let r = m1(n[t - 1], e, i);
         if (r.changes && !r.changes.empty || r.effects.length) {
             let s = n.slice(0, t);
             return s[t - 1] = r, s
         } else e = r.mapped, t--, i = r.selectionsAfter
     }
     return i.length ? [_t.selection(i)] : ii
 }
 
-function g1(n, e, t) {
+function m1(n, e, t) {
     let i = qp(n.selectionsAfter.length ? n.selectionsAfter.map(l => l.map(e)) : ii, t);
     if (!n.changes) return _t.selection(i);
     let r = n.changes.map(e),
         s = e.mapDesc(n.changes, !0),
         o = n.mapped ? n.mapped.composeDesc(s) : s;
     return new _t(r, me.mapEffects(n.effects, e), o, n.startSelection.map(s), i)
 }
-const m1 = /^(input\.type|delete)($|\.)/;
+const y1 = /^(input\.type|delete)($|\.)/;
 class Ni {
     constructor(e, t, i = 0, r = void 0) {
         this.done = e, this.undone = t, this.prevTime = i, this.prevUserEvent = r
     }
     isolate() {
         return this.prevTime ? new Ni(this.done, this.undone) : this
     }
     addChanges(e, t, i, r, s) {
         let o = this.done,
             l = o[o.length - 1];
-        return l && l.changes && !l.changes.empty && e.changes && (!i || m1.test(i)) && (!l.selectionsAfter.length && t - this.prevTime < r.newGroupDelay && r.joinToEvent(s, f1(l.changes, e.changes)) || i == "input.type.compose") ? o = el(o, o.length - 1, r.minDepth, new _t(e.changes.compose(l.changes), qp(e.effects, l.effects), l.mapped, l.startSelection, ii)) : o = el(o, o.length, r.minDepth, e), new Ni(o, ii, t, i)
+        return l && l.changes && !l.changes.empty && e.changes && (!i || y1.test(i)) && (!l.selectionsAfter.length && t - this.prevTime < r.newGroupDelay && r.joinToEvent(s, u1(l.changes, e.changes)) || i == "input.type.compose") ? o = el(o, o.length - 1, r.minDepth, new _t(e.changes.compose(l.changes), qp(e.effects, l.effects), l.mapped, l.startSelection, ii)) : o = el(o, o.length, r.minDepth, e), new Ni(o, ii, t, i)
     }
     addSelection(e, t, i, r) {
         let s = this.done.length ? this.done[this.done.length - 1].selectionsAfter : ii;
-        return s.length > 0 && t - this.prevTime < r && i == this.prevUserEvent && i && /^select($|\.)/.test(i) && u1(s[s.length - 1], e) ? this : new Ni(jp(this.done, e), this.undone, t, i)
+        return s.length > 0 && t - this.prevTime < r && i == this.prevUserEvent && i && /^select($|\.)/.test(i) && d1(s[s.length - 1], e) ? this : new Ni(jp(this.done, e), this.undone, t, i)
     }
     addMapping(e) {
         return new Ni(ba(this.done, e), ba(this.undone, e), this.prevTime, this.prevUserEvent)
     }
     pop(e, t, i) {
         let r = e == 0 ? this.done : this.undone;
         if (r.length == 0) return null;
         let s = r[r.length - 1],
             o = s.selectionsAfter[0] || t.selection;
         if (i && s.selectionsAfter.length) return t.update({
             selection: s.selectionsAfter[s.selectionsAfter.length - 1],
             annotations: yh.of({
                 side: e,
-                rest: p1(r),
+                rest: g1(r),
                 selection: o
             }),
             userEvent: e == 0 ? "select.undo" : "select.redo",
             scrollIntoView: !0
         });
         if (s.changes) {
             let l = r.length == 1 ? ii : r.slice(0, r.length - 1);
@@ -15442,35 +15442,35 @@
                 userEvent: e == 0 ? "undo" : "redo",
                 scrollIntoView: !0
             })
         } else return null
     }
 }
 Ni.empty = new Ni(ii, ii);
-const y1 = [{
+const b1 = [{
     key: "Mod-z",
     run: Wp,
     preventDefault: !0
 }, {
     key: "Mod-y",
     mac: "Mod-Shift-z",
     run: bh,
     preventDefault: !0
 }, {
     linux: "Ctrl-Shift-z",
     run: bh,
     preventDefault: !0
 }, {
     key: "Mod-u",
-    run: h1,
+    run: c1,
     preventDefault: !0
 }, {
     key: "Alt-u",
     mac: "Mod-Shift-u",
-    run: c1,
+    run: f1,
     preventDefault: !0
 }];
 
 function Tr(n, e) {
     return H.create(n.ranges.map(e), n.mainIndex)
 }
 
@@ -15503,37 +15503,37 @@
 }
 const Up = n => Vp(n, !At(n)),
     Qp = n => Vp(n, At(n));
 
 function Gp(n, e) {
     return mi(n, t => t.empty ? n.moveByGroup(t, e) : Al(t, e))
 }
-const b1 = n => Gp(n, !At(n)),
-    x1 = n => Gp(n, At(n));
+const x1 = n => Gp(n, !At(n)),
+    k1 = n => Gp(n, At(n));
 
-function k1(n, e, t) {
+function w1(n, e, t) {
     if (e.type.prop(t)) return !0;
     let i = e.to - e.from;
     return i && (i > 2 || /[^\s,.;:]/.test(n.sliceDoc(e.from, e.to))) || e.firstChild
 }
 
 function Tl(n, e, t) {
     let i = lt(n).resolveInner(e.head),
         r = t ? Se.closedBy : Se.openedBy;
     for (let h = e.head;;) {
         let f = t ? i.childAfter(h) : i.childBefore(h);
         if (!f) break;
-        k1(n, f, r) ? i = f : h = t ? f.to : f.from
+        w1(n, f, r) ? i = f : h = t ? f.to : f.from
     }
     let s = i.type.prop(r),
         o, l;
     return s && (o = t ? Pi(n, i.from, 1) : Pi(n, i.to, -1)) && o.matched ? l = t ? o.end.to : o.end.from : l = t ? i.to : i.from, H.cursor(l, t ? -1 : 1)
 }
-const w1 = n => mi(n, e => Tl(n.state, e, !At(n))),
-    v1 = n => mi(n, e => Tl(n.state, e, At(n)));
+const v1 = n => mi(n, e => Tl(n.state, e, !At(n))),
+    S1 = n => mi(n, e => Tl(n.state, e, At(n)));
 
 function Kp(n, e) {
     return mi(n, t => {
         if (!t.empty) return Al(t, e);
         let i = n.moveVertically(t, e);
         return i.head != t.head ? i : n.moveToLineBoundary(t, e)
     })
@@ -15591,36 +15591,36 @@
         r = n.moveToLineBoundary(e, t);
     if (r.head == e.head && r.head != (t ? i.to : i.from) && (r = n.moveToLineBoundary(e, t, !1)), !t && r.head == i.from && i.length) {
         let s = /^\s*/.exec(n.state.sliceDoc(i.from, Math.min(i.from + 100, i.to)))[0].length;
         s && e.head != i.from + s && (r = H.cursor(i.from + s))
     }
     return r
 }
-const S1 = n => mi(n, e => Tn(n, e, !0)),
-    C1 = n => mi(n, e => Tn(n, e, !1)),
-    A1 = n => mi(n, e => Tn(n, e, !At(n))),
-    T1 = n => mi(n, e => Tn(n, e, At(n))),
-    O1 = n => mi(n, e => H.cursor(n.lineBlockAt(e.head).from, 1)),
-    M1 = n => mi(n, e => H.cursor(n.lineBlockAt(e.head).to, -1));
+const C1 = n => mi(n, e => Tn(n, e, !0)),
+    A1 = n => mi(n, e => Tn(n, e, !1)),
+    T1 = n => mi(n, e => Tn(n, e, !At(n))),
+    O1 = n => mi(n, e => Tn(n, e, At(n))),
+    M1 = n => mi(n, e => H.cursor(n.lineBlockAt(e.head).from, 1)),
+    E1 = n => mi(n, e => H.cursor(n.lineBlockAt(e.head).to, -1));
 
-function E1(n, e, t) {
+function D1(n, e, t) {
     let i = !1,
         r = Tr(n.selection, s => {
             let o = Pi(n, s.head, -1) || Pi(n, s.head, 1) || s.head > 0 && Pi(n, s.head - 1, 1) || s.head < n.doc.length && Pi(n, s.head + 1, -1);
             if (!o || !o.end) return s;
             i = !0;
             let l = o.start.from == s.head ? o.end.to : o.end.from;
             return t ? H.range(s.anchor, l) : H.cursor(l)
         });
     return i ? (e(Fi(n, r)), !0) : !1
 }
-const D1 = ({
+const R1 = ({
     state: n,
     dispatch: e
-}) => E1(n, e, !1);
+}) => D1(n, e, !1);
 
 function li(n, e) {
     let t = Tr(n.state.selection, i => {
         let r = e(i);
         return H.range(i.anchor, r.head, r.goalColumn, r.bidiLevel || void 0)
     });
     return t.eq(n.state.selection) ? !1 : (n.dispatch(Fi(n.state, t)), !0)
@@ -15631,36 +15631,36 @@
 }
 const tg = n => eg(n, !At(n)),
     ig = n => eg(n, At(n));
 
 function ng(n, e) {
     return li(n, t => n.moveByGroup(t, e))
 }
-const R1 = n => ng(n, !At(n)),
-    L1 = n => ng(n, At(n)),
-    P1 = n => li(n, e => Tl(n.state, e, !At(n))),
-    N1 = n => li(n, e => Tl(n.state, e, At(n)));
+const L1 = n => ng(n, !At(n)),
+    P1 = n => ng(n, At(n)),
+    N1 = n => li(n, e => Tl(n.state, e, !At(n))),
+    I1 = n => li(n, e => Tl(n.state, e, At(n)));
 
 function rg(n, e) {
     return li(n, t => n.moveVertically(t, e))
 }
 const sg = n => rg(n, !1),
     og = n => rg(n, !0);
 
 function lg(n, e) {
     return li(n, t => n.moveVertically(t, e, Jp(n).height))
 }
 const Yf = n => lg(n, !1),
     Jf = n => lg(n, !0),
-    I1 = n => li(n, e => Tn(n, e, !0)),
-    B1 = n => li(n, e => Tn(n, e, !1)),
-    _1 = n => li(n, e => Tn(n, e, !At(n))),
-    H1 = n => li(n, e => Tn(n, e, At(n))),
-    F1 = n => li(n, e => H.cursor(n.lineBlockAt(e.head).from)),
-    z1 = n => li(n, e => H.cursor(n.lineBlockAt(e.head).to)),
+    B1 = n => li(n, e => Tn(n, e, !0)),
+    _1 = n => li(n, e => Tn(n, e, !1)),
+    H1 = n => li(n, e => Tn(n, e, !At(n))),
+    F1 = n => li(n, e => Tn(n, e, At(n))),
+    z1 = n => li(n, e => H.cursor(n.lineBlockAt(e.head).from)),
+    $1 = n => li(n, e => H.cursor(n.lineBlockAt(e.head).to)),
     Zf = ({
         state: n,
         dispatch: e
     }) => (e(Fi(n, {
         anchor: 0
     })), !0),
     eu = ({
@@ -15679,38 +15679,38 @@
     iu = ({
         state: n,
         dispatch: e
     }) => (e(Fi(n, {
         anchor: n.selection.main.anchor,
         head: n.doc.length
     })), !0),
-    $1 = ({
+    W1 = ({
         state: n,
         dispatch: e
     }) => (e(n.update({
         selection: {
             anchor: 0,
             head: n.doc.length
         },
         userEvent: "select"
     })), !0),
-    W1 = ({
+    q1 = ({
         state: n,
         dispatch: e
     }) => {
         let t = Ol(n).map(({
             from: i,
             to: r
         }) => H.range(i, Math.min(r + 1, n.doc.length)));
         return e(n.update({
             selection: H.create(t),
             userEvent: "select"
         })), !0
     },
-    q1 = ({
+    j1 = ({
         state: n,
         dispatch: e
     }) => {
         let t = Tr(n.selection, i => {
             var r;
             let s = lt(n).resolveStack(i.from, 1);
             for (let o = s; o; o = o.next) {
@@ -15719,15 +15719,15 @@
                 } = o;
                 if ((l.from < i.from && l.to >= i.to || l.to > i.to && l.from <= i.from) && (!((r = l.parent) === null || r === void 0) && r.parent)) return H.range(l.to, l.from)
             }
             return i
         });
         return e(Fi(n, t)), !0
     },
-    j1 = ({
+    V1 = ({
         state: n,
         dispatch: e
     }) => {
         let t = n.selection,
             i = null;
         return t.ranges.length > 1 ? i = H.create([t.main]) : t.main.empty || (i = H.create([H.cursor(t.main.head)])), i ? (e(Fi(n, i)), !0) : !1
     };
@@ -15806,28 +15806,28 @@
                 u = o(f);
             if (l != null && u != l) break;
             (f != " " || i != t.head) && (l = u), i = h
         }
         return i
     }),
     fg = n => cg(n, !1),
-    V1 = n => cg(n, !0),
-    U1 = n => Ls(n, e => {
+    U1 = n => cg(n, !0),
+    Q1 = n => Ls(n, e => {
         let t = n.lineBlockAt(e.head).to;
         return e.head < t ? t : Math.min(n.state.doc.length, e.head + 1)
     }),
-    Q1 = n => Ls(n, e => {
+    G1 = n => Ls(n, e => {
         let t = n.moveToLineBoundary(e, !1).head;
         return e.head > t ? t : Math.max(0, e.head - 1)
     }),
-    G1 = n => Ls(n, e => {
+    K1 = n => Ls(n, e => {
         let t = n.moveToLineBoundary(e, !0).head;
         return e.head < t ? t : Math.min(n.state.doc.length, e.head + 1)
     }),
-    K1 = ({
+    X1 = ({
         state: n,
         dispatch: e
     }) => {
         if (n.readOnly) return !1;
         let t = n.changeByRange(i => ({
             changes: {
                 from: i.from,
@@ -15837,15 +15837,15 @@
             range: H.cursor(i.from)
         }));
         return e(n.update(t, {
             scrollIntoView: !0,
             userEvent: "input"
         })), !0
     },
-    X1 = ({
+    Y1 = ({
         state: n,
         dispatch: e
     }) => {
         if (n.readOnly) return !1;
         let t = n.changeByRange(i => {
             if (!i.empty || i.from == 0 || i.from == n.doc.length) return {
                 range: i
@@ -15919,19 +15919,19 @@
     return i.length ? (e(n.update({
         changes: i,
         scrollIntoView: !0,
         selection: H.create(r, n.selection.mainIndex),
         userEvent: "move.line"
     })), !0) : !1
 }
-const Y1 = ({
+const J1 = ({
         state: n,
         dispatch: e
     }) => ug(n, e, !1),
-    J1 = ({
+    Z1 = ({
         state: n,
         dispatch: e
     }) => ug(n, e, !0);
 
 function dg(n, e, t) {
     if (n.readOnly) return !1;
     let i = [];
@@ -15944,23 +15944,23 @@
     });
     return e(n.update({
         changes: i,
         scrollIntoView: !0,
         userEvent: "input.copyline"
     })), !0
 }
-const Z1 = ({
+const ek = ({
         state: n,
         dispatch: e
     }) => dg(n, e, !1),
-    ek = ({
+    tk = ({
         state: n,
         dispatch: e
     }) => dg(n, e, !0),
-    tk = n => {
+    ik = n => {
         if (n.state.readOnly) return !1;
         let {
             state: e
         } = n, t = e.changes(Ol(e).map(({
             from: r,
             to: s
         }) => (r > 0 ? r-- : s < e.doc.length && s++, {
@@ -15971,61 +15971,61 @@
             changes: t,
             selection: i,
             scrollIntoView: !0,
             userEvent: "delete.line"
         }), !0
     };
 
-function ik(n, e) {
+function nk(n, e) {
     if (/\(\)|\[\]|\{\}/.test(n.sliceDoc(e - 1, e + 1))) return {
         from: e,
         to: e
     };
     let t = lt(n).resolveInner(e),
         i = t.childBefore(e),
         r = t.childAfter(e),
         s;
     return i && r && i.to <= e && r.from >= e && (s = i.type.prop(Se.closedBy)) && s.indexOf(r.name) > -1 && n.doc.lineAt(i.to).from == n.doc.lineAt(r.from).from && !/\S/.test(n.sliceDoc(i.to, r.from)) ? {
         from: i.to,
         to: r.from
     } : null
 }
-const nk = pg(!1),
-    rk = pg(!0);
+const rk = pg(!1),
+    sk = pg(!0);
 
 function pg(n) {
     return ({
         state: e,
         dispatch: t
     }) => {
         if (e.readOnly) return !1;
         let i = e.changeByRange(r => {
             let {
                 from: s,
                 to: o
-            } = r, l = e.doc.lineAt(s), h = !n && s == o && ik(e, s);
+            } = r, l = e.doc.lineAt(s), h = !n && s == o && nk(e, s);
             n && (s = o = (o <= l.to ? l : e.doc.lineAt(o)).to);
             let f = new wl(e, {
                     simulateBreak: s,
                     simulateDoubleBreak: !!h
                 }),
                 u = Gh(f, s);
             for (u == null && (u = Os(/^\s*/.exec(e.doc.lineAt(s).text)[0], e.tabSize)); o < l.to && /\s/.test(l.text[o - l.from]);) o++;
             h ? {
                 from: s,
                 to: o
             } = h : s > l.from && s < l.from + 100 && !/\S/.test(l.text.slice(0, s)) && (s = l.from);
-            let g = ["", ws(e, u)];
-            return h && g.push(ws(e, f.lineIndent(l.from, -1))), {
+            let m = ["", ws(e, u)];
+            return h && m.push(ws(e, f.lineIndent(l.from, -1))), {
                 changes: {
                     from: s,
                     to: o,
-                    insert: De.of(g)
+                    insert: De.of(m)
                 },
-                range: H.cursor(s + 1 + g[1].length)
+                range: H.cursor(s + 1 + m[1].length)
             }
         });
         return t(e.update(i, {
             scrollIntoView: !0,
             userEvent: "input"
         })), !0
     }
@@ -16042,15 +16042,15 @@
         let s = n.changes(r);
         return {
             changes: r,
             range: H.range(s.mapPos(i.anchor, 1), s.mapPos(i.head, 1))
         }
     })
 }
-const sk = ({
+const ok = ({
         state: n,
         dispatch: e
     }) => {
         if (n.readOnly) return !1;
         let t = Object.create(null),
             i = new wl(n, {
                 overrideIndentation: s => {
@@ -16070,26 +16070,26 @@
                     insert: u
                 }))
             });
         return r.changes.empty || e(n.update(r, {
             userEvent: "indent"
         })), !0
     },
-    ok = ({
+    lk = ({
         state: n,
         dispatch: e
     }) => n.readOnly ? !1 : (e(n.update(Zh(n, (t, i) => {
         i.push({
             from: t.from,
             insert: n.facet(Qh)
         })
     }), {
         userEvent: "input.indent"
     })), !0),
-    lk = ({
+    ak = ({
         state: n,
         dispatch: e
     }) => n.readOnly ? !1 : (e(n.update(Zh(n, (t, i) => {
         let r = /^\s*/.exec(t.text)[0];
         if (!r) return;
         let s = Os(r, n.tabSize),
             o = 0,
@@ -16099,15 +16099,15 @@
             from: t.from + o,
             to: t.from + r.length,
             insert: l.slice(o)
         })
     }), {
         userEvent: "delete.dedent"
     })), !0),
-    ak = [{
+    hk = [{
         key: "Ctrl-b",
         run: Up,
         shift: tg,
         preventDefault: !0
     }, {
         key: "Ctrl-f",
         run: Qp,
@@ -16118,73 +16118,73 @@
         shift: sg
     }, {
         key: "Ctrl-n",
         run: Yp,
         shift: og
     }, {
         key: "Ctrl-a",
-        run: O1,
-        shift: F1
-    }, {
-        key: "Ctrl-e",
         run: M1,
         shift: z1
     }, {
+        key: "Ctrl-e",
+        run: E1,
+        shift: $1
+    }, {
         key: "Ctrl-d",
         run: hg
     }, {
         key: "Ctrl-h",
         run: kh
     }, {
         key: "Ctrl-k",
-        run: U1
+        run: Q1
     }, {
         key: "Ctrl-Alt-h",
         run: fg
     }, {
         key: "Ctrl-o",
-        run: K1
+        run: X1
     }, {
         key: "Ctrl-t",
-        run: X1
+        run: Y1
     }, {
         key: "Ctrl-v",
         run: xh
     }],
-    hk = [{
+    ck = [{
         key: "ArrowLeft",
         run: Up,
         shift: tg,
         preventDefault: !0
     }, {
         key: "Mod-ArrowLeft",
         mac: "Alt-ArrowLeft",
-        run: b1,
-        shift: R1,
+        run: x1,
+        shift: L1,
         preventDefault: !0
     }, {
         mac: "Cmd-ArrowLeft",
-        run: A1,
-        shift: _1,
+        run: T1,
+        shift: H1,
         preventDefault: !0
     }, {
         key: "ArrowRight",
         run: Qp,
         shift: ig,
         preventDefault: !0
     }, {
         key: "Mod-ArrowRight",
         mac: "Alt-ArrowRight",
-        run: x1,
-        shift: L1,
+        run: k1,
+        shift: P1,
         preventDefault: !0
     }, {
         mac: "Cmd-ArrowRight",
-        run: T1,
-        shift: H1,
+        run: O1,
+        shift: F1,
         preventDefault: !0
     }, {
         key: "ArrowUp",
         run: Xp,
         shift: sg,
         preventDefault: !0
     }, {
@@ -16214,120 +16214,120 @@
         shift: Yf
     }, {
         key: "PageDown",
         run: xh,
         shift: Jf
     }, {
         key: "Home",
-        run: C1,
-        shift: B1,
+        run: A1,
+        shift: _1,
         preventDefault: !0
     }, {
         key: "Mod-Home",
         run: Zf,
         shift: tu
     }, {
         key: "End",
-        run: S1,
-        shift: I1,
+        run: C1,
+        shift: B1,
         preventDefault: !0
     }, {
         key: "Mod-End",
         run: eu,
         shift: iu
     }, {
         key: "Enter",
-        run: nk
+        run: rk
     }, {
         key: "Mod-a",
-        run: $1
+        run: W1
     }, {
         key: "Backspace",
         run: kh,
         shift: kh
     }, {
         key: "Delete",
         run: hg
     }, {
         key: "Mod-Backspace",
         mac: "Alt-Backspace",
         run: fg
     }, {
         key: "Mod-Delete",
         mac: "Alt-Delete",
-        run: V1
+        run: U1
     }, {
         mac: "Mod-Backspace",
-        run: Q1
+        run: G1
     }, {
         mac: "Mod-Delete",
-        run: G1
-    }].concat(ak.map(n => ({
+        run: K1
+    }].concat(hk.map(n => ({
         mac: n.key,
         run: n.run,
         shift: n.shift
     }))),
-    ck = [{
+    fk = [{
         key: "Alt-ArrowLeft",
         mac: "Ctrl-ArrowLeft",
-        run: w1,
-        shift: P1
+        run: v1,
+        shift: N1
     }, {
         key: "Alt-ArrowRight",
         mac: "Ctrl-ArrowRight",
-        run: v1,
-        shift: N1
+        run: S1,
+        shift: I1
     }, {
         key: "Alt-ArrowUp",
-        run: Y1
+        run: J1
     }, {
         key: "Shift-Alt-ArrowUp",
-        run: Z1
+        run: ek
     }, {
         key: "Alt-ArrowDown",
-        run: J1
+        run: Z1
     }, {
         key: "Shift-Alt-ArrowDown",
-        run: ek
+        run: tk
     }, {
         key: "Escape",
-        run: j1
+        run: V1
     }, {
         key: "Mod-Enter",
-        run: rk
+        run: sk
     }, {
         key: "Alt-l",
         mac: "Ctrl-l",
-        run: W1
+        run: q1
     }, {
         key: "Mod-i",
-        run: q1,
+        run: j1,
         preventDefault: !0
     }, {
         key: "Mod-[",
-        run: lk
+        run: ak
     }, {
         key: "Mod-]",
-        run: ok
+        run: lk
     }, {
         key: "Mod-Alt-\\",
-        run: sk
+        run: ok
     }, {
         key: "Shift-Mod-k",
-        run: tk
+        run: ik
     }, {
         key: "Shift-Mod-\\",
-        run: D1
+        run: R1
     }, {
         key: "Mod-/",
-        run: Zx
+        run: e1
     }, {
         key: "Alt-A",
-        run: t1
-    }].concat(hk);
+        run: i1
+    }].concat(ck);
 
 function $e() {
     var n = arguments[0];
     typeof n == "string" && (n = document.createElement(n));
     var e = 1,
         t = arguments[1];
     if (t && typeof t == "object" && t.nodeType == null && !Array.isArray(t)) {
@@ -16490,15 +16490,15 @@
         }
     }
 }
 typeof Symbol != "undefined" && (yg.prototype[Symbol.iterator] = bg.prototype[Symbol.iterator] = function() {
     return this
 });
 
-function fk(n) {
+function uk(n) {
     try {
         return new RegExp(n, ec), !0
     } catch (e) {
         return !1
     }
 }
 
@@ -16533,26 +16533,26 @@
         }, n.state.phrase("go")));
 
     function r() {
         let s = /^([+-])?(\d+)?(:\d+)?(%)?$/.exec(t.value);
         if (!s) return;
         let {
             state: o
-        } = n, l = o.doc.lineAt(o.selection.main.head), [, h, f, u, g] = s, y = u ? +u.slice(1) : 0, k = f ? +f : l.number;
-        if (f && g) {
+        } = n, l = o.doc.lineAt(o.selection.main.head), [, h, f, u, m] = s, y = u ? +u.slice(1) : 0, k = f ? +f : l.number;
+        if (f && m) {
             let O = k / 100;
             h && (O = O * (h == "-" ? -1 : 1) + l.number / o.doc.lines), k = Math.round(o.doc.lines * O)
         } else f && h && (k = k * (h == "-" ? -1 : 1) + l.number);
         let v = o.doc.line(Math.max(1, Math.min(o.doc.lines, k))),
-            C = H.cursor(v.from + Math.max(0, Math.min(y, v.length)));
+            A = H.cursor(v.from + Math.max(0, Math.min(y, v.length)));
         n.dispatch({
-            effects: [il.of(!1), te.scrollIntoView(C.from, {
+            effects: [il.of(!1), te.scrollIntoView(A.from, {
                 y: "center"
             })],
-            selection: C
+            selection: A
         }), n.focus()
     }
     return {
         dom: i
     }
 }
 const il = me.define(),
@@ -16562,67 +16562,67 @@
         },
         update(n, e) {
             for (let t of e.effects) t.is(il) && (n = t.value);
             return n
         },
         provide: n => xs.from(n, e => e ? wh : null)
     }),
-    uk = n => {
+    dk = n => {
         let e = bs(n, wh);
         if (!e) {
             let t = [il.of(!0)];
-            n.state.field(ru, !1) == null && t.push(me.appendConfig.of([ru, dk])), n.dispatch({
+            n.state.field(ru, !1) == null && t.push(me.appendConfig.of([ru, pk])), n.dispatch({
                 effects: t
             }), e = bs(n, wh)
         }
         return e && e.dom.querySelector("input").select(), !0
     },
-    dk = te.baseTheme({
+    pk = te.baseTheme({
         ".cm-panel.cm-gotoLine": {
             padding: "2px 6px 4px",
             "& label": {
                 fontSize: "80%"
             }
         }
     }),
-    pk = {
+    gk = {
         highlightWordAroundCursor: !1,
         minSelectionLength: 1,
         maxMatches: 100,
         wholeWords: !1
     },
     xg = Z.define({
         combine(n) {
-            return Hi(n, pk, {
+            return Hi(n, gk, {
                 highlightWordAroundCursor: (e, t) => e || t,
                 minSelectionLength: Math.min,
                 maxMatches: Math.min
             })
         }
     });
 
-function gk(n) {
-    let e = [kk, xk];
+function mk(n) {
+    let e = [wk, kk];
     return n && e.push(xg.of(n)), e
 }
-const mk = de.mark({
+const yk = de.mark({
         class: "cm-selectionMatch"
     }),
-    yk = de.mark({
+    bk = de.mark({
         class: "cm-selectionMatch cm-selectionMatch-main"
     });
 
 function su(n, e, t, i) {
     return (t == 0 || n(e.sliceDoc(t - 1, t)) != Ve.Word) && (i == e.doc.length || n(e.sliceDoc(i, i + 1)) != Ve.Word)
 }
 
-function bk(n, e, t, i) {
+function xk(n, e, t, i) {
     return n(e.sliceDoc(t, t + 1)) == Ve.Word && n(e.sliceDoc(i - 1, i)) == Ve.Word
 }
-const xk = rt.fromClass(class {
+const kk = rt.fromClass(class {
         constructor(n) {
             this.decorations = this.getDeco(n)
         }
         update(n) {
             (n.selectionSet || n.docChanged || n.viewportChanged) && (this.decorations = this.getDeco(n.view))
         }
         getDeco(n) {
@@ -16639,54 +16639,54 @@
                 let h = t.wordAt(r.head);
                 if (!h) return de.none;
                 o = t.charCategorizer(r.head), s = t.sliceDoc(h.from, h.to)
             } else {
                 let h = r.to - r.from;
                 if (h < e.minSelectionLength || h > 200) return de.none;
                 if (e.wholeWords) {
-                    if (s = t.sliceDoc(r.from, r.to), o = t.charCategorizer(r.head), !(su(o, t, r.from, r.to) && bk(o, t, r.from, r.to))) return de.none
+                    if (s = t.sliceDoc(r.from, r.to), o = t.charCategorizer(r.head), !(su(o, t, r.from, r.to) && xk(o, t, r.from, r.to))) return de.none
                 } else if (s = t.sliceDoc(r.from, r.to).trim(), !s) return de.none
             }
             let l = [];
             for (let h of n.visibleRanges) {
                 let f = new Cr(t.doc, s, h.from, h.to);
                 for (; !f.next().done;) {
                     let {
                         from: u,
-                        to: g
+                        to: m
                     } = f.value;
-                    if ((!o || su(o, t, u, g)) && (r.empty && u <= r.from && g >= r.to ? l.push(yk.range(u, g)) : (u >= r.to || g <= r.from) && l.push(mk.range(u, g)), l.length > e.maxMatches)) return de.none
+                    if ((!o || su(o, t, u, m)) && (r.empty && u <= r.from && m >= r.to ? l.push(bk.range(u, m)) : (u >= r.to || m <= r.from) && l.push(yk.range(u, m)), l.length > e.maxMatches)) return de.none
                 }
             }
             return de.set(l)
         }
     }, {
         decorations: n => n.decorations
     }),
-    kk = te.baseTheme({
+    wk = te.baseTheme({
         ".cm-selectionMatch": {
             backgroundColor: "#99ff7780"
         },
         ".cm-searchMatch .cm-selectionMatch": {
             backgroundColor: "transparent"
         }
     }),
-    wk = ({
+    vk = ({
         state: n,
         dispatch: e
     }) => {
         let {
             selection: t
         } = n, i = H.create(t.ranges.map(r => n.wordAt(r.head) || H.cursor(r.head)), t.mainIndex);
         return i.eq(t) ? !1 : (e(n.update({
             selection: i
         })), !0)
     };
 
-function vk(n, e) {
+function Sk(n, e) {
     let {
         main: t,
         ranges: i
     } = n.selection, r = n.wordAt(t.head), s = r && r.from == t.from && r.to == t.to;
     for (let o = !1, l = new Cr(n.doc, e, i[i.length - 1].to);;)
         if (l.next(), l.done) {
             if (o) return null;
@@ -16696,59 +16696,59 @@
             if (s) {
                 let h = n.wordAt(l.value.from);
                 if (!h || h.from != l.value.from || h.to != l.value.to) continue
             }
             return l.value
         }
 }
-const Sk = ({
+const Ck = ({
         state: n,
         dispatch: e
     }) => {
         let {
             ranges: t
         } = n.selection;
-        if (t.some(s => s.from === s.to)) return wk({
+        if (t.some(s => s.from === s.to)) return vk({
             state: n,
             dispatch: e
         });
         let i = n.sliceDoc(t[0].from, t[0].to);
         if (n.selection.ranges.some(s => n.sliceDoc(s.from, s.to) != i)) return !1;
-        let r = vk(n, i);
+        let r = Sk(n, i);
         return r ? (e(n.update({
             selection: n.selection.addRange(H.range(r.from, r.to), !1),
             effects: te.scrollIntoView(r.to)
         })), !0) : !1
     },
     Or = Z.define({
         combine(n) {
             return Hi(n, {
                 top: !1,
                 caseSensitive: !1,
                 literal: !1,
                 regexp: !1,
                 wholeWord: !1,
-                createPanel: e => new Ik(e),
+                createPanel: e => new Bk(e),
                 scrollToMatch: e => te.scrollIntoView(e)
             })
         }
     });
 class kg {
     constructor(e) {
-        this.search = e.search, this.caseSensitive = !!e.caseSensitive, this.literal = !!e.literal, this.regexp = !!e.regexp, this.replace = e.replace || "", this.valid = !!this.search && (!this.regexp || fk(this.search)), this.unquoted = this.unquote(this.search), this.wholeWord = !!e.wholeWord
+        this.search = e.search, this.caseSensitive = !!e.caseSensitive, this.literal = !!e.literal, this.regexp = !!e.regexp, this.replace = e.replace || "", this.valid = !!this.search && (!this.regexp || uk(this.search)), this.unquoted = this.unquote(this.search), this.wholeWord = !!e.wholeWord
     }
     unquote(e) {
         return this.literal ? e : e.replace(/\\([nrt\\])/g, (t, i) => i == "n" ? `
 ` : i == "r" ? "\r" : i == "t" ? "	" : "\\")
     }
     eq(e) {
         return this.search == e.search && this.replace == e.replace && this.caseSensitive == e.caseSensitive && this.regexp == e.regexp && this.wholeWord == e.wholeWord
     }
     create() {
-        return this.regexp ? new Ok(this) : new Ak(this)
+        return this.regexp ? new Mk(this) : new Tk(this)
     }
     getCursor(e, t = 0, i) {
         let r = e.doc ? e : Ee.create({
             doc: e
         });
         return i == null && (i = r.doc.length), this.regexp ? cr(this, r, t, i) : hr(this, r, t, i)
     }
@@ -16756,21 +16756,21 @@
 class wg {
     constructor(e) {
         this.spec = e
     }
 }
 
 function hr(n, e, t, i) {
-    return new Cr(e.doc, n.unquoted, t, i, n.caseSensitive ? void 0 : r => r.toLowerCase(), n.wholeWord ? Ck(e.doc, e.charCategorizer(e.selection.main.head)) : void 0)
+    return new Cr(e.doc, n.unquoted, t, i, n.caseSensitive ? void 0 : r => r.toLowerCase(), n.wholeWord ? Ak(e.doc, e.charCategorizer(e.selection.main.head)) : void 0)
 }
 
-function Ck(n, e) {
+function Ak(n, e) {
     return (t, i, r, s) => ((s > t || s + r.length < i) && (s = Math.max(0, t - 2), r = n.sliceString(s, Math.min(n.length, i + 2))), (e(nl(r, t - s)) != Ve.Word || e(rl(r, t - s)) != Ve.Word) && (e(rl(r, i - s)) != Ve.Word || e(nl(r, i - s)) != Ve.Word))
 }
-class Ak extends wg {
+class Tk extends wg {
     constructor(e) {
         super(e)
     }
     nextMatch(e, t, i) {
         let r = hr(this.spec, e, i, e.doc.length).nextOverlapping();
         return r.done && (r = hr(this.spec, e, 0, t).nextOverlapping()), r.done ? null : r.value
     }
@@ -16805,30 +16805,30 @@
         for (; !s.next().done;) r(s.value.from, s.value.to)
     }
 }
 
 function cr(n, e, t, i) {
     return new yg(e.doc, n.search, {
         ignoreCase: !n.caseSensitive,
-        test: n.wholeWord ? Tk(e.charCategorizer(e.selection.main.head)) : void 0
+        test: n.wholeWord ? Ok(e.charCategorizer(e.selection.main.head)) : void 0
     }, t, i)
 }
 
 function nl(n, e) {
     return n.slice(mt(n, e, !1), e)
 }
 
 function rl(n, e) {
     return n.slice(e, mt(n, e))
 }
 
-function Tk(n) {
+function Ok(n) {
     return (e, t, i) => !i[0].length || (n(nl(i.input, i.index)) != Ve.Word || n(rl(i.input, i.index)) != Ve.Word) && (n(rl(i.input, i.index + i[0].length)) != Ve.Word || n(nl(i.input, i.index + i[0].length)) != Ve.Word)
 }
-class Ok extends wg {
+class Mk extends wg {
     nextMatch(e, t, i) {
         let r = cr(this.spec, e, i, e.doc.length).next();
         return r.done && (r = cr(this.spec, e, 0, t).next()), r.done ? null : r.value
     }
     prevMatchInRange(e, t, i) {
         for (let r = 1;; r++) {
             let s = Math.max(t, i - r * 1e4),
@@ -16872,21 +16872,21 @@
         provide: n => xs.from(n, e => e.panel)
     });
 class ka {
     constructor(e, t) {
         this.query = e, this.panel = t
     }
 }
-const Mk = de.mark({
+const Ek = de.mark({
         class: "cm-searchMatch"
     }),
-    Ek = de.mark({
+    Dk = de.mark({
         class: "cm-searchMatch cm-searchMatch-selected"
     }),
-    Dk = rt.fromClass(class {
+    Rk = rt.fromClass(class {
         constructor(n) {
             this.view = n, this.decorations = this.highlight(n.state.field(yn))
         }
         update(n) {
             let e = n.state.field(yn);
             (e != n.startState.field(yn) || n.docChanged || n.selectionSet || n.viewportChanged) && (this.decorations = this.highlight(e))
         }
@@ -16901,16 +16901,16 @@
             for (let r = 0, s = t.visibleRanges, o = s.length; r < o; r++) {
                 let {
                     from: l,
                     to: h
                 } = s[r];
                 for (; r < o - 1 && h > s[r + 1].from - 2 * 250;) h = s[++r].to;
                 n.highlight(t.state, l, h, (f, u) => {
-                    let g = t.state.selection.ranges.some(y => y.from == f && y.to == u);
-                    i.add(f, u, g ? Ek : Mk)
+                    let m = t.state.selection.ranges.some(y => y.from == f && y.to == u);
+                    i.add(f, u, m ? Dk : Ek)
                 })
             }
             return i.finish()
         }
     }, {
         decorations: n => n.decorations
     });
@@ -16949,24 +16949,24 @@
             o = n.state.facet(Or);
         return n.dispatch({
             selection: s,
             effects: [nc(n, r), o.scrollToMatch(s.main, n)],
             userEvent: "select.search"
         }), Sg(n), !0
     }),
-    Rk = Ps((n, {
+    Lk = Ps((n, {
         query: e
     }) => {
         let t = e.matchAll(n.state, 1e3);
         return !t || !t.length ? !1 : (n.dispatch({
             selection: H.create(t.map(i => H.range(i.from, i.to))),
             userEvent: "select.search.matches"
         }), !0)
     }),
-    Lk = ({
+    Pk = ({
         state: n,
         dispatch: e
     }) => {
         let t = n.selection;
         if (t.ranges.length > 1 || t.main.empty) return !1;
         let {
             from: i,
@@ -17006,15 +17006,15 @@
         return n.dispatch({
             changes: o,
             selection: l,
             effects: f,
             userEvent: "input.replace"
         }), !0
     }),
-    Pk = Ps((n, {
+    Nk = Ps((n, {
         query: e
     }) => {
         if (n.state.readOnly) return !1;
         let t = e.matchAll(n.state, 1e9).map(r => {
             let {
                 from: s,
                 to: o
@@ -17069,27 +17069,27 @@
             if (t && t != n.root.activeElement) {
                 let i = vh(n.state, e.query.spec);
                 i.valid && n.dispatch({
                     effects: vs.of(i)
                 }), t.focus(), t.select()
             }
         } else n.dispatch({
-            effects: [tc.of(!0), e ? vs.of(vh(n.state, e.query.spec)) : me.appendConfig.of(_k)]
+            effects: [tc.of(!0), e ? vs.of(vh(n.state, e.query.spec)) : me.appendConfig.of(Hk)]
         });
         return !0
     },
     Ag = n => {
         let e = n.state.field(yn, !1);
         if (!e || !e.panel) return !1;
         let t = bs(n, ic);
         return t && t.dom.contains(n.root.activeElement) && n.focus(), n.dispatch({
             effects: tc.of(!1)
         }), !0
     },
-    Nk = [{
+    Ik = [{
         key: "Mod-f",
         run: Cg,
         scope: "editor search-panel"
     }, {
         key: "F3",
         run: sl,
         shift: ol,
@@ -17103,24 +17103,24 @@
         preventDefault: !0
     }, {
         key: "Escape",
         run: Ag,
         scope: "editor search-panel"
     }, {
         key: "Mod-Shift-l",
-        run: Lk
+        run: Pk
     }, {
         key: "Mod-Alt-g",
-        run: uk
+        run: dk
     }, {
         key: "Mod-d",
-        run: Sk,
+        run: Ck,
         preventDefault: !0
     }];
-class Ik {
+class Bk {
     constructor(e) {
         this.view = e;
         let t = this.query = e.state.field(yn).query.spec;
         this.commit = this.commit.bind(this), this.searchField = $e("input", {
             value: t.search,
             placeholder: $t(e, "Find"),
             "aria-label": $t(e, "Find"),
@@ -17166,15 +17166,15 @@
                 onclick: s,
                 type: "button"
             }, o)
         }
         this.dom = $e("div", {
             onkeydown: r => this.keydown(r),
             class: "cm-search"
-        }, [this.searchField, i("next", () => sl(e), [$t(e, "next")]), i("prev", () => ol(e), [$t(e, "previous")]), i("select", () => Rk(e), [$t(e, "all")]), $e("label", null, [this.caseField, $t(e, "match case")]), $e("label", null, [this.reField, $t(e, "regexp")]), $e("label", null, [this.wordField, $t(e, "by word")]), ...e.state.readOnly ? [] : [$e("br"), this.replaceField, i("replace", () => ou(e), [$t(e, "replace")]), i("replaceAll", () => Pk(e), [$t(e, "replace all")])], $e("button", {
+        }, [this.searchField, i("next", () => sl(e), [$t(e, "next")]), i("prev", () => ol(e), [$t(e, "previous")]), i("select", () => Lk(e), [$t(e, "all")]), $e("label", null, [this.caseField, $t(e, "match case")]), $e("label", null, [this.reField, $t(e, "regexp")]), $e("label", null, [this.wordField, $t(e, "by word")]), ...e.state.readOnly ? [] : [$e("br"), this.replaceField, i("replace", () => ou(e), [$t(e, "replace")]), i("replaceAll", () => Nk(e), [$t(e, "replace all")])], $e("button", {
             name: "close",
             onclick: () => Ag(e),
             "aria-label": $t(e, "close"),
             type: "button"
         }, ["×"])])
     }
     commit() {
@@ -17186,15 +17186,15 @@
             replace: this.replaceField.value
         });
         e.eq(this.query) || (this.query = e, this.view.dispatch({
             effects: vs.of(e)
         }))
     }
     keydown(e) {
-        Zy(this.view, e, "search-panel") ? e.preventDefault() : e.keyCode == 13 && e.target == this.searchField ? (e.preventDefault(), (e.shiftKey ? ol : sl)(this.view)) : e.keyCode == 13 && e.target == this.replaceField && (e.preventDefault(), ou(this.view))
+        eb(this.view, e, "search-panel") ? e.preventDefault() : e.keyCode == 13 && e.target == this.searchField ? (e.preventDefault(), (e.shiftKey ? ol : sl)(this.view)) : e.keyCode == 13 && e.target == this.replaceField && (e.preventDefault(), ou(this.view))
     }
     update(e) {
         for (let t of e.transactions)
             for (let i of t.effects) i.is(vs) && !i.value.eq(this.query) && this.setQuery(i.value)
     }
     setQuery(e) {
         this.query = e, this.searchField.value = e.search, this.replaceField.value = e.replace, this.caseField.checked = e.caseSensitive, this.reField.checked = e.regexp, this.wordField.checked = e.wholeWord
@@ -17237,15 +17237,15 @@
             if (!xo.test(l[h - 1]) && xo.test(l[h])) {
                 l = l.slice(0, h);
                 break
             }
     }
     return te.announce.of(`${n.state.phrase("current match")}. ${l} ${n.state.phrase("on line")} ${i.number}.`)
 }
-const Bk = te.baseTheme({
+const _k = te.baseTheme({
         ".cm-panel.cm-search": {
             padding: "2px 6px 4px",
             position: "relative",
             "& [name=close]": {
                 position: "absolute",
                 top: "0",
                 right: "4px",
@@ -17275,15 +17275,15 @@
         "&light .cm-searchMatch-selected": {
             backgroundColor: "#ff6a0054"
         },
         "&dark .cm-searchMatch-selected": {
             backgroundColor: "#ff00ff8a"
         }
     }),
-    _k = [yn, Kn.low(Dk), Bk];
+    Hk = [yn, Kn.low(Rk), _k];
 class Tg {
     constructor(e, t, i) {
         this.state = e, this.pos = t, this.explicit = i, this.abortListeners = []
     }
     tokenBefore(e) {
         let t = lt(this.state).resolveInner(this.pos, -1);
         for (; t && e.indexOf(t.name) < 0;) t = t.parent;
@@ -17315,15 +17315,15 @@
 
 function lu(n) {
     let e = Object.keys(n).join(""),
         t = /\w/.test(e);
     return t && (e = e.replace(/\w/g, "")), `[${t?"\\w":""}${e.replace(/[^\w\s]/g,"\\$&")}]`
 }
 
-function Hk(n) {
+function Fk(n) {
     let e = Object.create(null),
         t = Object.create(null);
     for (let {
             label: r
         }
         of n) {
         e[r[0]] = !0;
@@ -17333,26 +17333,26 @@
     return [new RegExp("^" + i), new RegExp(i)]
 }
 
 function Og(n) {
     let e = n.map(r => typeof r == "string" ? {
             label: r
         } : r),
-        [t, i] = e.every(r => /^\w+$/.test(r.label)) ? [/\w*$/, /\w+$/] : Hk(e);
+        [t, i] = e.every(r => /^\w+$/.test(r.label)) ? [/\w*$/, /\w+$/] : Fk(e);
     return r => {
         let s = r.matchBefore(i);
         return s || r.explicit ? {
             from: s ? s.from : r.pos,
             options: e,
             validFor: t
         } : null
     }
 }
 
-function Fk(n, e) {
+function zk(n, e) {
     return t => {
         for (let i = lt(t.state).resolveInner(t.pos, -1); i; i = i.parent) {
             if (n.indexOf(i.name) > -1) return null;
             if (i.type.isTop) break
         }
         return e(t)
     }
@@ -17370,17 +17370,17 @@
 function Mg(n, e) {
     var t;
     let {
         source: i
     } = n, r = e && i[0] != "^", s = i[i.length - 1] != "$";
     return !r && !s ? n : new RegExp(`${r?"^":""}(?:${i})${s?"$":""}`, (t = n.flags) !== null && t !== void 0 ? t : n.ignoreCase ? "i" : "")
 }
-const zk = Xi.define();
+const $k = Xi.define();
 
-function $k(n, e, t, i) {
+function Wk(n, e, t, i) {
     let {
         main: r
     } = n.selection, s = t - r.from, o = i - r.from;
     return Object.assign(Object.assign({}, n.changeByRange(l => l != r && t != i && n.sliceDoc(l.from + s, l.from + o) != n.sliceDoc(t, i) ? {
         range: l
     } : {
         changes: {
@@ -17392,22 +17392,22 @@
     })), {
         scrollIntoView: !0,
         userEvent: "input.complete"
     })
 }
 const hu = new WeakMap;
 
-function Wk(n) {
+function qk(n) {
     if (!Array.isArray(n)) return n;
     let e = hu.get(n);
     return e || hu.set(n, e = Og(n)), e
 }
 const rc = me.define(),
     Ss = me.define();
-class qk {
+class jk {
     constructor(e) {
         this.pattern = e, this.chars = [], this.folded = [], this.any = [], this.precise = [], this.byWord = [], this.score = 0, this.matched = [];
         for (let t = 0; t < e.length;) {
             let i = pt(e, t),
                 r = ti(i);
             this.chars.push(i);
             let s = e.slice(t, t + r),
@@ -17446,28 +17446,28 @@
             for (let F = 0, $ = Math.min(e.length, 200); F < $ && f < h;) {
                 let j = pt(e, F);
                 (j == t[f] || j == i[f]) && (r[f++] = F), F += ti(j)
             }
             if (f < h) return !1
         }
         let u = 0,
-            g = 0,
+            m = 0,
             y = !1,
             k = 0,
             v = -1,
-            C = -1,
+            A = -1,
             O = /[a-z]/.test(e),
             D = !0;
-        for (let F = 0, $ = Math.min(e.length, 200), j = 0; F < $ && g < h;) {
+        for (let F = 0, $ = Math.min(e.length, 200), j = 0; F < $ && m < h;) {
             let z = pt(e, F);
-            l < 0 && (u < h && z == t[u] && (s[u++] = F), k < h && (z == t[k] || z == i[k] ? (k == 0 && (v = F), C = F + 1, k++) : k = 0));
+            l < 0 && (u < h && z == t[u] && (s[u++] = F), k < h && (z == t[k] || z == i[k] ? (k == 0 && (v = F), A = F + 1, k++) : k = 0));
             let G, p = z < 255 ? z >= 48 && z <= 57 || z >= 97 && z <= 122 ? 2 : z >= 65 && z <= 90 ? 1 : 0 : (G = Rh(z)) != G.toLowerCase() ? 1 : G != G.toUpperCase() ? 2 : 0;
-            (!F || p == 1 && O || j == 0 && p != 0) && (t[g] == z || i[g] == z && (y = !0) ? o[g++] = F : o.length && (D = !1)), j = p, F += ti(z)
+            (!F || p == 1 && O || j == 0 && p != 0) && (t[m] == z || i[m] == z && (y = !0) ? o[m++] = F : o.length && (D = !1)), j = p, F += ti(z)
         }
-        return g == h && o[0] == 0 && D ? this.result(-100 + (y ? -200 : 0), o, e) : k == h && v == 0 ? this.ret(-200 - e.length + (C == e.length ? 0 : -100), [0, C]) : l > -1 ? this.ret(-700 - e.length, [l, l + this.pattern.length]) : k == h ? this.ret(-900 - e.length, [v, C]) : g == h ? this.result(-100 + (y ? -200 : 0) + -700 + (D ? 0 : -1100), o, e) : t.length == 2 ? !1 : this.result((r[0] ? -700 : 0) + -200 + -1100, r, e)
+        return m == h && o[0] == 0 && D ? this.result(-100 + (y ? -200 : 0), o, e) : k == h && v == 0 ? this.ret(-200 - e.length + (A == e.length ? 0 : -100), [0, A]) : l > -1 ? this.ret(-700 - e.length, [l, l + this.pattern.length]) : k == h ? this.ret(-900 - e.length, [v, A]) : m == h ? this.result(-100 + (y ? -200 : 0) + -700 + (D ? 0 : -1100), o, e) : t.length == 2 ? !1 : this.result((r[0] ? -700 : 0) + -200 + -1100, r, e)
     }
     result(e, t, i) {
         let r = [],
             s = 0;
         for (let o of t) {
             let l = o + (this.astral ? ti(pt(i, o)) : 1);
             s && r[s - 1] == o ? r[s - 1] = l : (r[s++] = o, r[s++] = l)
@@ -17485,15 +17485,15 @@
             maxRenderedOptions: 100,
             defaultKeymap: !0,
             tooltipClass: () => "",
             optionClass: () => "",
             aboveCursor: !1,
             icons: !0,
             addToOptions: [],
-            positionInfo: jk,
+            positionInfo: Vk,
             compareCompletions: (e, t) => e.label.localeCompare(t.label),
             interactionDelay: 75,
             updateSyncTime: 100
         }, {
             defaultKeymap: (e, t) => e && t,
             closeOnBlur: (e, t) => e && t,
             icons: (e, t) => e && t,
@@ -17504,38 +17504,38 @@
     }
 });
 
 function cu(n, e) {
     return n ? e ? n + " " + e : n : e
 }
 
-function jk(n, e, t, i, r, s) {
+function Vk(n, e, t, i, r, s) {
     let o = n.textDirection == Ue.RTL,
         l = o,
         h = !1,
         f = "top",
-        u, g, y = e.left - r.left,
+        u, m, y = e.left - r.left,
         k = r.right - e.right,
         v = i.right - i.left,
-        C = i.bottom - i.top;
-    if (l && y < Math.min(v, k) ? l = !1 : !l && k < Math.min(v, y) && (l = !0), v <= (l ? y : k)) u = Math.max(r.top, Math.min(t.top, r.bottom - C)) - e.top, g = Math.min(400, l ? y : k);
+        A = i.bottom - i.top;
+    if (l && y < Math.min(v, k) ? l = !1 : !l && k < Math.min(v, y) && (l = !0), v <= (l ? y : k)) u = Math.max(r.top, Math.min(t.top, r.bottom - A)) - e.top, m = Math.min(400, l ? y : k);
     else {
-        h = !0, g = Math.min(400, (o ? e.right : r.right - e.left) - 30);
+        h = !0, m = Math.min(400, (o ? e.right : r.right - e.left) - 30);
         let F = r.bottom - e.bottom;
-        F >= C || F > e.top ? u = t.bottom - e.top : (f = "bottom", u = e.bottom - t.top)
+        F >= A || F > e.top ? u = t.bottom - e.top : (f = "bottom", u = e.bottom - t.top)
     }
     let O = (e.bottom - e.top) / s.offsetHeight,
         D = (e.right - e.left) / s.offsetWidth;
     return {
-        style: `${f}: ${u/O}px; max-width: ${g/D}px`,
+        style: `${f}: ${u/O}px; max-width: ${m/D}px`,
         class: "cm-completionInfo-" + (h ? o ? "left-narrow" : "right-narrow" : l ? "left" : "right")
     }
 }
 
-function Vk(n) {
+function Uk(n) {
     let e = n.addToOptions.slice();
     return n.icons && e.push({
         render(t) {
             let i = document.createElement("div");
             return i.classList.add("cm-completionIcon"), t.type && i.classList.add(...t.type.split(/\s+/g).map(r => "cm-completionIcon-" + r)), i.setAttribute("aria-hidden", "true"), i
         },
         position: 20
@@ -17543,18 +17543,18 @@
         render(t, i, r, s) {
             let o = document.createElement("span");
             o.className = "cm-completionLabel";
             let l = t.displayLabel || t.label,
                 h = 0;
             for (let f = 0; f < s.length;) {
                 let u = s[f++],
-                    g = s[f++];
+                    m = s[f++];
                 u > h && o.appendChild(document.createTextNode(l.slice(h, u)));
                 let y = o.appendChild(document.createElement("span"));
-                y.appendChild(document.createTextNode(l.slice(u, g))), y.className = "cm-completionMatchedText", h = g
+                y.appendChild(document.createTextNode(l.slice(u, m))), y.className = "cm-completionMatchedText", h = m
             }
             return h < l.length && o.appendChild(document.createTextNode(l.slice(h))), o
         },
         position: 50
     }, {
         render(t) {
             if (!t.detail) return null;
@@ -17579,34 +17579,34 @@
     }
     let i = Math.floor((n - e) / t);
     return {
         from: n - (i + 1) * t,
         to: n - i * t
     }
 }
-class Uk {
+class Qk {
     constructor(e, t, i) {
         this.view = e, this.stateField = t, this.applyCompletion = i, this.info = null, this.infoDestroy = null, this.placeInfoReq = {
             read: () => this.measureInfo(),
             write: h => this.placeInfo(h),
             key: this
         }, this.space = null, this.currentClass = "";
         let r = e.state.field(t),
             {
                 options: s,
                 selected: o
             } = r.open,
             l = e.state.facet(Ct);
-        this.optionContent = Vk(l), this.optionClass = l.optionClass, this.tooltipClass = l.tooltipClass, this.range = wa(s.length, o, l.maxRenderedOptions), this.dom = document.createElement("div"), this.dom.className = "cm-tooltip-autocomplete", this.updateTooltipClass(e.state), this.dom.addEventListener("mousedown", h => {
+        this.optionContent = Uk(l), this.optionClass = l.optionClass, this.tooltipClass = l.tooltipClass, this.range = wa(s.length, o, l.maxRenderedOptions), this.dom = document.createElement("div"), this.dom.className = "cm-tooltip-autocomplete", this.updateTooltipClass(e.state), this.dom.addEventListener("mousedown", h => {
             let {
                 options: f
             } = e.state.field(t).open;
-            for (let u = h.target, g; u && u != this.dom; u = u.parentNode)
-                if (u.nodeName == "LI" && (g = /-(\d+)$/.exec(u.id)) && +g[1] < f.length) {
-                    this.applyCompletion(e, f[+g[1]]), h.preventDefault();
+            for (let u = h.target, m; u && u != this.dom; u = u.parentNode)
+                if (u.nodeName == "LI" && (m = /-(\d+)$/.exec(u.id)) && +m[1] < f.length) {
+                    this.applyCompletion(e, f[+m[1]]), h.preventDefault();
                     return
                 }
         }), this.dom.addEventListener("focusout", h => {
             let f = e.state.field(this.stateField, !1);
             f && f.tooltip && e.state.facet(Ct).closeOnBlur && h.relatedTarget != e.contentDOM && e.dispatch({
                 effects: Ss.of(null)
             })
@@ -17674,15 +17674,15 @@
             i.appendChild(r), this.infoDestroy = s || null
         }
         this.dom.appendChild(i), this.view.requestMeasure(this.placeInfoReq)
     }
     updateSelectedOption(e) {
         let t = null;
         for (let i = this.list.firstChild, r = this.range.from; i; i = i.nextSibling, r++) i.nodeName != "LI" || !i.id ? r-- : r == e ? i.hasAttribute("aria-selected") || (i.setAttribute("aria-selected", "true"), t = i) : i.hasAttribute("aria-selected") && i.removeAttribute("aria-selected");
-        return t && Gk(this.list, t), t
+        return t && Kk(this.list, t), t
     }
     measureInfo() {
         let e = this.dom.querySelector("[aria-selected]");
         if (!e || !this.info) return null;
         let t = this.dom.getBoundingClientRect(),
             i = this.info.getBoundingClientRect(),
             r = e.getBoundingClientRect(),
@@ -17719,16 +17719,16 @@
                     else {
                         let k = r.appendChild(document.createElement("completion-section"));
                         k.textContent = y
                     }
             }
             const u = r.appendChild(document.createElement("li"));
             u.id = t + "-" + o, u.setAttribute("role", "option");
-            let g = this.optionClass(l);
-            g && (u.className = g);
+            let m = this.optionClass(l);
+            m && (u.className = m);
             for (let y of this.optionContent) {
                 let k = y(l, this.view.state, this.view, h);
                 k && u.appendChild(k)
             }
         }
         return i.from && r.classList.add("cm-completionListIncompleteTop"), i.to < e.length && r.classList.add("cm-completionListIncompleteBottom"), r
     }
@@ -17736,71 +17736,71 @@
         this.info && (this.infoDestroy && this.infoDestroy(), this.info.remove(), this.info = null)
     }
     destroy() {
         this.destroyInfo()
     }
 }
 
-function Qk(n, e) {
-    return t => new Uk(t, n, e)
+function Gk(n, e) {
+    return t => new Qk(t, n, e)
 }
 
-function Gk(n, e) {
+function Kk(n, e) {
     let t = n.getBoundingClientRect(),
         i = e.getBoundingClientRect(),
         r = t.height / n.offsetHeight;
     i.top < t.top ? n.scrollTop -= (t.top - i.top) / r : i.bottom > t.bottom && (n.scrollTop += (i.bottom - t.bottom) / r)
 }
 
 function fu(n) {
     return (n.boost || 0) * 100 + (n.apply ? 10 : 0) + (n.info ? 5 : 0) + (n.type ? 1 : 0)
 }
 
-function Kk(n, e) {
+function Xk(n, e) {
     let t = [],
         i = null,
         r = h => {
             t.push(h);
             let {
                 section: f
             } = h.completion;
             if (f) {
                 i || (i = []);
                 let u = typeof f == "string" ? f : f.name;
-                i.some(g => g.name == u) || i.push(typeof f == "string" ? {
+                i.some(m => m.name == u) || i.push(typeof f == "string" ? {
                     name: u
                 } : f)
             }
         };
     for (let h of n)
         if (h.hasResult()) {
             let f = h.result.getMatch;
             if (h.result.filter === !1)
                 for (let u of h.result.options) r(new au(u, h.source, f ? f(u) : [], 1e9 - t.length));
             else {
-                let u = new qk(e.sliceDoc(h.from, h.to));
-                for (let g of h.result.options)
-                    if (u.match(g.label)) {
-                        let y = g.displayLabel ? f ? f(g, u.matched) : [] : u.matched;
-                        r(new au(g, h.source, y, u.score + (g.boost || 0)))
+                let u = new jk(e.sliceDoc(h.from, h.to));
+                for (let m of h.result.options)
+                    if (u.match(m.label)) {
+                        let y = m.displayLabel ? f ? f(m, u.matched) : [] : u.matched;
+                        r(new au(m, h.source, y, u.score + (m.boost || 0)))
                     }
             }
         } if (i) {
         let h = Object.create(null),
             f = 0,
-            u = (g, y) => {
+            u = (m, y) => {
                 var k, v;
-                return ((k = g.rank) !== null && k !== void 0 ? k : 1e9) - ((v = y.rank) !== null && v !== void 0 ? v : 1e9) || (g.name < y.name ? -1 : 1)
+                return ((k = m.rank) !== null && k !== void 0 ? k : 1e9) - ((v = y.rank) !== null && v !== void 0 ? v : 1e9) || (m.name < y.name ? -1 : 1)
             };
-        for (let g of i.sort(u)) f -= 1e5, h[g.name] = f;
-        for (let g of t) {
+        for (let m of i.sort(u)) f -= 1e5, h[m.name] = f;
+        for (let m of t) {
             let {
                 section: y
-            } = g.completion;
-            y && (g.score += h[typeof y == "string" ? y : y.name])
+            } = m.completion;
+            y && (m.score += h[typeof y == "string" ? y : y.name])
         }
     }
     let s = [],
         o = null,
         l = e.facet(Ct).compareCompletions;
     for (let h of t.sort((f, u) => u.score - f.score || l(f.completion, u.completion))) {
         let f = h.completion;
@@ -17812,86 +17812,86 @@
     constructor(e, t, i, r, s, o) {
         this.options = e, this.attrs = t, this.tooltip = i, this.timestamp = r, this.selected = s, this.disabled = o
     }
     setSelected(e, t) {
         return e == this.selected || e >= this.options.length ? this : new dr(this.options, uu(t, e), this.tooltip, this.timestamp, e, this.disabled)
     }
     static build(e, t, i, r, s) {
-        let o = Kk(e, t);
+        let o = Xk(e, t);
         if (!o.length) return r && e.some(h => h.state == 1) ? new dr(r.options, r.attrs, r.tooltip, r.timestamp, r.selected, !0) : null;
         let l = t.facet(Ct).selectOnOpen ? 0 : -1;
         if (r && r.selected != l && r.selected != -1) {
             let h = r.options[r.selected].completion;
             for (let f = 0; f < o.length; f++)
                 if (o[f].completion == h) {
                     l = f;
                     break
                 }
         }
         return new dr(o, uu(i, l), {
             pos: e.reduce((h, f) => f.hasResult() ? Math.min(h, f.from) : h, 1e8),
-            create: ew,
+            create: tw,
             above: s.aboveCursor
         }, r ? r.timestamp : Date.now(), l, !1)
     }
     map(e) {
         return new dr(this.options, this.attrs, Object.assign(Object.assign({}, this.tooltip), {
             pos: e.mapPos(this.tooltip.pos)
         }), this.timestamp, this.selected, this.disabled)
     }
 }
 class ll {
     constructor(e, t, i) {
         this.active = e, this.id = t, this.open = i
     }
     static start() {
-        return new ll(Jk, "cm-ac-" + Math.floor(Math.random() * 2e6).toString(36), null)
+        return new ll(Zk, "cm-ac-" + Math.floor(Math.random() * 2e6).toString(36), null)
     }
     update(e) {
         let {
             state: t
-        } = e, i = t.facet(Ct), s = (i.override || t.languageDataAt("autocomplete", bn(t)).map(Wk)).map(l => (this.active.find(f => f.source == l) || new Bt(l, this.active.some(f => f.state != 0) ? 1 : 0)).update(e, i));
+        } = e, i = t.facet(Ct), s = (i.override || t.languageDataAt("autocomplete", bn(t)).map(qk)).map(l => (this.active.find(f => f.source == l) || new Bt(l, this.active.some(f => f.state != 0) ? 1 : 0)).update(e, i));
         s.length == this.active.length && s.every((l, h) => l == this.active[h]) && (s = this.active);
         let o = this.open;
-        o && e.docChanged && (o = o.map(e.changes)), e.selection || s.some(l => l.hasResult() && e.changes.touchesRange(l.from, l.to)) || !Xk(s, this.active) ? o = dr.build(s, t, this.id, o, i) : o && o.disabled && !s.some(l => l.state == 1) && (o = null), !o && s.every(l => l.state != 1) && s.some(l => l.hasResult()) && (s = s.map(l => l.hasResult() ? new Bt(l.source, 0) : l));
+        o && e.docChanged && (o = o.map(e.changes)), e.selection || s.some(l => l.hasResult() && e.changes.touchesRange(l.from, l.to)) || !Yk(s, this.active) ? o = dr.build(s, t, this.id, o, i) : o && o.disabled && !s.some(l => l.state == 1) && (o = null), !o && s.every(l => l.state != 1) && s.some(l => l.hasResult()) && (s = s.map(l => l.hasResult() ? new Bt(l.source, 0) : l));
         for (let l of e.effects) l.is(Dg) && (o = o && o.setSelected(l.value, this.id));
         return s == this.active && o == this.open ? this : new ll(s, this.id, o)
     }
     get tooltip() {
         return this.open ? this.open.tooltip : null
     }
     get attrs() {
-        return this.open ? this.open.attrs : Yk
+        return this.open ? this.open.attrs : Jk
     }
 }
 
-function Xk(n, e) {
+function Yk(n, e) {
     if (n == e) return !0;
     for (let t = 0, i = 0;;) {
         for (; t < n.length && !n[t].hasResult;) t++;
         for (; i < e.length && !e[i].hasResult;) i++;
         let r = t == n.length,
             s = i == e.length;
         if (r || s) return r == s;
         if (n[t++].result != e[i++].result) return !1
     }
 }
-const Yk = {
+const Jk = {
     "aria-autocomplete": "list"
 };
 
 function uu(n, e) {
     let t = {
         "aria-autocomplete": "list",
         "aria-haspopup": "listbox",
         "aria-controls": n
     };
     return e > -1 && (t["aria-activedescendant"] = n + "-" + e), t
 }
-const Jk = [];
+const Zk = [];
 
 function Sh(n) {
     return n.isUserEvent("input.type") ? "input" : n.isUserEvent("delete.backward") ? "delete" : null
 }
 class Bt {
     constructor(e, t, i = -1) {
         this.source = e, this.state = t, this.explicitPos = i
@@ -17931,25 +17931,25 @@
         var r;
         let s = e.changes.mapPos(this.from),
             o = e.changes.mapPos(this.to, 1),
             l = bn(e.state);
         if ((this.explicitPos < 0 ? l <= s : l < this.from) || l > o || t == "delete" && bn(e.startState) == this.from) return new Bt(this.source, t == "input" && i.activateOnTyping ? 1 : 0);
         let h = this.explicitPos < 0 ? -1 : e.changes.mapPos(this.explicitPos),
             f;
-        return Zk(this.result.validFor, e.state, s, o) ? new xr(this.source, h, this.result, s, o) : this.result.update && (f = this.result.update(this.result, s, o, new Tg(e.state, l, h >= 0))) ? new xr(this.source, h, f, f.from, (r = f.to) !== null && r !== void 0 ? r : bn(e.state)) : new Bt(this.source, 1, h)
+        return ew(this.result.validFor, e.state, s, o) ? new xr(this.source, h, this.result, s, o) : this.result.update && (f = this.result.update(this.result, s, o, new Tg(e.state, l, h >= 0))) ? new xr(this.source, h, f, f.from, (r = f.to) !== null && r !== void 0 ? r : bn(e.state)) : new Bt(this.source, 1, h)
     }
     handleChange(e) {
         return e.changes.touchesRange(this.from, this.to) ? new Bt(this.source, 0) : this.map(e.changes)
     }
     map(e) {
         return e.empty ? this : new xr(this.source, this.explicitPos < 0 ? -1 : e.mapPos(this.explicitPos), this.result, e.mapPos(this.from), e.mapPos(this.to, 1))
     }
 }
 
-function Zk(n, e, t, i) {
+function ew(n, e, t, i) {
     if (!n) return !1;
     let r = e.sliceDoc(t, i);
     return typeof n == "function" ? n(r, t, i, e) : Mg(n, !0).test(r)
 }
 const Eg = me.define({
         map(n, e) {
             return n.map(t => t.map(e))
@@ -17965,19 +17965,19 @@
         },
         provide: n => [Wh.from(n, e => e.tooltip), te.contentAttributes.from(n, e => e.attrs)]
     });
 
 function Rg(n, e) {
     const t = e.completion.apply || e.completion.label;
     let i = n.state.field(Ut).active.find(r => r.source == e.source);
-    return i instanceof xr ? (typeof t == "string" ? n.dispatch(Object.assign(Object.assign({}, $k(n.state, t, i.from, i.to)), {
-        annotations: zk.of(e.completion)
+    return i instanceof xr ? (typeof t == "string" ? n.dispatch(Object.assign(Object.assign({}, Wk(n.state, t, i.from, i.to)), {
+        annotations: $k.of(e.completion)
     })) : t(n, e.completion, i.from, i.to), !0) : !1
 }
-const ew = Qk(Ut, Rg);
+const tw = Gk(Ut, Rg);
 
 function ko(n, e = "option") {
     return t => {
         let i = t.state.field(Ut, !1);
         if (!i || !i.open || i.open.disabled || Date.now() - i.open.timestamp < t.state.facet(Ct).interactionDelay) return !1;
         let r = 1,
             s;
@@ -17990,42 +17990,42 @@
         }), !0
     }
 }
 const Lg = n => {
         let e = n.state.field(Ut, !1);
         return n.state.readOnly || !e || !e.open || e.open.selected < 0 || e.open.disabled || Date.now() - e.open.timestamp < n.state.facet(Ct).interactionDelay ? !1 : Rg(n, e.open.options[e.open.selected])
     },
-    tw = n => n.state.field(Ut, !1) ? (n.dispatch({
+    iw = n => n.state.field(Ut, !1) ? (n.dispatch({
         effects: rc.of(!0)
     }), !0) : !1,
-    iw = n => {
+    nw = n => {
         let e = n.state.field(Ut, !1);
         return !e || !e.active.some(t => t.state != 0) ? !1 : (n.dispatch({
             effects: Ss.of(null)
         }), !0)
     };
-class nw {
+class rw {
     constructor(e, t) {
         this.active = e, this.context = t, this.time = Date.now(), this.updates = [], this.done = void 0
     }
 }
-const rw = 50,
-    sw = 1e3,
-    ow = rt.fromClass(class {
+const sw = 50,
+    ow = 1e3,
+    lw = rt.fromClass(class {
         constructor(n) {
             this.view = n, this.debounceUpdate = -1, this.running = [], this.debounceAccept = -1, this.composing = 0;
             for (let e of n.state.field(Ut).active) e.state == 1 && this.startQuery(e)
         }
         update(n) {
             let e = n.state.field(Ut);
             if (!n.selectionSet && !n.docChanged && n.startState.field(Ut) == e) return;
             let t = n.transactions.some(i => (i.selection || i.docChanged) && !Sh(i));
             for (let i = 0; i < this.running.length; i++) {
                 let r = this.running[i];
-                if (t || r.updates.length + n.transactions.length > rw && Date.now() - r.time > sw) {
+                if (t || r.updates.length + n.transactions.length > sw && Date.now() - r.time > ow) {
                     for (let s of r.context.abortListeners) try {
                         s()
                     } catch (o) {
                         ni(this.view.state, o)
                     }
                     r.context.abortListeners = null, this.running.splice(i--, 1)
                 } else r.updates.push(...n.transactions)
@@ -18039,15 +18039,15 @@
                 state: n
             } = this.view, e = n.field(Ut);
             for (let t of e.active) t.state == 1 && !this.running.some(i => i.active.source == t.source) && this.startQuery(t)
         }
         startQuery(n) {
             let {
                 state: e
-            } = this.view, t = bn(e), i = new Tg(e, t, n.explicitPos == t), r = new nw(n, i);
+            } = this.view, t = bn(e), i = new Tg(e, t, n.explicitPos == t), r = new rw(n, i);
             this.running.push(r), Promise.resolve(n.source(i)).then(s => {
                 r.context.aborted || (r.done = s || null, this.scheduleAccept())
             }, s => {
                 this.view.dispatch({
                     effects: Ss.of(null)
                 }), ni(this.view.state, s)
             })
@@ -18100,15 +18100,15 @@
             compositionend() {
                 this.composing == 3 && setTimeout(() => this.view.dispatch({
                     effects: rc.of(!1)
                 }), 20), this.composing = 0
             }
         }
     }),
-    lw = te.baseTheme({
+    aw = te.baseTheme({
         ".cm-tooltip.cm-tooltip-autocomplete": {
             "& > ul": {
                 fontFamily: "monospace",
                 whiteSpace: "nowrap",
                 overflow: "hidden auto",
                 maxWidth_fallback: "700px",
                 maxWidth: "min(700px, 95vw)",
@@ -18290,46 +18290,46 @@
         for (let t of e.effects) t.is(qn) && (n = n.update({
             add: [sc.range(t.value, t.value + 1)]
         }));
         return n
     }
 });
 
-function aw() {
-    return [cw, Pg]
+function hw() {
+    return [fw, Pg]
 }
 const va = "()[]{}<>";
 
 function Ng(n) {
     for (let e = 0; e < va.length; e += 2)
         if (va.charCodeAt(e) == n) return va.charAt(e + 1);
     return Rh(n < 128 ? n : n + 1)
 }
 
 function Ig(n, e) {
     return n.languageDataAt("closeBrackets", e)[0] || Cs
 }
-const hw = typeof navigator == "object" && /Android\b/.test(navigator.userAgent),
-    cw = te.inputHandler.of((n, e, t, i) => {
-        if ((hw ? n.composing : n.compositionStarted) || n.state.readOnly) return !1;
+const cw = typeof navigator == "object" && /Android\b/.test(navigator.userAgent),
+    fw = te.inputHandler.of((n, e, t, i) => {
+        if ((cw ? n.composing : n.compositionStarted) || n.state.readOnly) return !1;
         let r = n.state.selection.main;
         if (i.length > 2 || i.length == 2 && ti(pt(i, 0)) == 1 || e != r.from || t != r.to) return !1;
-        let s = dw(n.state, i);
+        let s = pw(n.state, i);
         return s ? (n.dispatch(s), !0) : !1
     }),
-    fw = ({
+    uw = ({
         state: n,
         dispatch: e
     }) => {
         if (n.readOnly) return !1;
         let i = Ig(n, n.selection.main.head).brackets || Cs.brackets,
             r = null,
             s = n.changeByRange(o => {
                 if (o.empty) {
-                    let l = pw(n.doc, o.head);
+                    let l = gw(n.doc, o.head);
                     for (let h of i)
                         if (h == l && Ml(n.doc, o.head) == Ng(pt(h, 0))) return {
                             changes: {
                                 from: o.head - h.length,
                                 to: o.head + h.length
                             },
                             range: H.cursor(o.head - h.length)
@@ -18340,26 +18340,26 @@
                 }
             });
         return r || e(n.update(s, {
             scrollIntoView: !0,
             userEvent: "delete.backward"
         })), !r
     },
-    uw = [{
+    dw = [{
         key: "Backspace",
-        run: fw
+        run: uw
     }];
 
-function dw(n, e) {
+function pw(n, e) {
     let t = Ig(n, n.selection.main.head),
         i = t.brackets || Cs.brackets;
     for (let r of i) {
         let s = Ng(pt(r, 0));
-        if (e == r) return s == r ? yw(n, r, i.indexOf(r + r + r) > -1, t) : gw(n, r, s, t.before || Cs.before);
-        if (e == s && Bg(n, n.selection.main.from)) return mw(n, r, s)
+        if (e == r) return s == r ? bw(n, r, i.indexOf(r + r + r) > -1, t) : mw(n, r, s, t.before || Cs.before);
+        if (e == s && Bg(n, n.selection.main.from)) return yw(n, r, s)
     }
     return null
 }
 
 function Bg(n, e) {
     let t = !1;
     return n.field(Pg).between(0, n.doc.length, i => {
@@ -18368,20 +18368,20 @@
 }
 
 function Ml(n, e) {
     let t = n.sliceString(e, e + 2);
     return t.slice(0, ti(pt(t, 0)))
 }
 
-function pw(n, e) {
+function gw(n, e) {
     let t = n.sliceString(e - 2, e);
     return ti(pt(t, 0)) == t.length ? t : t.slice(1)
 }
 
-function gw(n, e, t, i) {
+function mw(n, e, t, i) {
     let r = null,
         s = n.changeByRange(o => {
             if (!o.empty) return {
                 changes: [{
                     insert: e,
                     from: o.from
                 }, {
@@ -18405,15 +18405,15 @@
         });
     return r ? null : n.update(s, {
         scrollIntoView: !0,
         userEvent: "input.type"
     })
 }
 
-function mw(n, e, t) {
+function yw(n, e, t) {
     let i = null,
         r = n.changeByRange(s => s.empty && Ml(n.doc, s.head) == t ? {
             changes: {
                 from: s.head,
                 to: s.head + t.length,
                 insert: t
             },
@@ -18423,15 +18423,15 @@
         });
     return i ? null : n.update(r, {
         scrollIntoView: !0,
         userEvent: "input.type"
     })
 }
 
-function yw(n, e, t, i) {
+function bw(n, e, t, i) {
     let r = i.stringPrefixes || Cs.stringPrefixes,
         s = null,
         o = n.changeByRange(l => {
             if (!l.empty) return {
                 changes: [{
                     insert: e,
                     from: l.from
@@ -18470,15 +18470,15 @@
                     changes: {
                         insert: e + e + e + e,
                         from: h
                     },
                     effects: qn.of(h + e.length),
                     range: H.cursor(h + e.length)
                 };
-                if (n.charCategorizer(h)(f) != Ve.Word && pu(n, h, r) > -1 && !bw(n, h, e, r)) return {
+                if (n.charCategorizer(h)(f) != Ve.Word && pu(n, h, r) > -1 && !xw(n, h, e, r)) return {
                     changes: {
                         insert: e + e,
                         from: h
                     },
                     effects: qn.of(h + e.length),
                     range: H.cursor(h + e.length)
                 }
@@ -18494,15 +18494,15 @@
 }
 
 function du(n, e) {
     let t = lt(n).resolveInner(e + 1);
     return t.parent && t.from == e
 }
 
-function bw(n, e, t, i) {
+function xw(n, e, t, i) {
     let r = lt(n).resolveInner(e, -1),
         s = i.reduce((o, l) => Math.max(o, l.length), 0);
     for (let o = 0; o < 5; o++) {
         let l = n.sliceDoc(r.from, Math.min(r.to, r.from + t.length + s)),
             h = l.indexOf(t);
         if (!h || h > -1 && i.indexOf(l.slice(0, h)) > -1) {
             let u = r.firstChild;
@@ -18525,23 +18525,23 @@
     for (let r of t) {
         let s = e - r.length;
         if (n.sliceDoc(s, e) == r && i(n.sliceDoc(s - 1, s)) != Ve.Word) return s
     }
     return -1
 }
 
-function xw(n = {}) {
-    return [Ut, Ct.of(n), ow, kw, lw]
+function kw(n = {}) {
+    return [Ut, Ct.of(n), lw, ww, aw]
 }
 const _g = [{
         key: "Ctrl-Space",
-        run: tw
+        run: iw
     }, {
         key: "Escape",
-        run: iw
+        run: nw
     }, {
         key: "ArrowDown",
         run: ko(!0)
     }, {
         key: "ArrowUp",
         run: ko(!1)
     }, {
@@ -18550,30 +18550,30 @@
     }, {
         key: "PageUp",
         run: ko(!1, "page")
     }, {
         key: "Enter",
         run: Lg
     }],
-    kw = Kn.highest(xl.computeN([Ct], n => n.facet(Ct).defaultKeymap ? [_g] : []));
-class ww {
+    ww = Kn.highest(xl.computeN([Ct], n => n.facet(Ct).defaultKeymap ? [_g] : []));
+class vw {
     constructor(e, t, i) {
         this.from = e, this.to = t, this.diagnostic = i
     }
 }
 class $n {
     constructor(e, t, i) {
         this.diagnostics = e, this.panel = t, this.selected = i
     }
     static init(e, t, i) {
         let r = e,
             s = i.facet(zg).markerFilter;
         s && (r = s(r));
         let o = de.set(r.map(l => l.from == l.to || l.from == l.to - 1 && i.doc.lineAt(l.from).to == l.from ? de.widget({
-            widget: new Dw(l),
+            widget: new Rw(l),
             diagnostic: l
         }).range(l.from) : de.mark({
             attributes: {
                 class: "cm-lintRange cm-lintRange-" + l.severity + (l.markClass ? " " + l.markClass : "")
             },
             diagnostic: l
         }).range(l.from, l.to)), !0);
@@ -18582,25 +18582,25 @@
 }
 
 function Ar(n, e = null, t = 0) {
     let i = null;
     return n.between(t, 1e9, (r, s, {
         spec: o
     }) => {
-        if (!(e && o.diagnostic != e)) return i = new ww(r, s, o.diagnostic), !1
+        if (!(e && o.diagnostic != e)) return i = new vw(r, s, o.diagnostic), !1
     }), i
 }
 
-function vw(n, e) {
+function Sw(n, e) {
     let t = n.startState.doc.lineAt(e.pos);
     return !!(n.effects.some(i => i.is(Hg)) || n.changes.touchesRange(t.from, t.to))
 }
 
-function Sw(n, e) {
-    return n.field(Gt, !1) ? e : e.concat(me.appendConfig.of(Pw))
+function Cw(n, e) {
+    return n.field(Gt, !1) ? e : e.concat(me.appendConfig.of(Nw))
 }
 const Hg = me.define(),
     oc = me.define(),
     Fg = me.define(),
     Gt = yt.define({
         create() {
             return new $n(de.none, null, null)
@@ -18616,19 +18616,19 @@
                 n = new $n(t, n.panel, i)
             }
             for (let t of e.effects) t.is(Hg) ? n = $n.init(t.value, n.panel, e.state) : t.is(oc) ? n = new $n(n.diagnostics, t.value ? El.open : null, n.selected) : t.is(Fg) && (n = new $n(n.diagnostics, n.panel, t.value));
             return n
         },
         provide: n => [xs.from(n, e => e.panel), te.decorations.from(n, e => e.diagnostics)]
     }),
-    Cw = de.mark({
+    Aw = de.mark({
         class: "cm-lintRange cm-lintRange-active"
     });
 
-function Aw(n, e, t) {
+function Tw(n, e, t) {
     let {
         diagnostics: i
     } = n.state.field(Gt), r = [], s = 2e8, o = 0;
     i.between(e - (t < 0 ? 1 : 0), e + (t > 0 ? 1 : 0), (h, f, {
         spec: u
     }) => {
         e >= h && e <= f && (h == f || (e > h || t > 0) && (e < f || t < 0)) && (r.push(u.diagnostic), s = Math.min(h, s), o = Math.max(f, o))
@@ -18636,59 +18636,59 @@
     let l = n.state.facet(zg).tooltipFilter;
     return l && (r = l(r)), r.length ? {
         pos: s,
         end: o,
         above: n.state.doc.lineAt(s).to < o,
         create() {
             return {
-                dom: Tw(n, r)
+                dom: Ow(n, r)
             }
         }
     } : null
 }
 
-function Tw(n, e) {
+function Ow(n, e) {
     return $e("ul", {
         class: "cm-tooltip-lint"
     }, e.map(t => Wg(n, t, !1)))
 }
-const Ow = n => {
+const Mw = n => {
         let e = n.state.field(Gt, !1);
         (!e || !e.panel) && n.dispatch({
-            effects: Sw(n.state, [oc.of(!0)])
+            effects: Cw(n.state, [oc.of(!0)])
         });
         let t = bs(n, El.open);
         return t && t.dom.querySelector(".cm-panel-lint ul").focus(), !0
     },
     gu = n => {
         let e = n.state.field(Gt, !1);
         return !e || !e.panel ? !1 : (n.dispatch({
             effects: oc.of(!1)
         }), !0)
     },
-    Mw = n => {
+    Ew = n => {
         let e = n.state.field(Gt, !1);
         if (!e) return !1;
         let t = n.state.selection.main,
             i = e.diagnostics.iter(t.to + 1);
         return !i.value && (i = e.diagnostics.iter(0), !i.value || i.from == t.from && i.to == t.to) ? !1 : (n.dispatch({
             selection: {
                 anchor: i.from,
                 head: i.to
             },
             scrollIntoView: !0
         }), !0)
     },
-    Ew = [{
+    Dw = [{
         key: "Mod-Shift-m",
-        run: Ow,
+        run: Mw,
         preventDefault: !0
     }, {
         key: "F8",
-        run: Mw
+        run: Ew
     }],
     zg = Z.define({
         combine(n) {
             return Object.assign({
                 sources: n.map(e => e.source)
             }, Hi(n.map(e => e.config), {
                 delay: 750,
@@ -18734,27 +18734,27 @@
                 let k = Ar(n.state.field(Gt).diagnostics, e);
                 k && s.apply(n, k.from, k.to)
             },
             {
                 name: f
             } = s,
             u = r[o] ? f.indexOf(r[o]) : -1,
-            g = u < 0 ? f : [f.slice(0, u), $e("u", f.slice(u, u + 1)), f.slice(u + 1)];
+            m = u < 0 ? f : [f.slice(0, u), $e("u", f.slice(u, u + 1)), f.slice(u + 1)];
         return $e("button", {
             type: "button",
             class: "cm-diagnosticAction",
             onclick: h,
             onmousedown: h,
             "aria-label": ` Action: ${f}${u<0?"":` (access key "${r[o]})"`}.`
-        }, g)
+        }, m)
     }), e.source && $e("div", {
         class: "cm-diagnosticSource"
     }, e.source))
 }
-class Dw extends An {
+class Rw extends An {
     constructor(e) {
         super(), this.diagnostic = e
     }
     eq(e) {
         return e.diagnostic == this.diagnostic
     }
     toDOM() {
@@ -18821,17 +18821,17 @@
             selected: t
         } = this.view.state.field(Gt), i = 0, r = !1, s = null;
         for (e.between(0, this.view.state.doc.length, (o, l, {
                 spec: h
             }) => {
                 let f = -1,
                     u;
-                for (let g = i; g < this.items.length; g++)
-                    if (this.items[g].diagnostic == h.diagnostic) {
-                        f = g;
+                for (let m = i; m < this.items.length; m++)
+                    if (this.items[m].diagnostic == h.diagnostic) {
+                        f = m;
                         break
                     } f < 0 ? (u = new mu(this.view, h.diagnostic), this.items.splice(i, 0, u), r = !0) : (u = this.items[f], f > i && (this.items.splice(i, f - i), r = !0)), t && u.diagnostic == t.diagnostic ? u.dom.hasAttribute("aria-selected") || (u.dom.setAttribute("aria-selected", "true"), s = u) : u.dom.hasAttribute("aria-selected") && u.dom.removeAttribute("aria-selected"), i++
             }); i < this.items.length && !(this.items.length == 1 && this.items[0].diagnostic.from < 0);) r = !0, this.items.pop();
         this.items.length == 0 && (this.items.push(new mu(this.view, {
             from: -1,
             to: -1,
             severity: "info",
@@ -18879,22 +18879,22 @@
         })
     }
     static open(e) {
         return new El(e)
     }
 }
 
-function Rw(n, e = 'viewBox="0 0 40 40"') {
+function Lw(n, e = 'viewBox="0 0 40 40"') {
     return `url('data:image/svg+xml,<svg xmlns="http://www.w3.org/2000/svg" ${e}>${encodeURIComponent(n)}</svg>')`
 }
 
 function wo(n) {
-    return Rw(`<path d="m0 2.5 l2 -1.5 l1 0 l2 1.5 l1 0" stroke="${n}" fill="none" stroke-width=".7"/>`, 'width="6" height="3"')
+    return Lw(`<path d="m0 2.5 l2 -1.5 l1 0 l2 1.5 l1 0" stroke="${n}" fill="none" stroke-width=".7"/>`, 'width="6" height="3"')
 }
-const Lw = te.baseTheme({
+const Pw = te.baseTheme({
         ".cm-diagnostic": {
             padding: "3px 6px 3px 8px",
             marginLeft: "-1px",
             display: "block",
             whiteSpace: "pre-wrap"
         },
         ".cm-diagnostic-error": {
@@ -19005,27 +19005,27 @@
                 border: "none",
                 font: "inherit",
                 padding: 0,
                 margin: 0
             }
         }
     }),
-    Pw = [Gt, te.decorations.compute([Gt], n => {
+    Nw = [Gt, te.decorations.compute([Gt], n => {
         let {
             selected: e,
             panel: t
         } = n.field(Gt);
-        return !e || !t || e.from == e.to ? de.none : de.set([Cw.range(e.from, e.to)])
-    }), Lb(Aw, {
-        hideOn: vw
-    }), Lw];
+        return !e || !t || e.from == e.to ? de.none : de.set([Aw.range(e.from, e.to)])
+    }), Pb(Tw, {
+        hideOn: Sw
+    }), Pw];
 var yu = {};
 class al {
-    constructor(e, t, i, r, s, o, l, h, f, u = 0, g) {
-        this.p = e, this.stack = t, this.state = i, this.reducePos = r, this.pos = s, this.score = o, this.buffer = l, this.bufferBase = h, this.curContext = f, this.lookAhead = u, this.parent = g
+    constructor(e, t, i, r, s, o, l, h, f, u = 0, m) {
+        this.p = e, this.stack = t, this.state = i, this.reducePos = r, this.pos = s, this.score = o, this.buffer = l, this.bufferBase = h, this.curContext = f, this.lookAhead = u, this.parent = m
     }
     toString() {
         return `[${this.stack.filter((e,t)=>t%3==0).concat(this.state)}]@${this.pos}${this.score?"!"+this.score:""}`
     }
     static start(e, t, i = 0) {
         let r = e.parser.context;
         return new al(e, [], t, i, i, 0, [], 0, r ? new bu(r, r.start) : null, 0, null)
@@ -19049,18 +19049,18 @@
             return
         }
         let l = this.stack.length - (i - 1) * 3 - (e & 262144 ? 6 : 0),
             h = l ? this.stack[l - 2] : this.p.ranges[0].from,
             f = this.reducePos - h;
         f >= 2e3 && !(!((t = this.p.parser.nodeSet.types[r]) === null || t === void 0) && t.isAnonymous) && (h == this.p.lastBigReductionStart ? (this.p.bigReductionCount++, this.p.lastBigReductionSize = f) : this.p.lastBigReductionSize < f && (this.p.bigReductionCount = 1, this.p.lastBigReductionStart = h, this.p.lastBigReductionSize = f));
         let u = l ? this.stack[l - 1] : 0,
-            g = this.bufferBase + this.buffer.length - u;
+            m = this.bufferBase + this.buffer.length - u;
         if (r < s.minRepeatTerm || e & 131072) {
             let y = s.stateFlag(this.state, 1) ? this.pos : this.reducePos;
-            this.storeNode(r, h, y, g + 4, !0)
+            this.storeNode(r, h, y, m + 4, !0)
         }
         if (e & 262144) this.state = this.stack[l];
         else {
             let y = this.stack[l - 3];
             this.state = s.getGoto(y, r, !0)
         }
         for (; this.stack.length > l;) this.stack.pop();
@@ -19116,15 +19116,15 @@
         return new al(this.p, this.stack.slice(), this.state, this.reducePos, this.pos, this.score, i, r, this.curContext, this.lookAhead, e)
     }
     recoverByDelete(e, t) {
         let i = e <= this.p.parser.maxNode;
         i && this.storeNode(e, this.pos, t, 4), this.storeNode(0, this.pos, t, i ? 8 : 4), this.pos = this.reducePos = t, this.score -= 190
     }
     canShift(e) {
-        for (let t = new Nw(this);;) {
+        for (let t = new Iw(this);;) {
             let i = this.p.parser.stateSlot(t.state, 4) || this.p.parser.hasAction(t.state, e);
             if (i == 0) return !1;
             if (!(i & 65536)) return !0;
             t.reduce(i)
         }
     }
     recoverByInsert(e) {
@@ -19245,15 +19245,15 @@
     }
 }
 class bu {
     constructor(e, t) {
         this.tracker = e, this.context = t, this.hash = e.strict ? e.hash(t) : 0
     }
 }
-class Nw {
+class Iw {
     constructor(e) {
         this.start = e, this.state = e.state, this.stack = e.stack, this.base = this.stack.length
     }
     reduce(e) {
         let t = e & 65535,
             i = e >> 19;
         i == 0 ? (this.stack == this.start.stack && (this.stack = this.stack.slice()), this.stack.push(this.state, 0, 0), this.base += 3) : this.base -= (i - 1) * 3;
@@ -19315,15 +19315,15 @@
 }
 class _o {
     constructor() {
         this.start = -1, this.value = -1, this.end = -1, this.extended = -1, this.lookAhead = 0, this.mask = 0, this.context = 0
     }
 }
 const xu = new _o;
-class Iw {
+class Bw {
     constructor(e, t) {
         this.input = e, this.ranges = t, this.chunk = "", this.chunkOff = 0, this.chunk2 = "", this.chunk2Pos = 0, this.next = -1, this.token = xu, this.rangeIndex = 0, this.pos = this.chunkPos = t[0].from, this.range = t[0], this.end = t[t.length - 1].to, this.readNext()
     }
     resolveOffset(e, t) {
         let i = this.range,
             r = this.rangeIndex,
             s = this.pos + e;
@@ -19419,54 +19419,54 @@
     constructor(e, t) {
         this.data = e, this.id = t
     }
     token(e, t) {
         let {
             parser: i
         } = t.p;
-        _w(this.data, e, t, this.id, i.data, i.tokenPrecTable)
+        Hw(this.data, e, t, this.id, i.data, i.tokenPrecTable)
     }
 }
 kr.prototype.contextual = kr.prototype.fallback = kr.prototype.extend = !1;
 kr.prototype.fallback = kr.prototype.extend = !1;
-class Bw {
+class _w {
     constructor(e, t = {}) {
         this.token = e, this.contextual = !!t.contextual, this.fallback = !!t.fallback, this.extend = !!t.extend
     }
 }
 
-function _w(n, e, t, i, r, s) {
+function Hw(n, e, t, i, r, s) {
     let o = 0,
         l = 1 << i,
         {
             dialect: h
         } = t.p.parser;
     e: for (; l & n[o];) {
         let f = n[o + 1];
         for (let k = o + 3; k < f; k += 2)
             if ((n[k + 1] & l) > 0) {
                 let v = n[k];
-                if (h.allows(v) && (e.token.value == -1 || e.token.value == v || Hw(v, e.token.value, r, s))) {
+                if (h.allows(v) && (e.token.value == -1 || e.token.value == v || Fw(v, e.token.value, r, s))) {
                     e.acceptToken(v);
                     break
                 }
             } let u = e.next,
-            g = 0,
+            m = 0,
             y = n[o + 2];
-        if (e.next < 0 && y > g && n[f + y * 3 - 3] == 65535) {
+        if (e.next < 0 && y > m && n[f + y * 3 - 3] == 65535) {
             o = n[f + y * 3 - 1];
             continue e
         }
-        for (; g < y;) {
-            let k = g + y >> 1,
+        for (; m < y;) {
+            let k = m + y >> 1,
                 v = f + k + (k << 1),
-                C = n[v],
+                A = n[v],
                 O = n[v + 1] || 65536;
-            if (u < C) y = k;
-            else if (u >= O) g = k + 1;
+            if (u < A) y = k;
+            else if (u >= O) m = k + 1;
             else {
                 o = n[v + 2], e.advance();
                 continue e
             }
         }
         break
     }
@@ -19475,15 +19475,15 @@
 function ku(n, e, t) {
     for (let i = e, r;
         (r = n[i]) != 65535; i++)
         if (r == t) return i - e;
     return -1
 }
 
-function Hw(n, e, t, i) {
+function Fw(n, e, t, i) {
     let r = ku(t, i, e);
     return r < 0 || ku(t, i, n) < r
 }
 const Wt = typeof process != "undefined" && yu && /\bparse\b/.test(yu.LOG);
 let Sa = null;
 
 function wu(n, e, t) {
@@ -19492,15 +19492,15 @@
         if (!(t < 0 ? i.childBefore(e) : i.childAfter(e)))
             for (;;) {
                 if ((t < 0 ? i.to < e : i.from > e) && !i.type.isError) return t < 0 ? Math.max(0, Math.min(i.to - 1, e - 25)) : Math.min(n.length, Math.max(i.from + 1, e + 25));
                 if (t < 0 ? i.prevSibling() : i.nextSibling()) break;
                 if (!i.parent()) return t < 0 ? 0 : n.length
             }
 }
-class Fw {
+class zw {
     constructor(e, t) {
         this.fragments = e, this.nodeSet = t, this.i = 0, this.fragment = null, this.safeFrom = -1, this.safeTo = -1, this.trees = [], this.start = [], this.index = [], this.nextFragment()
     }
     nextFragment() {
         let e = this.fragment = this.i == this.fragments.length ? null : this.fragments[this.i++];
         if (e) {
             for (this.safeFrom = e.openStart ? wu(e.tree, e.from + e.offset, 1) - e.offset : e.from, this.safeTo = e.openEnd ? wu(e.tree, e.to + e.offset, -1) - e.offset : e.to; this.trees.length;) this.trees.pop(), this.start.pop(), this.index.pop();
@@ -19533,15 +19533,15 @@
                     }
                 }
                 this.index[t]++, o + s.length >= Math.max(this.safeFrom, e) && (this.trees.push(s), this.start.push(o), this.index.push(0))
             } else this.index[t]++, this.nextStart = o + s.length
         }
     }
 }
-class zw {
+class $w {
     constructor(e, t) {
         this.stream = t, this.tokens = [], this.mainToken = null, this.actions = [], this.tokens = e.tokenizers.map(i => new _o)
     }
     getActions(e) {
         let t = 0,
             i = null,
             {
@@ -19552,18 +19552,18 @@
             } = r,
             o = r.stateSlot(e.state, 3),
             l = e.curContext ? e.curContext.hash : 0,
             h = 0;
         for (let f = 0; f < s.length; f++) {
             if (!(1 << f & o)) continue;
             let u = s[f],
-                g = this.tokens[f];
-            if (!(i && !u.fallback) && ((u.contextual || g.start != e.pos || g.mask != o || g.context != l) && (this.updateCachedToken(g, u, e), g.mask = o, g.context = l), g.lookAhead > g.end + 25 && (h = Math.max(g.lookAhead, h)), g.value != 0)) {
+                m = this.tokens[f];
+            if (!(i && !u.fallback) && ((u.contextual || m.start != e.pos || m.mask != o || m.context != l) && (this.updateCachedToken(m, u, e), m.mask = o, m.context = l), m.lookAhead > m.end + 25 && (h = Math.max(m.lookAhead, h)), m.value != 0)) {
                 let y = t;
-                if (g.extended > -1 && (t = this.addActions(e, g.extended, g.end, t)), t = this.addActions(e, g.value, g.end, t), !u.extend && (i = g, t > y)) break
+                if (m.extended > -1 && (t = this.addActions(e, m.extended, m.end, t)), t = this.addActions(e, m.value, m.end, t), !u.extend && (i = m, t > y)) break
             }
         }
         for (; this.actions.length > t;) this.actions.pop();
         return h && e.setLookAhead(h), !i && e.pos == this.stream.end && (i = new _o, i.value = e.p.parser.eofTerm, i.start = i.end = e.pos, t = this.addActions(e, i.value, i.end, t)), this.mainToken = i, this.actions
     }
     getMainToken(e) {
         if (this.mainToken) return this.mainToken;
@@ -19611,21 +19611,21 @@
                         r == 0 && l[f + 1] == 2 && (r = this.putAction(Vi(l, f + 2), t, i, r));
                         break
                     } l[f] == t && (r = this.putAction(Vi(l, f + 1), t, i, r))
             }
         return r
     }
 }
-class $w {
+class Ww {
     constructor(e, t, i, r) {
-        this.parser = e, this.input = t, this.ranges = r, this.recovering = 0, this.nextStackID = 9812, this.minStackPos = 0, this.reused = [], this.stoppedAt = null, this.lastBigReductionStart = -1, this.lastBigReductionSize = 0, this.bigReductionCount = 0, this.stream = new Iw(t, r), this.tokens = new zw(e, this.stream), this.topTerm = e.top[1];
+        this.parser = e, this.input = t, this.ranges = r, this.recovering = 0, this.nextStackID = 9812, this.minStackPos = 0, this.reused = [], this.stoppedAt = null, this.lastBigReductionStart = -1, this.lastBigReductionSize = 0, this.bigReductionCount = 0, this.stream = new Bw(t, r), this.tokens = new $w(e, this.stream), this.topTerm = e.top[1];
         let {
             from: s
         } = r[0];
-        this.stacks = [al.start(this, e.top[0], s)], this.fragments = i.length && this.stream.end - s > e.bufferLength * 4 ? new Fw(i, e.nodeSet) : null
+        this.stacks = [al.start(this, e.top[0], s)], this.fragments = i.length && this.stream.end - s > e.bufferLength * 4 ? new zw(i, e.nodeSet) : null
     }
     get parsedPos() {
         return this.minStackPos
     }
     advance() {
         let e = this.stacks,
             t = this.minStackPos,
@@ -19648,15 +19648,15 @@
                         s.push(h.value, h.end)
                     }
                 }
                 break
             }
         }
         if (!i.length) {
-            let o = r && qw(r);
+            let o = r && jw(r);
             if (o) return Wt && console.log("Finish with " + this.stackID(o)), this.stackToTree(o);
             if (this.parser.strict) throw Wt && r && console.log("Stuck with token " + (this.tokens.mainToken ? this.parser.getName(this.tokens.mainToken.value) : "none")), new SyntaxError("No parse at " + t);
             this.recovering || (this.recovering = 5)
         }
         if (this.recovering && r) {
             let o = this.stoppedAt != null && r[0].pos > this.stoppedAt ? r[0] : this.runRecovery(r, s, i);
             if (o) return Wt && console.log("Force-finish " + this.stackID(o)), this.stackToTree(o.forceAll())
@@ -19695,36 +19695,36 @@
                 parser: s
             } = this,
             o = Wt ? this.stackID(e) + " -> " : "";
         if (this.stoppedAt != null && r > this.stoppedAt) return e.forceReduce() ? e : null;
         if (this.fragments) {
             let f = e.curContext && e.curContext.tracker.strict,
                 u = f ? e.curContext.hash : 0;
-            for (let g = this.fragments.nodeAt(r); g;) {
-                let y = this.parser.nodeSet.types[g.type.id] == g.type ? s.getGoto(e.state, g.type.id) : -1;
-                if (y > -1 && g.length && (!f || (g.prop(Se.contextHash) || 0) == u)) return e.useNode(g, y), Wt && console.log(o + this.stackID(e) + ` (via reuse of ${s.getName(g.type.id)})`), !0;
-                if (!(g instanceof Je) || g.children.length == 0 || g.positions[0] > 0) break;
-                let k = g.children[0];
-                if (k instanceof Je && g.positions[0] == 0) g = k;
+            for (let m = this.fragments.nodeAt(r); m;) {
+                let y = this.parser.nodeSet.types[m.type.id] == m.type ? s.getGoto(e.state, m.type.id) : -1;
+                if (y > -1 && m.length && (!f || (m.prop(Se.contextHash) || 0) == u)) return e.useNode(m, y), Wt && console.log(o + this.stackID(e) + ` (via reuse of ${s.getName(m.type.id)})`), !0;
+                if (!(m instanceof Je) || m.children.length == 0 || m.positions[0] > 0) break;
+                let k = m.children[0];
+                if (k instanceof Je && m.positions[0] == 0) m = k;
                 else break
             }
         }
         let l = s.stateSlot(e.state, 4);
         if (l > 0) return e.reduce(l), Wt && console.log(o + this.stackID(e) + ` (via always-reduce ${s.getName(l&65535)})`), !0;
         if (e.stack.length >= 8400)
             for (; e.stack.length > 6e3 && e.forceReduce(););
         let h = this.tokens.getActions(e);
         for (let f = 0; f < h.length;) {
             let u = h[f++],
-                g = h[f++],
+                m = h[f++],
                 y = h[f++],
                 k = f == h.length || !i,
                 v = k ? e : e.split(),
-                C = this.tokens.mainToken;
-            if (v.apply(u, g, C ? C.start : v.pos, y), Wt && console.log(o + this.stackID(v) + ` (via ${u&65536?`reduce of ${s.getName(u&65535)}`:"shift"} for ${s.getName(g)} @ ${r}${v==e?"":", split"})`), k) return !0;
+                A = this.tokens.mainToken;
+            if (v.apply(u, m, A ? A.start : v.pos, y), Wt && console.log(o + this.stackID(v) + ` (via ${u&65536?`reduce of ${s.getName(u&65535)}`:"shift"} for ${s.getName(m)} @ ${r}${v==e?"":", split"})`), k) return !0;
             v.pos > r ? t.push(v) : i.push(v)
         }
         return !1
     }
     advanceFully(e, t) {
         let i = e.pos;
         for (;;) {
@@ -19737,17 +19737,17 @@
             s = !1;
         for (let o = 0; o < e.length; o++) {
             let l = e[o],
                 h = t[o << 1],
                 f = t[(o << 1) + 1],
                 u = Wt ? this.stackID(l) + " -> " : "";
             if (l.deadEnd && (s || (s = !0, l.restart(), Wt && console.log(u + this.stackID(l) + " (restarted)"), this.advanceFully(l, i)))) continue;
-            let g = l.split(),
+            let m = l.split(),
                 y = u;
-            for (let k = 0; g.forceReduce() && k < 10 && (Wt && console.log(y + this.stackID(g) + " (via force-reduce)"), !this.advanceFully(g, i)); k++) Wt && (y = this.stackID(g) + " -> ");
+            for (let k = 0; m.forceReduce() && k < 10 && (Wt && console.log(y + this.stackID(m) + " (via force-reduce)"), !this.advanceFully(m, i)); k++) Wt && (y = this.stackID(m) + " -> ");
             for (let k of l.recoverByInsert(h)) Wt && console.log(u + this.stackID(k) + " (via recover-insert)"), this.advanceFully(k, i);
             this.stream.end > l.pos ? (f == l.pos && (f++, h = 0), l.recoverByDelete(h, f), Wt && console.log(u + this.stackID(l) + ` (via recover-delete ${this.parser.getName(h)})`), vu(l, i)) : (!r || r.score < l.score) && (r = l)
         }
         return r
     }
     stackToTree(e) {
         return e.close(), Je.build({
@@ -19773,15 +19773,15 @@
         if (i.pos == n.pos && i.sameState(n)) {
             e[t].score < n.score && (e[t] = n);
             return
         }
     }
     e.push(n)
 }
-class Ww {
+class qw {
     constructor(e, t, i) {
         this.source = e, this.flags = t, this.disabled = i
     }
     allows(e) {
         return !this.disabled || this.disabled[e] == 0
     }
 }
@@ -19802,16 +19802,16 @@
             for (let l of e.nodeProps) {
                 let h = l[0];
                 typeof h == "string" && (h = Se[h]);
                 for (let f = 1; f < l.length;) {
                     let u = l[f++];
                     if (u >= 0) s(u, h, l[f++]);
                     else {
-                        let g = l[f + -u];
-                        for (let y = -u; y > 0; y--) s(l[f++], h, g);
+                        let m = l[f + -u];
+                        for (let y = -u; y > 0; y--) s(l[f++], h, m);
                         f++
                     }
                 }
             }
         this.nodeSet = new qh(t.map((l, h) => Ht.define({
             name: h >= this.minRepeatTerm ? void 0 : l,
             id: h,
@@ -19822,15 +19822,15 @@
         }))), e.propSources && (this.nodeSet = this.nodeSet.extend(...e.propSources)), this.strict = !1, this.bufferLength = yp;
         let o = vo(e.tokenData);
         this.context = e.context, this.specializerSpecs = e.specialized || [], this.specialized = new Uint16Array(this.specializerSpecs.length);
         for (let l = 0; l < this.specializerSpecs.length; l++) this.specialized[l] = this.specializerSpecs[l].term;
         this.specializers = this.specializerSpecs.map(Su), this.states = vo(e.states, Uint32Array), this.data = vo(e.stateData), this.goto = vo(e.goto), this.maxTerm = e.maxTerm, this.tokenizers = e.tokenizers.map(l => typeof l == "number" ? new kr(o, l) : l), this.topRules = e.topRules, this.dialects = e.dialects || {}, this.dynamicPrecedences = e.dynamicPrecedences || null, this.tokenPrecTable = e.tokenPrec, this.termNames = e.termNames || null, this.maxNode = this.nodeSet.types.length - 1, this.dialect = this.parseDialect(), this.top = this.topRules[Object.keys(this.topRules)[0]]
     }
     createParse(e, t, i) {
-        let r = new $w(this, e, t, i);
+        let r = new Ww(this, e, t, i);
         for (let s of this.wrappers) r = s(r, e, t, i);
         return r
     }
     getGoto(e, t, i = !1) {
         let r = this.goto;
         if (t >= r[0]) return -1;
         for (let s = r[t + 1];;) {
@@ -19933,26 +19933,26 @@
                 o >= 0 && (i[o] = !0)
             }
         let r = null;
         for (let s = 0; s < t.length; s++)
             if (!i[s])
                 for (let o = this.dialects[t[s]], l;
                     (l = this.data[o++]) != 65535;)(r || (r = new Uint8Array(this.maxTerm + 1)))[l] = 1;
-        return new Ww(e, i, r)
+        return new qw(e, i, r)
     }
     static deserialize(e) {
         return new cl(e)
     }
 }
 
 function Vi(n, e) {
     return n[e] | n[e + 1] << 16
 }
 
-function qw(n) {
+function jw(n) {
     let e = null;
     for (let t of n) {
         let i = t.p.stoppedAt;
         (t.pos == t.p.stream.end || i != null && t.pos > i) && t.p.parser.stateFlag(t.state, 2) && (!e || e.score < t.score) && (e = t)
     }
     return e
 }
@@ -19960,71 +19960,71 @@
 function Su(n) {
     if (n.external) {
         let e = n.extend ? 1 : 0;
         return (t, i) => n.external(t, i) << 1 | e
     }
     return n.get
 }
-const jw = 36,
+const Vw = 36,
     Cu = 1,
-    Vw = 2,
+    Uw = 2,
     Gr = 3,
     Ca = 4,
-    Uw = 5,
-    Qw = 6,
-    Gw = 7,
-    Kw = 8,
-    Xw = 9,
-    Yw = 10,
-    Jw = 11,
-    Zw = 12,
-    ev = 13,
-    tv = 14,
-    iv = 15,
-    nv = 16,
-    rv = 17,
+    Qw = 5,
+    Gw = 6,
+    Kw = 7,
+    Xw = 8,
+    Yw = 9,
+    Jw = 10,
+    Zw = 11,
+    ev = 12,
+    tv = 13,
+    iv = 14,
+    nv = 15,
+    rv = 16,
+    sv = 17,
     Au = 18,
-    sv = 19,
+    ov = 19,
     qg = 20,
     jg = 21,
     Tu = 22,
-    ov = 23,
-    lv = 24;
+    lv = 23,
+    av = 24;
 
 function Ch(n) {
     return n >= 65 && n <= 90 || n >= 97 && n <= 122 || n >= 48 && n <= 57
 }
 
-function av(n) {
+function hv(n) {
     return n >= 48 && n <= 57 || n >= 97 && n <= 102 || n >= 65 && n <= 70
 }
 
 function Hn(n, e, t) {
     for (let i = !1;;) {
         if (n.next < 0) return;
         if (n.next == e && !i) {
             n.advance();
             return
         }
         i = t && !i && n.next == 92, n.advance()
     }
 }
 
-function hv(n) {
+function cv(n) {
     for (;;) {
         if (n.next < 0 || n.peek(1) < 0) return;
         if (n.next == 36 && n.peek(1) == 36) {
             n.advance(2);
             return
         }
         n.advance()
     }
 }
 
-function cv(n, e) {
+function fv(n, e) {
     let t = "[{<(".indexOf(String.fromCharCode(e)),
         i = t < 0 ? e : "]}>)".charCodeAt(t);
     for (;;) {
         if (n.next < 0) return;
         if (n.next == i && n.peek(1) == 39) {
             n.advance(2);
             return
@@ -20034,15 +20034,15 @@
 }
 
 function Vg(n, e) {
     for (; !(n.next != 95 && !Ch(n.next));) e != null && (e += String.fromCharCode(n.next)), n.advance();
     return e
 }
 
-function fv(n) {
+function uv(n) {
     if (n.next == 39 || n.next == 34 || n.next == 96) {
         let e = n.next;
         n.advance(), Hn(n, e, !1)
     } else Vg(n)
 }
 
 function Ou(n, e) {
@@ -20072,113 +20072,113 @@
     return !1
 }
 const Aa = ` 	\r
 `;
 
 function Ug(n, e, t) {
     let i = Object.create(null);
-    i.true = i.false = Uw, i.null = i.unknown = Qw;
+    i.true = i.false = Qw, i.null = i.unknown = Gw;
     for (let r of n.split(" ")) r && (i[r] = qg);
     for (let r of e.split(" ")) r && (i[r] = jg);
-    for (let r of (t || "").split(" ")) r && (i[r] = lv);
+    for (let r of (t || "").split(" ")) r && (i[r] = av);
     return i
 }
-const uv = "array binary bit boolean char character clob date decimal double float int integer interval large national nchar nclob numeric object precision real smallint time timestamp varchar varying ",
-    dv = "absolute action add after all allocate alter and any are as asc assertion at authorization before begin between both breadth by call cascade cascaded case cast catalog check close collate collation column commit condition connect connection constraint constraints constructor continue corresponding count create cross cube current current_date current_default_transform_group current_transform_group_for_type current_path current_role current_time current_timestamp current_user cursor cycle data day deallocate declare default deferrable deferred delete depth deref desc describe descriptor deterministic diagnostics disconnect distinct do domain drop dynamic each else elseif end end-exec equals escape except exception exec execute exists exit external fetch first for foreign found from free full function general get global go goto grant group grouping handle having hold hour identity if immediate in indicator initially inner inout input insert intersect into is isolation join key language last lateral leading leave left level like limit local localtime localtimestamp locator loop map match method minute modifies module month names natural nesting new next no none not of old on only open option or order ordinality out outer output overlaps pad parameter partial path prepare preserve primary prior privileges procedure public read reads recursive redo ref references referencing relative release repeat resignal restrict result return returns revoke right role rollback rollup routine row rows savepoint schema scroll search second section select session session_user set sets signal similar size some space specific specifictype sql sqlexception sqlstate sqlwarning start state static system_user table temporary then timezone_hour timezone_minute to trailing transaction translation treat trigger under undo union unique unnest until update usage user using value values view when whenever where while with without work write year zone ",
+const dv = "array binary bit boolean char character clob date decimal double float int integer interval large national nchar nclob numeric object precision real smallint time timestamp varchar varying ",
+    pv = "absolute action add after all allocate alter and any are as asc assertion at authorization before begin between both breadth by call cascade cascaded case cast catalog check close collate collation column commit condition connect connection constraint constraints constructor continue corresponding count create cross cube current current_date current_default_transform_group current_transform_group_for_type current_path current_role current_time current_timestamp current_user cursor cycle data day deallocate declare default deferrable deferred delete depth deref desc describe descriptor deterministic diagnostics disconnect distinct do domain drop dynamic each else elseif end end-exec equals escape except exception exec execute exists exit external fetch first for foreign found from free full function general get global go goto grant group grouping handle having hold hour identity if immediate in indicator initially inner inout input insert intersect into is isolation join key language last lateral leading leave left level like limit local localtime localtimestamp locator loop map match method minute modifies module month names natural nesting new next no none not of old on only open option or order ordinality out outer output overlaps pad parameter partial path prepare preserve primary prior privileges procedure public read reads recursive redo ref references referencing relative release repeat resignal restrict result return returns revoke right role rollback rollup routine row rows savepoint schema scroll search second section select session session_user set sets signal similar size some space specific specifictype sql sqlexception sqlstate sqlwarning start state static system_user table temporary then timezone_hour timezone_minute to trailing transaction translation treat trigger under undo union unique unnest until update usage user using value values view when whenever where while with without work write year zone ",
     Ah = {
         backslashEscapes: !1,
         hashComments: !1,
         spaceAfterDashes: !1,
         slashComments: !1,
         doubleQuotedStrings: !1,
         doubleDollarQuotedStrings: !1,
         unquotedBitLiterals: !1,
         treatBitsAsBytes: !1,
         charSetCasts: !1,
         plsqlQuotingMechanism: !1,
         operatorChars: "*+-%<>!=&|~^/",
         specialVar: "?",
         identifierQuotes: '"',
-        words: Ug(dv, uv)
+        words: Ug(pv, dv)
     };
 
-function pv(n, e, t, i) {
+function gv(n, e, t, i) {
     let r = {};
     for (let s in Ah) r[s] = (n.hasOwnProperty(s) ? n : Ah)[s];
     return e && (r.words = Ug(e, t || "", i)), r
 }
 
 function Qg(n) {
-    return new Bw(e => {
+    return new _w(e => {
         var t;
         let {
             next: i
         } = e;
         if (e.advance(), _n(i, Aa)) {
             for (; _n(e.next, Aa);) e.advance();
-            e.acceptToken(jw)
-        } else if (i == 36 && e.next == 36 && n.doubleDollarQuotedStrings) hv(e), e.acceptToken(Gr);
+            e.acceptToken(Vw)
+        } else if (i == 36 && e.next == 36 && n.doubleDollarQuotedStrings) cv(e), e.acceptToken(Gr);
         else if (i == 39 || i == 34 && n.doubleQuotedStrings) Hn(e, i, n.backslashEscapes), e.acceptToken(Gr);
         else if (i == 35 && n.hashComments || i == 47 && e.next == 47 && n.slashComments) Eu(e), e.acceptToken(Cu);
         else if (i == 45 && e.next == 45 && (!n.spaceAfterDashes || e.peek(1) == 32)) Eu(e), e.acceptToken(Cu);
         else if (i == 47 && e.next == 42) {
             e.advance();
             for (let r = 1;;) {
                 let s = e.next;
                 if (e.next < 0) break;
                 if (e.advance(), s == 42 && e.next == 47) {
                     if (r--, e.advance(), !r) break
                 } else s == 47 && e.next == 42 && (r++, e.advance())
             }
-            e.acceptToken(Vw)
+            e.acceptToken(Uw)
         } else if ((i == 101 || i == 69) && e.next == 39) e.advance(), Hn(e, 39, !0);
         else if ((i == 110 || i == 78) && e.next == 39 && n.charSetCasts) e.advance(), Hn(e, 39, n.backslashEscapes), e.acceptToken(Gr);
         else if (i == 95 && n.charSetCasts)
             for (let r = 0;; r++) {
                 if (e.next == 39 && r > 1) {
                     e.advance(), Hn(e, 39, n.backslashEscapes), e.acceptToken(Gr);
                     break
                 }
                 if (!Ch(e.next)) break;
                 e.advance()
             } else if (n.plsqlQuotingMechanism && (i == 113 || i == 81) && e.next == 39 && e.peek(1) > 0 && !_n(e.peek(1), Aa)) {
                 let r = e.peek(1);
-                e.advance(2), cv(e, r), e.acceptToken(Gr)
-            } else if (i == 40) e.acceptToken(Gw);
-        else if (i == 41) e.acceptToken(Kw);
-        else if (i == 123) e.acceptToken(Xw);
-        else if (i == 125) e.acceptToken(Yw);
-        else if (i == 91) e.acceptToken(Jw);
-        else if (i == 93) e.acceptToken(Zw);
-        else if (i == 59) e.acceptToken(ev);
+                e.advance(2), fv(e, r), e.acceptToken(Gr)
+            } else if (i == 40) e.acceptToken(Kw);
+        else if (i == 41) e.acceptToken(Xw);
+        else if (i == 123) e.acceptToken(Yw);
+        else if (i == 125) e.acceptToken(Jw);
+        else if (i == 91) e.acceptToken(Zw);
+        else if (i == 93) e.acceptToken(ev);
+        else if (i == 59) e.acceptToken(tv);
         else if (n.unquotedBitLiterals && i == 48 && e.next == 98) e.advance(), Ou(e), e.acceptToken(Tu);
         else if ((i == 98 || i == 66) && (e.next == 39 || e.next == 34)) {
             const r = e.next;
-            e.advance(), n.treatBitsAsBytes ? (Hn(e, r, n.backslashEscapes), e.acceptToken(ov)) : (Ou(e, r), e.acceptToken(Tu))
+            e.advance(), n.treatBitsAsBytes ? (Hn(e, r, n.backslashEscapes), e.acceptToken(lv)) : (Ou(e, r), e.acceptToken(Tu))
         } else if (i == 48 && (e.next == 120 || e.next == 88) || (i == 120 || i == 88) && e.next == 39) {
             let r = e.next == 39;
-            for (e.advance(); av(e.next);) e.advance();
+            for (e.advance(); hv(e.next);) e.advance();
             r && e.next == 39 && e.advance(), e.acceptToken(Ca)
         } else if (i == 46 && e.next >= 48 && e.next <= 57) Mu(e, !0), e.acceptToken(Ca);
-        else if (i == 46) e.acceptToken(tv);
+        else if (i == 46) e.acceptToken(iv);
         else if (i >= 48 && i <= 57) Mu(e, !1), e.acceptToken(Ca);
         else if (_n(i, n.operatorChars)) {
             for (; _n(e.next, n.operatorChars);) e.advance();
-            e.acceptToken(iv)
-        } else if (_n(i, n.specialVar)) e.next == i && e.advance(), fv(e), e.acceptToken(rv);
-        else if (_n(i, n.identifierQuotes)) Hn(e, i, !1), e.acceptToken(sv);
-        else if (i == 58 || i == 44) e.acceptToken(nv);
+            e.acceptToken(nv)
+        } else if (_n(i, n.specialVar)) e.next == i && e.advance(), uv(e), e.acceptToken(sv);
+        else if (_n(i, n.identifierQuotes)) Hn(e, i, !1), e.acceptToken(ov);
+        else if (i == 58 || i == 44) e.acceptToken(rv);
         else if (Ch(i)) {
             let r = Vg(e, String.fromCharCode(i));
             e.acceptToken(e.next == 46 ? Au : (t = n.words[r.toLowerCase()]) !== null && t !== void 0 ? t : Au)
         }
     })
 }
 const Gg = Qg(Ah),
-    gv = cl.deserialize({
+    mv = cl.deserialize({
         version: 14,
         states: "%vQ]QQOOO#wQRO'#DSO$OQQO'#CwO%eQQO'#CxO%lQQO'#CyO%sQQO'#CzOOQQ'#DS'#DSOOQQ'#C}'#C}O'UQRO'#C{OOQQ'#Cv'#CvOOQQ'#C|'#C|Q]QQOOQOQQOOO'`QQO'#DOO(xQRO,59cO)PQQO,59cO)UQQO'#DSOOQQ,59d,59dO)cQQO,59dOOQQ,59e,59eO)jQQO,59eOOQQ,59f,59fO)qQQO,59fOOQQ-E6{-E6{OOQQ,59b,59bOOQQ-E6z-E6zOOQQ,59j,59jOOQQ-E6|-E6|O+VQRO1G.}O+^QQO,59cOOQQ1G/O1G/OOOQQ1G/P1G/POOQQ1G/Q1G/QP+kQQO'#C}O+rQQO1G.}O)PQQO,59cO,PQQO'#Cw",
         stateData: ",[~OtOSPOSQOS~ORUOSUOTUOUUOVROXSOZTO]XO^QO_UO`UOaPObPOcPOdUOeUOfUOgUOhUO~O^]ORvXSvXTvXUvXVvXXvXZvX]vX_vX`vXavXbvXcvXdvXevXfvXgvXhvX~OsvX~P!jOa_Ob_Oc_O~ORUOSUOTUOUUOVROXSOZTO^tO_UO`UOa`Ob`Oc`OdUOeUOfUOgUOhUO~OWaO~P$ZOYcO~P$ZO[eO~P$ZORUOSUOTUOUUOVROXSOZTO^QO_UO`UOaPObPOcPOdUOeUOfUOgUOhUO~O]hOsoX~P%zOajObjOcjO~O^]ORkaSkaTkaUkaVkaXkaZka]ka_ka`kaakabkackadkaekafkagkahka~Oska~P'kO^]O~OWvXYvX[vX~P!jOWnO~P$ZOYoO~P$ZO[pO~P$ZO^]ORkiSkiTkiUkiVkiXkiZki]ki_ki`kiakibkickidkiekifkigkihki~Oski~P)xOWkaYka[ka~P'kO]hO~P$ZOWkiYki[ki~P)xOasObsOcsO~O",
         goto: "#hwPPPPPPPPPPPPPPPPPPPPPPPPPPx||||!Y!^!d!xPPP#[TYOZeUORSTWZbdfqT[OZQZORiZSWOZQbRQdSQfTZgWbdfqQ^PWk^lmrQl_Qm`RrseVORSTWZbdfq",
         nodeNames: "⚠ LineComment BlockComment String Number Bool Null ( ) { } [ ] ; . Operator Punctuation SpecialVar Identifier QuotedIdentifier Keyword Type Bits Bytes Builtin Script Statement CompositeIdentifier Parens Braces Brackets Statement",
         maxTerm: 38,
         skippedNodes: [0, 1, 2],
@@ -20204,15 +20204,15 @@
     return i ? i[2] : t
 }
 
 function fl(n) {
     return n && (n.name == "Identifier" || n.name == "QuotedIdentifier")
 }
 
-function mv(n, e) {
+function yv(n, e) {
     if (e.name == "CompositeIdentifier") {
         let t = [];
         for (let i = e.firstChild; i; i = i.nextSibling) fl(i) && t.push(As(n, i));
         return t
     }
     return [As(n, e)]
 }
@@ -20222,17 +20222,17 @@
         if (!e || e.name != ".") return t;
         let i = Th(e);
         if (!fl(i)) return t;
         t.unshift(As(n, i)), e = Th(i)
     }
 }
 
-function yv(n, e) {
+function bv(n, e) {
     let t = lt(n).resolveInner(e, -1),
-        i = xv(n.doc, t);
+        i = kv(n.doc, t);
     return t.name == "Identifier" || t.name == "QuotedIdentifier" || t.name == "Keyword" ? {
         from: t.from,
         quoted: t.name == "QuotedIdentifier" ? n.doc.sliceString(t.from, t.from + 1) : null,
         parents: Du(n.doc, Th(t)),
         aliases: i
     } : t.name == "." ? {
         from: e,
@@ -20243,45 +20243,45 @@
         from: e,
         quoted: null,
         parents: [],
         empty: !0,
         aliases: i
     }
 }
-const bv = new Set("where group having order union intersect except all distinct limit offset fetch for".split(" "));
+const xv = new Set("where group having order union intersect except all distinct limit offset fetch for".split(" "));
 
-function xv(n, e) {
+function kv(n, e) {
     let t;
     for (let r = e; !t; r = r.parent) {
         if (!r) return null;
         r.name == "Statement" && (t = r)
     }
     let i = null;
     for (let r = t.firstChild, s = !1, o = null; r; r = r.nextSibling) {
         let l = r.name == "Keyword" ? n.sliceString(r.from, r.to).toLowerCase() : null,
             h = null;
         if (!s) s = l == "from";
         else if (l == "as" && o && fl(r.nextSibling)) h = As(n, r.nextSibling);
         else {
-            if (l && bv.has(l)) break;
+            if (l && xv.has(l)) break;
             o && fl(r) && (h = As(n, r))
         }
-        h && (i || (i = Object.create(null)), i[h] = mv(n, o)), o = /Identifier$/.test(r.name) ? r : null
+        h && (i || (i = Object.create(null)), i[h] = yv(n, o)), o = /Identifier$/.test(r.name) ? r : null
     }
     return i
 }
 
-function kv(n, e) {
+function wv(n, e) {
     return n ? e.map(t => Object.assign(Object.assign({}, t), {
         label: n + t.label + n,
         apply: void 0
     })) : e
 }
-const wv = /^\w*$/,
-    vv = /^[`'"]?\w*[`'"]?$/;
+const vv = /^\w*$/,
+    Sv = /^[`'"]?\w*[`'"]?$/;
 class lc {
     constructor() {
         this.list = [], this.children = void 0
     }
     child(e, t) {
         let i = this.children || (this.children = Object.create(null)),
             r = i[e];
@@ -20302,68 +20302,68 @@
         apply: t + n + t
     } : {
         label: n,
         type: e
     }
 }
 
-function Sv(n, e, t, i, r, s) {
+function Cv(n, e, t, i, r, s) {
     var o;
     let l = new lc,
         h = ((o = s == null ? void 0 : s.spec.identifierQuotes) === null || o === void 0 ? void 0 : o[0]) || '"',
         f = l.child(r || "", h);
     for (let u in n) {
-        let g = u.replace(/\\?\./g, k => k == "." ? "\0" : k).split("\0"),
-            y = g.length == 1 ? f : l;
-        for (let k of g) y = y.child(k.replace(/\\\./g, "."), h);
+        let m = u.replace(/\\?\./g, k => k == "." ? "\0" : k).split("\0"),
+            y = m.length == 1 ? f : l;
+        for (let k of m) y = y.child(k.replace(/\\\./g, "."), h);
         for (let k of n[u]) k && y.list.push(typeof k == "string" ? Kg(k, "property", h) : k)
     }
     return e && f.addCompletions(e), t && l.addCompletions(t), l.addCompletions(f.list), i && l.addCompletions(f.child(i, h).list), u => {
         let {
-            parents: g,
+            parents: m,
             from: y,
             quoted: k,
             empty: v,
-            aliases: C
-        } = yv(u.state, u.pos);
+            aliases: A
+        } = bv(u.state, u.pos);
         if (v && !u.explicit) return null;
-        C && g.length == 1 && (g = C[g[0]] || g);
+        A && m.length == 1 && (m = A[m[0]] || m);
         let O = l;
-        for (let $ of g) {
+        for (let $ of m) {
             for (; !O.children || !O.children[$];)
                 if (O == l) O = f;
                 else if (O == f && i) O = O.child(i, h);
             else return null;
             O = O.child($, h)
         }
         let D = k && u.state.sliceDoc(u.pos, u.pos + 1) == k,
             F = O.list;
-        return O == l && C && (F = F.concat(Object.keys(C).map($ => ({
+        return O == l && A && (F = F.concat(Object.keys(A).map($ => ({
             label: $,
             type: "constant"
         })))), {
             from: y,
             to: D ? u.pos + 1 : void 0,
-            options: kv(k, F),
-            validFor: k ? vv : wv
+            options: wv(k, F),
+            validFor: k ? Sv : vv
         }
     }
 }
 
-function Cv(n, e) {
+function Av(n, e) {
     let t = Object.keys(n).map(i => ({
         label: e ? i.toUpperCase() : i,
         type: n[i] == jg ? "type" : n[i] == qg ? "keyword" : "variable",
         boost: -1
     }));
-    return Fk(["QuotedIdentifier", "SpecialVar", "String", "LineComment", "BlockComment", "."], Og(t))
+    return zk(["QuotedIdentifier", "SpecialVar", "String", "LineComment", "BlockComment", "."], Og(t))
 }
-let Av = gv.configure({
+let Tv = mv.configure({
     props: [Tp.add({
-        Statement: xx()
+        Statement: kx()
     }), Mp.add({
         Statement(n) {
             return {
                 from: n.firstChild.to,
                 to: n.to
             }
         },
@@ -20399,18 +20399,18 @@
     constructor(e, t, i) {
         this.dialect = e, this.language = t, this.spec = i
     }
     get extension() {
         return this.language.extension
     }
     static define(e) {
-        let t = pv(e, e.keywords, e.types, e.builtin),
+        let t = gv(e, e.keywords, e.types, e.builtin),
             i = Ko.define({
                 name: "sql",
-                parser: Av.configure({
+                parser: Tv.configure({
                     tokenizers: [{
                         from: Gg,
                         to: Qg(t)
                     }]
                 }),
                 languageData: {
                     commentTokens: {
@@ -20425,58 +20425,58 @@
                     }
                 }
             });
         return new ac(t, i, e)
     }
 }
 
-function Tv(n, e = !1) {
-    return Cv(n.dialect.words, e)
+function Ov(n, e = !1) {
+    return Av(n.dialect.words, e)
 }
 
-function Ov(n, e = !1) {
+function Mv(n, e = !1) {
     return n.language.data.of({
-        autocomplete: Tv(n, e)
+        autocomplete: Ov(n, e)
     })
 }
 
 function Xg(n) {
-    return n.schema ? Sv(n.schema, n.tables, n.schemas, n.defaultTable, n.defaultSchema, n.dialect || Dl) : () => null
+    return n.schema ? Cv(n.schema, n.tables, n.schemas, n.defaultTable, n.defaultSchema, n.dialect || Dl) : () => null
 }
 
-function Mv(n) {
+function Ev(n) {
     return n.schema ? (n.dialect || Dl).language.data.of({
         autocomplete: Xg(n)
     }) : []
 }
 
-function Ev(n = {}) {
+function Dv(n = {}) {
     let e = n.dialect || Dl;
-    return new cx(e.language, [Mv(n), Ov(e, !!n.upperCaseKeywords)])
+    return new fx(e.language, [Ev(n), Mv(e, !!n.upperCaseKeywords)])
 }
 const Dl = ac.define({});
-let Dv = te.updateListener.of(n => {
+let Rv = te.updateListener.of(n => {
     n.docChanged && document.dispatchEvent(new CustomEvent("docChanged", {}))
 });
 const Ru = new CustomEvent("submitEventFromCM", {}),
-    Rv = [{
+    Lv = [{
         key: "Ctrl-Enter",
         run: () => (document.dispatchEvent(Ru), !0)
     }, {
         key: "Cmd-Enter",
         run: () => (document.dispatchEvent(Ru), !0)
     }],
-    Lv = Kn.highest(xl.of(Rv)),
-    Pv = [{
+    Pv = Kn.highest(xl.of(Lv)),
+    Nv = [{
         key: "Tab",
         run: Lg
     }],
-    Nv = [Ev({}), $b(), jb(), mb(), a1(), Nx(), sb(), cb(), wx(), Bx(Fx, {
+    Iv = [Dv({}), Wb(), Vb(), yb(), h1(), Ix(), ob(), fb(), vx(), _x(zx, {
         fallback: !0
-    }), Ux(), aw(), xw(), vb(), gk(), Lv, Dv, xl.of([...uw, ...ck, ...Nk, ...y1, ...Dx, ..._g, ...Ew, ...Pv])];
+    }), Qx(), hw(), kw(), Sb(), mk(), Pv, Rv, xl.of([...dw, ...fk, ...Ik, ...b1, ...Rx, ..._g, ...Dw, ...Nv])];
 
 function hc() {
     return {
         async: !1,
         breaks: !1,
         extensions: null,
         gfm: !0,
@@ -20490,46 +20490,46 @@
 }
 let Xn = hc();
 
 function Yg(n) {
     Xn = n
 }
 const Jg = /[&<>"']/,
-    Iv = new RegExp(Jg.source, "g"),
+    Bv = new RegExp(Jg.source, "g"),
     Zg = /[<>"']|&(?!(#\d{1,7}|#[Xx][a-fA-F0-9]{1,6}|\w+);)/,
-    Bv = new RegExp(Zg.source, "g"),
-    _v = {
+    _v = new RegExp(Zg.source, "g"),
+    Hv = {
         "&": "&amp;",
         "<": "&lt;",
         ">": "&gt;",
         '"': "&quot;",
         "'": "&#39;"
     },
-    Lu = n => _v[n];
+    Lu = n => Hv[n];
 
 function Vt(n, e) {
     if (e) {
-        if (Jg.test(n)) return n.replace(Iv, Lu)
-    } else if (Zg.test(n)) return n.replace(Bv, Lu);
+        if (Jg.test(n)) return n.replace(Bv, Lu)
+    } else if (Zg.test(n)) return n.replace(_v, Lu);
     return n
 }
-const Hv = /&(#(?:\d+)|(?:#x[0-9A-Fa-f]+)|(?:\w+));?/ig;
+const Fv = /&(#(?:\d+)|(?:#x[0-9A-Fa-f]+)|(?:\w+));?/ig;
 
-function Fv(n) {
-    return n.replace(Hv, (e, t) => (t = t.toLowerCase(), t === "colon" ? ":" : t.charAt(0) === "#" ? t.charAt(1) === "x" ? String.fromCharCode(parseInt(t.substring(2), 16)) : String.fromCharCode(+t.substring(1)) : ""))
+function zv(n) {
+    return n.replace(Fv, (e, t) => (t = t.toLowerCase(), t === "colon" ? ":" : t.charAt(0) === "#" ? t.charAt(1) === "x" ? String.fromCharCode(parseInt(t.substring(2), 16)) : String.fromCharCode(+t.substring(1)) : ""))
 }
-const zv = /(^|[^\[])\^/g;
+const $v = /(^|[^\[])\^/g;
 
 function Ie(n, e) {
     let t = typeof n == "string" ? n : n.source;
     e = e || "";
     const i = {
         replace: (r, s) => {
             let o = typeof s == "string" ? s : s.source;
-            return o = o.replace(zv, "$1"), t = t.replace(r, o), i
+            return o = o.replace($v, "$1"), t = t.replace(r, o), i
         },
         getRegex: () => new RegExp(t, e)
     };
     return i
 }
 
 function Pu(n) {
@@ -20570,15 +20570,15 @@
         if (s === e && !t) r++;
         else if (s !== e && t) r++;
         else break
     }
     return n.slice(0, i - r)
 }
 
-function $v(n, e) {
+function Wv(n, e) {
     if (n.indexOf(e[1]) === -1) return -1;
     let t = 0;
     for (let i = 0; i < n.length; i++)
         if (n[i] === "\\") i++;
         else if (n[i] === e[0]) t++;
     else if (n[i] === e[1] && (t--, t < 0)) return i;
     return -1
@@ -20605,15 +20605,15 @@
         raw: t,
         href: r,
         title: s,
         text: Vt(o)
     }
 }
 
-function Wv(n, e) {
+function qv(n, e) {
     const t = n.match(/^(\s+)(?:```)/);
     if (t === null) return e;
     const i = t[1];
     return e.split(`
 `).map(r => {
         const s = r.match(/^\s+/);
         if (s === null) return r;
@@ -20649,15 +20649,15 @@
             }
         }
     }
     fences(e) {
         const t = this.rules.block.fences.exec(e);
         if (t) {
             const i = t[0],
-                r = Wv(i, t[3] || "");
+                r = qv(i, t[3] || "");
             return {
                 type: "code",
                 raw: i,
                 lang: t[2] ? t[2].trim().replace(this.rules.inline.anyPunctuation, "$1") : t[2],
                 text: r
             }
         }
@@ -20720,59 +20720,59 @@
             let l = "",
                 h = "",
                 f = !1;
             for (; e;) {
                 let u = !1;
                 if (!(t = o.exec(e)) || this.rules.block.hr.test(e)) break;
                 l = t[0], e = e.substring(l.length);
-                let g = t[2].split(`
+                let m = t[2].split(`
 `, 1)[0].replace(/^\t+/, D => " ".repeat(3 * D.length)),
                     y = e.split(`
 `, 1)[0],
                     k = 0;
-                this.options.pedantic ? (k = 2, h = g.trimStart()) : (k = t[2].search(/[^ ]/), k = k > 4 ? 1 : k, h = g.slice(k), k += t[1].length);
+                this.options.pedantic ? (k = 2, h = m.trimStart()) : (k = t[2].search(/[^ ]/), k = k > 4 ? 1 : k, h = m.slice(k), k += t[1].length);
                 let v = !1;
-                if (!g && /^ *$/.test(y) && (l += y + `
+                if (!m && /^ *$/.test(y) && (l += y + `
 `, e = e.substring(y.length + 1), u = !0), !u) {
                     const D = new RegExp(`^ {0,${Math.min(3,k-1)}}(?:[*+-]|\\d{1,9}[.)])((?:[ 	][^\\n]*)?(?:\\n|$))`),
                         F = new RegExp(`^ {0,${Math.min(3,k-1)}}((?:- *){3,}|(?:_ *){3,}|(?:\\* *){3,})(?:\\n+|$)`),
                         $ = new RegExp(`^ {0,${Math.min(3,k-1)}}(?:\`\`\`|~~~)`),
                         j = new RegExp(`^ {0,${Math.min(3,k-1)}}#`);
                     for (; e;) {
                         const z = e.split(`
 `, 1)[0];
                         if (y = z, this.options.pedantic && (y = y.replace(/^ {1,4}(?=( {4})*[^ ])/g, "  ")), $.test(y) || j.test(y) || D.test(y) || F.test(e)) break;
                         if (y.search(/[^ ]/) >= k || !y.trim()) h += `
 ` + y.slice(k);
                         else {
-                            if (v || g.search(/[^ ]/) >= 4 || $.test(g) || j.test(g) || F.test(g)) break;
+                            if (v || m.search(/[^ ]/) >= 4 || $.test(m) || j.test(m) || F.test(m)) break;
                             h += `
 ` + y
                         }!v && !y.trim() && (v = !0), l += z + `
-`, e = e.substring(z.length + 1), g = y.slice(k)
+`, e = e.substring(z.length + 1), m = y.slice(k)
                     }
                 }
                 s.loose || (f ? s.loose = !0 : /\n *\n *$/.test(l) && (f = !0));
-                let C = null,
+                let A = null,
                     O;
-                this.options.gfm && (C = /^\[[ xX]\] /.exec(h), C && (O = C[0] !== "[ ] ", h = h.replace(/^\[[ xX]\] +/, ""))), s.items.push({
+                this.options.gfm && (A = /^\[[ xX]\] /.exec(h), A && (O = A[0] !== "[ ] ", h = h.replace(/^\[[ xX]\] +/, ""))), s.items.push({
                     type: "list_item",
                     raw: l,
-                    task: !!C,
+                    task: !!A,
                     checked: O,
                     loose: !1,
                     text: h,
                     tokens: []
                 }), s.raw += l
             }
             s.items[s.items.length - 1].raw = l.trimEnd(), s.items[s.items.length - 1].text = h.trimEnd(), s.raw = s.raw.trimEnd();
             for (let u = 0; u < s.items.length; u++)
                 if (this.lexer.state.top = !1, s.items[u].tokens = this.lexer.blockTokens(s.items[u].text, []), !s.loose) {
-                    const g = s.items[u].tokens.filter(k => k.type === "space"),
-                        y = g.length > 0 && g.some(k => /\n.*\n/.test(k.raw));
+                    const m = s.items[u].tokens.filter(k => k.type === "space"),
+                        y = m.length > 0 && m.some(k => /\n.*\n/.test(k.raw));
                     s.loose = y
                 } if (s.loose)
                 for (let u = 0; u < s.items.length; u++) s.items[u].loose = !0;
             return s
         }
     }
     html(e) {
@@ -20883,15 +20883,15 @@
         if (t) {
             const i = t[2].trim();
             if (!this.options.pedantic && /^</.test(i)) {
                 if (!/>$/.test(i)) return;
                 const o = So(i.slice(0, -1), "\\");
                 if ((i.length - o.length) % 2 === 0) return
             } else {
-                const o = $v(t[2], "()");
+                const o = Wv(t[2], "()");
                 if (o > -1) {
                     const h = (t[0].indexOf("!") === 0 ? 5 : 4) + t[1].length + o;
                     t[2] = t[2].substring(0, o), t[0] = t[0].substring(0, h).trim(), t[3] = ""
                 }
             }
             let r = t[2],
                 s = "";
@@ -20924,36 +20924,36 @@
     emStrong(e, t, i = "") {
         let r = this.rules.inline.emStrongLDelim.exec(e);
         if (!r || r[3] && i.match(/[\p{L}\p{N}]/u)) return;
         if (!(r[1] || r[2] || "") || !i || this.rules.inline.punctuation.exec(i)) {
             const o = [...r[0]].length - 1;
             let l, h, f = o,
                 u = 0;
-            const g = r[0][0] === "*" ? this.rules.inline.emStrongRDelimAst : this.rules.inline.emStrongRDelimUnd;
-            for (g.lastIndex = 0, t = t.slice(-1 * e.length + o);
-                (r = g.exec(t)) != null;) {
+            const m = r[0][0] === "*" ? this.rules.inline.emStrongRDelimAst : this.rules.inline.emStrongRDelimUnd;
+            for (m.lastIndex = 0, t = t.slice(-1 * e.length + o);
+                (r = m.exec(t)) != null;) {
                 if (l = r[1] || r[2] || r[3] || r[4] || r[5] || r[6], !l) continue;
                 if (h = [...l].length, r[3] || r[4]) {
                     f += h;
                     continue
                 } else if ((r[5] || r[6]) && o % 3 && !((o + h) % 3)) {
                     u += h;
                     continue
                 }
                 if (f -= h, f > 0) continue;
                 h = Math.min(h, h + f + u);
                 const y = [...r[0]][0].length,
                     k = e.slice(0, o + r.index + y + h);
                 if (Math.min(o, h) % 2) {
-                    const C = k.slice(1, -1);
+                    const A = k.slice(1, -1);
                     return {
                         type: "em",
                         raw: k,
-                        text: C,
-                        tokens: this.lexer.inlineTokens(C)
+                        text: A,
+                        tokens: this.lexer.inlineTokens(A)
                     }
                 }
                 const v = k.slice(2, -2);
                 return {
                     type: "strong",
                     raw: k,
                     text: v,
@@ -21040,125 +21040,125 @@
                 type: "text",
                 raw: t[0],
                 text: i
             }
         }
     }
 }
-const qv = /^(?: *(?:\n|$))+/,
-    jv = /^( {4}[^\n]+(?:\n(?: *(?:\n|$))*)?)+/,
-    Vv = /^ {0,3}(`{3,}(?=[^`\n]*(?:\n|$))|~{3,})([^\n]*)(?:\n|$)(?:|([\s\S]*?)(?:\n|$))(?: {0,3}\1[~`]* *(?=\n|$)|$)/,
+const jv = /^(?: *(?:\n|$))+/,
+    Vv = /^( {4}[^\n]+(?:\n(?: *(?:\n|$))*)?)+/,
+    Uv = /^ {0,3}(`{3,}(?=[^`\n]*(?:\n|$))|~{3,})([^\n]*)(?:\n|$)(?:|([\s\S]*?)(?:\n|$))(?: {0,3}\1[~`]* *(?=\n|$)|$)/,
     Ns = /^ {0,3}((?:-[\t ]*){3,}|(?:_[ \t]*){3,}|(?:\*[ \t]*){3,})(?:\n+|$)/,
-    Uv = /^ {0,3}(#{1,6})(?=\s|$)(.*)(?:\n+|$)/,
+    Qv = /^ {0,3}(#{1,6})(?=\s|$)(.*)(?:\n+|$)/,
     em = /(?:[*+-]|\d{1,9}[.)])/,
     tm = Ie(/^(?!bull )((?:.|\n(?!\s*?\n|bull ))+?)\n {0,3}(=+|-+) *(?:\n+|$)/).replace(/bull/g, em).getRegex(),
     cc = /^([^\n]+(?:\n(?!hr|heading|lheading|blockquote|fences|list|html|table| +\n)[^\n]+)*)/,
-    Qv = /^[^\n]+/,
+    Gv = /^[^\n]+/,
     fc = /(?!\s*\])(?:\\.|[^\[\]\\])+/,
-    Gv = Ie(/^ {0,3}\[(label)\]: *(?:\n *)?([^<\s][^\s]*|<.*?>)(?:(?: +(?:\n *)?| *\n *)(title))? *(?:\n+|$)/).replace("label", fc).replace("title", /(?:"(?:\\"?|[^"\\])*"|'[^'\n]*(?:\n[^'\n]+)*\n?'|\([^()]*\))/).getRegex(),
-    Kv = Ie(/^( {0,3}bull)([ \t][^\n]+?)?(?:\n|$)/).replace(/bull/g, em).getRegex(),
+    Kv = Ie(/^ {0,3}\[(label)\]: *(?:\n *)?([^<\s][^\s]*|<.*?>)(?:(?: +(?:\n *)?| *\n *)(title))? *(?:\n+|$)/).replace("label", fc).replace("title", /(?:"(?:\\"?|[^"\\])*"|'[^'\n]*(?:\n[^'\n]+)*\n?'|\([^()]*\))/).getRegex(),
+    Xv = Ie(/^( {0,3}bull)([ \t][^\n]+?)?(?:\n|$)/).replace(/bull/g, em).getRegex(),
     Rl = "address|article|aside|base|basefont|blockquote|body|caption|center|col|colgroup|dd|details|dialog|dir|div|dl|dt|fieldset|figcaption|figure|footer|form|frame|frameset|h[1-6]|head|header|hr|html|iframe|legend|li|link|main|menu|menuitem|meta|nav|noframes|ol|optgroup|option|p|param|section|source|summary|table|tbody|td|tfoot|th|thead|title|tr|track|ul",
     uc = /<!--(?!-?>)[\s\S]*?(?:-->|$)/,
-    Xv = Ie("^ {0,3}(?:<(script|pre|style|textarea)[\\s>][\\s\\S]*?(?:</\\1>[^\\n]*\\n+|$)|comment[^\\n]*(\\n+|$)|<\\?[\\s\\S]*?(?:\\?>\\n*|$)|<![A-Z][\\s\\S]*?(?:>\\n*|$)|<!\\[CDATA\\[[\\s\\S]*?(?:\\]\\]>\\n*|$)|</?(tag)(?: +|\\n|/?>)[\\s\\S]*?(?:(?:\\n *)+\\n|$)|<(?!script|pre|style|textarea)([a-z][\\w-]*)(?:attribute)*? */?>(?=[ \\t]*(?:\\n|$))[\\s\\S]*?(?:(?:\\n *)+\\n|$)|</(?!script|pre|style|textarea)[a-z][\\w-]*\\s*>(?=[ \\t]*(?:\\n|$))[\\s\\S]*?(?:(?:\\n *)+\\n|$))", "i").replace("comment", uc).replace("tag", Rl).replace("attribute", / +[a-zA-Z:_][\w.:-]*(?: *= *"[^"\n]*"| *= *'[^'\n]*'| *= *[^\s"'=<>`]+)?/).getRegex(),
+    Yv = Ie("^ {0,3}(?:<(script|pre|style|textarea)[\\s>][\\s\\S]*?(?:</\\1>[^\\n]*\\n+|$)|comment[^\\n]*(\\n+|$)|<\\?[\\s\\S]*?(?:\\?>\\n*|$)|<![A-Z][\\s\\S]*?(?:>\\n*|$)|<!\\[CDATA\\[[\\s\\S]*?(?:\\]\\]>\\n*|$)|</?(tag)(?: +|\\n|/?>)[\\s\\S]*?(?:(?:\\n *)+\\n|$)|<(?!script|pre|style|textarea)([a-z][\\w-]*)(?:attribute)*? */?>(?=[ \\t]*(?:\\n|$))[\\s\\S]*?(?:(?:\\n *)+\\n|$)|</(?!script|pre|style|textarea)[a-z][\\w-]*\\s*>(?=[ \\t]*(?:\\n|$))[\\s\\S]*?(?:(?:\\n *)+\\n|$))", "i").replace("comment", uc).replace("tag", Rl).replace("attribute", / +[a-zA-Z:_][\w.:-]*(?: *= *"[^"\n]*"| *= *'[^'\n]*'| *= *[^\s"'=<>`]+)?/).getRegex(),
     im = Ie(cc).replace("hr", Ns).replace("heading", " {0,3}#{1,6}(?:\\s|$)").replace("|lheading", "").replace("|table", "").replace("blockquote", " {0,3}>").replace("fences", " {0,3}(?:`{3,}(?=[^`\\n]*\\n)|~{3,})[^\\n]*\\n").replace("list", " {0,3}(?:[*+-]|1[.)]) ").replace("html", "</?(?:tag)(?: +|\\n|/?>)|<(?:script|pre|style|textarea|!--)").replace("tag", Rl).getRegex(),
-    Yv = Ie(/^( {0,3}> ?(paragraph|[^\n]*)(?:\n|$))+/).replace("paragraph", im).getRegex(),
+    Jv = Ie(/^( {0,3}> ?(paragraph|[^\n]*)(?:\n|$))+/).replace("paragraph", im).getRegex(),
     dc = {
-        blockquote: Yv,
-        code: jv,
-        def: Gv,
-        fences: Vv,
-        heading: Uv,
+        blockquote: Jv,
+        code: Vv,
+        def: Kv,
+        fences: Uv,
+        heading: Qv,
         hr: Ns,
-        html: Xv,
+        html: Yv,
         lheading: tm,
-        list: Kv,
-        newline: qv,
+        list: Xv,
+        newline: jv,
         paragraph: im,
         table: as,
-        text: Qv
+        text: Gv
     },
     Bu = Ie("^ *([^\\n ].*)\\n {0,3}((?:\\| *)?:?-+:? *(?:\\| *:?-+:? *)*(?:\\| *)?)(?:\\n((?:(?! *\\n|hr|heading|blockquote|code|fences|list|html).*(?:\\n|$))*)\\n*|$)").replace("hr", Ns).replace("heading", " {0,3}#{1,6}(?:\\s|$)").replace("blockquote", " {0,3}>").replace("code", " {4}[^\\n]").replace("fences", " {0,3}(?:`{3,}(?=[^`\\n]*\\n)|~{3,})[^\\n]*\\n").replace("list", " {0,3}(?:[*+-]|1[.)]) ").replace("html", "</?(?:tag)(?: +|\\n|/?>)|<(?:script|pre|style|textarea|!--)").replace("tag", Rl).getRegex(),
-    Jv = lr(It({}, dc), {
+    Zv = lr(It({}, dc), {
         table: Bu,
         paragraph: Ie(cc).replace("hr", Ns).replace("heading", " {0,3}#{1,6}(?:\\s|$)").replace("|lheading", "").replace("table", Bu).replace("blockquote", " {0,3}>").replace("fences", " {0,3}(?:`{3,}(?=[^`\\n]*\\n)|~{3,})[^\\n]*\\n").replace("list", " {0,3}(?:[*+-]|1[.)]) ").replace("html", "</?(?:tag)(?: +|\\n|/?>)|<(?:script|pre|style|textarea|!--)").replace("tag", Rl).getRegex()
     }),
-    Zv = lr(It({}, dc), {
+    eS = lr(It({}, dc), {
         html: Ie(`^ *(?:comment *(?:\\n|\\s*$)|<(tag)[\\s\\S]+?</\\1> *(?:\\n{2,}|\\s*$)|<tag(?:"[^"]*"|'[^']*'|\\s[^'"/>\\s]*)*?/?> *(?:\\n{2,}|\\s*$))`).replace("comment", uc).replace(/tag/g, "(?!(?:a|em|strong|small|s|cite|q|dfn|abbr|data|time|code|var|samp|kbd|sub|sup|i|b|u|mark|ruby|rt|rp|bdi|bdo|span|br|wbr|ins|del|img)\\b)\\w+(?!:|[^\\w\\s@]*@)\\b").getRegex(),
         def: /^ *\[([^\]]+)\]: *<?([^\s>]+)>?(?: +(["(][^\n]+[")]))? *(?:\n+|$)/,
         heading: /^(#{1,6})(.*)(?:\n+|$)/,
         fences: as,
         lheading: /^(.+?)\n {0,3}(=+|-+) *(?:\n+|$)/,
         paragraph: Ie(cc).replace("hr", Ns).replace("heading", ` *#{1,6} *[^
 ]`).replace("lheading", tm).replace("|table", "").replace("blockquote", " {0,3}>").replace("|fences", "").replace("|list", "").replace("|html", "").replace("|tag", "").getRegex()
     }),
     nm = /^\\([!"#$%&'()*+,\-./:;<=>?@\[\]\\^_`{|}~])/,
-    eS = /^(`+)([^`]|[^`][\s\S]*?[^`])\1(?!`)/,
+    tS = /^(`+)([^`]|[^`][\s\S]*?[^`])\1(?!`)/,
     rm = /^( {2,}|\\)\n(?!\s*$)/,
-    tS = /^(`+|[^`])(?:(?= {2,}\n)|[\s\S]*?(?:(?=[\\<!\[`*_]|\b_|$)|[^ ](?= {2,}\n)))/,
+    iS = /^(`+|[^`])(?:(?= {2,}\n)|[\s\S]*?(?:(?=[\\<!\[`*_]|\b_|$)|[^ ](?= {2,}\n)))/,
     Is = "\\p{P}$+<=>`^|~",
-    iS = Ie(/^((?![*_])[\spunctuation])/, "u").replace(/punctuation/g, Is).getRegex(),
-    nS = /\[[^[\]]*?\]\([^\(\)]*?\)|`[^`]*?`|<[^<>]*?>/g,
-    rS = Ie(/^(?:\*+(?:((?!\*)[punct])|[^\s*]))|^_+(?:((?!_)[punct])|([^\s_]))/, "u").replace(/punct/g, Is).getRegex(),
-    sS = Ie("^[^_*]*?__[^_*]*?\\*[^_*]*?(?=__)|[^*]+(?=[^*])|(?!\\*)[punct](\\*+)(?=[\\s]|$)|[^punct\\s](\\*+)(?!\\*)(?=[punct\\s]|$)|(?!\\*)[punct\\s](\\*+)(?=[^punct\\s])|[\\s](\\*+)(?!\\*)(?=[punct])|(?!\\*)[punct](\\*+)(?!\\*)(?=[punct])|[^punct\\s](\\*+)(?=[^punct\\s])", "gu").replace(/punct/g, Is).getRegex(),
-    oS = Ie("^[^_*]*?\\*\\*[^_*]*?_[^_*]*?(?=\\*\\*)|[^_]+(?=[^_])|(?!_)[punct](_+)(?=[\\s]|$)|[^punct\\s](_+)(?!_)(?=[punct\\s]|$)|(?!_)[punct\\s](_+)(?=[^punct\\s])|[\\s](_+)(?!_)(?=[punct])|(?!_)[punct](_+)(?!_)(?=[punct])", "gu").replace(/punct/g, Is).getRegex(),
-    lS = Ie(/\\([punct])/, "gu").replace(/punct/g, Is).getRegex(),
-    aS = Ie(/^<(scheme:[^\s\x00-\x1f<>]*|email)>/).replace("scheme", /[a-zA-Z][a-zA-Z0-9+.-]{1,31}/).replace("email", /[a-zA-Z0-9.!#$%&'*+/=?^_`{|}~-]+(@)[a-zA-Z0-9](?:[a-zA-Z0-9-]{0,61}[a-zA-Z0-9])?(?:\.[a-zA-Z0-9](?:[a-zA-Z0-9-]{0,61}[a-zA-Z0-9])?)+(?![-_])/).getRegex(),
-    hS = Ie(uc).replace("(?:-->|$)", "-->").getRegex(),
-    cS = Ie("^comment|^</[a-zA-Z][\\w:-]*\\s*>|^<[a-zA-Z][\\w-]*(?:attribute)*?\\s*/?>|^<\\?[\\s\\S]*?\\?>|^<![a-zA-Z]+\\s[\\s\\S]*?>|^<!\\[CDATA\\[[\\s\\S]*?\\]\\]>").replace("comment", hS).replace("attribute", /\s+[a-zA-Z:_][\w.:-]*(?:\s*=\s*"[^"]*"|\s*=\s*'[^']*'|\s*=\s*[^\s"'=<>`]+)?/).getRegex(),
+    nS = Ie(/^((?![*_])[\spunctuation])/, "u").replace(/punctuation/g, Is).getRegex(),
+    rS = /\[[^[\]]*?\]\([^\(\)]*?\)|`[^`]*?`|<[^<>]*?>/g,
+    sS = Ie(/^(?:\*+(?:((?!\*)[punct])|[^\s*]))|^_+(?:((?!_)[punct])|([^\s_]))/, "u").replace(/punct/g, Is).getRegex(),
+    oS = Ie("^[^_*]*?__[^_*]*?\\*[^_*]*?(?=__)|[^*]+(?=[^*])|(?!\\*)[punct](\\*+)(?=[\\s]|$)|[^punct\\s](\\*+)(?!\\*)(?=[punct\\s]|$)|(?!\\*)[punct\\s](\\*+)(?=[^punct\\s])|[\\s](\\*+)(?!\\*)(?=[punct])|(?!\\*)[punct](\\*+)(?!\\*)(?=[punct])|[^punct\\s](\\*+)(?=[^punct\\s])", "gu").replace(/punct/g, Is).getRegex(),
+    lS = Ie("^[^_*]*?\\*\\*[^_*]*?_[^_*]*?(?=\\*\\*)|[^_]+(?=[^_])|(?!_)[punct](_+)(?=[\\s]|$)|[^punct\\s](_+)(?!_)(?=[punct\\s]|$)|(?!_)[punct\\s](_+)(?=[^punct\\s])|[\\s](_+)(?!_)(?=[punct])|(?!_)[punct](_+)(?!_)(?=[punct])", "gu").replace(/punct/g, Is).getRegex(),
+    aS = Ie(/\\([punct])/, "gu").replace(/punct/g, Is).getRegex(),
+    hS = Ie(/^<(scheme:[^\s\x00-\x1f<>]*|email)>/).replace("scheme", /[a-zA-Z][a-zA-Z0-9+.-]{1,31}/).replace("email", /[a-zA-Z0-9.!#$%&'*+/=?^_`{|}~-]+(@)[a-zA-Z0-9](?:[a-zA-Z0-9-]{0,61}[a-zA-Z0-9])?(?:\.[a-zA-Z0-9](?:[a-zA-Z0-9-]{0,61}[a-zA-Z0-9])?)+(?![-_])/).getRegex(),
+    cS = Ie(uc).replace("(?:-->|$)", "-->").getRegex(),
+    fS = Ie("^comment|^</[a-zA-Z][\\w:-]*\\s*>|^<[a-zA-Z][\\w-]*(?:attribute)*?\\s*/?>|^<\\?[\\s\\S]*?\\?>|^<![a-zA-Z]+\\s[\\s\\S]*?>|^<!\\[CDATA\\[[\\s\\S]*?\\]\\]>").replace("comment", cS).replace("attribute", /\s+[a-zA-Z:_][\w.:-]*(?:\s*=\s*"[^"]*"|\s*=\s*'[^']*'|\s*=\s*[^\s"'=<>`]+)?/).getRegex(),
     dl = /(?:\[(?:\\.|[^\[\]\\])*\]|\\.|`[^`]*`|[^\[\]\\`])*?/,
-    fS = Ie(/^!?\[(label)\]\(\s*(href)(?:\s+(title))?\s*\)/).replace("label", dl).replace("href", /<(?:\\.|[^\n<>\\])+>|[^\s\x00-\x1f]*/).replace("title", /"(?:\\"?|[^"\\])*"|'(?:\\'?|[^'\\])*'|\((?:\\\)?|[^)\\])*\)/).getRegex(),
+    uS = Ie(/^!?\[(label)\]\(\s*(href)(?:\s+(title))?\s*\)/).replace("label", dl).replace("href", /<(?:\\.|[^\n<>\\])+>|[^\s\x00-\x1f]*/).replace("title", /"(?:\\"?|[^"\\])*"|'(?:\\'?|[^'\\])*'|\((?:\\\)?|[^)\\])*\)/).getRegex(),
     sm = Ie(/^!?\[(label)\]\[(ref)\]/).replace("label", dl).replace("ref", fc).getRegex(),
     om = Ie(/^!?\[(ref)\](?:\[\])?/).replace("ref", fc).getRegex(),
-    uS = Ie("reflink|nolink(?!\\()", "g").replace("reflink", sm).replace("nolink", om).getRegex(),
+    dS = Ie("reflink|nolink(?!\\()", "g").replace("reflink", sm).replace("nolink", om).getRegex(),
     pc = {
         _backpedal: as,
-        anyPunctuation: lS,
-        autolink: aS,
-        blockSkip: nS,
+        anyPunctuation: aS,
+        autolink: hS,
+        blockSkip: rS,
         br: rm,
-        code: eS,
+        code: tS,
         del: as,
-        emStrongLDelim: rS,
-        emStrongRDelimAst: sS,
-        emStrongRDelimUnd: oS,
+        emStrongLDelim: sS,
+        emStrongRDelimAst: oS,
+        emStrongRDelimUnd: lS,
         escape: nm,
-        link: fS,
+        link: uS,
         nolink: om,
-        punctuation: iS,
+        punctuation: nS,
         reflink: sm,
-        reflinkSearch: uS,
-        tag: cS,
-        text: tS,
+        reflinkSearch: dS,
+        tag: fS,
+        text: iS,
         url: as
     },
-    dS = lr(It({}, pc), {
+    pS = lr(It({}, pc), {
         link: Ie(/^!?\[(label)\]\((.*?)\)/).replace("label", dl).getRegex(),
         reflink: Ie(/^!?\[(label)\]\s*\[([^\]]*)\]/).replace("label", dl).getRegex()
     }),
     Oh = lr(It({}, pc), {
         escape: Ie(nm).replace("])", "~|])").getRegex(),
         url: Ie(/^((?:ftp|https?):\/\/|www\.)(?:[a-zA-Z0-9\-]+\.?)+[^\s<]*|^email/, "i").replace("email", /[A-Za-z0-9._+-]+(@)[a-zA-Z0-9-_]+(?:\.[a-zA-Z0-9-_]*[a-zA-Z0-9])+(?![-_])/).getRegex(),
         _backpedal: /(?:[^?!.,:;*_'"~()&]+|\([^)]*\)|&(?![a-zA-Z0-9]+;$)|[?!.,:;*_'"~)]+(?!$))+/,
         del: /^(~~?)(?=[^\s~])([\s\S]*?[^\s~])\1(?=[^~]|$)/,
         text: /^([`~]+|[^`~])(?:(?= {2,}\n)|(?=[a-zA-Z0-9.!#$%&'*+\/=?_`{\|}~-]+@)|[\s\S]*?(?:(?=[\\<!\[`*~_]|\b_|https?:\/\/|ftp:\/\/|www\.|$)|[^ ](?= {2,}\n)|[^a-zA-Z0-9.!#$%&'*+\/=?_`{\|}~-](?=[a-zA-Z0-9.!#$%&'*+\/=?_`{\|}~-]+@)))/
     }),
-    pS = lr(It({}, Oh), {
+    gS = lr(It({}, Oh), {
         br: Ie(rm).replace("{2,}", "*").getRegex(),
         text: Ie(Oh.text).replace("\\b_", "\\b_| {2,}\\n").replace(/\{2,\}/g, "*").getRegex()
     }),
     Co = {
         normal: dc,
-        gfm: Jv,
-        pedantic: Zv
+        gfm: Zv,
+        pedantic: eS
     },
     Kr = {
         normal: pc,
         gfm: Oh,
-        breaks: pS,
-        pedantic: dS
+        breaks: gS,
+        pedantic: pS
     };
 class Ii {
     constructor(e) {
         ze(this, "tokens");
         ze(this, "options");
         ze(this, "state");
         ze(this, "tokenizer");
@@ -21346,20 +21346,20 @@
                 }
                 if (!this.state.inLink && (i = this.tokenizer.url(e))) {
                     e = e.substring(i.raw.length), t.push(i);
                     continue
                 }
                 if (s = e, this.options.extensions && this.options.extensions.startInline) {
                     let u = 1 / 0;
-                    const g = e.slice(1);
+                    const m = e.slice(1);
                     let y;
                     this.options.extensions.startInline.forEach(k => {
                         y = k.call({
                             lexer: this
-                        }, g), typeof y == "number" && y >= 0 && (u = Math.min(u, y))
+                        }, m), typeof y == "number" && y >= 0 && (u = Math.min(u, y))
                     }), u < 1 / 0 && u >= 0 && (s = e.substring(0, u + 1))
                 }
                 if (i = this.tokenizer.inlineText(s)) {
                     e = e.substring(i.raw.length), i.raw.slice(-1) !== "_" && (f = i.raw.slice(-1)), h = !0, r = t[t.length - 1], r && r.type === "text" ? (r.raw += i.raw, r.text += i.text) : t.push(i);
                     continue
                 }
                 if (e) {
@@ -21530,15 +21530,15 @@
                     continue;
                 case "hr": {
                     i += this.renderer.hr();
                     continue
                 }
                 case "heading": {
                     const o = s;
-                    i += this.renderer.heading(this.parseInline(o.tokens), o.depth, Fv(this.parseInline(o.tokens, this.textRenderer)));
+                    i += this.renderer.heading(this.parseInline(o.tokens), o.depth, zv(this.parseInline(o.tokens, this.textRenderer)));
                     continue
                 }
                 case "code": {
                     const o = s;
                     i += this.renderer.code(o.text, o.lang, !!o.escaped);
                     continue
                 }
@@ -21549,17 +21549,17 @@
                     for (let u = 0; u < o.header.length; u++) h += this.renderer.tablecell(this.parseInline(o.header[u].tokens), {
                         header: !0,
                         align: o.align[u]
                     });
                     l += this.renderer.tablerow(h);
                     let f = "";
                     for (let u = 0; u < o.rows.length; u++) {
-                        const g = o.rows[u];
+                        const m = o.rows[u];
                         h = "";
-                        for (let y = 0; y < g.length; y++) h += this.renderer.tablecell(this.parseInline(g[y].tokens), {
+                        for (let y = 0; y < m.length; y++) h += this.renderer.tablecell(this.parseInline(m[y].tokens), {
                             header: !1,
                             align: o.align[y]
                         });
                         f += this.renderer.tablerow(h)
                     }
                     i += this.renderer.table(l, f);
                     continue
@@ -21572,27 +21572,27 @@
                 }
                 case "list": {
                     const o = s,
                         l = o.ordered,
                         h = o.start,
                         f = o.loose;
                     let u = "";
-                    for (let g = 0; g < o.items.length; g++) {
-                        const y = o.items[g],
+                    for (let m = 0; m < o.items.length; m++) {
+                        const y = o.items[m],
                             k = y.checked,
                             v = y.task;
-                        let C = "";
+                        let A = "";
                         if (y.task) {
                             const O = this.renderer.checkbox(!!k);
                             f ? y.tokens.length > 0 && y.tokens[0].type === "paragraph" ? (y.tokens[0].text = O + " " + y.tokens[0].text, y.tokens[0].tokens && y.tokens[0].tokens.length > 0 && y.tokens[0].tokens[0].type === "text" && (y.tokens[0].tokens[0].text = O + " " + y.tokens[0].tokens[0].text)) : y.tokens.unshift({
                                 type: "text",
                                 text: O + " "
-                            }) : C += O + " "
+                            }) : A += O + " "
                         }
-                        C += this.parse(y.tokens, f), u += this.renderer.listitem(C, v, !!k)
+                        A += this.parse(y.tokens, f), u += this.renderer.listitem(A, v, !!k)
                     }
                     i += this.renderer.list(u, l, h);
                     continue
                 }
                 case "html": {
                     const o = s;
                     i += this.renderer.html(o.text, o.block);
@@ -21707,15 +21707,15 @@
     }
     processAllTokens(e) {
         return e
     }
 }
 ze(hs, "passThroughHooks", new Set(["preprocess", "postprocess", "processAllTokens"]));
 var Ts, Mh, gl, lm;
-class gS {
+class mS {
     constructor(...e) {
         Yl(this, Ts);
         Yl(this, gl);
         ze(this, "defaults", hc());
         ze(this, "options", this.setOptions);
         ze(this, "parse", Js(this, Ts, Mh).call(this, Ii.lex, Bi.parse));
         ze(this, "parseInline", Js(this, Ts, Mh).call(this, Ii.lexInline, Bi.parseInline));
@@ -21779,50 +21779,50 @@
                 for (const o in i.renderer) {
                     if (!(o in s)) throw new Error(`renderer '${o}' does not exist`);
                     if (o === "options") continue;
                     const l = o,
                         h = i.renderer[l],
                         f = s[l];
                     s[l] = (...u) => {
-                        let g = h.apply(s, u);
-                        return g === !1 && (g = f.apply(s, u)), g || ""
+                        let m = h.apply(s, u);
+                        return m === !1 && (m = f.apply(s, u)), m || ""
                     }
                 }
                 r.renderer = s
             }
             if (i.tokenizer) {
                 const s = this.defaults.tokenizer || new ul(this.defaults);
                 for (const o in i.tokenizer) {
                     if (!(o in s)) throw new Error(`tokenizer '${o}' does not exist`);
                     if (["options", "rules", "lexer"].includes(o)) continue;
                     const l = o,
                         h = i.tokenizer[l],
                         f = s[l];
                     s[l] = (...u) => {
-                        let g = h.apply(s, u);
-                        return g === !1 && (g = f.apply(s, u)), g
+                        let m = h.apply(s, u);
+                        return m === !1 && (m = f.apply(s, u)), m
                     }
                 }
                 r.tokenizer = s
             }
             if (i.hooks) {
                 const s = this.defaults.hooks || new hs;
                 for (const o in i.hooks) {
                     if (!(o in s)) throw new Error(`hook '${o}' does not exist`);
                     if (o === "options") continue;
                     const l = o,
                         h = i.hooks[l],
                         f = s[l];
                     hs.passThroughHooks.has(o) ? s[l] = u => {
                         if (this.defaults.async) return Promise.resolve(h.call(s, u)).then(y => f.call(s, y));
-                        const g = h.call(s, u);
-                        return f.call(s, g)
+                        const m = h.call(s, u);
+                        return f.call(s, m)
                     } : s[l] = (...u) => {
-                        let g = h.apply(s, u);
-                        return g === !1 && (g = f.apply(s, u)), g
+                        let m = h.apply(s, u);
+                        return m === !1 && (m = f.apply(s, u)), m
                     }
                 }
                 r.hooks = s
             }
             if (i.walkTokens) {
                 const s = this.defaults.walkTokens,
                     o = i.walkTokens;
@@ -21870,15 +21870,15 @@
             const r = "<p>An error occurred:</p><pre>" + Vt(i.message + "", !0) + "</pre>";
             return t ? Promise.resolve(r) : r
         }
         if (t) return Promise.reject(i);
         throw i
     }
 };
-const Gn = new gS;
+const Gn = new mS;
 
 function Ne(n, e) {
     return Gn.parse(n, e)
 }
 Ne.options = Ne.setOptions = function(n) {
     return Gn.setOptions(n), Ne.defaults = Gn.defaults, Yg(Ne.defaults), Ne
 };
@@ -21906,16 +21906,16 @@
 Ne.walkTokens;
 Ne.parseInline;
 Bi.parse;
 Ii.lex; /*! @license DOMPurify 3.0.7 | (c) Cure53 and other contributors | Released under the Apache license 2.0 and Mozilla Public License 2.0 | github.com/cure53/DOMPurify/blob/3.0.7/LICENSE */
 const {
     entries: am,
     setPrototypeOf: _u,
-    isFrozen: mS,
-    getPrototypeOf: yS,
+    isFrozen: yS,
+    getPrototypeOf: bS,
     getOwnPropertyDescriptor: mc
 } = Object;
 let {
     freeze: Lt,
     seal: gi,
     create: hm
 } = Object, {
@@ -21935,112 +21935,112 @@
     return new e(...t)
 });
 const Ao = oi(Array.prototype.forEach),
     Hu = oi(Array.prototype.pop),
     Xr = oi(Array.prototype.push),
     Ho = oi(String.prototype.toLowerCase),
     Ta = oi(String.prototype.toString),
-    bS = oi(String.prototype.match),
+    xS = oi(String.prototype.match),
     Yr = oi(String.prototype.replace),
-    xS = oi(String.prototype.indexOf),
-    kS = oi(String.prototype.trim),
+    kS = oi(String.prototype.indexOf),
+    wS = oi(String.prototype.trim),
     qt = oi(RegExp.prototype.test),
-    Jr = wS(TypeError);
+    Jr = vS(TypeError);
 
 function oi(n) {
     return function(e) {
         for (var t = arguments.length, i = new Array(t > 1 ? t - 1 : 0), r = 1; r < t; r++) i[r - 1] = arguments[r];
         return Eh(n, e, i)
     }
 }
 
-function wS(n) {
+function vS(n) {
     return function() {
         for (var e = arguments.length, t = new Array(e), i = 0; i < e; i++) t[i] = arguments[i];
         return Dh(n, t)
     }
 }
 
 function we(n, e) {
     let t = arguments.length > 2 && arguments[2] !== void 0 ? arguments[2] : Ho;
     _u && _u(n, null);
     let i = e.length;
     for (; i--;) {
         let r = e[i];
         if (typeof r == "string") {
             const s = t(r);
-            s !== r && (mS(e) || (e[i] = s), r = s)
+            s !== r && (yS(e) || (e[i] = s), r = s)
         }
         n[r] = !0
     }
     return n
 }
 
-function vS(n) {
+function SS(n) {
     for (let e = 0; e < n.length; e++) mc(n, e) === void 0 && (n[e] = null);
     return n
 }
 
 function Fn(n) {
     const e = hm(null);
-    for (const [t, i] of am(n)) mc(n, t) !== void 0 && (Array.isArray(i) ? e[t] = vS(i) : typeof i == "object" && i.constructor === Object ? e[t] = Fn(i) : e[t] = i);
+    for (const [t, i] of am(n)) mc(n, t) !== void 0 && (Array.isArray(i) ? e[t] = SS(i) : typeof i == "object" && i.constructor === Object ? e[t] = Fn(i) : e[t] = i);
     return e
 }
 
 function To(n, e) {
     for (; n !== null;) {
         const i = mc(n, e);
         if (i) {
             if (i.get) return oi(i.get);
             if (typeof i.value == "function") return oi(i.value)
         }
-        n = yS(n)
+        n = bS(n)
     }
 
     function t(i) {
         return console.warn("fallback value for", i), null
     }
     return t
 }
 const Fu = Lt(["a", "abbr", "acronym", "address", "area", "article", "aside", "audio", "b", "bdi", "bdo", "big", "blink", "blockquote", "body", "br", "button", "canvas", "caption", "center", "cite", "code", "col", "colgroup", "content", "data", "datalist", "dd", "decorator", "del", "details", "dfn", "dialog", "dir", "div", "dl", "dt", "element", "em", "fieldset", "figcaption", "figure", "font", "footer", "form", "h1", "h2", "h3", "h4", "h5", "h6", "head", "header", "hgroup", "hr", "html", "i", "img", "input", "ins", "kbd", "label", "legend", "li", "main", "map", "mark", "marquee", "menu", "menuitem", "meter", "nav", "nobr", "ol", "optgroup", "option", "output", "p", "picture", "pre", "progress", "q", "rp", "rt", "ruby", "s", "samp", "section", "select", "shadow", "small", "source", "spacer", "span", "strike", "strong", "style", "sub", "summary", "sup", "table", "tbody", "td", "template", "textarea", "tfoot", "th", "thead", "time", "tr", "track", "tt", "u", "ul", "var", "video", "wbr"]),
     Oa = Lt(["svg", "a", "altglyph", "altglyphdef", "altglyphitem", "animatecolor", "animatemotion", "animatetransform", "circle", "clippath", "defs", "desc", "ellipse", "filter", "font", "g", "glyph", "glyphref", "hkern", "image", "line", "lineargradient", "marker", "mask", "metadata", "mpath", "path", "pattern", "polygon", "polyline", "radialgradient", "rect", "stop", "style", "switch", "symbol", "text", "textpath", "title", "tref", "tspan", "view", "vkern"]),
     Ma = Lt(["feBlend", "feColorMatrix", "feComponentTransfer", "feComposite", "feConvolveMatrix", "feDiffuseLighting", "feDisplacementMap", "feDistantLight", "feDropShadow", "feFlood", "feFuncA", "feFuncB", "feFuncG", "feFuncR", "feGaussianBlur", "feImage", "feMerge", "feMergeNode", "feMorphology", "feOffset", "fePointLight", "feSpecularLighting", "feSpotLight", "feTile", "feTurbulence"]),
-    SS = Lt(["animate", "color-profile", "cursor", "discard", "font-face", "font-face-format", "font-face-name", "font-face-src", "font-face-uri", "foreignobject", "hatch", "hatchpath", "mesh", "meshgradient", "meshpatch", "meshrow", "missing-glyph", "script", "set", "solidcolor", "unknown", "use"]),
+    CS = Lt(["animate", "color-profile", "cursor", "discard", "font-face", "font-face-format", "font-face-name", "font-face-src", "font-face-uri", "foreignobject", "hatch", "hatchpath", "mesh", "meshgradient", "meshpatch", "meshrow", "missing-glyph", "script", "set", "solidcolor", "unknown", "use"]),
     Ea = Lt(["math", "menclose", "merror", "mfenced", "mfrac", "mglyph", "mi", "mlabeledtr", "mmultiscripts", "mn", "mo", "mover", "mpadded", "mphantom", "mroot", "mrow", "ms", "mspace", "msqrt", "mstyle", "msub", "msup", "msubsup", "mtable", "mtd", "mtext", "mtr", "munder", "munderover", "mprescripts"]),
-    CS = Lt(["maction", "maligngroup", "malignmark", "mlongdiv", "mscarries", "mscarry", "msgroup", "mstack", "msline", "msrow", "semantics", "annotation", "annotation-xml", "mprescripts", "none"]),
+    AS = Lt(["maction", "maligngroup", "malignmark", "mlongdiv", "mscarries", "mscarry", "msgroup", "mstack", "msline", "msrow", "semantics", "annotation", "annotation-xml", "mprescripts", "none"]),
     zu = Lt(["#text"]),
     $u = Lt(["accept", "action", "align", "alt", "autocapitalize", "autocomplete", "autopictureinpicture", "autoplay", "background", "bgcolor", "border", "capture", "cellpadding", "cellspacing", "checked", "cite", "class", "clear", "color", "cols", "colspan", "controls", "controlslist", "coords", "crossorigin", "datetime", "decoding", "default", "dir", "disabled", "disablepictureinpicture", "disableremoteplayback", "download", "draggable", "enctype", "enterkeyhint", "face", "for", "headers", "height", "hidden", "high", "href", "hreflang", "id", "inputmode", "integrity", "ismap", "kind", "label", "lang", "list", "loading", "loop", "low", "max", "maxlength", "media", "method", "min", "minlength", "multiple", "muted", "name", "nonce", "noshade", "novalidate", "nowrap", "open", "optimum", "pattern", "placeholder", "playsinline", "poster", "preload", "pubdate", "radiogroup", "readonly", "rel", "required", "rev", "reversed", "role", "rows", "rowspan", "spellcheck", "scope", "selected", "shape", "size", "sizes", "span", "srclang", "start", "src", "srcset", "step", "style", "summary", "tabindex", "title", "translate", "type", "usemap", "valign", "value", "width", "xmlns", "slot"]),
     Da = Lt(["accent-height", "accumulate", "additive", "alignment-baseline", "ascent", "attributename", "attributetype", "azimuth", "basefrequency", "baseline-shift", "begin", "bias", "by", "class", "clip", "clippathunits", "clip-path", "clip-rule", "color", "color-interpolation", "color-interpolation-filters", "color-profile", "color-rendering", "cx", "cy", "d", "dx", "dy", "diffuseconstant", "direction", "display", "divisor", "dur", "edgemode", "elevation", "end", "fill", "fill-opacity", "fill-rule", "filter", "filterunits", "flood-color", "flood-opacity", "font-family", "font-size", "font-size-adjust", "font-stretch", "font-style", "font-variant", "font-weight", "fx", "fy", "g1", "g2", "glyph-name", "glyphref", "gradientunits", "gradienttransform", "height", "href", "id", "image-rendering", "in", "in2", "k", "k1", "k2", "k3", "k4", "kerning", "keypoints", "keysplines", "keytimes", "lang", "lengthadjust", "letter-spacing", "kernelmatrix", "kernelunitlength", "lighting-color", "local", "marker-end", "marker-mid", "marker-start", "markerheight", "markerunits", "markerwidth", "maskcontentunits", "maskunits", "max", "mask", "media", "method", "mode", "min", "name", "numoctaves", "offset", "operator", "opacity", "order", "orient", "orientation", "origin", "overflow", "paint-order", "path", "pathlength", "patterncontentunits", "patterntransform", "patternunits", "points", "preservealpha", "preserveaspectratio", "primitiveunits", "r", "rx", "ry", "radius", "refx", "refy", "repeatcount", "repeatdur", "restart", "result", "rotate", "scale", "seed", "shape-rendering", "specularconstant", "specularexponent", "spreadmethod", "startoffset", "stddeviation", "stitchtiles", "stop-color", "stop-opacity", "stroke-dasharray", "stroke-dashoffset", "stroke-linecap", "stroke-linejoin", "stroke-miterlimit", "stroke-opacity", "stroke", "stroke-width", "style", "surfacescale", "systemlanguage", "tabindex", "targetx", "targety", "transform", "transform-origin", "text-anchor", "text-decoration", "text-rendering", "textlength", "type", "u1", "u2", "unicode", "values", "viewbox", "visibility", "version", "vert-adv-y", "vert-origin-x", "vert-origin-y", "width", "word-spacing", "wrap", "writing-mode", "xchannelselector", "ychannelselector", "x", "x1", "x2", "xmlns", "y", "y1", "y2", "z", "zoomandpan"]),
     Wu = Lt(["accent", "accentunder", "align", "bevelled", "close", "columnsalign", "columnlines", "columnspan", "denomalign", "depth", "dir", "display", "displaystyle", "encoding", "fence", "frame", "height", "href", "id", "largeop", "length", "linethickness", "lspace", "lquote", "mathbackground", "mathcolor", "mathsize", "mathvariant", "maxsize", "minsize", "movablelimits", "notation", "numalign", "open", "rowalign", "rowlines", "rowspacing", "rowspan", "rspace", "rquote", "scriptlevel", "scriptminsize", "scriptsizemultiplier", "selection", "separator", "separators", "stretchy", "subscriptshift", "supscriptshift", "symmetric", "voffset", "width", "xmlns"]),
     Oo = Lt(["xlink:href", "xml:id", "xlink:title", "xml:space", "xmlns:xlink"]),
-    AS = gi(/\{\{[\w\W]*|[\w\W]*\}\}/gm),
-    TS = gi(/<%[\w\W]*|[\w\W]*%>/gm),
-    OS = gi(/\${[\w\W]*}/gm),
-    MS = gi(/^data-[\-\w.\u00B7-\uFFFF]/),
-    ES = gi(/^aria-[\-\w]+$/),
+    TS = gi(/\{\{[\w\W]*|[\w\W]*\}\}/gm),
+    OS = gi(/<%[\w\W]*|[\w\W]*%>/gm),
+    MS = gi(/\${[\w\W]*}/gm),
+    ES = gi(/^data-[\-\w.\u00B7-\uFFFF]/),
+    DS = gi(/^aria-[\-\w]+$/),
     cm = gi(/^(?:(?:(?:f|ht)tps?|mailto|tel|callto|sms|cid|xmpp):|[^a-z]|[a-z+.\-]+(?:[^a-z+.\-:]|$))/i),
-    DS = gi(/^(?:\w+script|data):/i),
-    RS = gi(/[\u0000-\u0020\u00A0\u1680\u180E\u2000-\u2029\u205F\u3000]/g),
+    RS = gi(/^(?:\w+script|data):/i),
+    LS = gi(/[\u0000-\u0020\u00A0\u1680\u180E\u2000-\u2029\u205F\u3000]/g),
     fm = gi(/^html$/i);
 var qu = Object.freeze({
     __proto__: null,
-    MUSTACHE_EXPR: AS,
-    ERB_EXPR: TS,
-    TMPLIT_EXPR: OS,
-    DATA_ATTR: MS,
-    ARIA_ATTR: ES,
+    MUSTACHE_EXPR: TS,
+    ERB_EXPR: OS,
+    TMPLIT_EXPR: MS,
+    DATA_ATTR: ES,
+    ARIA_ATTR: DS,
     IS_ALLOWED_URI: cm,
-    IS_SCRIPT_OR_DATA: DS,
-    ATTR_WHITESPACE: RS,
+    IS_SCRIPT_OR_DATA: RS,
+    ATTR_WHITESPACE: LS,
     DOCTYPE_NAME: fm
 });
-const LS = function() {
+const PS = function() {
         return typeof window == "undefined" ? null : window
     },
-    PS = function(e, t) {
+    NS = function(e, t) {
         if (typeof e != "object" || typeof e.createPolicy != "function") return null;
         let i = null;
         const r = "data-tt-policy-suffix";
         t && t.hasAttribute(r) && (i = t.getAttribute(r));
         const s = "dompurify" + (i ? "#" + i : "");
         try {
             return e.createPolicy(s, {
@@ -22053,35 +22053,35 @@
             })
         } catch (o) {
             return console.warn("TrustedTypes policy " + s + " could not be created."), null
         }
     };
 
 function um() {
-    let n = arguments.length > 0 && arguments[0] !== void 0 ? arguments[0] : LS();
+    let n = arguments.length > 0 && arguments[0] !== void 0 ? arguments[0] : PS();
     const e = se => um(se);
     if (e.version = "3.0.7", e.removed = [], !n || !n.document || n.document.nodeType !== 9) return e.isSupported = !1, e;
     let {
         document: t
     } = n;
     const i = t,
         r = i.currentScript,
         {
             DocumentFragment: s,
             HTMLTemplateElement: o,
             Node: l,
             Element: h,
             NodeFilter: f,
             NamedNodeMap: u = n.NamedNodeMap || n.MozNamedAttrMap,
-            HTMLFormElement: g,
+            HTMLFormElement: m,
             DOMParser: y,
             trustedTypes: k
         } = n,
         v = h.prototype,
-        C = To(v, "cloneNode"),
+        A = To(v, "cloneNode"),
         O = To(v, "nextSibling"),
         D = To(v, "childNodes"),
         F = To(v, "parentNode");
     if (typeof o == "function") {
         const se = t.createElement("template");
         se.content && se.content.ownerDocument && (t = se.content.ownerDocument)
     }
@@ -22105,15 +22105,15 @@
         IS_SCRIPT_OR_DATA: st,
         ATTR_WHITESPACE: _e
     } = qu;
     let {
         IS_ALLOWED_URI: Ye
     } = qu, be = null;
     const We = we({}, [...Fu, ...Oa, ...Ma, ...Ea, ...zu]);
-    let Ae = null;
+    let Ce = null;
     const bt = we({}, [...$u, ...Da, ...Wu, ...Oo]);
     let Oe = Object.seal(hm(null, {
             tagNameCheck: {
                 writable: !0,
                 configurable: !1,
                 enumerable: !0,
                 value: null
@@ -22171,27 +22171,27 @@
     const nn = t.createElement("form"),
         rn = function(R) {
             return R instanceof RegExp || R instanceof Function
         },
         er = function() {
             let R = arguments.length > 0 && arguments[0] !== void 0 ? arguments[0] : {};
             if (!(tn && tn === R)) {
-                if ((!R || typeof R != "object") && (R = {}), R = Fn(R), Rn = Zn.indexOf(R.PARSER_MEDIA_TYPE) === -1 ? Hs : R.PARSER_MEDIA_TYPE, Ge = Rn === "application/xhtml+xml" ? Ta : Ho, be = "ALLOWED_TAGS" in R ? we({}, R.ALLOWED_TAGS, Ge) : We, Ae = "ALLOWED_ATTR" in R ? we({}, R.ALLOWED_ATTR, Ge) : bt, ai = "ALLOWED_NAMESPACES" in R ? we({}, R.ALLOWED_NAMESPACES, Ta) : en, Rr = "ADD_URI_SAFE_ATTR" in R ? we(Fn(_s), R.ADD_URI_SAFE_ATTR, Ge) : _s, ne = "ADD_DATA_URI_TAGS" in R ? we(Fn(ct), R.ADD_DATA_URI_TAGS, Ge) : ct, Xt = "FORBID_CONTENTS" in R ? we({}, R.FORBID_CONTENTS, Ge) : Zi, Tt = "FORBID_TAGS" in R ? we({}, R.FORBID_TAGS, Ge) : {}, yi = "FORBID_ATTR" in R ? we({}, R.FORBID_ATTR, Ge) : {}, ht = "USE_PROFILES" in R ? R.USE_PROFILES : !1, On = R.ALLOW_ARIA_ATTR !== !1, Mr = R.ALLOW_DATA_ATTR !== !1, Bs = R.ALLOW_UNKNOWN_PROTOCOLS || !1, Er = R.ALLOW_SELF_CLOSE_IN_ATTR !== !1, at = R.SAFE_FOR_TEMPLATES || !1, zi = R.WHOLE_DOCUMENT || !1, $i = R.RETURN_DOM || !1, Yn = R.RETURN_DOM_FRAGMENT || !1, Ji = R.RETURN_TRUSTED_TYPE || !1, Yi = R.FORCE_BODY || !1, Mn = R.SANITIZE_DOM !== !1, Kt = R.SANITIZE_NAMED_PROPS || !1, Dr = R.KEEP_CONTENT !== !1, En = R.IN_PLACE || !1, Ye = R.ALLOWED_URI_REGEXP || cm, Jt = R.NAMESPACE || Yt, Oe = R.CUSTOM_ELEMENT_HANDLING || {}, R.CUSTOM_ELEMENT_HANDLING && rn(R.CUSTOM_ELEMENT_HANDLING.tagNameCheck) && (Oe.tagNameCheck = R.CUSTOM_ELEMENT_HANDLING.tagNameCheck), R.CUSTOM_ELEMENT_HANDLING && rn(R.CUSTOM_ELEMENT_HANDLING.attributeNameCheck) && (Oe.attributeNameCheck = R.CUSTOM_ELEMENT_HANDLING.attributeNameCheck), R.CUSTOM_ELEMENT_HANDLING && typeof R.CUSTOM_ELEMENT_HANDLING.allowCustomizedBuiltInElements == "boolean" && (Oe.allowCustomizedBuiltInElements = R.CUSTOM_ELEMENT_HANDLING.allowCustomizedBuiltInElements), at && (Mr = !1), Yn && ($i = !0), ht && (be = we({}, zu), Ae = [], ht.html === !0 && (we(be, Fu), we(Ae, $u)), ht.svg === !0 && (we(be, Oa), we(Ae, Da), we(Ae, Oo)), ht.svgFilters === !0 && (we(be, Ma), we(Ae, Da), we(Ae, Oo)), ht.mathMl === !0 && (we(be, Ea), we(Ae, Wu), we(Ae, Oo))), R.ADD_TAGS && (be === We && (be = Fn(be)), we(be, R.ADD_TAGS, Ge)), R.ADD_ATTR && (Ae === bt && (Ae = Fn(Ae)), we(Ae, R.ADD_ATTR, Ge)), R.ADD_URI_SAFE_ATTR && we(Rr, R.ADD_URI_SAFE_ATTR, Ge), R.FORBID_CONTENTS && (Xt === Zi && (Xt = Fn(Xt)), we(Xt, R.FORBID_CONTENTS, Ge)), Dr && (be["#text"] = !0), zi && we(be, ["html", "head", "body"]), be.table && (we(be, ["tbody"]), delete Tt.tbody), R.TRUSTED_TYPES_POLICY) {
+                if ((!R || typeof R != "object") && (R = {}), R = Fn(R), Rn = Zn.indexOf(R.PARSER_MEDIA_TYPE) === -1 ? Hs : R.PARSER_MEDIA_TYPE, Ge = Rn === "application/xhtml+xml" ? Ta : Ho, be = "ALLOWED_TAGS" in R ? we({}, R.ALLOWED_TAGS, Ge) : We, Ce = "ALLOWED_ATTR" in R ? we({}, R.ALLOWED_ATTR, Ge) : bt, ai = "ALLOWED_NAMESPACES" in R ? we({}, R.ALLOWED_NAMESPACES, Ta) : en, Rr = "ADD_URI_SAFE_ATTR" in R ? we(Fn(_s), R.ADD_URI_SAFE_ATTR, Ge) : _s, ne = "ADD_DATA_URI_TAGS" in R ? we(Fn(ct), R.ADD_DATA_URI_TAGS, Ge) : ct, Xt = "FORBID_CONTENTS" in R ? we({}, R.FORBID_CONTENTS, Ge) : Zi, Tt = "FORBID_TAGS" in R ? we({}, R.FORBID_TAGS, Ge) : {}, yi = "FORBID_ATTR" in R ? we({}, R.FORBID_ATTR, Ge) : {}, ht = "USE_PROFILES" in R ? R.USE_PROFILES : !1, On = R.ALLOW_ARIA_ATTR !== !1, Mr = R.ALLOW_DATA_ATTR !== !1, Bs = R.ALLOW_UNKNOWN_PROTOCOLS || !1, Er = R.ALLOW_SELF_CLOSE_IN_ATTR !== !1, at = R.SAFE_FOR_TEMPLATES || !1, zi = R.WHOLE_DOCUMENT || !1, $i = R.RETURN_DOM || !1, Yn = R.RETURN_DOM_FRAGMENT || !1, Ji = R.RETURN_TRUSTED_TYPE || !1, Yi = R.FORCE_BODY || !1, Mn = R.SANITIZE_DOM !== !1, Kt = R.SANITIZE_NAMED_PROPS || !1, Dr = R.KEEP_CONTENT !== !1, En = R.IN_PLACE || !1, Ye = R.ALLOWED_URI_REGEXP || cm, Jt = R.NAMESPACE || Yt, Oe = R.CUSTOM_ELEMENT_HANDLING || {}, R.CUSTOM_ELEMENT_HANDLING && rn(R.CUSTOM_ELEMENT_HANDLING.tagNameCheck) && (Oe.tagNameCheck = R.CUSTOM_ELEMENT_HANDLING.tagNameCheck), R.CUSTOM_ELEMENT_HANDLING && rn(R.CUSTOM_ELEMENT_HANDLING.attributeNameCheck) && (Oe.attributeNameCheck = R.CUSTOM_ELEMENT_HANDLING.attributeNameCheck), R.CUSTOM_ELEMENT_HANDLING && typeof R.CUSTOM_ELEMENT_HANDLING.allowCustomizedBuiltInElements == "boolean" && (Oe.allowCustomizedBuiltInElements = R.CUSTOM_ELEMENT_HANDLING.allowCustomizedBuiltInElements), at && (Mr = !1), Yn && ($i = !0), ht && (be = we({}, zu), Ce = [], ht.html === !0 && (we(be, Fu), we(Ce, $u)), ht.svg === !0 && (we(be, Oa), we(Ce, Da), we(Ce, Oo)), ht.svgFilters === !0 && (we(be, Ma), we(Ce, Da), we(Ce, Oo)), ht.mathMl === !0 && (we(be, Ea), we(Ce, Wu), we(Ce, Oo))), R.ADD_TAGS && (be === We && (be = Fn(be)), we(be, R.ADD_TAGS, Ge)), R.ADD_ATTR && (Ce === bt && (Ce = Fn(Ce)), we(Ce, R.ADD_ATTR, Ge)), R.ADD_URI_SAFE_ATTR && we(Rr, R.ADD_URI_SAFE_ATTR, Ge), R.FORBID_CONTENTS && (Xt === Zi && (Xt = Fn(Xt)), we(Xt, R.FORBID_CONTENTS, Ge)), Dr && (be["#text"] = !0), zi && we(be, ["html", "head", "body"]), be.table && (we(be, ["tbody"]), delete Tt.tbody), R.TRUSTED_TYPES_POLICY) {
                     if (typeof R.TRUSTED_TYPES_POLICY.createHTML != "function") throw Jr('TRUSTED_TYPES_POLICY configuration option must provide a "createHTML" hook.');
                     if (typeof R.TRUSTED_TYPES_POLICY.createScriptURL != "function") throw Jr('TRUSTED_TYPES_POLICY configuration option must provide a "createScriptURL" hook.');
                     $ = R.TRUSTED_TYPES_POLICY, j = $.createHTML("")
-                } else $ === void 0 && ($ = PS(k, r)), $ !== null && typeof j == "string" && (j = $.createHTML(""));
+                } else $ === void 0 && ($ = NS(k, r)), $ !== null && typeof j == "string" && (j = $.createHTML(""));
                 Lt && Lt(R), tn = R
             }
         },
         Lr = we({}, ["mi", "mo", "mn", "ms", "mtext"]),
         Ot = we({}, ["foreignobject", "desc", "title", "annotation-xml"]),
         xt = we({}, ["title", "style", "font", "a", "script"]),
-        tr = we({}, [...Oa, ...Ma, ...SS]),
-        Fs = we({}, [...Ea, ...CS]),
+        tr = we({}, [...Oa, ...Ma, ...CS]),
+        Fs = we({}, [...Ea, ...AS]),
         zs = function(R) {
             let V = F(R);
             (!V || !V.tagName) && (V = {
                 namespaceURI: Jt,
                 tagName: "template"
             });
             const Y = Ho(R.tagName),
@@ -22216,27 +22216,27 @@
                 })
             } catch (Y) {
                 Xr(e.removed, {
                     attribute: null,
                     from: V
                 })
             }
-            if (V.removeAttribute(R), R === "is" && !Ae[R])
+            if (V.removeAttribute(R), R === "is" && !Ce[R])
                 if ($i || Yn) try {
                     xi(V)
                 } catch (Y) {} else try {
                     V.setAttribute(R, "")
                 } catch (Y) {}
         },
         Wi = function(R) {
             let V = null,
                 Y = null;
             if (Yi) R = "<remove></remove>" + R;
             else {
-                const Ze = bS(R, /^[\r\n\t ]+/);
+                const Ze = xS(R, /^[\r\n\t ]+/);
                 Y = Ze && Ze[0]
             }
             Rn === "application/xhtml+xml" && Jt === Yt && (R = '<html xmlns="http://www.w3.org/1999/xhtml"><head></head><body>' + R + "</body></html>");
             const Re = $ ? $.createHTML(R) : R;
             if (Jt === Yt) try {
                 V = new y().parseFromString(Re, Rn)
             } catch (Ze) {}
@@ -22249,15 +22249,15 @@
             const Ke = V.body || V.documentElement;
             return R && Y && Ke.insertBefore(t.createTextNode(Y), Ke.childNodes[0] || null), Jt === Yt ? he.call(V, zi ? "html" : "body")[0] : zi ? V.documentElement : Ke
         },
         ir = function(R) {
             return G.call(R.ownerDocument || R, R, f.SHOW_ELEMENT | f.SHOW_COMMENT | f.SHOW_TEXT, null)
         },
         nr = function(R) {
-            return R instanceof g && (typeof R.nodeName != "string" || typeof R.textContent != "string" || typeof R.removeChild != "function" || !(R.attributes instanceof u) || typeof R.removeAttribute != "function" || typeof R.setAttribute != "function" || typeof R.namespaceURI != "string" || typeof R.insertBefore != "function" || typeof R.hasChildNodes != "function")
+            return R instanceof m && (typeof R.nodeName != "string" || typeof R.textContent != "string" || typeof R.removeChild != "function" || !(R.attributes instanceof u) || typeof R.removeAttribute != "function" || typeof R.setAttribute != "function" || typeof R.namespaceURI != "string" || typeof R.insertBefore != "function" || typeof R.hasChildNodes != "function")
         },
         $s = function(R) {
             return typeof l == "function" && R instanceof l
         },
         hi = function(R, V, Y) {
             ae[R] && Ao(ae[R], Re => {
                 Re.call(e, V, Y, tn)
@@ -22274,34 +22274,34 @@
             if (!be[Y] || Tt[Y]) {
                 if (!Tt[Y] && qs(Y) && (Oe.tagNameCheck instanceof RegExp && qt(Oe.tagNameCheck, Y) || Oe.tagNameCheck instanceof Function && Oe.tagNameCheck(Y))) return !1;
                 if (Dr && !Xt[Y]) {
                     const Re = F(R) || R.parentNode,
                         Ke = D(R) || R.childNodes;
                     if (Ke && Re) {
                         const Ze = Ke.length;
-                        for (let kt = Ze - 1; kt >= 0; --kt) Re.insertBefore(C(Ke[kt], !0), O(R))
+                        for (let kt = Ze - 1; kt >= 0; --kt) Re.insertBefore(A(Ke[kt], !0), O(R))
                     }
                 }
                 return xi(R), !0
             }
             return R instanceof h && !zs(R) || (Y === "noscript" || Y === "noembed" || Y === "noframes") && qt(/<\/no(script|embed|frames)/i, R.innerHTML) ? (xi(R), !0) : (at && R.nodeType === 3 && (V = R.textContent, Ao([pe, fe, ie], Re => {
                 V = Yr(V, Re, " ")
             }), R.textContent !== V && (Xr(e.removed, {
                 element: R.cloneNode()
             }), R.textContent = V)), hi("afterSanitizeElements", R, null), !1)
         },
         Pr = function(R, V, Y) {
             if (Mn && (V === "id" || V === "name") && (Y in t || Y in nn)) return !1;
             if (!(Mr && !yi[V] && qt(ye, V))) {
                 if (!(On && qt(Be, V))) {
-                    if (!Ae[V] || yi[V]) {
+                    if (!Ce[V] || yi[V]) {
                         if (!(qs(R) && (Oe.tagNameCheck instanceof RegExp && qt(Oe.tagNameCheck, R) || Oe.tagNameCheck instanceof Function && Oe.tagNameCheck(R)) && (Oe.attributeNameCheck instanceof RegExp && qt(Oe.attributeNameCheck, V) || Oe.attributeNameCheck instanceof Function && Oe.attributeNameCheck(V)) || V === "is" && Oe.allowCustomizedBuiltInElements && (Oe.tagNameCheck instanceof RegExp && qt(Oe.tagNameCheck, Y) || Oe.tagNameCheck instanceof Function && Oe.tagNameCheck(Y)))) return !1
                     } else if (!Rr[V]) {
                         if (!qt(Ye, Yr(Y, _e, ""))) {
-                            if (!((V === "src" || V === "xlink:href" || V === "href") && R !== "script" && xS(Y, "data:") === 0 && ne[R])) {
+                            if (!((V === "src" || V === "xlink:href" || V === "href") && R !== "script" && kS(Y, "data:") === 0 && ne[R])) {
                                 if (!(Bs && !qt(st, Yr(Y, _e, "")))) {
                                     if (Y) return !1
                                 }
                             }
                         }
                     }
                 }
@@ -22317,26 +22317,26 @@
                 attributes: V
             } = R;
             if (!V) return;
             const Y = {
                 attrName: "",
                 attrValue: "",
                 keepAttr: !0,
-                allowedAttributes: Ae
+                allowedAttributes: Ce
             };
             let Re = V.length;
             for (; Re--;) {
                 const Ke = V[Re],
                     {
                         name: Ze,
                         namespaceURI: kt,
                         value: zt
                     } = Ke,
                     sn = Ge(Ze);
-                let ft = Ze === "value" ? zt : kS(zt);
+                let ft = Ze === "value" ? zt : wS(zt);
                 if (Y.attrName = sn, Y.attrValue = ft, Y.keepAttr = !0, Y.forceKeepAttr = void 0, hi("uponSanitizeAttribute", R, Y), ft = Y.attrValue, Y.forceKeepAttr || (ki(Ze, R), !Y.keepAttr)) continue;
                 if (!Er && qt(/\/>/i, ft)) {
                     ki(Ze, R);
                     continue
                 }
                 at && Ao([pe, fe, ie], Ir => {
                     ft = Yr(ft, Ir, " ")
@@ -22391,15 +22391,15 @@
         const Ze = ir(En ? se : V);
         for (; Re = Ze.nextNode();) Ws(Re) || (Re.content instanceof s && Vs(Re.content), js(Re));
         if (En) return se;
         if ($i) {
             if (Yn)
                 for (Ke = p.call(V.ownerDocument); V.firstChild;) Ke.appendChild(V.firstChild);
             else Ke = V;
-            return (Ae.shadowroot || Ae.shadowrootmode) && (Ke = J.call(i, Ke, !0)), Ke
+            return (Ce.shadowroot || Ce.shadowrootmode) && (Ke = J.call(i, Ke, !0)), Ke
         }
         let kt = zi ? V.outerHTML : V.innerHTML;
         return zi && be["!doctype"] && V.ownerDocument && V.ownerDocument.doctype && V.ownerDocument.doctype.name && qt(fm, V.ownerDocument.doctype.name) && (kt = "<!DOCTYPE " + V.ownerDocument.doctype.name + `>
 ` + kt), at && Ao([pe, fe, ie], zt => {
             kt = Yr(kt, zt, " ")
         }), $ && Ji ? $.createHTML(kt) : kt
     }, e.setConfig = function() {
@@ -22418,91 +22418,93 @@
         if (ae[se]) return Hu(ae[se])
     }, e.removeHooks = function(se) {
         ae[se] && (ae[se] = [])
     }, e.removeAllHooks = function() {
         ae = {}
     }, e
 }
-var NS = um();
-const IS = '<div class="spinner-border text-primary" role="status"><span class="visually-hidden">Loading...</span></div>';
+var IS = um();
 
-function ju() {
+function dm() {
     const n = document.querySelector(".alert-danger.db-error");
     return n ? n.textContent.trim() : null
 }
 
-function BS(n = !1) {
-    const e = ju();
+function BS() {
+    document.getElementById("search_assistant_tables").focus()
+}
+
+function _S(n = !1) {
+    const e = dm();
     if (n || e) {
         const l = document.getElementById("assistant_collapse");
-        if (new Jm(l, {
-                toggle: !1
-            }).show(), e) {
-            const f = document.getElementById("id_assistant_input");
-            f.value = "Please help me fix the error(s) in this query.";
-            const u = document.createElement("div");
-            u.textContent = 'Error messages are automatically included in the prompt. Just hit "Ask Assistant" and all relevant context will be injected to the LLM request.', u.className = "text-secondary small", f.parentNode.insertBefore(u, f.nextSibling)
-        }
-    } [...document.querySelectorAll('[data-bs-toggle="tooltip"]')].map(l => new Zm(l)), fetch("../schema.json/" + Ce("#id_connection").val()).then(l => l.json()).then(l => {
+        new Zm(l, {
+            toggle: !1
+        }).show(), e && document.getElementById("id_error_help_message").classList.remove("d-none")
+    } [...document.querySelectorAll('[data-bs-toggle="tooltip"]')].map(l => new e0(l)), fetch("../schema.json/" + Te("#id_connection").val()).then(l => l.json()).then(l => {
         const h = Object.keys(l),
             f = document.getElementById("table-list");
-        f.innerHTML = "", h.forEach((g, y) => {
+        f.innerHTML = "", h.forEach((m, y) => {
             const k = document.createElement("div");
             k.className = "form-check";
             const v = document.createElement("input");
-            v.className = "form-check-input table-checkbox", v.type = "checkbox", v.value = g, v.id = "flexCheckDefault" + y;
-            const C = document.createElement("label");
-            C.className = "form-check-label", C.setAttribute("for", v.id), C.textContent = g, k.appendChild(v), k.appendChild(C), f.appendChild(k)
+            v.className = "form-check-input table-checkbox", v.type = "checkbox", v.value = m, v.id = "flexCheckDefault" + y;
+            const A = document.createElement("label");
+            A.className = "form-check-label", A.setAttribute("for", v.id), A.textContent = m, k.appendChild(v), k.appendChild(A), f.appendChild(k)
         });
         let u = {
             valueNames: ["form-check-label"]
         };
         new Vu("additional_table_container", u)
     }).catch(l => {
         console.error("Error retrieving JSON schema:", l)
     });
     const i = document.getElementById("include_other_tables"),
         r = document.getElementById("additional_table_container"),
         s = document.getElementById("assistant_input_wrapper");
 
     function o(l) {
-        l ? (r.classList.remove("d-none"), s.classList.remove("col-12"), s.classList.add("col-9")) : (r.classList.add("d-none"), s.classList.remove("col-9"), s.classList.add("col-12"))
+        l ? (r.classList.remove("d-none"), s.classList.remove("col-12"), s.classList.add("col-9"), BS()) : (r.classList.add("d-none"), s.classList.remove("col-9"), s.classList.add("col-12"))
     }
     i.addEventListener("change", function() {
         o(this.checked)
-    }), o(i.checked), document.getElementById("ask_assistant_btn").addEventListener("click", function() {
-        var f, u, g, y, k, v;
-        const l = Array.from(document.querySelectorAll(".table-checkbox:checked")).map(C => C.value),
-            h = {
-                sql: (u = (f = window.editor) == null ? void 0 : f.state.doc.toString()) != null ? u : null,
-                connection: (y = (g = document.getElementById("id_connection")) == null ? void 0 : g.value) != null ? y : null,
-                assistant_request: (v = (k = document.getElementById("id_assistant_input")) == null ? void 0 : k.value) != null ? v : null,
-                selected_tables: l,
-                db_error: ju()
-            };
-        document.getElementById("response_block").style.display = "block", document.getElementById("assistant_response").innerHTML = IS, fetch("/assistant/", {
-            method: "POST",
-            headers: {
-                "Content-Type": "application/json",
-                "X-CSRFToken": Uu()
-            },
-            body: JSON.stringify(h)
-        }).then(C => {
-            if (!C.ok) throw new Error("Network response was not ok");
-            return C.json()
-        }).then(C => {
-            const O = NS.sanitize(Ne.parse(C.message));
-            document.getElementById("response_block").style.display = "block", document.getElementById("assistant_response").innerHTML = O, _S()
-        }).catch(C => {
-            console.error("Error:", C)
-        })
+    }), o(i.checked), document.getElementById("id_assistant_input").addEventListener("keydown", function(l) {
+        (l.ctrlKey || l.metaKey) && l.key === "Enter" && (l.preventDefault(), ju())
+    }), document.getElementById("ask_assistant_btn").addEventListener("click", ju)
+}
+
+function ju() {
+    var t, i, r, s, o, l;
+    const n = Array.from(document.querySelectorAll(".table-checkbox:checked")).map(h => h.value),
+        e = {
+            sql: (i = (t = window.editor) == null ? void 0 : t.state.doc.toString()) != null ? i : null,
+            connection: (s = (r = document.getElementById("id_connection")) == null ? void 0 : r.value) != null ? s : null,
+            assistant_request: (l = (o = document.getElementById("id_assistant_input")) == null ? void 0 : o.value) != null ? l : null,
+            selected_tables: n,
+            db_error: dm()
+        };
+    document.getElementById("response_block").classList.remove("d-none"), document.getElementById("assistant_spinner").classList.remove("d-none"), fetch("../assistant/", {
+        method: "POST",
+        headers: {
+            "Content-Type": "application/json",
+            "X-CSRFToken": Uu()
+        },
+        body: JSON.stringify(e)
+    }).then(h => {
+        if (!h.ok) throw new Error("Network response was not ok");
+        return h.json()
+    }).then(h => {
+        const f = IS.sanitize(Ne.parse(h.message));
+        document.getElementById("assistant_response").innerHTML = f, HS()
+    }).catch(h => {
+        console.error("Error:", h)
     })
 }
 
-function _S() {
+function HS() {
     document.querySelectorAll("#assistant_response pre").forEach(n => {
         const e = document.createElement("i");
         e.classList.add("copy-btn"), e.classList.add("bi-copy");
         const t = document.createElement("span");
         t.textContent = "Copied!", t.style.display = "none", t.style.marginLeft = "8px", e.appendChild(t), n.appendChild(e), e.addEventListener("click", function() {
             const i = this.parentNode.firstElementChild.innerText;
             navigator.clipboard.writeText(i).then(() => {
@@ -22512,34 +22514,34 @@
             }).catch(r => {
                 console.error("Error in copying text: ", r)
             })
         })
     })
 }
 
-function HS(n) {
+function FS(n) {
     let e = new te({
         doc: n.value,
-        extensions: [Nv]
+        extensions: [Iv]
     });
     return n.parentNode.insertBefore(e.dom, n), n.style.display = "none", n.form && n.form.addEventListener("submit", () => {
         n.value = e.state.doc.toString()
     }), e
 }
-class VS {
+class US {
     constructor(e) {
         ze(this, "handleBeforeUnload", e => {
             if (clientRoute === "query_detail" && this.docChanged) {
                 const t = "You have unsaved changes to your query.";
                 return e.returnValue = t, t
             }
         });
         const t = document.getElementById("assistant_accordion"),
             i = document.getElementById("nav-preview");
-        t && BS(!i && e === "new"), this.queryId = e, this.$table = Ce("#preview"), this.$rows = Ce("#rows"), this.$form = Ce("form"), this.$snapshotField = Ce("#id_snapshot"), this.docChanged = !1, this.$submit = Ce("#refresh_play_button, #save_button"), this.$submit.length || (this.$submit = Ce("#refresh_button")), this.editor = HS(document.getElementById("id_sql")), window.editor = this.editor, document.addEventListener("submitEventFromCM", r => {
+        t && _S(!i && e === "new"), this.queryId = e, this.$rows = Te("#rows"), this.$form = Te("form"), this.$snapshotField = Te("#id_snapshot"), this.docChanged = !1, this.$submit = Te("#refresh_play_button, #save_button"), this.$submit.length || (this.$submit = Te("#refresh_button")), this.editor = FS(document.getElementById("id_sql")), window.editor = this.editor, document.addEventListener("submitEventFromCM", r => {
             this.$submit.click()
         }), document.addEventListener("docChanged", r => {
             this.docChanged = !0
         }), this.bind(), Jl.get("schema_sidebar_open") === "true" && this.showSchema(!0)
     }
     getParams() {
         let e = !1;
@@ -22585,56 +22587,56 @@
     }
     showRows() {
         let e = document.getElementById("rows").value,
             t = document.getElementById("editor");
         t.setAttribute("action", this.updateQueryString("rows", e, window.location.href)), t.submit()
     }
     showSchema(e) {
-        Ce("#schema_frame").attr("src", "../schema/" + Ce("#id_connection").val()), e === !0 && Ce("#schema_frame").addClass("no-autofocus"), Ce("#query_area").removeClass("col").addClass("col-9");
-        var t = Ce("#schema");
-        return t.addClass("col-md-3"), t.show(), Ce("#show_schema_button").hide(), Ce("#hide_schema_button").show(), Jl.set("schema_sidebar_open", "true"), !1
+        Te("#schema_frame").attr("src", "../schema/" + Te("#id_connection").val()), e === !0 && Te("#schema_frame").addClass("no-autofocus"), Te("#query_area").removeClass("col").addClass("col-9");
+        var t = Te("#schema");
+        return t.addClass("col-md-3"), t.show(), Te("#show_schema_button").hide(), Te("#hide_schema_button").show(), Jl.set("schema_sidebar_open", "true"), !1
     }
     hideSchema() {
-        Ce("#query_area").removeClass("col-9").addClass("col");
-        var e = Ce("#schema");
-        return e.removeClass("col-3"), e.hide(), Ce("#hide_schema_button").hide(), Ce("#show_schema_button").show(), Jl.set("schema_sidebar_open", "false"), !1
+        Te("#query_area").removeClass("col-9").addClass("col");
+        var e = Te("#schema");
+        return e.removeClass("col-3"), e.hide(), Te("#hide_schema_button").hide(), Te("#show_schema_button").show(), Jl.set("schema_sidebar_open", "false"), !1
     }
     bind() {
         window.addEventListener("beforeunload", this.handleBeforeUnload), document.addEventListener("submit", r => {
             r.target.id === "editor" && window.removeEventListener("beforeunload", this.handleBeforeUnload)
         }), document.querySelectorAll(".query_favorite_toggle").forEach(function(r) {
-            r.addEventListener("click", n0)
-        }), document.getElementById("show_schema_button").addEventListener("click", this.showSchema.bind(this)), document.getElementById("hide_schema_button").addEventListener("click", this.hideSchema.bind(this)), Ce("#format_button").click(function(r) {
+            r.addEventListener("click", r0)
+        }), document.getElementById("show_schema_button").addEventListener("click", this.showSchema.bind(this)), document.getElementById("hide_schema_button").addEventListener("click", this.hideSchema.bind(this)), Te("#format_button").click(function(r) {
             r.preventDefault(), this.formatSql()
-        }.bind(this)), Ce("#rows").keyup(function() {
-            var r = Ce("#fullscreen").attr("href"),
-                s = r.replace(/rows=\d+/, "rows=" + Ce("#rows").val());
-            Ce("#fullscreen").attr("href", s)
-        }.bind(this)), Ce("#save_button").click(function() {
+        }.bind(this)), Te("#rows").keyup(function() {
+            var r = Te("#fullscreen").attr("href"),
+                s = r.replace(/rows=\d+/, "rows=" + Te("#rows").val());
+            Te("#fullscreen").attr("href", s)
+        }.bind(this)), Te("#save_button").click(function() {
             var r = this.getParams(this);
             r && this.$form.attr("action", "../" + this.queryId + "/?params=" + this.serializeParams(r)), this.$snapshotField.hide(), this.$form.append(this.$snapshotField)
-        }.bind(this)), Ce("#save_only_button").click(function() {
+        }.bind(this)), Te("#save_only_button").click(function() {
             var r = this.getParams(this);
             r ? this.$form.attr("action", "../" + this.queryId + "/?show=0&params=" + this.serializeParams(r)) : this.$form.attr("action", "../" + this.queryId + "/?show=0"), this.$snapshotField.hide(), this.$form.append(this.$snapshotField)
-        }.bind(this)), Ce("#refresh_button").click(function(r) {
+        }.bind(this)), Te("#refresh_button").click(function(r) {
             r.preventDefault();
             var s = this.getParams();
             s ? window.location.href = "../" + this.queryId + "/?params=" + this.serializeParams(s) : window.location.href = "../" + this.queryId + "/"
-        }.bind(this)), Ce("#refresh_play_button").click(function() {
+        }.bind(this)), Te("#refresh_play_button").click(function() {
             this.$form.attr("action", "../play/")
-        }.bind(this)), Ce("#playground_button").click(function(r) {
+        }.bind(this)), Te("#playground_button").click(function(r) {
             r.preventDefault(), this.$form.attr("action", "../play/?show=0"), this.$form.submit()
-        }.bind(this)), Ce("#create_button").click(function() {
+        }.bind(this)), Te("#create_button").click(function() {
             this.$form.attr("action", "../new/")
-        }.bind(this)), Ce(".download-button").click(function(r) {
-            var s = "../download?format=" + Ce(r.target).data("format"),
+        }.bind(this)), Te(".download-button").click(function(r) {
+            var s = "../download?format=" + Te(r.target).data("format"),
                 o = this.getParams();
             o && (s = s + "&params=" + o), this.$form.attr("action", s)
-        }.bind(this)), Ce(".download-query-button").click(function(r) {
-            var s = "../download?format=" + Ce(r.target).data("format"),
+        }.bind(this)), Te(".download-query-button").click(function(r) {
+            var s = "../download?format=" + Te(r.target).data("format"),
                 o = this.getParams();
             o && (s = s + "&params=" + o), this.$form.attr("action", s)
         }.bind(this)), document.querySelectorAll(".stats-expand").forEach(r => {
             r.addEventListener("click", function(s) {
                 s.preventDefault(), document.querySelectorAll(".stats-expand").forEach(o => o.style.display = "none"), document.querySelectorAll(".stats-wrapper").forEach(o => o.style.display = "")
             })
         });
@@ -22657,34 +22659,34 @@
                 document.querySelectorAll(".sort").forEach(l => {
                     l.classList.add("bi-chevron-expand"), l.classList.remove("bi-chevron-down", "bi-chevron-up")
                 }), o.classList.contains("asc") ? (o.classList.replace("bi-chevron-expand", "bi-chevron-up"), o.classList.remove("bi-chevron-down")) : (o.classList.replace("bi-chevron-expand", "bi-chevron-down"), o.classList.remove("bi-chevron-up"))
             }.bind(this))
         });
         const i = document.querySelector('button[data-bs-target="#nav-pivot"]');
         i && i.addEventListener("shown.bs.tab", r => {
-            e0(() => import("./pivot-setup.js"), __vite__mapDeps([0, 1, 2, 3]), import.meta.url).then(({
+            t0(() => import("./pivot-setup.js"), __vite__mapDeps([0, 1, 2, 3]), import.meta.url).then(({
                 pivotSetup: s
-            }) => s(Ce))
+            }) => s(Te))
         }), window.location.hash && document.querySelector("#nav-pivot-tab").click(), this.$rows.change(function() {
             this.showRows()
         }.bind(this)), this.$rows.keyup(function(r) {
             r.keyCode === 13 && this.showRows()
-        }.bind(this)), fetch("../schema.json/" + Ce("#id_connection").val()).then(r => r.json()).then(r => (this.editor.dispatch({
+        }.bind(this)), fetch("../schema.json/" + Te("#id_connection").val()).then(r => r.json()).then(r => (this.editor.dispatch({
             effects: me.appendConfig.of(Dl.language.data.of({
                 autocomplete: Xg({
                     schema: r
                 })
             }))
         }), r)).catch(r => {
             console.error("Error retrieving JSON schema:", r)
         })
     }
 }
 export {
-    VS as ExplorerEditor
+    US as ExplorerEditor
 };
 
 function __vite__mapDeps(indexes) {
     if (!__vite__mapDeps.viteFileDeps) {
         __vite__mapDeps.viteFileDeps = ["./pivot-setup.js", "./main.js", "./index.js", "./favorites.js"]
     }
     return indexes.map((i) => __vite__mapDeps.viteFileDeps[i])
```

### Comparing `django_sql_explorer-4.1b5/explorer/static/explorer/favorites.js` & `django_sql_explorer-4.1b6/explorer/static/explorer/favorites.js`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b5/explorer/static/explorer/index.js` & `django_sql_explorer-4.1b6/explorer/static/explorer/index.js`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b5/explorer/static/explorer/main.js` & `django_sql_explorer-4.1b6/explorer/static/explorer/main.js`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b5/explorer/static/explorer/pivot-setup.js` & `django_sql_explorer-4.1b6/explorer/static/explorer/pivot-setup.js`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b5/explorer/static/explorer/query-list.js` & `django_sql_explorer-4.1b6/explorer/static/explorer/query-list.js`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b5/explorer/static/explorer/schema.js` & `django_sql_explorer-4.1b6/explorer/static/explorer/schema.js`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b5/explorer/static/explorer/styles.css` & `django_sql_explorer-4.1b6/explorer/static/explorer/styles.css`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b5/explorer/tasks.py` & `django_sql_explorer-4.1b6/explorer/tasks.py`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b5/explorer/templates/explorer/assistant.html` & `django_sql_explorer-4.1b6/explorer/templates/explorer/assistant.html`

 * *Files 16% similar despite different names*

```diff
@@ -8,42 +8,49 @@
         </div>
     </div>
     <div id="assistant_collapse" class="accordion-collapse collapse" aria-labelledby="assistant_accordion_header" data-bs-parent="#assistant_accordion">
         <div class="accordion-body">
             <div class="row assistant_input_parent">
                 <div class="mt-3 col-12" id="assistant_input_wrapper">
                     <textarea
-                        class="form-control" id="id_assistant_input"
+                        class="form-control mb-4" id="id_assistant_input"
                         name="sql_assistant" rows="3" placeholder="What do you need help with?"></textarea>
-                    <label for="id_assistant_input" class="form-label" id="id_assistant_input_label"></label>
+                    <label for="id_assistant_input" class="form-label d-none" id="id_assistant_input_label">Assistant prompt</label>
+                    <div id="id_error_help_message" class="d-none text-secondary small">
+                        Hit "Ask Assistant" to try and fix the issue. The assistant is automatically aware of error messages & context.
+                    </div>
                 </div>
                 <div id="additional_table_container" class="d-none col-3">
                     <input id="search_assistant_tables" class="search" placeholder="{% trans "Search Tables" %}" />
                     <label for="search_assistant_tables" class="d-none" id="search_assistant_tables_label">Search tables</label>
                     <div id="table-list" class="list"></div>
                 </div>
             </div>
 
             <div class="row">
                 <div class="col-6">
                     <div class="form-check form-check-inline">
                         <input type="checkbox" class="form-check-input" name="assistant-include-other-tables" id="include_other_tables" autocomplete="off">
                         <label class="form-check-label" for="include_other_tables">Include Other Tables (<a class="small text-secondary" style="cursor: pointer;"
                             data-bs-toggle="tooltip" data-bs-placement="top"
-                            data-bs-title="SQL Assistant builds a prompt with your query, your request, relevant schema (tables referenced in your query) and sample data from those tables. You can optionally include other tables (schema + data sample) that you'd like SQL Assistant to know about.">What is this?</a>)</label>
+                            data-bs-title="SQL Assistant builds a prompt with your query, your request, relevant schema (tables referenced in your query) and sample data from those tables. You can optionally include other tables (schema + data sample) that you'd like SQL Assistant to know about.">?</a>)</label>
                     </div>
                 </div>
                 <div class="col-6 text-end">
                     <div class="btn-group" role="group">
                         <button type="button" class="btn btn-outline-primary" id="ask_assistant_btn">Ask Assistant</button>
                     </div>
                 </div>
             </div>
 
 
-            <div id="response_block" style="display: none" class="position-relative">
-                <div class="mt-3 p-2 pt-3 rounded-2 border bg-light" id="assistant_response"></div>
+            <div id="response_block" class="position-relative d-none">
+                <div class="mt-3 p-2 pt-4 rounded-2 border bg-light" id="assistant_response">
+                    <p class="spinner-border text-primary d-none" id="assistant_spinner" role="status">
+                        <span class="visually-hidden">Loading...</span>
+                    </p>
+                </div>
             </div>
         </div>
     </div>
 </div>
```

### Comparing `django_sql_explorer-4.1b5/explorer/templates/explorer/base.html` & `django_sql_explorer-4.1b6/explorer/templates/explorer/base.html`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b5/explorer/templates/explorer/export_buttons.html` & `django_sql_explorer-4.1b6/explorer/templates/explorer/export_buttons.html`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b5/explorer/templates/explorer/fullscreen.html` & `django_sql_explorer-4.1b6/explorer/templates/explorer/fullscreen.html`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b5/explorer/templates/explorer/params.html` & `django_sql_explorer-4.1b6/explorer/templates/explorer/params.html`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b5/explorer/templates/explorer/pdf_template.html` & `django_sql_explorer-4.1b6/explorer/templates/explorer/pdf_template.html`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b5/explorer/templates/explorer/play.html` & `django_sql_explorer-4.1b6/explorer/templates/explorer/play.html`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b5/explorer/templates/explorer/preview_pane.html` & `django_sql_explorer-4.1b6/explorer/templates/explorer/preview_pane.html`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b5/explorer/templates/explorer/query.html` & `django_sql_explorer-4.1b6/explorer/templates/explorer/query.html`

 * *Files 2% similar despite different names*

```diff
@@ -58,15 +58,14 @@
                         id="id_description" class="form-control" cols="40" name="description"
                         {% if not can_change %}disabled{% endif %} rows="2"
                     >{{ form.description.value|default_if_none:"" }}</textarea>
                     <label for="id_description" class="form-label">
                         {% trans "Description"%}
                     </label>
                 </div>
-                <input type="hidden" id="id_created_by_user" name="created_by_user" value="{{ form.created_by_user_email }}" />
                 {% if form.sql.errors %}
                     {% for error in form.sql.errors %}
                         <div class="alert alert-danger">{{ error|escape }}</div>
                     {% endfor %}
                 {% endif %}
                 <div class ="accordion accordion-flush" id="sql_accordion">
                     <div class="accordion-item">
@@ -138,16 +137,16 @@
     </div>
 </div>
 
 {% include 'explorer/preview_pane.html' %}
 
 <div class="container mt-1 text-end small">
     {% if query.avg_duration %}
-        {% blocktrans trimmed with avg_duration_display=query.avg_duration_display user_email=form.created_by_user_email created=form.created_at_time %}
-            Avg. execution: {{ avg_duration_display }}ms. Query created by {{ user_email }} on {{ created }}.
+        {% blocktrans trimmed with avg_duration_display=query.avg_duration_display cuser=query.created_by_user created=form.created_at_time %}
+            Avg. execution: {{ avg_duration_display }}ms. Query created by {{ cuser }} on {{ created }}.
         {% endblocktrans %}
         {% if query %}<a href="{% url 'explorer_logs' %}?query_id={{ query.id }}"> {% trans "History" %}</a>{% endif %}
     {% endif %}
 </div>
 <div class="container mt-1 text-end small">
     {% if query and can_change and tasks_enabled %}{{ form.snapshot }} {% trans "Snapshot" %}{% endif %}
 </div>
```

### Comparing `django_sql_explorer-4.1b5/explorer/templates/explorer/query_confirm_delete.html` & `django_sql_explorer-4.1b6/explorer/templates/explorer/query_confirm_delete.html`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b5/explorer/templates/explorer/query_favorites.html` & `django_sql_explorer-4.1b6/explorer/templates/explorer/query_favorites.html`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b5/explorer/templates/explorer/query_list.html` & `django_sql_explorer-4.1b6/explorer/templates/explorer/query_list.html`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b5/explorer/templates/explorer/querylog_list.html` & `django_sql_explorer-4.1b6/explorer/templates/explorer/querylog_list.html`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b5/explorer/templates/explorer/schema.html` & `django_sql_explorer-4.1b6/explorer/templates/explorer/schema.html`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b5/explorer/templatetags/explorer_tags.py` & `django_sql_explorer-4.1b6/explorer/templatetags/explorer_tags.py`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b5/explorer/templatetags/vite.py` & `django_sql_explorer-4.1b6/explorer/templatetags/vite.py`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b5/explorer/tests/factories.py` & `django_sql_explorer-4.1b6/explorer/tests/factories.py`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b5/explorer/tests/settings.py` & `django_sql_explorer-4.1b6/explorer/tests/settings.py`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b5/explorer/tests/test_actions.py` & `django_sql_explorer-4.1b6/explorer/tests/test_actions.py`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b5/explorer/tests/test_apps.py` & `django_sql_explorer-4.1b6/explorer/tests/test_apps.py`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b5/explorer/tests/test_csrf_cookie_name.py` & `django_sql_explorer-4.1b6/explorer/tests/test_csrf_cookie_name.py`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b5/explorer/tests/test_exporters.py` & `django_sql_explorer-4.1b6/explorer/tests/test_exporters.py`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b5/explorer/tests/test_forms.py` & `django_sql_explorer-4.1b6/explorer/tests/test_forms.py`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b5/explorer/tests/test_models.py` & `django_sql_explorer-4.1b6/explorer/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b5/explorer/tests/test_schema.py` & `django_sql_explorer-4.1b6/explorer/tests/test_schema.py`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b5/explorer/tests/test_tasks.py` & `django_sql_explorer-4.1b6/explorer/tests/test_tasks.py`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b5/explorer/tests/test_tracker.py` & `django_sql_explorer-4.1b6/explorer/tests/test_tracker.py`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b5/explorer/tests/test_utils.py` & `django_sql_explorer-4.1b6/explorer/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b5/explorer/tests/test_views.py` & `django_sql_explorer-4.1b6/explorer/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b5/explorer/tracker.py` & `django_sql_explorer-4.1b6/explorer/tracker.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,16 @@
 from enum import Enum, auto
 from django.core.cache import cache
 from django.db import connection
 from django.db.models import Count
 from django.db.migrations.recorder import MigrationRecorder
 from django.conf import settings
 
+import explorer
+
 logger = logging.getLogger(__name__)
 
 
 def _instance_identifier():
     """
     We need a way of identifying unique instances of explorer to track usage.
     There isn"t an established approach I"m aware of, so have come up with
@@ -80,15 +82,15 @@
 def _send(data):
     from explorer import app_settings
     try:
         requests.post(app_settings.EXPLORER_COLLECT_ENDPOINT_URL,
                       data=data,
                       headers={"Content-Type": "application/json"})
     except Exception as e:
-        logger.exception("Failed to send stats: %s" % e)
+        logger.warning("Failed to send stats: %s" % e)
 
 
 def gather_summary_stats():
 
     from explorer import app_settings
     from explorer.models import Query, QueryLog
 
@@ -113,10 +115,11 @@
             "default_database": connection.vendor,
             "django_install_date": install_date,
             "debug": settings.DEBUG,
             "tasks_enabled": app_settings.ENABLE_TASKS,
             "unsafe_rendering": app_settings.UNSAFE_RENDERING,
             "transform_count": len(app_settings.EXPLORER_TRANSFORMS),
             "assistant_enabled": app_settings.EXPLORER_AI_API_KEY is not None,
+            "version": explorer.get_version()
         }
     except Exception as e:
         return {"error": "error gathering stats: %s" % e}
```

### Comparing `django_sql_explorer-4.1b5/explorer/urls.py` & `django_sql_explorer-4.1b6/explorer/urls.py`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b5/explorer/utils.py` & `django_sql_explorer-4.1b6/explorer/utils.py`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b5/explorer/views/__init__.py` & `django_sql_explorer-4.1b6/explorer/views/__init__.py`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b5/explorer/views/auth.py` & `django_sql_explorer-4.1b6/explorer/views/auth.py`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b5/explorer/views/create.py` & `django_sql_explorer-4.1b6/explorer/views/create.py`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b5/explorer/views/download.py` & `django_sql_explorer-4.1b6/explorer/views/download.py`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b5/explorer/views/email.py` & `django_sql_explorer-4.1b6/explorer/views/email.py`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b5/explorer/views/export.py` & `django_sql_explorer-4.1b6/explorer/views/export.py`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b5/explorer/views/list.py` & `django_sql_explorer-4.1b6/explorer/views/list.py`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b5/explorer/views/mixins.py` & `django_sql_explorer-4.1b6/explorer/views/mixins.py`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b5/explorer/views/query.py` & `django_sql_explorer-4.1b6/explorer/views/query.py`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b5/explorer/views/query_favorite.py` & `django_sql_explorer-4.1b6/explorer/views/query_favorite.py`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b5/explorer/views/schema.py` & `django_sql_explorer-4.1b6/explorer/views/schema.py`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b5/explorer/views/stream.py` & `django_sql_explorer-4.1b6/explorer/views/stream.py`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b5/explorer/views/utils.py` & `django_sql_explorer-4.1b6/explorer/views/utils.py`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b5/package.json` & `django_sql_explorer-4.1b6/package.json`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b5/setup.cfg` & `django_sql_explorer-4.1b6/setup.cfg`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b5/setup.py` & `django_sql_explorer-4.1b6/setup.py`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b5/vite.config.js` & `django_sql_explorer-4.1b6/vite.config.js`

 * *Files identical despite different names*

