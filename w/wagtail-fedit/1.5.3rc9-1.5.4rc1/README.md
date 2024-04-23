# Comparing `tmp/wagtail_fedit-1.5.3rc9.tar.gz` & `tmp/wagtail_fedit-1.5.4rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wagtail_fedit-1.5.3rc9.tar", last modified: Sun Apr 21 21:47:14 2024, max compression
+gzip compressed data, was "wagtail_fedit-1.5.4rc1.tar", last modified: Tue Apr 23 15:51:39 2024, max compression
```

## Comparing `wagtail_fedit-1.5.3rc9.tar` & `wagtail_fedit-1.5.4rc1.tar`

### file list

```diff
@@ -1,131 +1,137 @@
-drwxrwxrwx   0        0        0        0 2024-04-21 21:47:14.907633 wagtail_fedit-1.5.3rc9/
--rw-rw-rw-   0        0        0    18429 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.3rc9/LICENSE
--rw-rw-rw-   0        0        0      257 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.3rc9/MANIFEST.in
--rw-rw-rw-   0        0        0    21085 2024-04-21 21:47:14.907633 wagtail_fedit-1.5.3rc9/PKG-INFO
--rw-rw-rw-   0        0        0    19884 2024-04-21 20:38:03.000000 wagtail_fedit-1.5.3rc9/README.md
--rw-rw-rw-   0        0        0       90 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.3rc9/pyproject.toml
--rw-rw-rw-   0        0        0     1189 2024-04-21 21:47:14.921738 wagtail_fedit-1.5.3rc9/setup.cfg
--rw-rw-rw-   0        0        0       39 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.3rc9/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-21 21:47:14.770326 wagtail_fedit-1.5.3rc9/wagtail_fedit/
--rw-rw-rw-   0        0        0        0 2024-03-29 20:13:25.000000 wagtail_fedit-1.5.3rc9/wagtail_fedit/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-21 21:47:14.826150 wagtail_fedit-1.5.3rc9/wagtail_fedit/adapters/
--rw-rw-rw-   0        0        0      518 2024-04-21 16:44:17.000000 wagtail_fedit-1.5.3rc9/wagtail_fedit/adapters/__init__.py
--rw-rw-rw-   0        0        0    11210 2024-04-21 21:26:41.000000 wagtail_fedit-1.5.3rc9/wagtail_fedit/adapters/base.py
--rw-rw-rw-   0        0        0     6215 2024-04-21 21:34:32.000000 wagtail_fedit-1.5.3rc9/wagtail_fedit/adapters/block.py
--rw-rw-rw-   0        0        0     8677 2024-04-21 20:08:37.000000 wagtail_fedit-1.5.3rc9/wagtail_fedit/adapters/field.py
--rw-rw-rw-   0        0        0     2076 2024-04-21 12:09:20.000000 wagtail_fedit-1.5.3rc9/wagtail_fedit/adapters/funcs.py
--rw-rw-rw-   0        0        0     2390 2024-04-21 12:09:35.000000 wagtail_fedit-1.5.3rc9/wagtail_fedit/adapters/misc.py
--rw-rw-rw-   0        0        0     3200 2024-04-21 21:44:02.000000 wagtail_fedit-1.5.3rc9/wagtail_fedit/adapters/models.py
--rw-rw-rw-   0        0        0     1595 2024-04-18 20:22:37.000000 wagtail_fedit-1.5.3rc9/wagtail_fedit/adapters/registry.py
--rw-rw-rw-   0        0        0      163 2024-03-29 20:13:25.000000 wagtail_fedit-1.5.3rc9/wagtail_fedit/apps.py
-drwxrwxrwx   0        0        0        0 2024-04-21 21:47:14.828629 wagtail_fedit-1.5.3rc9/wagtail_fedit/forms/
--rw-rw-rw-   0        0        0       71 2024-04-02 19:03:21.000000 wagtail_fedit-1.5.3rc9/wagtail_fedit/forms/__init__.py
--rw-rw-rw-   0        0        0     2881 2024-04-18 20:27:35.000000 wagtail_fedit-1.5.3rc9/wagtail_fedit/forms/blocks.py
--rw-rw-rw-   0        0        0     3110 2024-04-21 02:24:44.000000 wagtail_fedit-1.5.3rc9/wagtail_fedit/forms/fields.py
--rw-rw-rw-   0        0        0     4617 2024-04-21 02:08:33.000000 wagtail_fedit-1.5.3rc9/wagtail_fedit/hooks.py
-drwxrwxrwx   0        0        0        0 2024-04-21 21:47:14.730902 wagtail_fedit-1.5.3rc9/wagtail_fedit/locale/
-drwxrwxrwx   0        0        0        0 2024-04-21 21:47:14.730902 wagtail_fedit-1.5.3rc9/wagtail_fedit/locale/nl/
-drwxrwxrwx   0        0        0        0 2024-04-21 21:47:14.830628 wagtail_fedit-1.5.3rc9/wagtail_fedit/locale/nl/LC_MESSAGES/
--rw-rw-rw-   0        0        0     7129 2024-04-11 09:05:50.000000 wagtail_fedit-1.5.3rc9/wagtail_fedit/locale/nl/LC_MESSAGES/django.mo
--rw-rw-rw-   0        0        0    12687 2024-04-11 09:05:42.000000 wagtail_fedit-1.5.3rc9/wagtail_fedit/locale/nl/LC_MESSAGES/django.po
-drwxrwxrwx   0        0        0        0 2024-04-21 21:47:14.831628 wagtail_fedit-1.5.3rc9/wagtail_fedit/migrations/
--rw-rw-rw-   0        0        0        0 2024-03-29 20:13:25.000000 wagtail_fedit-1.5.3rc9/wagtail_fedit/migrations/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-21 21:47:14.832728 wagtail_fedit-1.5.3rc9/wagtail_fedit/migrations/__pycache__/
--rw-rw-rw-   0        0        0      215 2024-03-29 21:05:00.000000 wagtail_fedit-1.5.3rc9/wagtail_fedit/migrations/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0        0        0     3170 2024-04-05 20:30:10.000000 wagtail_fedit-1.5.3rc9/wagtail_fedit/models.py
--rw-rw-rw-   0        0        0      973 2024-04-21 00:46:27.000000 wagtail_fedit-1.5.3rc9/wagtail_fedit/settings.py
-drwxrwxrwx   0        0        0        0 2024-04-21 21:47:14.732413 wagtail_fedit-1.5.3rc9/wagtail_fedit/static/
-drwxrwxrwx   0        0        0        0 2024-04-21 21:47:14.733419 wagtail_fedit-1.5.3rc9/wagtail_fedit/static/wagtail_fedit/
-drwxrwxrwx   0        0        0        0 2024-04-21 21:47:14.837025 wagtail_fedit-1.5.3rc9/wagtail_fedit/static/wagtail_fedit/css/
--rw-rw-rw-   0        0        0     5500 2024-04-21 17:02:30.000000 wagtail_fedit-1.5.3rc9/wagtail_fedit/static/wagtail_fedit/css/frontend.css
--rw-rw-rw-   0        0        0     5098 2024-04-17 20:40:49.000000 wagtail_fedit-1.5.3rc9/wagtail_fedit/static/wagtail_fedit/css/furniture.css
--rw-rw-rw-   0        0        0     1266 2024-04-05 19:37:44.000000 wagtail_fedit-1.5.3rc9/wagtail_fedit/static/wagtail_fedit/css/userbar-menu.css
-drwxrwxrwx   0        0        0        0 2024-04-21 21:47:14.838024 wagtail_fedit-1.5.3rc9/wagtail_fedit/static/wagtail_fedit/js/
--rw-rw-rw-   0        0        0    20559 2024-04-21 20:02:32.000000 wagtail_fedit-1.5.3rc9/wagtail_fedit/static/wagtail_fedit/js/frontend.js
-drwxrwxrwx   0        0        0        0 2024-04-21 21:47:14.734419 wagtail_fedit-1.5.3rc9/wagtail_fedit/templates/
-drwxrwxrwx   0        0        0        0 2024-04-21 21:47:14.839912 wagtail_fedit-1.5.3rc9/wagtail_fedit/templates/wagtail_fedit/
--rw-rw-rw-   0        0        0       56 2024-04-16 18:37:39.000000 wagtail_fedit-1.5.3rc9/wagtail_fedit/templates/wagtail_fedit/_hook_output.html
-drwxrwxrwx   0        0        0        0 2024-04-21 21:47:14.841912 wagtail_fedit-1.5.3rc9/wagtail_fedit/templates/wagtail_fedit/content/
-drwxrwxrwx   0        0        0        0 2024-04-21 21:47:14.842909 wagtail_fedit-1.5.3rc9/wagtail_fedit/templates/wagtail_fedit/content/buttons/
--rw-rw-rw-   0        0        0      871 2024-04-19 20:16:18.000000 wagtail_fedit-1.5.3rc9/wagtail_fedit/templates/wagtail_fedit/content/buttons/admin_link.html
--rw-rw-rw-   0        0        0      872 2024-04-19 20:15:44.000000 wagtail_fedit-1.5.3rc9/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_adapter.html
--rw-rw-rw-   0        0        0      534 2024-04-21 17:21:38.000000 wagtail_fedit-1.5.3rc9/wagtail_fedit/templates/wagtail_fedit/content/editable_adapter.html
-drwxrwxrwx   0        0        0        0 2024-04-21 21:47:14.853795 wagtail_fedit-1.5.3rc9/wagtail_fedit/templates/wagtail_fedit/editor/
--rw-rw-rw-   0        0        0     2259 2024-04-11 08:02:26.000000 wagtail_fedit-1.5.3rc9/wagtail_fedit/templates/wagtail_fedit/editor/action_confirm.html
--rw-rw-rw-   0        0        0     3699 2024-04-20 21:55:10.000000 wagtail_fedit-1.5.3rc9/wagtail_fedit/templates/wagtail_fedit/editor/action_publish_confirm.html
--rw-rw-rw-   0        0        0      266 2024-04-21 21:15:09.000000 wagtail_fedit-1.5.3rc9/wagtail_fedit/templates/wagtail_fedit/editor/adapter_edit_handler.html
--rw-rw-rw-   0        0        0      265 2024-04-21 21:23:24.000000 wagtail_fedit-1.5.3rc9/wagtail_fedit/templates/wagtail_fedit/editor/adapter_edit_handler_form.html
--rw-rw-rw-   0        0        0      555 2024-04-21 21:13:45.000000 wagtail_fedit-1.5.3rc9/wagtail_fedit/templates/wagtail_fedit/editor/adapter_form.html
--rw-rw-rw-   0        0        0      455 2024-04-21 00:11:35.000000 wagtail_fedit-1.5.3rc9/wagtail_fedit/templates/wagtail_fedit/editor/adapter_form_errors.html
--rw-rw-rw-   0        0        0      330 2024-04-21 00:12:14.000000 wagtail_fedit-1.5.3rc9/wagtail_fedit/templates/wagtail_fedit/editor/adapter_iframe.html
--rw-rw-rw-   0        0        0     5271 2024-04-21 00:11:24.000000 wagtail_fedit-1.5.3rc9/wagtail_fedit/templates/wagtail_fedit/editor/base_iframe.html
--rw-rw-rw-   0        0        0      496 2024-04-02 17:46:59.000000 wagtail_fedit-1.5.3rc9/wagtail_fedit/templates/wagtail_fedit/editor/field.html
-drwxrwxrwx   0        0        0        0 2024-04-21 21:47:14.859346 wagtail_fedit-1.5.3rc9/wagtail_fedit/templates/wagtail_fedit/icons/
--rw-rw-rw-   0        0        0      797 2024-04-11 08:36:19.000000 wagtail_fedit-1.5.3rc9/wagtail_fedit/templates/wagtail_fedit/icons/fedit-check-list.svg
--rw-rw-rw-   0        0        0      584 2024-04-11 08:36:55.000000 wagtail_fedit-1.5.3rc9/wagtail_fedit/templates/wagtail_fedit/icons/fedit-eye-closed.svg
--rw-rw-rw-   0        0        0      377 2024-04-11 08:23:07.000000 wagtail_fedit-1.5.3rc9/wagtail_fedit/templates/wagtail_fedit/icons/fedit-eye-open.svg
--rw-rw-rw-   0        0        0      725 2024-04-11 09:02:58.000000 wagtail_fedit-1.5.3rc9/wagtail_fedit/templates/wagtail_fedit/icons/fedit-save.svg
--rw-rw-rw-   0        0        0     1323 2024-04-11 08:36:52.000000 wagtail_fedit-1.5.3rc9/wagtail_fedit/templates/wagtail_fedit/icons/fedit-stop-sign.svg
-drwxrwxrwx   0        0        0        0 2024-04-21 21:47:14.861353 wagtail_fedit-1.5.3rc9/wagtail_fedit/templates/wagtail_fedit/userbar/
--rw-rw-rw-   0        0        0      867 2024-04-03 17:05:21.000000 wagtail_fedit-1.5.3rc9/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit.html
--rw-rw-rw-   0        0        0      876 2024-04-03 16:59:31.000000 wagtail_fedit-1.5.3rc9/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_view_live.html
-drwxrwxrwx   0        0        0        0 2024-04-21 21:47:14.863350 wagtail_fedit-1.5.3rc9/wagtail_fedit/templates/wagtail_fedit/userbar/publish/
--rw-rw-rw-   0        0        0      263 2024-04-11 08:24:35.000000 wagtail_fedit-1.5.3rc9/wagtail_fedit/templates/wagtail_fedit/userbar/publish/action_button.html
--rw-rw-rw-   0        0        0      967 2024-04-11 09:03:51.000000 wagtail_fedit-1.5.3rc9/wagtail_fedit/templates/wagtail_fedit/userbar/publish/item_fedit_publishing.html
-drwxrwxrwx   0        0        0        0 2024-04-21 21:47:14.864754 wagtail_fedit-1.5.3rc9/wagtail_fedit/templatetags/
--rw-rw-rw-   0        0        0        0 2024-03-29 20:13:42.000000 wagtail_fedit-1.5.3rc9/wagtail_fedit/templatetags/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-21 21:47:14.867755 wagtail_fedit-1.5.3rc9/wagtail_fedit/templatetags/__pycache__/
--rw-rw-rw-   0        0        0      217 2024-03-29 21:05:00.000000 wagtail_fedit-1.5.3rc9/wagtail_fedit/templatetags/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0        0        0    11089 2024-04-21 18:54:08.000000 wagtail_fedit-1.5.3rc9/wagtail_fedit/templatetags/__pycache__/fedit.cpython-311.pyc
--rw-rw-rw-   0        0        0     8664 2024-04-21 18:53:42.000000 wagtail_fedit-1.5.3rc9/wagtail_fedit/templatetags/fedit.py
-drwxrwxrwx   0        0        0        0 2024-04-21 21:47:14.869295 wagtail_fedit-1.5.3rc9/wagtail_fedit/test/
--rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.3rc9/wagtail_fedit/test/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-21 21:47:14.875293 wagtail_fedit-1.5.3rc9/wagtail_fedit/test/core/
--rw-rw-rw-   0        0        0      151 2024-04-05 07:59:49.000000 wagtail_fedit-1.5.3rc9/wagtail_fedit/test/core/__init__.py
--rw-rw-rw-   0        0        0      165 2024-04-05 08:41:40.000000 wagtail_fedit-1.5.3rc9/wagtail_fedit/test/core/apps.py
--rw-rw-rw-   0        0        0      130 2024-04-15 20:12:38.000000 wagtail_fedit-1.5.3rc9/wagtail_fedit/test/core/context_processors.py
-drwxrwxrwx   0        0        0        0 2024-04-21 21:47:14.879036 wagtail_fedit-1.5.3rc9/wagtail_fedit/test/core/migrations/
--rw-rw-rw-   0        0        0    12115 2024-04-20 22:33:35.000000 wagtail_fedit-1.5.3rc9/wagtail_fedit/test/core/migrations/0001_initial.py
--rw-rw-rw-   0        0        0      509 2024-04-21 18:41:55.000000 wagtail_fedit-1.5.3rc9/wagtail_fedit/test/core/migrations/0002_basicmodel_related_field.py
--rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.3rc9/wagtail_fedit/test/core/migrations/__init__.py
--rw-rw-rw-   0        0        0     5603 2024-04-21 18:39:18.000000 wagtail_fedit-1.5.3rc9/wagtail_fedit/test/core/models.py
-drwxrwxrwx   0        0        0        0 2024-04-21 21:47:14.888150 wagtail_fedit-1.5.3rc9/wagtail_fedit/test/core/tests/
--rw-rw-rw-   0        0        0        0 2024-04-05 07:59:29.000000 wagtail_fedit-1.5.3rc9/wagtail_fedit/test/core/tests/__init__.py
--rw-rw-rw-   0        0        0     8132 2024-04-21 18:49:27.000000 wagtail_fedit-1.5.3rc9/wagtail_fedit/test/core/tests/base.py
--rw-rw-rw-   0        0        0    18772 2024-04-21 19:32:12.000000 wagtail_fedit-1.5.3rc9/wagtail_fedit/test/core/tests/test_adapters.py
--rw-rw-rw-   0        0        0     4320 2024-04-06 22:44:26.000000 wagtail_fedit-1.5.3rc9/wagtail_fedit/test/core/tests/test_block_edit.py
--rw-rw-rw-   0        0        0     5664 2024-04-05 10:31:29.000000 wagtail_fedit-1.5.3rc9/wagtail_fedit/test/core/tests/test_blocks.py
--rw-rw-rw-   0        0        0     3642 2024-04-05 18:00:23.000000 wagtail_fedit-1.5.3rc9/wagtail_fedit/test/core/tests/test_field_edit.py
--rw-rw-rw-   0        0        0     3709 2024-04-10 13:03:30.000000 wagtail_fedit-1.5.3rc9/wagtail_fedit/test/core/tests/test_generic.py
--rw-rw-rw-   0        0        0     1574 2024-04-20 20:49:12.000000 wagtail_fedit-1.5.3rc9/wagtail_fedit/test/core/tests/test_revision.py
--rw-rw-rw-   0        0        0     9545 2024-04-20 21:54:40.000000 wagtail_fedit-1.5.3rc9/wagtail_fedit/test/core/tests/test_submit.py
--rw-rw-rw-   0        0        0      704 2024-04-05 17:55:36.000000 wagtail_fedit-1.5.3rc9/wagtail_fedit/test/manage.py
-drwxrwxrwx   0        0        0        0 2024-04-21 21:47:14.893025 wagtail_fedit-1.5.3rc9/wagtail_fedit/test/testapp/
--rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.3rc9/wagtail_fedit/test/testapp/__init__.py
--rw-rw-rw-   0        0        0      407 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.3rc9/wagtail_fedit/test/testapp/asgi.py
--rw-rw-rw-   0        0        0     3625 2024-04-15 20:14:41.000000 wagtail_fedit-1.5.3rc9/wagtail_fedit/test/testapp/settings.py
--rw-rw-rw-   0        0        0      897 2024-04-05 08:04:53.000000 wagtail_fedit-1.5.3rc9/wagtail_fedit/test/testapp/urls.py
--rw-rw-rw-   0        0        0      407 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.3rc9/wagtail_fedit/test/testapp/wsgi.py
--rw-rw-rw-   0        0        0     2009 2024-04-19 20:04:30.000000 wagtail_fedit-1.5.3rc9/wagtail_fedit/toolbar.py
--rw-rw-rw-   0        0        0      934 2024-04-21 16:55:23.000000 wagtail_fedit-1.5.3rc9/wagtail_fedit/urls.py
--rw-rw-rw-   0        0        0    16829 2024-04-21 18:51:40.000000 wagtail_fedit-1.5.3rc9/wagtail_fedit/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-21 21:47:14.897608 wagtail_fedit-1.5.3rc9/wagtail_fedit/views/
--rw-rw-rw-   0        0        0      190 2024-04-13 19:36:44.000000 wagtail_fedit-1.5.3rc9/wagtail_fedit/views/__init__.py
--rw-rw-rw-   0        0        0     7220 2024-04-21 21:28:24.000000 wagtail_fedit-1.5.3rc9/wagtail_fedit/views/adapters.py
--rw-rw-rw-   0        0        0    17563 2024-04-21 20:25:17.000000 wagtail_fedit-1.5.3rc9/wagtail_fedit/views/editable.py
--rw-rw-rw-   0        0        0     1923 2024-04-21 20:29:01.000000 wagtail_fedit-1.5.3rc9/wagtail_fedit/views/mixins.py
-drwxrwxrwx   0        0        0        0 2024-04-21 21:47:14.906635 wagtail_fedit-1.5.3rc9/wagtail_fedit/wagtail_hooks/
--rw-rw-rw-   0        0        0      184 2024-04-16 10:03:02.000000 wagtail_fedit-1.5.3rc9/wagtail_fedit/wagtail_hooks/__init__.py
--rw-rw-rw-   0        0        0     1748 2024-04-06 18:37:13.000000 wagtail_fedit-1.5.3rc9/wagtail_fedit/wagtail_hooks/action_menu.py
--rw-rw-rw-   0        0        0     2378 2024-04-21 02:17:05.000000 wagtail_fedit-1.5.3rc9/wagtail_fedit/wagtail_hooks/adapter_hooks.py
--rw-rw-rw-   0        0        0      328 2024-04-21 16:44:33.000000 wagtail_fedit-1.5.3rc9/wagtail_fedit/wagtail_hooks/adapter_registry.py
--rw-rw-rw-   0        0        0      398 2024-04-11 09:03:10.000000 wagtail_fedit-1.5.3rc9/wagtail_fedit/wagtail_hooks/icons.py
--rw-rw-rw-   0        0        0     2573 2024-04-11 07:39:50.000000 wagtail_fedit-1.5.3rc9/wagtail_fedit/wagtail_hooks/log_actions.py
--rw-rw-rw-   0        0        0      340 2024-03-30 17:10:05.000000 wagtail_fedit-1.5.3rc9/wagtail_fedit/wagtail_hooks/urls.py
--rw-rw-rw-   0        0        0     7630 2024-04-19 20:11:56.000000 wagtail_fedit-1.5.3rc9/wagtail_fedit/wagtail_hooks/userbar.py
-drwxrwxrwx   0        0        0        0 2024-04-21 21:47:14.814300 wagtail_fedit-1.5.3rc9/wagtail_fedit.egg-info/
--rw-rw-rw-   0        0        0    21085 2024-04-21 21:47:14.000000 wagtail_fedit-1.5.3rc9/wagtail_fedit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     4286 2024-04-21 21:47:14.000000 wagtail_fedit-1.5.3rc9/wagtail_fedit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-21 21:47:14.000000 wagtail_fedit-1.5.3rc9/wagtail_fedit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2024-04-21 21:47:14.000000 wagtail_fedit-1.5.3rc9/wagtail_fedit.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-04-21 21:47:14.000000 wagtail_fedit-1.5.3rc9/wagtail_fedit.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-23 15:51:39.533671 wagtail_fedit-1.5.4rc1/
+-rw-rw-rw-   0        0        0    18429 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.4rc1/LICENSE
+-rw-rw-rw-   0        0        0      257 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.4rc1/MANIFEST.in
+-rw-rw-rw-   0        0        0    21651 2024-04-23 15:51:39.535673 wagtail_fedit-1.5.4rc1/PKG-INFO
+-rw-rw-rw-   0        0        0    20450 2024-04-23 11:23:03.000000 wagtail_fedit-1.5.4rc1/README.md
+-rw-rw-rw-   0        0        0       90 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.4rc1/pyproject.toml
+-rw-rw-rw-   0        0        0     1189 2024-04-23 15:51:39.546302 wagtail_fedit-1.5.4rc1/setup.cfg
+-rw-rw-rw-   0        0        0       39 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.4rc1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-23 15:51:38.776287 wagtail_fedit-1.5.4rc1/wagtail_fedit/
+-rw-rw-rw-   0        0        0        0 2024-03-29 20:13:25.000000 wagtail_fedit-1.5.4rc1/wagtail_fedit/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-23 15:51:38.873340 wagtail_fedit-1.5.4rc1/wagtail_fedit/adapters/
+-rw-rw-rw-   0        0        0      532 2024-04-22 21:01:35.000000 wagtail_fedit-1.5.4rc1/wagtail_fedit/adapters/__init__.py
+-rw-rw-rw-   0        0        0    14330 2024-04-23 15:34:38.000000 wagtail_fedit-1.5.4rc1/wagtail_fedit/adapters/base.py
+-rw-rw-rw-   0        0        0     6408 2024-04-23 15:37:06.000000 wagtail_fedit-1.5.4rc1/wagtail_fedit/adapters/block.py
+-rw-rw-rw-   0        0        0     8508 2024-04-23 15:38:57.000000 wagtail_fedit-1.5.4rc1/wagtail_fedit/adapters/field.py
+-rw-rw-rw-   0        0        0     2671 2024-04-22 20:52:19.000000 wagtail_fedit-1.5.4rc1/wagtail_fedit/adapters/funcs.py
+-rw-rw-rw-   0        0        0     2739 2024-04-23 14:30:53.000000 wagtail_fedit-1.5.4rc1/wagtail_fedit/adapters/misc.py
+-rw-rw-rw-   0        0        0     4632 2024-04-23 15:46:14.000000 wagtail_fedit-1.5.4rc1/wagtail_fedit/adapters/models.py
+-rw-rw-rw-   0        0        0     1595 2024-04-18 20:22:37.000000 wagtail_fedit-1.5.4rc1/wagtail_fedit/adapters/registry.py
+-rw-rw-rw-   0        0        0      163 2024-03-29 20:13:25.000000 wagtail_fedit-1.5.4rc1/wagtail_fedit/apps.py
+drwxrwxrwx   0        0        0        0 2024-04-23 15:51:38.912174 wagtail_fedit-1.5.4rc1/wagtail_fedit/forms/
+-rw-rw-rw-   0        0        0      215 2024-04-23 13:02:23.000000 wagtail_fedit-1.5.4rc1/wagtail_fedit/forms/__init__.py
+-rw-rw-rw-   0        0        0     2881 2024-04-18 20:27:35.000000 wagtail_fedit-1.5.4rc1/wagtail_fedit/forms/blocks.py
+-rw-rw-rw-   0        0        0     3269 2024-04-23 13:28:56.000000 wagtail_fedit-1.5.4rc1/wagtail_fedit/forms/fields.py
+-rw-rw-rw-   0        0        0     4617 2024-04-21 02:08:33.000000 wagtail_fedit-1.5.4rc1/wagtail_fedit/hooks.py
+drwxrwxrwx   0        0        0        0 2024-04-23 15:51:38.722243 wagtail_fedit-1.5.4rc1/wagtail_fedit/locale/
+drwxrwxrwx   0        0        0        0 2024-04-23 15:51:38.723450 wagtail_fedit-1.5.4rc1/wagtail_fedit/locale/nl/
+drwxrwxrwx   0        0        0        0 2024-04-23 15:51:38.938357 wagtail_fedit-1.5.4rc1/wagtail_fedit/locale/nl/LC_MESSAGES/
+-rw-rw-rw-   0        0        0     7262 2024-04-23 15:50:58.000000 wagtail_fedit-1.5.4rc1/wagtail_fedit/locale/nl/LC_MESSAGES/django.mo
+-rw-rw-rw-   0        0        0    13018 2024-04-23 15:50:49.000000 wagtail_fedit-1.5.4rc1/wagtail_fedit/locale/nl/LC_MESSAGES/django.po
+drwxrwxrwx   0        0        0        0 2024-04-23 15:51:38.939337 wagtail_fedit-1.5.4rc1/wagtail_fedit/migrations/
+-rw-rw-rw-   0        0        0        0 2024-03-29 20:13:25.000000 wagtail_fedit-1.5.4rc1/wagtail_fedit/migrations/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-23 15:51:38.941301 wagtail_fedit-1.5.4rc1/wagtail_fedit/migrations/__pycache__/
+-rw-rw-rw-   0        0        0      215 2024-03-29 21:05:00.000000 wagtail_fedit-1.5.4rc1/wagtail_fedit/migrations/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0     3170 2024-04-05 20:30:10.000000 wagtail_fedit-1.5.4rc1/wagtail_fedit/models.py
+-rw-rw-rw-   0        0        0     1452 2024-04-21 22:19:50.000000 wagtail_fedit-1.5.4rc1/wagtail_fedit/settings.py
+drwxrwxrwx   0        0        0        0 2024-04-23 15:51:38.725221 wagtail_fedit-1.5.4rc1/wagtail_fedit/static/
+drwxrwxrwx   0        0        0        0 2024-04-23 15:51:38.725221 wagtail_fedit-1.5.4rc1/wagtail_fedit/static/wagtail_fedit/
+drwxrwxrwx   0        0        0        0 2024-04-23 15:51:38.965348 wagtail_fedit-1.5.4rc1/wagtail_fedit/static/wagtail_fedit/css/
+-rw-rw-rw-   0        0        0     5750 2024-04-23 15:45:28.000000 wagtail_fedit-1.5.4rc1/wagtail_fedit/static/wagtail_fedit/css/frontend.css
+-rw-rw-rw-   0        0        0     5098 2024-04-17 20:40:49.000000 wagtail_fedit-1.5.4rc1/wagtail_fedit/static/wagtail_fedit/css/furniture.css
+-rw-rw-rw-   0        0        0     1266 2024-04-05 19:37:44.000000 wagtail_fedit-1.5.4rc1/wagtail_fedit/static/wagtail_fedit/css/userbar-menu.css
+drwxrwxrwx   0        0        0        0 2024-04-23 15:51:38.994192 wagtail_fedit-1.5.4rc1/wagtail_fedit/static/wagtail_fedit/js/
+-rw-rw-rw-   0        0        0    21312 2024-04-23 15:26:37.000000 wagtail_fedit-1.5.4rc1/wagtail_fedit/static/wagtail_fedit/js/frontend.js
+drwxrwxrwx   0        0        0        0 2024-04-23 15:51:38.726220 wagtail_fedit-1.5.4rc1/wagtail_fedit/static/wagtail_fedit/vendor/
+drwxrwxrwx   0        0        0        0 2024-04-23 15:51:39.087093 wagtail_fedit-1.5.4rc1/wagtail_fedit/static/wagtail_fedit/vendor/tippy/
+-rw-rw-rw-   0        0        0     1091 2024-04-23 15:39:19.000000 wagtail_fedit-1.5.4rc1/wagtail_fedit/static/wagtail_fedit/vendor/tippy/LICENSE
+-rw-rw-rw-   0        0        0    20122 2024-04-23 14:51:23.000000 wagtail_fedit-1.5.4rc1/wagtail_fedit/static/wagtail_fedit/vendor/tippy/popper.min.js
+-rw-rw-rw-   0        0        0    25717 2024-04-23 14:51:31.000000 wagtail_fedit-1.5.4rc1/wagtail_fedit/static/wagtail_fedit/vendor/tippy/tippy-bundle.min.js
+drwxrwxrwx   0        0        0        0 2024-04-23 15:51:38.727222 wagtail_fedit-1.5.4rc1/wagtail_fedit/templates/
+drwxrwxrwx   0        0        0        0 2024-04-23 15:51:39.097873 wagtail_fedit-1.5.4rc1/wagtail_fedit/templates/wagtail_fedit/
+-rw-rw-rw-   0        0        0       56 2024-04-16 18:37:39.000000 wagtail_fedit-1.5.4rc1/wagtail_fedit/templates/wagtail_fedit/_hook_output.html
+drwxrwxrwx   0        0        0        0 2024-04-23 15:51:39.107895 wagtail_fedit-1.5.4rc1/wagtail_fedit/templates/wagtail_fedit/content/
+drwxrwxrwx   0        0        0        0 2024-04-23 15:51:39.130990 wagtail_fedit-1.5.4rc1/wagtail_fedit/templates/wagtail_fedit/content/buttons/
+-rw-rw-rw-   0        0        0      929 2024-04-23 15:23:24.000000 wagtail_fedit-1.5.4rc1/wagtail_fedit/templates/wagtail_fedit/content/buttons/admin_link.html
+-rw-rw-rw-   0        0        0      991 2024-04-23 15:27:54.000000 wagtail_fedit-1.5.4rc1/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_adapter.html
+-rw-rw-rw-   0        0        0      534 2024-04-21 17:21:38.000000 wagtail_fedit-1.5.4rc1/wagtail_fedit/templates/wagtail_fedit/content/editable_adapter.html
+drwxrwxrwx   0        0        0        0 2024-04-23 15:51:39.218760 wagtail_fedit-1.5.4rc1/wagtail_fedit/templates/wagtail_fedit/editor/
+-rw-rw-rw-   0        0        0     2259 2024-04-11 08:02:26.000000 wagtail_fedit-1.5.4rc1/wagtail_fedit/templates/wagtail_fedit/editor/action_confirm.html
+-rw-rw-rw-   0        0        0     3699 2024-04-20 21:55:10.000000 wagtail_fedit-1.5.4rc1/wagtail_fedit/templates/wagtail_fedit/editor/action_publish_confirm.html
+-rw-rw-rw-   0        0        0      266 2024-04-21 21:15:09.000000 wagtail_fedit-1.5.4rc1/wagtail_fedit/templates/wagtail_fedit/editor/adapter_edit_handler.html
+-rw-rw-rw-   0        0        0      265 2024-04-21 21:23:24.000000 wagtail_fedit-1.5.4rc1/wagtail_fedit/templates/wagtail_fedit/editor/adapter_edit_handler_form.html
+-rw-rw-rw-   0        0        0      555 2024-04-21 21:13:45.000000 wagtail_fedit-1.5.4rc1/wagtail_fedit/templates/wagtail_fedit/editor/adapter_form.html
+-rw-rw-rw-   0        0        0      455 2024-04-21 00:11:35.000000 wagtail_fedit-1.5.4rc1/wagtail_fedit/templates/wagtail_fedit/editor/adapter_form_errors.html
+-rw-rw-rw-   0        0        0      330 2024-04-21 00:12:14.000000 wagtail_fedit-1.5.4rc1/wagtail_fedit/templates/wagtail_fedit/editor/adapter_iframe.html
+-rw-rw-rw-   0        0        0     5271 2024-04-21 00:11:24.000000 wagtail_fedit-1.5.4rc1/wagtail_fedit/templates/wagtail_fedit/editor/base_iframe.html
+-rw-rw-rw-   0        0        0      496 2024-04-02 17:46:59.000000 wagtail_fedit-1.5.4rc1/wagtail_fedit/templates/wagtail_fedit/editor/field.html
+drwxrwxrwx   0        0        0        0 2024-04-23 15:51:39.260760 wagtail_fedit-1.5.4rc1/wagtail_fedit/templates/wagtail_fedit/icons/
+-rw-rw-rw-   0        0        0      797 2024-04-11 08:36:19.000000 wagtail_fedit-1.5.4rc1/wagtail_fedit/templates/wagtail_fedit/icons/fedit-check-list.svg
+-rw-rw-rw-   0        0        0      584 2024-04-11 08:36:55.000000 wagtail_fedit-1.5.4rc1/wagtail_fedit/templates/wagtail_fedit/icons/fedit-eye-closed.svg
+-rw-rw-rw-   0        0        0      377 2024-04-11 08:23:07.000000 wagtail_fedit-1.5.4rc1/wagtail_fedit/templates/wagtail_fedit/icons/fedit-eye-open.svg
+-rw-rw-rw-   0        0        0      725 2024-04-11 09:02:58.000000 wagtail_fedit-1.5.4rc1/wagtail_fedit/templates/wagtail_fedit/icons/fedit-save.svg
+-rw-rw-rw-   0        0        0     1323 2024-04-11 08:36:52.000000 wagtail_fedit-1.5.4rc1/wagtail_fedit/templates/wagtail_fedit/icons/fedit-stop-sign.svg
+drwxrwxrwx   0        0        0        0 2024-04-23 15:51:39.277374 wagtail_fedit-1.5.4rc1/wagtail_fedit/templates/wagtail_fedit/userbar/
+-rw-rw-rw-   0        0        0      867 2024-04-03 17:05:21.000000 wagtail_fedit-1.5.4rc1/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit.html
+-rw-rw-rw-   0        0        0      876 2024-04-03 16:59:31.000000 wagtail_fedit-1.5.4rc1/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_view_live.html
+drwxrwxrwx   0        0        0        0 2024-04-23 15:51:39.293236 wagtail_fedit-1.5.4rc1/wagtail_fedit/templates/wagtail_fedit/userbar/publish/
+-rw-rw-rw-   0        0        0      263 2024-04-11 08:24:35.000000 wagtail_fedit-1.5.4rc1/wagtail_fedit/templates/wagtail_fedit/userbar/publish/action_button.html
+-rw-rw-rw-   0        0        0      967 2024-04-11 09:03:51.000000 wagtail_fedit-1.5.4rc1/wagtail_fedit/templates/wagtail_fedit/userbar/publish/item_fedit_publishing.html
+drwxrwxrwx   0        0        0        0 2024-04-23 15:51:39.296235 wagtail_fedit-1.5.4rc1/wagtail_fedit/templatetags/
+-rw-rw-rw-   0        0        0        0 2024-03-29 20:13:42.000000 wagtail_fedit-1.5.4rc1/wagtail_fedit/templatetags/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-23 15:51:39.300619 wagtail_fedit-1.5.4rc1/wagtail_fedit/templatetags/__pycache__/
+-rw-rw-rw-   0        0        0      217 2024-03-29 21:05:00.000000 wagtail_fedit-1.5.4rc1/wagtail_fedit/templatetags/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0    12420 2024-04-23 15:25:11.000000 wagtail_fedit-1.5.4rc1/wagtail_fedit/templatetags/__pycache__/fedit.cpython-311.pyc
+-rw-rw-rw-   0        0        0     9470 2024-04-23 15:25:09.000000 wagtail_fedit-1.5.4rc1/wagtail_fedit/templatetags/fedit.py
+drwxrwxrwx   0        0        0        0 2024-04-23 15:51:39.303620 wagtail_fedit-1.5.4rc1/wagtail_fedit/test/
+-rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.4rc1/wagtail_fedit/test/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-23 15:51:39.347894 wagtail_fedit-1.5.4rc1/wagtail_fedit/test/core/
+-rw-rw-rw-   0        0        0      151 2024-04-05 07:59:49.000000 wagtail_fedit-1.5.4rc1/wagtail_fedit/test/core/__init__.py
+-rw-rw-rw-   0        0        0      165 2024-04-05 08:41:40.000000 wagtail_fedit-1.5.4rc1/wagtail_fedit/test/core/apps.py
+-rw-rw-rw-   0        0        0      130 2024-04-15 20:12:38.000000 wagtail_fedit-1.5.4rc1/wagtail_fedit/test/core/context_processors.py
+drwxrwxrwx   0        0        0        0 2024-04-23 15:51:39.357982 wagtail_fedit-1.5.4rc1/wagtail_fedit/test/core/migrations/
+-rw-rw-rw-   0        0        0    12115 2024-04-20 22:33:35.000000 wagtail_fedit-1.5.4rc1/wagtail_fedit/test/core/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0      509 2024-04-21 18:41:55.000000 wagtail_fedit-1.5.4rc1/wagtail_fedit/test/core/migrations/0002_basicmodel_related_field.py
+-rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.4rc1/wagtail_fedit/test/core/migrations/__init__.py
+-rw-rw-rw-   0        0        0     6047 2024-04-23 13:09:46.000000 wagtail_fedit-1.5.4rc1/wagtail_fedit/test/core/models.py
+drwxrwxrwx   0        0        0        0 2024-04-23 15:51:39.483516 wagtail_fedit-1.5.4rc1/wagtail_fedit/test/core/tests/
+-rw-rw-rw-   0        0        0        0 2024-04-05 07:59:29.000000 wagtail_fedit-1.5.4rc1/wagtail_fedit/test/core/tests/__init__.py
+-rw-rw-rw-   0        0        0     8475 2024-04-23 13:35:29.000000 wagtail_fedit-1.5.4rc1/wagtail_fedit/test/core/tests/base.py
+-rw-rw-rw-   0        0        0    22637 2024-04-23 12:36:52.000000 wagtail_fedit-1.5.4rc1/wagtail_fedit/test/core/tests/test_adapters.py
+-rw-rw-rw-   0        0        0     4320 2024-04-06 22:44:26.000000 wagtail_fedit-1.5.4rc1/wagtail_fedit/test/core/tests/test_block_edit.py
+-rw-rw-rw-   0        0        0     5664 2024-04-05 10:31:29.000000 wagtail_fedit-1.5.4rc1/wagtail_fedit/test/core/tests/test_blocks.py
+-rw-rw-rw-   0        0        0     3642 2024-04-05 18:00:23.000000 wagtail_fedit-1.5.4rc1/wagtail_fedit/test/core/tests/test_field_edit.py
+-rw-rw-rw-   0        0        0     3709 2024-04-10 13:03:30.000000 wagtail_fedit-1.5.4rc1/wagtail_fedit/test/core/tests/test_generic.py
+-rw-rw-rw-   0        0        0     4865 2024-04-23 14:23:09.000000 wagtail_fedit-1.5.4rc1/wagtail_fedit/test/core/tests/test_model_edit.py
+-rw-rw-rw-   0        0        0     1574 2024-04-20 20:49:12.000000 wagtail_fedit-1.5.4rc1/wagtail_fedit/test/core/tests/test_revision.py
+-rw-rw-rw-   0        0        0     9545 2024-04-20 21:54:40.000000 wagtail_fedit-1.5.4rc1/wagtail_fedit/test/core/tests/test_submit.py
+-rw-rw-rw-   0        0        0      704 2024-04-05 17:55:36.000000 wagtail_fedit-1.5.4rc1/wagtail_fedit/test/manage.py
+drwxrwxrwx   0        0        0        0 2024-04-23 15:51:39.489126 wagtail_fedit-1.5.4rc1/wagtail_fedit/test/testapp/
+-rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.4rc1/wagtail_fedit/test/testapp/__init__.py
+-rw-rw-rw-   0        0        0      407 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.4rc1/wagtail_fedit/test/testapp/asgi.py
+-rw-rw-rw-   0        0        0     3625 2024-04-15 20:14:41.000000 wagtail_fedit-1.5.4rc1/wagtail_fedit/test/testapp/settings.py
+-rw-rw-rw-   0        0        0      897 2024-04-05 08:04:53.000000 wagtail_fedit-1.5.4rc1/wagtail_fedit/test/testapp/urls.py
+-rw-rw-rw-   0        0        0      407 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.4rc1/wagtail_fedit/test/testapp/wsgi.py
+-rw-rw-rw-   0        0        0     2220 2024-04-23 14:21:34.000000 wagtail_fedit-1.5.4rc1/wagtail_fedit/toolbar.py
+-rw-rw-rw-   0        0        0      934 2024-04-21 16:55:23.000000 wagtail_fedit-1.5.4rc1/wagtail_fedit/urls.py
+-rw-rw-rw-   0        0        0    17111 2024-04-23 15:38:05.000000 wagtail_fedit-1.5.4rc1/wagtail_fedit/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-23 15:51:39.517713 wagtail_fedit-1.5.4rc1/wagtail_fedit/views/
+-rw-rw-rw-   0        0        0      190 2024-04-13 19:36:44.000000 wagtail_fedit-1.5.4rc1/wagtail_fedit/views/__init__.py
+-rw-rw-rw-   0        0        0     7220 2024-04-23 13:39:08.000000 wagtail_fedit-1.5.4rc1/wagtail_fedit/views/adapters.py
+-rw-rw-rw-   0        0        0    17563 2024-04-21 20:25:17.000000 wagtail_fedit-1.5.4rc1/wagtail_fedit/views/editable.py
+-rw-rw-rw-   0        0        0     1923 2024-04-21 20:29:01.000000 wagtail_fedit-1.5.4rc1/wagtail_fedit/views/mixins.py
+drwxrwxrwx   0        0        0        0 2024-04-23 15:51:39.531937 wagtail_fedit-1.5.4rc1/wagtail_fedit/wagtail_hooks/
+-rw-rw-rw-   0        0        0      184 2024-04-16 10:03:02.000000 wagtail_fedit-1.5.4rc1/wagtail_fedit/wagtail_hooks/__init__.py
+-rw-rw-rw-   0        0        0     1748 2024-04-06 18:37:13.000000 wagtail_fedit-1.5.4rc1/wagtail_fedit/wagtail_hooks/action_menu.py
+-rw-rw-rw-   0        0        0     2668 2024-04-23 14:52:44.000000 wagtail_fedit-1.5.4rc1/wagtail_fedit/wagtail_hooks/adapter_hooks.py
+-rw-rw-rw-   0        0        0      328 2024-04-21 16:44:33.000000 wagtail_fedit-1.5.4rc1/wagtail_fedit/wagtail_hooks/adapter_registry.py
+-rw-rw-rw-   0        0        0      398 2024-04-11 09:03:10.000000 wagtail_fedit-1.5.4rc1/wagtail_fedit/wagtail_hooks/icons.py
+-rw-rw-rw-   0        0        0     2573 2024-04-11 07:39:50.000000 wagtail_fedit-1.5.4rc1/wagtail_fedit/wagtail_hooks/log_actions.py
+-rw-rw-rw-   0        0        0      340 2024-03-30 17:10:05.000000 wagtail_fedit-1.5.4rc1/wagtail_fedit/wagtail_hooks/urls.py
+-rw-rw-rw-   0        0        0     7630 2024-04-19 20:11:56.000000 wagtail_fedit-1.5.4rc1/wagtail_fedit/wagtail_hooks/userbar.py
+drwxrwxrwx   0        0        0        0 2024-04-23 15:51:38.823541 wagtail_fedit-1.5.4rc1/wagtail_fedit.egg-info/
+-rw-rw-rw-   0        0        0    21651 2024-04-23 15:51:38.000000 wagtail_fedit-1.5.4rc1/wagtail_fedit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     4521 2024-04-23 15:51:38.000000 wagtail_fedit-1.5.4rc1/wagtail_fedit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-23 15:51:38.000000 wagtail_fedit-1.5.4rc1/wagtail_fedit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       25 2024-04-23 15:51:38.000000 wagtail_fedit-1.5.4rc1/wagtail_fedit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-04-23 15:51:38.000000 wagtail_fedit-1.5.4rc1/wagtail_fedit.egg-info/top_level.txt
```

### Comparing `wagtail_fedit-1.5.3rc9/LICENSE` & `wagtail_fedit-1.5.4rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc9/PKG-INFO` & `wagtail_fedit-1.5.4rc1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wagtail_fedit
-Version: 1.5.3rc9
+Version: 1.5.4rc1
 Summary: Frontend editing for your Wagtail site
 Home-page: https://github.com/Nigel2392/wagtail_fedit
 Author: Nigel
 Author-email: nigel@goodadvice.it
 License: GPL-2.0-only
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
@@ -57,14 +57,15 @@
   - [Register CSS](#wagtail_feditregister_css)
   - [Register JS](#wagtail_feditregister_js)
   - [Field Editor Size](#wagtail_feditfield_editor_size)
 - [Settings](#settings)
   - [Sign Shared Context](#wagtail_fedit_sign_shared_context)
   - [Share With Sessions](#wagtail_fedit_share_with_sessions)
   - [Use Adapter Session ID](#wagtail_fedit_use_adapter_session_id)
+  - [Track Locales](#wagtail_fedit_track_locales)
 - [How your content is rendered](#how-your-content-is-rendered)
   - [Rendered output HTML](#rendered-editable-output-html)
 - [Implemented](#implemented)
 
 Getting Started
 ---------------
 
@@ -303,52 +304,49 @@
 Adapters can be defined anywhere; we recommend a separate `adapters.py` file.
 
 Adapter instances also have access to the following variables:
 
 * `self.object` - The model instance.
 * `self.field_name` - The field name.
 * `self.meta_field` - The models.Field instance.
-* `self.field_value` - The field value (Retrieved with `self.meta_field.value_from_object(self.object)`)
+* `self.field_value` - The field value (Retrieved with `getattr(self.object, self.field_name)`).
 * `self.request` - The django HTTP request object.
 * `self.kwargs` - Any shared context / keyword arguments for this adapter.
 
 ```python
 # myapp/adapters.py
 
 from wagtail_fedit.adapters import (
     BaseFieldFuncAdapter,
     VARIABLES,
 )
 
 class ColorizerAdapter(BaseFieldFuncAdapter):
-    # Required keyword arguments for the template tag are defined by the superclass.
-    # required_kwargs = [
-    #   "target",
-    #   "name", # the function name, override in __init__ method.
-    # ]
-
-    # Optional kwargs are used to inform inside of the adapter_help command.
-    # They are only for developer convenience.
-    # optional_kwargs = []
+    # Keywords for the adapter can easily be defined.
+    # These will be used to inform the templatetag on what is nescessary, required and counts as a flag.
+    keywords = (
+        Keyword(
+            "target",
+            help_text="The target element to apply the background-image to - this should be a css selector.",
+            type_hint="str",  # Type hint for the `adapter_help` command.
+            # optional=False, # Required is the default.
+            # absolute=False, # Counts as a keyword argument key=value instead of a boolean flag.
+            # default=None,   # Default value if not provided, only for optional keyword arguments.
+        ),
+    )
 
     # How the adapter will be adressed inside of the template tag.
     identifier = "colorizer"
 
+    # The function to call in javascript.
+    js_function = "myColorizerJavascriptFunction"
+
     # A simple description of what this adapter does.
     usage_description = "Change the color of the text for the given target element."
 
-    # Optional explanation of keyword arguments
-    help_text_dict = {
-        "target": "The target element to apply the color to.",
-    }
-
-    def __init__(self, object, field_name: str, request: HttpRequest, **kwargs):
-        kwargs["name"] = "myColorizerJavascriptFunction"
-        super().__init__(object, field_name, request, **kwargs)
-
     def render_content(self, parent_context=None):
         # This is not required; we will replace a CSS variable; thus we are not returning any actual content.
         return ""
   
     def get_response_data(self, parent_context=None):
         """
         Return the data to be sent to the frontend adapter.
@@ -591,14 +589,26 @@
 Default: `True`
 
 Use the get_element_id method of the adapter to generate a session ID.
 *This could __maybe__ interfere with other editable- block's session data, but is highly unlikely!*
 This is useful to not clutter session data too much.
 If `False`, the session ID will be generated each time the page is loaded.
 
+### `WAGTAIL_FEDIT_TRACK_LOCALES`
+
+Default: `False`
+
+Track the locales of the users across the views.
+
+**This sets the initial request.LANGUAGE_CODE (if available) in the shared context.**
+
+If this is false, there is no guarantee that the language of a saved field/model
+will be the same as it initially was, generally it will be - however this might mess up with Wagtail's `Page.locale` and
+the page not being available in the context afterwards.
+
 ## How your content is rendered
 
 (**Maintainer's note:** In my experience this doesn't mess the CSS up too much, or even at all for most content - **if** you don't get hyperspecific with your CSS selectors and structure your templates well.)
 
 Your block and field are wrapped in a `div`, any CSS for your templates should keep this in mind.
 
 ### Rendered editable output HTML
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: wagtail_fedit Version: 1.5.3rc9 Summary: Frontend
+Metadata-Version: 2.1 Name: wagtail_fedit Version: 1.5.4rc1 Summary: Frontend
 editing for your Wagtail site Home-page: https://github.com/Nigel2392/
 wagtail_fedit Author: Nigel Author-email: nigel@goodadvice.it License: GPL-2.0-
 only Classifier: Environment :: Web Environment Classifier: Framework :: Django
 Classifier: Framework :: Django :: 4.2 Classifier: Framework :: Wagtail
 Classifier: Framework :: Wagtail :: 5 Classifier: Framework :: Wagtail :: 6
 Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
 :: GNU General Public License v2 or later (GPLv2+) Classifier: Operating System
@@ -28,17 +28,18 @@
 (#wagtail_feditregister_field_widgets) - [Exclude Related Forms]
 (#wagtail_feditexclude_related_forms) - [Action Menu Item Is Shown]
 (#wagtail_feditaction_menu_item_is_shown) - [Register CSS]
 (#wagtail_feditregister_css) - [Register JS](#wagtail_feditregister_js) -
 [Field Editor Size](#wagtail_feditfield_editor_size) - [Settings](#settings) -
 [Sign Shared Context](#wagtail_fedit_sign_shared_context) - [Share With
 Sessions](#wagtail_fedit_share_with_sessions) - [Use Adapter Session ID]
-(#wagtail_fedit_use_adapter_session_id) - [How your content is rendered](#how-
-your-content-is-rendered) - [Rendered output HTML](#rendered-editable-output-
-html) - [Implemented](#implemented) Getting Started --------------- 1. Add
+(#wagtail_fedit_use_adapter_session_id) - [Track Locales]
+(#wagtail_fedit_track_locales) - [How your content is rendered](#how-your-
+content-is-rendered) - [Rendered output HTML](#rendered-editable-output-html) -
+[Implemented](#implemented) Getting Started --------------- 1. Add
 'wagtail_fedit' to your INSTALLED_APPS setting like this: ``` INSTALLED_APPS =
 [ ..., 'wagtail_fedit', ] ``` 2. Run `py ./manage.py collectstatic`. 3. Run `py
 ./manage.py adapter_help` to see all your options and their requirements. ##
 Getting Editing! 1. If you want to get into the frontend-editing interface for
 a model it must inherit from `PreviewableMixin`. **This is a requirement.** It
 is however not always required for your model to inherit from
 `PreviewableMixin`. **Any model can be edited**; you just can't access the
@@ -136,53 +137,53 @@
 colorizer page.color target=".my-colorized-div" %}
 ************ CCoolloorriizzeedd TTeexxtt!! ************
 ... ``` ### Adapters Python We will get started creating the adapter
 definition. Adapters can be defined anywhere; we recommend a separate
 `adapters.py` file. Adapter instances also have access to the following
 variables: * `self.object` - The model instance. * `self.field_name` - The
 field name. * `self.meta_field` - The models.Field instance. *
-`self.field_value` - The field value (Retrieved with
-`self.meta_field.value_from_object(self.object)`) * `self.request` - The django
-HTTP request object. * `self.kwargs` - Any shared context / keyword arguments
-for this adapter. ```python # myapp/adapters.py from wagtail_fedit.adapters
-import ( BaseFieldFuncAdapter, VARIABLES, ) class ColorizerAdapter
-(BaseFieldFuncAdapter): # Required keyword arguments for the template tag are
-defined by the superclass. # required_kwargs = [ # "target", # "name", # the
-function name, override in __init__ method. # ] # Optional kwargs are used to
-inform inside of the adapter_help command. # They are only for developer
-convenience. # optional_kwargs = [] # How the adapter will be adressed inside
-of the template tag. identifier = "colorizer" # A simple description of what
-this adapter does. usage_description = "Change the color of the text for the
-given target element." # Optional explanation of keyword arguments
-help_text_dict = { "target": "The target element to apply the color to.", } def
-__init__(self, object, field_name: str, request: HttpRequest, **kwargs): kwargs
-["name"] = "myColorizerJavascriptFunction" super().__init__(object, field_name,
-request, **kwargs) def render_content(self, parent_context=None): # This is not
-required; we will replace a CSS variable; thus we are not returning any actual
-content. return "" def get_response_data(self, parent_context=None): """ Return
-the data to be sent to the frontend adapter. """ data = super
-().get_response_data(parent_context) return data | { "color": self.field_value,
-} def get_form_attrs(self) -> dict: """ Return form attributes for the form
-inside of the edit modal. This can be used to control editor size. """ attrs =
-super().get_form_attrs() attrs[VARIABLES.FORM_SIZE_VAR] = "full" # Fullscreen,
-there is also `large`. return attrs ``` We must then register the adapter to
-make sure it is available for templates. This should be done in a
+`self.field_value` - The field value (Retrieved with `getattr(self.object,
+self.field_name)`). * `self.request` - The django HTTP request object. *
+`self.kwargs` - Any shared context / keyword arguments for this adapter.
+```python # myapp/adapters.py from wagtail_fedit.adapters import
+( BaseFieldFuncAdapter, VARIABLES, ) class ColorizerAdapter
+(BaseFieldFuncAdapter): # Keywords for the adapter can easily be defined. #
+These will be used to inform the templatetag on what is nescessary, required
+and counts as a flag. keywords = ( Keyword( "target", help_text="The target
+element to apply the background-image to - this should be a css selector.",
+type_hint="str", # Type hint for the `adapter_help` command. # optional=False,
+# Required is the default. # absolute=False, # Counts as a keyword argument
+key=value instead of a boolean flag. # default=None, # Default value if not
+provided, only for optional keyword arguments. ), ) # How the adapter will be
+adressed inside of the template tag. identifier = "colorizer" # The function to
+call in javascript. js_function = "myColorizerJavascriptFunction" # A simple
+description of what this adapter does. usage_description = "Change the color of
+the text for the given target element." def render_content(self,
+parent_context=None): # This is not required; we will replace a CSS variable;
+thus we are not returning any actual content. return "" def get_response_data
+(self, parent_context=None): """ Return the data to be sent to the frontend
+adapter. """ data = super().get_response_data(parent_context) return data |
+{ "color": self.field_value, } def get_form_attrs(self) -> dict: """ Return
+form attributes for the form inside of the edit modal. This can be used to
+control editor size. """ attrs = super().get_form_attrs() attrs
+[VARIABLES.FORM_SIZE_VAR] = "full" # Fullscreen, there is also `large`. return
+attrs ``` We must then register the adapter to make sure it is available for
+templates. This should be done in a `wagtail_hooks.py` file. ```python # myapp/
+wagtail_hooks.py from wagtail_fedit.adapters import adapter_registry from
+myapp.adapters import ColorizerAdapter adapter_registry.register
+(ColorizerAdapter) ``` ### Adapters Javascript We now need to create the
+javascript function to actually apply the color to the styles of the element.
+This function will be called `myColorizerJavascriptFunction`, as defined in the
+adapter's `__init__` method. ```javascript // myapp/static/myapp/js/custom.js
+function myColorizerJavascriptFunction(element, response) { element.style.color
+= response.color; } ``` We must then register this javascript file to be
+included in the frontend editing interface. This should be done in a
 `wagtail_hooks.py` file. ```python # myapp/wagtail_hooks.py from
-wagtail_fedit.adapters import adapter_registry from myapp.adapters import
-ColorizerAdapter adapter_registry.register(ColorizerAdapter) ``` ### Adapters
-Javascript We now need to create the javascript function to actually apply the
-color to the styles of the element. This function will be called
-`myColorizerJavascriptFunction`, as defined in the adapter's `__init__` method.
-```javascript // myapp/static/myapp/js/custom.js function
-myColorizerJavascriptFunction(element, response) { element.style.color =
-response.color; } ``` We must then register this javascript file to be included
-in the frontend editing interface. This should be done in a `wagtail_hooks.py`
-file. ```python # myapp/wagtail_hooks.py from django.utils.html import
-format_html from django.templatetags.static import static from
-wagtail_fedit.hooks import REGISTER_JS from wagtail import hooks
+django.utils.html import format_html from django.templatetags.static import
+static from wagtail_fedit.hooks import REGISTER_JS from wagtail import hooks
 @hooks.register(REGISTER_JS) def register_js(request): return [ format_html( '
 ', static('myapp/js/custom.js') ), ] ``` ## Hooks ###
 wagtail_fedit.construct_adapter_toolbar Construct the toolbar for the given
 adapter. This is used to display the edit icon for the given adapter. How it is
 called: ```python items = [ FeditAdapterEditButton(), ] for hook in
 hooks.get_hooks(CONSTRUCT_ADAPTER_TOOLBAR): hook(items=items, adapter=adapter)
 ``` ### wagtail_fedit.register_type_renderer Register a custom renderer for a
@@ -237,20 +238,26 @@
 Default: `False` Share the context through the session data. This is useful if
 you are running into limits with the URL length. This will store the context in
 the session and pass the session key to the iFrame instead of the context. ###
 `WAGTAIL_FEDIT_USE_ADAPTER_SESSION_ID` Default: `True` Use the get_element_id
 method of the adapter to generate a session ID. *This could __maybe__ interfere
 with other editable- block's session data, but is highly unlikely!* This is
 useful to not clutter session data too much. If `False`, the session ID will be
-generated each time the page is loaded. ## How your content is rendered
-(**Maintainer's note:** In my experience this doesn't mess the CSS up too much,
-or even at all for most content - **if** you don't get hyperspecific with your
-CSS selectors and structure your templates well.) Your block and field are
-wrapped in a `div`, any CSS for your templates should keep this in mind. ###
-Rendered editable output HTML ```html {% load fedit %}
+generated each time the page is loaded. ### `WAGTAIL_FEDIT_TRACK_LOCALES`
+Default: `False` Track the locales of the users across the views. **This sets
+the initial request.LANGUAGE_CODE (if available) in the shared context.** If
+this is false, there is no guarantee that the language of a saved field/model
+will be the same as it initially was, generally it will be - however this might
+mess up with Wagtail's `Page.locale` and the page not being available in the
+context afterwards. ## How your content is rendered (**Maintainer's note:** In
+my experience this doesn't mess the CSS up too much, or even at all for most
+content - **if** you don't get hyperspecific with your CSS selectors and
+structure your templates well.) Your block and field are wrapped in a `div`,
+any CSS for your templates should keep this in mind. ### Rendered editable
+output HTML ```html {% load fedit %}
 % if shared %} data-shared-context="{{ shared }}"{%endif%} data-edit-url="{
 { edit_url }}">
 {% for button in buttons %} {{ button }} {% endfor %}
 {% render_adapter adapter %}
 ``` ## Implemented * Revision Support * Locked Support * Draft Support *
 Preview Support * Workflow Support * Permissions * Audit Logs * Full block
 capabilities on Frontend Editing
```

### Comparing `wagtail_fedit-1.5.3rc9/README.md` & `wagtail_fedit-1.5.4rc1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -27,14 +27,15 @@
   - [Register CSS](#wagtail_feditregister_css)
   - [Register JS](#wagtail_feditregister_js)
   - [Field Editor Size](#wagtail_feditfield_editor_size)
 - [Settings](#settings)
   - [Sign Shared Context](#wagtail_fedit_sign_shared_context)
   - [Share With Sessions](#wagtail_fedit_share_with_sessions)
   - [Use Adapter Session ID](#wagtail_fedit_use_adapter_session_id)
+  - [Track Locales](#wagtail_fedit_track_locales)
 - [How your content is rendered](#how-your-content-is-rendered)
   - [Rendered output HTML](#rendered-editable-output-html)
 - [Implemented](#implemented)
 
 Getting Started
 ---------------
 
@@ -273,52 +274,49 @@
 Adapters can be defined anywhere; we recommend a separate `adapters.py` file.
 
 Adapter instances also have access to the following variables:
 
 * `self.object` - The model instance.
 * `self.field_name` - The field name.
 * `self.meta_field` - The models.Field instance.
-* `self.field_value` - The field value (Retrieved with `self.meta_field.value_from_object(self.object)`)
+* `self.field_value` - The field value (Retrieved with `getattr(self.object, self.field_name)`).
 * `self.request` - The django HTTP request object.
 * `self.kwargs` - Any shared context / keyword arguments for this adapter.
 
 ```python
 # myapp/adapters.py
 
 from wagtail_fedit.adapters import (
     BaseFieldFuncAdapter,
     VARIABLES,
 )
 
 class ColorizerAdapter(BaseFieldFuncAdapter):
-    # Required keyword arguments for the template tag are defined by the superclass.
-    # required_kwargs = [
-    #   "target",
-    #   "name", # the function name, override in __init__ method.
-    # ]
-
-    # Optional kwargs are used to inform inside of the adapter_help command.
-    # They are only for developer convenience.
-    # optional_kwargs = []
+    # Keywords for the adapter can easily be defined.
+    # These will be used to inform the templatetag on what is nescessary, required and counts as a flag.
+    keywords = (
+        Keyword(
+            "target",
+            help_text="The target element to apply the background-image to - this should be a css selector.",
+            type_hint="str",  # Type hint for the `adapter_help` command.
+            # optional=False, # Required is the default.
+            # absolute=False, # Counts as a keyword argument key=value instead of a boolean flag.
+            # default=None,   # Default value if not provided, only for optional keyword arguments.
+        ),
+    )
 
     # How the adapter will be adressed inside of the template tag.
     identifier = "colorizer"
 
+    # The function to call in javascript.
+    js_function = "myColorizerJavascriptFunction"
+
     # A simple description of what this adapter does.
     usage_description = "Change the color of the text for the given target element."
 
-    # Optional explanation of keyword arguments
-    help_text_dict = {
-        "target": "The target element to apply the color to.",
-    }
-
-    def __init__(self, object, field_name: str, request: HttpRequest, **kwargs):
-        kwargs["name"] = "myColorizerJavascriptFunction"
-        super().__init__(object, field_name, request, **kwargs)
-
     def render_content(self, parent_context=None):
         # This is not required; we will replace a CSS variable; thus we are not returning any actual content.
         return ""
   
     def get_response_data(self, parent_context=None):
         """
         Return the data to be sent to the frontend adapter.
@@ -561,14 +559,26 @@
 Default: `True`
 
 Use the get_element_id method of the adapter to generate a session ID.
 *This could __maybe__ interfere with other editable- block's session data, but is highly unlikely!*
 This is useful to not clutter session data too much.
 If `False`, the session ID will be generated each time the page is loaded.
 
+### `WAGTAIL_FEDIT_TRACK_LOCALES`
+
+Default: `False`
+
+Track the locales of the users across the views.
+
+**This sets the initial request.LANGUAGE_CODE (if available) in the shared context.**
+
+If this is false, there is no guarantee that the language of a saved field/model
+will be the same as it initially was, generally it will be - however this might mess up with Wagtail's `Page.locale` and
+the page not being available in the context afterwards.
+
 ## How your content is rendered
 
 (**Maintainer's note:** In my experience this doesn't mess the CSS up too much, or even at all for most content - **if** you don't get hyperspecific with your CSS selectors and structure your templates well.)
 
 Your block and field are wrapped in a `div`, any CSS for your templates should keep this in mind.
 
 ### Rendered editable output HTML
```

#### html2text {}

```diff
@@ -13,17 +13,18 @@
 (#wagtail_feditregister_field_widgets) - [Exclude Related Forms]
 (#wagtail_feditexclude_related_forms) - [Action Menu Item Is Shown]
 (#wagtail_feditaction_menu_item_is_shown) - [Register CSS]
 (#wagtail_feditregister_css) - [Register JS](#wagtail_feditregister_js) -
 [Field Editor Size](#wagtail_feditfield_editor_size) - [Settings](#settings) -
 [Sign Shared Context](#wagtail_fedit_sign_shared_context) - [Share With
 Sessions](#wagtail_fedit_share_with_sessions) - [Use Adapter Session ID]
-(#wagtail_fedit_use_adapter_session_id) - [How your content is rendered](#how-
-your-content-is-rendered) - [Rendered output HTML](#rendered-editable-output-
-html) - [Implemented](#implemented) Getting Started --------------- 1. Add
+(#wagtail_fedit_use_adapter_session_id) - [Track Locales]
+(#wagtail_fedit_track_locales) - [How your content is rendered](#how-your-
+content-is-rendered) - [Rendered output HTML](#rendered-editable-output-html) -
+[Implemented](#implemented) Getting Started --------------- 1. Add
 'wagtail_fedit' to your INSTALLED_APPS setting like this: ``` INSTALLED_APPS =
 [ ..., 'wagtail_fedit', ] ``` 2. Run `py ./manage.py collectstatic`. 3. Run `py
 ./manage.py adapter_help` to see all your options and their requirements. ##
 Getting Editing! 1. If you want to get into the frontend-editing interface for
 a model it must inherit from `PreviewableMixin`. **This is a requirement.** It
 is however not always required for your model to inherit from
 `PreviewableMixin`. **Any model can be edited**; you just can't access the
@@ -121,53 +122,53 @@
 colorizer page.color target=".my-colorized-div" %}
 ************ CCoolloorriizzeedd TTeexxtt!! ************
 ... ``` ### Adapters Python We will get started creating the adapter
 definition. Adapters can be defined anywhere; we recommend a separate
 `adapters.py` file. Adapter instances also have access to the following
 variables: * `self.object` - The model instance. * `self.field_name` - The
 field name. * `self.meta_field` - The models.Field instance. *
-`self.field_value` - The field value (Retrieved with
-`self.meta_field.value_from_object(self.object)`) * `self.request` - The django
-HTTP request object. * `self.kwargs` - Any shared context / keyword arguments
-for this adapter. ```python # myapp/adapters.py from wagtail_fedit.adapters
-import ( BaseFieldFuncAdapter, VARIABLES, ) class ColorizerAdapter
-(BaseFieldFuncAdapter): # Required keyword arguments for the template tag are
-defined by the superclass. # required_kwargs = [ # "target", # "name", # the
-function name, override in __init__ method. # ] # Optional kwargs are used to
-inform inside of the adapter_help command. # They are only for developer
-convenience. # optional_kwargs = [] # How the adapter will be adressed inside
-of the template tag. identifier = "colorizer" # A simple description of what
-this adapter does. usage_description = "Change the color of the text for the
-given target element." # Optional explanation of keyword arguments
-help_text_dict = { "target": "The target element to apply the color to.", } def
-__init__(self, object, field_name: str, request: HttpRequest, **kwargs): kwargs
-["name"] = "myColorizerJavascriptFunction" super().__init__(object, field_name,
-request, **kwargs) def render_content(self, parent_context=None): # This is not
-required; we will replace a CSS variable; thus we are not returning any actual
-content. return "" def get_response_data(self, parent_context=None): """ Return
-the data to be sent to the frontend adapter. """ data = super
-().get_response_data(parent_context) return data | { "color": self.field_value,
-} def get_form_attrs(self) -> dict: """ Return form attributes for the form
-inside of the edit modal. This can be used to control editor size. """ attrs =
-super().get_form_attrs() attrs[VARIABLES.FORM_SIZE_VAR] = "full" # Fullscreen,
-there is also `large`. return attrs ``` We must then register the adapter to
-make sure it is available for templates. This should be done in a
+`self.field_value` - The field value (Retrieved with `getattr(self.object,
+self.field_name)`). * `self.request` - The django HTTP request object. *
+`self.kwargs` - Any shared context / keyword arguments for this adapter.
+```python # myapp/adapters.py from wagtail_fedit.adapters import
+( BaseFieldFuncAdapter, VARIABLES, ) class ColorizerAdapter
+(BaseFieldFuncAdapter): # Keywords for the adapter can easily be defined. #
+These will be used to inform the templatetag on what is nescessary, required
+and counts as a flag. keywords = ( Keyword( "target", help_text="The target
+element to apply the background-image to - this should be a css selector.",
+type_hint="str", # Type hint for the `adapter_help` command. # optional=False,
+# Required is the default. # absolute=False, # Counts as a keyword argument
+key=value instead of a boolean flag. # default=None, # Default value if not
+provided, only for optional keyword arguments. ), ) # How the adapter will be
+adressed inside of the template tag. identifier = "colorizer" # The function to
+call in javascript. js_function = "myColorizerJavascriptFunction" # A simple
+description of what this adapter does. usage_description = "Change the color of
+the text for the given target element." def render_content(self,
+parent_context=None): # This is not required; we will replace a CSS variable;
+thus we are not returning any actual content. return "" def get_response_data
+(self, parent_context=None): """ Return the data to be sent to the frontend
+adapter. """ data = super().get_response_data(parent_context) return data |
+{ "color": self.field_value, } def get_form_attrs(self) -> dict: """ Return
+form attributes for the form inside of the edit modal. This can be used to
+control editor size. """ attrs = super().get_form_attrs() attrs
+[VARIABLES.FORM_SIZE_VAR] = "full" # Fullscreen, there is also `large`. return
+attrs ``` We must then register the adapter to make sure it is available for
+templates. This should be done in a `wagtail_hooks.py` file. ```python # myapp/
+wagtail_hooks.py from wagtail_fedit.adapters import adapter_registry from
+myapp.adapters import ColorizerAdapter adapter_registry.register
+(ColorizerAdapter) ``` ### Adapters Javascript We now need to create the
+javascript function to actually apply the color to the styles of the element.
+This function will be called `myColorizerJavascriptFunction`, as defined in the
+adapter's `__init__` method. ```javascript // myapp/static/myapp/js/custom.js
+function myColorizerJavascriptFunction(element, response) { element.style.color
+= response.color; } ``` We must then register this javascript file to be
+included in the frontend editing interface. This should be done in a
 `wagtail_hooks.py` file. ```python # myapp/wagtail_hooks.py from
-wagtail_fedit.adapters import adapter_registry from myapp.adapters import
-ColorizerAdapter adapter_registry.register(ColorizerAdapter) ``` ### Adapters
-Javascript We now need to create the javascript function to actually apply the
-color to the styles of the element. This function will be called
-`myColorizerJavascriptFunction`, as defined in the adapter's `__init__` method.
-```javascript // myapp/static/myapp/js/custom.js function
-myColorizerJavascriptFunction(element, response) { element.style.color =
-response.color; } ``` We must then register this javascript file to be included
-in the frontend editing interface. This should be done in a `wagtail_hooks.py`
-file. ```python # myapp/wagtail_hooks.py from django.utils.html import
-format_html from django.templatetags.static import static from
-wagtail_fedit.hooks import REGISTER_JS from wagtail import hooks
+django.utils.html import format_html from django.templatetags.static import
+static from wagtail_fedit.hooks import REGISTER_JS from wagtail import hooks
 @hooks.register(REGISTER_JS) def register_js(request): return [ format_html( '
 ', static('myapp/js/custom.js') ), ] ``` ## Hooks ###
 wagtail_fedit.construct_adapter_toolbar Construct the toolbar for the given
 adapter. This is used to display the edit icon for the given adapter. How it is
 called: ```python items = [ FeditAdapterEditButton(), ] for hook in
 hooks.get_hooks(CONSTRUCT_ADAPTER_TOOLBAR): hook(items=items, adapter=adapter)
 ``` ### wagtail_fedit.register_type_renderer Register a custom renderer for a
@@ -222,20 +223,26 @@
 Default: `False` Share the context through the session data. This is useful if
 you are running into limits with the URL length. This will store the context in
 the session and pass the session key to the iFrame instead of the context. ###
 `WAGTAIL_FEDIT_USE_ADAPTER_SESSION_ID` Default: `True` Use the get_element_id
 method of the adapter to generate a session ID. *This could __maybe__ interfere
 with other editable- block's session data, but is highly unlikely!* This is
 useful to not clutter session data too much. If `False`, the session ID will be
-generated each time the page is loaded. ## How your content is rendered
-(**Maintainer's note:** In my experience this doesn't mess the CSS up too much,
-or even at all for most content - **if** you don't get hyperspecific with your
-CSS selectors and structure your templates well.) Your block and field are
-wrapped in a `div`, any CSS for your templates should keep this in mind. ###
-Rendered editable output HTML ```html {% load fedit %}
+generated each time the page is loaded. ### `WAGTAIL_FEDIT_TRACK_LOCALES`
+Default: `False` Track the locales of the users across the views. **This sets
+the initial request.LANGUAGE_CODE (if available) in the shared context.** If
+this is false, there is no guarantee that the language of a saved field/model
+will be the same as it initially was, generally it will be - however this might
+mess up with Wagtail's `Page.locale` and the page not being available in the
+context afterwards. ## How your content is rendered (**Maintainer's note:** In
+my experience this doesn't mess the CSS up too much, or even at all for most
+content - **if** you don't get hyperspecific with your CSS selectors and
+structure your templates well.) Your block and field are wrapped in a `div`,
+any CSS for your templates should keep this in mind. ### Rendered editable
+output HTML ```html {% load fedit %}
 % if shared %} data-shared-context="{{ shared }}"{%endif%} data-edit-url="{
 { edit_url }}">
 {% for button in buttons %} {{ button }} {% endfor %}
 {% render_adapter adapter %}
 ``` ## Implemented * Revision Support * Locked Support * Draft Support *
 Preview Support * Workflow Support * Permissions * Audit Logs * Full block
 capabilities on Frontend Editing
```

### Comparing `wagtail_fedit-1.5.3rc9/setup.cfg` & `wagtail_fedit-1.5.4rc1/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2077 6167 7461 696c 5f66 6564 6974   = wagtail_fedit
 00000020: 0d0a 7665 7273 696f 6e20 3d20 312e 352e  ..version = 1.5.
-00000030: 3372 6339 0d0a 6465 7363 7269 7074 696f  3rc9..descriptio
+00000030: 3472 6331 0d0a 6465 7363 7269 7074 696f  4rc1..descriptio
 00000040: 6e20 3d20 4672 6f6e 7465 6e64 2065 6469  n = Frontend edi
 00000050: 7469 6e67 2066 6f72 2079 6f75 7220 5761  ting for your Wa
 00000060: 6774 6169 6c20 7369 7465 0d0a 6c6f 6e67  gtail site..long
 00000070: 5f64 6573 6372 6970 7469 6f6e 203d 2066  _description = f
 00000080: 696c 653a 2052 4541 444d 452e 6d64 0d0a  ile: README.md..
 00000090: 6c6f 6e67 5f64 6573 6372 6970 7469 6f6e  long_description
 000000a0: 5f63 6f6e 7465 6e74 5f74 7970 6520 3d20  _content_type =
```

### Comparing `wagtail_fedit-1.5.3rc9/wagtail_fedit/adapters/base.py` & `wagtail_fedit-1.5.4rc1/wagtail_fedit/adapters/base.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 from typing import (
-    TYPE_CHECKING, Any,
+    TYPE_CHECKING, Any, Type,
 )
 from django import forms
 from django.db import models
+from django.utils import translation
 from django.utils.translation import gettext_lazy as _
+from django.utils.functional import cached_property
 from django.utils.text import (
     slugify,
 )
 from django.core.signing import (
     Signer,
 )
 from django.http import (
     HttpRequest,
 )
 from ..settings import (
     SIGN_SHARED_CONTEXT,
     SHARE_WITH_SESSIONS,
     USE_ADAPTER_SESSION_ID,
+    TRACK_LOCALES,
 )
 from ..utils import (
     FeditIFrameMixin,
     wrap_adapter,
 )
 
 import uuid
@@ -61,86 +64,181 @@
 
 def Base85_json_dumps(obj):
     return base64.b85encode(json.dumps(obj).encode("utf-8")).decode("utf-8")
 
 def Base85_json_loads(data):
     return json.loads(base64.b85decode(data).decode("utf-8"))
 
-class BaseAdapter(FeditIFrameMixin):
+
+
+class Keyword:
+    def __init__(self, name: str, optional: bool = False, absolute: bool = False, default=None, help_text: str = None, type_hint: Type[Any] = None):
+
+        if (default and absolute) or (default and not optional):
+            raise AdapterError("Keywords cannot be absolute or required and have a default value")
+
+        if optional and absolute:
+            raise AdapterError("Keywords cannot be optional and absolute")
+        
+        if default is not None and not type_hint:
+            type_hint = type(default)
+        
+        self.name = name
+        self.optional = optional
+        self.absolute = absolute
+        self.default = default
+        self.help_text = help_text
+        self.type_hint = type_hint
+
+    def __str__(self):
+        k = []
+
+        if self.optional:
+            k.append("?")
+        if self.absolute:
+            k.append("!")
+
+        k.append(self.name)
+
+        if self.type_hint and not self.absolute:
+            if isinstance(self.type_hint, str):
+                k.append(f": {self.type_hint}")
+            else:
+                k.append(f": {self.type_hint.__name__}")
+                
+        if self.default is not None and not self.absolute:
+            default = self.default
+            if isinstance(default, str):
+                default = f"'{default}'"
+            k.append(f"={default}")
+
+        return "".join(k)
+
+    def __repr__(self):
+        s = ["Keyword", self.name]
+        if self.optional:
+            s.append("optional")
+        elif not self.absolute:
+            s.append("required")
+        if self.absolute:
+            s.append("absolute")
+        if self.default:
+            s.append(f"default={self.default}")
+        if self.help_text:
+            s.append(f"help_text='{self.help_text}'")
+        if self.type_hint:
+            s.append(f"type: {self.type_hint}")
+        s = " ".join(s)
+        return f"<{s}>"
+
+def _get_keywords(bases, attrs):
+    if "keywords" in attrs:
+        return list(attrs["keywords"])
+    
+    for base in bases:
+        if hasattr(base, "keywords"):
+            return list(base.keywords)
+        
+    return list()
+
+def _sort_keywords(keywords):
+    _s = sorted(keywords, key=lambda x: (not x.absolute, x.optional))
+    return _s
+
+class AdapterMeta(type):
+    def __new__(cls, name, bases, attrs):
+        keywords: list[Keyword] = _get_keywords(bases, attrs)
+        required_kwargs = []
+        absolute_tokens = []
+        optional_kwargs = {}
+
+        for keyword in keywords:
+            if keyword.absolute:
+                absolute_tokens.append(keyword.name)
+            elif keyword.optional:
+                if keyword.default is not None:
+                    optional_kwargs[keyword.name] = keyword.default
+                else:
+                    optional_kwargs[keyword.name] = None
+            else:
+                required_kwargs.append(keyword.name)
+
+        cls = super().__new__(cls, name, bases, attrs)
+
+        cls.required_kwargs: tuple[str]     = tuple(required_kwargs)
+        cls.absolute_tokens: tuple[str]     = tuple(absolute_tokens)
+        cls.optional_kwargs: dict[str, Any] = optional_kwargs
+        cls.keywords:        tuple[Keyword] = tuple(
+            _sort_keywords(keywords)
+        )
+
+        return cls
+
+
+class BaseAdapter(FeditIFrameMixin, metaclass=AdapterMeta):
     # How the adapter is identified on inside of the templatetag.
     identifier              = None
 
     # If the templatetag required the first argument to be model.field or just model
     field_required          = True
 
     # The template used to render the form.
     template_name           = "wagtail_fedit/editor/adapter_iframe.html"
 
     signer: Signer          = Signer()
-    # Required keyword arguments for the adapter
-    required_kwargs         = []
-    # Optional keyword arguments for the adapter, these are only used to print the help example.
-    optional_kwargs         = []
-    # Tokens which should be resolved absolutely (no parser.compile_filter)
-    # These are NOT required.
-    absolute_tokens         = [
-        "inline",
-    ]
+    
+    # Keyword arguments for the adapter
+    keywords: tuple[Keyword]     = (
+        Keyword(
+            "inline",
+            absolute=True,
+            help_text="if passed; the adapter will be rendered with inline styles."
+        ),
+    )
+
     # An optional description to be displayed when running the help command.
     usage_description       = "This adapter is used to edit a field of a model instance."
-    # A dictionary of help text for the adapter.
-    help_text_dict          = {}
 
     # The JS constructor for the adapter.
     # This will receive the data after a successful form submission.
     js_constructor          = None
 
     def __init__(self, object: models.Model, field_name: str, request: HttpRequest, **kwargs):
-        self.object         = object
-        self.request        = request
-        self.kwargs         = kwargs
+        self.object           = object
+        self.request          = request
+        self.kwargs           = kwargs
+
+        for k, v in self.optional_kwargs.items():
+            if k not in self.kwargs and v is not None:
+                self.kwargs[k] = v
+
+        if hasattr(request, "LANGUAGE_CODE") and TRACK_LOCALES:
+            if "LANGUAGE_CODE" not in self.kwargs:
+                self.kwargs["LANGUAGE_CODE"] = request.LANGUAGE_CODE
+
+            if self.kwargs["LANGUAGE_CODE"] != request.LANGUAGE_CODE:
+                translation.activate(self.kwargs["LANGUAGE_CODE"])
 
         if self.field_required:
             self.field_name     = field_name
             self.meta_field     = object._meta.get_field(field_name)
         else:
             self.field_name     = None
             self.meta_field     = None
 
     @classmethod
     def get_usage_string(cls) -> str:
         """
         Return a string which describes how to use the adapter.
         """
         s = []
-        for i, token in enumerate(cls.absolute_tokens):
-            s.append(f"{token}")
-            if i < len(cls.absolute_tokens) - 1:
-                s.append(" ")
-        
-        if cls.absolute_tokens and cls.required_kwargs:
-            s.append(" ")
-
-        for i, kwarg in enumerate(cls.required_kwargs):
-            s.append(f"{kwarg}=value")
-            if i < len(cls.required_kwargs) - 1:
-                s.append(" ")
-
-        if (
-            cls.required_kwargs and cls.optional_kwargs or\
-            not cls.required_kwargs and cls.absolute_tokens and cls.optional_kwargs
-        ):
-            s.append(" ")
-        
-        for i, kwarg in enumerate(cls.optional_kwargs):
-            s.append(f"[{kwarg}=value]")
-            if i < len(cls.optional_kwargs) - 1:
-                s.append(" ")
+        for keyword in cls.keywords:
+            s.append(str(keyword))
                 
-        return "".join(s)
+        return " ".join(s)
     
     def get_form_context(self, **kwargs):
         return {
             "adapter": self,
             "field_name": self.field_name,
             "meta_field": self.meta_field,
         }
@@ -154,20 +252,19 @@
     
     @classmethod
     def get_usage_help_text(cls) -> list[str]:
         """
         Return a help text which describes how to use the adapter.
         This might be a good time to exalain the kwargs.
         """
-        if "inline" in cls.absolute_tokens:
-            return {
-                "inline": "if passed; the adapter will be rendered with inline styles.",
-                **cls.help_text_dict,
-            }
-        return cls.help_text_dict
+        d = {}
+        for keyword in cls.keywords:
+            if keyword.name not in d:
+                d[keyword.name] = keyword.help_text
+        return d
     
     def get_template_names(self) -> list[str]:
         """
         Return the template names for the adapter.
         """
         return [self.template_name]
 
@@ -175,21 +272,28 @@
     def field_value(self):
         """
         Call the value_from_object method on
         the meta field to get the value from the instance.
         """
         return getattr(self.object, self.field_name)
     
-    @property
+    @cached_property
     def model(self):
         """
         Return the model class of the object.
         """
         return self.object.__class__
     
+    @cached_property
+    def tooltip(self):
+        """
+        Return the tooltip for the adapter.
+        """
+        return self.get_header_title()
+    
     def check_permissions(self):
         """
         Check if the user has the required permissions to edit the field.
         If false; the field will be rendered as normal (read only).
         """
         if not self.request.user.is_authenticated:
             return False
```

### Comparing `wagtail_fedit-1.5.3rc9/wagtail_fedit/adapters/block.py` & `wagtail_fedit-1.5.4rc1/wagtail_fedit/adapters/block.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 from django.db import models
 from django.utils import translation
 from django.utils.translation import gettext_lazy as _
+from django.utils.functional import cached_property
 from django.http import HttpRequest
 
 from wagtail.log_actions import log
 from wagtail.blocks import (
     StreamValue,
 )
 from wagtail.models import (
     RevisionMixin,
 )
 
 from .base import (
     BlockFieldReplacementAdapter,
     AdapterError,
+    Keyword,
     VARIABLES,
 )
 from ..forms import (
     blocks as block_forms,
 )
 from .. import utils
 from wagtail.admin.admin_url_finder import (
@@ -34,28 +36,29 @@
     """
     An adapter for editing Wagtail blocks.
     This will render the block and replace it on the frontend
     on successful form submission.
     """
     identifier = "block"
     usage_description = "This adapter is used to edit a block of a streamfield."
-    help_text_dict = {
-        "block": "the block instance to edit. This can be a regular block isntance or a BoundBlock.",
-        "block_id": "the ID of the block to edit, required if block is not a BoundBlock.",
-        "admin": "if passed; the adapter will a quick- link to the Wagtail Admin for this block.",
-    }
-    required_kwargs = [
-        "block",
-    ]
-    optional_kwargs = [
-        "block_id",
-    ]
-    absolute_tokens = [ # override; remove "inline"
-        "admin", # allows for displaying admin URLs
-    ]
+    keywords = (
+        Keyword("block",
+            help_text="the block instance to edit. This can be a regular block instance or a BoundBlock.",
+            type_hint="blocks.Block"
+        ),
+        Keyword("block_id",
+            optional=True,
+            help_text="the ID of the block to edit, required if block is not a BoundBlock.",
+            type_hint="int"
+        ),
+        Keyword("admin",
+            absolute=True,
+            help_text="if passed; the adapter will a quick- link to the Wagtail Admin for this block."
+        ),
+    )
 
     def __init__(self, object: models.Model, field_name: str, request: HttpRequest, **kwargs):
         super().__init__(object, field_name, request, **kwargs)
 
         self.block = self.kwargs.pop("block", None)
         if self.block:
             if not hasattr(self.block, "id") and not "block_id" in self.kwargs:
@@ -72,14 +75,18 @@
             self.streamfield: StreamValue = getattr(self.object, self.field_name)
             result = utils.find_block(block_id, self.streamfield)
             if not result:
                 raise AdapterError("Block not found; did you provide the correct block ID?")
             
             self.block, _ = result
 
+    @cached_property
+    def tooltip(self) -> str:
+        return self.get_header_title()
+
     def get_admin_url(self) -> str:
         finder = AdminURLFinder(self.request.user)
         url = finder.get_edit_url(self.object)
         hash = f"#block-{self.kwargs['block_id']}-section"
         return f"{url}{hash}"
 
     def get_toolbar_buttons(self) -> list[FeditAdapterComponent]:
@@ -96,15 +103,15 @@
 
         model_string = getattr(self.object, "get_admin_display_title", None)
         if model_string:
             model_string = model_string()
         else:
             model_string = getattr(self.object, "title", str(self.object))
 
-        return _("Edit block %(block_label)s for %(model_name)s %(model_string)s") % {
+        return _("Edit block %(block_label)s for %(model_name)s '%(model_string)s'") % {
             "block_label": self.block.block.label,
             "model_name": self.model._meta.verbose_name,
             "model_string": model_string,
         }
     
     def get_element_id(self) -> str:
         return f"block-{self.kwargs['block_id']}-section"
```

### Comparing `wagtail_fedit-1.5.3rc9/wagtail_fedit/adapters/field.py` & `wagtail_fedit-1.5.4rc1/wagtail_fedit/adapters/field.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,21 +64,21 @@
 
     def get_header_title(self):
         meta_field: models.Field = self.model._meta.get_field(self.field_name)
 
         model_string = get_model_string(self.original_object)
         if self.original_object != self.object:
             instance_string = get_model_string(self.object)
-            return _("Edit model %(instance_string)s for %(model_name)s %(model_string)s") % {
+            return _("Edit model '%(instance_string)s' for %(model_name)s '%(model_string)s'") % {
                 "instance_string": instance_string,
                 "model_name": self.model._meta.verbose_name,
                 "model_string": model_string,
             }
 
-        return _("Edit field %(field_name)s for %(model_name)s %(model_string)s") % {
+        return _("Edit field '%(field_name)s' for %(model_name)s '%(model_string)s'") % {
             "field_name": meta_field.verbose_name,
             "model_name": self.model._meta.verbose_name,
             "model_string": model_string,
         }
     
     def get_help_text(self):
         if is_draft_capable(self.original_object)\
@@ -117,19 +117,15 @@
                 "text": mark_safe(_("You must publish the related object of type %(type)s (%(model)s) to make any changes visible.") % {
                     "type": self.original_object._meta.verbose_name,
                     "model": get_model_string(self.original_object, publish_url=True, request=self.request),
                 })
             }
 
         return super().get_help_text()
-          
-    def get_element_id(self) -> str:
-        m = self.model
-        return f"field-{self.field_name}-{m._meta.app_label}-{m._meta.model_name}-{self.object.pk}"
-      
+    
     def get_form_attrs(self) -> dict:
         attrs = super().get_form_attrs()
 
         size = getattr(self.object, f"{VARIABLES.PY_SIZE_VAR}_{self.field_name}", None)
         if not size:
 
             for hook in hooks.get_hooks(FIELD_EDITOR_SIZE):
```

### Comparing `wagtail_fedit-1.5.3rc9/wagtail_fedit/adapters/funcs.py` & `wagtail_fedit-1.5.4rc1/wagtail_fedit/adapters/funcs.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from django.utils.functional import classproperty
+from .base import Keyword
 from .block import BlockAdapter
 from .field import FieldAdapter
 from itertools import chain
 
 
 # https://stackoverflow.com/a/29088221/18020941
 def dj_model_to_dict(instance):
@@ -13,55 +14,72 @@
     for f in opts.many_to_many:
         data[f.name] = [i.id for i in f.value_from_object(instance)]
     return data
 
 
 class FuncAdapterMixin:
     base_identifier = None
-    base_required_kwargs = []
+    base_keywords = ()
     js_constructor = "wagtail_fedit.editors.BaseFuncEditor"
     js_function = None
 
     @classproperty
     def identifier(cls):
         if not cls.base_identifier:
             raise NotImplementedError("base_identifier is required")
         
         return f"{cls.base_identifier}_func"
     
+    def get_element_id_parts(self) -> list[str]:
+        return super().get_element_id_parts() + [
+            self.kwargs["target"],
+        ]
+
     @classproperty
-    def required_kwargs(cls):
+    def keywords(cls):
 
         if cls.js_function:
-            return cls.base_required_kwargs + [
+            return cls.base_keywords + (
+                Keyword(
+                    "target",
+                    help_text="The target element to apply the function to.",
+                    type_hint="str",
+                ),
+            )
+
+        return cls.base_keywords + (
+            Keyword(
+                "name",
+                help_text="The name of the javascript function to call.",
+                type_hint="str",
+            ),
+            Keyword(
                 "target",
-            ]
-
-        return cls.base_required_kwargs + [
-            "name",
-            "target",
-        ]
+                help_text="The target element to apply the function to.",
+                type_hint="str",
+            ),
+        )
 
     def get_response_data(self, parent_context=None):
         data = super().get_response_data(parent_context)
         name = self.js_function or self.kwargs["name"]
         target = self.kwargs["target"]
         target = target.format(object=self.object)
         data["func"] = {
             "name": name,
             "target": target,
         }
         return data
 
 class BaseFieldFuncAdapter(FuncAdapterMixin, FieldAdapter):
     base_identifier = FieldAdapter.identifier
-    base_required_kwargs = FieldAdapter.required_kwargs
+    base_keywords = FieldAdapter.keywords
 
 class BaseBlockFuncAdapter(FuncAdapterMixin, BlockAdapter):
     base_identifier = BlockAdapter.identifier
-    required_kwargs = BlockAdapter.required_kwargs
+    base_keywords = BlockAdapter.keywords
 
     def get_response_data(self, parent_context=None):
         data = super().get_response_data(parent_context)
         data["block"] = self.block.get_prep_value()
         return data
```

### Comparing `wagtail_fedit-1.5.3rc9/wagtail_fedit/adapters/misc.py` & `wagtail_fedit-1.5.4rc1/wagtail_fedit/adapters/misc.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from django.http import HttpRequest
 from django.utils.functional import classproperty
+from .base import Keyword
 from .field import (
     FieldAdapter,
 )
 from .funcs import (
     BaseFieldFuncAdapter,
 )
 
@@ -19,45 +20,56 @@
     Adapter for background-images.
     On succesful form submission; will return the URL of the image.
     This is placed in the background-image property of the target element. 
     """
     inline = True
     identifier = "field_bg_image"
     usage_description = "This adapter is used for changing a css property of a target element to a background-image."
-    help_text_dict = {
-        "target": "the target element to apply the background-image to - this should be a css selector.",
-        "css_variable_name": "the CSS variable name to apply the background-image to. element.style.setProperty(css_variable_name, url);",
-    }
-    required_kwargs = FieldAdapter.required_kwargs + [
-        "target",
-    ]
-    optional_kwargs = [
-        "css_variable_name",
-    ]
-    absolute_tokens = []
+    keywords = (
+        Keyword(
+            "target",
+            help_text="The target element to apply the background-image to - this should be a css selector.",
+            type_hint="str",
+        ),
+        Keyword(
+            "css_variable_name",
+            optional=True,
+            help_text="The CSS variable name to apply the background-image to. element.style.setProperty(css_variable_name, url);",
+            type_hint="str",
+        ),
+        Keyword(
+            "filter_spec",
+            optional=True,
+            default="original",
+            help_text="The filter spec to apply to the image.",
+        ),
+        Keyword(
+            "preserve_svg",
+            optional=True,
+            default=False,
+            help_text="Preserve SVG images by converting them to a safe format.",
+        ),
+    )
     js_constructor = "wagtail_fedit.editors.WagtailFeditFuncEditor"
     js_function = "wagtail_fedit.funcs.backgroundImageFunc"
 
     def render_content(self, parent_context=None):
         return ""
-
+    
     def get_response_data(self, parent_context=None):
         data = super().get_response_data(parent_context)
         image = getattr(self.object, self.field_name, None)
         if not image:
             return data
 
-        filter_spec = self.kwargs.get("filter_spec", None)
-        if not filter_spec:
-            filter_spec = "original"
-
+        filter_spec = self.kwargs["filter_spec"]
         if not isinstance(filter_spec, str):
             filter_spec = "|".join(filter_spec)
 
-        if image.is_svg() or self.kwargs.get("preserve_svg", False):
+        if image.is_svg() or self.kwargs["preserve_svg"]:
             filter = Filter(to_svg_safe_spec(filter_spec.split("|")))
         else:
             filter = Filter(spec=filter_spec)
 
         rendition = get_rendition_or_not_found(
             image,
             filter,
```

### Comparing `wagtail_fedit-1.5.3rc9/wagtail_fedit/adapters/registry.py` & `wagtail_fedit-1.5.4rc1/wagtail_fedit/adapters/registry.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc9/wagtail_fedit/forms/blocks.py` & `wagtail_fedit-1.5.4rc1/wagtail_fedit/forms/blocks.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc9/wagtail_fedit/forms/fields.py` & `wagtail_fedit-1.5.4rc1/wagtail_fedit/forms/fields.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,24 +15,28 @@
 
 from ..hooks import (
     REGISTER_FIELD_WIDGETS,
 )
 
 from wagtail import hooks
 
+
+
 _looked_for_widgets = False
 _widgets = {}
 
+
 def _look_for_widgets():
     global _looked_for_widgets
     if not _looked_for_widgets:
         _looked_for_widgets = True
         for fn in hooks.get_hooks(REGISTER_FIELD_WIDGETS):
             _widgets.update(fn(_widgets))
 
+
 def get_widget_for_field(field: models.Field) -> Type[forms.Widget]:
     """
     Return a widget for a field.
     """
     _look_for_widgets()
     global _widgets
 
@@ -44,29 +48,14 @@
 
     if widget is None:
         pass
 
     return widget
 
 
-class PossibleRevisionForm(WagtailAdminModelForm):
-    """
-    A form that can save a revision if the model is a RevisionMixin.
-    Otherwise resorts to the default save method; this saves the (live) instance.
-    """
-    def __init__(self, *args, request = None, **kwargs):
-        self.request = request
-        super().__init__(*args, **kwargs)
-
-    def save(self, commit=True):
-        instance = super().save(commit=False)
-        if commit:
-            instance = save_possible_revision(instance, self.request)
-        return instance
-
 def save_possible_revision(instance: models.Model, request: HttpRequest, **kwargs) -> models.Model:
     """
     Save an instance as a revision if the model supports it.
     """
     if isinstance(instance, RevisionMixin):
         instance = instance.save_revision(
             user=request.user,
@@ -74,15 +63,16 @@
         )
         instance = instance.as_object()
     else:
         instance.save()
 
     return instance
 
-def get_form_class_for_fields(form_model: models.Model, form_fields: list[str]) -> Type[PossibleRevisionForm]:
+
+def get_form_class_for_fields(form_model: models.Model, form_fields: list[str]) -> Type["PossibleRevisionForm"]:
     """
     Return a form class for a model with specific fields.
     This is similar to django's modelform_factory, but with the added benefit of using the custom widgets.
     It also keeps the revision functionality in mind.
     """
 
     if hasattr(form_model, "get_fedit_form"):
@@ -101,7 +91,30 @@
     class RevisionForm(PossibleRevisionForm):
         class Meta:
             model = form_model
             fields = form_fields
             widgets = form_widgets
 
     return RevisionForm
+
+
+class PossibleRevisionFormMixin:
+    """
+    A form that can save a revision if the model is a RevisionMixin.
+    Otherwise resorts to the default save method; this saves the (live) instance.
+    """
+    def __init__(self, *args, request = None, **kwargs):
+        self.request = request
+        super().__init__(*args, **kwargs)
+
+    def save(self, commit=True):
+        self.instance = super().save(commit=False)
+        if commit:
+            self.instance = save_possible_revision(
+                self.instance,
+                self.request,
+            )
+        return self.instance
+
+
+class PossibleRevisionForm(PossibleRevisionFormMixin, WagtailAdminModelForm):
+    pass
```

### Comparing `wagtail_fedit-1.5.3rc9/wagtail_fedit/hooks.py` & `wagtail_fedit-1.5.4rc1/wagtail_fedit/hooks.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc9/wagtail_fedit/locale/nl/LC_MESSAGES/django.mo` & `wagtail_fedit-1.5.4rc1/wagtail_fedit/locale/nl/LC_MESSAGES/django.mo`

 * *Files 9% similar despite different names*

#### msgunfmt {}

```diff
@@ -34,17 +34,14 @@
 
 msgid "Are you sure you want to continue?"
 msgstr "Weet u zeker dat u wilt doorgaan?"
 
 msgid "Block Changed (Frontend)"
 msgstr "Blok gewijzigd (Frontend)"
 
-msgid "Block Validation Errors"
-msgstr "Blokvalidatiefouten"
-
 msgid "Cancel"
 msgstr "Annuleren"
 
 msgid "Cancel Workflow"
 msgstr "Workflow annuleren"
 
 msgid ""
@@ -80,34 +77,38 @@
 
 msgid "Current draft"
 msgstr "Huidige concept"
 
 msgid "Date / Time"
 msgstr "Datum / Tijd"
 
+msgid "Edit %(type)s '%(model)s'"
+msgstr "Bewerk %(type)s '%(model)s'"
+
 msgid "Edit Field"
 msgstr "Bewerk veld"
 
 msgid "Edit Related"
 msgstr "Bewerk gerelateerd"
 
-msgid "Edit block"
-msgstr "Bewerk blok"
-
-msgid "Edit block %(block_label)s for %(model_name)s %(model_string)s"
-msgstr "Bewerk blok %(block_label)s voor %(model_name)s %(model_string)s"
+msgid "Edit block %(block_label)s for %(model_name)s '%(model_string)s'"
+msgstr "Bewerk blok %(block_label)s voor %(model_name)s '%(model_string)s'"
 
-msgid "Edit field %(field_name)s for %(model_name)s %(model_string)s"
-msgstr "Bewerk veld %(field_name)s voor %(model_name)s %(model_string)s"
+msgid "Edit field '%(field_name)s' for %(model_name)s '%(model_string)s'"
+msgstr "Bewerk veld %(field_name)s voor %(model_name)s' %(model_string)s'"
 
 msgid "Edit in Wagtail Admin"
 msgstr "Bewerk in Wagtail Admin"
 
-msgid "Edit model %(instance_string)s for %(model_name)s %(model_string)s"
-msgstr "Bewerk model %(instance_string)s voor %(model_name)s %(model_string)s"
+msgid "Edit model '%(instance_string)s'"
+msgstr "Bewerk model '%(instance_string)s'"
+
+msgid "Edit model '%(instance_string)s' for %(model_name)s '%(model_string)s'"
+msgstr ""
+"Bewerk model %(instance_string)s voor %(model_name)s '%(model_string)s'"
 
 msgid "Field Changed (Frontend)"
 msgstr "Veld gewijzigd (Frontend)"
 
 msgid "Frontend Edit"
 msgstr "Bewerk op frontend"
 
@@ -213,14 +214,17 @@
 
 msgid "Validation Errors"
 msgstr "Validatiefouten"
 
 msgid "View Live Page"
 msgstr "Bekijk live pagina"
 
+msgid "View in Wagtail admin"
+msgstr "Bekijk in Wagtail admin"
+
 msgid ""
 "You are not required to publish this object to make this change visible."
 msgstr ""
 "U hoeft dit object niet te publiceren om deze wijziging zichtbaar te maken."
 
 msgid "You are still able to edit this object."
 msgstr "U kunt dit object nog steeds bewerken."
```

### Comparing `wagtail_fedit-1.5.3rc9/wagtail_fedit/locale/nl/LC_MESSAGES/django.po` & `wagtail_fedit-1.5.4rc1/wagtail_fedit/locale/nl/LC_MESSAGES/django.po`

 * *Files 6% similar despite different names*

```diff
@@ -4,32 +4,75 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2024-04-11 11:04+0200\n"
+"POT-Creation-Date: 2024-04-23 17:49+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
-#: .\tester\wagtail_fedit\templates\wagtail_fedit\content\buttons\edit_block.html:3
-msgid "Edit block"
-msgstr "Bewerk blok"
+#: .\tester\wagtail_fedit\adapters\block.py:110
+msgid "Edit block %(block_label)s for %(model_name)s '%(model_string)s'"
+msgstr "Bewerk blok %(block_label)s voor %(model_name)s '%(model_string)s'"
+
+#: .\tester\wagtail_fedit\adapters\field.py:71
+msgid "Edit model '%(instance_string)s' for %(model_name)s '%(model_string)s'"
+msgstr "Bewerk model %(instance_string)s voor %(model_name)s '%(model_string)s'"
+
+#: .\tester\wagtail_fedit\adapters\field.py:77
+msgid "Edit field '%(field_name)s' for %(model_name)s '%(model_string)s'"
+msgstr "Bewerk veld %(field_name)s voor %(model_name)s' %(model_string)s'"
 
-#: .\tester\wagtail_fedit\templates\wagtail_fedit\content\buttons\edit_field.html:3
-#: .\tester\wagtail_fedit\wagtail_hooks\log_actions.py:49
-msgid "Edit Field"
-msgstr "Bewerk veld"
+#: .\tester\wagtail_fedit\adapters\field.py:91
+#, python-format
+msgid ""
+"You must publish %(model)s and the related object of type "
+"%(related_verbose_name)s (%(related_model)s) to make any changes visible."
+msgstr ""
+"U moet %(model)s en het gerelateerde object van het type "
+"%(related_verbose_name)s (%(related_model)s) publiceren om wijzigingen "
+"zichtbaar te maken."
+
+#: .\tester\wagtail_fedit\adapters\field.py:115
+msgid "Publishing related object required."
+msgstr "Publicatie van gerelateerd object vereist."
+
+#: .\tester\wagtail_fedit\adapters\field.py:116
+#: .\tester\wagtail_fedit\utils.py:71
+msgid "The object you are editing supports drafts."
+msgstr "Het object dat u bewerkt ondersteunt concepten."
+
+#: .\tester\wagtail_fedit\adapters\field.py:117
+#, python-format
+msgid ""
+"You must publish the related object of type %(type)s (%(model)s) to make any "
+"changes visible."
+msgstr ""
+"U moet het gerelateerde object van het type %(type)s (%(model)s) publiceren "
+"om wijzigingen zichtbaar te maken."
+
+#: .\tester\wagtail_fedit\adapters\models.py:41
+msgid "This adapter is used for directly editing a model instance."
+msgstr ""
+
+#: .\tester\wagtail_fedit\adapters\models.py:108
+msgid "Edit model '%(instance_string)s'"
+msgstr "Bewerk model '%(instance_string)s'"
+
+#: .\tester\wagtail_fedit\templates\wagtail_fedit\content\buttons\admin_link.html:1
+msgid "View in Wagtail admin"
+msgstr "Bekijk in Wagtail admin"
 
 #: .\tester\wagtail_fedit\templates\wagtail_fedit\editor\action_confirm.html:32
 msgid "Are you sure you want to continue?"
 msgstr "Weet u zeker dat u wilt doorgaan?"
 
 #: .\tester\wagtail_fedit\templates\wagtail_fedit\editor\action_confirm.html:45
 msgid "Cancel"
@@ -55,15 +98,15 @@
 msgid "Comment"
 msgstr "Commentaar"
 
 #: .\tester\wagtail_fedit\templates\wagtail_fedit\editor\action_publish_confirm.html:38
 msgid "Current draft"
 msgstr "Huidige concept"
 
-#: .\tester\wagtail_fedit\templates\wagtail_fedit\editor\action_publish_confirm.html:55
+#: .\tester\wagtail_fedit\templates\wagtail_fedit\editor\action_publish_confirm.html:57
 #, python-format
 msgid ""
 "This object has more changes. <a href=\"%(view_more_url)s\">View all changes."
 "</a>"
 msgstr ""
 "Dit object heeft meer wijzigingen. <a href=\"%(view_more_url)s\">Bekijk alle "
 "wijzigingen.</a>"
@@ -80,25 +123,25 @@
 msgid "You are still able to edit this object."
 msgstr "U kunt dit object nog steeds bewerken."
 
 #: .\tester\wagtail_fedit\templates\wagtail_fedit\editor\base_iframe.html:68
 msgid "This object is locked and cannot be edited."
 msgstr "Dit object is vergrendeld en kan niet worden bewerkt."
 
-#: .\tester\wagtail_fedit\templates\wagtail_fedit\editor\base_iframe.html:100
+#: .\tester\wagtail_fedit\templates\wagtail_fedit\editor\base_iframe.html:90
 msgid "Edit in Wagtail Admin"
 msgstr "Bewerk in Wagtail Admin"
 
-#: .\tester\wagtail_fedit\templates\wagtail_fedit\editor\base_iframe.html:104
-#: .\tester\wagtail_fedit\templates\wagtail_fedit\editor\base_iframe.html:105
+#: .\tester\wagtail_fedit\templates\wagtail_fedit\editor\base_iframe.html:94
+#: .\tester\wagtail_fedit\templates\wagtail_fedit\editor\base_iframe.html:95
 msgid "Save"
 msgstr "Opslaan"
 
-#: .\tester\wagtail_fedit\templates\wagtail_fedit\editor\base_iframe.html:111
-#: .\tester\wagtail_fedit\templates\wagtail_fedit\editor\base_iframe.html:112
+#: .\tester\wagtail_fedit\templates\wagtail_fedit\editor\base_iframe.html:101
+#: .\tester\wagtail_fedit\templates\wagtail_fedit\editor\base_iframe.html:102
 msgid "Close"
 msgstr "Sluiten"
 
 #: .\tester\wagtail_fedit\templates\wagtail_fedit\userbar\item_fedit.html:11
 msgid "Frontend Editing"
 msgstr "Bewerken op frontend"
 
@@ -106,207 +149,167 @@
 msgid "View Live Page"
 msgstr "Bekijk live pagina"
 
 #: .\tester\wagtail_fedit\templates\wagtail_fedit\userbar\publish\item_fedit_publishing.html:17
 msgid "Revision Management"
 msgstr "Revisiebeheer"
 
-#: .\tester\wagtail_fedit\utils.py:54 .\tester\wagtail_fedit\views\fields.py:51
+#: .\tester\wagtail_fedit\utils.py:68
+#: .\tester\wagtail_fedit\views\adapters.py:40
 msgid "Validation Errors"
 msgstr "Validatiefouten"
 
-#: .\tester\wagtail_fedit\utils.py:56
+#: .\tester\wagtail_fedit\utils.py:70
 msgid "Publishing Required"
 msgstr "Publicatie vereist"
 
-#: .\tester\wagtail_fedit\utils.py:57
-#: .\tester\wagtail_fedit\views\fields.py:183
-msgid "The object you are editing supports drafts."
-msgstr "Het object dat u bewerkt ondersteunt concepten."
-
-#: .\tester\wagtail_fedit\utils.py:58
+#: .\tester\wagtail_fedit\utils.py:72
 #, python-format
 msgid "You must publish %(model)s to make any changes visible."
 msgstr "U moet %(model)s publiceren om wijzigingen zichtbaar te maken."
 
-#: .\tester\wagtail_fedit\utils.py:60
+#: .\tester\wagtail_fedit\utils.py:74
 msgid "No Publishing Required"
 msgstr "Geen publicatie vereist"
 
-#: .\tester\wagtail_fedit\utils.py:61
+#: .\tester\wagtail_fedit\utils.py:75
 msgid "The object you are editing does not support drafts."
 msgstr "Het object dat u bewerkt ondersteunt geen concepten."
 
-#: .\tester\wagtail_fedit\utils.py:62
+#: .\tester\wagtail_fedit\utils.py:76
 msgid ""
 "You are not required to publish this object to make this change visible."
 msgstr ""
 "U hoeft dit object niet te publiceren om deze wijziging zichtbaar te maken."
 
-#: .\tester\wagtail_fedit\views\blocks.py:31
-msgid "Block Validation Errors"
-msgstr "Blokvalidatiefouten"
-
-#: .\tester\wagtail_fedit\views\blocks.py:91
+#: .\tester\wagtail_fedit\utils.py:90
 #, python-format
-msgid "Edit block %(block_label)s for %(model_name)s %(model_string)s"
-msgstr "Bewerk blok %(block_label)s voor %(model_name)s %(model_string)s"
+msgid "Edit %(type)s '%(model)s'"
+msgstr "Bewerk %(type)s '%(model)s'"
 
-#: .\tester\wagtail_fedit\views\editable.py:218
+#: .\tester\wagtail_fedit\views\editable.py:222
 msgid "This object is locked. It cannot be acted upon."
 msgstr "Dit object is vergrendeld. Er kan niet op worden gereageerd."
 
-#: .\tester\wagtail_fedit\views\editable.py:222
+#: .\tester\wagtail_fedit\views\editable.py:226
 msgid "No action specified"
 msgstr "Geen actie opgegeven"
 
-#: .\tester\wagtail_fedit\views\editable.py:226
+#: .\tester\wagtail_fedit\views\editable.py:230
 msgid "Invalid action specified: {}"
 msgstr "Ongeldige actie opgegeven: {}"
 
-#: .\tester\wagtail_fedit\views\editable.py:235
-#: .\tester\wagtail_fedit\wagtail_hooks\userbar.py:48
+#: .\tester\wagtail_fedit\views\editable.py:239
+#: .\tester\wagtail_fedit\wagtail_hooks\userbar.py:53
 msgid "Publish"
 msgstr "Publiceren"
 
-#: .\tester\wagtail_fedit\views\editable.py:239
+#: .\tester\wagtail_fedit\views\editable.py:243
 msgid "Publishing {} \"{}\""
 msgstr "Publiceren van {} \"{}\""
 
-#: .\tester\wagtail_fedit\views\editable.py:242
+#: .\tester\wagtail_fedit\views\editable.py:246
 msgid "About publishing"
 msgstr "Over publiceren"
 
-#: .\tester\wagtail_fedit\views\editable.py:246
+#: .\tester\wagtail_fedit\views\editable.py:250
 msgid "Publishing this object will make it visible to users on the site."
 msgstr ""
 "Publicatie van dit object maakt het zichtbaar voor gebruikers op de site."
 
-#: .\tester\wagtail_fedit\views\editable.py:247
+#: .\tester\wagtail_fedit\views\editable.py:251
 msgid ""
 "That means that any changes you make will be immediately visible to everyone."
 msgstr ""
 "Dit betekent dat alle wijzigingen die u aanbrengt, onmiddellijk zichtbaar "
 "zijnvoor iedereen."
 
-#: .\tester\wagtail_fedit\views\editable.py:251
+#: .\tester\wagtail_fedit\views\editable.py:255
 msgid "You can always choose to unpublish it."
 msgstr "U kunt er altijd voor kiezen om het te depubliceren."
 
-#: .\tester\wagtail_fedit\views\editable.py:347
-#: .\tester\wagtail_fedit\wagtail_hooks\userbar.py:59
+#: .\tester\wagtail_fedit\views\editable.py:356
+#: .\tester\wagtail_fedit\wagtail_hooks\userbar.py:65
 msgid "Unpublish"
 msgstr "Depubliceren"
 
-#: .\tester\wagtail_fedit\views\editable.py:348
+#: .\tester\wagtail_fedit\views\editable.py:357
 msgid "About unpublishing"
 msgstr "Over depubliceren"
 
-#: .\tester\wagtail_fedit\views\editable.py:350
+#: .\tester\wagtail_fedit\views\editable.py:359
 msgid "Unpublishing this object will make it invisible to users on the site."
 msgstr ""
 "Depublicatie van dit object maakt het onzichtbaar voor gebruikers op de site."
 
-#: .\tester\wagtail_fedit\views\editable.py:351
-#: .\tester\wagtail_fedit\views\editable.py:390
-#: .\tester\wagtail_fedit\views\editable.py:433
+#: .\tester\wagtail_fedit\views\editable.py:360
+#: .\tester\wagtail_fedit\views\editable.py:399
+#: .\tester\wagtail_fedit\views\editable.py:442
 msgid "That means that it will no longer be visible to anyone."
 msgstr "Dat betekent dat het niet langer zichtbaar is voor iedereen."
 
-#: .\tester\wagtail_fedit\views\editable.py:352
-#: .\tester\wagtail_fedit\views\editable.py:391
+#: .\tester\wagtail_fedit\views\editable.py:361
+#: .\tester\wagtail_fedit\views\editable.py:400
 msgid "You can always choose to publish it again."
 msgstr "U kunt er altijd voor kiezen om het opnieuw te publiceren."
 
-#: .\tester\wagtail_fedit\views\editable.py:356
+#: .\tester\wagtail_fedit\views\editable.py:365
 msgid "Unpublishing {} \"{}\""
 msgstr "Depubliceren van {} \"{}\""
 
-#: .\tester\wagtail_fedit\views\editable.py:370
+#: .\tester\wagtail_fedit\views\editable.py:379
 msgid "This object is not live"
 msgstr "Dit object is niet live"
 
-#: .\tester\wagtail_fedit\views\editable.py:386
-#: .\tester\wagtail_fedit\wagtail_hooks\userbar.py:70
+#: .\tester\wagtail_fedit\views\editable.py:395
+#: .\tester\wagtail_fedit\wagtail_hooks\userbar.py:76
 msgid "Submit for moderation"
 msgstr "Indienen voor moderatie"
 
-#: .\tester\wagtail_fedit\views\editable.py:387
+#: .\tester\wagtail_fedit\views\editable.py:396
 msgid "About submitting for moderation"
 msgstr "Over indienen voor moderatie"
 
-#: .\tester\wagtail_fedit\views\editable.py:389
+#: .\tester\wagtail_fedit\views\editable.py:398
 msgid ""
 "Submitting this object for moderation will make it invisible to users on the "
 "site."
 msgstr ""
 "Het indienen van dit object voor moderatie maakt het onzichtbaar voor "
 "gebruikers op de site."
 
-#: .\tester\wagtail_fedit\views\editable.py:395
+#: .\tester\wagtail_fedit\views\editable.py:404
 msgid "Submitting {} \"{}\" for moderation"
 msgstr "Indienen van {} \"{}\" voor moderatie"
 
-#: .\tester\wagtail_fedit\views\editable.py:429
-#: .\tester\wagtail_fedit\wagtail_hooks\userbar.py:81
+#: .\tester\wagtail_fedit\views\editable.py:438
+#: .\tester\wagtail_fedit\wagtail_hooks\userbar.py:88
 msgid "Cancel Workflow"
 msgstr "Workflow annuleren"
 
-#: .\tester\wagtail_fedit\views\editable.py:430
+#: .\tester\wagtail_fedit\views\editable.py:439
 msgid "About cancelling workflows"
 msgstr "Over het annuleren van workflows"
 
-#: .\tester\wagtail_fedit\views\editable.py:432
+#: .\tester\wagtail_fedit\views\editable.py:441
 msgid ""
 "Cancelling the workflow for this object will remove it from the moderation "
 "process."
 msgstr ""
 "Het annuleren van de workflow voor dit object verwijdert het uit het "
 "moderatieproces."
 
-#: .\tester\wagtail_fedit\views\editable.py:434
+#: .\tester\wagtail_fedit\views\editable.py:443
 msgid "You can always choose to submit it for moderation again."
-msgstr "Je kunt er altijd voor kiezen om het opnieuw in te dienen voor moderatie."
-
-#: .\tester\wagtail_fedit\views\editable.py:438
-msgid "Cancelling workflow for {} \"{}\""
-msgstr ""
-
-#: .\tester\wagtail_fedit\views\fields.py:122
-#, python-format
-msgid "Edit model %(instance_string)s for %(model_name)s %(model_string)s"
-msgstr "Bewerk model %(instance_string)s voor %(model_name)s %(model_string)s"
-
-#: .\tester\wagtail_fedit\views\fields.py:128
-#, python-format
-msgid "Edit field %(field_name)s for %(model_name)s %(model_string)s"
-msgstr "Bewerk veld %(field_name)s voor %(model_name)s %(model_string)s"
-
-#: .\tester\wagtail_fedit\views\fields.py:158
-#, python-format
-msgid ""
-"You must publish %(model)s and the related object of type "
-"%(related_verbose_name)s (%(related_model)s) to make any changes visible."
 msgstr ""
-"U moet %(model)s en het gerelateerde object van het type "
-"%(related_verbose_name)s (%(related_model)s) publiceren om wijzigingen "
-"zichtbaar te maken."
-
-#: .\tester\wagtail_fedit\views\fields.py:182
-msgid "Publishing related object required."
-msgstr "Publicatie van gerelateerd object vereist."
+"Je kunt er altijd voor kiezen om het opnieuw in te dienen voor moderatie."
 
-#: .\tester\wagtail_fedit\views\fields.py:184
-#, python-format
-msgid ""
-"You must publish the related object of type %(type)s (%(model)s) to make any "
-"changes visible."
+#: .\tester\wagtail_fedit\views\editable.py:447
+msgid "Cancelling workflow for {} \"{}\""
 msgstr ""
-"U moet het gerelateerde object van het type %(type)s (%(model)s) publiceren "
-"om wijzigingen zichtbaar te maken."
 
 #: .\tester\wagtail_fedit\wagtail_hooks\action_menu.py:14
 msgid "Frontend Edit"
 msgstr "Bewerk op frontend"
 
 #: .\tester\wagtail_fedit\wagtail_hooks\log_actions.py:10
 msgid "Edit Related"
@@ -334,14 +337,18 @@
 "'%(field)s' (Frontend)"
 
 #: .\tester\wagtail_fedit\wagtail_hooks\log_actions.py:42
 #, python-format
 msgid "Changed '%(field)s' from '%(old)s' to '%(new)s' (Frontend)"
 msgstr "Gewijzigd '%(field)s' van '%(old)s' naar '%(new)s' (Frontend)"
 
+#: .\tester\wagtail_fedit\wagtail_hooks\log_actions.py:49
+msgid "Edit Field"
+msgstr "Bewerk veld"
+
 #: .\tester\wagtail_fedit\wagtail_hooks\log_actions.py:54
 msgid "Block Changed (Frontend)"
 msgstr "Blok gewijzigd (Frontend)"
 
 #: .\tester\wagtail_fedit\wagtail_hooks\log_actions.py:55
 msgid "A block was changed from the frontend"
 msgstr "Een blok is gewijzigd vanaf de frontend"
@@ -349,9 +356,15 @@
 #: .\tester\wagtail_fedit\wagtail_hooks\log_actions.py:68
 #, python-format
 msgid ""
 "Changed block \"%(block)s\" on field \"%(field)s\" (%(block_id)s, Frontend)"
 msgstr ""
 "Blok \"%(block)s\" gewijzigd op veld \"%(field)s\" (%(block_id)s, Frontend)"
 
+#~ msgid "Edit block"
+#~ msgstr "Bewerk blok"
+
+#~ msgid "Block Validation Errors"
+#~ msgstr "Blokvalidatiefouten"
+
 #~ msgid "Submit for Moderation"
 #~ msgstr "Indienen voor moderatie"
```

### Comparing `wagtail_fedit-1.5.3rc9/wagtail_fedit/models.py` & `wagtail_fedit-1.5.4rc1/wagtail_fedit/models.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc9/wagtail_fedit/static/wagtail_fedit/css/frontend.css` & `wagtail_fedit-1.5.4rc1/wagtail_fedit/static/wagtail_fedit/css/frontend.css`

 * *Files 5% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 .wagtail-fedit-adapter-wrapper {
     position: relative;
     min-height: 24px;
 }
 .wagtail-fedit-field_bg_image {
     display: inline-flex;
 }
+.wagtail-fedit-adapter-wrapper:has(> .wagtail-fedit-buttons a:hover)::after,
 .wagtail-fedit-adapter-wrapper:has(> .wagtail-fedit-buttons button:hover)::after {
     content: '';
     display: block;
     position: absolute;
     top: 0;
     left: 0;
     width: 100%;
@@ -50,45 +51,51 @@
     margin-left: 0.25rem;
     margin-right: 0.25rem;
     vertical-align: top;
     left: unset;
     right: unset;
 }
 
+.wagtail-fedit-adapter-wrapper .wagtail-fedit-adapter-wrapper > .wagtail-fedit-buttons {
+    flex-direction: column-reverse;
+}
+
 /* .wagtail-fedit-field-wrapper > .wagtail-fedit-buttons { */
     /* position: relative; */
 /* } */
 .wagtail-fedit-adapter-wrapper > .wagtail-fedit-buttons .wagtail-fedit-toolbar-button,
 .wagtail-fedit-adapter-wrapper > .wagtail-fedit-buttons button {
-    display: inline-block;
     vertical-align: middle;
 }
 .wagtail-fedit-buttons .wagtail-fedit-toolbar-button,
 .wagtail-fedit-buttons button {
     border: none;
-    background-color: white;
+    background-color: rgba(0, 0, 0, 0.85);
     padding: 0.1em;
     border-radius: 0.25em;
     width: 24px;
     height: 24px;
     cursor: pointer;
+    display: flex;
+    justify-content: center;
+    align-items: center;
 }
 .wagtail-fedit-buttons button,
 .wagtail-fedit-buttons button svg,
 .wagtail-fedit-buttons > a,
 .wagtail-fedit-buttons > a svg,
 .wagtail-fedit-buttons > a:hover svg,
 .wagtail-fedit-buttons > a:visited,
 .wagtail-fedit-buttons > a:hover,
 .wagtail-fedit-buttons > a:active{
-    color: rgb(14, 49, 100) !important;
+    color: white !important;
 }
 .wagtail-fedit-buttons svg {
     vertical-align: middle;
-    color: rgb(14, 49, 100);
+    color: white;
 }
 body:has(.wagtail-fedit-modal) {
     overflow: hidden;
 }
 /* *:target::after { */
     /* content: ''; */
     /* display: block; */
```

### Comparing `wagtail_fedit-1.5.3rc9/wagtail_fedit/static/wagtail_fedit/css/furniture.css` & `wagtail_fedit-1.5.4rc1/wagtail_fedit/static/wagtail_fedit/css/furniture.css`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc9/wagtail_fedit/static/wagtail_fedit/css/userbar-menu.css` & `wagtail_fedit-1.5.4rc1/wagtail_fedit/static/wagtail_fedit/css/userbar-menu.css`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc9/wagtail_fedit/static/wagtail_fedit/js/frontend.js` & `wagtail_fedit-1.5.4rc1/wagtail_fedit/static/wagtail_fedit/js/frontend.js`

 * *Files 7% similar despite different names*

#### js-beautify {}

```diff
@@ -93,14 +93,38 @@
             onError();
         };
         return iframe;
     }
 }
 
 
+class Tooltip {
+    constructor(element) {
+        this.element = element;
+        this.tooltipConfig = this.makeConfig();
+        this.init();
+    }
+
+    init() {
+        tippy(this.element, this.tooltipConfig);
+    }
+
+    makeConfig() {
+        const cfg = {}
+        for (const attr of this.element.attributes) {
+            if (attr.name.startsWith("data-tooltip-")) {
+                const key = attr.name.replace("data-tooltip-", "");
+                cfg[key] = attr.value;
+            }
+        }
+        this.tooltipConfig = cfg;
+        return cfg;
+    }
+}
+
 const modalHtml = `
 <div class="wagtail-fedit-modal-wrapper">
     <div class="wagtail-fedit-modal" id="wagtail-fedit-modal-__ID__-modal">
     </div>
 </div>`
 
 
@@ -330,32 +354,42 @@
             e.preventDefault();
             e.stopPropagation();
             await this.makeModal();
         });
     }
 
     initNewEditors() {
-        const wagtailFeditBlockEditors = this.wrapperElement.querySelectorAll(".wagtail-fedit-adapter-wrapper");
-        for (const editor of wagtailFeditBlockEditors) {
-            if (!editor.classList.contains("wagtail-fedit-initialized")) {
-                editor.classList.add("wagtail-fedit-initialized");
-                const editorClass = getEditorClass(editor);
-                if (editorClass) {
-                    new editorClass({
-                        element: editor
-                    });
-                } else {
-                    console.error("No editor class found for element", editor);
-                }
+        initNewEditors(this.wrapperElement);
+    }
+}
+
+function initNewEditors(wrapper = document) {
+    const wagtailFeditBlockEditors = wrapper.querySelectorAll(".wagtail-fedit-adapter-wrapper");
+    for (const editor of wagtailFeditBlockEditors) {
+        if (!editor.classList.contains("wagtail-fedit-initialized")) {
+            editor.classList.add("wagtail-fedit-initialized");
+            const editorClass = getEditorClass(editor);
+            if (editorClass) {
+                new editorClass({
+                    element: editor
+                });
+            } else {
+                console.error("No editor class found for element", editor);
             }
         }
     }
+    const editButtons = wrapper.querySelectorAll("[data-tooltip='true']");
+    for (const button of editButtons) {
+        if (button.dataset.tooltip == "true") {
+            new Tooltip(button);
+            delete button.dataset.tooltip;
+        }
+    }
 }
 
-
 class BaseFuncEditor extends BaseWagtailFeditEditor {
     static get funcMap() {
         return window
     }
 
     onResponse(response) {
         const name = response.func.name;
@@ -497,28 +531,15 @@
         return window.wagtailFedit.editors[editorClass];
     }
     return null;
 }
 
 
 function initFEditors() {
-    const editors = document.querySelectorAll(".wagtail-fedit-adapter-wrapper");
-    for (const editor of editors) {
-        if (!editor.classList.contains("wagtail-fedit-initialized")) {
-            editor.classList.add("wagtail-fedit-initialized");
-            const editorClass = getEditorClass(editor);
-            if (editorClass) {
-                new editorClass({
-                    element: editor
-                });
-            } else {
-                console.error("No editor class found for element", editor);
-            }
-        }
-    }
+    initNewEditors()
     const observer = new MutationObserver((mutations) => {
         for (const mutation of mutations) {
             for (const node of mutation.addedNodes) {
                 if (node.nodeType === 1) {
                     if (node.classList.contains("wagtail-fedit-adapter-wrapper") && !node.classList.contains("wagtail-fedit-initialized")) {
                         node.classList.add("wagtail-fedit-initialized");
                         const editorClass = getEditorClass(node);
@@ -526,14 +547,21 @@
                             new editorClass({
                                 element: node
                             });
                         } else {
                             console.error("No editor class found for element", node);
                         }
                     }
+                    const editButtons = node.querySelectorAll("[data-tooltip='true']");
+                    for (const button of editButtons) {
+                        if (button.dataset.tooltip == "true") {
+                            new Tooltip(button);
+                            delete button.dataset.tooltip;
+                        }
+                    }
                 }
             }
         }
     });
     observer.observe(document.body, {
         childList: true,
         subtree: true
```

### Comparing `wagtail_fedit-1.5.3rc9/wagtail_fedit/templates/wagtail_fedit/content/buttons/admin_link.html` & `wagtail_fedit-1.5.4rc1/wagtail_fedit/templates/wagtail_fedit/content/buttons/admin_link.html`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-{% load i18n %}
-<a href="{{ admin_url }}" target="_blank" class="wagtail-fedit-adapter-admin-link wagtail-fedit-toolbar-button wagtail-fedit-link-button">
-    <svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" fill="currentColor" class="bi bi-box-arrow-up-right" viewBox="0 0 16 16" aria-label="{% translate "View in Wagtail admin" %}">
+{% load i18n fedit %}{% translate "View in Wagtail admin" as edit_text %}
+<a href="{{ admin_url }}" target="_blank" class="wagtail-fedit-adapter-admin-link wagtail-fedit-toolbar-button wagtail-fedit-link-button" {% tooltip edit_text %}>
+    <svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" fill="currentColor" class="bi bi-box-arrow-up-right" viewBox="0 0 16 16" aria-label="{{ edit_text }}">
         <!-- The MIT License (MIT) -->
         <!-- Copyright (c) 2011-2024 The Bootstrap Authors -->
         <path fill-rule="evenodd" d="M8.636 3.5a.5.5 0 0 0-.5-.5H1.5A1.5 1.5 0 0 0 0 4.5v10A1.5 1.5 0 0 0 1.5 16h10a1.5 1.5 0 0 0 1.5-1.5V7.864a.5.5 0 0 0-1 0V14.5a.5.5 0 0 1-.5.5h-10a.5.5 0 0 1-.5-.5v-10a.5.5 0 0 1 .5-.5h6.636a.5.5 0 0 0 .5-.5"/>
         <path fill-rule="evenodd" d="M16 .5a.5.5 0 0 0-.5-.5h-5a.5.5 0 0 0 0 1h3.793L6.146 9.146a.5.5 0 1 0 .708.708L15 1.707V5.5a.5.5 0 0 0 1 0z"/>
     </svg>
 </a>
```

#### html2text {}

```diff
@@ -1,2 +1,2 @@
-{% load i18n %}
-}">
+{% load i18n fedit %}{% translate "View in Wagtail admin" as edit_text %}
+% tooltip edit_text %}>
```

### Comparing `wagtail_fedit-1.5.3rc9/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_adapter.html` & `wagtail_fedit-1.5.4rc1/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_adapter.html`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-{% load i18n %}
-<button class="wagtail-fedit-adapter-edit wagtail-fedit-toolbar-button wagtail-fedit-edit-button">
-    <svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" fill="currentColor" class="bi bi-pencil-square" viewBox="0 0 16 16" aria-label="{% translate "Edit Field" %}">
+{% load i18n fedit %}
+<button class="wagtail-fedit-adapter-edit wagtail-fedit-toolbar-button wagtail-fedit-edit-button" {% if self.adapter.tooltip %}{% tooltip self.adapter.tooltip %}{% endif %}>
+    <svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" fill="currentColor" class="bi bi-pencil-square" viewBox="0 0 16 16" {% if self.adapter.tooltip %}aria-label="{{ self.adapter.tooltip }}"{% endif %}>
         <!-- The MIT License (MIT) -->
         <!-- Copyright (c) 2011-2024 The Bootstrap Authors -->
         <path d="M15.502 1.94a.5.5 0 0 1 0 .706L14.459 3.69l-2-2L13.502.646a.5.5 0 0 1 .707 0l1.293 1.293zm-1.75 2.456-2-2L4.939 9.21a.5.5 0 0 0-.121.196l-.805 2.414a.25.25 0 0 0 .316.316l2.414-.805a.5.5 0 0 0 .196-.12l6.813-6.814z"/>
         <path fill-rule="evenodd" d="M1 13.5A1.5 1.5 0 0 0 2.5 15h11a1.5 1.5 0 0 0 1.5-1.5v-6a.5.5 0 0 0-1 0v6a.5.5 0 0 1-.5.5h-11a.5.5 0 0 1-.5-.5v-11a.5.5 0 0 1 .5-.5H9a.5.5 0 0 0 0-1H2.5A1.5 1.5 0 0 0 1 2.5z"/>
     </svg>
 </button>
```

### Comparing `wagtail_fedit-1.5.3rc9/wagtail_fedit/templates/wagtail_fedit/content/editable_adapter.html` & `wagtail_fedit-1.5.4rc1/wagtail_fedit/templates/wagtail_fedit/content/editable_adapter.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc9/wagtail_fedit/templates/wagtail_fedit/editor/action_confirm.html` & `wagtail_fedit-1.5.4rc1/wagtail_fedit/templates/wagtail_fedit/editor/action_confirm.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc9/wagtail_fedit/templates/wagtail_fedit/editor/action_publish_confirm.html` & `wagtail_fedit-1.5.4rc1/wagtail_fedit/templates/wagtail_fedit/editor/action_publish_confirm.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc9/wagtail_fedit/templates/wagtail_fedit/editor/adapter_form.html` & `wagtail_fedit-1.5.4rc1/wagtail_fedit/templates/wagtail_fedit/editor/adapter_form.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc9/wagtail_fedit/templates/wagtail_fedit/editor/base_iframe.html` & `wagtail_fedit-1.5.4rc1/wagtail_fedit/templates/wagtail_fedit/editor/base_iframe.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc9/wagtail_fedit/templates/wagtail_fedit/icons/fedit-check-list.svg` & `wagtail_fedit-1.5.4rc1/wagtail_fedit/templates/wagtail_fedit/icons/fedit-check-list.svg`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc9/wagtail_fedit/templates/wagtail_fedit/icons/fedit-eye-closed.svg` & `wagtail_fedit-1.5.4rc1/wagtail_fedit/templates/wagtail_fedit/icons/fedit-eye-closed.svg`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc9/wagtail_fedit/templates/wagtail_fedit/icons/fedit-save.svg` & `wagtail_fedit-1.5.4rc1/wagtail_fedit/templates/wagtail_fedit/icons/fedit-save.svg`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc9/wagtail_fedit/templates/wagtail_fedit/icons/fedit-stop-sign.svg` & `wagtail_fedit-1.5.4rc1/wagtail_fedit/templates/wagtail_fedit/icons/fedit-stop-sign.svg`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc9/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit.html` & `wagtail_fedit-1.5.4rc1/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc9/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_view_live.html` & `wagtail_fedit-1.5.4rc1/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_view_live.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc9/wagtail_fedit/templates/wagtail_fedit/userbar/publish/item_fedit_publishing.html` & `wagtail_fedit-1.5.4rc1/wagtail_fedit/templates/wagtail_fedit/userbar/publish/item_fedit_publishing.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc9/wagtail_fedit/templatetags/__pycache__/fedit.cpython-311.pyc` & `wagtail_fedit-1.5.4rc1/wagtail_fedit/templatetags/__pycache__/fedit.cpython-311.pyc`

 * *Files 14% similar despite different names*

#### Python bytecode

```diff
@@ -1,269 +1,320 @@
 magic:    0xa70d0d0a
-moddate:  0xb6602566 (Sun Apr 21 18:53:42 2024 UTC)
-files sz: 8664
+moddate:  0xd5d22766 (Tue Apr 23 15:25:09 2024 UTC)
+files sz: 9470
 code
    argcount  : 0
    nlocals   : 0
-   stacksize : 11
+   stacksize : 13
    flags     : 0
    code
-      0x9700640064016c006d015a010100640064026c026d035a036d045a046d
-      055a050100640064036c066d075a070100640064046c086d095a096d0a5a
-      0a6d0b5a0b0100640064056c0c6d0d5a0d0100640064066c0e6d0f5a0f01
-      00640064076c106d115a110100640064086c126d135a130100640064096c
-      145a14640a640b6c156d165a166d175a176d185a186d195a190100640a64
-      0c6c1a6d1b5a1b6d1c5a1c6d1d5a1d6d1e5a1e0100640a640d6c136d1f5a
-      1f6d205a200100020065036a210000000000000000a6000000ab00000000
-      00000000005a22640e5a23640f5a24641065256411650764126525641365
-      256608641484045a26020047006415840064166504a6030000ab03000000
-      00000000005a276522a02800000000000000000000000000000000000000
-      00651eac17a6010000ab010000000000000000641865096419650a660464
-      1a8404a6000000ab0000000000000000005a296522a02a00000000000000
-      00000000000000000000000000641bac1ca6010000ab0100000000000000
-      0064116507641d6518641365256606641e8404a6000000ab000000000000
-      0000005a2b6522a02c000000000000000000000000000000000000000064
-      1f6420641bac21a6030000ab0300000000000000006413652d6602642284
-      04a6000000ab0000000000000000005a2e6427641865096423652f652519
-      0000000000000000006424652f6525190000000000000000006425652f65
-      25190000000000000000006413652d660a642684055a3064095300
+      0x9700640064016c006d015a016d025a020100640064026c036d045a046d
+      055a056d065a060100640064036c076d085a080100640064046c096d0a5a
+      0a6d0b5a0b6d0c5a0c0100640064056c0d6d0e5a0e0100640064066c0f6d
+      105a100100640064076c116d125a120100640064086c136d145a14010064
+      0064096c156d165a1601006400640a6c176d185a1801006400640b6c195a
+      19640c640d6c1a6d1b5a1b6d1c5a1c6d1d5a1d6d1e5a1e0100640c640e6c
+      1f6d205a206d215a216d225a226d235a230100640c640f6c186d245a246d
+      255a250100020065046a260000000000000000a6000000ab000000000000
+      0000005a2764105a2864115a296412652a641365086414652a6415652a66
+      08641684045a2b020047006417840064186505a6030000ab030000000000
+      0000005a2c6527a02d000000000000000000000000000000000000000065
+      23ac19a6010000ab010000000000000000641a650a641b650b6604641c84
+      04a6000000ab0000000000000000005a2e6527a02f000000000000000000
+      0000000000000000000000641dac1ea6010000ab01000000000000000064
+      136508641f651d6415652a660664208404a6000000ab0000000000000000
+      005a306527a0310000000000000000000000000000000000000000642164
+      22641dac23a6030000ab03000000000000000064156532660264248404a6
+      000000ab0000000000000000005a336527a02f0000000000000000000000
+      00000000000000000064256426ac27a6020000ab02000000000000000064
+      2f6428652a6415652a660464298405a6000000ab0000000000000000005a
+      346430641a650a642a6535652a19000000000000000000642b6535652a19
+      000000000000000000642c6535652a19000000000000000000642d653265
+      2a650266021900000000000000000064156532660c642e84055a36640b53
+      00
      0           0 RESUME                   0
    
      1           2 LOAD_CONST               0 (0)
-                 4 LOAD_CONST               1 (('Type',))
+                 4 LOAD_CONST               1 (('Type', 'Any'))
                  6 IMPORT_NAME              0 (typing)
                  8 IMPORT_FROM              1 (Type)
                 10 STORE_NAME               1 (Type)
-                12 POP_TOP
-   
-     2          14 LOAD_CONST               0 (0)
-                16 LOAD_CONST               2 (('library', 'Node', 'TemplateSyntaxError'))
-                18 IMPORT_NAME              2 (django.template)
-                20 IMPORT_FROM              3 (library)
-                22 STORE_NAME               3 (library)
-                24 IMPORT_FROM              4 (Node)
-                26 STORE_NAME               4 (Node)
-                28 IMPORT_FROM              5 (TemplateSyntaxError)
-                30 STORE_NAME               5 (TemplateSyntaxError)
-                32 POP_TOP
-   
-     5          34 LOAD_CONST               0 (0)
-                36 LOAD_CONST               3 (('Context',))
-                38 IMPORT_NAME              6 (django.template.context)
-                40 IMPORT_FROM              7 (Context)
-                42 STORE_NAME               7 (Context)
-                44 POP_TOP
-   
-     8          46 LOAD_CONST               0 (0)
-                48 LOAD_CONST               4 (('Parser', 'Token', 'FilterExpression'))
-                50 IMPORT_NAME              8 (django.template.base)
-                52 IMPORT_FROM              9 (Parser)
-                54 STORE_NAME               9 (Parser)
-                56 IMPORT_FROM             10 (Token)
-                58 STORE_NAME              10 (Token)
-                60 IMPORT_FROM             11 (FilterExpression)
-                62 STORE_NAME              11 (FilterExpression)
-                64 POP_TOP
-   
-    12          66 LOAD_CONST               0 (0)
-                68 LOAD_CONST               5 (('HttpRequest',))
-                70 IMPORT_NAME             12 (django.http)
-                72 IMPORT_FROM             13 (HttpRequest)
-                74 STORE_NAME              13 (HttpRequest)
-                76 POP_TOP
-   
-    13          78 LOAD_CONST               0 (0)
-                80 LOAD_CONST               6 (('reverse',))
-                82 IMPORT_NAME             14 (django.urls)
-                84 IMPORT_FROM             15 (reverse)
-                86 STORE_NAME              15 (reverse)
-                88 POP_TOP
-   
-    14          90 LOAD_CONST               0 (0)
-                92 LOAD_CONST               7 (('signing',))
-                94 IMPORT_NAME             16 (django.core)
-                96 IMPORT_FROM             17 (signing)
-                98 STORE_NAME              17 (signing)
-               100 POP_TOP
-   
-    16         102 LOAD_CONST               0 (0)
-               104 LOAD_CONST               8 (('hooks',))
-               106 IMPORT_NAME             18 (wagtail)
-               108 IMPORT_FROM             19 (hooks)
-               110 STORE_NAME              19 (hooks)
-               112 POP_TOP
-   
-    18         114 LOAD_CONST               0 (0)
-               116 LOAD_CONST               9 (None)
-               118 IMPORT_NAME             20 (warnings)
-               120 STORE_NAME              20 (warnings)
-   
-    20         122 LOAD_CONST              10 (2)
-               124 LOAD_CONST              11 (('adapter_registry', 'RegistryLookUpError', 'BaseAdapter', 'AdapterError'))
-               126 IMPORT_NAME             21 (adapters)
-               128 IMPORT_FROM             22 (adapter_registry)
-               130 STORE_NAME              22 (adapter_registry)
-               132 IMPORT_FROM             23 (RegistryLookUpError)
-               134 STORE_NAME              23 (RegistryLookUpError)
-               136 IMPORT_FROM             24 (BaseAdapter)
-               138 STORE_NAME              24 (BaseAdapter)
-               140 IMPORT_FROM             25 (AdapterError)
-               142 STORE_NAME              25 (AdapterError)
-               144 POP_TOP
-   
-    26         146 LOAD_CONST              10 (2)
-               148 LOAD_CONST              12 (('wrap_adapter', '_can_edit', 'FEDIT_PREVIEW_VAR', 'TEMPLATE_TAG_NAME'))
-               150 IMPORT_NAME             26 (utils)
-               152 IMPORT_FROM             27 (wrap_adapter)
-               154 STORE_NAME              27 (wrap_adapter)
-               156 IMPORT_FROM             28 (_can_edit)
-               158 STORE_NAME              28 (_can_edit)
-               160 IMPORT_FROM             29 (FEDIT_PREVIEW_VAR)
-               162 STORE_NAME              29 (FEDIT_PREVIEW_VAR)
-               164 IMPORT_FROM             30 (TEMPLATE_TAG_NAME)
-               166 STORE_NAME              30 (TEMPLATE_TAG_NAME)
-               168 POP_TOP
-   
-    32         170 LOAD_CONST              10 (2)
-               172 LOAD_CONST              13 (('REGISTER_CSS', 'REGISTER_JS'))
-               174 IMPORT_NAME             19 (hooks)
-               176 IMPORT_FROM             31 (REGISTER_CSS)
-               178 STORE_NAME              31 (REGISTER_CSS)
-               180 IMPORT_FROM             32 (REGISTER_JS)
-               182 STORE_NAME              32 (REGISTER_JS)
-               184 POP_TOP
-   
-    38         186 PUSH_NULL
-               188 LOAD_NAME                3 (library)
-               190 LOAD_ATTR               33 (Library)
-               200 PRECALL                  0
-               204 CALL                     0
-               214 STORE_NAME              34 (register)
-   
-    41         216 LOAD_CONST              14 ('Field name is not available in the context for %(object)s.')
-               218 STORE_NAME              35 (WARNING_FIELD_NAME_NOT_AVAILABLE)
-   
-    42         220 LOAD_CONST              15 ('Model instance is not available in the context for %(object)s.')
-               222 STORE_NAME              36 (WARNING_MODEL_INSTANCE_NOT_AVAILABLE)
-   
-    45         224 LOAD_CONST              16 ('var')
-               226 LOAD_NAME               37 (str)
-               228 LOAD_CONST              17 ('context')
-               230 LOAD_NAME                7 (Context)
-               232 LOAD_CONST              18 ('value')
-               234 LOAD_NAME               37 (str)
-               236 LOAD_CONST              19 ('return')
-               238 LOAD_NAME               37 (str)
-               240 BUILD_TUPLE              8
-               242 LOAD_CONST              20 (<code object as_var, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Packages\wagtail_fedit\wagtail_fedit\templatetags\fedit.py", line 45>)
-               244 MAKE_FUNCTION            4 (annotations)
-               246 STORE_NAME              38 (as_var)
-   
-    52         248 PUSH_NULL
-               250 LOAD_BUILD_CLASS
-               252 LOAD_CONST              21 (<code object AdapterNode, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Packages\wagtail_fedit\wagtail_fedit\templatetags\fedit.py", line 52>)
-               254 MAKE_FUNCTION            0
-               256 LOAD_CONST              22 ('AdapterNode')
-               258 LOAD_NAME                4 (Node)
-               260 PRECALL                  3
-               264 CALL                     3
-               274 STORE_NAME              39 (AdapterNode)
-   
-   138         276 LOAD_NAME               34 (register)
-               278 LOAD_METHOD             40 (tag)
-               300 LOAD_NAME               30 (TEMPLATE_TAG_NAME)
-               302 KW_NAMES                23
-               304 PRECALL                  1
-               308 CALL                     1
-   
-   139         318 LOAD_CONST              24 ('parser')
-               320 LOAD_NAME                9 (Parser)
-               322 LOAD_CONST              25 ('token')
-               324 LOAD_NAME               10 (Token)
-               326 BUILD_TUPLE              4
-               328 LOAD_CONST              26 (<code object do_render_fedit, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Packages\wagtail_fedit\wagtail_fedit\templatetags\fedit.py", line 138>)
-               330 MAKE_FUNCTION            4 (annotations)
-   
-   138         332 PRECALL                  0
-               336 CALL                     0
-   
-   139         346 STORE_NAME              41 (do_render_fedit)
-   
-   195         348 LOAD_NAME               34 (register)
-               350 LOAD_METHOD             42 (simple_tag)
-               372 LOAD_CONST              27 (True)
-               374 KW_NAMES                28
-               376 PRECALL                  1
-               380 CALL                     1
-   
-   196         390 LOAD_CONST              17 ('context')
-               392 LOAD_NAME                7 (Context)
-               394 LOAD_CONST              29 ('adapter')
-               396 LOAD_NAME               24 (BaseAdapter)
-               398 LOAD_CONST              19 ('return')
-               400 LOAD_NAME               37 (str)
-               402 BUILD_TUPLE              6
-               404 LOAD_CONST              30 (<code object render_adapter, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Packages\wagtail_fedit\wagtail_fedit\templatetags\fedit.py", line 195>)
-               406 MAKE_FUNCTION            4 (annotations)
-   
-   195         408 PRECALL                  0
-               412 CALL                     0
-   
-   196         422 STORE_NAME              43 (render_adapter)
-   
-   212         424 LOAD_NAME               34 (register)
-               426 LOAD_METHOD             44 (inclusion_tag)
-               448 LOAD_CONST              31 ('wagtail_fedit/_hook_output.html')
-               450 LOAD_CONST              32 ('fedit_scripts')
-               452 LOAD_CONST              27 (True)
-               454 KW_NAMES                33
-               456 PRECALL                  3
-               460 CALL                     3
-   
-   213         470 LOAD_CONST              19 ('return')
-               472 LOAD_NAME               45 (dict)
-               474 BUILD_TUPLE              2
-               476 LOAD_CONST              34 (<code object static_hook_output, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Packages\wagtail_fedit\wagtail_fedit\templatetags\fedit.py", line 212>)
-               478 MAKE_FUNCTION            4 (annotations)
-   
-   212         480 PRECALL                  0
-               484 CALL                     0
-   
-   213         494 STORE_NAME              46 (static_hook_output)
-   
-   243         496 LOAD_CONST              39 ((None, None))
-               498 LOAD_CONST              24 ('parser')
-               500 LOAD_NAME                9 (Parser)
-               502 LOAD_CONST              35 ('tokens')
-               504 LOAD_NAME               47 (list)
-               506 LOAD_NAME               37 (str)
-               508 BINARY_SUBSCR
-               518 LOAD_CONST              36 ('kwarg_list')
-               520 LOAD_NAME               47 (list)
-               522 LOAD_NAME               37 (str)
-               524 BINARY_SUBSCR
-               534 LOAD_CONST              37 ('absolute_tokens')
-               536 LOAD_NAME               47 (list)
-               538 LOAD_NAME               37 (str)
-               540 BINARY_SUBSCR
-               550 LOAD_CONST              19 ('return')
-               552 LOAD_NAME               45 (dict)
-               554 BUILD_TUPLE             10
-               556 LOAD_CONST              38 (<code object get_kwargs, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Packages\wagtail_fedit\wagtail_fedit\templatetags\fedit.py", line 243>)
-               558 MAKE_FUNCTION            5 (defaults, annotations)
-               560 STORE_NAME              48 (get_kwargs)
-               562 LOAD_CONST               9 (None)
-               564 RETURN_VALUE
+                12 IMPORT_FROM              2 (Any)
+                14 STORE_NAME               2 (Any)
+                16 POP_TOP
+   
+     2          18 LOAD_CONST               0 (0)
+                20 LOAD_CONST               2 (('library', 'Node', 'TemplateSyntaxError'))
+                22 IMPORT_NAME              3 (django.template)
+                24 IMPORT_FROM              4 (library)
+                26 STORE_NAME               4 (library)
+                28 IMPORT_FROM              5 (Node)
+                30 STORE_NAME               5 (Node)
+                32 IMPORT_FROM              6 (TemplateSyntaxError)
+                34 STORE_NAME               6 (TemplateSyntaxError)
+                36 POP_TOP
+   
+     5          38 LOAD_CONST               0 (0)
+                40 LOAD_CONST               3 (('Context',))
+                42 IMPORT_NAME              7 (django.template.context)
+                44 IMPORT_FROM              8 (Context)
+                46 STORE_NAME               8 (Context)
+                48 POP_TOP
+   
+     8          50 LOAD_CONST               0 (0)
+                52 LOAD_CONST               4 (('Parser', 'Token', 'FilterExpression'))
+                54 IMPORT_NAME              9 (django.template.base)
+                56 IMPORT_FROM             10 (Parser)
+                58 STORE_NAME              10 (Parser)
+                60 IMPORT_FROM             11 (Token)
+                62 STORE_NAME              11 (Token)
+                64 IMPORT_FROM             12 (FilterExpression)
+                66 STORE_NAME              12 (FilterExpression)
+                68 POP_TOP
+   
+    12          70 LOAD_CONST               0 (0)
+                72 LOAD_CONST               5 (('HttpRequest',))
+                74 IMPORT_NAME             13 (django.http)
+                76 IMPORT_FROM             14 (HttpRequest)
+                78 STORE_NAME              14 (HttpRequest)
+                80 POP_TOP
+   
+    13          82 LOAD_CONST               0 (0)
+                84 LOAD_CONST               6 (('escape',))
+                86 IMPORT_NAME             15 (django.utils.html)
+                88 IMPORT_FROM             16 (escape)
+                90 STORE_NAME              16 (escape)
+                92 POP_TOP
+   
+    14          94 LOAD_CONST               0 (0)
+                96 LOAD_CONST               7 (('mark_safe',))
+                98 IMPORT_NAME             17 (django.utils.safestring)
+               100 IMPORT_FROM             18 (mark_safe)
+               102 STORE_NAME              18 (mark_safe)
+               104 POP_TOP
+   
+    15         106 LOAD_CONST               0 (0)
+               108 LOAD_CONST               8 (('reverse',))
+               110 IMPORT_NAME             19 (django.urls)
+               112 IMPORT_FROM             20 (reverse)
+               114 STORE_NAME              20 (reverse)
+               116 POP_TOP
+   
+    16         118 LOAD_CONST               0 (0)
+               120 LOAD_CONST               9 (('signing',))
+               122 IMPORT_NAME             21 (django.core)
+               124 IMPORT_FROM             22 (signing)
+               126 STORE_NAME              22 (signing)
+               128 POP_TOP
+   
+    18         130 LOAD_CONST               0 (0)
+               132 LOAD_CONST              10 (('hooks',))
+               134 IMPORT_NAME             23 (wagtail)
+               136 IMPORT_FROM             24 (hooks)
+               138 STORE_NAME              24 (hooks)
+               140 POP_TOP
+   
+    20         142 LOAD_CONST               0 (0)
+               144 LOAD_CONST              11 (None)
+               146 IMPORT_NAME             25 (warnings)
+               148 STORE_NAME              25 (warnings)
+   
+    22         150 LOAD_CONST              12 (2)
+               152 LOAD_CONST              13 (('adapter_registry', 'RegistryLookUpError', 'BaseAdapter', 'AdapterError'))
+               154 IMPORT_NAME             26 (adapters)
+               156 IMPORT_FROM             27 (adapter_registry)
+               158 STORE_NAME              27 (adapter_registry)
+               160 IMPORT_FROM             28 (RegistryLookUpError)
+               162 STORE_NAME              28 (RegistryLookUpError)
+               164 IMPORT_FROM             29 (BaseAdapter)
+               166 STORE_NAME              29 (BaseAdapter)
+               168 IMPORT_FROM             30 (AdapterError)
+               170 STORE_NAME              30 (AdapterError)
+               172 POP_TOP
+   
+    28         174 LOAD_CONST              12 (2)
+               176 LOAD_CONST              14 (('wrap_adapter', '_can_edit', 'FEDIT_PREVIEW_VAR', 'TEMPLATE_TAG_NAME'))
+               178 IMPORT_NAME             31 (utils)
+               180 IMPORT_FROM             32 (wrap_adapter)
+               182 STORE_NAME              32 (wrap_adapter)
+               184 IMPORT_FROM             33 (_can_edit)
+               186 STORE_NAME              33 (_can_edit)
+               188 IMPORT_FROM             34 (FEDIT_PREVIEW_VAR)
+               190 STORE_NAME              34 (FEDIT_PREVIEW_VAR)
+               192 IMPORT_FROM             35 (TEMPLATE_TAG_NAME)
+               194 STORE_NAME              35 (TEMPLATE_TAG_NAME)
+               196 POP_TOP
+   
+    34         198 LOAD_CONST              12 (2)
+               200 LOAD_CONST              15 (('REGISTER_CSS', 'REGISTER_JS'))
+               202 IMPORT_NAME             24 (hooks)
+               204 IMPORT_FROM             36 (REGISTER_CSS)
+               206 STORE_NAME              36 (REGISTER_CSS)
+               208 IMPORT_FROM             37 (REGISTER_JS)
+               210 STORE_NAME              37 (REGISTER_JS)
+               212 POP_TOP
+   
+    40         214 PUSH_NULL
+               216 LOAD_NAME                4 (library)
+               218 LOAD_ATTR               38 (Library)
+               228 PRECALL                  0
+               232 CALL                     0
+               242 STORE_NAME              39 (register)
+   
+    43         244 LOAD_CONST              16 ('Field name is not available in the context for %(object)s.')
+               246 STORE_NAME              40 (WARNING_FIELD_NAME_NOT_AVAILABLE)
+   
+    44         248 LOAD_CONST              17 ('Model instance is not available in the context for %(object)s.')
+               250 STORE_NAME              41 (WARNING_MODEL_INSTANCE_NOT_AVAILABLE)
+   
+    47         252 LOAD_CONST              18 ('var')
+               254 LOAD_NAME               42 (str)
+               256 LOAD_CONST              19 ('context')
+               258 LOAD_NAME                8 (Context)
+               260 LOAD_CONST              20 ('value')
+               262 LOAD_NAME               42 (str)
+               264 LOAD_CONST              21 ('return')
+               266 LOAD_NAME               42 (str)
+               268 BUILD_TUPLE              8
+               270 LOAD_CONST              22 (<code object as_var, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 47>)
+               272 MAKE_FUNCTION            4 (annotations)
+               274 STORE_NAME              43 (as_var)
+   
+    54         276 PUSH_NULL
+               278 LOAD_BUILD_CLASS
+               280 LOAD_CONST              23 (<code object AdapterNode, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 54>)
+               282 MAKE_FUNCTION            0
+               284 LOAD_CONST              24 ('AdapterNode')
+               286 LOAD_NAME                5 (Node)
+               288 PRECALL                  3
+               292 CALL                     3
+               302 STORE_NAME              44 (AdapterNode)
+   
+   140         304 LOAD_NAME               39 (register)
+               306 LOAD_METHOD             45 (tag)
+               328 LOAD_NAME               35 (TEMPLATE_TAG_NAME)
+               330 KW_NAMES                25
+               332 PRECALL                  1
+               336 CALL                     1
+   
+   141         346 LOAD_CONST              26 ('parser')
+               348 LOAD_NAME               10 (Parser)
+               350 LOAD_CONST              27 ('token')
+               352 LOAD_NAME               11 (Token)
+               354 BUILD_TUPLE              4
+               356 LOAD_CONST              28 (<code object do_render_fedit, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 140>)
+               358 MAKE_FUNCTION            4 (annotations)
+   
+   140         360 PRECALL                  0
+               364 CALL                     0
+   
+   141         374 STORE_NAME              46 (do_render_fedit)
+   
+   198         376 LOAD_NAME               39 (register)
+               378 LOAD_METHOD             47 (simple_tag)
+               400 LOAD_CONST              29 (True)
+               402 KW_NAMES                30
+               404 PRECALL                  1
+               408 CALL                     1
+   
+   199         418 LOAD_CONST              19 ('context')
+               420 LOAD_NAME                8 (Context)
+               422 LOAD_CONST              31 ('adapter')
+               424 LOAD_NAME               29 (BaseAdapter)
+               426 LOAD_CONST              21 ('return')
+               428 LOAD_NAME               42 (str)
+               430 BUILD_TUPLE              6
+               432 LOAD_CONST              32 (<code object render_adapter, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 198>)
+               434 MAKE_FUNCTION            4 (annotations)
+   
+   198         436 PRECALL                  0
+               440 CALL                     0
+   
+   199         450 STORE_NAME              48 (render_adapter)
+   
+   215         452 LOAD_NAME               39 (register)
+               454 LOAD_METHOD             49 (inclusion_tag)
+               476 LOAD_CONST              33 ('wagtail_fedit/_hook_output.html')
+               478 LOAD_CONST              34 ('fedit_scripts')
+               480 LOAD_CONST              29 (True)
+               482 KW_NAMES                35
+               484 PRECALL                  3
+               488 CALL                     3
+   
+   216         498 LOAD_CONST              21 ('return')
+               500 LOAD_NAME               50 (dict)
+               502 BUILD_TUPLE              2
+               504 LOAD_CONST              36 (<code object static_hook_output, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 215>)
+               506 MAKE_FUNCTION            4 (annotations)
+   
+   215         508 PRECALL                  0
+               512 CALL                     0
+   
+   216         522 STORE_NAME              51 (static_hook_output)
+   
+   245         524 LOAD_NAME               39 (register)
+               526 LOAD_METHOD             47 (simple_tag)
+               548 LOAD_CONST              37 (False)
+               550 LOAD_CONST              38 ('tooltip')
+               552 KW_NAMES                39
+               554 PRECALL                  2
+               558 CALL                     2
+   
+   246         568 LOAD_CONST              47 ((None,))
+               570 LOAD_CONST              40 ('wrapping')
+               572 LOAD_NAME               42 (str)
+               574 LOAD_CONST              21 ('return')
+               576 LOAD_NAME               42 (str)
+               578 BUILD_TUPLE              4
+               580 LOAD_CONST              41 (<code object tooltip, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 245>)
+               582 MAKE_FUNCTION            5 (defaults, annotations)
+   
+   245         584 PRECALL                  0
+               588 CALL                     0
+   
+   246         598 STORE_NAME              52 (tooltip)
+   
+   261         600 LOAD_CONST              48 ((None, None, None))
+               602 LOAD_CONST              26 ('parser')
+               604 LOAD_NAME               10 (Parser)
+               606 LOAD_CONST              42 ('tokens')
+               608 LOAD_NAME               53 (list)
+               610 LOAD_NAME               42 (str)
+               612 BINARY_SUBSCR
+               622 LOAD_CONST              43 ('kwarg_list')
+               624 LOAD_NAME               53 (list)
+               626 LOAD_NAME               42 (str)
+               628 BINARY_SUBSCR
+               638 LOAD_CONST              44 ('absolute_tokens')
+               640 LOAD_NAME               53 (list)
+               642 LOAD_NAME               42 (str)
+               644 BINARY_SUBSCR
+               654 LOAD_CONST              45 ('optional_tokens')
+               656 LOAD_NAME               50 (dict)
+               658 LOAD_NAME               42 (str)
+               660 LOAD_NAME                2 (Any)
+               662 BUILD_TUPLE              2
+               664 BINARY_SUBSCR
+               674 LOAD_CONST              21 ('return')
+               676 LOAD_NAME               50 (dict)
+               678 BUILD_TUPLE             12
+               680 LOAD_CONST              46 (<code object get_kwargs, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 261>)
+               682 MAKE_FUNCTION            5 (defaults, annotations)
+               684 STORE_NAME              54 (get_kwargs)
+               686 LOAD_CONST              11 (None)
+               688 RETURN_VALUE
    consts
       0
-      ('Type',)
+      ('Type', 'Any')
       ('library', 'Node', 'TemplateSyntaxError')
       ('Context',)
       ('Parser', 'Token', 'FilterExpression')
       ('HttpRequest',)
+      ('escape',)
+      ('mark_safe',)
       ('reverse',)
       ('signing',)
       ('hooks',)
       None
       2
       ('adapter_registry', 'RegistryLookUpError', 'BaseAdapter', 'AdapterError')
       ('wrap_adapter', '_can_edit', 'FEDIT_PREVIEW_VAR', 'TEMPLATE_TAG_NAME')
@@ -276,86 +327,86 @@
       'return'
       code
          argcount  : 3
          nlocals   : 3
          stacksize : 3
          flags     : 3
          code 0x97007c0073027c0253007c027c017c003c00000064015300
-          45           0 RESUME                   0
+          47           0 RESUME                   0
          
-          46           2 LOAD_FAST                0 (var)
+          48           2 LOAD_FAST                0 (var)
                        4 POP_JUMP_FORWARD_IF_TRUE     2 (to 10)
          
-          47           6 LOAD_FAST                2 (value)
+          49           6 LOAD_FAST                2 (value)
                        8 RETURN_VALUE
          
-          49     >>   10 LOAD_FAST                2 (value)
+          51     >>   10 LOAD_FAST                2 (value)
                       12 LOAD_FAST                1 (context)
                       14 LOAD_FAST                0 (var)
                       16 STORE_SUBSCR
          
-          50          20 LOAD_CONST               1 ('')
+          52          20 LOAD_CONST               1 ('')
                       22 RETURN_VALUE
          consts
             None
             ''
          names      ()
          varnames   ('var', 'context', 'value')
          freevars   ()
          cellvars   ()
-         filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Packages\\wagtail_fedit\\wagtail_fedit\\templatetags\\fedit.py'
+         filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\tester\\wagtail_fedit\\templatetags\\fedit.py'
          name       'as_var'
-         firstlineno 45
+         firstlineno 47
          lnotab 0x0201040104020a01
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 9
          flags     : 0
          code
             0x970065005a0164005a02020065036a040000000000000000a6000000ab
             0000000000000000005a0564096402650665071900000000000000000064
             03650864046509650a190000000000000000006405650a6608640684055a
             0b640784005a0c640884005a0d64015300
-          52           0 RESUME                   0
+          54           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('AdapterNode')
                        8 STORE_NAME               2 (__qualname__)
          
-          53          10 PUSH_NULL
+          55          10 PUSH_NULL
                       12 LOAD_NAME                3 (signing)
                       14 LOAD_ATTR                4 (TimestampSigner)
                       24 PRECALL                  0
                       28 CALL                     0
                       38 STORE_NAME               5 (signer)
          
-          55          40 LOAD_CONST               9 ((None,))
+          57          40 LOAD_CONST               9 ((None,))
                       42 LOAD_CONST               2 ('adapter')
                       44 LOAD_NAME                6 (Type)
                       46 LOAD_NAME                7 (BaseAdapter)
                       48 BINARY_SUBSCR
                       58 LOAD_CONST               3 ('model')
                       60 LOAD_NAME                8 (FilterExpression)
                       62 LOAD_CONST               4 ('getters')
                       64 LOAD_NAME                9 (list)
                       66 LOAD_NAME               10 (str)
                       68 BINARY_SUBSCR
                       78 LOAD_CONST               5 ('as_var')
                       80 LOAD_NAME               10 (str)
                       82 BUILD_TUPLE              8
-                      84 LOAD_CONST               6 (<code object __init__, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Packages\wagtail_fedit\wagtail_fedit\templatetags\fedit.py", line 55>)
+                      84 LOAD_CONST               6 (<code object __init__, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 57>)
                       86 MAKE_FUNCTION            5 (defaults, annotations)
                       88 STORE_NAME              11 (__init__)
          
-          62          90 LOAD_CONST               7 (<code object _resolve_expressions, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Packages\wagtail_fedit\wagtail_fedit\templatetags\fedit.py", line 62>)
+          64          90 LOAD_CONST               7 (<code object _resolve_expressions, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 64>)
                       92 MAKE_FUNCTION            0
                       94 STORE_NAME              12 (_resolve_expressions)
          
-          72          96 LOAD_CONST               8 (<code object render, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Packages\wagtail_fedit\wagtail_fedit\templatetags\fedit.py", line 72>)
+          74          96 LOAD_CONST               8 (<code object render, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 74>)
                       98 MAKE_FUNCTION            0
                      100 STORE_NAME              13 (render)
                      102 LOAD_CONST               1 (None)
                      104 RETURN_VALUE
          consts
             'AdapterNode'
             None
@@ -368,46 +419,46 @@
                nlocals   : 6
                stacksize : 2
                flags     : 11
                code
                   0x97007c017c005f0000000000000000007c027c005f0100000000000000
                   007c037c005f0200000000000000007c057c005f0300000000000000007c
                   047c005f04000000000000000064005300
-                55           0 RESUME                   0
+                57           0 RESUME                   0
                
-                56           2 LOAD_FAST                1 (adapter)
+                58           2 LOAD_FAST                1 (adapter)
                              4 LOAD_FAST                0 (self)
                              6 STORE_ATTR               0 (adapter)
                
-                57          16 LOAD_FAST                2 (model)
+                59          16 LOAD_FAST                2 (model)
                             18 LOAD_FAST                0 (self)
                             20 STORE_ATTR               1 (model)
                
-                58          30 LOAD_FAST                3 (getters)
+                60          30 LOAD_FAST                3 (getters)
                             32 LOAD_FAST                0 (self)
                             34 STORE_ATTR               2 (getters)
                
-                59          44 LOAD_FAST                5 (kwargs)
+                61          44 LOAD_FAST                5 (kwargs)
                             46 LOAD_FAST                0 (self)
                             48 STORE_ATTR               3 (kwargs)
                
-                60          58 LOAD_FAST                4 (as_var)
+                62          58 LOAD_FAST                4 (as_var)
                             60 LOAD_FAST                0 (self)
                             62 STORE_ATTR               4 (as_var)
                             72 LOAD_CONST               0 (None)
                             74 RETURN_VALUE
                consts
                   None
                names      ('adapter', 'model', 'getters', 'kwargs', 'as_var')
                varnames   ('self', 'adapter', 'model', 'getters', 'as_var', 'kwargs')
                freevars   ()
                cellvars   ()
-               filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Packages\\wagtail_fedit\\wagtail_fedit\\templatetags\\fedit.py'
+               filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\tester\\wagtail_fedit\\templatetags\\fedit.py'
                name       '__init__'
-               firstlineno 55
+               firstlineno 57
                lnotab 0x02010e010e010e010e01
             code
                argcount  : 3
                nlocals   : 6
                stacksize : 5
                flags     : 11
                code
@@ -415,70 +466,70 @@
                   00ab00000000000000000044005d325c0200007d047d0574030000000000
                   00000000007c05740400000000000000000000a6020000ab020000000000
                   00000072187c05a00300000000000000000000000000000000000000007c
                   01a6010000ab0100000000000000007c037c043c0000008c337403000000
                   000000000000007c02740400000000000000000000a6020000ab02000000
                   000000000072157c02a00300000000000000000000000000000000000000
                   007c01a6010000ab0100000000000000007d027c027c0366025300
-                62           0 RESUME                   0
+                64           0 RESUME                   0
                
-                63           2 LOAD_FAST                3 (kwargs)
+                65           2 LOAD_FAST                3 (kwargs)
                              4 LOAD_METHOD              0 (items)
                             26 PRECALL                  0
                             30 CALL                     0
                             40 GET_ITER
                        >>   42 FOR_ITER                50 (to 144)
                             44 UNPACK_SEQUENCE          2
                             48 STORE_FAST               4 (k)
                             50 STORE_FAST               5 (v)
                
-                64          52 LOAD_GLOBAL              3 (NULL + isinstance)
+                66          52 LOAD_GLOBAL              3 (NULL + isinstance)
                             64 LOAD_FAST                5 (v)
                             66 LOAD_GLOBAL              4 (FilterExpression)
                             78 PRECALL                  2
                             82 CALL                     2
                             92 POP_JUMP_FORWARD_IF_FALSE    24 (to 142)
                
-                65          94 LOAD_FAST                5 (v)
+                67          94 LOAD_FAST                5 (v)
                             96 LOAD_METHOD              3 (resolve)
                            118 LOAD_FAST                1 (context)
                            120 PRECALL                  1
                            124 CALL                     1
                            134 LOAD_FAST                3 (kwargs)
                            136 LOAD_FAST                4 (k)
                            138 STORE_SUBSCR
                        >>  142 JUMP_BACKWARD           51 (to 42)
                
-                67     >>  144 LOAD_GLOBAL              3 (NULL + isinstance)
+                69     >>  144 LOAD_GLOBAL              3 (NULL + isinstance)
                            156 LOAD_FAST                2 (model)
                            158 LOAD_GLOBAL              4 (FilterExpression)
                            170 PRECALL                  2
                            174 CALL                     2
                            184 POP_JUMP_FORWARD_IF_FALSE    21 (to 228)
                
-                68         186 LOAD_FAST                2 (model)
+                70         186 LOAD_FAST                2 (model)
                            188 LOAD_METHOD              3 (resolve)
                            210 LOAD_FAST                1 (context)
                            212 PRECALL                  1
                            216 CALL                     1
                            226 STORE_FAST               2 (model)
                
-                70     >>  228 LOAD_FAST                2 (model)
+                72     >>  228 LOAD_FAST                2 (model)
                            230 LOAD_FAST                3 (kwargs)
                            232 BUILD_TUPLE              2
                            234 RETURN_VALUE
                consts
                   None
                names      ('items', 'isinstance', 'FilterExpression', 'resolve')
                varnames   ('self', 'context', 'model', 'kwargs', 'k', 'v')
                freevars   ()
                cellvars   ()
-               filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Packages\\wagtail_fedit\\wagtail_fedit\\templatetags\\fedit.py'
+               filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\tester\\wagtail_fedit\\templatetags\\fedit.py'
                name       '_resolve_expressions'
-               firstlineno 62
+               firstlineno 64
                lnotab 0x020132012a0132022a012a02
             code
                argcount  : 2
                nlocals   : 12
                stacksize : 9
                flags     : 3
                code
@@ -515,299 +566,299 @@
                   0000000000000072107431000000000000000000007c0a7c06a6020000ab
                   02000000000000000073297419000000000000000000007c006a0c000000
                   00000000007c017c0ba01900000000000000000000000000000000000000
                   007c01a6010000ab010000000000000000a6030000ab0300000000000000
                   0053007419000000000000000000007c006a0c00000000000000007c0174
                   35000000000000000000007c0a7c0b7c01a6030000ab0300000000000000
                   00a6030000ab0300000000000000005300
-                72           0 RESUME                   0
+                74           0 RESUME                   0
                
-                73           2 LOAD_FAST                0 (self)
+                75           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (model)
                             14 STORE_FAST               2 (model)
                
-                74          16 LOAD_FAST                0 (self)
+                76          16 LOAD_FAST                0 (self)
                             18 LOAD_ATTR                1 (getters)
                             28 STORE_FAST               3 (getters)
                
-                76          30 PUSH_NULL
+                78          30 PUSH_NULL
                             32 LOAD_FAST                0 (self)
                             34 LOAD_ATTR                2 (_resolve_expressions)
                
-                77          44 LOAD_FAST                1 (context)
+                79          44 LOAD_FAST                1 (context)
                             46 LOAD_FAST                2 (model)
                
-                76          48 BUILD_TUPLE              2
+                78          48 BUILD_TUPLE              2
                             50 BUILD_MAP                0
                
-                77          52 LOAD_FAST                0 (self)
+                79          52 LOAD_FAST                0 (self)
                             54 LOAD_ATTR                3 (kwargs)
                
-                76          64 DICT_MERGE               1
+                78          64 DICT_MERGE               1
                             66 CALL_FUNCTION_EX         1
                             68 UNPACK_SEQUENCE          2
                             72 STORE_FAST               2 (model)
                             74 STORE_FAST               4 (kwargs)
                
-                80          76 LOAD_CONST               1 ('wagtail_fedit_field')
+                82          76 LOAD_CONST               1 ('wagtail_fedit_field')
                             78 LOAD_FAST                1 (context)
                             80 CONTAINS_OP              0
                             82 POP_JUMP_FORWARD_IF_FALSE    36 (to 156)
                
-                81          84 LOAD_CONST               2 ('wagtail_fedit_instance')
+                83          84 LOAD_CONST               2 ('wagtail_fedit_instance')
                             86 LOAD_FAST                1 (context)
                             88 CONTAINS_OP              0
                             90 POP_JUMP_FORWARD_IF_FALSE    32 (to 156)
                
-                82          92 LOAD_FAST                2 (model)
+                84          92 LOAD_FAST                2 (model)
                
-                81          94 POP_JUMP_FORWARD_IF_TRUE    30 (to 156)
+                83          94 POP_JUMP_FORWARD_IF_TRUE    30 (to 156)
                
-                82          96 LOAD_FAST                0 (self)
+                84          96 LOAD_FAST                0 (self)
                             98 LOAD_ATTR                4 (adapter)
                            108 LOAD_ATTR                5 (field_required)
                
-                81         118 POP_JUMP_FORWARD_IF_FALSE    18 (to 156)
+                83         118 POP_JUMP_FORWARD_IF_FALSE    18 (to 156)
                
-                84         120 LOAD_FAST                1 (context)
+                86         120 LOAD_FAST                1 (context)
                            122 LOAD_CONST               1 ('wagtail_fedit_field')
                            124 BINARY_SUBSCR
                            134 STORE_FAST               5 (field_name)
                
-                85         136 LOAD_FAST                1 (context)
+                87         136 LOAD_FAST                1 (context)
                            138 LOAD_CONST               2 ('wagtail_fedit_instance')
                            140 BINARY_SUBSCR
                            150 STORE_FAST               6 (obj)
                            152 EXTENDED_ARG             1
                            154 JUMP_FORWARD           318 (to 792)
                
-                87     >>  156 LOAD_FAST                2 (model)
+                89     >>  156 LOAD_FAST                2 (model)
                            158 POP_JUMP_FORWARD_IF_TRUE    28 (to 216)
                            160 LOAD_CONST               2 ('wagtail_fedit_instance')
                            162 LOAD_FAST                1 (context)
                            164 CONTAINS_OP              0
                            166 POP_JUMP_FORWARD_IF_FALSE    24 (to 216)
                            168 LOAD_FAST                0 (self)
                            170 LOAD_ATTR                4 (adapter)
                            180 LOAD_ATTR                5 (field_required)
                            190 POP_JUMP_FORWARD_IF_TRUE    12 (to 216)
                
-                88         192 LOAD_FAST                1 (context)
+                90         192 LOAD_FAST                1 (context)
                            194 LOAD_CONST               2 ('wagtail_fedit_instance')
                            196 BINARY_SUBSCR
                            206 STORE_FAST               6 (obj)
                
-                89         208 LOAD_CONST               0 (None)
+                91         208 LOAD_CONST               0 (None)
                            210 STORE_FAST               5 (field_name)
                            212 EXTENDED_ARG             1
                            214 JUMP_FORWARD           288 (to 792)
                
-                93     >>  216 LOAD_FAST                2 (model)
+                95     >>  216 LOAD_FAST                2 (model)
                            218 POP_JUMP_FORWARD_IF_TRUE   152 (to 524)
                
-                94         220 LOAD_GLOBAL             13 (NULL + warnings)
+                96         220 LOAD_GLOBAL             13 (NULL + warnings)
                            232 LOAD_ATTR                7 (warn)
                
-                95         242 LOAD_GLOBAL             16 (WARNING_MODEL_INSTANCE_NOT_AVAILABLE)
+                97         242 LOAD_GLOBAL             16 (WARNING_MODEL_INSTANCE_NOT_AVAILABLE)
                
-                96         254 LOAD_CONST               3 ('object')
+                98         254 LOAD_CONST               3 ('object')
                            256 LOAD_FAST                0 (self)
                            258 LOAD_ATTR                4 (adapter)
                            268 LOAD_ATTR                9 (__name__)
                
-                95         278 BUILD_MAP                1
+                97         278 BUILD_MAP                1
                            280 BINARY_OP                6 (%)
                
-                98         284 LOAD_GLOBAL             20 (RuntimeWarning)
+               100         284 LOAD_GLOBAL             20 (RuntimeWarning)
                
-                94         296 PRECALL                  2
+                96         296 PRECALL                  2
                            300 CALL                     2
                            310 POP_TOP
                
-               101         312 LOAD_FAST                1 (context)
+               103         312 LOAD_FAST                1 (context)
                            314 LOAD_METHOD             11 (flatten)
                            336 PRECALL                  0
                            340 CALL                     0
                            350 STORE_FAST               1 (context)
                
-               103         352 NOP
+               105         352 NOP
                
-               104         354 LOAD_GLOBAL             25 (NULL + as_var)
+               106         354 LOAD_GLOBAL             25 (NULL + as_var)
                            366 LOAD_FAST                0 (self)
                            368 LOAD_ATTR               12 (as_var)
                            378 LOAD_FAST                1 (context)
                            380 PUSH_NULL
                            382 LOAD_FAST                0 (self)
                            384 LOAD_ATTR                4 (adapter)
                            394 LOAD_ATTR               13 (render_from_kwargs)
                
-               105         404 LOAD_FAST                1 (context)
+               107         404 LOAD_FAST                1 (context)
                
-               104         406 BUILD_TUPLE              1
+               106         406 BUILD_TUPLE              1
                            408 BUILD_MAP                0
                
-               105         410 LOAD_FAST                4 (kwargs)
+               107         410 LOAD_FAST                4 (kwargs)
                
-               104         412 DICT_MERGE               1
+               106         412 DICT_MERGE               1
                            414 CALL_FUNCTION_EX         1
                            416 PRECALL                  3
                            420 CALL                     3
                            430 RETURN_VALUE
                        >>  432 PUSH_EXC_INFO
                
-               107         434 LOAD_GLOBAL             28 (AdapterError)
+               109         434 LOAD_GLOBAL             28 (AdapterError)
                            446 CHECK_EXC_MATCH
                            448 POP_JUMP_FORWARD_IF_FALSE    33 (to 516)
                            450 STORE_FAST               7 (e)
                
-               108         452 LOAD_GLOBAL             31 (NULL + TemplateSyntaxError)
+               110         452 LOAD_GLOBAL             31 (NULL + TemplateSyntaxError)
                            464 LOAD_GLOBAL             33 (NULL + str)
                            476 LOAD_FAST                7 (e)
                            478 PRECALL                  1
                            482 CALL                     1
                            492 PRECALL                  1
                            496 CALL                     1
                            506 RAISE_VARARGS            1
                        >>  508 LOAD_CONST               0 (None)
                            510 STORE_FAST               7 (e)
                            512 DELETE_FAST              7 (e)
                            514 RERAISE                  1
                
-               107     >>  516 RERAISE                  0
+               109     >>  516 RERAISE                  0
                        >>  518 COPY                     3
                            520 POP_EXCEPT
                            522 RERAISE                  1
                
-               110     >>  524 LOAD_CONST               0 (None)
+               112     >>  524 LOAD_CONST               0 (None)
                            526 STORE_FAST               5 (field_name)
                
-               111         528 LOAD_FAST                2 (model)
+               113         528 LOAD_FAST                2 (model)
                            530 STORE_FAST               6 (obj)
                
-               112         532 LOAD_FAST                3 (getters)
+               114         532 LOAD_FAST                3 (getters)
                            534 POP_JUMP_FORWARD_IF_FALSE   128 (to 792)
                
-               113         536 LOAD_FAST                3 (getters)
+               115         536 LOAD_FAST                3 (getters)
                            538 LOAD_GLOBAL             35 (NULL + len)
                            550 LOAD_FAST                3 (getters)
                            552 PRECALL                  1
                            556 CALL                     1
                            566 LOAD_CONST               4 (1)
                            568 BINARY_OP               10 (-)
                            572 BINARY_SUBSCR
                            582 STORE_FAST               5 (field_name)
                
-               115         584 LOAD_GLOBAL             37 (NULL + range)
+               117         584 LOAD_GLOBAL             37 (NULL + range)
                            596 LOAD_GLOBAL             35 (NULL + len)
                            608 LOAD_FAST                3 (getters)
                            610 PRECALL                  1
                            614 CALL                     1
                            624 LOAD_CONST               4 (1)
                            626 BINARY_OP               10 (-)
                            630 PRECALL                  1
                            634 CALL                     1
                            644 GET_ITER
                        >>  646 FOR_ITER                72 (to 792)
                            648 STORE_FAST               8 (i)
                
-               116         650 LOAD_FAST                3 (getters)
+               118         650 LOAD_FAST                3 (getters)
                            652 LOAD_FAST                8 (i)
                            654 BINARY_SUBSCR
                            664 STORE_FAST               9 (getter)
                
-               117         666 NOP
+               119         666 NOP
                
-               118         668 LOAD_GLOBAL             39 (NULL + getattr)
+               120         668 LOAD_GLOBAL             39 (NULL + getattr)
                            680 LOAD_FAST                6 (obj)
                            682 LOAD_FAST                9 (getter)
                            684 PRECALL                  2
                            688 CALL                     2
                            698 STORE_FAST               6 (obj)
                            700 JUMP_BACKWARD           28 (to 646)
                        >>  702 PUSH_EXC_INFO
                
-               119         704 LOAD_GLOBAL             40 (AttributeError)
+               121         704 LOAD_GLOBAL             40 (AttributeError)
                            716 CHECK_EXC_MATCH
                            718 POP_JUMP_FORWARD_IF_FALSE    32 (to 784)
                            720 POP_TOP
                
-               120         722 LOAD_GLOBAL             41 (NULL + AttributeError)
+               122         722 LOAD_GLOBAL             41 (NULL + AttributeError)
                            734 LOAD_CONST               5 ('Object ')
                            736 LOAD_FAST                2 (model)
                            738 LOAD_ATTR               21 (__class__)
                            748 LOAD_ATTR                9 (__name__)
                            758 FORMAT_VALUE             0
                            760 LOAD_CONST               6 (' does not have attribute ')
                            762 LOAD_FAST                9 (getter)
                            764 FORMAT_VALUE             0
                            766 BUILD_STRING             4
                            768 PRECALL                  1
                            772 CALL                     1
                            782 RAISE_VARARGS            1
                
-               119     >>  784 RERAISE                  0
+               121     >>  784 RERAISE                  0
                        >>  786 COPY                     3
                            788 POP_EXCEPT
                            790 RERAISE                  1
                
-               123     >>  792 LOAD_FAST                1 (context)
+               125     >>  792 LOAD_FAST                1 (context)
                            794 LOAD_METHOD             22 (get)
                            816 LOAD_CONST               7 ('request')
                            818 PRECALL                  1
                            822 CALL                     1
                            832 STORE_FAST              10 (request)
                
-               124         834 PUSH_NULL
+               126         834 PUSH_NULL
                            836 LOAD_FAST                0 (self)
                            838 LOAD_ATTR                4 (adapter)
                            848 LOAD_CONST               9 (())
                
-               125         850 LOAD_FAST                6 (obj)
+               127         850 LOAD_FAST                6 (obj)
                
-               126         852 LOAD_FAST                5 (field_name)
+               128         852 LOAD_FAST                5 (field_name)
                
-               127         854 LOAD_FAST               10 (request)
+               129         854 LOAD_FAST               10 (request)
                
-               124         856 LOAD_CONST               8 (('object', 'field_name', 'request'))
+               126         856 LOAD_CONST               8 (('object', 'field_name', 'request'))
                            858 BUILD_CONST_KEY_MAP      3
                
-               128         860 LOAD_FAST                4 (kwargs)
+               130         860 LOAD_FAST                4 (kwargs)
                
-               124         862 DICT_MERGE               1
+               126         862 DICT_MERGE               1
                            864 CALL_FUNCTION_EX         1
                            866 STORE_FAST              11 (adapter)
                
-               131         868 LOAD_FAST               11 (adapter)
+               133         868 LOAD_FAST               11 (adapter)
                            870 LOAD_METHOD             23 (check_permissions)
                            892 PRECALL                  0
                            896 CALL                     0
                            906 POP_JUMP_FORWARD_IF_FALSE    16 (to 940)
                
-               132         908 LOAD_GLOBAL             49 (NULL + _can_edit)
+               134         908 LOAD_GLOBAL             49 (NULL + _can_edit)
                            920 LOAD_FAST               10 (request)
                            922 LOAD_FAST                6 (obj)
                            924 PRECALL                  2
                            928 CALL                     2
                
-               131         938 POP_JUMP_FORWARD_IF_TRUE    41 (to 1022)
+               133         938 POP_JUMP_FORWARD_IF_TRUE    41 (to 1022)
                
-               133     >>  940 LOAD_GLOBAL             25 (NULL + as_var)
+               135     >>  940 LOAD_GLOBAL             25 (NULL + as_var)
                            952 LOAD_FAST                0 (self)
                            954 LOAD_ATTR               12 (as_var)
                            964 LOAD_FAST                1 (context)
                            966 LOAD_FAST               11 (adapter)
                            968 LOAD_METHOD             25 (render_content)
                            990 LOAD_FAST                1 (context)
                            992 PRECALL                  1
                            996 CALL                     1
                           1006 PRECALL                  3
                           1010 CALL                     3
                           1020 RETURN_VALUE
                
-               135     >> 1022 LOAD_GLOBAL             25 (NULL + as_var)
+               137     >> 1022 LOAD_GLOBAL             25 (NULL + as_var)
                           1034 LOAD_FAST                0 (self)
                           1036 LOAD_ATTR               12 (as_var)
                           1046 LOAD_FAST                1 (context)
                           1048 LOAD_GLOBAL             53 (NULL + wrap_adapter)
                           1060 LOAD_FAST               10 (request)
                           1062 LOAD_FAST               11 (adapter)
                           1064 LOAD_FAST                1 (context)
@@ -834,30 +885,30 @@
                   'request'
                   ('object', 'field_name', 'request')
                   ()
                names      ('model', 'getters', '_resolve_expressions', 'kwargs', 'adapter', 'field_required', 'warnings', 'warn', 'WARNING_MODEL_INSTANCE_NOT_AVAILABLE', '__name__', 'RuntimeWarning', 'flatten', 'as_var', 'render_from_kwargs', 'AdapterError', 'TemplateSyntaxError', 'str', 'len', 'range', 'getattr', 'AttributeError', '__class__', 'get', 'check_permissions', '_can_edit', 'render_content', 'wrap_adapter')
                varnames   ('self', 'context', 'model', 'getters', 'kwargs', 'field_name', 'obj', 'e', 'i', 'getter', 'request', 'adapter')
                freevars   ()
                cellvars   ()
-               filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Packages\\wagtail_fedit\\wagtail_fedit\\templatetags\\fedit.py'
+               filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\tester\\wagtail_fedit\\templatetags\\fedit.py'
                name       'render'
-               firstlineno 72
+               firstlineno 74
                lnotab
                   0x02010e010e020e0104ff04010cff0c040801080102ff020116ff020310
                   011402240110010804040116010c0118ff06030cfc100728020201320102
                   ff040102ff1603120140ff08030401040104013002420110010201240112
                   013eff08042a0110010201020102fd040402fc060728011eff02025202
             (None,)
          names      ('__name__', '__module__', '__qualname__', 'signing', 'TimestampSigner', 'signer', 'Type', 'BaseAdapter', 'FilterExpression', 'list', 'str', '__init__', '_resolve_expressions', 'render')
          varnames   ()
          freevars   ()
          cellvars   ()
-         filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Packages\\wagtail_fedit\\wagtail_fedit\\templatetags\\fedit.py'
+         filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\tester\\wagtail_fedit\\templatetags\\fedit.py'
          name       'AdapterNode'
-         firstlineno 52
+         firstlineno 54
          lnotab 0x0a011e023207060a
       'AdapterNode'
       ('name',)
       'parser'
       'token'
       code
          argcount  : 2
@@ -888,221 +939,224 @@
             00000000007c02a6010000ab01000000000000000064067a0a0000190000
             00000000000000640a6b0200000000724a7c02a001000000000000000000
             0000000000000000000000740d000000000000000000007c02a6010000ab
             01000000000000000064097a0a0000a6010000ab0100000000000000007d
             097c02a0010000000000000000000000000000000000000000740d000000
             000000000000007c02a6010000ab01000000000000000064097a0a0000a6
             010000ab01000000000000000001007413000000000000000000007c007c
-            027c056a0a00000000000000007c056a0b0000000000000000a6040000ab
-            0400000000000000007d0a741900000000000000000000640c7c057c067c
-            077c09640b9c047c0aa4018e015300
-         138           0 RESUME                   0
+            027c056a0a00000000000000007c056a0b00000000000000007c056a0c00
+            00000000000000a6050000ab0500000000000000007d0a741b0000000000
+            0000000000640c7c057c067c077c09640b9c047c0aa4018e015300
+         140           0 RESUME                   0
          
-         141           2 LOAD_FAST                1 (token)
+         143           2 LOAD_FAST                1 (token)
                        4 LOAD_METHOD              0 (split_contents)
                       26 PRECALL                  0
                       30 CALL                     0
                       40 STORE_FAST               2 (tokens)
          
-         143          42 LOAD_FAST                2 (tokens)
+         145          42 LOAD_FAST                2 (tokens)
                       44 LOAD_METHOD              1 (pop)
                       66 LOAD_CONST               1 (0)
                       68 PRECALL                  1
                       72 CALL                     1
                       82 STORE_FAST               3 (_)
          
-         144          84 LOAD_FAST                2 (tokens)
+         146          84 LOAD_FAST                2 (tokens)
                       86 LOAD_METHOD              1 (pop)
                      108 LOAD_CONST               1 (0)
                      110 PRECALL                  1
                      114 CALL                     1
                      124 STORE_FAST               4 (adapter_id)
          
-         146         126 NOP
+         148         126 NOP
          
-         147         128 LOAD_GLOBAL              4 (adapter_registry)
+         149         128 LOAD_GLOBAL              4 (adapter_registry)
                      140 LOAD_FAST                4 (adapter_id)
                      142 BINARY_SUBSCR
                      152 STORE_FAST               5 (adapter)
                      154 JUMP_FORWARD            33 (to 222)
                  >>  156 PUSH_EXC_INFO
          
-         148         158 LOAD_GLOBAL              6 (RegistryLookUpError)
+         150         158 LOAD_GLOBAL              6 (RegistryLookUpError)
                      170 CHECK_EXC_MATCH
                      172 POP_JUMP_FORWARD_IF_FALSE    20 (to 214)
                      174 POP_TOP
          
-         149         176 LOAD_GLOBAL              9 (NULL + TemplateSyntaxError)
+         151         176 LOAD_GLOBAL              9 (NULL + TemplateSyntaxError)
                      188 LOAD_CONST               2 ("No adapter found with identifier '")
                      190 LOAD_FAST                4 (adapter_id)
                      192 FORMAT_VALUE             0
                      194 LOAD_CONST               3 ("'")
                      196 BUILD_STRING             3
                      198 PRECALL                  1
                      202 CALL                     1
                      212 RAISE_VARARGS            1
          
-         148     >>  214 RERAISE                  0
+         150     >>  214 RERAISE                  0
                  >>  216 COPY                     3
                      218 POP_EXCEPT
                      220 RERAISE                  1
          
-         151     >>  222 LOAD_CONST               4 ((None, None))
+         153     >>  222 LOAD_CONST               4 ((None, None))
                      224 UNPACK_SEQUENCE          2
                      228 STORE_FAST               6 (model)
                      230 STORE_FAST               7 (model_tokens)
          
-         152         232 LOAD_FAST                2 (tokens)
+         154         232 LOAD_FAST                2 (tokens)
                      234 POP_JUMP_FORWARD_IF_FALSE   173 (to 582)
          
-         153         236 LOAD_FAST                2 (tokens)
+         155         236 LOAD_FAST                2 (tokens)
                      238 LOAD_METHOD              1 (pop)
                      260 LOAD_CONST               1 (0)
                      262 PRECALL                  1
                      266 CALL                     1
                      276 STORE_FAST               8 (model__field)
          
-         154         278 LOAD_FAST                8 (model__field)
+         156         278 LOAD_FAST                8 (model__field)
                      280 LOAD_METHOD              5 (split)
                      302 LOAD_CONST               5 ('.')
                      304 PRECALL                  1
                      308 CALL                     1
                      318 STORE_FAST               7 (model_tokens)
          
-         158         320 LOAD_GLOBAL             13 (NULL + len)
+         160         320 LOAD_GLOBAL             13 (NULL + len)
                      332 LOAD_FAST                7 (model_tokens)
                      334 PRECALL                  1
                      338 CALL                     1
                      348 LOAD_CONST               6 (2)
                      350 COMPARE_OP               0 (<)
                      356 POP_JUMP_FORWARD_IF_FALSE    34 (to 426)
          
-         159         358 LOAD_FAST                7 (model_tokens)
+         161         358 LOAD_FAST                7 (model_tokens)
                      360 LOAD_CONST               1 (0)
                      362 BINARY_SUBSCR
                      372 LOAD_CONST               7 ('from_context')
                      374 COMPARE_OP               3 (!=)
                      380 POP_JUMP_FORWARD_IF_FALSE    22 (to 426)
                      382 LOAD_FAST                5 (adapter)
                      384 LOAD_ATTR                7 (field_required)
                      394 POP_JUMP_FORWARD_IF_FALSE    15 (to 426)
          
-         160         396 LOAD_GLOBAL              9 (NULL + TemplateSyntaxError)
+         162         396 LOAD_GLOBAL              9 (NULL + TemplateSyntaxError)
          
-         161         408 LOAD_CONST               8 ("Model and field name are required: 'mymodel.myfield' or 'from_context'")
+         163         408 LOAD_CONST               8 ("Model and field name are required: 'mymodel.myfield' or 'from_context'")
          
-         160         410 PRECALL                  1
+         162         410 PRECALL                  1
                      414 CALL                     1
                      424 RAISE_VARARGS            1
          
-         165     >>  426 LOAD_GLOBAL             13 (NULL + len)
+         167     >>  426 LOAD_GLOBAL             13 (NULL + len)
                      438 LOAD_FAST                7 (model_tokens)
                      440 PRECALL                  1
                      444 CALL                     1
                      454 LOAD_CONST               9 (1)
                      456 COMPARE_OP               4 (>)
                      462 POP_JUMP_FORWARD_IF_TRUE    19 (to 502)
          
-         166         464 LOAD_FAST                7 (model_tokens)
+         168         464 LOAD_FAST                7 (model_tokens)
                      466 LOAD_CONST               1 (0)
                      468 BINARY_SUBSCR
                      478 LOAD_CONST               7 ('from_context')
                      480 COMPARE_OP               3 (!=)
                      486 POP_JUMP_FORWARD_IF_FALSE    47 (to 582)
                      488 LOAD_FAST                5 (adapter)
                      490 LOAD_ATTR                7 (field_required)
                      500 POP_JUMP_FORWARD_IF_TRUE    40 (to 582)
          
-         171     >>  502 LOAD_FAST                0 (parser)
+         173     >>  502 LOAD_FAST                0 (parser)
                      504 LOAD_METHOD              8 (compile_filter)
                      526 LOAD_FAST                7 (model_tokens)
                      528 LOAD_METHOD              1 (pop)
                      550 LOAD_CONST               1 (0)
                      552 PRECALL                  1
                      556 CALL                     1
                      566 PRECALL                  1
                      570 CALL                     1
                      580 STORE_FAST               6 (model)
          
-         173     >>  582 LOAD_CONST               0 (None)
+         175     >>  582 LOAD_CONST               0 (None)
                      584 STORE_FAST               9 (as_var)
          
-         174         586 LOAD_FAST                2 (tokens)
+         176         586 LOAD_FAST                2 (tokens)
                      588 POP_JUMP_FORWARD_IF_FALSE   102 (to 794)
                      590 LOAD_FAST                2 (tokens)
                      592 LOAD_GLOBAL             13 (NULL + len)
                      604 LOAD_FAST                2 (tokens)
                      606 PRECALL                  1
                      610 CALL                     1
                      620 LOAD_CONST               6 (2)
                      622 BINARY_OP               10 (-)
                      626 BINARY_SUBSCR
                      636 LOAD_CONST              10 ('as')
                      638 COMPARE_OP               2 (==)
                      644 POP_JUMP_FORWARD_IF_FALSE    74 (to 794)
          
-         175         646 LOAD_FAST                2 (tokens)
+         177         646 LOAD_FAST                2 (tokens)
                      648 LOAD_METHOD              1 (pop)
                      670 LOAD_GLOBAL             13 (NULL + len)
                      682 LOAD_FAST                2 (tokens)
                      684 PRECALL                  1
                      688 CALL                     1
                      698 LOAD_CONST               9 (1)
                      700 BINARY_OP               10 (-)
                      704 PRECALL                  1
                      708 CALL                     1
                      718 STORE_FAST               9 (as_var)
          
-         176         720 LOAD_FAST                2 (tokens)
+         178         720 LOAD_FAST                2 (tokens)
                      722 LOAD_METHOD              1 (pop)
                      744 LOAD_GLOBAL             13 (NULL + len)
                      756 LOAD_FAST                2 (tokens)
                      758 PRECALL                  1
                      762 CALL                     1
                      772 LOAD_CONST               9 (1)
                      774 BINARY_OP               10 (-)
                      778 PRECALL                  1
                      782 CALL                     1
                      792 POP_TOP
          
-         178     >>  794 LOAD_GLOBAL             19 (NULL + get_kwargs)
+         180     >>  794 LOAD_GLOBAL             19 (NULL + get_kwargs)
          
-         179         806 LOAD_FAST                0 (parser)
+         181         806 LOAD_FAST                0 (parser)
          
-         180         808 LOAD_FAST                2 (tokens)
+         182         808 LOAD_FAST                2 (tokens)
          
-         181         810 LOAD_FAST                5 (adapter)
+         183         810 LOAD_FAST                5 (adapter)
                      812 LOAD_ATTR               10 (required_kwargs)
          
-         182         822 LOAD_FAST                5 (adapter)
+         184         822 LOAD_FAST                5 (adapter)
                      824 LOAD_ATTR               11 (absolute_tokens)
          
-         178         834 PRECALL                  4
-                     838 CALL                     4
-                     848 STORE_FAST              10 (kwargs)
+         185         834 LOAD_FAST                5 (adapter)
+                     836 LOAD_ATTR               12 (optional_kwargs)
+         
+         180         846 PRECALL                  5
+                     850 CALL                     5
+                     860 STORE_FAST              10 (kwargs)
          
-         185         850 LOAD_GLOBAL             25 (NULL + AdapterNode)
-                     862 LOAD_CONST              12 (())
+         188         862 LOAD_GLOBAL             27 (NULL + AdapterNode)
+                     874 LOAD_CONST              12 (())
          
-         186         864 LOAD_FAST                5 (adapter)
+         189         876 LOAD_FAST                5 (adapter)
          
-         187         866 LOAD_FAST                6 (model)
+         190         878 LOAD_FAST                6 (model)
          
-         188         868 LOAD_FAST                7 (model_tokens)
+         191         880 LOAD_FAST                7 (model_tokens)
          
-         189         870 LOAD_FAST                9 (as_var)
+         192         882 LOAD_FAST                9 (as_var)
          
-         185         872 LOAD_CONST              11 (('adapter', 'model', 'getters', 'as_var'))
-                     874 BUILD_CONST_KEY_MAP      4
+         188         884 LOAD_CONST              11 (('adapter', 'model', 'getters', 'as_var'))
+                     886 BUILD_CONST_KEY_MAP      4
          
-         190         876 LOAD_FAST               10 (kwargs)
+         193         888 LOAD_FAST               10 (kwargs)
          
-         185         878 DICT_MERGE               1
-                     880 CALL_FUNCTION_EX         1
-                     882 RETURN_VALUE
+         188         890 DICT_MERGE               1
+                     892 CALL_FUNCTION_EX         1
+                     894 RETURN_VALUE
          ExceptionTable:
            128 to 152 -> 156 [0]
            156 to 214 -> 216 [1] lasti
          consts
             None
             0
             "No adapter found with identifier '"
@@ -1112,25 +1166,25 @@
             2
             'from_context'
             "Model and field name are required: 'mymodel.myfield' or 'from_context'"
             1
             'as'
             ('adapter', 'model', 'getters', 'as_var')
             ()
-         names      ('split_contents', 'pop', 'adapter_registry', 'RegistryLookUpError', 'TemplateSyntaxError', 'split', 'len', 'field_required', 'compile_filter', 'get_kwargs', 'required_kwargs', 'absolute_tokens', 'AdapterNode')
+         names      ('split_contents', 'pop', 'adapter_registry', 'RegistryLookUpError', 'TemplateSyntaxError', 'split', 'len', 'field_required', 'compile_filter', 'get_kwargs', 'required_kwargs', 'absolute_tokens', 'optional_kwargs', 'AdapterNode')
          varnames   ('parser', 'token', 'tokens', '_', 'adapter_id', 'adapter', 'model', 'model_tokens', 'model__field', 'as_var', 'kwargs')
          freevars   ()
          cellvars   ()
-         filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Packages\\wagtail_fedit\\wagtail_fedit\\templatetags\\fedit.py'
+         filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\tester\\wagtail_fedit\\templatetags\\fedit.py'
          name       'do_render_fedit'
-         firstlineno 138
+         firstlineno 140
          lnotab
             0x020328022a012a0202011e01120126ff08030a0104012a012a04260126
             010c0102ff100526012605500204013c014a014a020c01020102010c010c
-            fc10070e0102010201020102fc040502fb
+            010cfb10080e0102010201020102fc040502fb
       True
       ('takes_context',)
       'adapter'
       code
          argcount  : 2
          nlocals   : 3
          stacksize : 3
@@ -1139,59 +1193,59 @@
             0x970069007d0264017c007600720b7c006401190000000000000000007d
             027c0064013d007c00a00000000000000000000000000000000000000000
             007c02a6010000ab01000000000000000001007c016a0100000000000000
             007c0064023c0000007c016a0200000000000000007c0064033c0000007c
             016a0300000000000000007c0064043c0000007c01a00400000000000000
             000000000000000000000000007c00a6010000ab01000000000000000053
             00
-         195           0 RESUME                   0
+         198           0 RESUME                   0
          
-         197           2 BUILD_MAP                0
+         200           2 BUILD_MAP                0
                        4 STORE_FAST               2 (parent_context)
          
-         199           6 LOAD_CONST               1 ('parent_context')
+         202           6 LOAD_CONST               1 ('parent_context')
                        8 LOAD_FAST                0 (context)
                       10 CONTAINS_OP              0
                       12 POP_JUMP_FORWARD_IF_FALSE    11 (to 36)
          
-         200          14 LOAD_FAST                0 (context)
+         203          14 LOAD_FAST                0 (context)
                       16 LOAD_CONST               1 ('parent_context')
                       18 BINARY_SUBSCR
                       28 STORE_FAST               2 (parent_context)
          
-         201          30 LOAD_FAST                0 (context)
+         204          30 LOAD_FAST                0 (context)
                       32 LOAD_CONST               1 ('parent_context')
                       34 DELETE_SUBSCR
          
-         203     >>   36 LOAD_FAST                0 (context)
+         206     >>   36 LOAD_FAST                0 (context)
                       38 LOAD_METHOD              0 (update)
                       60 LOAD_FAST                2 (parent_context)
                       62 PRECALL                  1
                       66 CALL                     1
                       76 POP_TOP
          
-         205          78 LOAD_FAST                1 (adapter)
+         208          78 LOAD_FAST                1 (adapter)
                       80 LOAD_ATTR                1 (field_name)
                       90 LOAD_FAST                0 (context)
                       92 LOAD_CONST               2 ('wagtail_fedit_field')
                       94 STORE_SUBSCR
          
-         206          98 LOAD_FAST                1 (adapter)
+         209          98 LOAD_FAST                1 (adapter)
                      100 LOAD_ATTR                2 (object)
                      110 LOAD_FAST                0 (context)
                      112 LOAD_CONST               3 ('wagtail_fedit_instance')
                      114 STORE_SUBSCR
          
-         207         118 LOAD_FAST                1 (adapter)
+         210         118 LOAD_FAST                1 (adapter)
                      120 LOAD_ATTR                3 (request)
                      130 LOAD_FAST                0 (context)
                      132 LOAD_CONST               4 ('request')
                      134 STORE_SUBSCR
          
-         209         138 LOAD_FAST                1 (adapter)
+         212         138 LOAD_FAST                1 (adapter)
                      140 LOAD_METHOD              4 (render_content)
                      162 LOAD_FAST                0 (context)
                      164 PRECALL                  1
                      168 CALL                     1
                      178 RETURN_VALUE
          consts
             None
@@ -1199,17 +1253,17 @@
             'wagtail_fedit_field'
             'wagtail_fedit_instance'
             'request'
          names      ('update', 'field_name', 'object', 'request', 'render_content')
          varnames   ('context', 'adapter', 'parent_context')
          freevars   ()
          cellvars   ()
-         filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Packages\\wagtail_fedit\\wagtail_fedit\\templatetags\\fedit.py'
+         filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\tester\\wagtail_fedit\\templatetags\\fedit.py'
          name       'render_adapter'
-         firstlineno 195
+         firstlineno 198
          lnotab 0x020204020801100106022a02140114011402
       'wagtail_fedit/_hook_output.html'
       'fedit_scripts'
       ('name', 'takes_context')
       code
          argcount  : 2
          nlocals   : 7
@@ -1226,376 +1280,520 @@
             00530067007d04740f000000000000000000006a0800000000000000007c
             03a6010000ab01000000000000000044005d417d0502007c057c02a60100
             00ab0100000000000000007d067413000000000000000000007c06741400
             0000000000000000007416000000000000000000006602a6020000ab0200
             0000000000000073037c0667017d067c04a00c0000000000000000000000
             0000000000000000007c06a6010000ab01000000000000000001008c4264
             067c0469015300
-         212           0 RESUME                   0
+         215           0 RESUME                   0
          
-         214           2 LOAD_FAST                1 (css_or_js)
+         217           2 LOAD_FAST                1 (css_or_js)
                        4 LOAD_METHOD              0 (lower)
                       26 PRECALL                  0
                       30 CALL                     0
                       40 STORE_FAST               1 (css_or_js)
          
-         216          42 LOAD_FAST                1 (css_or_js)
+         219          42 LOAD_FAST                1 (css_or_js)
                       44 LOAD_CONST               1 (('css', 'js'))
                       46 CONTAINS_OP              1
                       48 POP_JUMP_FORWARD_IF_FALSE    15 (to 80)
          
-         217          50 LOAD_GLOBAL              3 (NULL + ValueError)
+         220          50 LOAD_GLOBAL              3 (NULL + ValueError)
                       62 LOAD_CONST               2 ("Invalid argument, must be 'css' or 'js'")
                       64 PRECALL                  1
                       68 CALL                     1
                       78 RAISE_VARARGS            1
          
-         219     >>   80 LOAD_FAST                0 (context)
+         222     >>   80 LOAD_FAST                0 (context)
                       82 LOAD_METHOD              2 (get)
                      104 LOAD_CONST               3 ('request')
                      106 PRECALL                  1
                      110 CALL                     1
                      120 STORE_FAST               2 (request)
          
-         221         122 LOAD_FAST                1 (css_or_js)
+         224         122 LOAD_FAST                1 (css_or_js)
                      124 LOAD_CONST               4 ('css')
                      126 COMPARE_OP               2 (==)
                      132 POP_JUMP_FORWARD_IF_FALSE     8 (to 150)
          
-         222         134 LOAD_GLOBAL              6 (REGISTER_CSS)
+         225         134 LOAD_GLOBAL              6 (REGISTER_CSS)
                      146 STORE_FAST               3 (hook_name)
                      148 JUMP_FORWARD             7 (to 164)
          
-         224     >>  150 LOAD_GLOBAL              8 (REGISTER_JS)
+         227     >>  150 LOAD_GLOBAL              8 (REGISTER_JS)
                      162 STORE_FAST               3 (hook_name)
          
-         226     >>  164 LOAD_GLOBAL             11 (NULL + getattr)
+         229     >>  164 LOAD_GLOBAL             11 (NULL + getattr)
                      176 LOAD_FAST                2 (request)
                      178 LOAD_GLOBAL             12 (FEDIT_PREVIEW_VAR)
                      190 LOAD_CONST               5 (False)
                      192 PRECALL                  3
                      196 CALL                     3
                      206 POP_JUMP_FORWARD_IF_TRUE     2 (to 212)
          
-         227         208 BUILD_MAP                0
+         230         208 BUILD_MAP                0
                      210 RETURN_VALUE
          
-         229     >>  212 BUILD_LIST               0
+         232     >>  212 BUILD_LIST               0
                      214 STORE_FAST               4 (files)
          
-         230         216 LOAD_GLOBAL             15 (NULL + hooks)
+         233         216 LOAD_GLOBAL             15 (NULL + hooks)
                      228 LOAD_ATTR                8 (get_hooks)
                      238 LOAD_FAST                3 (hook_name)
                      240 PRECALL                  1
                      244 CALL                     1
                      254 GET_ITER
                  >>  256 FOR_ITER                65 (to 388)
                      258 STORE_FAST               5 (hook)
          
-         231         260 PUSH_NULL
+         234         260 PUSH_NULL
                      262 LOAD_FAST                5 (hook)
                      264 LOAD_FAST                2 (request)
                      266 PRECALL                  1
                      270 CALL                     1
                      280 STORE_FAST               6 (ret)
          
-         233         282 LOAD_GLOBAL             19 (NULL + isinstance)
+         236         282 LOAD_GLOBAL             19 (NULL + isinstance)
                      294 LOAD_FAST                6 (ret)
                      296 LOAD_GLOBAL             20 (list)
                      308 LOAD_GLOBAL             22 (tuple)
                      320 BUILD_TUPLE              2
                      322 PRECALL                  2
                      326 CALL                     2
                      336 POP_JUMP_FORWARD_IF_TRUE     3 (to 344)
          
-         234         338 LOAD_FAST                6 (ret)
+         237         338 LOAD_FAST                6 (ret)
                      340 BUILD_LIST               1
                      342 STORE_FAST               6 (ret)
          
-         236     >>  344 LOAD_FAST                4 (files)
+         239     >>  344 LOAD_FAST                4 (files)
                      346 LOAD_METHOD             12 (extend)
                      368 LOAD_FAST                6 (ret)
                      370 PRECALL                  1
                      374 CALL                     1
                      384 POP_TOP
                      386 JUMP_BACKWARD           66 (to 256)
          
-         239     >>  388 LOAD_CONST               6 ('hook_output')
+         242     >>  388 LOAD_CONST               6 ('hook_output')
                      390 LOAD_FAST                4 (files)
          
-         238         392 BUILD_MAP                1
+         241         392 BUILD_MAP                1
                      394 RETURN_VALUE
          consts
             None
             ('css', 'js')
             "Invalid argument, must be 'css' or 'js'"
             'request'
             'css'
             False
             'hook_output'
          names      ('lower', 'ValueError', 'get', 'REGISTER_CSS', 'REGISTER_JS', 'getattr', 'FEDIT_PREVIEW_VAR', 'hooks', 'get_hooks', 'isinstance', 'list', 'tuple', 'extend')
          varnames   ('context', 'css_or_js', 'request', 'hook_name', 'files', 'hook', 'ret')
          freevars   ()
          cellvars   ()
-         filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Packages\\wagtail_fedit\\wagtail_fedit\\templatetags\\fedit.py'
+         filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\tester\\wagtail_fedit\\templatetags\\fedit.py'
          name       'static_hook_output'
-         firstlineno 212
+         firstlineno 215
          lnotab
             0x0202280208011e022a020c0110020e022c01040204012c011602380106
             022c0304ff
+      False
+      'tooltip'
+      ('takes_context', 'name')
+      'wrapping'
+      code
+         argcount  : 2
+         nlocals   : 7
+         stacksize : 9
+         flags     : 11
+         code
+            0x97007c007c0264013c000000640267017d037c02a00000000000000000
+            00000000000000000000000000a6000000ab00000000000000000044005d
+            2e5c0200007d047d057c03a0010000000000000000000000000000000000
+            00000064037c049b0064047405000000000000000000007c05a6010000ab
+            0100000000000000009b0064059d05a6010000ab01000000000000000001
+            008c2f6406a00300000000000000000000000000000000000000007c03a6
+            010000ab0100000000000000007d067c01730f7409000000000000000000
+            007c06a6010000ab01000000000000000053007409000000000000000000
+            0064077c069b0064087c019b0064099d05a6010000ab0100000000000000
+            005300
+         245           0 RESUME                   0
+         
+         247           2 LOAD_FAST                0 (content)
+                       4 LOAD_FAST                2 (kwargs)
+                       6 LOAD_CONST               1 ('content')
+                       8 STORE_SUBSCR
+         
+         249          12 LOAD_CONST               2 ("data-tooltip='true'")
+         
+         248          14 BUILD_LIST               1
+                      16 STORE_FAST               3 (s)
+         
+         251          18 LOAD_FAST                2 (kwargs)
+                      20 LOAD_METHOD              0 (items)
+                      42 PRECALL                  0
+                      46 CALL                     0
+                      56 GET_ITER
+                 >>   58 FOR_ITER                46 (to 152)
+                      60 UNPACK_SEQUENCE          2
+                      64 STORE_FAST               4 (key)
+                      66 STORE_FAST               5 (value)
+         
+         252          68 LOAD_FAST                3 (s)
+                      70 LOAD_METHOD              1 (append)
+                      92 LOAD_CONST               3 ('data-tooltip-')
+                      94 LOAD_FAST                4 (key)
+                      96 FORMAT_VALUE             0
+                      98 LOAD_CONST               4 ("='")
+                     100 LOAD_GLOBAL              5 (NULL + escape)
+                     112 LOAD_FAST                5 (value)
+                     114 PRECALL                  1
+                     118 CALL                     1
+                     128 FORMAT_VALUE             0
+                     130 LOAD_CONST               5 ("'")
+                     132 BUILD_STRING             5
+                     134 PRECALL                  1
+                     138 CALL                     1
+                     148 POP_TOP
+                     150 JUMP_BACKWARD           47 (to 58)
+         
+         253     >>  152 LOAD_CONST               6 (' ')
+                     154 LOAD_METHOD              3 (join)
+                     176 LOAD_FAST                3 (s)
+                     178 PRECALL                  1
+                     182 CALL                     1
+                     192 STORE_FAST               6 (attrs)
+         
+         255         194 LOAD_FAST                1 (wrapping)
+                     196 POP_JUMP_FORWARD_IF_TRUE    15 (to 228)
+         
+         256         198 LOAD_GLOBAL              9 (NULL + mark_safe)
+                     210 LOAD_FAST                6 (attrs)
+                     212 PRECALL                  1
+                     216 CALL                     1
+                     226 RETURN_VALUE
+         
+         258     >>  228 LOAD_GLOBAL              9 (NULL + mark_safe)
+                     240 LOAD_CONST               7 ('<span ')
+                     242 LOAD_FAST                6 (attrs)
+                     244 FORMAT_VALUE             0
+                     246 LOAD_CONST               8 ('>')
+                     248 LOAD_FAST                1 (wrapping)
+                     250 FORMAT_VALUE             0
+                     252 LOAD_CONST               9 ('</span>')
+                     254 BUILD_STRING             5
+                     256 PRECALL                  1
+                     260 CALL                     1
+                     270 RETURN_VALUE
+         consts
+            None
+            'content'
+            "data-tooltip='true'"
+            'data-tooltip-'
+            "='"
+            "'"
+            ' '
+            '<span '
+            '>'
+            '</span>'
+         names      ('items', 'append', 'escape', 'join', 'mark_safe')
+         varnames   ('content', 'wrapping', 'kwargs', 's', 'key', 'value', 'attrs')
+         freevars   ()
+         cellvars   ()
+         filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\tester\\wagtail_fedit\\templatetags\\fedit.py'
+         name       'tooltip'
+         firstlineno 245
+         lnotab 0x02020a0202ff0403320154012a0204011e02
       'tokens'
       'kwarg_list'
       'absolute_tokens'
+      'optional_tokens'
       code
-         argcount  : 4
-         nlocals   : 12
+         argcount  : 5
+         nlocals   : 13
          stacksize : 6
          flags     : 3
          code
-            0x970064017d0469007d057c02730267007d027c03730267007d03740100
-            0000000000000000007c01a6010000ab010000000000000000440090015d
-            125c0200007d067d077c07a0010000000000000000000000000000000000
-            0000006402a6010000ab0100000000000000007d08740500000000000000
-            0000007c08a6010000ab01000000000000000064036b0200000000725974
-            05000000000000000000007c02a6010000ab0100000000000000007c066b
-            040000000072467c086404190000000000000000007c037600720c64057c
-            057c086404190000000000000000003c0000008c577c04720f7407000000
-            000000000000006406a6010000ab01000000000000000082017c00a00400
-            000000000000000000000000000000000000007c07a6010000ab01000000
-            00000000007c057c027c06190000000000000000003c0000008c87740500
-            0000000000000000007c08a6010000ab01000000000000000064036b0200
-            00000072397c086404190000000000000000007c037600720c64057c057c
-            086404190000000000000000003c0000008cb07c08640419000000000000
-            0000007d097c00a00400000000000000000000000000000000000000007c
-            09a6010000ab0100000000000000007d0a7c0a7c057c093c0000008cd37c
-            086404190000000000000000007d097c097c037600721374070000000000
-            000000000064077c099b0064089d03a6010000ab01000000000000000082
-            017c00a00400000000000000000000000000000000000000007c08640319
-            000000000000000000a6010000ab0100000000000000007c057c093c0000
-            0064057d0490018c147c0244005d187d0b7c0b7c0576017212740b000000
-            0000000000000064097c0b9b009d02a6010000ab01000000000000000082
-            018c197c055300
-         243           0 RESUME                   0
-         
-         244           2 LOAD_CONST               1 (False)
-                       4 STORE_FAST               4 (had_kwargs)
-         
-         245           6 BUILD_MAP                0
-                       8 STORE_FAST               5 (kwargs)
-         
-         247          10 LOAD_FAST                2 (kwarg_list)
-                      12 POP_JUMP_FORWARD_IF_TRUE     2 (to 18)
-         
-         248          14 BUILD_LIST               0
-                      16 STORE_FAST               2 (kwarg_list)
-         
-         250     >>   18 LOAD_FAST                3 (absolute_tokens)
-                      20 POP_JUMP_FORWARD_IF_TRUE     2 (to 26)
-         
-         251          22 BUILD_LIST               0
-                      24 STORE_FAST               3 (absolute_tokens)
-         
-         253     >>   26 LOAD_GLOBAL              1 (NULL + enumerate)
-                      38 LOAD_FAST                1 (tokens)
-                      40 PRECALL                  1
-                      44 CALL                     1
-                      54 GET_ITER
-                 >>   56 EXTENDED_ARG             1
-                      58 FOR_ITER               274 (to 608)
-                      60 UNPACK_SEQUENCE          2
-                      64 STORE_FAST               6 (i)
-                      66 STORE_FAST               7 (token)
+            0x970064017d0569007d067c02730e740100000000000000000000a60000
+            00ab0000000000000000007d027c03730e740100000000000000000000a6
+            000000ab0000000000000000007d037c04730269007d0474030000000000
+            00000000007c01a6010000ab010000000000000000440090015d125c0200
+            007d077d087c08a002000000000000000000000000000000000000000064
+            02a6010000ab0100000000000000007d097407000000000000000000007c
+            09a6010000ab01000000000000000064036b020000000072597407000000
+            000000000000007c02a6010000ab0100000000000000007c076b04000000
+            0072467c096404190000000000000000007c037600720c64057c067c0964
+            04190000000000000000003c0000008c577c05720f740900000000000000
+            0000006406a6010000ab01000000000000000082017c00a0050000000000
+            0000000000000000000000000000007c08a6010000ab0100000000000000
+            007c067c027c07190000000000000000003c0000008c8774070000000000
+            00000000007c09a6010000ab01000000000000000064036b020000000072
+            397c096404190000000000000000007c037600720c64057c067c09640419
+            0000000000000000003c0000008cb07c096404190000000000000000007d
+            0a7c00a00500000000000000000000000000000000000000007c0aa60100
+            00ab0100000000000000007d0b7c0b7c067c0a3c0000008cd37c09640419
+            0000000000000000007d0a7c0a7c03760072137409000000000000000000
+            0064077c0a9b0064089d03a6010000ab01000000000000000082017c00a0
+            0500000000000000000000000000000000000000007c0964031900000000
+            0000000000a6010000ab0100000000000000007c067c0a3c00000064057d
+            0590018c147c0244005d187d0c7c0c7c0676017212740d00000000000000
+            00000064097c0c9b009d02a6010000ab01000000000000000082018c197c
+            04a0070000000000000000000000000000000000000000a6000000ab0000
+            0000000000000044005d0e5c0200007d0a7d0b7c0a7c06760172057c0b7c
+            067c0a3c0000008c0f7c065300
+         261           0 RESUME                   0
+         
+         262           2 LOAD_CONST               1 (False)
+                       4 STORE_FAST               5 (had_kwargs)
          
-         254          68 LOAD_FAST                7 (token)
-                      70 LOAD_METHOD              1 (split)
-                      92 LOAD_CONST               2 ('=')
-                      94 PRECALL                  1
-                      98 CALL                     1
-                     108 STORE_FAST               8 (split)
-         
-         255         110 LOAD_GLOBAL              5 (NULL + len)
-                     122 LOAD_FAST                8 (split)
-                     124 PRECALL                  1
-                     128 CALL                     1
-                     138 LOAD_CONST               3 (1)
-                     140 COMPARE_OP               2 (==)
-                     146 POP_JUMP_FORWARD_IF_FALSE    89 (to 326)
-                     148 LOAD_GLOBAL              5 (NULL + len)
-                     160 LOAD_FAST                2 (kwarg_list)
-                     162 PRECALL                  1
-                     166 CALL                     1
-                     176 LOAD_FAST                6 (i)
-                     178 COMPARE_OP               4 (>)
-                     184 POP_JUMP_FORWARD_IF_FALSE    70 (to 326)
-         
-         256         186 LOAD_FAST                8 (split)
-                     188 LOAD_CONST               4 (0)
-                     190 BINARY_SUBSCR
-                     200 LOAD_FAST                3 (absolute_tokens)
-                     202 CONTAINS_OP              0
-                     204 POP_JUMP_FORWARD_IF_FALSE    12 (to 230)
-         
-         257         206 LOAD_CONST               5 (True)
-                     208 LOAD_FAST                5 (kwargs)
-                     210 LOAD_FAST                8 (split)
-                     212 LOAD_CONST               4 (0)
-                     214 BINARY_SUBSCR
-                     224 STORE_SUBSCR
-         
-         258         228 JUMP_BACKWARD           87 (to 56)
-         
-         260     >>  230 LOAD_FAST                4 (had_kwargs)
-                     232 POP_JUMP_FORWARD_IF_FALSE    15 (to 264)
-         
-         261         234 LOAD_GLOBAL              7 (NULL + ValueError)
-                     246 LOAD_CONST               6 ('Unexpected positional argument after keyword argument')
-                     248 PRECALL                  1
-                     252 CALL                     1
-                     262 RAISE_VARARGS            1
-         
-         263     >>  264 LOAD_FAST                0 (parser)
-                     266 LOAD_METHOD              4 (compile_filter)
-                     288 LOAD_FAST                7 (token)
-                     290 PRECALL                  1
-                     294 CALL                     1
-                     304 LOAD_FAST                5 (kwargs)
-                     306 LOAD_FAST                2 (kwarg_list)
-                     308 LOAD_FAST                6 (i)
-                     310 BINARY_SUBSCR
-                     320 STORE_SUBSCR
-                     324 JUMP_BACKWARD          135 (to 56)
-         
-         264     >>  326 LOAD_GLOBAL              5 (NULL + len)
-                     338 LOAD_FAST                8 (split)
-                     340 PRECALL                  1
-                     344 CALL                     1
-                     354 LOAD_CONST               3 (1)
-                     356 COMPARE_OP               2 (==)
-                     362 POP_JUMP_FORWARD_IF_FALSE    57 (to 478)
-         
-         265         364 LOAD_FAST                8 (split)
-                     366 LOAD_CONST               4 (0)
-                     368 BINARY_SUBSCR
-                     378 LOAD_FAST                3 (absolute_tokens)
-                     380 CONTAINS_OP              0
-                     382 POP_JUMP_FORWARD_IF_FALSE    12 (to 408)
-         
-         266         384 LOAD_CONST               5 (True)
-                     386 LOAD_FAST                5 (kwargs)
-                     388 LOAD_FAST                8 (split)
-                     390 LOAD_CONST               4 (0)
-                     392 BINARY_SUBSCR
-                     402 STORE_SUBSCR
-         
-         267         406 JUMP_BACKWARD          176 (to 56)
-         
-         269     >>  408 LOAD_FAST                8 (split)
-                     410 LOAD_CONST               4 (0)
-                     412 BINARY_SUBSCR
-                     422 STORE_FAST               9 (key)
-         
-         270         424 LOAD_FAST                0 (parser)
-                     426 LOAD_METHOD              4 (compile_filter)
-                     448 LOAD_FAST                9 (key)
-                     450 PRECALL                  1
-                     454 CALL                     1
-                     464 STORE_FAST              10 (value)
-         
-         271         466 LOAD_FAST               10 (value)
-                     468 LOAD_FAST                5 (kwargs)
-                     470 LOAD_FAST                9 (key)
-                     472 STORE_SUBSCR
-                     476 JUMP_BACKWARD          211 (to 56)
-         
-         273     >>  478 LOAD_FAST                8 (split)
-                     480 LOAD_CONST               4 (0)
-                     482 BINARY_SUBSCR
-                     492 STORE_FAST               9 (key)
-         
-         276         494 LOAD_FAST                9 (key)
-                     496 LOAD_FAST                3 (absolute_tokens)
-                     498 CONTAINS_OP              0
-                     500 POP_JUMP_FORWARD_IF_FALSE    19 (to 540)
-         
-         277         502 LOAD_GLOBAL              7 (NULL + ValueError)
-                     514 LOAD_CONST               7 ('Keyword argument ')
-                     516 LOAD_FAST                9 (key)
-                     518 FORMAT_VALUE             0
-                     520 LOAD_CONST               8 (' cannot be resolved; it will not be parsed as a variable.')
-                     522 BUILD_STRING             3
-                     524 PRECALL                  1
-                     528 CALL                     1
-                     538 RAISE_VARARGS            1
-         
-         279     >>  540 LOAD_FAST                0 (parser)
-                     542 LOAD_METHOD              4 (compile_filter)
-                     564 LOAD_FAST                8 (split)
-                     566 LOAD_CONST               3 (1)
-                     568 BINARY_SUBSCR
-                     578 PRECALL                  1
-                     582 CALL                     1
-                     592 LOAD_FAST                5 (kwargs)
-                     594 LOAD_FAST                9 (key)
-                     596 STORE_SUBSCR
-         
-         280         600 LOAD_CONST               5 (True)
-                     602 STORE_FAST               4 (had_kwargs)
-                     604 EXTENDED_ARG             1
-                     606 JUMP_BACKWARD          276 (to 56)
-         
-         282     >>  608 LOAD_FAST                2 (kwarg_list)
-                     610 GET_ITER
-                 >>  612 FOR_ITER                24 (to 662)
-                     614 STORE_FAST              11 (kwarg)
-         
-         283         616 LOAD_FAST               11 (kwarg)
-                     618 LOAD_FAST                5 (kwargs)
-                     620 CONTAINS_OP              1
-                     622 POP_JUMP_FORWARD_IF_FALSE    18 (to 660)
-         
-         284         624 LOAD_GLOBAL             11 (NULL + TemplateSyntaxError)
-                     636 LOAD_CONST               9 ('Missing required keyword argument ')
-                     638 LOAD_FAST               11 (kwarg)
-                     640 FORMAT_VALUE             0
-                     642 BUILD_STRING             2
-                     644 PRECALL                  1
-                     648 CALL                     1
-                     658 RAISE_VARARGS            1
+         263           6 BUILD_MAP                0
+                       8 STORE_FAST               6 (kwargs)
+         
+         265          10 LOAD_FAST                2 (kwarg_list)
+                      12 POP_JUMP_FORWARD_IF_TRUE    14 (to 42)
+         
+         266          14 LOAD_GLOBAL              1 (NULL + tuple)
+                      26 PRECALL                  0
+                      30 CALL                     0
+                      40 STORE_FAST               2 (kwarg_list)
+         
+         268     >>   42 LOAD_FAST                3 (absolute_tokens)
+                      44 POP_JUMP_FORWARD_IF_TRUE    14 (to 74)
+         
+         269          46 LOAD_GLOBAL              1 (NULL + tuple)
+                      58 PRECALL                  0
+                      62 CALL                     0
+                      72 STORE_FAST               3 (absolute_tokens)
+         
+         271     >>   74 LOAD_FAST                4 (optional_tokens)
+                      76 POP_JUMP_FORWARD_IF_TRUE     2 (to 82)
+         
+         272          78 BUILD_MAP                0
+                      80 STORE_FAST               4 (optional_tokens)
+         
+         274     >>   82 LOAD_GLOBAL              3 (NULL + enumerate)
+                      94 LOAD_FAST                1 (tokens)
+                      96 PRECALL                  1
+                     100 CALL                     1
+                     110 GET_ITER
+                 >>  112 EXTENDED_ARG             1
+                     114 FOR_ITER               274 (to 664)
+                     116 UNPACK_SEQUENCE          2
+                     120 STORE_FAST               7 (i)
+                     122 STORE_FAST               8 (token)
+         
+         275         124 LOAD_FAST                8 (token)
+                     126 LOAD_METHOD              2 (split)
+                     148 LOAD_CONST               2 ('=')
+                     150 PRECALL                  1
+                     154 CALL                     1
+                     164 STORE_FAST               9 (split)
+         
+         276         166 LOAD_GLOBAL              7 (NULL + len)
+                     178 LOAD_FAST                9 (split)
+                     180 PRECALL                  1
+                     184 CALL                     1
+                     194 LOAD_CONST               3 (1)
+                     196 COMPARE_OP               2 (==)
+                     202 POP_JUMP_FORWARD_IF_FALSE    89 (to 382)
+                     204 LOAD_GLOBAL              7 (NULL + len)
+                     216 LOAD_FAST                2 (kwarg_list)
+                     218 PRECALL                  1
+                     222 CALL                     1
+                     232 LOAD_FAST                7 (i)
+                     234 COMPARE_OP               4 (>)
+                     240 POP_JUMP_FORWARD_IF_FALSE    70 (to 382)
+         
+         277         242 LOAD_FAST                9 (split)
+                     244 LOAD_CONST               4 (0)
+                     246 BINARY_SUBSCR
+                     256 LOAD_FAST                3 (absolute_tokens)
+                     258 CONTAINS_OP              0
+                     260 POP_JUMP_FORWARD_IF_FALSE    12 (to 286)
+         
+         278         262 LOAD_CONST               5 (True)
+                     264 LOAD_FAST                6 (kwargs)
+                     266 LOAD_FAST                9 (split)
+                     268 LOAD_CONST               4 (0)
+                     270 BINARY_SUBSCR
+                     280 STORE_SUBSCR
+         
+         279         284 JUMP_BACKWARD           87 (to 112)
+         
+         281     >>  286 LOAD_FAST                5 (had_kwargs)
+                     288 POP_JUMP_FORWARD_IF_FALSE    15 (to 320)
+         
+         282         290 LOAD_GLOBAL              9 (NULL + ValueError)
+                     302 LOAD_CONST               6 ('Unexpected positional argument after keyword argument')
+                     304 PRECALL                  1
+                     308 CALL                     1
+                     318 RAISE_VARARGS            1
+         
+         284     >>  320 LOAD_FAST                0 (parser)
+                     322 LOAD_METHOD              5 (compile_filter)
+                     344 LOAD_FAST                8 (token)
+                     346 PRECALL                  1
+                     350 CALL                     1
+                     360 LOAD_FAST                6 (kwargs)
+                     362 LOAD_FAST                2 (kwarg_list)
+                     364 LOAD_FAST                7 (i)
+                     366 BINARY_SUBSCR
+                     376 STORE_SUBSCR
+                     380 JUMP_BACKWARD          135 (to 112)
+         
+         285     >>  382 LOAD_GLOBAL              7 (NULL + len)
+                     394 LOAD_FAST                9 (split)
+                     396 PRECALL                  1
+                     400 CALL                     1
+                     410 LOAD_CONST               3 (1)
+                     412 COMPARE_OP               2 (==)
+                     418 POP_JUMP_FORWARD_IF_FALSE    57 (to 534)
+         
+         286         420 LOAD_FAST                9 (split)
+                     422 LOAD_CONST               4 (0)
+                     424 BINARY_SUBSCR
+                     434 LOAD_FAST                3 (absolute_tokens)
+                     436 CONTAINS_OP              0
+                     438 POP_JUMP_FORWARD_IF_FALSE    12 (to 464)
+         
+         287         440 LOAD_CONST               5 (True)
+                     442 LOAD_FAST                6 (kwargs)
+                     444 LOAD_FAST                9 (split)
+                     446 LOAD_CONST               4 (0)
+                     448 BINARY_SUBSCR
+                     458 STORE_SUBSCR
+         
+         288         462 JUMP_BACKWARD          176 (to 112)
+         
+         290     >>  464 LOAD_FAST                9 (split)
+                     466 LOAD_CONST               4 (0)
+                     468 BINARY_SUBSCR
+                     478 STORE_FAST              10 (key)
          
-         283     >>  660 JUMP_BACKWARD           25 (to 612)
+         291         480 LOAD_FAST                0 (parser)
+                     482 LOAD_METHOD              5 (compile_filter)
+                     504 LOAD_FAST               10 (key)
+                     506 PRECALL                  1
+                     510 CALL                     1
+                     520 STORE_FAST              11 (value)
+         
+         292         522 LOAD_FAST               11 (value)
+                     524 LOAD_FAST                6 (kwargs)
+                     526 LOAD_FAST               10 (key)
+                     528 STORE_SUBSCR
+                     532 JUMP_BACKWARD          211 (to 112)
+         
+         294     >>  534 LOAD_FAST                9 (split)
+                     536 LOAD_CONST               4 (0)
+                     538 BINARY_SUBSCR
+                     548 STORE_FAST              10 (key)
+         
+         297         550 LOAD_FAST               10 (key)
+                     552 LOAD_FAST                3 (absolute_tokens)
+                     554 CONTAINS_OP              0
+                     556 POP_JUMP_FORWARD_IF_FALSE    19 (to 596)
+         
+         298         558 LOAD_GLOBAL              9 (NULL + ValueError)
+                     570 LOAD_CONST               7 ('Keyword argument ')
+                     572 LOAD_FAST               10 (key)
+                     574 FORMAT_VALUE             0
+                     576 LOAD_CONST               8 (' cannot be resolved; it will not be parsed as a variable.')
+                     578 BUILD_STRING             3
+                     580 PRECALL                  1
+                     584 CALL                     1
+                     594 RAISE_VARARGS            1
+         
+         300     >>  596 LOAD_FAST                0 (parser)
+                     598 LOAD_METHOD              5 (compile_filter)
+                     620 LOAD_FAST                9 (split)
+                     622 LOAD_CONST               3 (1)
+                     624 BINARY_SUBSCR
+                     634 PRECALL                  1
+                     638 CALL                     1
+                     648 LOAD_FAST                6 (kwargs)
+                     650 LOAD_FAST               10 (key)
+                     652 STORE_SUBSCR
+         
+         301         656 LOAD_CONST               5 (True)
+                     658 STORE_FAST               5 (had_kwargs)
+                     660 EXTENDED_ARG             1
+                     662 JUMP_BACKWARD          276 (to 112)
+         
+         303     >>  664 LOAD_FAST                2 (kwarg_list)
+                     666 GET_ITER
+                 >>  668 FOR_ITER                24 (to 718)
+                     670 STORE_FAST              12 (kwarg)
+         
+         304         672 LOAD_FAST               12 (kwarg)
+                     674 LOAD_FAST                6 (kwargs)
+                     676 CONTAINS_OP              1
+                     678 POP_JUMP_FORWARD_IF_FALSE    18 (to 716)
+         
+         305         680 LOAD_GLOBAL             13 (NULL + TemplateSyntaxError)
+                     692 LOAD_CONST               9 ('Missing required keyword argument ')
+                     694 LOAD_FAST               12 (kwarg)
+                     696 FORMAT_VALUE             0
+                     698 BUILD_STRING             2
+                     700 PRECALL                  1
+                     704 CALL                     1
+                     714 RAISE_VARARGS            1
+         
+         304     >>  716 JUMP_BACKWARD           25 (to 668)
+         
+         307     >>  718 LOAD_FAST                4 (optional_tokens)
+                     720 LOAD_METHOD              7 (items)
+                     742 PRECALL                  0
+                     746 CALL                     0
+                     756 GET_ITER
+                 >>  758 FOR_ITER                14 (to 788)
+                     760 UNPACK_SEQUENCE          2
+                     764 STORE_FAST              10 (key)
+                     766 STORE_FAST              11 (value)
+         
+         308         768 LOAD_FAST               10 (key)
+                     770 LOAD_FAST                6 (kwargs)
+                     772 CONTAINS_OP              1
+                     774 POP_JUMP_FORWARD_IF_FALSE     5 (to 786)
+         
+         309         776 LOAD_FAST               11 (value)
+                     778 LOAD_FAST                6 (kwargs)
+                     780 LOAD_FAST               10 (key)
+                     782 STORE_SUBSCR
+                 >>  786 JUMP_BACKWARD           15 (to 758)
          
-         286     >>  662 LOAD_FAST                5 (kwargs)
-                     664 RETURN_VALUE
+         311     >>  788 LOAD_FAST                6 (kwargs)
+                     790 RETURN_VALUE
          consts
             None
             False
             '='
             1
             0
             True
             'Unexpected positional argument after keyword argument'
             'Keyword argument '
             ' cannot be resolved; it will not be parsed as a variable.'
             'Missing required keyword argument '
-         names      ('enumerate', 'split', 'len', 'ValueError', 'compile_filter', 'TemplateSyntaxError')
-         varnames   ('parser', 'tokens', 'kwarg_list', 'absolute_tokens', 'had_kwargs', 'kwargs', 'i', 'token', 'split', 'key', 'value', 'kwarg')
+         names      ('tuple', 'enumerate', 'split', 'len', 'ValueError', 'compile_filter', 'TemplateSyntaxError', 'items')
+         varnames   ('parser', 'tokens', 'kwarg_list', 'absolute_tokens', 'optional_tokens', 'had_kwargs', 'kwargs', 'i', 'token', 'split', 'key', 'value', 'kwarg')
          freevars   ()
          cellvars   ()
-         filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Packages\\wagtail_fedit\\wagtail_fedit\\templatetags\\fedit.py'
+         filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\tester\\wagtail_fedit\\templatetags\\fedit.py'
          name       'get_kwargs'
-         firstlineno 243
+         firstlineno 261
          lnotab
-            0x02010401040204010402040104022a012a014c0114011601020204011e
-            023e01260114011601020210012a010c021003080126023c010802080108
-            0124ff0203
-      (None, None)
-   names      ('typing', 'Type', 'django.template', 'library', 'Node', 'TemplateSyntaxError', 'django.template.context', 'Context', 'django.template.base', 'Parser', 'Token', 'FilterExpression', 'django.http', 'HttpRequest', 'django.urls', 'reverse', 'django.core', 'signing', 'wagtail', 'hooks', 'warnings', 'adapters', 'adapter_registry', 'RegistryLookUpError', 'BaseAdapter', 'AdapterError', 'utils', 'wrap_adapter', '_can_edit', 'FEDIT_PREVIEW_VAR', 'TEMPLATE_TAG_NAME', 'REGISTER_CSS', 'REGISTER_JS', 'Library', 'register', 'WARNING_FIELD_NAME_NOT_AVAILABLE', 'WARNING_MODEL_INSTANCE_NOT_AVAILABLE', 'str', 'as_var', 'AdapterNode', 'tag', 'do_render_fedit', 'simple_tag', 'render_adapter', 'inclusion_tag', 'dict', 'static_hook_output', 'list', 'get_kwargs')
+            0x02010401040204011c0204011c02040104022a012a014c011401160102
+            0204011e023e01260114011601020210012a010c021003080126023c0108
+            020801080124ff0203320108010c02
+      (None,)
+      (None, None, None)
+   names      ('typing', 'Type', 'Any', 'django.template', 'library', 'Node', 'TemplateSyntaxError', 'django.template.context', 'Context', 'django.template.base', 'Parser', 'Token', 'FilterExpression', 'django.http', 'HttpRequest', 'django.utils.html', 'escape', 'django.utils.safestring', 'mark_safe', 'django.urls', 'reverse', 'django.core', 'signing', 'wagtail', 'hooks', 'warnings', 'adapters', 'adapter_registry', 'RegistryLookUpError', 'BaseAdapter', 'AdapterError', 'utils', 'wrap_adapter', '_can_edit', 'FEDIT_PREVIEW_VAR', 'TEMPLATE_TAG_NAME', 'REGISTER_CSS', 'REGISTER_JS', 'Library', 'register', 'WARNING_FIELD_NAME_NOT_AVAILABLE', 'WARNING_MODEL_INSTANCE_NOT_AVAILABLE', 'str', 'as_var', 'AdapterNode', 'tag', 'do_render_fedit', 'simple_tag', 'render_adapter', 'inclusion_tag', 'dict', 'static_hook_output', 'tooltip', 'list', 'get_kwargs')
    varnames   ()
    freevars   ()
    cellvars   ()
-   filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Packages\\wagtail_fedit\\wagtail_fedit\\templatetags\\fedit.py'
+   filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\tester\\wagtail_fedit\\templatetags\\fedit.py'
    name       '<module>'
    firstlineno 1
    lnotab
-      0x00ff02010c0114030c0314040c010c010c020c0208021806180610061e
-      030401040318071c562a010eff0e0102382a0112ff0e0102102e010aff0e
-      01021e
+      0x00ff0201100114030c0314040c010c010c010c010c020c020802180618
+      0610061e030401040318071c562a010eff0e0102392a0112ff0e0102102e
+      010aff0e01021d2c0110ff0e01020f
```

### Comparing `wagtail_fedit-1.5.3rc9/wagtail_fedit/templatetags/fedit.py` & `wagtail_fedit-1.5.4rc1/wagtail_fedit/templatetags/fedit.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,21 @@
-from typing import Type
+from typing import Type, Any
 from django.template import (
     library, Node, TemplateSyntaxError,
 )
 from django.template.context import (
     Context,
 )
 from django.template.base import (
     Parser, Token,
     FilterExpression,
 )
 from django.http import HttpRequest
+from django.utils.html import escape
+from django.utils.safestring import mark_safe
 from django.urls import reverse
 from django.core import signing
 
 from wagtail import hooks
 
 import warnings
 
@@ -176,14 +178,15 @@
         tokens.pop(len(tokens)-1)
 
     kwargs = get_kwargs(
         parser,
         tokens,
         adapter.required_kwargs,
         adapter.absolute_tokens,
+        adapter.optional_kwargs,
     )
 
     return AdapterNode(
         adapter=adapter,
         model=model,
         getters=model_tokens,
         as_var=as_var,
@@ -235,24 +238,42 @@
 
         files.extend(ret)
         
     return {
         "hook_output": files,
     }
 
+@register.simple_tag(takes_context=False, name="tooltip")
+def tooltip(content, wrapping: str = None, **kwargs) -> str:
+    kwargs["content"] = content
+    s = [
+        "data-tooltip='true'"
+    ]
+    for key, value in kwargs.items():
+        s.append(f"data-tooltip-{key}='{escape(value)}'")
+    attrs = " ".join(s)
 
-def get_kwargs(parser: Parser, tokens: list[str], kwarg_list: list[str] = None, absolute_tokens: list[str] = None) -> dict:
+    if not wrapping:
+        return mark_safe(attrs)
+    
+    return mark_safe(f"<span {attrs}>{wrapping}</span>")
+
+
+def get_kwargs(parser: Parser, tokens: list[str], kwarg_list: list[str] = None, absolute_tokens: list[str] = None, optional_tokens: dict[str, Any] = None) -> dict:
     had_kwargs = False
     kwargs = {}
 
     if not kwarg_list:
-        kwarg_list = []
+        kwarg_list = tuple()
 
     if not absolute_tokens:
-        absolute_tokens = []
+        absolute_tokens = tuple()
+
+    if not optional_tokens:
+        optional_tokens = {}
 
     for i, token in enumerate(tokens):
         split = token.split("=")
         if len(split) == 1 and len(kwarg_list) > i:
             if split[0] in absolute_tokens:
                 kwargs[split[0]] = True
                 continue
@@ -278,10 +299,14 @@
             
             kwargs[key] = parser.compile_filter(split[1])
             had_kwargs = True
 
     for kwarg in kwarg_list:
         if kwarg not in kwargs:
             raise TemplateSyntaxError(f"Missing required keyword argument {kwarg}")
+        
+    for key, value in optional_tokens.items():
+        if key not in kwargs:
+            kwargs[key] = value
 
     return kwargs
```

### Comparing `wagtail_fedit-1.5.3rc9/wagtail_fedit/test/core/migrations/0001_initial.py` & `wagtail_fedit-1.5.4rc1/wagtail_fedit/test/core/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc9/wagtail_fedit/test/core/models.py` & `wagtail_fedit-1.5.4rc1/wagtail_fedit/test/core/models.py`

 * *Files 3% similar despite different names*

```diff
@@ -86,28 +86,37 @@
 
 class BaseEditableMixin:
     def get_url(self, request):
         return f"/{slugify(self.title)}/"
     
     def serve(self, request, *args, **kwargs):
         return HttpResponse(self.body)
-        
+
+    def render_as_content(self, request, context=None):
+        return f"<h1>{self.title}</h1><p>{self.body}</p>"
+
 @register_snippet
 class BasicModel(models.Model):
     title = models.CharField(max_length=255)
     body = models.TextField()
     content: StreamValue = StreamField([
         ("heading_component", HeadingComponent()),
         ("flat_menu_component", FlatMenuComponent())
     ], use_json_field=True)
     related_field = models.ForeignKey("self", on_delete=models.CASCADE, null=True, blank=True)
 
+    panels = [
+        FieldPanel("title"),
+        FieldPanel("body"),
+    ]
+
     def render_as_content(self, request, context=None):
         return f"<h1>{self.title}</h1><p>{self.body}</p>"
 
+
 @register_snippet
 class EditableFullModel(BaseEditableMixin, FEditableMixin):
     title = models.CharField(max_length=255)
     body = models.TextField()
     content: StreamValue = StreamField([
         ("heading_component", HeadingComponent()),
         ("flat_menu_component", FlatMenuComponent())
@@ -148,14 +157,18 @@
     title = models.CharField(max_length=255)
     body = models.TextField()
     content: StreamValue = StreamField([
         ("heading_component", HeadingComponent()),
         ("flat_menu_component", FlatMenuComponent())
     ], use_json_field=True)
 
+    panels = [
+        FieldPanel("title"),
+        FieldPanel("body"),
+    ]
     
     def get_permissions_policy(self):
         return ModelPermissionPolicy(self.__class__)
     
     def permissions_for_user(self, user):
         return FeditPermissionTester(
             self,
@@ -168,9 +181,15 @@
     body = models.TextField()
     content: StreamValue = StreamField([
         ("heading_component", HeadingComponent()),
         ("flat_menu_component", FlatMenuComponent())
     ], use_json_field=True)
 
     content_panels = Page.content_panels + [
-        FieldPanel("content")
+        FieldPanel("body")
     ]
+
+    promote_panels = []
+    settings_panels = []
+
+    def render_as_content(self, request, context=None):
+        return f"<h1>{self.title}</h1><p>{self.body}</p>"
```

#### html2text {}

```diff
@@ -26,21 +26,25 @@
 template = Template(""" {% load wagtailcore_tags %}
 ************ {{{{ ttiittllee }}}} ************
 {{ subtitle }}
     * {% for item in items %} {% include_block item %} {% endfor %}
 """) context = self.get_context(value, parent_context=context) return
 template.render(Context(context)) class BaseEditableMixin: def get_url(self,
 request): return f"/{slugify(self.title)}/" def serve(self, request, *args,
-**kwargs): return HttpResponse(self.body) @register_snippet class BasicModel
-(models.Model): title = models.CharField(max_length=255) body =
-models.TextField() content: StreamValue = StreamField([ ("heading_component",
-HeadingComponent()), ("flat_menu_component", FlatMenuComponent()) ],
-use_json_field=True) related_field = models.ForeignKey("self",
-on_delete=models.CASCADE, null=True, blank=True) def render_as_content(self,
-request, context=None): return f"
+**kwargs): return HttpResponse(self.body) def render_as_content(self, request,
+context=None): return f"
+************ {{sseellff..ttiittllee}} ************
+{self.body}
+" @register_snippet class BasicModel(models.Model): title = models.CharField
+(max_length=255) body = models.TextField() content: StreamValue = StreamField(
+[ ("heading_component", HeadingComponent()), ("flat_menu_component",
+FlatMenuComponent()) ], use_json_field=True) related_field = models.ForeignKey
+("self", on_delete=models.CASCADE, null=True, blank=True) panels = [ FieldPanel
+("title"), FieldPanel("body"), ] def render_as_content(self, request,
+context=None): return f"
 ************ {{sseellff..ttiittllee}} ************
 {self.body}
 " @register_snippet class EditableFullModel(BaseEditableMixin, FEditableMixin):
 title = models.CharField(max_length=255) body = models.TextField() content:
 StreamValue = StreamField([ ("heading_component", HeadingComponent()),
 ("flat_menu_component", FlatMenuComponent()) ], use_json_field=True)
 @register_snippet class EditableDraftModel(BaseEditableMixin, DraftStateMixin,
@@ -56,15 +60,20 @@
 = models.CharField(max_length=255) body = models.TextField() content:
 StreamValue = StreamField([ ("heading_component", HeadingComponent()),
 ("flat_menu_component", FlatMenuComponent()) ], use_json_field=True)
 @register_snippet class EditableLockModel(BaseEditableMixin, WorkflowMixin,
 DraftStateMixin, RevisionMixin, LockableMixin, models.Model): title =
 models.CharField(max_length=255) body = models.TextField() content: StreamValue
 = StreamField([ ("heading_component", HeadingComponent()),
-("flat_menu_component", FlatMenuComponent()) ], use_json_field=True) def
-get_permissions_policy(self): return ModelPermissionPolicy(self.__class__) def
-permissions_for_user(self, user): return FeditPermissionTester( self,
-user=user, policy=self.get_permissions_policy() ) class EditablePageModel
-(Page): body = models.TextField() content: StreamValue = StreamField([
-("heading_component", HeadingComponent()), ("flat_menu_component",
-FlatMenuComponent()) ], use_json_field=True) content_panels =
-Page.content_panels + [ FieldPanel("content") ]
+("flat_menu_component", FlatMenuComponent()) ], use_json_field=True) panels =
+[ FieldPanel("title"), FieldPanel("body"), ] def get_permissions_policy(self):
+return ModelPermissionPolicy(self.__class__) def permissions_for_user(self,
+user): return FeditPermissionTester( self, user=user,
+policy=self.get_permissions_policy() ) class EditablePageModel(Page): body =
+models.TextField() content: StreamValue = StreamField([ ("heading_component",
+HeadingComponent()), ("flat_menu_component", FlatMenuComponent()) ],
+use_json_field=True) content_panels = Page.content_panels + [ FieldPanel
+("body") ] promote_panels = [] settings_panels = [] def render_as_content(self,
+request, context=None): return f"
+************ {{sseellff..ttiittllee}} ************
+{self.body}
+"
```

### Comparing `wagtail_fedit-1.5.3rc9/wagtail_fedit/test/core/tests/base.py` & `wagtail_fedit-1.5.4rc1/wagtail_fedit/test/core/tests/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -199,15 +199,14 @@
         
         self.models: list[models.Model] = [
             self.full_model,
             self.draft_model,
             self.revision_model,
             self.preview_model,
             self.basic_model,
-            self.lock_model,
         ]
 
     def get_editable_url(self, object_id, app_label, model_name):
         url_name = "editable"
         return reverse(
             f"wagtail_fedit:{url_name}",
             kwargs={
@@ -235,14 +234,26 @@
                 "adapter_id": "field",
                 "field_name": field_name,
                 "app_label": app_label,
                 "model_name": model_name,
                 "model_id": model_id
             }
         )
+    
+    def get_model_url(self, app_label, model_name, model_id):
+        url_name = "edit"
+        return reverse(
+            f"wagtail_fedit:{url_name}",
+            kwargs={
+                "adapter_id": "model",
+                "app_label": app_label,
+                "model_name": model_name,
+                "model_id": model_id
+            }
+        )
 
 
     def get_block_url(self, block_id, field_name, app_label, model_name, model_id):
         url_name = "edit"
         url = reverse(
             f"wagtail_fedit:{url_name}",
             kwargs={
```

### Comparing `wagtail_fedit-1.5.3rc9/wagtail_fedit/test/core/tests/test_adapters.py` & `wagtail_fedit-1.5.4rc1/wagtail_fedit/test/core/tests/test_adapters.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from django.db.models.base import Model as Model
 from django.http import HttpRequest
 from django.template import (
     Context, Template,
     TemplateSyntaxError,
 )
 from wagtail_fedit.adapters import (
+    Keyword,
     BaseAdapter,
     adapter_registry,
     BlockAdapter,
     FieldAdapter,
     ModelAdapter,
 )
 from wagtail_fedit.utils import (
@@ -22,15 +23,17 @@
     BaseFEditTest,
 )
 
 adapters = {}
 
 class TestAdapter(BaseAdapter):
     identifier = "test"
-    required_kwargs = ["test"]
+    keywords = (
+        Keyword("test", help_text="A test keyword argument", type_hint="str"),
+    )
     js_constructor = "wagtail_fedit.ThisDoesntGetUsedAnyways"
 
     def __init__(self, object: Model, field_name: str, request: HttpRequest, **kwargs):
         super().__init__(object, field_name, request, **kwargs)
         adapters[self.kwargs["id"]] = self
 
     def get_element_id(self) -> str:
@@ -43,15 +46,19 @@
     identifier = "test_context"
 
     def render_content(self, parent_context: dict = None) -> str:
         return parent_context["testing"]
 
 class TestAbsoluteTokensAdapter(TestAdapter):
     identifier = "test_absolute_tokens"
-    absolute_tokens = ["absolute"]
+
+    keywords = TestAdapter.keywords + (
+        Keyword("optional", optional=True, help_text="A test keyword argument", type_hint="str", default="default"),
+        Keyword("absolute", absolute=True, help_text="A test keyword argument", type_hint="bool"),
+    )
 
     def render_content(self, parent_context: dict = None) -> str:
         return str(self.kwargs.get("absolute", False))
 
 class TestBlockAdapter(BlockAdapter, TestAdapter):
     identifier = "test_block"
 
@@ -64,23 +71,34 @@
 adapter_registry.register(TestAdapter)
 adapter_registry.register(TestBlockAdapter)
 adapter_registry.register(TestFieldAdapter)
 adapter_registry.register(TestModelAdapter)
 adapter_registry.register(TestContextAdapter)
 adapter_registry.register(TestAbsoluteTokensAdapter)
 
+import uuid
+
+def get_adapter_id() -> str:
+    return str(uuid.uuid4())
 
 class TestBaseAdapter(BaseFEditTest):
 
+    def test_required_kwargs(self):
+        self.assertEqual(TestAdapter.required_kwargs, tuple(["test"]))
+
+    def test_absolute_tokens(self):
+        self.assertEqual(TestAbsoluteTokensAdapter.absolute_tokens, tuple(["absolute"]))
+
     def test_required_kwargs_ok(self):
-        self.assertEqual(TestAdapter.required_kwargs, ["test"])
+        self.assertEqual(TestAdapter.required_kwargs, tuple(["test"]))
+        id = get_adapter_id()
 
         template_ok = Template(
             "{% load fedit %}"
-            "{% fedit test object.title test='test' id=1 %}"
+            f"{{% fedit test object.title test='test' id='{id}' %}}"
         )
 
         request = self.request_factory.get(
             self.get_editable_url(
                 self.basic_model.pk, self.basic_model._meta.app_label, self.basic_model._meta.model_name,
             )
         )
@@ -95,30 +113,31 @@
 
         self.assertHTMLEqual(
             template_ok,
             f'TestAdapter: {self.basic_model.title}'
         )
 
         self.assertDictEqual(
-            adapters[1].kwargs,
-            {"test": "test", "id": 1}
+            adapters[id].kwargs,
+            {"test": "test", "id": id}
         )
 
     def test_required_kwargs_fail(self):
+        id = get_adapter_id()
         request = self.request_factory.get(
             self.get_editable_url(
                 self.basic_model.pk, self.basic_model._meta.app_label, self.basic_model._meta.model_name,
             )
         )
         request.user = self.admin_user
 
         try:
             template_fail = Template(
                 "{% load fedit %}"
-                "{% fedit test object.title id=2 %}"
+                f"{{% fedit test object.title id='{id}' %}}"
             )
 
             # self.fail(f"Expected exception: {e}")
             template_fail.render(Context({
                 "request": request,
                 "object": self.basic_model,
             }))
@@ -131,35 +150,75 @@
 
         except Exception as e:
             self.fail(f"Unexpected exception: {e} ({type(e)})")
 
         else:
             self.fail("Expected exception not raised")
 
-    def test_adapter_render_content(self):
-        adapter = TestAdapter(
-            self.basic_model,
-            "title",
-            self.request_factory.get(
-                self.get_editable_url(
-                    self.basic_model.pk, self.basic_model._meta.app_label, self.basic_model._meta.model_name,
-                )
-            ),
-            id=3,
+    def test_optional_kwargs_default(self):
+        id = get_adapter_id()
+        template = Template(
+            "{% load fedit %}"
+            f"{{% fedit test_absolute_tokens object.title test='test' id='{id}' %}}"
+        )
+
+        request = self.request_factory.get(
+            self.get_editable_url(
+                self.basic_model.pk, self.basic_model._meta.app_label, self.basic_model._meta.model_name,
+            )
+        )
+        request.user = self.admin_user
+
+        template = template.render(
+            Context({
+                "request": request,
+                "object": self.basic_model,
+            })
         )
 
+        adapter = adapters[id]
+
         self.assertEqual(
-            adapter.render_content(),
-            f"TestAdapter: {self.basic_model.title}"
+            adapter.kwargs["optional"],
+            "default",
+        )
+
+    def test_optional_kwargs_override(self):
+        id = get_adapter_id()
+        template = Template(
+            "{% load fedit %}"
+            f"{{% fedit test_absolute_tokens object.title optional='not default' test='test' id='{id}' %}}"
+        )
+
+        request = self.request_factory.get(
+            self.get_editable_url(
+                self.basic_model.pk, self.basic_model._meta.app_label, self.basic_model._meta.model_name,
+            )
+        )
+        request.user = self.admin_user
+
+        template = template.render(
+            Context({
+                "request": request,
+                "object": self.basic_model,
+            })
+        )
+
+        adapter = adapters[id]
+
+        self.assertEqual(
+            adapter.kwargs["optional"],
+            "not default",
         )
 
     def test_adapter_absolute_tokens(self):
+        id = get_adapter_id()
         tpl = Template(
             "{% load fedit %}"
-            "{% fedit test_absolute_tokens object.title test='test' absolute id=4 %}"
+            f"{{% fedit test_absolute_tokens object.title test='test' absolute id='{id}' %}}"
         )
 
         request = self.request_factory.get(
             self.get_editable_url(
                 self.basic_model.pk, self.basic_model._meta.app_label, self.basic_model._meta.model_name,
             )
         )
@@ -173,18 +232,52 @@
         )
 
         self.assertHTMLEqual(
             tpl,
             str(True),
         )
 
+    def test_positional_kwargs(self):
+        id = get_adapter_id()
+        tpl = Template(
+            "{% load fedit %}"
+            f"{{% fedit test_absolute_tokens object.title 'test' absolute id='{id}' %}}"
+        )
+
+        request = self.request_factory.get(
+            self.get_editable_url(
+                self.basic_model.pk, self.basic_model._meta.app_label, self.basic_model._meta.model_name,
+            )
+        )
+        request.user = self.admin_user
+
+        tpl = tpl.render(
+            Context({
+                "request": request,
+                "object": self.basic_model,
+            })
+        )
+
+        adapter = adapters[id]
+
+        self.assertEqual(
+            adapter.kwargs["test"],
+            "test",
+        )
+
+        self.assertEqual(
+            adapter.kwargs["absolute"],
+            True,
+        )
+
     def test_adapter_absolute_tokens_fail(self):
+        id = get_adapter_id()
         tpl = Template(
             "{% load fedit %}"
-            "{% fedit test_absolute_tokens object.title test='test' id=4 %}"
+            f"{{% fedit test_absolute_tokens object.title test='test' id='{id}' %}}"
         )
 
         request = self.request_factory.get(
             self.get_editable_url(
                 self.basic_model.pk, self.basic_model._meta.app_label, self.basic_model._meta.model_name,
             )
         )
@@ -198,20 +291,38 @@
         )
 
         self.assertHTMLEqual(
             tpl,
             str(False),
         )
 
+    def test_adapter_render_content(self):
+        adapter = TestAdapter(
+            self.basic_model,
+            "title",
+            self.request_factory.get(
+                self.get_editable_url(
+                    self.basic_model.pk, self.basic_model._meta.app_label, self.basic_model._meta.model_name,
+                )
+            ),
+            id=3,
+        )
+
+        self.assertEqual(
+            adapter.render_content(),
+            f"TestAdapter: {self.basic_model.title}"
+        )
+
     def test_adapter_editable(self):
-        self.assertEqual(TestAdapter.required_kwargs, ["test"])
+        id = get_adapter_id()
+        self.assertEqual(TestAdapter.required_kwargs, tuple(["test"]))
 
         tpl = Template(
             "{% load fedit %}"
-            "{% fedit test object.title test='test' id=4 %}"
+            f"{{% fedit test object.title test='test' id='{id}' %}}"
         )
 
         request = self.request_factory.get(
             self.get_editable_url(
                 self.basic_model.pk, self.basic_model._meta.app_label, self.basic_model._meta.model_name,
             )
         )
@@ -228,23 +339,24 @@
                 "request": request,
                 "object": self.basic_model,
             })
         )
 
         self.assertHTMLEqual(
             tpl,
-            wrap_adapter(request, adapters[4], {})
+            wrap_adapter(request, adapters[id], {})
         )
 
     def test_adapter_editable_as_var(self):
-        self.assertEqual(TestAdapter.required_kwargs, ["test"])
+        id = get_adapter_id()
+        self.assertEqual(TestAdapter.required_kwargs, tuple(["test"]))
 
         tpl = Template(
             "{% load fedit %}"
-            "{% fedit test object.title test='test' id=5 as test_adapter_as_variable_name %}"
+            f"{{% fedit test object.title test='test' id='{id}' as test_adapter_as_variable_name %}}"
             "{{ test_adapter_as_variable_name }}"
         )
 
         request = self.request_factory.get(
             self.get_editable_url(
                 self.basic_model.pk, self.basic_model._meta.app_label, self.basic_model._meta.model_name,
             )
@@ -262,21 +374,22 @@
                 "request": request,
                 "object": self.basic_model,
             })
         )
 
         self.assertHTMLEqual(
             tpl,
-            wrap_adapter(request, adapters[5], {})
+            wrap_adapter(request, adapters[id], {})
         )
 
     def test_context_processors_run(self):
+        id = get_adapter_id()
         tpl = Template(
             "{% load fedit %}"
-            "{% fedit test_context object.title test='test' id=5 %}"
+            f"{{% fedit test_context object.title test='test' id='{id}' %}}"
         )
 
         request = self.request_factory.get(
             self.get_editable_url(
                 self.basic_model.pk, self.basic_model._meta.app_label, self.basic_model._meta.model_name,
             )
         )
@@ -295,21 +408,22 @@
                 "object": self.basic_model,
                 "testing": "testing context processor",
             }),
         )
 
         self.assertHTMLEqual(
             tpl,
-            wrap_adapter(request, adapters[5], {}, run_context_processors=True)
+            wrap_adapter(request, adapters[id], {}, run_context_processors=True)
         )
 
 
 class TestBlockAdapter(BaseFEditTest):
 
     def test_render(self):
+        id = get_adapter_id()
         streamfield = self.basic_model.content
         block = find_block(self.BLOCK_ID, streamfield)
         request = self.request_factory.get(
             self.get_editable_url(
                 self.basic_model.pk, self.basic_model._meta.app_label, self.basic_model._meta.model_name,
             )
         )
@@ -318,32 +432,33 @@
             request,
             FEDIT_PREVIEW_VAR,
             True,
         )
         block_value, _ = block
         template = Template(
             "{% load fedit %}"
-            "{% fedit test_block object.content block=block block_id=block_id id=5 %}"
+            f"{{% fedit test_block object.content block=block block_id=block_id id='{id}' %}}"
         )
 
         context = {
             "object": self.basic_model,
             "request": request,
             "block": block_value,
             "block_id": self.BLOCK_ID,
         }
 
         tpl = template.render(Context(context))
 
         self.assertHTMLEqual(
             tpl,
-            wrap_adapter(request, adapters[5], {})
+            wrap_adapter(request, adapters[id], {})
         )
 
     def test_render_as_var(self):
+        id = get_adapter_id()
         streamfield = self.basic_model.content
         block = find_block(self.BLOCK_ID, streamfield)
 
         request = self.request_factory.get(
             self.get_editable_url(
                 self.basic_model.pk, self.basic_model._meta.app_label, self.basic_model._meta.model_name,
             )
@@ -354,33 +469,34 @@
             request,
             FEDIT_PREVIEW_VAR,
             True,
         )
         block_value, _ = block
         template = Template(
             "{% load fedit %}"
-            "{% fedit test_block object.content block=block block_id=block_id id=6 as test %}"
+            f"{{% fedit test_block object.content block=block block_id=block_id id='{id}' as test %}}"
             "{{ test }}"
         )
 
         context = {
             "object": self.basic_model,
             "request": request,
             "block": block_value,
             "block_id": self.BLOCK_ID,
         }
 
         tpl = template.render(Context(context))
 
         self.assertHTMLEqual(
             tpl,
-            wrap_adapter(request, adapters[6], {})
+            wrap_adapter(request, adapters[id], {})
         )
 
     def test_render_from_context(self):
+        id = get_adapter_id()
         streamfield = self.basic_model.content
         block = find_block(self.BLOCK_ID, streamfield)
         request = self.request_factory.get(
             self.get_editable_url(
                 self.basic_model.pk, self.basic_model._meta.app_label, self.basic_model._meta.model_name,
             )
         )
@@ -389,15 +505,15 @@
             request,
             FEDIT_PREVIEW_VAR,
             True,
         )
         block_value, _ = block
         template = Template(
             "{% load fedit %}"
-            "{% fedit test_block from_context block=block block_id=block_id id=6 %}"
+            f"{{% fedit test_block from_context block=block block_id=block_id id='{id}' %}}"
         )
 
         context = {
             "object": self.basic_model,
             "request": request,
             "block": block_value,
             "block_id": self.BLOCK_ID,
@@ -405,31 +521,32 @@
             "wagtail_fedit_instance": self.basic_model,
         }
 
         tpl = template.render(Context(context))
 
         self.assertHTMLEqual(
             tpl,
-            wrap_adapter(request, adapters[6], context)
+            wrap_adapter(request, adapters[id], context)
         )
 
 
     def test_render_from_context_missing(self):
+        id = get_adapter_id()
         streamfield = self.basic_model.content
         block = find_block(self.BLOCK_ID, streamfield)
         request = self.request_factory.get(
             self.get_editable_url(
                 self.basic_model.pk, self.basic_model._meta.app_label, self.basic_model._meta.model_name,
             )
         )
         request.user = self.admin_user
         block_value, _ = block
         template = Template(
             "{% load fedit %}"
-            "{% fedit test_block from_context block=block block_id=block_id id=6 %}"
+            f"{{% fedit test_block from_context block=block block_id=block_id id='{id}' %}}"
         )
 
         context = {
             "object": self.basic_model,
             "request": request,
             "block": block_value,
             "block_id": self.BLOCK_ID,
@@ -442,185 +559,191 @@
             block_value.render(context),
         )
 
 
 class TestFieldAdapter(BaseFEditTest):
     
         def test_render(self):
+            id = get_adapter_id()
             request = self.request_factory.get(
                 self.get_editable_url(
                     self.basic_model.pk, self.basic_model._meta.app_label, self.basic_model._meta.model_name,
                 )
             )
             request.user = self.admin_user
             setattr(
                 request,
                 FEDIT_PREVIEW_VAR,
                 True,
             )
             template = Template(
                 "{% load fedit %}"
-                "{% fedit test_field object.title test=True id=7 %}"
+                f"{{% fedit test_field object.title test=True id='{id}' %}}"
             )
     
             context = {
                 "object": self.basic_model,
                 "request": request,
             }
     
             tpl = template.render(Context(context))
     
             self.assertHTMLEqual(
                 tpl,
-                wrap_adapter(request, adapters[7], {})
+                wrap_adapter(request, adapters[id], {})
             )
 
         def test_render_as_var(self):
+            id = get_adapter_id()
             request = self.request_factory.get(
                 self.get_editable_url(
                     self.basic_model.pk, self.basic_model._meta.app_label, self.basic_model._meta.model_name,
                 )
             )
             request.user = self.admin_user
             setattr(
                 request,
                 FEDIT_PREVIEW_VAR,
                 True,
             )
             template = Template(
                 "{% load fedit %}"
-                "{% fedit test_field object.title test=True id=8 as test %}"
+                f"{{% fedit test_field object.title test=True id='{id}' as test %}}"
                 "{{ test }}"
             )
     
             context = {
                 "object": self.basic_model,
                 "request": request,
             }
     
             tpl = template.render(Context(context))
     
             self.assertHTMLEqual(
                 tpl,
-                wrap_adapter(request, adapters[8], {})
+                wrap_adapter(request, adapters[id], {})
             )
 
         def test_render_related_field(self):
+            id = get_adapter_id()
             request = self.request_factory.get(
                 self.get_editable_url(
                     self.basic_model.pk, self.basic_model._meta.app_label, self.basic_model._meta.model_name,
                 )
             )
             request.user = self.admin_user
             setattr(
                 request,
                 FEDIT_PREVIEW_VAR,
                 True,
             )
             template = Template(
                 "{% load fedit %}"
-                "{% fedit test_field object.related_field test=True id=8 as test %}"
+                f"{{% fedit test_field object.related_field test=True id='{id}' as test %}}"
                 "{{ test }}"
             )
 
             context = {
                 "object": self.basic_model,
                 "request": request,
             }
     
             tpl = template.render(Context(context))
     
             self.assertHTMLEqual(
                 tpl,
-                wrap_adapter(request, adapters[8], {})
+                wrap_adapter(request, adapters[id], {})
             )
 
 class TestModelAdapter(BaseFEditTest):
     
         def test_render(self):
+            id = get_adapter_id()
             request = self.request_factory.get(
                 self.get_editable_url(
                     self.basic_model.pk, self.basic_model._meta.app_label, self.basic_model._meta.model_name,
                 )
             )
             request.user = self.admin_user
             setattr(
                 request,
                 FEDIT_PREVIEW_VAR,
                 True,
             )
             template = Template(
                 "{% load fedit %}"
-                "{% fedit test_model object test=True id=9 %}"
+                f"{{% fedit test_model object test=True id='{id}' %}}"
             )
     
             context = {
                 "object": self.basic_model,
                 "request": request,
             }
     
             tpl = template.render(Context(context))
     
             self.assertHTMLEqual(
                 tpl,
-                wrap_adapter(request, adapters[9], {})
+                wrap_adapter(request, adapters[id], {})
             )
     
         def test_render_as_var(self):
+            id = get_adapter_id()
             request = self.request_factory.get(
                 self.get_editable_url(
                     self.basic_model.pk, self.basic_model._meta.app_label, self.basic_model._meta.model_name,
                 )
             )
             request.user = self.admin_user
             setattr(
                 request,
                 FEDIT_PREVIEW_VAR,
                 True,
             )
             template = Template(
                 "{% load fedit %}"
-                "{% fedit test_model object test=True id=10 as test %}"
+                f"{{% fedit test_model object test=True id='{id}' as test %}}"
                 "{{ test }}"
             )
     
             context = {
                 "object": self.basic_model,
                 "request": request,
             }
     
             tpl = template.render(Context(context))
     
             self.assertHTMLEqual(
                 tpl,
-                wrap_adapter(request, adapters[10], {})
+                wrap_adapter(request, adapters[id], {})
             )
     
         def test_render_from_context(self):
+            id = get_adapter_id()
             request = self.request_factory.get(
                 self.get_editable_url(
                     self.basic_model.pk, self.basic_model._meta.app_label, self.basic_model._meta.model_name,
                 )
             )
             request.user = self.admin_user
             setattr(
                 request,
                 FEDIT_PREVIEW_VAR,
                 True,
             )
             template = Template(
                 "{% load fedit %}"
-                "{% fedit test_model from_context test=True id=11 %}"
+                f"{{% fedit test_model from_context test=True id='{id}' %}}"
             )
     
             context = {
                 "object": self.basic_model,
                 "request": request,
                 "wagtail_fedit_instance": self.basic_model,
             }
     
             tpl = template.render(Context(context))
     
             self.assertHTMLEqual(
                 tpl,
-                wrap_adapter(request, adapters[11], context)
+                wrap_adapter(request, adapters[id], context)
             )
```

### Comparing `wagtail_fedit-1.5.3rc9/wagtail_fedit/test/core/tests/test_block_edit.py` & `wagtail_fedit-1.5.4rc1/wagtail_fedit/test/core/tests/test_block_edit.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc9/wagtail_fedit/test/core/tests/test_blocks.py` & `wagtail_fedit-1.5.4rc1/wagtail_fedit/test/core/tests/test_blocks.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc9/wagtail_fedit/test/core/tests/test_field_edit.py` & `wagtail_fedit-1.5.4rc1/wagtail_fedit/test/core/tests/test_field_edit.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc9/wagtail_fedit/test/core/tests/test_generic.py` & `wagtail_fedit-1.5.4rc1/wagtail_fedit/test/core/tests/test_generic.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc9/wagtail_fedit/test/core/tests/test_revision.py` & `wagtail_fedit-1.5.4rc1/wagtail_fedit/test/core/tests/test_revision.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc9/wagtail_fedit/test/core/tests/test_submit.py` & `wagtail_fedit-1.5.4rc1/wagtail_fedit/test/core/tests/test_submit.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc9/wagtail_fedit/test/manage.py` & `wagtail_fedit-1.5.4rc1/wagtail_fedit/test/manage.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc9/wagtail_fedit/test/testapp/settings.py` & `wagtail_fedit-1.5.4rc1/wagtail_fedit/test/testapp/settings.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc9/wagtail_fedit/test/testapp/urls.py` & `wagtail_fedit-1.5.4rc1/wagtail_fedit/test/testapp/urls.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc9/wagtail_fedit/toolbar.py` & `wagtail_fedit-1.5.4rc1/wagtail_fedit/toolbar.py`

 * *Files 9% similar despite different names*

```diff
@@ -48,21 +48,29 @@
         This button is handled by the script in `wagtail_fedit/js/frontend.js`
     """
     template_name = "wagtail_fedit/content/buttons/edit_adapter.html"
     permissions = [
         "wagtailadmin.access_admin",
     ]
 
+
 class FeditAdapterAdminLinkButton(FeditAdapterComponent):
     """
         Required button class for the edit modal to function.
         This button is handled by the script in `wagtail_fedit/js/frontend.js`
     """
     template_name = "wagtail_fedit/content/buttons/admin_link.html"
     permissions = [
         "wagtailadmin.access_admin",
     ]
 
+    def __init__(self, request, adapter: "BaseAdapter"):
+        super().__init__(request, adapter)
+        self.url = adapter.get_admin_url()
+
+    def is_shown(self):
+        return super().is_shown() and bool(self.url)
+
     def get_context_data(self):
         return super().get_context_data() | {
-            "admin_url": self.adapter.get_admin_url(),
+            "admin_url": self.url,
         }
```

### Comparing `wagtail_fedit-1.5.3rc9/wagtail_fedit/urls.py` & `wagtail_fedit-1.5.4rc1/wagtail_fedit/urls.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc9/wagtail_fedit/utils.py` & `wagtail_fedit-1.5.4rc1/wagtail_fedit/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,14 +80,21 @@
         context = super().get_context_data(**kwargs)
         context["help_text"] = self.get_help_text()
         context["error_title"] = self.get_error_title()
         return context
     
     def get_error_title(self) -> str:
         return self.ERROR_TITLE
+    
+        
+    def get_header_title(self) -> str:
+        return _("Edit %(type)s '%(model)s'") % {
+            "type": self.object._meta.verbose_name,
+            "model": get_model_string(getattr(self, "absolute_instance", self.object), request=self.request),
+        }
 
     def get_help_text(self) -> str:
         # No relations. Maybe draft support.
         if is_draft_capable(getattr(self, "absolute_instance", self.object)):
             return {
                 "status": "warning",
                 "heading": self.HEADING_SUPPORTS_DRAFTS,
```

### Comparing `wagtail_fedit-1.5.3rc9/wagtail_fedit/views/adapters.py` & `wagtail_fedit-1.5.4rc1/wagtail_fedit/views/adapters.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc9/wagtail_fedit/views/editable.py` & `wagtail_fedit-1.5.4rc1/wagtail_fedit/views/editable.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc9/wagtail_fedit/views/mixins.py` & `wagtail_fedit-1.5.4rc1/wagtail_fedit/views/mixins.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc9/wagtail_fedit/wagtail_hooks/action_menu.py` & `wagtail_fedit-1.5.4rc1/wagtail_fedit/wagtail_hooks/action_menu.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc9/wagtail_fedit/wagtail_hooks/adapter_hooks.py` & `wagtail_fedit-1.5.4rc1/wagtail_fedit/wagtail_hooks/adapter_hooks.py`

 * *Files 18% similar despite different names*

```diff
@@ -74,10 +74,18 @@
     ]
 
 @hooks.register(REGISTER_JS, order=-1)
 def register_js(request):
     return [
         format_html(
             '<script src="{0}"></script>',
+            static('wagtail_fedit/vendor/tippy/popper.min.js')
+        ),
+        format_html(
+            '<script src="{0}"></script>',
+            static('wagtail_fedit/vendor/tippy/tippy-bundle.min.js')
+        ),
+        format_html(
+            '<script src="{0}"></script>',
             static('wagtail_fedit/js/frontend.js')
         ),
     ]
```

#### html2text {}

```diff
@@ -21,8 +21,10 @@
 RichTextField): return "large" if isinstance(model_field, StreamField): return
 "full" return None #
 #
 @hooks.register(REGISTER_CSS, order=-1) def register_css(request): return
 [ format_html( '
 ', static('wagtail_fedit/css/frontend.css') ), ] @hooks.register(REGISTER_JS,
 order=-1) def register_js(request): return [ format_html( '
+', static('wagtail_fedit/vendor/tippy/popper.min.js') ), format_html( '
+', static('wagtail_fedit/vendor/tippy/tippy-bundle.min.js') ), format_html( '
 ', static('wagtail_fedit/js/frontend.js') ), ]
```

### Comparing `wagtail_fedit-1.5.3rc9/wagtail_fedit/wagtail_hooks/log_actions.py` & `wagtail_fedit-1.5.4rc1/wagtail_fedit/wagtail_hooks/log_actions.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc9/wagtail_fedit/wagtail_hooks/userbar.py` & `wagtail_fedit-1.5.4rc1/wagtail_fedit/wagtail_hooks/userbar.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc9/wagtail_fedit.egg-info/PKG-INFO` & `wagtail_fedit-1.5.4rc1/wagtail_fedit.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wagtail-fedit
-Version: 1.5.3rc9
+Version: 1.5.4rc1
 Summary: Frontend editing for your Wagtail site
 Home-page: https://github.com/Nigel2392/wagtail_fedit
 Author: Nigel
 Author-email: nigel@goodadvice.it
 License: GPL-2.0-only
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
@@ -57,14 +57,15 @@
   - [Register CSS](#wagtail_feditregister_css)
   - [Register JS](#wagtail_feditregister_js)
   - [Field Editor Size](#wagtail_feditfield_editor_size)
 - [Settings](#settings)
   - [Sign Shared Context](#wagtail_fedit_sign_shared_context)
   - [Share With Sessions](#wagtail_fedit_share_with_sessions)
   - [Use Adapter Session ID](#wagtail_fedit_use_adapter_session_id)
+  - [Track Locales](#wagtail_fedit_track_locales)
 - [How your content is rendered](#how-your-content-is-rendered)
   - [Rendered output HTML](#rendered-editable-output-html)
 - [Implemented](#implemented)
 
 Getting Started
 ---------------
 
@@ -303,52 +304,49 @@
 Adapters can be defined anywhere; we recommend a separate `adapters.py` file.
 
 Adapter instances also have access to the following variables:
 
 * `self.object` - The model instance.
 * `self.field_name` - The field name.
 * `self.meta_field` - The models.Field instance.
-* `self.field_value` - The field value (Retrieved with `self.meta_field.value_from_object(self.object)`)
+* `self.field_value` - The field value (Retrieved with `getattr(self.object, self.field_name)`).
 * `self.request` - The django HTTP request object.
 * `self.kwargs` - Any shared context / keyword arguments for this adapter.
 
 ```python
 # myapp/adapters.py
 
 from wagtail_fedit.adapters import (
     BaseFieldFuncAdapter,
     VARIABLES,
 )
 
 class ColorizerAdapter(BaseFieldFuncAdapter):
-    # Required keyword arguments for the template tag are defined by the superclass.
-    # required_kwargs = [
-    #   "target",
-    #   "name", # the function name, override in __init__ method.
-    # ]
-
-    # Optional kwargs are used to inform inside of the adapter_help command.
-    # They are only for developer convenience.
-    # optional_kwargs = []
+    # Keywords for the adapter can easily be defined.
+    # These will be used to inform the templatetag on what is nescessary, required and counts as a flag.
+    keywords = (
+        Keyword(
+            "target",
+            help_text="The target element to apply the background-image to - this should be a css selector.",
+            type_hint="str",  # Type hint for the `adapter_help` command.
+            # optional=False, # Required is the default.
+            # absolute=False, # Counts as a keyword argument key=value instead of a boolean flag.
+            # default=None,   # Default value if not provided, only for optional keyword arguments.
+        ),
+    )
 
     # How the adapter will be adressed inside of the template tag.
     identifier = "colorizer"
 
+    # The function to call in javascript.
+    js_function = "myColorizerJavascriptFunction"
+
     # A simple description of what this adapter does.
     usage_description = "Change the color of the text for the given target element."
 
-    # Optional explanation of keyword arguments
-    help_text_dict = {
-        "target": "The target element to apply the color to.",
-    }
-
-    def __init__(self, object, field_name: str, request: HttpRequest, **kwargs):
-        kwargs["name"] = "myColorizerJavascriptFunction"
-        super().__init__(object, field_name, request, **kwargs)
-
     def render_content(self, parent_context=None):
         # This is not required; we will replace a CSS variable; thus we are not returning any actual content.
         return ""
   
     def get_response_data(self, parent_context=None):
         """
         Return the data to be sent to the frontend adapter.
@@ -591,14 +589,26 @@
 Default: `True`
 
 Use the get_element_id method of the adapter to generate a session ID.
 *This could __maybe__ interfere with other editable- block's session data, but is highly unlikely!*
 This is useful to not clutter session data too much.
 If `False`, the session ID will be generated each time the page is loaded.
 
+### `WAGTAIL_FEDIT_TRACK_LOCALES`
+
+Default: `False`
+
+Track the locales of the users across the views.
+
+**This sets the initial request.LANGUAGE_CODE (if available) in the shared context.**
+
+If this is false, there is no guarantee that the language of a saved field/model
+will be the same as it initially was, generally it will be - however this might mess up with Wagtail's `Page.locale` and
+the page not being available in the context afterwards.
+
 ## How your content is rendered
 
 (**Maintainer's note:** In my experience this doesn't mess the CSS up too much, or even at all for most content - **if** you don't get hyperspecific with your CSS selectors and structure your templates well.)
 
 Your block and field are wrapped in a `div`, any CSS for your templates should keep this in mind.
 
 ### Rendered editable output HTML
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: wagtail-fedit Version: 1.5.3rc9 Summary: Frontend
+Metadata-Version: 2.1 Name: wagtail-fedit Version: 1.5.4rc1 Summary: Frontend
 editing for your Wagtail site Home-page: https://github.com/Nigel2392/
 wagtail_fedit Author: Nigel Author-email: nigel@goodadvice.it License: GPL-2.0-
 only Classifier: Environment :: Web Environment Classifier: Framework :: Django
 Classifier: Framework :: Django :: 4.2 Classifier: Framework :: Wagtail
 Classifier: Framework :: Wagtail :: 5 Classifier: Framework :: Wagtail :: 6
 Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
 :: GNU General Public License v2 or later (GPLv2+) Classifier: Operating System
@@ -28,17 +28,18 @@
 (#wagtail_feditregister_field_widgets) - [Exclude Related Forms]
 (#wagtail_feditexclude_related_forms) - [Action Menu Item Is Shown]
 (#wagtail_feditaction_menu_item_is_shown) - [Register CSS]
 (#wagtail_feditregister_css) - [Register JS](#wagtail_feditregister_js) -
 [Field Editor Size](#wagtail_feditfield_editor_size) - [Settings](#settings) -
 [Sign Shared Context](#wagtail_fedit_sign_shared_context) - [Share With
 Sessions](#wagtail_fedit_share_with_sessions) - [Use Adapter Session ID]
-(#wagtail_fedit_use_adapter_session_id) - [How your content is rendered](#how-
-your-content-is-rendered) - [Rendered output HTML](#rendered-editable-output-
-html) - [Implemented](#implemented) Getting Started --------------- 1. Add
+(#wagtail_fedit_use_adapter_session_id) - [Track Locales]
+(#wagtail_fedit_track_locales) - [How your content is rendered](#how-your-
+content-is-rendered) - [Rendered output HTML](#rendered-editable-output-html) -
+[Implemented](#implemented) Getting Started --------------- 1. Add
 'wagtail_fedit' to your INSTALLED_APPS setting like this: ``` INSTALLED_APPS =
 [ ..., 'wagtail_fedit', ] ``` 2. Run `py ./manage.py collectstatic`. 3. Run `py
 ./manage.py adapter_help` to see all your options and their requirements. ##
 Getting Editing! 1. If you want to get into the frontend-editing interface for
 a model it must inherit from `PreviewableMixin`. **This is a requirement.** It
 is however not always required for your model to inherit from
 `PreviewableMixin`. **Any model can be edited**; you just can't access the
@@ -136,53 +137,53 @@
 colorizer page.color target=".my-colorized-div" %}
 ************ CCoolloorriizzeedd TTeexxtt!! ************
 ... ``` ### Adapters Python We will get started creating the adapter
 definition. Adapters can be defined anywhere; we recommend a separate
 `adapters.py` file. Adapter instances also have access to the following
 variables: * `self.object` - The model instance. * `self.field_name` - The
 field name. * `self.meta_field` - The models.Field instance. *
-`self.field_value` - The field value (Retrieved with
-`self.meta_field.value_from_object(self.object)`) * `self.request` - The django
-HTTP request object. * `self.kwargs` - Any shared context / keyword arguments
-for this adapter. ```python # myapp/adapters.py from wagtail_fedit.adapters
-import ( BaseFieldFuncAdapter, VARIABLES, ) class ColorizerAdapter
-(BaseFieldFuncAdapter): # Required keyword arguments for the template tag are
-defined by the superclass. # required_kwargs = [ # "target", # "name", # the
-function name, override in __init__ method. # ] # Optional kwargs are used to
-inform inside of the adapter_help command. # They are only for developer
-convenience. # optional_kwargs = [] # How the adapter will be adressed inside
-of the template tag. identifier = "colorizer" # A simple description of what
-this adapter does. usage_description = "Change the color of the text for the
-given target element." # Optional explanation of keyword arguments
-help_text_dict = { "target": "The target element to apply the color to.", } def
-__init__(self, object, field_name: str, request: HttpRequest, **kwargs): kwargs
-["name"] = "myColorizerJavascriptFunction" super().__init__(object, field_name,
-request, **kwargs) def render_content(self, parent_context=None): # This is not
-required; we will replace a CSS variable; thus we are not returning any actual
-content. return "" def get_response_data(self, parent_context=None): """ Return
-the data to be sent to the frontend adapter. """ data = super
-().get_response_data(parent_context) return data | { "color": self.field_value,
-} def get_form_attrs(self) -> dict: """ Return form attributes for the form
-inside of the edit modal. This can be used to control editor size. """ attrs =
-super().get_form_attrs() attrs[VARIABLES.FORM_SIZE_VAR] = "full" # Fullscreen,
-there is also `large`. return attrs ``` We must then register the adapter to
-make sure it is available for templates. This should be done in a
+`self.field_value` - The field value (Retrieved with `getattr(self.object,
+self.field_name)`). * `self.request` - The django HTTP request object. *
+`self.kwargs` - Any shared context / keyword arguments for this adapter.
+```python # myapp/adapters.py from wagtail_fedit.adapters import
+( BaseFieldFuncAdapter, VARIABLES, ) class ColorizerAdapter
+(BaseFieldFuncAdapter): # Keywords for the adapter can easily be defined. #
+These will be used to inform the templatetag on what is nescessary, required
+and counts as a flag. keywords = ( Keyword( "target", help_text="The target
+element to apply the background-image to - this should be a css selector.",
+type_hint="str", # Type hint for the `adapter_help` command. # optional=False,
+# Required is the default. # absolute=False, # Counts as a keyword argument
+key=value instead of a boolean flag. # default=None, # Default value if not
+provided, only for optional keyword arguments. ), ) # How the adapter will be
+adressed inside of the template tag. identifier = "colorizer" # The function to
+call in javascript. js_function = "myColorizerJavascriptFunction" # A simple
+description of what this adapter does. usage_description = "Change the color of
+the text for the given target element." def render_content(self,
+parent_context=None): # This is not required; we will replace a CSS variable;
+thus we are not returning any actual content. return "" def get_response_data
+(self, parent_context=None): """ Return the data to be sent to the frontend
+adapter. """ data = super().get_response_data(parent_context) return data |
+{ "color": self.field_value, } def get_form_attrs(self) -> dict: """ Return
+form attributes for the form inside of the edit modal. This can be used to
+control editor size. """ attrs = super().get_form_attrs() attrs
+[VARIABLES.FORM_SIZE_VAR] = "full" # Fullscreen, there is also `large`. return
+attrs ``` We must then register the adapter to make sure it is available for
+templates. This should be done in a `wagtail_hooks.py` file. ```python # myapp/
+wagtail_hooks.py from wagtail_fedit.adapters import adapter_registry from
+myapp.adapters import ColorizerAdapter adapter_registry.register
+(ColorizerAdapter) ``` ### Adapters Javascript We now need to create the
+javascript function to actually apply the color to the styles of the element.
+This function will be called `myColorizerJavascriptFunction`, as defined in the
+adapter's `__init__` method. ```javascript // myapp/static/myapp/js/custom.js
+function myColorizerJavascriptFunction(element, response) { element.style.color
+= response.color; } ``` We must then register this javascript file to be
+included in the frontend editing interface. This should be done in a
 `wagtail_hooks.py` file. ```python # myapp/wagtail_hooks.py from
-wagtail_fedit.adapters import adapter_registry from myapp.adapters import
-ColorizerAdapter adapter_registry.register(ColorizerAdapter) ``` ### Adapters
-Javascript We now need to create the javascript function to actually apply the
-color to the styles of the element. This function will be called
-`myColorizerJavascriptFunction`, as defined in the adapter's `__init__` method.
-```javascript // myapp/static/myapp/js/custom.js function
-myColorizerJavascriptFunction(element, response) { element.style.color =
-response.color; } ``` We must then register this javascript file to be included
-in the frontend editing interface. This should be done in a `wagtail_hooks.py`
-file. ```python # myapp/wagtail_hooks.py from django.utils.html import
-format_html from django.templatetags.static import static from
-wagtail_fedit.hooks import REGISTER_JS from wagtail import hooks
+django.utils.html import format_html from django.templatetags.static import
+static from wagtail_fedit.hooks import REGISTER_JS from wagtail import hooks
 @hooks.register(REGISTER_JS) def register_js(request): return [ format_html( '
 ', static('myapp/js/custom.js') ), ] ``` ## Hooks ###
 wagtail_fedit.construct_adapter_toolbar Construct the toolbar for the given
 adapter. This is used to display the edit icon for the given adapter. How it is
 called: ```python items = [ FeditAdapterEditButton(), ] for hook in
 hooks.get_hooks(CONSTRUCT_ADAPTER_TOOLBAR): hook(items=items, adapter=adapter)
 ``` ### wagtail_fedit.register_type_renderer Register a custom renderer for a
@@ -237,20 +238,26 @@
 Default: `False` Share the context through the session data. This is useful if
 you are running into limits with the URL length. This will store the context in
 the session and pass the session key to the iFrame instead of the context. ###
 `WAGTAIL_FEDIT_USE_ADAPTER_SESSION_ID` Default: `True` Use the get_element_id
 method of the adapter to generate a session ID. *This could __maybe__ interfere
 with other editable- block's session data, but is highly unlikely!* This is
 useful to not clutter session data too much. If `False`, the session ID will be
-generated each time the page is loaded. ## How your content is rendered
-(**Maintainer's note:** In my experience this doesn't mess the CSS up too much,
-or even at all for most content - **if** you don't get hyperspecific with your
-CSS selectors and structure your templates well.) Your block and field are
-wrapped in a `div`, any CSS for your templates should keep this in mind. ###
-Rendered editable output HTML ```html {% load fedit %}
+generated each time the page is loaded. ### `WAGTAIL_FEDIT_TRACK_LOCALES`
+Default: `False` Track the locales of the users across the views. **This sets
+the initial request.LANGUAGE_CODE (if available) in the shared context.** If
+this is false, there is no guarantee that the language of a saved field/model
+will be the same as it initially was, generally it will be - however this might
+mess up with Wagtail's `Page.locale` and the page not being available in the
+context afterwards. ## How your content is rendered (**Maintainer's note:** In
+my experience this doesn't mess the CSS up too much, or even at all for most
+content - **if** you don't get hyperspecific with your CSS selectors and
+structure your templates well.) Your block and field are wrapped in a `div`,
+any CSS for your templates should keep this in mind. ### Rendered editable
+output HTML ```html {% load fedit %}
 % if shared %} data-shared-context="{{ shared }}"{%endif%} data-edit-url="{
 { edit_url }}">
 {% for button in buttons %} {{ button }} {% endfor %}
 {% render_adapter adapter %}
 ``` ## Implemented * Revision Support * Locked Support * Draft Support *
 Preview Support * Workflow Support * Permissions * Audit Logs * Full block
 capabilities on Frontend Editing
```

### Comparing `wagtail_fedit-1.5.3rc9/wagtail_fedit.egg-info/SOURCES.txt` & `wagtail_fedit-1.5.4rc1/wagtail_fedit.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -32,14 +32,17 @@
 wagtail_fedit/locale/nl/LC_MESSAGES/django.po
 wagtail_fedit/migrations/__init__.py
 wagtail_fedit/migrations/__pycache__/__init__.cpython-311.pyc
 wagtail_fedit/static/wagtail_fedit/css/frontend.css
 wagtail_fedit/static/wagtail_fedit/css/furniture.css
 wagtail_fedit/static/wagtail_fedit/css/userbar-menu.css
 wagtail_fedit/static/wagtail_fedit/js/frontend.js
+wagtail_fedit/static/wagtail_fedit/vendor/tippy/LICENSE
+wagtail_fedit/static/wagtail_fedit/vendor/tippy/popper.min.js
+wagtail_fedit/static/wagtail_fedit/vendor/tippy/tippy-bundle.min.js
 wagtail_fedit/templates/wagtail_fedit/_hook_output.html
 wagtail_fedit/templates/wagtail_fedit/content/editable_adapter.html
 wagtail_fedit/templates/wagtail_fedit/content/buttons/admin_link.html
 wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_adapter.html
 wagtail_fedit/templates/wagtail_fedit/editor/action_confirm.html
 wagtail_fedit/templates/wagtail_fedit/editor/action_publish_confirm.html
 wagtail_fedit/templates/wagtail_fedit/editor/adapter_edit_handler.html
@@ -74,14 +77,15 @@
 wagtail_fedit/test/core/tests/__init__.py
 wagtail_fedit/test/core/tests/base.py
 wagtail_fedit/test/core/tests/test_adapters.py
 wagtail_fedit/test/core/tests/test_block_edit.py
 wagtail_fedit/test/core/tests/test_blocks.py
 wagtail_fedit/test/core/tests/test_field_edit.py
 wagtail_fedit/test/core/tests/test_generic.py
+wagtail_fedit/test/core/tests/test_model_edit.py
 wagtail_fedit/test/core/tests/test_revision.py
 wagtail_fedit/test/core/tests/test_submit.py
 wagtail_fedit/test/testapp/__init__.py
 wagtail_fedit/test/testapp/asgi.py
 wagtail_fedit/test/testapp/settings.py
 wagtail_fedit/test/testapp/urls.py
 wagtail_fedit/test/testapp/wsgi.py
```

