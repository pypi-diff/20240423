# Comparing `tmp/wagtail_fedit-1.5.3rc8.tar.gz` & `tmp/wagtail_fedit-1.5.3rc9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wagtail_fedit-1.5.3rc8.tar", last modified: Sun Apr 21 07:56:53 2024, max compression
+gzip compressed data, was "wagtail_fedit-1.5.3rc9.tar", last modified: Sun Apr 21 21:47:14 2024, max compression
```

## Comparing `wagtail_fedit-1.5.3rc8.tar` & `wagtail_fedit-1.5.3rc9.tar`

### file list

```diff
@@ -1,127 +1,131 @@
-drwxrwxrwx   0        0        0        0 2024-04-21 07:56:53.614204 wagtail_fedit-1.5.3rc8/
--rw-rw-rw-   0        0        0    18429 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.3rc8/LICENSE
--rw-rw-rw-   0        0        0      257 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.3rc8/MANIFEST.in
--rw-rw-rw-   0        0        0    20741 2024-04-21 07:56:53.612769 wagtail_fedit-1.5.3rc8/PKG-INFO
--rw-rw-rw-   0        0        0    19483 2024-04-21 02:27:07.000000 wagtail_fedit-1.5.3rc8/README.md
--rw-rw-rw-   0        0        0       90 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.3rc8/pyproject.toml
--rw-rw-rw-   0        0        0     1189 2024-04-21 07:56:53.639382 wagtail_fedit-1.5.3rc8/setup.cfg
--rw-rw-rw-   0        0        0       39 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.3rc8/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-21 07:56:52.439307 wagtail_fedit-1.5.3rc8/wagtail_fedit/
--rw-rw-rw-   0        0        0        0 2024-03-29 20:13:25.000000 wagtail_fedit-1.5.3rc8/wagtail_fedit/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-21 07:56:52.535109 wagtail_fedit-1.5.3rc8/wagtail_fedit/adapters/
--rw-rw-rw-   0        0        0      473 2024-04-18 15:33:48.000000 wagtail_fedit-1.5.3rc8/wagtail_fedit/adapters/__init__.py
--rw-rw-rw-   0        0        0    10463 2024-04-21 01:05:15.000000 wagtail_fedit-1.5.3rc8/wagtail_fedit/adapters/base.py
--rw-rw-rw-   0        0        0     6279 2024-04-20 13:16:40.000000 wagtail_fedit-1.5.3rc8/wagtail_fedit/adapters/block.py
--rw-rw-rw-   0        0        0     8677 2024-04-18 20:24:49.000000 wagtail_fedit-1.5.3rc8/wagtail_fedit/adapters/field.py
--rw-rw-rw-   0        0        0     1908 2024-04-21 07:55:42.000000 wagtail_fedit-1.5.3rc8/wagtail_fedit/adapters/funcs.py
--rw-rw-rw-   0        0        0     2546 2024-04-20 13:17:28.000000 wagtail_fedit-1.5.3rc8/wagtail_fedit/adapters/misc.py
--rw-rw-rw-   0        0        0     1595 2024-04-18 20:22:37.000000 wagtail_fedit-1.5.3rc8/wagtail_fedit/adapters/registry.py
--rw-rw-rw-   0        0        0      163 2024-03-29 20:13:25.000000 wagtail_fedit-1.5.3rc8/wagtail_fedit/apps.py
-drwxrwxrwx   0        0        0        0 2024-04-21 07:56:52.570669 wagtail_fedit-1.5.3rc8/wagtail_fedit/forms/
--rw-rw-rw-   0        0        0       71 2024-04-02 19:03:21.000000 wagtail_fedit-1.5.3rc8/wagtail_fedit/forms/__init__.py
--rw-rw-rw-   0        0        0     2881 2024-04-18 20:27:35.000000 wagtail_fedit-1.5.3rc8/wagtail_fedit/forms/blocks.py
--rw-rw-rw-   0        0        0     3110 2024-04-21 02:24:44.000000 wagtail_fedit-1.5.3rc8/wagtail_fedit/forms/fields.py
--rw-rw-rw-   0        0        0     4617 2024-04-21 02:08:33.000000 wagtail_fedit-1.5.3rc8/wagtail_fedit/hooks.py
-drwxrwxrwx   0        0        0        0 2024-04-21 07:56:52.294967 wagtail_fedit-1.5.3rc8/wagtail_fedit/locale/
-drwxrwxrwx   0        0        0        0 2024-04-21 07:56:52.296055 wagtail_fedit-1.5.3rc8/wagtail_fedit/locale/nl/
-drwxrwxrwx   0        0        0        0 2024-04-21 07:56:52.585574 wagtail_fedit-1.5.3rc8/wagtail_fedit/locale/nl/LC_MESSAGES/
--rw-rw-rw-   0        0        0     7129 2024-04-11 09:05:50.000000 wagtail_fedit-1.5.3rc8/wagtail_fedit/locale/nl/LC_MESSAGES/django.mo
--rw-rw-rw-   0        0        0    12687 2024-04-11 09:05:42.000000 wagtail_fedit-1.5.3rc8/wagtail_fedit/locale/nl/LC_MESSAGES/django.po
-drwxrwxrwx   0        0        0        0 2024-04-21 07:56:52.589274 wagtail_fedit-1.5.3rc8/wagtail_fedit/migrations/
--rw-rw-rw-   0        0        0        0 2024-03-29 20:13:25.000000 wagtail_fedit-1.5.3rc8/wagtail_fedit/migrations/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-21 07:56:52.591327 wagtail_fedit-1.5.3rc8/wagtail_fedit/migrations/__pycache__/
--rw-rw-rw-   0        0        0      215 2024-03-29 21:05:00.000000 wagtail_fedit-1.5.3rc8/wagtail_fedit/migrations/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0        0        0     3170 2024-04-05 20:30:10.000000 wagtail_fedit-1.5.3rc8/wagtail_fedit/models.py
--rw-rw-rw-   0        0        0      973 2024-04-21 00:46:27.000000 wagtail_fedit-1.5.3rc8/wagtail_fedit/settings.py
-drwxrwxrwx   0        0        0        0 2024-04-21 07:56:52.299766 wagtail_fedit-1.5.3rc8/wagtail_fedit/static/
-drwxrwxrwx   0        0        0        0 2024-04-21 07:56:52.301055 wagtail_fedit-1.5.3rc8/wagtail_fedit/static/wagtail_fedit/
-drwxrwxrwx   0        0        0        0 2024-04-21 07:56:52.628965 wagtail_fedit-1.5.3rc8/wagtail_fedit/static/wagtail_fedit/css/
--rw-rw-rw-   0        0        0     5388 2024-04-19 20:19:25.000000 wagtail_fedit-1.5.3rc8/wagtail_fedit/static/wagtail_fedit/css/frontend.css
--rw-rw-rw-   0        0        0     5098 2024-04-17 20:40:49.000000 wagtail_fedit-1.5.3rc8/wagtail_fedit/static/wagtail_fedit/css/furniture.css
--rw-rw-rw-   0        0        0     1266 2024-04-05 19:37:44.000000 wagtail_fedit-1.5.3rc8/wagtail_fedit/static/wagtail_fedit/css/userbar-menu.css
-drwxrwxrwx   0        0        0        0 2024-04-21 07:56:52.656360 wagtail_fedit-1.5.3rc8/wagtail_fedit/static/wagtail_fedit/js/
--rw-rw-rw-   0        0        0    19663 2024-04-20 12:39:36.000000 wagtail_fedit-1.5.3rc8/wagtail_fedit/static/wagtail_fedit/js/frontend.js
-drwxrwxrwx   0        0        0        0 2024-04-21 07:56:52.303512 wagtail_fedit-1.5.3rc8/wagtail_fedit/templates/
-drwxrwxrwx   0        0        0        0 2024-04-21 07:56:52.659879 wagtail_fedit-1.5.3rc8/wagtail_fedit/templates/wagtail_fedit/
--rw-rw-rw-   0        0        0       56 2024-04-16 18:37:39.000000 wagtail_fedit-1.5.3rc8/wagtail_fedit/templates/wagtail_fedit/_hook_output.html
-drwxrwxrwx   0        0        0        0 2024-04-21 07:56:52.668646 wagtail_fedit-1.5.3rc8/wagtail_fedit/templates/wagtail_fedit/content/
-drwxrwxrwx   0        0        0        0 2024-04-21 07:56:52.703891 wagtail_fedit-1.5.3rc8/wagtail_fedit/templates/wagtail_fedit/content/buttons/
--rw-rw-rw-   0        0        0      871 2024-04-19 20:16:18.000000 wagtail_fedit-1.5.3rc8/wagtail_fedit/templates/wagtail_fedit/content/buttons/admin_link.html
--rw-rw-rw-   0        0        0      872 2024-04-19 20:15:44.000000 wagtail_fedit-1.5.3rc8/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_adapter.html
--rw-rw-rw-   0        0        0      513 2024-04-18 15:42:23.000000 wagtail_fedit-1.5.3rc8/wagtail_fedit/templates/wagtail_fedit/content/editable_adapter.html
-drwxrwxrwx   0        0        0        0 2024-04-21 07:56:52.791297 wagtail_fedit-1.5.3rc8/wagtail_fedit/templates/wagtail_fedit/editor/
--rw-rw-rw-   0        0        0     2259 2024-04-11 08:02:26.000000 wagtail_fedit-1.5.3rc8/wagtail_fedit/templates/wagtail_fedit/editor/action_confirm.html
--rw-rw-rw-   0        0        0     3699 2024-04-20 21:55:10.000000 wagtail_fedit-1.5.3rc8/wagtail_fedit/templates/wagtail_fedit/editor/action_publish_confirm.html
--rw-rw-rw-   0        0        0      566 2024-04-21 00:09:10.000000 wagtail_fedit-1.5.3rc8/wagtail_fedit/templates/wagtail_fedit/editor/adapter_form.html
--rw-rw-rw-   0        0        0      455 2024-04-21 00:11:35.000000 wagtail_fedit-1.5.3rc8/wagtail_fedit/templates/wagtail_fedit/editor/adapter_form_errors.html
--rw-rw-rw-   0        0        0      330 2024-04-21 00:12:14.000000 wagtail_fedit-1.5.3rc8/wagtail_fedit/templates/wagtail_fedit/editor/adapter_iframe.html
--rw-rw-rw-   0        0        0     5271 2024-04-21 00:11:24.000000 wagtail_fedit-1.5.3rc8/wagtail_fedit/templates/wagtail_fedit/editor/base_iframe.html
--rw-rw-rw-   0        0        0      496 2024-04-02 17:46:59.000000 wagtail_fedit-1.5.3rc8/wagtail_fedit/templates/wagtail_fedit/editor/field.html
-drwxrwxrwx   0        0        0        0 2024-04-21 07:56:52.825413 wagtail_fedit-1.5.3rc8/wagtail_fedit/templates/wagtail_fedit/icons/
--rw-rw-rw-   0        0        0      797 2024-04-11 08:36:19.000000 wagtail_fedit-1.5.3rc8/wagtail_fedit/templates/wagtail_fedit/icons/fedit-check-list.svg
--rw-rw-rw-   0        0        0      584 2024-04-11 08:36:55.000000 wagtail_fedit-1.5.3rc8/wagtail_fedit/templates/wagtail_fedit/icons/fedit-eye-closed.svg
--rw-rw-rw-   0        0        0      377 2024-04-11 08:23:07.000000 wagtail_fedit-1.5.3rc8/wagtail_fedit/templates/wagtail_fedit/icons/fedit-eye-open.svg
--rw-rw-rw-   0        0        0      725 2024-04-11 09:02:58.000000 wagtail_fedit-1.5.3rc8/wagtail_fedit/templates/wagtail_fedit/icons/fedit-save.svg
--rw-rw-rw-   0        0        0     1323 2024-04-11 08:36:52.000000 wagtail_fedit-1.5.3rc8/wagtail_fedit/templates/wagtail_fedit/icons/fedit-stop-sign.svg
-drwxrwxrwx   0        0        0        0 2024-04-21 07:56:52.848534 wagtail_fedit-1.5.3rc8/wagtail_fedit/templates/wagtail_fedit/userbar/
--rw-rw-rw-   0        0        0      867 2024-04-03 17:05:21.000000 wagtail_fedit-1.5.3rc8/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit.html
--rw-rw-rw-   0        0        0      876 2024-04-03 16:59:31.000000 wagtail_fedit-1.5.3rc8/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_view_live.html
-drwxrwxrwx   0        0        0        0 2024-04-21 07:56:52.870307 wagtail_fedit-1.5.3rc8/wagtail_fedit/templates/wagtail_fedit/userbar/publish/
--rw-rw-rw-   0        0        0      263 2024-04-11 08:24:35.000000 wagtail_fedit-1.5.3rc8/wagtail_fedit/templates/wagtail_fedit/userbar/publish/action_button.html
--rw-rw-rw-   0        0        0      967 2024-04-11 09:03:51.000000 wagtail_fedit-1.5.3rc8/wagtail_fedit/templates/wagtail_fedit/userbar/publish/item_fedit_publishing.html
-drwxrwxrwx   0        0        0        0 2024-04-21 07:56:52.885889 wagtail_fedit-1.5.3rc8/wagtail_fedit/templatetags/
--rw-rw-rw-   0        0        0        0 2024-03-29 20:13:42.000000 wagtail_fedit-1.5.3rc8/wagtail_fedit/templatetags/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-21 07:56:52.890841 wagtail_fedit-1.5.3rc8/wagtail_fedit/templatetags/__pycache__/
--rw-rw-rw-   0        0        0      217 2024-03-29 21:05:00.000000 wagtail_fedit-1.5.3rc8/wagtail_fedit/templatetags/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0        0        0    10817 2024-04-21 01:26:50.000000 wagtail_fedit-1.5.3rc8/wagtail_fedit/templatetags/__pycache__/fedit.cpython-311.pyc
--rw-rw-rw-   0        0        0     7961 2024-04-21 01:25:52.000000 wagtail_fedit-1.5.3rc8/wagtail_fedit/templatetags/fedit.py
-drwxrwxrwx   0        0        0        0 2024-04-21 07:56:52.905588 wagtail_fedit-1.5.3rc8/wagtail_fedit/test/
--rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.3rc8/wagtail_fedit/test/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-21 07:56:52.957613 wagtail_fedit-1.5.3rc8/wagtail_fedit/test/core/
--rw-rw-rw-   0        0        0      151 2024-04-05 07:59:49.000000 wagtail_fedit-1.5.3rc8/wagtail_fedit/test/core/__init__.py
--rw-rw-rw-   0        0        0      165 2024-04-05 08:41:40.000000 wagtail_fedit-1.5.3rc8/wagtail_fedit/test/core/apps.py
--rw-rw-rw-   0        0        0      130 2024-04-15 20:12:38.000000 wagtail_fedit-1.5.3rc8/wagtail_fedit/test/core/context_processors.py
-drwxrwxrwx   0        0        0        0 2024-04-21 07:56:52.981617 wagtail_fedit-1.5.3rc8/wagtail_fedit/test/core/migrations/
--rw-rw-rw-   0        0        0    12115 2024-04-20 22:33:35.000000 wagtail_fedit-1.5.3rc8/wagtail_fedit/test/core/migrations/0001_initial.py
--rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.3rc8/wagtail_fedit/test/core/migrations/__init__.py
--rw-rw-rw-   0        0        0     5389 2024-04-20 21:34:01.000000 wagtail_fedit-1.5.3rc8/wagtail_fedit/test/core/models.py
-drwxrwxrwx   0        0        0        0 2024-04-21 07:56:53.140949 wagtail_fedit-1.5.3rc8/wagtail_fedit/test/core/tests/
--rw-rw-rw-   0        0        0        0 2024-04-05 07:59:29.000000 wagtail_fedit-1.5.3rc8/wagtail_fedit/test/core/tests/__init__.py
--rw-rw-rw-   0        0        0     7885 2024-04-20 21:42:28.000000 wagtail_fedit-1.5.3rc8/wagtail_fedit/test/core/tests/base.py
--rw-rw-rw-   0        0        0    14761 2024-04-21 01:30:53.000000 wagtail_fedit-1.5.3rc8/wagtail_fedit/test/core/tests/test_adapters.py
--rw-rw-rw-   0        0        0     4320 2024-04-06 22:44:26.000000 wagtail_fedit-1.5.3rc8/wagtail_fedit/test/core/tests/test_block_edit.py
--rw-rw-rw-   0        0        0     5664 2024-04-05 10:31:29.000000 wagtail_fedit-1.5.3rc8/wagtail_fedit/test/core/tests/test_blocks.py
--rw-rw-rw-   0        0        0     3642 2024-04-05 18:00:23.000000 wagtail_fedit-1.5.3rc8/wagtail_fedit/test/core/tests/test_field_edit.py
--rw-rw-rw-   0        0        0     3709 2024-04-10 13:03:30.000000 wagtail_fedit-1.5.3rc8/wagtail_fedit/test/core/tests/test_generic.py
--rw-rw-rw-   0        0        0     1574 2024-04-20 20:49:12.000000 wagtail_fedit-1.5.3rc8/wagtail_fedit/test/core/tests/test_revision.py
--rw-rw-rw-   0        0        0     9545 2024-04-20 21:54:40.000000 wagtail_fedit-1.5.3rc8/wagtail_fedit/test/core/tests/test_submit.py
--rw-rw-rw-   0        0        0      704 2024-04-05 17:55:36.000000 wagtail_fedit-1.5.3rc8/wagtail_fedit/test/manage.py
-drwxrwxrwx   0        0        0        0 2024-04-21 07:56:53.218890 wagtail_fedit-1.5.3rc8/wagtail_fedit/test/testapp/
--rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.3rc8/wagtail_fedit/test/testapp/__init__.py
--rw-rw-rw-   0        0        0      407 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.3rc8/wagtail_fedit/test/testapp/asgi.py
--rw-rw-rw-   0        0        0     3625 2024-04-15 20:14:41.000000 wagtail_fedit-1.5.3rc8/wagtail_fedit/test/testapp/settings.py
--rw-rw-rw-   0        0        0      897 2024-04-05 08:04:53.000000 wagtail_fedit-1.5.3rc8/wagtail_fedit/test/testapp/urls.py
--rw-rw-rw-   0        0        0      407 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.3rc8/wagtail_fedit/test/testapp/wsgi.py
--rw-rw-rw-   0        0        0     2009 2024-04-19 20:04:30.000000 wagtail_fedit-1.5.3rc8/wagtail_fedit/toolbar.py
--rw-rw-rw-   0        0        0      777 2024-04-13 10:38:39.000000 wagtail_fedit-1.5.3rc8/wagtail_fedit/urls.py
--rw-rw-rw-   0        0        0    16719 2024-04-20 21:53:34.000000 wagtail_fedit-1.5.3rc8/wagtail_fedit/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-21 07:56:53.361942 wagtail_fedit-1.5.3rc8/wagtail_fedit/views/
--rw-rw-rw-   0        0        0      190 2024-04-13 19:36:44.000000 wagtail_fedit-1.5.3rc8/wagtail_fedit/views/__init__.py
--rw-rw-rw-   0        0        0     6551 2024-04-21 00:08:49.000000 wagtail_fedit-1.5.3rc8/wagtail_fedit/views/adapters.py
--rw-rw-rw-   0        0        0    17494 2024-04-20 21:54:53.000000 wagtail_fedit-1.5.3rc8/wagtail_fedit/views/editable.py
--rw-rw-rw-   0        0        0     1458 2024-04-05 20:53:30.000000 wagtail_fedit-1.5.3rc8/wagtail_fedit/views/mixins.py
-drwxrwxrwx   0        0        0        0 2024-04-21 07:56:53.603680 wagtail_fedit-1.5.3rc8/wagtail_fedit/wagtail_hooks/
--rw-rw-rw-   0        0        0      184 2024-04-16 10:03:02.000000 wagtail_fedit-1.5.3rc8/wagtail_fedit/wagtail_hooks/__init__.py
--rw-rw-rw-   0        0        0     1748 2024-04-06 18:37:13.000000 wagtail_fedit-1.5.3rc8/wagtail_fedit/wagtail_hooks/action_menu.py
--rw-rw-rw-   0        0        0     2378 2024-04-21 02:17:05.000000 wagtail_fedit-1.5.3rc8/wagtail_fedit/wagtail_hooks/adapter_hooks.py
--rw-rw-rw-   0        0        0      268 2024-04-18 15:33:56.000000 wagtail_fedit-1.5.3rc8/wagtail_fedit/wagtail_hooks/adapter_registry.py
--rw-rw-rw-   0        0        0      398 2024-04-11 09:03:10.000000 wagtail_fedit-1.5.3rc8/wagtail_fedit/wagtail_hooks/icons.py
--rw-rw-rw-   0        0        0     2573 2024-04-11 07:39:50.000000 wagtail_fedit-1.5.3rc8/wagtail_fedit/wagtail_hooks/log_actions.py
--rw-rw-rw-   0        0        0      340 2024-03-30 17:10:05.000000 wagtail_fedit-1.5.3rc8/wagtail_fedit/wagtail_hooks/urls.py
--rw-rw-rw-   0        0        0     7630 2024-04-19 20:11:56.000000 wagtail_fedit-1.5.3rc8/wagtail_fedit/wagtail_hooks/userbar.py
-drwxrwxrwx   0        0        0        0 2024-04-21 07:56:53.609438 wagtail_fedit-1.5.3rc8/wagtail_fedit.egg-info/
--rw-rw-rw-   0        0        0    20741 2024-04-21 07:56:51.000000 wagtail_fedit-1.5.3rc8/wagtail_fedit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     4038 2024-04-21 07:56:52.000000 wagtail_fedit-1.5.3rc8/wagtail_fedit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-21 07:56:51.000000 wagtail_fedit-1.5.3rc8/wagtail_fedit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2024-04-21 07:56:51.000000 wagtail_fedit-1.5.3rc8/wagtail_fedit.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-04-21 07:56:51.000000 wagtail_fedit-1.5.3rc8/wagtail_fedit.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-21 21:47:14.907633 wagtail_fedit-1.5.3rc9/
+-rw-rw-rw-   0        0        0    18429 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.3rc9/LICENSE
+-rw-rw-rw-   0        0        0      257 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.3rc9/MANIFEST.in
+-rw-rw-rw-   0        0        0    21085 2024-04-21 21:47:14.907633 wagtail_fedit-1.5.3rc9/PKG-INFO
+-rw-rw-rw-   0        0        0    19884 2024-04-21 20:38:03.000000 wagtail_fedit-1.5.3rc9/README.md
+-rw-rw-rw-   0        0        0       90 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.3rc9/pyproject.toml
+-rw-rw-rw-   0        0        0     1189 2024-04-21 21:47:14.921738 wagtail_fedit-1.5.3rc9/setup.cfg
+-rw-rw-rw-   0        0        0       39 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.3rc9/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-21 21:47:14.770326 wagtail_fedit-1.5.3rc9/wagtail_fedit/
+-rw-rw-rw-   0        0        0        0 2024-03-29 20:13:25.000000 wagtail_fedit-1.5.3rc9/wagtail_fedit/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-21 21:47:14.826150 wagtail_fedit-1.5.3rc9/wagtail_fedit/adapters/
+-rw-rw-rw-   0        0        0      518 2024-04-21 16:44:17.000000 wagtail_fedit-1.5.3rc9/wagtail_fedit/adapters/__init__.py
+-rw-rw-rw-   0        0        0    11210 2024-04-21 21:26:41.000000 wagtail_fedit-1.5.3rc9/wagtail_fedit/adapters/base.py
+-rw-rw-rw-   0        0        0     6215 2024-04-21 21:34:32.000000 wagtail_fedit-1.5.3rc9/wagtail_fedit/adapters/block.py
+-rw-rw-rw-   0        0        0     8677 2024-04-21 20:08:37.000000 wagtail_fedit-1.5.3rc9/wagtail_fedit/adapters/field.py
+-rw-rw-rw-   0        0        0     2076 2024-04-21 12:09:20.000000 wagtail_fedit-1.5.3rc9/wagtail_fedit/adapters/funcs.py
+-rw-rw-rw-   0        0        0     2390 2024-04-21 12:09:35.000000 wagtail_fedit-1.5.3rc9/wagtail_fedit/adapters/misc.py
+-rw-rw-rw-   0        0        0     3200 2024-04-21 21:44:02.000000 wagtail_fedit-1.5.3rc9/wagtail_fedit/adapters/models.py
+-rw-rw-rw-   0        0        0     1595 2024-04-18 20:22:37.000000 wagtail_fedit-1.5.3rc9/wagtail_fedit/adapters/registry.py
+-rw-rw-rw-   0        0        0      163 2024-03-29 20:13:25.000000 wagtail_fedit-1.5.3rc9/wagtail_fedit/apps.py
+drwxrwxrwx   0        0        0        0 2024-04-21 21:47:14.828629 wagtail_fedit-1.5.3rc9/wagtail_fedit/forms/
+-rw-rw-rw-   0        0        0       71 2024-04-02 19:03:21.000000 wagtail_fedit-1.5.3rc9/wagtail_fedit/forms/__init__.py
+-rw-rw-rw-   0        0        0     2881 2024-04-18 20:27:35.000000 wagtail_fedit-1.5.3rc9/wagtail_fedit/forms/blocks.py
+-rw-rw-rw-   0        0        0     3110 2024-04-21 02:24:44.000000 wagtail_fedit-1.5.3rc9/wagtail_fedit/forms/fields.py
+-rw-rw-rw-   0        0        0     4617 2024-04-21 02:08:33.000000 wagtail_fedit-1.5.3rc9/wagtail_fedit/hooks.py
+drwxrwxrwx   0        0        0        0 2024-04-21 21:47:14.730902 wagtail_fedit-1.5.3rc9/wagtail_fedit/locale/
+drwxrwxrwx   0        0        0        0 2024-04-21 21:47:14.730902 wagtail_fedit-1.5.3rc9/wagtail_fedit/locale/nl/
+drwxrwxrwx   0        0        0        0 2024-04-21 21:47:14.830628 wagtail_fedit-1.5.3rc9/wagtail_fedit/locale/nl/LC_MESSAGES/
+-rw-rw-rw-   0        0        0     7129 2024-04-11 09:05:50.000000 wagtail_fedit-1.5.3rc9/wagtail_fedit/locale/nl/LC_MESSAGES/django.mo
+-rw-rw-rw-   0        0        0    12687 2024-04-11 09:05:42.000000 wagtail_fedit-1.5.3rc9/wagtail_fedit/locale/nl/LC_MESSAGES/django.po
+drwxrwxrwx   0        0        0        0 2024-04-21 21:47:14.831628 wagtail_fedit-1.5.3rc9/wagtail_fedit/migrations/
+-rw-rw-rw-   0        0        0        0 2024-03-29 20:13:25.000000 wagtail_fedit-1.5.3rc9/wagtail_fedit/migrations/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-21 21:47:14.832728 wagtail_fedit-1.5.3rc9/wagtail_fedit/migrations/__pycache__/
+-rw-rw-rw-   0        0        0      215 2024-03-29 21:05:00.000000 wagtail_fedit-1.5.3rc9/wagtail_fedit/migrations/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0     3170 2024-04-05 20:30:10.000000 wagtail_fedit-1.5.3rc9/wagtail_fedit/models.py
+-rw-rw-rw-   0        0        0      973 2024-04-21 00:46:27.000000 wagtail_fedit-1.5.3rc9/wagtail_fedit/settings.py
+drwxrwxrwx   0        0        0        0 2024-04-21 21:47:14.732413 wagtail_fedit-1.5.3rc9/wagtail_fedit/static/
+drwxrwxrwx   0        0        0        0 2024-04-21 21:47:14.733419 wagtail_fedit-1.5.3rc9/wagtail_fedit/static/wagtail_fedit/
+drwxrwxrwx   0        0        0        0 2024-04-21 21:47:14.837025 wagtail_fedit-1.5.3rc9/wagtail_fedit/static/wagtail_fedit/css/
+-rw-rw-rw-   0        0        0     5500 2024-04-21 17:02:30.000000 wagtail_fedit-1.5.3rc9/wagtail_fedit/static/wagtail_fedit/css/frontend.css
+-rw-rw-rw-   0        0        0     5098 2024-04-17 20:40:49.000000 wagtail_fedit-1.5.3rc9/wagtail_fedit/static/wagtail_fedit/css/furniture.css
+-rw-rw-rw-   0        0        0     1266 2024-04-05 19:37:44.000000 wagtail_fedit-1.5.3rc9/wagtail_fedit/static/wagtail_fedit/css/userbar-menu.css
+drwxrwxrwx   0        0        0        0 2024-04-21 21:47:14.838024 wagtail_fedit-1.5.3rc9/wagtail_fedit/static/wagtail_fedit/js/
+-rw-rw-rw-   0        0        0    20559 2024-04-21 20:02:32.000000 wagtail_fedit-1.5.3rc9/wagtail_fedit/static/wagtail_fedit/js/frontend.js
+drwxrwxrwx   0        0        0        0 2024-04-21 21:47:14.734419 wagtail_fedit-1.5.3rc9/wagtail_fedit/templates/
+drwxrwxrwx   0        0        0        0 2024-04-21 21:47:14.839912 wagtail_fedit-1.5.3rc9/wagtail_fedit/templates/wagtail_fedit/
+-rw-rw-rw-   0        0        0       56 2024-04-16 18:37:39.000000 wagtail_fedit-1.5.3rc9/wagtail_fedit/templates/wagtail_fedit/_hook_output.html
+drwxrwxrwx   0        0        0        0 2024-04-21 21:47:14.841912 wagtail_fedit-1.5.3rc9/wagtail_fedit/templates/wagtail_fedit/content/
+drwxrwxrwx   0        0        0        0 2024-04-21 21:47:14.842909 wagtail_fedit-1.5.3rc9/wagtail_fedit/templates/wagtail_fedit/content/buttons/
+-rw-rw-rw-   0        0        0      871 2024-04-19 20:16:18.000000 wagtail_fedit-1.5.3rc9/wagtail_fedit/templates/wagtail_fedit/content/buttons/admin_link.html
+-rw-rw-rw-   0        0        0      872 2024-04-19 20:15:44.000000 wagtail_fedit-1.5.3rc9/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_adapter.html
+-rw-rw-rw-   0        0        0      534 2024-04-21 17:21:38.000000 wagtail_fedit-1.5.3rc9/wagtail_fedit/templates/wagtail_fedit/content/editable_adapter.html
+drwxrwxrwx   0        0        0        0 2024-04-21 21:47:14.853795 wagtail_fedit-1.5.3rc9/wagtail_fedit/templates/wagtail_fedit/editor/
+-rw-rw-rw-   0        0        0     2259 2024-04-11 08:02:26.000000 wagtail_fedit-1.5.3rc9/wagtail_fedit/templates/wagtail_fedit/editor/action_confirm.html
+-rw-rw-rw-   0        0        0     3699 2024-04-20 21:55:10.000000 wagtail_fedit-1.5.3rc9/wagtail_fedit/templates/wagtail_fedit/editor/action_publish_confirm.html
+-rw-rw-rw-   0        0        0      266 2024-04-21 21:15:09.000000 wagtail_fedit-1.5.3rc9/wagtail_fedit/templates/wagtail_fedit/editor/adapter_edit_handler.html
+-rw-rw-rw-   0        0        0      265 2024-04-21 21:23:24.000000 wagtail_fedit-1.5.3rc9/wagtail_fedit/templates/wagtail_fedit/editor/adapter_edit_handler_form.html
+-rw-rw-rw-   0        0        0      555 2024-04-21 21:13:45.000000 wagtail_fedit-1.5.3rc9/wagtail_fedit/templates/wagtail_fedit/editor/adapter_form.html
+-rw-rw-rw-   0        0        0      455 2024-04-21 00:11:35.000000 wagtail_fedit-1.5.3rc9/wagtail_fedit/templates/wagtail_fedit/editor/adapter_form_errors.html
+-rw-rw-rw-   0        0        0      330 2024-04-21 00:12:14.000000 wagtail_fedit-1.5.3rc9/wagtail_fedit/templates/wagtail_fedit/editor/adapter_iframe.html
+-rw-rw-rw-   0        0        0     5271 2024-04-21 00:11:24.000000 wagtail_fedit-1.5.3rc9/wagtail_fedit/templates/wagtail_fedit/editor/base_iframe.html
+-rw-rw-rw-   0        0        0      496 2024-04-02 17:46:59.000000 wagtail_fedit-1.5.3rc9/wagtail_fedit/templates/wagtail_fedit/editor/field.html
+drwxrwxrwx   0        0        0        0 2024-04-21 21:47:14.859346 wagtail_fedit-1.5.3rc9/wagtail_fedit/templates/wagtail_fedit/icons/
+-rw-rw-rw-   0        0        0      797 2024-04-11 08:36:19.000000 wagtail_fedit-1.5.3rc9/wagtail_fedit/templates/wagtail_fedit/icons/fedit-check-list.svg
+-rw-rw-rw-   0        0        0      584 2024-04-11 08:36:55.000000 wagtail_fedit-1.5.3rc9/wagtail_fedit/templates/wagtail_fedit/icons/fedit-eye-closed.svg
+-rw-rw-rw-   0        0        0      377 2024-04-11 08:23:07.000000 wagtail_fedit-1.5.3rc9/wagtail_fedit/templates/wagtail_fedit/icons/fedit-eye-open.svg
+-rw-rw-rw-   0        0        0      725 2024-04-11 09:02:58.000000 wagtail_fedit-1.5.3rc9/wagtail_fedit/templates/wagtail_fedit/icons/fedit-save.svg
+-rw-rw-rw-   0        0        0     1323 2024-04-11 08:36:52.000000 wagtail_fedit-1.5.3rc9/wagtail_fedit/templates/wagtail_fedit/icons/fedit-stop-sign.svg
+drwxrwxrwx   0        0        0        0 2024-04-21 21:47:14.861353 wagtail_fedit-1.5.3rc9/wagtail_fedit/templates/wagtail_fedit/userbar/
+-rw-rw-rw-   0        0        0      867 2024-04-03 17:05:21.000000 wagtail_fedit-1.5.3rc9/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit.html
+-rw-rw-rw-   0        0        0      876 2024-04-03 16:59:31.000000 wagtail_fedit-1.5.3rc9/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_view_live.html
+drwxrwxrwx   0        0        0        0 2024-04-21 21:47:14.863350 wagtail_fedit-1.5.3rc9/wagtail_fedit/templates/wagtail_fedit/userbar/publish/
+-rw-rw-rw-   0        0        0      263 2024-04-11 08:24:35.000000 wagtail_fedit-1.5.3rc9/wagtail_fedit/templates/wagtail_fedit/userbar/publish/action_button.html
+-rw-rw-rw-   0        0        0      967 2024-04-11 09:03:51.000000 wagtail_fedit-1.5.3rc9/wagtail_fedit/templates/wagtail_fedit/userbar/publish/item_fedit_publishing.html
+drwxrwxrwx   0        0        0        0 2024-04-21 21:47:14.864754 wagtail_fedit-1.5.3rc9/wagtail_fedit/templatetags/
+-rw-rw-rw-   0        0        0        0 2024-03-29 20:13:42.000000 wagtail_fedit-1.5.3rc9/wagtail_fedit/templatetags/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-21 21:47:14.867755 wagtail_fedit-1.5.3rc9/wagtail_fedit/templatetags/__pycache__/
+-rw-rw-rw-   0        0        0      217 2024-03-29 21:05:00.000000 wagtail_fedit-1.5.3rc9/wagtail_fedit/templatetags/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0    11089 2024-04-21 18:54:08.000000 wagtail_fedit-1.5.3rc9/wagtail_fedit/templatetags/__pycache__/fedit.cpython-311.pyc
+-rw-rw-rw-   0        0        0     8664 2024-04-21 18:53:42.000000 wagtail_fedit-1.5.3rc9/wagtail_fedit/templatetags/fedit.py
+drwxrwxrwx   0        0        0        0 2024-04-21 21:47:14.869295 wagtail_fedit-1.5.3rc9/wagtail_fedit/test/
+-rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.3rc9/wagtail_fedit/test/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-21 21:47:14.875293 wagtail_fedit-1.5.3rc9/wagtail_fedit/test/core/
+-rw-rw-rw-   0        0        0      151 2024-04-05 07:59:49.000000 wagtail_fedit-1.5.3rc9/wagtail_fedit/test/core/__init__.py
+-rw-rw-rw-   0        0        0      165 2024-04-05 08:41:40.000000 wagtail_fedit-1.5.3rc9/wagtail_fedit/test/core/apps.py
+-rw-rw-rw-   0        0        0      130 2024-04-15 20:12:38.000000 wagtail_fedit-1.5.3rc9/wagtail_fedit/test/core/context_processors.py
+drwxrwxrwx   0        0        0        0 2024-04-21 21:47:14.879036 wagtail_fedit-1.5.3rc9/wagtail_fedit/test/core/migrations/
+-rw-rw-rw-   0        0        0    12115 2024-04-20 22:33:35.000000 wagtail_fedit-1.5.3rc9/wagtail_fedit/test/core/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0      509 2024-04-21 18:41:55.000000 wagtail_fedit-1.5.3rc9/wagtail_fedit/test/core/migrations/0002_basicmodel_related_field.py
+-rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.3rc9/wagtail_fedit/test/core/migrations/__init__.py
+-rw-rw-rw-   0        0        0     5603 2024-04-21 18:39:18.000000 wagtail_fedit-1.5.3rc9/wagtail_fedit/test/core/models.py
+drwxrwxrwx   0        0        0        0 2024-04-21 21:47:14.888150 wagtail_fedit-1.5.3rc9/wagtail_fedit/test/core/tests/
+-rw-rw-rw-   0        0        0        0 2024-04-05 07:59:29.000000 wagtail_fedit-1.5.3rc9/wagtail_fedit/test/core/tests/__init__.py
+-rw-rw-rw-   0        0        0     8132 2024-04-21 18:49:27.000000 wagtail_fedit-1.5.3rc9/wagtail_fedit/test/core/tests/base.py
+-rw-rw-rw-   0        0        0    18772 2024-04-21 19:32:12.000000 wagtail_fedit-1.5.3rc9/wagtail_fedit/test/core/tests/test_adapters.py
+-rw-rw-rw-   0        0        0     4320 2024-04-06 22:44:26.000000 wagtail_fedit-1.5.3rc9/wagtail_fedit/test/core/tests/test_block_edit.py
+-rw-rw-rw-   0        0        0     5664 2024-04-05 10:31:29.000000 wagtail_fedit-1.5.3rc9/wagtail_fedit/test/core/tests/test_blocks.py
+-rw-rw-rw-   0        0        0     3642 2024-04-05 18:00:23.000000 wagtail_fedit-1.5.3rc9/wagtail_fedit/test/core/tests/test_field_edit.py
+-rw-rw-rw-   0        0        0     3709 2024-04-10 13:03:30.000000 wagtail_fedit-1.5.3rc9/wagtail_fedit/test/core/tests/test_generic.py
+-rw-rw-rw-   0        0        0     1574 2024-04-20 20:49:12.000000 wagtail_fedit-1.5.3rc9/wagtail_fedit/test/core/tests/test_revision.py
+-rw-rw-rw-   0        0        0     9545 2024-04-20 21:54:40.000000 wagtail_fedit-1.5.3rc9/wagtail_fedit/test/core/tests/test_submit.py
+-rw-rw-rw-   0        0        0      704 2024-04-05 17:55:36.000000 wagtail_fedit-1.5.3rc9/wagtail_fedit/test/manage.py
+drwxrwxrwx   0        0        0        0 2024-04-21 21:47:14.893025 wagtail_fedit-1.5.3rc9/wagtail_fedit/test/testapp/
+-rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.3rc9/wagtail_fedit/test/testapp/__init__.py
+-rw-rw-rw-   0        0        0      407 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.3rc9/wagtail_fedit/test/testapp/asgi.py
+-rw-rw-rw-   0        0        0     3625 2024-04-15 20:14:41.000000 wagtail_fedit-1.5.3rc9/wagtail_fedit/test/testapp/settings.py
+-rw-rw-rw-   0        0        0      897 2024-04-05 08:04:53.000000 wagtail_fedit-1.5.3rc9/wagtail_fedit/test/testapp/urls.py
+-rw-rw-rw-   0        0        0      407 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.3rc9/wagtail_fedit/test/testapp/wsgi.py
+-rw-rw-rw-   0        0        0     2009 2024-04-19 20:04:30.000000 wagtail_fedit-1.5.3rc9/wagtail_fedit/toolbar.py
+-rw-rw-rw-   0        0        0      934 2024-04-21 16:55:23.000000 wagtail_fedit-1.5.3rc9/wagtail_fedit/urls.py
+-rw-rw-rw-   0        0        0    16829 2024-04-21 18:51:40.000000 wagtail_fedit-1.5.3rc9/wagtail_fedit/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-21 21:47:14.897608 wagtail_fedit-1.5.3rc9/wagtail_fedit/views/
+-rw-rw-rw-   0        0        0      190 2024-04-13 19:36:44.000000 wagtail_fedit-1.5.3rc9/wagtail_fedit/views/__init__.py
+-rw-rw-rw-   0        0        0     7220 2024-04-21 21:28:24.000000 wagtail_fedit-1.5.3rc9/wagtail_fedit/views/adapters.py
+-rw-rw-rw-   0        0        0    17563 2024-04-21 20:25:17.000000 wagtail_fedit-1.5.3rc9/wagtail_fedit/views/editable.py
+-rw-rw-rw-   0        0        0     1923 2024-04-21 20:29:01.000000 wagtail_fedit-1.5.3rc9/wagtail_fedit/views/mixins.py
+drwxrwxrwx   0        0        0        0 2024-04-21 21:47:14.906635 wagtail_fedit-1.5.3rc9/wagtail_fedit/wagtail_hooks/
+-rw-rw-rw-   0        0        0      184 2024-04-16 10:03:02.000000 wagtail_fedit-1.5.3rc9/wagtail_fedit/wagtail_hooks/__init__.py
+-rw-rw-rw-   0        0        0     1748 2024-04-06 18:37:13.000000 wagtail_fedit-1.5.3rc9/wagtail_fedit/wagtail_hooks/action_menu.py
+-rw-rw-rw-   0        0        0     2378 2024-04-21 02:17:05.000000 wagtail_fedit-1.5.3rc9/wagtail_fedit/wagtail_hooks/adapter_hooks.py
+-rw-rw-rw-   0        0        0      328 2024-04-21 16:44:33.000000 wagtail_fedit-1.5.3rc9/wagtail_fedit/wagtail_hooks/adapter_registry.py
+-rw-rw-rw-   0        0        0      398 2024-04-11 09:03:10.000000 wagtail_fedit-1.5.3rc9/wagtail_fedit/wagtail_hooks/icons.py
+-rw-rw-rw-   0        0        0     2573 2024-04-11 07:39:50.000000 wagtail_fedit-1.5.3rc9/wagtail_fedit/wagtail_hooks/log_actions.py
+-rw-rw-rw-   0        0        0      340 2024-03-30 17:10:05.000000 wagtail_fedit-1.5.3rc9/wagtail_fedit/wagtail_hooks/urls.py
+-rw-rw-rw-   0        0        0     7630 2024-04-19 20:11:56.000000 wagtail_fedit-1.5.3rc9/wagtail_fedit/wagtail_hooks/userbar.py
+drwxrwxrwx   0        0        0        0 2024-04-21 21:47:14.814300 wagtail_fedit-1.5.3rc9/wagtail_fedit.egg-info/
+-rw-rw-rw-   0        0        0    21085 2024-04-21 21:47:14.000000 wagtail_fedit-1.5.3rc9/wagtail_fedit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     4286 2024-04-21 21:47:14.000000 wagtail_fedit-1.5.3rc9/wagtail_fedit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-21 21:47:14.000000 wagtail_fedit-1.5.3rc9/wagtail_fedit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       25 2024-04-21 21:47:14.000000 wagtail_fedit-1.5.3rc9/wagtail_fedit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-04-21 21:47:14.000000 wagtail_fedit-1.5.3rc9/wagtail_fedit.egg-info/top_level.txt
```

### Comparing `wagtail_fedit-1.5.3rc8/LICENSE` & `wagtail_fedit-1.5.3rc9/LICENSE`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc8/PKG-INFO` & `wagtail_fedit-1.5.3rc9/wagtail_fedit.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: wagtail_fedit
-Version: 1.5.3rc8
+Name: wagtail-fedit
+Version: 1.5.3rc9
 Summary: Frontend editing for your Wagtail site
 Home-page: https://github.com/Nigel2392/wagtail_fedit
 Author: Nigel
 Author-email: nigel@goodadvice.it
 License: GPL-2.0-only
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
@@ -23,16 +23,14 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: Django>=4.2
-Requires-Dist: Wagtail>=5.2
 
 wagtail_fedit
 =============
 
 ![Wagtail FEdit Example](https://github.com/Nigel2392/wagtail_fedit/blob/main/.github/images/wagtail_fedit_example.png?raw=true)
 
 Wagtail FEdit is a library to allow your Wagtail pages and content-blocks to be edited on the frontend.
@@ -79,17 +77,24 @@
    ]
    ```
 2. Run `py ./manage.py collectstatic`.
 3. Run `py ./manage.py adapter_help` to see all your options and their requirements.
 
 ## Getting Editing!
 
-1. Make sure the models you wish to edit inherit from PreviewableMixin.
+1. If you want to get into the frontend-editing interface for a model it must inherit from `PreviewableMixin`.
 
    **This is a requirement.**
+
+   It is however not always required for your model to inherit from `PreviewableMixin`.
+
+   **Any model can be edited**; you just can't access the specific frontend editing interface URL for that model if it does not inherit from `PreviewableMixin`.
+
+   I.E: If a random model which does not inherit from `PreviewableMixin` appears on an editable page; **you will be able to edit it.**
+
 2. Define a template for your model.
 
    Example:
 
    ```django-html
    {% load fedit static wagtailuserbar %} {# Load the required template tag libraries #}
    <!DOCTYPE html>
@@ -339,15 +344,15 @@
     def __init__(self, object, field_name: str, request: HttpRequest, **kwargs):
         kwargs["name"] = "myColorizerJavascriptFunction"
         super().__init__(object, field_name, request, **kwargs)
 
     def render_content(self, parent_context=None):
         # This is not required; we will replace a CSS variable; thus we are not returning any actual content.
         return ""
-    
+  
     def get_response_data(self, parent_context=None):
         """
         Return the data to be sent to the frontend adapter.
         """
         data = super().get_response_data(parent_context)
         return data | {
             "color": self.field_value,
@@ -479,15 +484,24 @@
 
 Register a custom JS file to be included when the utils.FEDIT_PREVIEW_VAR is set to True.
 
 This can be used to register custom adapter JS.
 
 Example of how this hook is used in wagtail_hooks.py:
 
-    ``python     @hooks.register(REGISTER_JS)     def register_js(request):         return [             format_html(                 '<script src="{0}"></script>',                 static('js/custom.js')             ),         ]     ``
+```python
+@hooks.register(REGISTER_JS)
+def register_js(request):
+    return [
+        format_html(
+            '<script src="{0}"></script>',
+            static('js/custom.js')
+        ),
+    ]
+```
 
 ### wagtail_fedit.register_field_renderer
 
 Register a custom renderer for a field.
 
 Example of how this type of renderer is used in wagtail_hooks/renderers.py:
 
@@ -498,18 +512,19 @@
     # This is a custom renderer for RichText fields.
     # It will render the RichText field as a RichText block.
     renderer_map[RichTextField] =\
         lambda request, context, instance, value: richtext(value)
 ```
 
 ### wagtail_fedit.register_field_widgets
+
 Register a custom widget for a field.
 
 Example of how this hook is used in wagtail_hooks.py:
-    
+
 ```python
 @hooks.register(REGISTER_FIELD_WIDGETS)
 def register_field_widgets(widgets):
     widgets[RichTextField] = AdminRichTextField
     return widgets
 ```
```

#### html2text {}

```diff
@@ -1,25 +1,24 @@
-Metadata-Version: 2.1 Name: wagtail_fedit Version: 1.5.3rc8 Summary: Frontend
+Metadata-Version: 2.1 Name: wagtail-fedit Version: 1.5.3rc9 Summary: Frontend
 editing for your Wagtail site Home-page: https://github.com/Nigel2392/
 wagtail_fedit Author: Nigel Author-email: nigel@goodadvice.it License: GPL-2.0-
 only Classifier: Environment :: Web Environment Classifier: Framework :: Django
 Classifier: Framework :: Django :: 4.2 Classifier: Framework :: Wagtail
 Classifier: Framework :: Wagtail :: 5 Classifier: Framework :: Wagtail :: 6
 Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
 :: GNU General Public License v2 or later (GPLv2+) Classifier: Operating System
 :: OS Independent Classifier: Programming Language :: Python Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3 :: Only Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
 Topic :: Internet :: WWW/HTTP Classifier: Topic :: Internet :: WWW/HTTP ::
 Dynamic Content Requires-Python: >=3.8 Description-Content-Type: text/markdown
-License-File: LICENSE Requires-Dist: Django>=4.2 Requires-Dist: Wagtail>=5.2
-wagtail_fedit ============= ![Wagtail FEdit Example](https://github.com/
-Nigel2392/wagtail_fedit/blob/main/.github/images/
+License-File: LICENSE wagtail_fedit ============= ![Wagtail FEdit Example]
+(https://github.com/Nigel2392/wagtail_fedit/blob/main/.github/images/
 wagtail_fedit_example.png?raw=true) Wagtail FEdit is a library to allow your
 Wagtail pages and content-blocks to be edited on the frontend. # Table of
 Contents - [Getting Started](#getting-started) - [Getting Editing!](#getting-
 editing) - [Permissions](#permissions) - [Revisions](#revisions) - [Workflows]
 (#workflows) - [Logs](#logs) - [Caveats](#caveats) - [Adapters](#adapters) -
 [Adapters Python](#adapters-python) - [Adapters Javascript](#adapters-
 javascript) - [Hooks](#hooks) - [Construct Adapter Toolbar]
@@ -35,18 +34,23 @@
 Sessions](#wagtail_fedit_share_with_sessions) - [Use Adapter Session ID]
 (#wagtail_fedit_use_adapter_session_id) - [How your content is rendered](#how-
 your-content-is-rendered) - [Rendered output HTML](#rendered-editable-output-
 html) - [Implemented](#implemented) Getting Started --------------- 1. Add
 'wagtail_fedit' to your INSTALLED_APPS setting like this: ``` INSTALLED_APPS =
 [ ..., 'wagtail_fedit', ] ``` 2. Run `py ./manage.py collectstatic`. 3. Run `py
 ./manage.py adapter_help` to see all your options and their requirements. ##
-Getting Editing! 1. Make sure the models you wish to edit inherit from
-PreviewableMixin. **This is a requirement.** 2. Define a template for your
-model. Example: ```django-html {% load fedit static wagtailuserbar %} {# Load
-the required template tag libraries #}
+Getting Editing! 1. If you want to get into the frontend-editing interface for
+a model it must inherit from `PreviewableMixin`. **This is a requirement.** It
+is however not always required for your model to inherit from
+`PreviewableMixin`. **Any model can be edited**; you just can't access the
+specific frontend editing interface URL for that model if it does not inherit
+from `PreviewableMixin`. I.E: If a random model which does not inherit from
+`PreviewableMixin` appears on an editable page; **you will be able to edit
+it.** 2. Define a template for your model. Example: ```django-html {% load
+fedit static wagtailuserbar %} {# Load the required template tag libraries #}
 {# Load all registered CSS required for the adapters. Only included inside edit
 view! #} {% fedit_scripts "css" %}
 {# Adress the model.field or model.my.related.field you wish to edit. #} {# For
 help on arguments for the adapters please run the adapter_help command. #} {#
 Example: `python3 ./manage.py adapter_help` #}
 ************ {{%% ffeeddiitt ffiieelldd sseellff..ttiittllee iinnlliinnee %%}} ************
 {% fedit field self.content %} {% wagtailuserbar %} {# Load all registered
@@ -195,17 +199,17 @@
 ', static('css/custom.css') ), ] ``` ### wagtail_fedit.field_editor_size
 Control the size of the editor for the given model-field type. Example of how
 this hook is called: ```python for hook in hooks.get_hooks
 (FEDIT_FIELD_EDITOR_SIZE): size = hook(model_instance, model_field) if size:
 return size ``` ### wagtail_fedit.register_js Register a custom JS file to be
 included when the utils.FEDIT_PREVIEW_VAR is set to True. This can be used to
 register custom adapter JS. Example of how this hook is used in
-wagtail_hooks.py: ``python @hooks.register(REGISTER_JS) def register_js
+wagtail_hooks.py: ```python @hooks.register(REGISTER_JS) def register_js
 (request): return [ format_html( '
-', static('js/custom.js') ), ] `` ### wagtail_fedit.register_field_renderer
+', static('js/custom.js') ), ] ``` ### wagtail_fedit.register_field_renderer
 Register a custom renderer for a field. Example of how this type of renderer is
 used in wagtail_hooks/renderers.py: ```python @hooks.register
 (REGISTER_FIELD_RENDERER) def register_renderers(renderer_map): # This is a
 custom renderer for RichText fields. # It will render the RichText field as a
 RichText block. renderer_map[RichTextField] =\ lambda request, context,
 instance, value: richtext(value) ``` ### wagtail_fedit.register_field_widgets
 Register a custom widget for a field. Example of how this hook is used in
```

### Comparing `wagtail_fedit-1.5.3rc8/README.md` & `wagtail_fedit-1.5.3rc9/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -47,17 +47,24 @@
    ]
    ```
 2. Run `py ./manage.py collectstatic`.
 3. Run `py ./manage.py adapter_help` to see all your options and their requirements.
 
 ## Getting Editing!
 
-1. Make sure the models you wish to edit inherit from PreviewableMixin.
+1. If you want to get into the frontend-editing interface for a model it must inherit from `PreviewableMixin`.
 
    **This is a requirement.**
+
+   It is however not always required for your model to inherit from `PreviewableMixin`.
+
+   **Any model can be edited**; you just can't access the specific frontend editing interface URL for that model if it does not inherit from `PreviewableMixin`.
+
+   I.E: If a random model which does not inherit from `PreviewableMixin` appears on an editable page; **you will be able to edit it.**
+
 2. Define a template for your model.
 
    Example:
 
    ```django-html
    {% load fedit static wagtailuserbar %} {# Load the required template tag libraries #}
    <!DOCTYPE html>
@@ -307,15 +314,15 @@
     def __init__(self, object, field_name: str, request: HttpRequest, **kwargs):
         kwargs["name"] = "myColorizerJavascriptFunction"
         super().__init__(object, field_name, request, **kwargs)
 
     def render_content(self, parent_context=None):
         # This is not required; we will replace a CSS variable; thus we are not returning any actual content.
         return ""
-    
+  
     def get_response_data(self, parent_context=None):
         """
         Return the data to be sent to the frontend adapter.
         """
         data = super().get_response_data(parent_context)
         return data | {
             "color": self.field_value,
@@ -447,15 +454,24 @@
 
 Register a custom JS file to be included when the utils.FEDIT_PREVIEW_VAR is set to True.
 
 This can be used to register custom adapter JS.
 
 Example of how this hook is used in wagtail_hooks.py:
 
-    ``python     @hooks.register(REGISTER_JS)     def register_js(request):         return [             format_html(                 '<script src="{0}"></script>',                 static('js/custom.js')             ),         ]     ``
+```python
+@hooks.register(REGISTER_JS)
+def register_js(request):
+    return [
+        format_html(
+            '<script src="{0}"></script>',
+            static('js/custom.js')
+        ),
+    ]
+```
 
 ### wagtail_fedit.register_field_renderer
 
 Register a custom renderer for a field.
 
 Example of how this type of renderer is used in wagtail_hooks/renderers.py:
 
@@ -466,18 +482,19 @@
     # This is a custom renderer for RichText fields.
     # It will render the RichText field as a RichText block.
     renderer_map[RichTextField] =\
         lambda request, context, instance, value: richtext(value)
 ```
 
 ### wagtail_fedit.register_field_widgets
+
 Register a custom widget for a field.
 
 Example of how this hook is used in wagtail_hooks.py:
-    
+
 ```python
 @hooks.register(REGISTER_FIELD_WIDGETS)
 def register_field_widgets(widgets):
     widgets[RichTextField] = AdminRichTextField
     return widgets
 ```
```

#### html2text {}

```diff
@@ -19,18 +19,23 @@
 Sessions](#wagtail_fedit_share_with_sessions) - [Use Adapter Session ID]
 (#wagtail_fedit_use_adapter_session_id) - [How your content is rendered](#how-
 your-content-is-rendered) - [Rendered output HTML](#rendered-editable-output-
 html) - [Implemented](#implemented) Getting Started --------------- 1. Add
 'wagtail_fedit' to your INSTALLED_APPS setting like this: ``` INSTALLED_APPS =
 [ ..., 'wagtail_fedit', ] ``` 2. Run `py ./manage.py collectstatic`. 3. Run `py
 ./manage.py adapter_help` to see all your options and their requirements. ##
-Getting Editing! 1. Make sure the models you wish to edit inherit from
-PreviewableMixin. **This is a requirement.** 2. Define a template for your
-model. Example: ```django-html {% load fedit static wagtailuserbar %} {# Load
-the required template tag libraries #}
+Getting Editing! 1. If you want to get into the frontend-editing interface for
+a model it must inherit from `PreviewableMixin`. **This is a requirement.** It
+is however not always required for your model to inherit from
+`PreviewableMixin`. **Any model can be edited**; you just can't access the
+specific frontend editing interface URL for that model if it does not inherit
+from `PreviewableMixin`. I.E: If a random model which does not inherit from
+`PreviewableMixin` appears on an editable page; **you will be able to edit
+it.** 2. Define a template for your model. Example: ```django-html {% load
+fedit static wagtailuserbar %} {# Load the required template tag libraries #}
 {# Load all registered CSS required for the adapters. Only included inside edit
 view! #} {% fedit_scripts "css" %}
 {# Adress the model.field or model.my.related.field you wish to edit. #} {# For
 help on arguments for the adapters please run the adapter_help command. #} {#
 Example: `python3 ./manage.py adapter_help` #}
 ************ {{%% ffeeddiitt ffiieelldd sseellff..ttiittllee iinnlliinnee %%}} ************
 {% fedit field self.content %} {% wagtailuserbar %} {# Load all registered
@@ -179,17 +184,17 @@
 ', static('css/custom.css') ), ] ``` ### wagtail_fedit.field_editor_size
 Control the size of the editor for the given model-field type. Example of how
 this hook is called: ```python for hook in hooks.get_hooks
 (FEDIT_FIELD_EDITOR_SIZE): size = hook(model_instance, model_field) if size:
 return size ``` ### wagtail_fedit.register_js Register a custom JS file to be
 included when the utils.FEDIT_PREVIEW_VAR is set to True. This can be used to
 register custom adapter JS. Example of how this hook is used in
-wagtail_hooks.py: ``python @hooks.register(REGISTER_JS) def register_js
+wagtail_hooks.py: ```python @hooks.register(REGISTER_JS) def register_js
 (request): return [ format_html( '
-', static('js/custom.js') ), ] `` ### wagtail_fedit.register_field_renderer
+', static('js/custom.js') ), ] ``` ### wagtail_fedit.register_field_renderer
 Register a custom renderer for a field. Example of how this type of renderer is
 used in wagtail_hooks/renderers.py: ```python @hooks.register
 (REGISTER_FIELD_RENDERER) def register_renderers(renderer_map): # This is a
 custom renderer for RichText fields. # It will render the RichText field as a
 RichText block. renderer_map[RichTextField] =\ lambda request, context,
 instance, value: richtext(value) ``` ### wagtail_fedit.register_field_widgets
 Register a custom widget for a field. Example of how this hook is used in
```

### Comparing `wagtail_fedit-1.5.3rc8/setup.cfg` & `wagtail_fedit-1.5.3rc9/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2077 6167 7461 696c 5f66 6564 6974   = wagtail_fedit
 00000020: 0d0a 7665 7273 696f 6e20 3d20 312e 352e  ..version = 1.5.
-00000030: 3372 6338 0d0a 6465 7363 7269 7074 696f  3rc8..descriptio
+00000030: 3372 6339 0d0a 6465 7363 7269 7074 696f  3rc9..descriptio
 00000040: 6e20 3d20 4672 6f6e 7465 6e64 2065 6469  n = Frontend edi
 00000050: 7469 6e67 2066 6f72 2079 6f75 7220 5761  ting for your Wa
 00000060: 6774 6169 6c20 7369 7465 0d0a 6c6f 6e67  gtail site..long
 00000070: 5f64 6573 6372 6970 7469 6f6e 203d 2066  _description = f
 00000080: 696c 653a 2052 4541 444d 452e 6d64 0d0a  ile: README.md..
 00000090: 6c6f 6e67 5f64 6573 6372 6970 7469 6f6e  long_description
 000000a0: 5f63 6f6e 7465 6e74 5f74 7970 6520 3d20  _content_type =
```

### Comparing `wagtail_fedit-1.5.3rc8/wagtail_fedit/adapters/base.py` & `wagtail_fedit-1.5.3rc9/wagtail_fedit/adapters/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -62,16 +62,20 @@
 def Base85_json_dumps(obj):
     return base64.b85encode(json.dumps(obj).encode("utf-8")).decode("utf-8")
 
 def Base85_json_loads(data):
     return json.loads(base64.b85decode(data).decode("utf-8"))
 
 class BaseAdapter(FeditIFrameMixin):
+    # How the adapter is identified on inside of the templatetag.
     identifier              = None
 
+    # If the templatetag required the first argument to be model.field or just model
+    field_required          = True
+
     # The template used to render the form.
     template_name           = "wagtail_fedit/editor/adapter_iframe.html"
 
     signer: Signer          = Signer()
     # Required keyword arguments for the adapter
     required_kwargs         = []
     # Optional keyword arguments for the adapter, these are only used to print the help example.
@@ -88,19 +92,24 @@
 
     # The JS constructor for the adapter.
     # This will receive the data after a successful form submission.
     js_constructor          = None
 
     def __init__(self, object: models.Model, field_name: str, request: HttpRequest, **kwargs):
         self.object         = object
-        self.field_name     = field_name
-        self.meta_field     = object._meta.get_field(field_name)
         self.request        = request
         self.kwargs         = kwargs
 
+        if self.field_required:
+            self.field_name     = field_name
+            self.meta_field     = object._meta.get_field(field_name)
+        else:
+            self.field_name     = None
+            self.meta_field     = None
+
     @classmethod
     def get_usage_string(cls) -> str:
         """
         Return a string which describes how to use the adapter.
         """
         s = []
         for i, token in enumerate(cls.absolute_tokens):
@@ -125,14 +134,21 @@
         for i, kwarg in enumerate(cls.optional_kwargs):
             s.append(f"[{kwarg}=value]")
             if i < len(cls.optional_kwargs) - 1:
                 s.append(" ")
                 
         return "".join(s)
     
+    def get_form_context(self, **kwargs):
+        return {
+            "adapter": self,
+            "field_name": self.field_name,
+            "meta_field": self.meta_field,
+        }
+
     @classmethod
     def get_usage_description(cls) -> str:
         """
         Return a description of how the adapter is used.
         """
         return cls.usage_description
     
@@ -157,15 +173,15 @@
 
     @property
     def field_value(self):
         """
         Call the value_from_object method on
         the meta field to get the value from the instance.
         """
-        return self.meta_field.value_from_object(self.object)
+        return getattr(self.object, self.field_name)
     
     @property
     def model(self):
         """
         Return the model class of the object.
         """
         return self.object.__class__
@@ -185,15 +201,15 @@
         This is used to link actions from the adapter to the frontend.
         """
         if not self.js_constructor:
             raise AdapterError("No JS constructor defined")
         
         return self.js_constructor
 
-    def get_response_data(self) -> dict:
+    def get_response_data(self, parent_context) -> dict:
         """
         The data which is returned to the frontend on a successful form submission.
         """
         return {
             "adapter": {
                 "identifier":   self.identifier,
                 "constructor":  self.get_js_constructor(),
@@ -214,24 +230,32 @@
 
     def get_toolbar_buttons(self) -> list["FeditToolbarComponent"]:
         """
         Extra possible toolbar buttons.
         This is where for example; the edit icon goes.
         """
         return []
-
-    def get_element_id(self) -> str:
+    
+    def get_element_id_parts(self) -> list[str]:
         """
-        Return a unique identifier for the elements on the frontend.
+        Return the parts of the element ID.
         """
-        return content_id_from_parts(
+        return [
             self.model._meta.app_label,
             self.model._meta.model_name,
             self.object.pk,
             self.field_name,
+        ]
+
+    def get_element_id(self) -> str:
+        """
+        Return a unique identifier for the elements on the frontend.
+        """
+        return content_id_from_parts(
+            *self.get_element_id_parts(),
         )
     
     def get_form_attrs(self) -> dict:
         """
         Extra possible form attributes rendered in the iFrame.
         """
         return {}
@@ -317,19 +341,20 @@
         
         try:
             return Base85_json_loads(context)
         except json.JSONDecodeError:
             pass
         return {}
     
+    
 class BlockFieldReplacementAdapter(BaseAdapter):
     js_constructor = "wagtail_fedit.editors.BlockFieldEditor"
 
     def get_response_data(self, parent_context = None):
-        data = super().get_response_data()
+        data = super().get_response_data(parent_context)
         data["html"] = wrap_adapter(
             request=self.request,
             adapter=self,
             context=parent_context,
             run_context_processors=True
         )
         return data
```

### Comparing `wagtail_fedit-1.5.3rc8/wagtail_fedit/adapters/block.py` & `wagtail_fedit-1.5.3rc9/wagtail_fedit/adapters/block.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 from django.db import models
 from django.utils import translation
 from django.utils.translation import gettext_lazy as _
-from django.utils.safestring import mark_safe
 from django.http import HttpRequest
 
 from wagtail.log_actions import log
 from wagtail.blocks import (
     StreamValue,
-    BoundBlock,
 )
 from wagtail.models import (
     RevisionMixin,
 )
 
 from .base import (
     BlockFieldReplacementAdapter,
```

### Comparing `wagtail_fedit-1.5.3rc8/wagtail_fedit/adapters/field.py` & `wagtail_fedit-1.5.3rc9/wagtail_fedit/adapters/field.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc8/wagtail_fedit/adapters/funcs.py` & `wagtail_fedit-1.5.3rc9/wagtail_fedit/adapters/funcs.py`

 * *Files 14% similar despite different names*

```diff
@@ -15,32 +15,39 @@
     return data
 
 
 class FuncAdapterMixin:
     base_identifier = None
     base_required_kwargs = []
     js_constructor = "wagtail_fedit.editors.BaseFuncEditor"
+    js_function = None
 
     @classproperty
     def identifier(cls):
         if not cls.base_identifier:
             raise NotImplementedError("base_identifier is required")
         
         return f"{cls.base_identifier}_func"
     
     @classproperty
     def required_kwargs(cls):
+
+        if cls.js_function:
+            return cls.base_required_kwargs + [
+                "target",
+            ]
+
         return cls.base_required_kwargs + [
             "name",
             "target",
         ]
 
     def get_response_data(self, parent_context=None):
         data = super().get_response_data(parent_context)
-        name = self.kwargs["name"]
+        name = self.js_function or self.kwargs["name"]
         target = self.kwargs["target"]
         target = target.format(object=self.object)
         data["func"] = {
             "name": name,
             "target": target,
         }
         return data
```

### Comparing `wagtail_fedit-1.5.3rc8/wagtail_fedit/adapters/misc.py` & `wagtail_fedit-1.5.3rc9/wagtail_fedit/adapters/misc.py`

 * *Files 11% similar despite different names*

```diff
@@ -31,18 +31,15 @@
         "target",
     ]
     optional_kwargs = [
         "css_variable_name",
     ]
     absolute_tokens = []
     js_constructor = "wagtail_fedit.editors.WagtailFeditFuncEditor"
-
-    def __init__(self, object, field_name: str, request: HttpRequest, **kwargs):
-        kwargs["name"] = "wagtail_fedit.funcs.backgroundImageFunc"
-        super().__init__(object, field_name, request, **kwargs)
+    js_function = "wagtail_fedit.funcs.backgroundImageFunc"
 
     def render_content(self, parent_context=None):
         return ""
 
     def get_response_data(self, parent_context=None):
         data = super().get_response_data(parent_context)
         image = getattr(self.object, self.field_name, None)
```

### Comparing `wagtail_fedit-1.5.3rc8/wagtail_fedit/adapters/registry.py` & `wagtail_fedit-1.5.3rc9/wagtail_fedit/adapters/registry.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc8/wagtail_fedit/forms/blocks.py` & `wagtail_fedit-1.5.3rc9/wagtail_fedit/forms/blocks.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc8/wagtail_fedit/forms/fields.py` & `wagtail_fedit-1.5.3rc9/wagtail_fedit/forms/fields.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc8/wagtail_fedit/hooks.py` & `wagtail_fedit-1.5.3rc9/wagtail_fedit/hooks.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc8/wagtail_fedit/locale/nl/LC_MESSAGES/django.mo` & `wagtail_fedit-1.5.3rc9/wagtail_fedit/locale/nl/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc8/wagtail_fedit/locale/nl/LC_MESSAGES/django.po` & `wagtail_fedit-1.5.3rc9/wagtail_fedit/locale/nl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc8/wagtail_fedit/models.py` & `wagtail_fedit-1.5.3rc9/wagtail_fedit/models.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc8/wagtail_fedit/settings.py` & `wagtail_fedit-1.5.3rc9/wagtail_fedit/settings.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc8/wagtail_fedit/static/wagtail_fedit/css/frontend.css` & `wagtail_fedit-1.5.3rc9/wagtail_fedit/static/wagtail_fedit/css/frontend.css`

 * *Files 1% similar despite different names*

```diff
@@ -23,26 +23,31 @@
     width: 100%;
     height: 100%;
     background-color: rgba(0, 0, 0, 0.05);
     outline: 2px solid #333333;
     pointer-events: none;
     z-index: 300;
 }
-.wagtail-fedit-adapter-wrapper.wagtail-fedit-field:has(.wagtail-fedit-adapter-wrapper) > .wagtail-fedit-buttons {
+.wagtail-fedit-adapter-wrapper:not(.wagtail-fedit-block):has(.wagtail-fedit-adapter-wrapper) > .wagtail-fedit-buttons {
     right: 30px;
 }
 .wagtail-fedit-buttons {
     display: flex;
     gap: 0.5em;
     border-radius: 0.5em;
     position: absolute;
     right: 0;
     z-index: 1;
 }
 
+.wagtail-fedit-adapter-wrapper.wagtail-fedit-inline {
+    display: flex;
+    flex-direction: row;
+}
+
 .wagtail-fedit-inline > .wagtail-fedit-buttons {
     display: inline-block;
     position: relative;
     margin-left: 0.25rem;
     margin-right: 0.25rem;
     vertical-align: top;
     left: unset;
```

### Comparing `wagtail_fedit-1.5.3rc8/wagtail_fedit/static/wagtail_fedit/css/furniture.css` & `wagtail_fedit-1.5.3rc9/wagtail_fedit/static/wagtail_fedit/css/furniture.css`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc8/wagtail_fedit/static/wagtail_fedit/css/userbar-menu.css` & `wagtail_fedit-1.5.3rc9/wagtail_fedit/static/wagtail_fedit/css/userbar-menu.css`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc8/wagtail_fedit/static/wagtail_fedit/js/frontend.js` & `wagtail_fedit-1.5.3rc9/wagtail_fedit/static/wagtail_fedit/js/frontend.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -114,39 +114,81 @@
     openModal() {
         this.#editor.makeModal();
     }
 
     closeModal() {
         this.#editor.closeModal();
     }
+
+    updateHtml(html) {
+
+        const update = (innerHtml) => {
+            const blockWrapper = this.#editor.wrapperElement;
+            const element = document.createElement("div");
+            element.innerHTML = innerHtml;
+            const newBlockWrapper = element.firstElementChild;
+            newBlockWrapper.classList.add("wagtail-fedit-initialized");
+            blockWrapper.parentNode.insertBefore(newBlockWrapper, blockWrapper);
+            blockWrapper.parentNode.removeChild(blockWrapper);
+            this.#editor.wrapperElement = newBlockWrapper;
+            this.#editor.initNewEditors();
+            this.#editor.init();
+
+            return blockWrapper;
+        }
+
+        if (typeof html === "string") {
+            update(html);
+            return;
+        }
+
+        if (typeof html === "function") {
+            this.#editor.wrapperElement.editorAPI = this;
+            html(update);
+            return;
+        }
+    }
+
+    execRelated(func) {
+        for (const wrapper of this.#editor.relatedWrappers) {
+            func(wrapper.editorAPI);
+        }
+    }
 }
 
 
 class BaseWagtailFeditEditor {
     constructor(options) {
         const {
             element = null,
         } = options;
 
         this.initialTitle = document.title;
 
         /**@type {HTMLElement} */
         this.wrapperElement = element;
+        this.api = new WagtailFeditorAPI(this);
         this.sharedContext = null;
         this.modalHtml = null;
         this.editBtn = null;
         this.init();
         this.iframe = null;
 
+
         if (window.location.hash === `#${this.wrapperElement.id}`) {
             this.makeModal();
             this.focus();
         }
     }
 
+    get relatedWrappers() {
+        const wrapperId = this.wrapperElement.dataset.wrapperId;
+        return document.querySelectorAll(`[data-wrapper-id="${wrapperId}"]`);
+    }
+
     focus() {
         this.wrapperElement.focus();
     }
 
     getEditUrl() {
         // build the edit url from relative edit url
         const url = new URL(window.location.href);
@@ -278,16 +320,15 @@
     }
 
     init() {
         this.sharedContext = this.wrapperElement.dataset.sharedContext;
         this.modalHtml = modalHtml.replace("__ID__", this.wrapperElement.dataset.id);
         this.editBtn = this.wrapperElement.querySelector(".wagtail-fedit-edit-button");
 
-        const api = new WagtailFeditorAPI(this);
-        this.wrapperElement.editorAPI = api;
+        this.wrapperElement.editorAPI = this.api;
 
         this.editBtn.addEventListener("click", async (e) => {
             e.preventDefault();
             e.stopPropagation();
             await this.makeModal();
         });
     }
@@ -347,54 +388,44 @@
     }
 }
 
 
 class BlockFieldEditor extends BaseWagtailFeditEditor {
     onResponse(response) {
         const html = response.html;
-
-        // Fade out the old block
-        const anim = this.wrapperElement.animate([{
-            opacity: 1
-        }, {
-            opacity: 0
-        }, ], {
-            duration: 350,
-            easing: "ease-in-out",
-        });
-
-        anim.onfinish = () => {
-            // replace the HTML of the block we are editing with the new HTML
-            const newBlock = document.createElement("div");
-            newBlock.innerHTML = html;
-            const blockWrapper = newBlock.firstElementChild;
-            blockWrapper.classList.add("wagtail-fedit-initialized");
-            this.wrapperElement.parentNode.insertBefore(blockWrapper, this.wrapperElement);
-            this.wrapperElement.parentNode.removeChild(this.wrapperElement);
-            blockWrapper.style.opacity = 0;
-            this.wrapperElement = blockWrapper;
-
-            // reinitialize possibly new / replaced editor instances
-            this.initNewEditors();
-
-            // reinitialize proper variables with from new HTML
-            this.init();
-
-            // Fade in the new block
-            const anim = blockWrapper.animate([{
-                opacity: 0
-            }, {
-                opacity: 1
-            }, ], {
-                duration: 350,
-                easing: "ease-in-out",
+        for (const wrapper of this.relatedWrappers) {
+            wrapper.editorAPI.updateHtml((update) => {
+                // Fade out the old block
+                const anim = wrapper.animate([{
+                    opacity: 1
+                }, {
+                    opacity: 0
+                }, ], {
+                    duration: 350,
+                    easing: "ease-in-out",
+                });
+
+                anim.onfinish = () => {
+
+                    const blockWrapper = update(html);
+
+                    // Fade in the new block
+                    const anim = blockWrapper.animate([{
+                        opacity: 0
+                    }, {
+                        opacity: 1
+                    }, ], {
+                        duration: 350,
+                        easing: "ease-in-out",
+                    });
+                    anim.onfinish = () => {
+                        blockWrapper.style.opacity = 1;
+                    };
+                }
             });
-            anim.onfinish = () => {
-                blockWrapper.style.opacity = 1;
-            };
         }
     }
 }
 
 
 class WagtailFeditPublishMenu {
     constructor(publishButton) {
```

### Comparing `wagtail_fedit-1.5.3rc8/wagtail_fedit/templates/wagtail_fedit/content/buttons/admin_link.html` & `wagtail_fedit-1.5.3rc9/wagtail_fedit/templates/wagtail_fedit/content/buttons/admin_link.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc8/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_adapter.html` & `wagtail_fedit-1.5.3rc9/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_adapter.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc8/wagtail_fedit/templates/wagtail_fedit/content/editable_adapter.html` & `wagtail_fedit-1.5.3rc9/wagtail_fedit/templates/wagtail_fedit/content/editable_adapter.html`

 * *Files 24% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-{% load fedit %}<div id="{{ adapter.get_element_id }}" class="wagtail-fedit-adapter-wrapper{% if shared_context.inline or adapter.inline %} wagtail-fedit-inline{%endif%} wagtail-fedit-{{ identifier }}" data-fedit-constructor="{{ js_constructor }}" {% if shared %} data-shared-context="{{ shared }}"{%endif%} data-edit-url="{{ edit_url }}">
+{% load fedit %}<div id="{{ unique_id }}" data-wrapper-id="{{ unique_id }}" class="wagtail-fedit-adapter-wrapper{% if shared_context.inline or adapter.inline %} wagtail-fedit-inline{%endif%} wagtail-fedit-{{ identifier }}" data-fedit-constructor="{{ js_constructor }}" {% if shared %} data-shared-context="{{ shared }}"{%endif%} data-edit-url="{{ edit_url }}">
     <div class="wagtail-fedit-buttons">
         {% for button in buttons %}
             {{ button }}
         {% endfor %}
     </div>{% render_adapter adapter %}
 </div>
```

### Comparing `wagtail_fedit-1.5.3rc8/wagtail_fedit/templates/wagtail_fedit/editor/action_confirm.html` & `wagtail_fedit-1.5.3rc9/wagtail_fedit/templates/wagtail_fedit/editor/action_confirm.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc8/wagtail_fedit/templates/wagtail_fedit/editor/action_publish_confirm.html` & `wagtail_fedit-1.5.3rc9/wagtail_fedit/templates/wagtail_fedit/editor/action_publish_confirm.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc8/wagtail_fedit/templates/wagtail_fedit/editor/adapter_form.html` & `wagtail_fedit-1.5.3rc9/wagtail_fedit/templates/wagtail_fedit/editor/adapter_form.html`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 {% load i18n wagtailadmin_tags %}
 <form id="wagtail-fedit-form" data-edit-form action="{{ edit_url }}" method="post" {% for k, v in form_attrs.items %}{{ k }}="{{ v|safe }}" {% endfor %}>
     {% csrf_token %}
     {% block form %}
-        {% panel id="wagtail-fedit-editor" icon="draft" heading=meta_field.verbose_name %}
+        {% panel id="wagtail-fedit-editor" icon="draft" heading=verbose_name %}
             <div class="wagtail-fedit-form">
                 {% for field in form %}
                     {% include "./field.html" %}
                 {% endfor %}
             </div>
         {% endpanel %}
     {% endblock %}
```

### Comparing `wagtail_fedit-1.5.3rc8/wagtail_fedit/templates/wagtail_fedit/editor/base_iframe.html` & `wagtail_fedit-1.5.3rc9/wagtail_fedit/templates/wagtail_fedit/editor/base_iframe.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc8/wagtail_fedit/templates/wagtail_fedit/icons/fedit-check-list.svg` & `wagtail_fedit-1.5.3rc9/wagtail_fedit/templates/wagtail_fedit/icons/fedit-check-list.svg`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc8/wagtail_fedit/templates/wagtail_fedit/icons/fedit-eye-closed.svg` & `wagtail_fedit-1.5.3rc9/wagtail_fedit/templates/wagtail_fedit/icons/fedit-eye-closed.svg`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc8/wagtail_fedit/templates/wagtail_fedit/icons/fedit-save.svg` & `wagtail_fedit-1.5.3rc9/wagtail_fedit/templates/wagtail_fedit/icons/fedit-save.svg`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc8/wagtail_fedit/templates/wagtail_fedit/icons/fedit-stop-sign.svg` & `wagtail_fedit-1.5.3rc9/wagtail_fedit/templates/wagtail_fedit/icons/fedit-stop-sign.svg`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc8/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit.html` & `wagtail_fedit-1.5.3rc9/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc8/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_view_live.html` & `wagtail_fedit-1.5.3rc9/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_view_live.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc8/wagtail_fedit/templates/wagtail_fedit/userbar/publish/item_fedit_publishing.html` & `wagtail_fedit-1.5.3rc9/wagtail_fedit/templates/wagtail_fedit/userbar/publish/item_fedit_publishing.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc8/wagtail_fedit/templatetags/__pycache__/fedit.cpython-311.pyc` & `wagtail_fedit-1.5.3rc9/wagtail_fedit/templatetags/__pycache__/fedit.cpython-311.pyc`

 * *Files 6% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0x206b2466 (Sun Apr 21 01:25:52 2024 UTC)
-files sz: 7961
+moddate:  0xb6602566 (Sun Apr 21 18:53:42 2024 UTC)
+files sz: 8664
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 11
    flags     : 0
    code
       0x9700640064016c006d015a010100640064026c026d035a036d045a046d
@@ -164,77 +164,77 @@
                254 MAKE_FUNCTION            0
                256 LOAD_CONST              22 ('AdapterNode')
                258 LOAD_NAME                4 (Node)
                260 PRECALL                  3
                264 CALL                     3
                274 STORE_NAME              39 (AdapterNode)
    
-   130         276 LOAD_NAME               34 (register)
+   138         276 LOAD_NAME               34 (register)
                278 LOAD_METHOD             40 (tag)
                300 LOAD_NAME               30 (TEMPLATE_TAG_NAME)
                302 KW_NAMES                23
                304 PRECALL                  1
                308 CALL                     1
    
-   131         318 LOAD_CONST              24 ('parser')
+   139         318 LOAD_CONST              24 ('parser')
                320 LOAD_NAME                9 (Parser)
                322 LOAD_CONST              25 ('token')
                324 LOAD_NAME               10 (Token)
                326 BUILD_TUPLE              4
-               328 LOAD_CONST              26 (<code object do_render_fedit, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Packages\wagtail_fedit\wagtail_fedit\templatetags\fedit.py", line 130>)
+               328 LOAD_CONST              26 (<code object do_render_fedit, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Packages\wagtail_fedit\wagtail_fedit\templatetags\fedit.py", line 138>)
                330 MAKE_FUNCTION            4 (annotations)
    
-   130         332 PRECALL                  0
+   138         332 PRECALL                  0
                336 CALL                     0
    
-   131         346 STORE_NAME              41 (do_render_fedit)
+   139         346 STORE_NAME              41 (do_render_fedit)
    
-   182         348 LOAD_NAME               34 (register)
+   195         348 LOAD_NAME               34 (register)
                350 LOAD_METHOD             42 (simple_tag)
                372 LOAD_CONST              27 (True)
                374 KW_NAMES                28
                376 PRECALL                  1
                380 CALL                     1
    
-   183         390 LOAD_CONST              17 ('context')
+   196         390 LOAD_CONST              17 ('context')
                392 LOAD_NAME                7 (Context)
                394 LOAD_CONST              29 ('adapter')
                396 LOAD_NAME               24 (BaseAdapter)
                398 LOAD_CONST              19 ('return')
                400 LOAD_NAME               37 (str)
                402 BUILD_TUPLE              6
-               404 LOAD_CONST              30 (<code object render_adapter, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Packages\wagtail_fedit\wagtail_fedit\templatetags\fedit.py", line 182>)
+               404 LOAD_CONST              30 (<code object render_adapter, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Packages\wagtail_fedit\wagtail_fedit\templatetags\fedit.py", line 195>)
                406 MAKE_FUNCTION            4 (annotations)
    
-   182         408 PRECALL                  0
+   195         408 PRECALL                  0
                412 CALL                     0
    
-   183         422 STORE_NAME              43 (render_adapter)
+   196         422 STORE_NAME              43 (render_adapter)
    
-   199         424 LOAD_NAME               34 (register)
+   212         424 LOAD_NAME               34 (register)
                426 LOAD_METHOD             44 (inclusion_tag)
                448 LOAD_CONST              31 ('wagtail_fedit/_hook_output.html')
                450 LOAD_CONST              32 ('fedit_scripts')
                452 LOAD_CONST              27 (True)
                454 KW_NAMES                33
                456 PRECALL                  3
                460 CALL                     3
    
-   200         470 LOAD_CONST              19 ('return')
+   213         470 LOAD_CONST              19 ('return')
                472 LOAD_NAME               45 (dict)
                474 BUILD_TUPLE              2
-               476 LOAD_CONST              34 (<code object static_hook_output, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Packages\wagtail_fedit\wagtail_fedit\templatetags\fedit.py", line 199>)
+               476 LOAD_CONST              34 (<code object static_hook_output, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Packages\wagtail_fedit\wagtail_fedit\templatetags\fedit.py", line 212>)
                478 MAKE_FUNCTION            4 (annotations)
    
-   199         480 PRECALL                  0
+   212         480 PRECALL                  0
                484 CALL                     0
    
-   200         494 STORE_NAME              46 (static_hook_output)
+   213         494 STORE_NAME              46 (static_hook_output)
    
-   230         496 LOAD_CONST              39 ((None, None))
+   243         496 LOAD_CONST              39 ((None, None))
                498 LOAD_CONST              24 ('parser')
                500 LOAD_NAME                9 (Parser)
                502 LOAD_CONST              35 ('tokens')
                504 LOAD_NAME               47 (list)
                506 LOAD_NAME               37 (str)
                508 BINARY_SUBSCR
                518 LOAD_CONST              36 ('kwarg_list')
@@ -244,15 +244,15 @@
                534 LOAD_CONST              37 ('absolute_tokens')
                536 LOAD_NAME               47 (list)
                538 LOAD_NAME               37 (str)
                540 BINARY_SUBSCR
                550 LOAD_CONST              19 ('return')
                552 LOAD_NAME               45 (dict)
                554 BUILD_TUPLE             10
-               556 LOAD_CONST              38 (<code object get_kwargs, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Packages\wagtail_fedit\wagtail_fedit\templatetags\fedit.py", line 230>)
+               556 LOAD_CONST              38 (<code object get_kwargs, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Packages\wagtail_fedit\wagtail_fedit\templatetags\fedit.py", line 243>)
                558 MAKE_FUNCTION            5 (defaults, annotations)
                560 STORE_NAME              48 (get_kwargs)
                562 LOAD_CONST               9 (None)
                564 RETURN_VALUE
    consts
       0
       ('Type',)
@@ -480,46 +480,49 @@
                argcount  : 2
                nlocals   : 12
                stacksize : 9
                flags     : 3
                code
                   0x97007c006a0000000000000000007d027c006a0100000000000000007d
                   0302007c006a0200000000000000007c017c02660269007c006a03000000
-                  0000000000a4018e015c0200007d027d0464017c017600721864027c0176
-                  0072147c0273127c016401190000000000000000007d057c016402190000
-                  000000000000007d0690016e1c7c0273987409000000000000000000006a
-                  050000000000000000740c0000000000000000000064037c006a07000000
-                  00000000006a08000000000000000069017a060000741200000000000000
-                  000000a6020000ab02000000000000000001007c01a00a00000000000000
-                  00000000000000000000000000a6000000ab0000000000000000007d0109
-                  007417000000000000000000007c006a0b00000000000000007c0102007c
-                  006a0700000000000000006a0c00000000000000007c01660169007c04a4
-                  018e01a6030000ab03000000000000000053002300741a00000000000000
-                  000000240072217d07741d00000000000000000000741f00000000000000
-                  0000007c07a6010000ab010000000000000000a6010000ab010000000000
-                  000000820164007d077e07770177007803590077017c0374210000000000
-                  00000000007c03a6010000ab01000000000000000064047a0a0000190000
-                  000000000000007d057c027d067423000000000000000000007421000000
-                  000000000000007c03a6010000ab01000000000000000064047a0a0000a6
-                  010000ab01000000000000000044005d487d087c037c0819000000000000
-                  0000007d0909007425000000000000000000007c067c09a6020000ab0200
-                  000000000000007d068c1c23007426000000000000000000002400722001
-                  0074270000000000000000000064057c026a1400000000000000006a0800
-                  000000000000009b0064067c099b009d04a6010000ab0100000000000000
-                  00820177007803590077017c01a015000000000000000000000000000000
-                  00000000006407a6010000ab0100000000000000007d0a02007c006a0700
-                  0000000000000064097c067c057c0a64089c037c04a4018e017d0b7c0ba0
-                  160000000000000000000000000000000000000000a6000000ab00000000
-                  00000000007210742f000000000000000000007c0a7c06a6020000ab0200
-                  0000000000000073297417000000000000000000007c006a0b0000000000
-                  0000007c017c0ba01800000000000000000000000000000000000000007c
-                  01a6010000ab010000000000000000a6030000ab03000000000000000053
-                  007417000000000000000000007c006a0b00000000000000007c01743300
-                  0000000000000000007c0a7c0b7c01a6030000ab030000000000000000a6
-                  030000ab0300000000000000005300
+                  0000000000a4018e015c0200007d027d0464017c017600722464027c0176
+                  0072207c02731e7c006a0400000000000000006a05000000000000000072
+                  127c016401190000000000000000007d057c016402190000000000000000
+                  007d0690016e3e7c02731c64027c01760072187c006a0400000000000000
+                  006a050000000000000000730c7c016402190000000000000000007d0664
+                  007d0590016e207c027398740d000000000000000000006a070000000000
+                  00000074100000000000000000000064037c006a0400000000000000006a
+                  09000000000000000069017a060000741400000000000000000000a60200
+                  00ab02000000000000000001007c01a00b00000000000000000000000000
+                  00000000000000a6000000ab0000000000000000007d0109007419000000
+                  000000000000007c006a0c00000000000000007c0102007c006a04000000
+                  00000000006a0d00000000000000007c01660169007c04a4018e01a60300
+                  00ab03000000000000000053002300741c00000000000000000000240072
+                  217d07741f000000000000000000007421000000000000000000007c07a6
+                  010000ab010000000000000000a6010000ab010000000000000000820164
+                  007d077e077701770078035900770164007d057c027d067c0372807c0374
+                  23000000000000000000007c03a6010000ab01000000000000000064047a
+                  0a0000190000000000000000007d05742500000000000000000000742300
+                  0000000000000000007c03a6010000ab01000000000000000064047a0a00
+                  00a6010000ab01000000000000000044005d487d087c037c081900000000
+                  00000000007d0909007427000000000000000000007c067c09a6020000ab
+                  0200000000000000007d068c1c2300742800000000000000000000240072
+                  20010074290000000000000000000064057c026a1500000000000000006a
+                  0900000000000000009b0064067c099b009d04a6010000ab010000000000
+                  000000820177007803590077017c01a01600000000000000000000000000
+                  000000000000006407a6010000ab0100000000000000007d0a02007c006a
+                  04000000000000000064097c067c057c0a64089c037c04a4018e017d0b7c
+                  0ba0170000000000000000000000000000000000000000a6000000ab0000
+                  0000000000000072107431000000000000000000007c0a7c06a6020000ab
+                  02000000000000000073297419000000000000000000007c006a0c000000
+                  00000000007c017c0ba01900000000000000000000000000000000000000
+                  007c01a6010000ab010000000000000000a6030000ab0300000000000000
+                  0053007419000000000000000000007c006a0c00000000000000007c0174
+                  35000000000000000000007c0a7c0b7c01a6030000ab0300000000000000
+                  00a6030000ab0300000000000000005300
                 72           0 RESUME                   0
                
                 73           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (model)
                             14 STORE_FAST               2 (model)
                
                 74          16 LOAD_FAST                0 (self)
@@ -544,276 +547,309 @@
                             68 UNPACK_SEQUENCE          2
                             72 STORE_FAST               2 (model)
                             74 STORE_FAST               4 (kwargs)
                
                 80          76 LOAD_CONST               1 ('wagtail_fedit_field')
                             78 LOAD_FAST                1 (context)
                             80 CONTAINS_OP              0
-                            82 POP_JUMP_FORWARD_IF_FALSE    24 (to 132)
+                            82 POP_JUMP_FORWARD_IF_FALSE    36 (to 156)
                
                 81          84 LOAD_CONST               2 ('wagtail_fedit_instance')
                             86 LOAD_FAST                1 (context)
                             88 CONTAINS_OP              0
-                            90 POP_JUMP_FORWARD_IF_FALSE    20 (to 132)
+                            90 POP_JUMP_FORWARD_IF_FALSE    32 (to 156)
                
                 82          92 LOAD_FAST                2 (model)
                
-                81          94 POP_JUMP_FORWARD_IF_TRUE    18 (to 132)
+                81          94 POP_JUMP_FORWARD_IF_TRUE    30 (to 156)
                
-                84          96 LOAD_FAST                1 (context)
-                            98 LOAD_CONST               1 ('wagtail_fedit_field')
-                           100 BINARY_SUBSCR
-                           110 STORE_FAST               5 (field_name)
-               
-                85         112 LOAD_FAST                1 (context)
-                           114 LOAD_CONST               2 ('wagtail_fedit_instance')
-                           116 BINARY_SUBSCR
-                           126 STORE_FAST               6 (obj)
-                           128 EXTENDED_ARG             1
-                           130 JUMP_FORWARD           284 (to 700)
-               
-                89     >>  132 LOAD_FAST                2 (model)
-                           134 POP_JUMP_FORWARD_IF_TRUE   152 (to 440)
-               
-                90         136 LOAD_GLOBAL              9 (NULL + warnings)
-                           148 LOAD_ATTR                5 (warn)
-               
-                91         158 LOAD_GLOBAL             12 (WARNING_MODEL_INSTANCE_NOT_AVAILABLE)
-               
-                92         170 LOAD_CONST               3 ('object')
-                           172 LOAD_FAST                0 (self)
-                           174 LOAD_ATTR                7 (adapter)
-                           184 LOAD_ATTR                8 (__name__)
-               
-                91         194 BUILD_MAP                1
-                           196 BINARY_OP                6 (%)
-               
-                94         200 LOAD_GLOBAL             18 (RuntimeWarning)
-               
-                90         212 PRECALL                  2
-                           216 CALL                     2
-                           226 POP_TOP
-               
-                97         228 LOAD_FAST                1 (context)
-                           230 LOAD_METHOD             10 (flatten)
-                           252 PRECALL                  0
-                           256 CALL                     0
-                           266 STORE_FAST               1 (context)
-               
-                99         268 NOP
-               
-               100         270 LOAD_GLOBAL             23 (NULL + as_var)
-                           282 LOAD_FAST                0 (self)
-                           284 LOAD_ATTR               11 (as_var)
-                           294 LOAD_FAST                1 (context)
-                           296 PUSH_NULL
-                           298 LOAD_FAST                0 (self)
-                           300 LOAD_ATTR                7 (adapter)
-                           310 LOAD_ATTR               12 (render_from_kwargs)
-               
-               101         320 LOAD_FAST                1 (context)
-               
-               100         322 BUILD_TUPLE              1
-                           324 BUILD_MAP                0
-               
-               101         326 LOAD_FAST                4 (kwargs)
-               
-               100         328 DICT_MERGE               1
-                           330 CALL_FUNCTION_EX         1
-                           332 PRECALL                  3
-                           336 CALL                     3
-                           346 RETURN_VALUE
-                       >>  348 PUSH_EXC_INFO
-               
-               103         350 LOAD_GLOBAL             26 (AdapterError)
-                           362 CHECK_EXC_MATCH
-                           364 POP_JUMP_FORWARD_IF_FALSE    33 (to 432)
-                           366 STORE_FAST               7 (e)
-               
-               104         368 LOAD_GLOBAL             29 (NULL + TemplateSyntaxError)
-                           380 LOAD_GLOBAL             31 (NULL + str)
-                           392 LOAD_FAST                7 (e)
-                           394 PRECALL                  1
-                           398 CALL                     1
-                           408 PRECALL                  1
-                           412 CALL                     1
-                           422 RAISE_VARARGS            1
-                       >>  424 LOAD_CONST               0 (None)
-                           426 STORE_FAST               7 (e)
-                           428 DELETE_FAST              7 (e)
-                           430 RERAISE                  1
-               
-               103     >>  432 RERAISE                  0
-                       >>  434 COPY                     3
-                           436 POP_EXCEPT
-                           438 RERAISE                  1
-               
-               106     >>  440 LOAD_FAST                3 (getters)
-                           442 LOAD_GLOBAL             33 (NULL + len)
-                           454 LOAD_FAST                3 (getters)
-                           456 PRECALL                  1
-                           460 CALL                     1
-                           470 LOAD_CONST               4 (1)
-                           472 BINARY_OP               10 (-)
-                           476 BINARY_SUBSCR
-                           486 STORE_FAST               5 (field_name)
-               
-               107         488 LOAD_FAST                2 (model)
-                           490 STORE_FAST               6 (obj)
-               
-               108         492 LOAD_GLOBAL             35 (NULL + range)
-                           504 LOAD_GLOBAL             33 (NULL + len)
-                           516 LOAD_FAST                3 (getters)
-                           518 PRECALL                  1
-                           522 CALL                     1
-                           532 LOAD_CONST               4 (1)
-                           534 BINARY_OP               10 (-)
-                           538 PRECALL                  1
-                           542 CALL                     1
-                           552 GET_ITER
-                       >>  554 FOR_ITER                72 (to 700)
-                           556 STORE_FAST               8 (i)
-               
-               109         558 LOAD_FAST                3 (getters)
-                           560 LOAD_FAST                8 (i)
-                           562 BINARY_SUBSCR
-                           572 STORE_FAST               9 (getter)
-               
-               110         574 NOP
-               
-               111         576 LOAD_GLOBAL             37 (NULL + getattr)
-                           588 LOAD_FAST                6 (obj)
-                           590 LOAD_FAST                9 (getter)
-                           592 PRECALL                  2
-                           596 CALL                     2
-                           606 STORE_FAST               6 (obj)
-                           608 JUMP_BACKWARD           28 (to 554)
-                       >>  610 PUSH_EXC_INFO
-               
-               112         612 LOAD_GLOBAL             38 (AttributeError)
-                           624 CHECK_EXC_MATCH
-                           626 POP_JUMP_FORWARD_IF_FALSE    32 (to 692)
-                           628 POP_TOP
-               
-               113         630 LOAD_GLOBAL             39 (NULL + AttributeError)
-                           642 LOAD_CONST               5 ('Object ')
-                           644 LOAD_FAST                2 (model)
-                           646 LOAD_ATTR               20 (__class__)
-                           656 LOAD_ATTR                8 (__name__)
-                           666 FORMAT_VALUE             0
-                           668 LOAD_CONST               6 (' does not have attribute ')
-                           670 LOAD_FAST                9 (getter)
-                           672 FORMAT_VALUE             0
-                           674 BUILD_STRING             4
-                           676 PRECALL                  1
-                           680 CALL                     1
-                           690 RAISE_VARARGS            1
-               
-               112     >>  692 RERAISE                  0
-                       >>  694 COPY                     3
-                           696 POP_EXCEPT
-                           698 RERAISE                  1
-               
-               115     >>  700 LOAD_FAST                1 (context)
-                           702 LOAD_METHOD             21 (get)
-                           724 LOAD_CONST               7 ('request')
-                           726 PRECALL                  1
-                           730 CALL                     1
-                           740 STORE_FAST              10 (request)
-               
-               116         742 PUSH_NULL
-                           744 LOAD_FAST                0 (self)
-                           746 LOAD_ATTR                7 (adapter)
-                           756 LOAD_CONST               9 (())
-               
-               117         758 LOAD_FAST                6 (obj)
-               
-               118         760 LOAD_FAST                5 (field_name)
-               
-               119         762 LOAD_FAST               10 (request)
-               
-               116         764 LOAD_CONST               8 (('object', 'field_name', 'request'))
-                           766 BUILD_CONST_KEY_MAP      3
-               
-               120         768 LOAD_FAST                4 (kwargs)
-               
-               116         770 DICT_MERGE               1
-                           772 CALL_FUNCTION_EX         1
-                           774 STORE_FAST              11 (adapter)
-               
-               123         776 LOAD_FAST               11 (adapter)
-                           778 LOAD_METHOD             22 (check_permissions)
-                           800 PRECALL                  0
-                           804 CALL                     0
-                           814 POP_JUMP_FORWARD_IF_FALSE    16 (to 848)
-               
-               124         816 LOAD_GLOBAL             47 (NULL + _can_edit)
-                           828 LOAD_FAST               10 (request)
-                           830 LOAD_FAST                6 (obj)
-                           832 PRECALL                  2
-                           836 CALL                     2
-               
-               123         846 POP_JUMP_FORWARD_IF_TRUE    41 (to 930)
-               
-               125     >>  848 LOAD_GLOBAL             23 (NULL + as_var)
-                           860 LOAD_FAST                0 (self)
-                           862 LOAD_ATTR               11 (as_var)
-                           872 LOAD_FAST                1 (context)
-                           874 LOAD_FAST               11 (adapter)
-                           876 LOAD_METHOD             24 (render_content)
-                           898 LOAD_FAST                1 (context)
-                           900 PRECALL                  1
-                           904 CALL                     1
-                           914 PRECALL                  3
-                           918 CALL                     3
-                           928 RETURN_VALUE
-               
-               127     >>  930 LOAD_GLOBAL             23 (NULL + as_var)
-                           942 LOAD_FAST                0 (self)
-                           944 LOAD_ATTR               11 (as_var)
-                           954 LOAD_FAST                1 (context)
-                           956 LOAD_GLOBAL             51 (NULL + wrap_adapter)
-                           968 LOAD_FAST               10 (request)
-                           970 LOAD_FAST               11 (adapter)
-                           972 LOAD_FAST                1 (context)
-                           974 PRECALL                  3
-                           978 CALL                     3
-                           988 PRECALL                  3
-                           992 CALL                     3
-                          1002 RETURN_VALUE
+                82          96 LOAD_FAST                0 (self)
+                            98 LOAD_ATTR                4 (adapter)
+                           108 LOAD_ATTR                5 (field_required)
+               
+                81         118 POP_JUMP_FORWARD_IF_FALSE    18 (to 156)
+               
+                84         120 LOAD_FAST                1 (context)
+                           122 LOAD_CONST               1 ('wagtail_fedit_field')
+                           124 BINARY_SUBSCR
+                           134 STORE_FAST               5 (field_name)
+               
+                85         136 LOAD_FAST                1 (context)
+                           138 LOAD_CONST               2 ('wagtail_fedit_instance')
+                           140 BINARY_SUBSCR
+                           150 STORE_FAST               6 (obj)
+                           152 EXTENDED_ARG             1
+                           154 JUMP_FORWARD           318 (to 792)
+               
+                87     >>  156 LOAD_FAST                2 (model)
+                           158 POP_JUMP_FORWARD_IF_TRUE    28 (to 216)
+                           160 LOAD_CONST               2 ('wagtail_fedit_instance')
+                           162 LOAD_FAST                1 (context)
+                           164 CONTAINS_OP              0
+                           166 POP_JUMP_FORWARD_IF_FALSE    24 (to 216)
+                           168 LOAD_FAST                0 (self)
+                           170 LOAD_ATTR                4 (adapter)
+                           180 LOAD_ATTR                5 (field_required)
+                           190 POP_JUMP_FORWARD_IF_TRUE    12 (to 216)
+               
+                88         192 LOAD_FAST                1 (context)
+                           194 LOAD_CONST               2 ('wagtail_fedit_instance')
+                           196 BINARY_SUBSCR
+                           206 STORE_FAST               6 (obj)
+               
+                89         208 LOAD_CONST               0 (None)
+                           210 STORE_FAST               5 (field_name)
+                           212 EXTENDED_ARG             1
+                           214 JUMP_FORWARD           288 (to 792)
+               
+                93     >>  216 LOAD_FAST                2 (model)
+                           218 POP_JUMP_FORWARD_IF_TRUE   152 (to 524)
+               
+                94         220 LOAD_GLOBAL             13 (NULL + warnings)
+                           232 LOAD_ATTR                7 (warn)
+               
+                95         242 LOAD_GLOBAL             16 (WARNING_MODEL_INSTANCE_NOT_AVAILABLE)
+               
+                96         254 LOAD_CONST               3 ('object')
+                           256 LOAD_FAST                0 (self)
+                           258 LOAD_ATTR                4 (adapter)
+                           268 LOAD_ATTR                9 (__name__)
+               
+                95         278 BUILD_MAP                1
+                           280 BINARY_OP                6 (%)
+               
+                98         284 LOAD_GLOBAL             20 (RuntimeWarning)
+               
+                94         296 PRECALL                  2
+                           300 CALL                     2
+                           310 POP_TOP
+               
+               101         312 LOAD_FAST                1 (context)
+                           314 LOAD_METHOD             11 (flatten)
+                           336 PRECALL                  0
+                           340 CALL                     0
+                           350 STORE_FAST               1 (context)
+               
+               103         352 NOP
+               
+               104         354 LOAD_GLOBAL             25 (NULL + as_var)
+                           366 LOAD_FAST                0 (self)
+                           368 LOAD_ATTR               12 (as_var)
+                           378 LOAD_FAST                1 (context)
+                           380 PUSH_NULL
+                           382 LOAD_FAST                0 (self)
+                           384 LOAD_ATTR                4 (adapter)
+                           394 LOAD_ATTR               13 (render_from_kwargs)
+               
+               105         404 LOAD_FAST                1 (context)
+               
+               104         406 BUILD_TUPLE              1
+                           408 BUILD_MAP                0
+               
+               105         410 LOAD_FAST                4 (kwargs)
+               
+               104         412 DICT_MERGE               1
+                           414 CALL_FUNCTION_EX         1
+                           416 PRECALL                  3
+                           420 CALL                     3
+                           430 RETURN_VALUE
+                       >>  432 PUSH_EXC_INFO
+               
+               107         434 LOAD_GLOBAL             28 (AdapterError)
+                           446 CHECK_EXC_MATCH
+                           448 POP_JUMP_FORWARD_IF_FALSE    33 (to 516)
+                           450 STORE_FAST               7 (e)
+               
+               108         452 LOAD_GLOBAL             31 (NULL + TemplateSyntaxError)
+                           464 LOAD_GLOBAL             33 (NULL + str)
+                           476 LOAD_FAST                7 (e)
+                           478 PRECALL                  1
+                           482 CALL                     1
+                           492 PRECALL                  1
+                           496 CALL                     1
+                           506 RAISE_VARARGS            1
+                       >>  508 LOAD_CONST               0 (None)
+                           510 STORE_FAST               7 (e)
+                           512 DELETE_FAST              7 (e)
+                           514 RERAISE                  1
+               
+               107     >>  516 RERAISE                  0
+                       >>  518 COPY                     3
+                           520 POP_EXCEPT
+                           522 RERAISE                  1
+               
+               110     >>  524 LOAD_CONST               0 (None)
+                           526 STORE_FAST               5 (field_name)
+               
+               111         528 LOAD_FAST                2 (model)
+                           530 STORE_FAST               6 (obj)
+               
+               112         532 LOAD_FAST                3 (getters)
+                           534 POP_JUMP_FORWARD_IF_FALSE   128 (to 792)
+               
+               113         536 LOAD_FAST                3 (getters)
+                           538 LOAD_GLOBAL             35 (NULL + len)
+                           550 LOAD_FAST                3 (getters)
+                           552 PRECALL                  1
+                           556 CALL                     1
+                           566 LOAD_CONST               4 (1)
+                           568 BINARY_OP               10 (-)
+                           572 BINARY_SUBSCR
+                           582 STORE_FAST               5 (field_name)
+               
+               115         584 LOAD_GLOBAL             37 (NULL + range)
+                           596 LOAD_GLOBAL             35 (NULL + len)
+                           608 LOAD_FAST                3 (getters)
+                           610 PRECALL                  1
+                           614 CALL                     1
+                           624 LOAD_CONST               4 (1)
+                           626 BINARY_OP               10 (-)
+                           630 PRECALL                  1
+                           634 CALL                     1
+                           644 GET_ITER
+                       >>  646 FOR_ITER                72 (to 792)
+                           648 STORE_FAST               8 (i)
+               
+               116         650 LOAD_FAST                3 (getters)
+                           652 LOAD_FAST                8 (i)
+                           654 BINARY_SUBSCR
+                           664 STORE_FAST               9 (getter)
+               
+               117         666 NOP
+               
+               118         668 LOAD_GLOBAL             39 (NULL + getattr)
+                           680 LOAD_FAST                6 (obj)
+                           682 LOAD_FAST                9 (getter)
+                           684 PRECALL                  2
+                           688 CALL                     2
+                           698 STORE_FAST               6 (obj)
+                           700 JUMP_BACKWARD           28 (to 646)
+                       >>  702 PUSH_EXC_INFO
+               
+               119         704 LOAD_GLOBAL             40 (AttributeError)
+                           716 CHECK_EXC_MATCH
+                           718 POP_JUMP_FORWARD_IF_FALSE    32 (to 784)
+                           720 POP_TOP
+               
+               120         722 LOAD_GLOBAL             41 (NULL + AttributeError)
+                           734 LOAD_CONST               5 ('Object ')
+                           736 LOAD_FAST                2 (model)
+                           738 LOAD_ATTR               21 (__class__)
+                           748 LOAD_ATTR                9 (__name__)
+                           758 FORMAT_VALUE             0
+                           760 LOAD_CONST               6 (' does not have attribute ')
+                           762 LOAD_FAST                9 (getter)
+                           764 FORMAT_VALUE             0
+                           766 BUILD_STRING             4
+                           768 PRECALL                  1
+                           772 CALL                     1
+                           782 RAISE_VARARGS            1
+               
+               119     >>  784 RERAISE                  0
+                       >>  786 COPY                     3
+                           788 POP_EXCEPT
+                           790 RERAISE                  1
+               
+               123     >>  792 LOAD_FAST                1 (context)
+                           794 LOAD_METHOD             22 (get)
+                           816 LOAD_CONST               7 ('request')
+                           818 PRECALL                  1
+                           822 CALL                     1
+                           832 STORE_FAST              10 (request)
+               
+               124         834 PUSH_NULL
+                           836 LOAD_FAST                0 (self)
+                           838 LOAD_ATTR                4 (adapter)
+                           848 LOAD_CONST               9 (())
+               
+               125         850 LOAD_FAST                6 (obj)
+               
+               126         852 LOAD_FAST                5 (field_name)
+               
+               127         854 LOAD_FAST               10 (request)
+               
+               124         856 LOAD_CONST               8 (('object', 'field_name', 'request'))
+                           858 BUILD_CONST_KEY_MAP      3
+               
+               128         860 LOAD_FAST                4 (kwargs)
+               
+               124         862 DICT_MERGE               1
+                           864 CALL_FUNCTION_EX         1
+                           866 STORE_FAST              11 (adapter)
+               
+               131         868 LOAD_FAST               11 (adapter)
+                           870 LOAD_METHOD             23 (check_permissions)
+                           892 PRECALL                  0
+                           896 CALL                     0
+                           906 POP_JUMP_FORWARD_IF_FALSE    16 (to 940)
+               
+               132         908 LOAD_GLOBAL             49 (NULL + _can_edit)
+                           920 LOAD_FAST               10 (request)
+                           922 LOAD_FAST                6 (obj)
+                           924 PRECALL                  2
+                           928 CALL                     2
+               
+               131         938 POP_JUMP_FORWARD_IF_TRUE    41 (to 1022)
+               
+               133     >>  940 LOAD_GLOBAL             25 (NULL + as_var)
+                           952 LOAD_FAST                0 (self)
+                           954 LOAD_ATTR               12 (as_var)
+                           964 LOAD_FAST                1 (context)
+                           966 LOAD_FAST               11 (adapter)
+                           968 LOAD_METHOD             25 (render_content)
+                           990 LOAD_FAST                1 (context)
+                           992 PRECALL                  1
+                           996 CALL                     1
+                          1006 PRECALL                  3
+                          1010 CALL                     3
+                          1020 RETURN_VALUE
+               
+               135     >> 1022 LOAD_GLOBAL             25 (NULL + as_var)
+                          1034 LOAD_FAST                0 (self)
+                          1036 LOAD_ATTR               12 (as_var)
+                          1046 LOAD_FAST                1 (context)
+                          1048 LOAD_GLOBAL             53 (NULL + wrap_adapter)
+                          1060 LOAD_FAST               10 (request)
+                          1062 LOAD_FAST               11 (adapter)
+                          1064 LOAD_FAST                1 (context)
+                          1066 PRECALL                  3
+                          1070 CALL                     3
+                          1080 PRECALL                  3
+                          1084 CALL                     3
+                          1094 RETURN_VALUE
                ExceptionTable:
-                 270 to 344 -> 348 [0]
-                 348 to 366 -> 434 [1] lasti
-                 368 to 422 -> 424 [1] lasti
-                 424 to 432 -> 434 [1] lasti
-                 576 to 606 -> 610 [1]
-                 610 to 692 -> 694 [2] lasti
+                 354 to 428 -> 432 [0]
+                 432 to 450 -> 518 [1] lasti
+                 452 to 506 -> 508 [1] lasti
+                 508 to 516 -> 518 [1] lasti
+                 668 to 698 -> 702 [1]
+                 702 to 784 -> 786 [2] lasti
                consts
                   None
                   'wagtail_fedit_field'
                   'wagtail_fedit_instance'
                   'object'
                   1
                   'Object '
                   ' does not have attribute '
                   'request'
                   ('object', 'field_name', 'request')
                   ()
-               names      ('model', 'getters', '_resolve_expressions', 'kwargs', 'warnings', 'warn', 'WARNING_MODEL_INSTANCE_NOT_AVAILABLE', 'adapter', '__name__', 'RuntimeWarning', 'flatten', 'as_var', 'render_from_kwargs', 'AdapterError', 'TemplateSyntaxError', 'str', 'len', 'range', 'getattr', 'AttributeError', '__class__', 'get', 'check_permissions', '_can_edit', 'render_content', 'wrap_adapter')
+               names      ('model', 'getters', '_resolve_expressions', 'kwargs', 'adapter', 'field_required', 'warnings', 'warn', 'WARNING_MODEL_INSTANCE_NOT_AVAILABLE', '__name__', 'RuntimeWarning', 'flatten', 'as_var', 'render_from_kwargs', 'AdapterError', 'TemplateSyntaxError', 'str', 'len', 'range', 'getattr', 'AttributeError', '__class__', 'get', 'check_permissions', '_can_edit', 'render_content', 'wrap_adapter')
                varnames   ('self', 'context', 'model', 'getters', 'kwargs', 'field_name', 'obj', 'e', 'i', 'getter', 'request', 'adapter')
                freevars   ()
                cellvars   ()
                filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Packages\\wagtail_fedit\\wagtail_fedit\\templatetags\\fedit.py'
                name       'render'
                firstlineno 72
                lnotab
-                  0x02010e010e020e0104ff04010cff0c040801080102ff02031001140404
-                  0116010c0118ff06030cfc100728020201320102ff040102ff1603120140
-                  ff080330010401420110010201240112013eff08032a0110010201020102
-                  fd040402fc060728011eff02025202
+                  0x02010e010e020e0104ff04010cff0c040801080102ff020116ff020310
+                  011402240110010804040116010c0118ff06030cfc100728020201320102
+                  ff040102ff1603120140ff08030401040104013002420110010201240112
+                  013eff08042a0110010201020102fd040402fc060728011eff02025202
             (None,)
          names      ('__name__', '__module__', '__qualname__', 'signing', 'TimestampSigner', 'signer', 'Type', 'BaseAdapter', 'FilterExpression', 'list', 'str', '__init__', '_resolve_expressions', 'render')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Packages\\wagtail_fedit\\wagtail_fedit\\templatetags\\fedit.py'
          name       'AdapterNode'
@@ -832,226 +868,241 @@
             0x97007c01a0000000000000000000000000000000000000000000a60000
             00ab0000000000000000007d027c02a00100000000000000000000000000
             000000000000006401a6010000ab0100000000000000007d037c02a00100
             000000000000000000000000000000000000006401a6010000ab01000000
             00000000007d0409007404000000000000000000007c0419000000000000
             0000007d056e212300740600000000000000000000240072140100740900
             00000000000000000064027c049b0064039d03a6010000ab010000000000
-            0000008201770078035900770164045c0200007d067d077c0272937c02a0
+            0000008201770078035900770164045c0200007d067d077c0272ad7c02a0
             0100000000000000000000000000000000000000006401a6010000ab0100
             000000000000007d087c08a0050000000000000000000000000000000000
             0000006405a6010000ab0100000000000000007d07740d00000000000000
-            0000007c07a6010000ab01000000000000000064066b0000000000721b7c
-            0764011900000000000000000064076b0300000000720f74090000000000
-            00000000006408a6010000ab0100000000000000008201740d0000000000
-            00000000007c07a6010000ab01000000000000000064096b040000000072
-            287c00a00700000000000000000000000000000000000000007c07a00100
-            000000000000000000000000000000000000006401a6010000ab01000000
-            0000000000a6010000ab0100000000000000007d0664007d097c0272667c
-            02740d000000000000000000007c02a6010000ab01000000000000000064
-            067a0a000019000000000000000000640a6b0200000000724a7c02a00100
-            00000000000000000000000000000000000000740d000000000000000000
-            007c02a6010000ab01000000000000000064097a0a0000a6010000ab0100
-            000000000000007d097c02a0010000000000000000000000000000000000
-            000000740d000000000000000000007c02a6010000ab0100000000000000
-            0064097a0a0000a6010000ab010000000000000000010074110000000000
-            00000000007c007c027c056a0900000000000000007c056a0a0000000000
-            000000a6040000ab0400000000000000007d0a7417000000000000000000
-            00640c7c057c067c077c09640b9c047c0aa4018e015300
-         130           0 RESUME                   0
+            0000007c07a6010000ab01000000000000000064066b000000000072227c
+            0764011900000000000000000064076b030000000072167c056a07000000
+            0000000000720f7409000000000000000000006408a6010000ab01000000
+            00000000008201740d000000000000000000007c07a6010000ab01000000
+            000000000064096b040000000073137c0764011900000000000000000064
+            076b0300000000722f7c056a07000000000000000073287c00a008000000
+            00000000000000000000000000000000007c07a001000000000000000000
+            00000000000000000000006401a6010000ab010000000000000000a60100
+            00ab0100000000000000007d0664007d097c0272667c02740d0000000000
+            00000000007c02a6010000ab01000000000000000064067a0a0000190000
+            00000000000000640a6b0200000000724a7c02a001000000000000000000
+            0000000000000000000000740d000000000000000000007c02a6010000ab
+            01000000000000000064097a0a0000a6010000ab0100000000000000007d
+            097c02a0010000000000000000000000000000000000000000740d000000
+            000000000000007c02a6010000ab01000000000000000064097a0a0000a6
+            010000ab01000000000000000001007413000000000000000000007c007c
+            027c056a0a00000000000000007c056a0b0000000000000000a6040000ab
+            0400000000000000007d0a741900000000000000000000640c7c057c067c
+            077c09640b9c047c0aa4018e015300
+         138           0 RESUME                   0
          
-         133           2 LOAD_FAST                1 (token)
+         141           2 LOAD_FAST                1 (token)
                        4 LOAD_METHOD              0 (split_contents)
                       26 PRECALL                  0
                       30 CALL                     0
                       40 STORE_FAST               2 (tokens)
          
-         135          42 LOAD_FAST                2 (tokens)
+         143          42 LOAD_FAST                2 (tokens)
                       44 LOAD_METHOD              1 (pop)
                       66 LOAD_CONST               1 (0)
                       68 PRECALL                  1
                       72 CALL                     1
                       82 STORE_FAST               3 (_)
          
-         136          84 LOAD_FAST                2 (tokens)
+         144          84 LOAD_FAST                2 (tokens)
                       86 LOAD_METHOD              1 (pop)
                      108 LOAD_CONST               1 (0)
                      110 PRECALL                  1
                      114 CALL                     1
                      124 STORE_FAST               4 (adapter_id)
          
-         138         126 NOP
+         146         126 NOP
          
-         139         128 LOAD_GLOBAL              4 (adapter_registry)
+         147         128 LOAD_GLOBAL              4 (adapter_registry)
                      140 LOAD_FAST                4 (adapter_id)
                      142 BINARY_SUBSCR
                      152 STORE_FAST               5 (adapter)
                      154 JUMP_FORWARD            33 (to 222)
                  >>  156 PUSH_EXC_INFO
          
-         140         158 LOAD_GLOBAL              6 (RegistryLookUpError)
+         148         158 LOAD_GLOBAL              6 (RegistryLookUpError)
                      170 CHECK_EXC_MATCH
                      172 POP_JUMP_FORWARD_IF_FALSE    20 (to 214)
                      174 POP_TOP
          
-         141         176 LOAD_GLOBAL              9 (NULL + TemplateSyntaxError)
+         149         176 LOAD_GLOBAL              9 (NULL + TemplateSyntaxError)
                      188 LOAD_CONST               2 ("No adapter found with identifier '")
                      190 LOAD_FAST                4 (adapter_id)
                      192 FORMAT_VALUE             0
                      194 LOAD_CONST               3 ("'")
                      196 BUILD_STRING             3
                      198 PRECALL                  1
                      202 CALL                     1
                      212 RAISE_VARARGS            1
          
-         140     >>  214 RERAISE                  0
+         148     >>  214 RERAISE                  0
                  >>  216 COPY                     3
                      218 POP_EXCEPT
                      220 RERAISE                  1
          
-         143     >>  222 LOAD_CONST               4 ((None, None))
+         151     >>  222 LOAD_CONST               4 ((None, None))
                      224 UNPACK_SEQUENCE          2
                      228 STORE_FAST               6 (model)
                      230 STORE_FAST               7 (model_tokens)
          
-         144         232 LOAD_FAST                2 (tokens)
-                     234 POP_JUMP_FORWARD_IF_FALSE   147 (to 530)
+         152         232 LOAD_FAST                2 (tokens)
+                     234 POP_JUMP_FORWARD_IF_FALSE   173 (to 582)
          
-         145         236 LOAD_FAST                2 (tokens)
+         153         236 LOAD_FAST                2 (tokens)
                      238 LOAD_METHOD              1 (pop)
                      260 LOAD_CONST               1 (0)
                      262 PRECALL                  1
                      266 CALL                     1
                      276 STORE_FAST               8 (model__field)
          
-         146         278 LOAD_FAST                8 (model__field)
+         154         278 LOAD_FAST                8 (model__field)
                      280 LOAD_METHOD              5 (split)
                      302 LOAD_CONST               5 ('.')
                      304 PRECALL                  1
                      308 CALL                     1
                      318 STORE_FAST               7 (model_tokens)
          
-         148         320 LOAD_GLOBAL             13 (NULL + len)
+         158         320 LOAD_GLOBAL             13 (NULL + len)
                      332 LOAD_FAST                7 (model_tokens)
                      334 PRECALL                  1
                      338 CALL                     1
                      348 LOAD_CONST               6 (2)
                      350 COMPARE_OP               0 (<)
-                     356 POP_JUMP_FORWARD_IF_FALSE    27 (to 412)
+                     356 POP_JUMP_FORWARD_IF_FALSE    34 (to 426)
          
-         149         358 LOAD_FAST                7 (model_tokens)
+         159         358 LOAD_FAST                7 (model_tokens)
                      360 LOAD_CONST               1 (0)
                      362 BINARY_SUBSCR
                      372 LOAD_CONST               7 ('from_context')
                      374 COMPARE_OP               3 (!=)
-                     380 POP_JUMP_FORWARD_IF_FALSE    15 (to 412)
-         
-         150         382 LOAD_GLOBAL              9 (NULL + TemplateSyntaxError)
-         
-         151         394 LOAD_CONST               8 ("Model and field name are required: 'mymodel.myfield' or 'from_context'")
-         
-         150         396 PRECALL                  1
-                     400 CALL                     1
-                     410 RAISE_VARARGS            1
-         
-         154     >>  412 LOAD_GLOBAL             13 (NULL + len)
-                     424 LOAD_FAST                7 (model_tokens)
-                     426 PRECALL                  1
-                     430 CALL                     1
-                     440 LOAD_CONST               9 (1)
-                     442 COMPARE_OP               4 (>)
-                     448 POP_JUMP_FORWARD_IF_FALSE    40 (to 530)
-         
-         157         450 LOAD_FAST                0 (parser)
-                     452 LOAD_METHOD              7 (compile_filter)
-                     474 LOAD_FAST                7 (model_tokens)
-                     476 LOAD_METHOD              1 (pop)
-                     498 LOAD_CONST               1 (0)
-                     500 PRECALL                  1
-                     504 CALL                     1
-                     514 PRECALL                  1
-                     518 CALL                     1
-                     528 STORE_FAST               6 (model)
-         
-         159     >>  530 LOAD_CONST               0 (None)
-                     532 STORE_FAST               9 (as_var)
-         
-         160         534 LOAD_FAST                2 (tokens)
-                     536 POP_JUMP_FORWARD_IF_FALSE   102 (to 742)
-                     538 LOAD_FAST                2 (tokens)
-                     540 LOAD_GLOBAL             13 (NULL + len)
-                     552 LOAD_FAST                2 (tokens)
-                     554 PRECALL                  1
-                     558 CALL                     1
-                     568 LOAD_CONST               6 (2)
-                     570 BINARY_OP               10 (-)
-                     574 BINARY_SUBSCR
-                     584 LOAD_CONST              10 ('as')
-                     586 COMPARE_OP               2 (==)
-                     592 POP_JUMP_FORWARD_IF_FALSE    74 (to 742)
-         
-         161         594 LOAD_FAST                2 (tokens)
-                     596 LOAD_METHOD              1 (pop)
-                     618 LOAD_GLOBAL             13 (NULL + len)
-                     630 LOAD_FAST                2 (tokens)
-                     632 PRECALL                  1
-                     636 CALL                     1
-                     646 LOAD_CONST               9 (1)
-                     648 BINARY_OP               10 (-)
-                     652 PRECALL                  1
-                     656 CALL                     1
-                     666 STORE_FAST               9 (as_var)
-         
-         162         668 LOAD_FAST                2 (tokens)
-                     670 LOAD_METHOD              1 (pop)
-                     692 LOAD_GLOBAL             13 (NULL + len)
-                     704 LOAD_FAST                2 (tokens)
-                     706 PRECALL                  1
-                     710 CALL                     1
-                     720 LOAD_CONST               9 (1)
-                     722 BINARY_OP               10 (-)
-                     726 PRECALL                  1
-                     730 CALL                     1
-                     740 POP_TOP
-         
-         165     >>  742 LOAD_GLOBAL             17 (NULL + get_kwargs)
-         
-         166         754 LOAD_FAST                0 (parser)
-         
-         167         756 LOAD_FAST                2 (tokens)
-         
-         168         758 LOAD_FAST                5 (adapter)
-                     760 LOAD_ATTR                9 (required_kwargs)
-         
-         169         770 LOAD_FAST                5 (adapter)
-                     772 LOAD_ATTR               10 (absolute_tokens)
-         
-         165         782 PRECALL                  4
-                     786 CALL                     4
-                     796 STORE_FAST              10 (kwargs)
-         
-         172         798 LOAD_GLOBAL             23 (NULL + AdapterNode)
-                     810 LOAD_CONST              12 (())
-         
-         173         812 LOAD_FAST                5 (adapter)
-         
-         174         814 LOAD_FAST                6 (model)
-         
-         175         816 LOAD_FAST                7 (model_tokens)
-         
-         176         818 LOAD_FAST                9 (as_var)
-         
-         172         820 LOAD_CONST              11 (('adapter', 'model', 'getters', 'as_var'))
-                     822 BUILD_CONST_KEY_MAP      4
-         
-         177         824 LOAD_FAST               10 (kwargs)
-         
-         172         826 DICT_MERGE               1
-                     828 CALL_FUNCTION_EX         1
-                     830 RETURN_VALUE
+                     380 POP_JUMP_FORWARD_IF_FALSE    22 (to 426)
+                     382 LOAD_FAST                5 (adapter)
+                     384 LOAD_ATTR                7 (field_required)
+                     394 POP_JUMP_FORWARD_IF_FALSE    15 (to 426)
+         
+         160         396 LOAD_GLOBAL              9 (NULL + TemplateSyntaxError)
+         
+         161         408 LOAD_CONST               8 ("Model and field name are required: 'mymodel.myfield' or 'from_context'")
+         
+         160         410 PRECALL                  1
+                     414 CALL                     1
+                     424 RAISE_VARARGS            1
+         
+         165     >>  426 LOAD_GLOBAL             13 (NULL + len)
+                     438 LOAD_FAST                7 (model_tokens)
+                     440 PRECALL                  1
+                     444 CALL                     1
+                     454 LOAD_CONST               9 (1)
+                     456 COMPARE_OP               4 (>)
+                     462 POP_JUMP_FORWARD_IF_TRUE    19 (to 502)
+         
+         166         464 LOAD_FAST                7 (model_tokens)
+                     466 LOAD_CONST               1 (0)
+                     468 BINARY_SUBSCR
+                     478 LOAD_CONST               7 ('from_context')
+                     480 COMPARE_OP               3 (!=)
+                     486 POP_JUMP_FORWARD_IF_FALSE    47 (to 582)
+                     488 LOAD_FAST                5 (adapter)
+                     490 LOAD_ATTR                7 (field_required)
+                     500 POP_JUMP_FORWARD_IF_TRUE    40 (to 582)
+         
+         171     >>  502 LOAD_FAST                0 (parser)
+                     504 LOAD_METHOD              8 (compile_filter)
+                     526 LOAD_FAST                7 (model_tokens)
+                     528 LOAD_METHOD              1 (pop)
+                     550 LOAD_CONST               1 (0)
+                     552 PRECALL                  1
+                     556 CALL                     1
+                     566 PRECALL                  1
+                     570 CALL                     1
+                     580 STORE_FAST               6 (model)
+         
+         173     >>  582 LOAD_CONST               0 (None)
+                     584 STORE_FAST               9 (as_var)
+         
+         174         586 LOAD_FAST                2 (tokens)
+                     588 POP_JUMP_FORWARD_IF_FALSE   102 (to 794)
+                     590 LOAD_FAST                2 (tokens)
+                     592 LOAD_GLOBAL             13 (NULL + len)
+                     604 LOAD_FAST                2 (tokens)
+                     606 PRECALL                  1
+                     610 CALL                     1
+                     620 LOAD_CONST               6 (2)
+                     622 BINARY_OP               10 (-)
+                     626 BINARY_SUBSCR
+                     636 LOAD_CONST              10 ('as')
+                     638 COMPARE_OP               2 (==)
+                     644 POP_JUMP_FORWARD_IF_FALSE    74 (to 794)
+         
+         175         646 LOAD_FAST                2 (tokens)
+                     648 LOAD_METHOD              1 (pop)
+                     670 LOAD_GLOBAL             13 (NULL + len)
+                     682 LOAD_FAST                2 (tokens)
+                     684 PRECALL                  1
+                     688 CALL                     1
+                     698 LOAD_CONST               9 (1)
+                     700 BINARY_OP               10 (-)
+                     704 PRECALL                  1
+                     708 CALL                     1
+                     718 STORE_FAST               9 (as_var)
+         
+         176         720 LOAD_FAST                2 (tokens)
+                     722 LOAD_METHOD              1 (pop)
+                     744 LOAD_GLOBAL             13 (NULL + len)
+                     756 LOAD_FAST                2 (tokens)
+                     758 PRECALL                  1
+                     762 CALL                     1
+                     772 LOAD_CONST               9 (1)
+                     774 BINARY_OP               10 (-)
+                     778 PRECALL                  1
+                     782 CALL                     1
+                     792 POP_TOP
+         
+         178     >>  794 LOAD_GLOBAL             19 (NULL + get_kwargs)
+         
+         179         806 LOAD_FAST                0 (parser)
+         
+         180         808 LOAD_FAST                2 (tokens)
+         
+         181         810 LOAD_FAST                5 (adapter)
+                     812 LOAD_ATTR               10 (required_kwargs)
+         
+         182         822 LOAD_FAST                5 (adapter)
+                     824 LOAD_ATTR               11 (absolute_tokens)
+         
+         178         834 PRECALL                  4
+                     838 CALL                     4
+                     848 STORE_FAST              10 (kwargs)
+         
+         185         850 LOAD_GLOBAL             25 (NULL + AdapterNode)
+                     862 LOAD_CONST              12 (())
+         
+         186         864 LOAD_FAST                5 (adapter)
+         
+         187         866 LOAD_FAST                6 (model)
+         
+         188         868 LOAD_FAST                7 (model_tokens)
+         
+         189         870 LOAD_FAST                9 (as_var)
+         
+         185         872 LOAD_CONST              11 (('adapter', 'model', 'getters', 'as_var'))
+                     874 BUILD_CONST_KEY_MAP      4
+         
+         190         876 LOAD_FAST               10 (kwargs)
+         
+         185         878 DICT_MERGE               1
+                     880 CALL_FUNCTION_EX         1
+                     882 RETURN_VALUE
          ExceptionTable:
            128 to 152 -> 156 [0]
            156 to 214 -> 216 [1] lasti
          consts
             None
             0
             "No adapter found with identifier '"
@@ -1061,25 +1112,25 @@
             2
             'from_context'
             "Model and field name are required: 'mymodel.myfield' or 'from_context'"
             1
             'as'
             ('adapter', 'model', 'getters', 'as_var')
             ()
-         names      ('split_contents', 'pop', 'adapter_registry', 'RegistryLookUpError', 'TemplateSyntaxError', 'split', 'len', 'compile_filter', 'get_kwargs', 'required_kwargs', 'absolute_tokens', 'AdapterNode')
+         names      ('split_contents', 'pop', 'adapter_registry', 'RegistryLookUpError', 'TemplateSyntaxError', 'split', 'len', 'field_required', 'compile_filter', 'get_kwargs', 'required_kwargs', 'absolute_tokens', 'AdapterNode')
          varnames   ('parser', 'token', 'tokens', '_', 'adapter_id', 'adapter', 'model', 'model_tokens', 'model__field', 'as_var', 'kwargs')
          freevars   ()
          cellvars   ()
          filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Packages\\wagtail_fedit\\wagtail_fedit\\templatetags\\fedit.py'
          name       'do_render_fedit'
-         firstlineno 130
+         firstlineno 138
          lnotab
-            0x020328022a012a0202011e01120126ff08030a0104012a012a02260118
-            010c0102ff10042603500204013c014a014a030c01020102010c010cfc10
-            070e0102010201020102fc040502fb
+            0x020328022a012a0202011e01120126ff08030a0104012a012a04260126
+            010c0102ff100526012605500204013c014a014a020c01020102010c010c
+            fc10070e0102010201020102fc040502fb
       True
       ('takes_context',)
       'adapter'
       code
          argcount  : 2
          nlocals   : 3
          stacksize : 3
@@ -1088,59 +1139,59 @@
             0x970069007d0264017c007600720b7c006401190000000000000000007d
             027c0064013d007c00a00000000000000000000000000000000000000000
             007c02a6010000ab01000000000000000001007c016a0100000000000000
             007c0064023c0000007c016a0200000000000000007c0064033c0000007c
             016a0300000000000000007c0064043c0000007c01a00400000000000000
             000000000000000000000000007c00a6010000ab01000000000000000053
             00
-         182           0 RESUME                   0
+         195           0 RESUME                   0
          
-         184           2 BUILD_MAP                0
+         197           2 BUILD_MAP                0
                        4 STORE_FAST               2 (parent_context)
          
-         186           6 LOAD_CONST               1 ('parent_context')
+         199           6 LOAD_CONST               1 ('parent_context')
                        8 LOAD_FAST                0 (context)
                       10 CONTAINS_OP              0
                       12 POP_JUMP_FORWARD_IF_FALSE    11 (to 36)
          
-         187          14 LOAD_FAST                0 (context)
+         200          14 LOAD_FAST                0 (context)
                       16 LOAD_CONST               1 ('parent_context')
                       18 BINARY_SUBSCR
                       28 STORE_FAST               2 (parent_context)
          
-         188          30 LOAD_FAST                0 (context)
+         201          30 LOAD_FAST                0 (context)
                       32 LOAD_CONST               1 ('parent_context')
                       34 DELETE_SUBSCR
          
-         190     >>   36 LOAD_FAST                0 (context)
+         203     >>   36 LOAD_FAST                0 (context)
                       38 LOAD_METHOD              0 (update)
                       60 LOAD_FAST                2 (parent_context)
                       62 PRECALL                  1
                       66 CALL                     1
                       76 POP_TOP
          
-         192          78 LOAD_FAST                1 (adapter)
+         205          78 LOAD_FAST                1 (adapter)
                       80 LOAD_ATTR                1 (field_name)
                       90 LOAD_FAST                0 (context)
                       92 LOAD_CONST               2 ('wagtail_fedit_field')
                       94 STORE_SUBSCR
          
-         193          98 LOAD_FAST                1 (adapter)
+         206          98 LOAD_FAST                1 (adapter)
                      100 LOAD_ATTR                2 (object)
                      110 LOAD_FAST                0 (context)
                      112 LOAD_CONST               3 ('wagtail_fedit_instance')
                      114 STORE_SUBSCR
          
-         194         118 LOAD_FAST                1 (adapter)
+         207         118 LOAD_FAST                1 (adapter)
                      120 LOAD_ATTR                3 (request)
                      130 LOAD_FAST                0 (context)
                      132 LOAD_CONST               4 ('request')
                      134 STORE_SUBSCR
          
-         196         138 LOAD_FAST                1 (adapter)
+         209         138 LOAD_FAST                1 (adapter)
                      140 LOAD_METHOD              4 (render_content)
                      162 LOAD_FAST                0 (context)
                      164 PRECALL                  1
                      168 CALL                     1
                      178 RETURN_VALUE
          consts
             None
@@ -1150,15 +1201,15 @@
             'request'
          names      ('update', 'field_name', 'object', 'request', 'render_content')
          varnames   ('context', 'adapter', 'parent_context')
          freevars   ()
          cellvars   ()
          filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Packages\\wagtail_fedit\\wagtail_fedit\\templatetags\\fedit.py'
          name       'render_adapter'
-         firstlineno 182
+         firstlineno 195
          lnotab 0x020204020801100106022a02140114011402
       'wagtail_fedit/_hook_output.html'
       'fedit_scripts'
       ('name', 'takes_context')
       code
          argcount  : 2
          nlocals   : 7
@@ -1175,107 +1226,107 @@
             00530067007d04740f000000000000000000006a0800000000000000007c
             03a6010000ab01000000000000000044005d417d0502007c057c02a60100
             00ab0100000000000000007d067413000000000000000000007c06741400
             0000000000000000007416000000000000000000006602a6020000ab0200
             0000000000000073037c0667017d067c04a00c0000000000000000000000
             0000000000000000007c06a6010000ab01000000000000000001008c4264
             067c0469015300
-         199           0 RESUME                   0
+         212           0 RESUME                   0
          
-         201           2 LOAD_FAST                1 (css_or_js)
+         214           2 LOAD_FAST                1 (css_or_js)
                        4 LOAD_METHOD              0 (lower)
                       26 PRECALL                  0
                       30 CALL                     0
                       40 STORE_FAST               1 (css_or_js)
          
-         203          42 LOAD_FAST                1 (css_or_js)
+         216          42 LOAD_FAST                1 (css_or_js)
                       44 LOAD_CONST               1 (('css', 'js'))
                       46 CONTAINS_OP              1
                       48 POP_JUMP_FORWARD_IF_FALSE    15 (to 80)
          
-         204          50 LOAD_GLOBAL              3 (NULL + ValueError)
+         217          50 LOAD_GLOBAL              3 (NULL + ValueError)
                       62 LOAD_CONST               2 ("Invalid argument, must be 'css' or 'js'")
                       64 PRECALL                  1
                       68 CALL                     1
                       78 RAISE_VARARGS            1
          
-         206     >>   80 LOAD_FAST                0 (context)
+         219     >>   80 LOAD_FAST                0 (context)
                       82 LOAD_METHOD              2 (get)
                      104 LOAD_CONST               3 ('request')
                      106 PRECALL                  1
                      110 CALL                     1
                      120 STORE_FAST               2 (request)
          
-         208         122 LOAD_FAST                1 (css_or_js)
+         221         122 LOAD_FAST                1 (css_or_js)
                      124 LOAD_CONST               4 ('css')
                      126 COMPARE_OP               2 (==)
                      132 POP_JUMP_FORWARD_IF_FALSE     8 (to 150)
          
-         209         134 LOAD_GLOBAL              6 (REGISTER_CSS)
+         222         134 LOAD_GLOBAL              6 (REGISTER_CSS)
                      146 STORE_FAST               3 (hook_name)
                      148 JUMP_FORWARD             7 (to 164)
          
-         211     >>  150 LOAD_GLOBAL              8 (REGISTER_JS)
+         224     >>  150 LOAD_GLOBAL              8 (REGISTER_JS)
                      162 STORE_FAST               3 (hook_name)
          
-         213     >>  164 LOAD_GLOBAL             11 (NULL + getattr)
+         226     >>  164 LOAD_GLOBAL             11 (NULL + getattr)
                      176 LOAD_FAST                2 (request)
                      178 LOAD_GLOBAL             12 (FEDIT_PREVIEW_VAR)
                      190 LOAD_CONST               5 (False)
                      192 PRECALL                  3
                      196 CALL                     3
                      206 POP_JUMP_FORWARD_IF_TRUE     2 (to 212)
          
-         214         208 BUILD_MAP                0
+         227         208 BUILD_MAP                0
                      210 RETURN_VALUE
          
-         216     >>  212 BUILD_LIST               0
+         229     >>  212 BUILD_LIST               0
                      214 STORE_FAST               4 (files)
          
-         217         216 LOAD_GLOBAL             15 (NULL + hooks)
+         230         216 LOAD_GLOBAL             15 (NULL + hooks)
                      228 LOAD_ATTR                8 (get_hooks)
                      238 LOAD_FAST                3 (hook_name)
                      240 PRECALL                  1
                      244 CALL                     1
                      254 GET_ITER
                  >>  256 FOR_ITER                65 (to 388)
                      258 STORE_FAST               5 (hook)
          
-         218         260 PUSH_NULL
+         231         260 PUSH_NULL
                      262 LOAD_FAST                5 (hook)
                      264 LOAD_FAST                2 (request)
                      266 PRECALL                  1
                      270 CALL                     1
                      280 STORE_FAST               6 (ret)
          
-         220         282 LOAD_GLOBAL             19 (NULL + isinstance)
+         233         282 LOAD_GLOBAL             19 (NULL + isinstance)
                      294 LOAD_FAST                6 (ret)
                      296 LOAD_GLOBAL             20 (list)
                      308 LOAD_GLOBAL             22 (tuple)
                      320 BUILD_TUPLE              2
                      322 PRECALL                  2
                      326 CALL                     2
                      336 POP_JUMP_FORWARD_IF_TRUE     3 (to 344)
          
-         221         338 LOAD_FAST                6 (ret)
+         234         338 LOAD_FAST                6 (ret)
                      340 BUILD_LIST               1
                      342 STORE_FAST               6 (ret)
          
-         223     >>  344 LOAD_FAST                4 (files)
+         236     >>  344 LOAD_FAST                4 (files)
                      346 LOAD_METHOD             12 (extend)
                      368 LOAD_FAST                6 (ret)
                      370 PRECALL                  1
                      374 CALL                     1
                      384 POP_TOP
                      386 JUMP_BACKWARD           66 (to 256)
          
-         226     >>  388 LOAD_CONST               6 ('hook_output')
+         239     >>  388 LOAD_CONST               6 ('hook_output')
                      390 LOAD_FAST                4 (files)
          
-         225         392 BUILD_MAP                1
+         238         392 BUILD_MAP                1
                      394 RETURN_VALUE
          consts
             None
             ('css', 'js')
             "Invalid argument, must be 'css' or 'js'"
             'request'
             'css'
@@ -1283,15 +1334,15 @@
             'hook_output'
          names      ('lower', 'ValueError', 'get', 'REGISTER_CSS', 'REGISTER_JS', 'getattr', 'FEDIT_PREVIEW_VAR', 'hooks', 'get_hooks', 'isinstance', 'list', 'tuple', 'extend')
          varnames   ('context', 'css_or_js', 'request', 'hook_name', 'files', 'hook', 'ret')
          freevars   ()
          cellvars   ()
          filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Packages\\wagtail_fedit\\wagtail_fedit\\templatetags\\fedit.py'
          name       'static_hook_output'
-         firstlineno 199
+         firstlineno 212
          lnotab
             0x0202280208011e022a020c0110020e022c01040204012c011602380106
             022c0304ff
       'tokens'
       'kwarg_list'
       'absolute_tokens'
       code
@@ -1319,204 +1370,204 @@
             086404190000000000000000007d097c097c037600721374070000000000
             000000000064077c099b0064089d03a6010000ab01000000000000000082
             017c00a00400000000000000000000000000000000000000007c08640319
             000000000000000000a6010000ab0100000000000000007c057c093c0000
             0064057d0490018c147c0244005d187d0b7c0b7c0576017212740b000000
             0000000000000064097c0b9b009d02a6010000ab01000000000000000082
             018c197c055300
-         230           0 RESUME                   0
+         243           0 RESUME                   0
          
-         231           2 LOAD_CONST               1 (False)
+         244           2 LOAD_CONST               1 (False)
                        4 STORE_FAST               4 (had_kwargs)
          
-         232           6 BUILD_MAP                0
+         245           6 BUILD_MAP                0
                        8 STORE_FAST               5 (kwargs)
          
-         234          10 LOAD_FAST                2 (kwarg_list)
+         247          10 LOAD_FAST                2 (kwarg_list)
                       12 POP_JUMP_FORWARD_IF_TRUE     2 (to 18)
          
-         235          14 BUILD_LIST               0
+         248          14 BUILD_LIST               0
                       16 STORE_FAST               2 (kwarg_list)
          
-         237     >>   18 LOAD_FAST                3 (absolute_tokens)
+         250     >>   18 LOAD_FAST                3 (absolute_tokens)
                       20 POP_JUMP_FORWARD_IF_TRUE     2 (to 26)
          
-         238          22 BUILD_LIST               0
+         251          22 BUILD_LIST               0
                       24 STORE_FAST               3 (absolute_tokens)
          
-         240     >>   26 LOAD_GLOBAL              1 (NULL + enumerate)
+         253     >>   26 LOAD_GLOBAL              1 (NULL + enumerate)
                       38 LOAD_FAST                1 (tokens)
                       40 PRECALL                  1
                       44 CALL                     1
                       54 GET_ITER
                  >>   56 EXTENDED_ARG             1
                       58 FOR_ITER               274 (to 608)
                       60 UNPACK_SEQUENCE          2
                       64 STORE_FAST               6 (i)
                       66 STORE_FAST               7 (token)
          
-         241          68 LOAD_FAST                7 (token)
+         254          68 LOAD_FAST                7 (token)
                       70 LOAD_METHOD              1 (split)
                       92 LOAD_CONST               2 ('=')
                       94 PRECALL                  1
                       98 CALL                     1
                      108 STORE_FAST               8 (split)
          
-         242         110 LOAD_GLOBAL              5 (NULL + len)
+         255         110 LOAD_GLOBAL              5 (NULL + len)
                      122 LOAD_FAST                8 (split)
                      124 PRECALL                  1
                      128 CALL                     1
                      138 LOAD_CONST               3 (1)
                      140 COMPARE_OP               2 (==)
                      146 POP_JUMP_FORWARD_IF_FALSE    89 (to 326)
                      148 LOAD_GLOBAL              5 (NULL + len)
                      160 LOAD_FAST                2 (kwarg_list)
                      162 PRECALL                  1
                      166 CALL                     1
                      176 LOAD_FAST                6 (i)
                      178 COMPARE_OP               4 (>)
                      184 POP_JUMP_FORWARD_IF_FALSE    70 (to 326)
          
-         243         186 LOAD_FAST                8 (split)
+         256         186 LOAD_FAST                8 (split)
                      188 LOAD_CONST               4 (0)
                      190 BINARY_SUBSCR
                      200 LOAD_FAST                3 (absolute_tokens)
                      202 CONTAINS_OP              0
                      204 POP_JUMP_FORWARD_IF_FALSE    12 (to 230)
          
-         244         206 LOAD_CONST               5 (True)
+         257         206 LOAD_CONST               5 (True)
                      208 LOAD_FAST                5 (kwargs)
                      210 LOAD_FAST                8 (split)
                      212 LOAD_CONST               4 (0)
                      214 BINARY_SUBSCR
                      224 STORE_SUBSCR
          
-         245         228 JUMP_BACKWARD           87 (to 56)
+         258         228 JUMP_BACKWARD           87 (to 56)
          
-         247     >>  230 LOAD_FAST                4 (had_kwargs)
+         260     >>  230 LOAD_FAST                4 (had_kwargs)
                      232 POP_JUMP_FORWARD_IF_FALSE    15 (to 264)
          
-         248         234 LOAD_GLOBAL              7 (NULL + ValueError)
+         261         234 LOAD_GLOBAL              7 (NULL + ValueError)
                      246 LOAD_CONST               6 ('Unexpected positional argument after keyword argument')
                      248 PRECALL                  1
                      252 CALL                     1
                      262 RAISE_VARARGS            1
          
-         250     >>  264 LOAD_FAST                0 (parser)
+         263     >>  264 LOAD_FAST                0 (parser)
                      266 LOAD_METHOD              4 (compile_filter)
                      288 LOAD_FAST                7 (token)
                      290 PRECALL                  1
                      294 CALL                     1
                      304 LOAD_FAST                5 (kwargs)
                      306 LOAD_FAST                2 (kwarg_list)
                      308 LOAD_FAST                6 (i)
                      310 BINARY_SUBSCR
                      320 STORE_SUBSCR
                      324 JUMP_BACKWARD          135 (to 56)
          
-         251     >>  326 LOAD_GLOBAL              5 (NULL + len)
+         264     >>  326 LOAD_GLOBAL              5 (NULL + len)
                      338 LOAD_FAST                8 (split)
                      340 PRECALL                  1
                      344 CALL                     1
                      354 LOAD_CONST               3 (1)
                      356 COMPARE_OP               2 (==)
                      362 POP_JUMP_FORWARD_IF_FALSE    57 (to 478)
          
-         252         364 LOAD_FAST                8 (split)
+         265         364 LOAD_FAST                8 (split)
                      366 LOAD_CONST               4 (0)
                      368 BINARY_SUBSCR
                      378 LOAD_FAST                3 (absolute_tokens)
                      380 CONTAINS_OP              0
                      382 POP_JUMP_FORWARD_IF_FALSE    12 (to 408)
          
-         253         384 LOAD_CONST               5 (True)
+         266         384 LOAD_CONST               5 (True)
                      386 LOAD_FAST                5 (kwargs)
                      388 LOAD_FAST                8 (split)
                      390 LOAD_CONST               4 (0)
                      392 BINARY_SUBSCR
                      402 STORE_SUBSCR
          
-         254         406 JUMP_BACKWARD          176 (to 56)
+         267         406 JUMP_BACKWARD          176 (to 56)
          
-         256     >>  408 LOAD_FAST                8 (split)
+         269     >>  408 LOAD_FAST                8 (split)
                      410 LOAD_CONST               4 (0)
                      412 BINARY_SUBSCR
                      422 STORE_FAST               9 (key)
          
-         257         424 LOAD_FAST                0 (parser)
+         270         424 LOAD_FAST                0 (parser)
                      426 LOAD_METHOD              4 (compile_filter)
                      448 LOAD_FAST                9 (key)
                      450 PRECALL                  1
                      454 CALL                     1
                      464 STORE_FAST              10 (value)
          
-         258         466 LOAD_FAST               10 (value)
+         271         466 LOAD_FAST               10 (value)
                      468 LOAD_FAST                5 (kwargs)
                      470 LOAD_FAST                9 (key)
                      472 STORE_SUBSCR
                      476 JUMP_BACKWARD          211 (to 56)
          
-         260     >>  478 LOAD_FAST                8 (split)
+         273     >>  478 LOAD_FAST                8 (split)
                      480 LOAD_CONST               4 (0)
                      482 BINARY_SUBSCR
                      492 STORE_FAST               9 (key)
          
-         263         494 LOAD_FAST                9 (key)
+         276         494 LOAD_FAST                9 (key)
                      496 LOAD_FAST                3 (absolute_tokens)
                      498 CONTAINS_OP              0
                      500 POP_JUMP_FORWARD_IF_FALSE    19 (to 540)
          
-         264         502 LOAD_GLOBAL              7 (NULL + ValueError)
+         277         502 LOAD_GLOBAL              7 (NULL + ValueError)
                      514 LOAD_CONST               7 ('Keyword argument ')
                      516 LOAD_FAST                9 (key)
                      518 FORMAT_VALUE             0
                      520 LOAD_CONST               8 (' cannot be resolved; it will not be parsed as a variable.')
                      522 BUILD_STRING             3
                      524 PRECALL                  1
                      528 CALL                     1
                      538 RAISE_VARARGS            1
          
-         266     >>  540 LOAD_FAST                0 (parser)
+         279     >>  540 LOAD_FAST                0 (parser)
                      542 LOAD_METHOD              4 (compile_filter)
                      564 LOAD_FAST                8 (split)
                      566 LOAD_CONST               3 (1)
                      568 BINARY_SUBSCR
                      578 PRECALL                  1
                      582 CALL                     1
                      592 LOAD_FAST                5 (kwargs)
                      594 LOAD_FAST                9 (key)
                      596 STORE_SUBSCR
          
-         267         600 LOAD_CONST               5 (True)
+         280         600 LOAD_CONST               5 (True)
                      602 STORE_FAST               4 (had_kwargs)
                      604 EXTENDED_ARG             1
                      606 JUMP_BACKWARD          276 (to 56)
          
-         269     >>  608 LOAD_FAST                2 (kwarg_list)
+         282     >>  608 LOAD_FAST                2 (kwarg_list)
                      610 GET_ITER
                  >>  612 FOR_ITER                24 (to 662)
                      614 STORE_FAST              11 (kwarg)
          
-         270         616 LOAD_FAST               11 (kwarg)
+         283         616 LOAD_FAST               11 (kwarg)
                      618 LOAD_FAST                5 (kwargs)
                      620 CONTAINS_OP              1
                      622 POP_JUMP_FORWARD_IF_FALSE    18 (to 660)
          
-         271         624 LOAD_GLOBAL             11 (NULL + TemplateSyntaxError)
+         284         624 LOAD_GLOBAL             11 (NULL + TemplateSyntaxError)
                      636 LOAD_CONST               9 ('Missing required keyword argument ')
                      638 LOAD_FAST               11 (kwarg)
                      640 FORMAT_VALUE             0
                      642 BUILD_STRING             2
                      644 PRECALL                  1
                      648 CALL                     1
                      658 RAISE_VARARGS            1
          
-         270     >>  660 JUMP_BACKWARD           25 (to 612)
+         283     >>  660 JUMP_BACKWARD           25 (to 612)
          
-         273     >>  662 LOAD_FAST                5 (kwargs)
+         286     >>  662 LOAD_FAST                5 (kwargs)
                      664 RETURN_VALUE
          consts
             None
             False
             '='
             1
             0
@@ -1527,24 +1578,24 @@
             'Missing required keyword argument '
          names      ('enumerate', 'split', 'len', 'ValueError', 'compile_filter', 'TemplateSyntaxError')
          varnames   ('parser', 'tokens', 'kwarg_list', 'absolute_tokens', 'had_kwargs', 'kwargs', 'i', 'token', 'split', 'key', 'value', 'kwarg')
          freevars   ()
          cellvars   ()
          filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Packages\\wagtail_fedit\\wagtail_fedit\\templatetags\\fedit.py'
          name       'get_kwargs'
-         firstlineno 230
+         firstlineno 243
          lnotab
             0x02010401040204010402040104022a012a014c0114011601020204011e
             023e01260114011601020210012a010c021003080126023c010802080108
             0124ff0203
       (None, None)
    names      ('typing', 'Type', 'django.template', 'library', 'Node', 'TemplateSyntaxError', 'django.template.context', 'Context', 'django.template.base', 'Parser', 'Token', 'FilterExpression', 'django.http', 'HttpRequest', 'django.urls', 'reverse', 'django.core', 'signing', 'wagtail', 'hooks', 'warnings', 'adapters', 'adapter_registry', 'RegistryLookUpError', 'BaseAdapter', 'AdapterError', 'utils', 'wrap_adapter', '_can_edit', 'FEDIT_PREVIEW_VAR', 'TEMPLATE_TAG_NAME', 'REGISTER_CSS', 'REGISTER_JS', 'Library', 'register', 'WARNING_FIELD_NAME_NOT_AVAILABLE', 'WARNING_MODEL_INSTANCE_NOT_AVAILABLE', 'str', 'as_var', 'AdapterNode', 'tag', 'do_render_fedit', 'simple_tag', 'render_adapter', 'inclusion_tag', 'dict', 'static_hook_output', 'list', 'get_kwargs')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Packages\\wagtail_fedit\\wagtail_fedit\\templatetags\\fedit.py'
    name       '<module>'
    firstlineno 1
    lnotab
       0x00ff02010c0114030c0314040c010c010c020c0208021806180610061e
-      030401040318071c4e2a010eff0e0102332a0112ff0e0102102e010aff0e
+      030401040318071c562a010eff0e0102382a0112ff0e0102102e010aff0e
       01021e
```

### Comparing `wagtail_fedit-1.5.3rc8/wagtail_fedit/templatetags/fedit.py` & `wagtail_fedit-1.5.3rc9/wagtail_fedit/templatetags/fedit.py`

 * *Files 4% similar despite different names*

```diff
@@ -75,19 +75,23 @@
 
         model, kwargs = self._resolve_expressions(
             context, model, **self.kwargs,
         )
 
         if "wagtail_fedit_field" in context\
             and "wagtail_fedit_instance" in context\
-            and not model:
+            and not model and self.adapter.field_required:
 
             field_name = context["wagtail_fedit_field"]
             obj = context["wagtail_fedit_instance"]
 
+        elif not model and "wagtail_fedit_instance" in context and not self.adapter.field_required:
+            obj = context["wagtail_fedit_instance"]
+            field_name = None
+            
         else:
 
             if not model:
                 warnings.warn(
                     WARNING_MODEL_INSTANCE_NOT_AVAILABLE % {
                         "object": self.adapter.__name__,
                     },
@@ -99,22 +103,26 @@
                 try:
                     return as_var(self.as_var, context, self.adapter.render_from_kwargs(
                         context, **kwargs,
                     ))
                 except AdapterError as e:
                     raise TemplateSyntaxError(str(e))
 
-            field_name = getters[len(getters)-1]
+            field_name = None
             obj = model
-            for i in range(len(getters) - 1):
-                getter = getters[i]
-                try:
-                    obj = getattr(obj, getter)
-                except AttributeError:
-                    raise AttributeError(f"Object {model.__class__.__name__} does not have attribute {getter}")
+            if getters:
+                field_name = getters[len(getters) - 1]
+
+                for i in range(len(getters) - 1):
+                    getter = getters[i]
+                    try:
+                        obj = getattr(obj, getter)
+                    except AttributeError:
+                        raise AttributeError(f"Object {model.__class__.__name__} does not have attribute {getter}")
+                    
 
         request = context.get("request")
         adapter = self.adapter(
             object=obj,
             field_name=field_name,
             request=request,
             **kwargs,
@@ -140,32 +148,37 @@
     except RegistryLookUpError:
         raise TemplateSyntaxError(f"No adapter found with identifier '{adapter_id}'")
 
     model, model_tokens = None, None
     if tokens:
         model__field = tokens.pop(0)
         model_tokens = model__field.split(".")
-
+        
+        # If the field is required; the length must be at least 2,
+        # or the first token must be "from_context"
         if len(model_tokens) < 2:
-            if model_tokens[0] != "from_context":
+            if model_tokens[0] != "from_context" and adapter.field_required:
                 raise TemplateSyntaxError(
                     "Model and field name are required: 'mymodel.myfield' or 'from_context'",
                 )
 
-        if len(model_tokens) > 1:
+        # If the field is not required; the length could be 1 by specifying only a model.
+        if len(model_tokens) > 1 or (
+            model_tokens[0] != "from_context" and not adapter.field_required
+        ):
+            # mymodel
             # mymodel.myfield
             # mymodel.related_field.myfield
             model = parser.compile_filter(model_tokens.pop(0))
 
     as_var = None
     if tokens and tokens[len(tokens)-2] == "as":
         as_var = tokens.pop(len(tokens)-1)
         tokens.pop(len(tokens)-1)
 
-
     kwargs = get_kwargs(
         parser,
         tokens,
         adapter.required_kwargs,
         adapter.absolute_tokens,
     )
```

### Comparing `wagtail_fedit-1.5.3rc8/wagtail_fedit/test/core/migrations/0001_initial.py` & `wagtail_fedit-1.5.3rc9/wagtail_fedit/test/core/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc8/wagtail_fedit/test/core/models.py` & `wagtail_fedit-1.5.3rc9/wagtail_fedit/test/core/models.py`

 * *Files 3% similar despite different names*

```diff
@@ -95,14 +95,18 @@
 class BasicModel(models.Model):
     title = models.CharField(max_length=255)
     body = models.TextField()
     content: StreamValue = StreamField([
         ("heading_component", HeadingComponent()),
         ("flat_menu_component", FlatMenuComponent())
     ], use_json_field=True)
+    related_field = models.ForeignKey("self", on_delete=models.CASCADE, null=True, blank=True)
+
+    def render_as_content(self, request, context=None):
+        return f"<h1>{self.title}</h1><p>{self.body}</p>"
 
 @register_snippet
 class EditableFullModel(BaseEditableMixin, FEditableMixin):
     title = models.CharField(max_length=255)
     body = models.TextField()
     content: StreamValue = StreamField([
         ("heading_component", HeadingComponent()),
```

#### html2text {}

```diff
@@ -30,37 +30,41 @@
 """) context = self.get_context(value, parent_context=context) return
 template.render(Context(context)) class BaseEditableMixin: def get_url(self,
 request): return f"/{slugify(self.title)}/" def serve(self, request, *args,
 **kwargs): return HttpResponse(self.body) @register_snippet class BasicModel
 (models.Model): title = models.CharField(max_length=255) body =
 models.TextField() content: StreamValue = StreamField([ ("heading_component",
 HeadingComponent()), ("flat_menu_component", FlatMenuComponent()) ],
-use_json_field=True) @register_snippet class EditableFullModel
-(BaseEditableMixin, FEditableMixin): title = models.CharField(max_length=255)
-body = models.TextField() content: StreamValue = StreamField([
-("heading_component", HeadingComponent()), ("flat_menu_component",
-FlatMenuComponent()) ], use_json_field=True) @register_snippet class
-EditableDraftModel(BaseEditableMixin, DraftStateMixin, RevisionMixin,
-models.Model): title = models.CharField(max_length=255) body = models.TextField
-() content: StreamValue = StreamField([ ("heading_component", HeadingComponent
-()), ("flat_menu_component", FlatMenuComponent()) ], use_json_field=True)
-@register_snippet class EditableRevisionModel(BaseEditableMixin, RevisionMixin,
-models.Model): title = models.CharField(max_length=255) body = models.TextField
-() content: StreamValue = StreamField([ ("heading_component", HeadingComponent
-()), ("flat_menu_component", FlatMenuComponent()) ], use_json_field=True)
-@register_snippet class EditablePreviewModel(BaseEditableMixin,
-PreviewableMixin, models.Model): title = models.CharField(max_length=255) body
-= models.TextField() content: StreamValue = StreamField([ ("heading_component",
-HeadingComponent()), ("flat_menu_component", FlatMenuComponent()) ],
-use_json_field=True) @register_snippet class EditableLockModel
-(BaseEditableMixin, WorkflowMixin, DraftStateMixin, RevisionMixin,
-LockableMixin, models.Model): title = models.CharField(max_length=255) body =
+use_json_field=True) related_field = models.ForeignKey("self",
+on_delete=models.CASCADE, null=True, blank=True) def render_as_content(self,
+request, context=None): return f"
+************ {{sseellff..ttiittllee}} ************
+{self.body}
+" @register_snippet class EditableFullModel(BaseEditableMixin, FEditableMixin):
+title = models.CharField(max_length=255) body = models.TextField() content:
+StreamValue = StreamField([ ("heading_component", HeadingComponent()),
+("flat_menu_component", FlatMenuComponent()) ], use_json_field=True)
+@register_snippet class EditableDraftModel(BaseEditableMixin, DraftStateMixin,
+RevisionMixin, models.Model): title = models.CharField(max_length=255) body =
 models.TextField() content: StreamValue = StreamField([ ("heading_component",
 HeadingComponent()), ("flat_menu_component", FlatMenuComponent()) ],
-use_json_field=True) def get_permissions_policy(self): return
-ModelPermissionPolicy(self.__class__) def permissions_for_user(self, user):
-return FeditPermissionTester( self, user=user,
-policy=self.get_permissions_policy() ) class EditablePageModel(Page): body =
-models.TextField() content: StreamValue = StreamField([ ("heading_component",
-HeadingComponent()), ("flat_menu_component", FlatMenuComponent()) ],
-use_json_field=True) content_panels = Page.content_panels + [ FieldPanel
-("content") ]
+use_json_field=True) @register_snippet class EditableRevisionModel
+(BaseEditableMixin, RevisionMixin, models.Model): title = models.CharField
+(max_length=255) body = models.TextField() content: StreamValue = StreamField(
+[ ("heading_component", HeadingComponent()), ("flat_menu_component",
+FlatMenuComponent()) ], use_json_field=True) @register_snippet class
+EditablePreviewModel(BaseEditableMixin, PreviewableMixin, models.Model): title
+= models.CharField(max_length=255) body = models.TextField() content:
+StreamValue = StreamField([ ("heading_component", HeadingComponent()),
+("flat_menu_component", FlatMenuComponent()) ], use_json_field=True)
+@register_snippet class EditableLockModel(BaseEditableMixin, WorkflowMixin,
+DraftStateMixin, RevisionMixin, LockableMixin, models.Model): title =
+models.CharField(max_length=255) body = models.TextField() content: StreamValue
+= StreamField([ ("heading_component", HeadingComponent()),
+("flat_menu_component", FlatMenuComponent()) ], use_json_field=True) def
+get_permissions_policy(self): return ModelPermissionPolicy(self.__class__) def
+permissions_for_user(self, user): return FeditPermissionTester( self,
+user=user, policy=self.get_permissions_policy() ) class EditablePageModel
+(Page): body = models.TextField() content: StreamValue = StreamField([
+("heading_component", HeadingComponent()), ("flat_menu_component",
+FlatMenuComponent()) ], use_json_field=True) content_panels =
+Page.content_panels + [ FieldPanel("content") ]
```

### Comparing `wagtail_fedit-1.5.3rc8/wagtail_fedit/test/core/tests/base.py` & `wagtail_fedit-1.5.3rc9/wagtail_fedit/test/core/tests/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -184,14 +184,22 @@
             title="Lock Model",
             body="Lock Model Body",
             content=TEST_BLOCK_DATA,
             locked=True,
             locked_by=self.admin_user,
             has_unpublished_changes=True,
         )
+
+        self.basic_model.related_field = self.basic_model.__class__.objects.create(
+            title="Related Field",
+            body="Related Field Body",
+            content=TEST_BLOCK_DATA,
+        )
+
+        self.basic_model.save()
         
         self.models: list[models.Model] = [
             self.full_model,
             self.draft_model,
             self.revision_model,
             self.preview_model,
             self.basic_model,
```

### Comparing `wagtail_fedit-1.5.3rc8/wagtail_fedit/test/core/tests/test_adapters.py` & `wagtail_fedit-1.5.3rc9/wagtail_fedit/test/core/tests/test_adapters.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,14 +5,15 @@
     TemplateSyntaxError,
 )
 from wagtail_fedit.adapters import (
     BaseAdapter,
     adapter_registry,
     BlockAdapter,
     FieldAdapter,
+    ModelAdapter,
 )
 from wagtail_fedit.utils import (
     FEDIT_PREVIEW_VAR,
     find_block,
 )
 from wagtail_fedit.templatetags.fedit import (
     wrap_adapter,
@@ -53,17 +54,21 @@
 
 class TestBlockAdapter(BlockAdapter, TestAdapter):
     identifier = "test_block"
 
 class TestFieldAdapter(FieldAdapter, TestAdapter):
     identifier = "test_field"
 
+class TestModelAdapter(ModelAdapter, TestAdapter):
+    identifier = "test_model"
+
 adapter_registry.register(TestAdapter)
 adapter_registry.register(TestBlockAdapter)
 adapter_registry.register(TestFieldAdapter)
+adapter_registry.register(TestModelAdapter)
 adapter_registry.register(TestContextAdapter)
 adapter_registry.register(TestAbsoluteTokensAdapter)
 
 
 class TestBaseAdapter(BaseFEditTest):
 
     def test_required_kwargs_ok(self):
@@ -494,8 +499,128 @@
     
             tpl = template.render(Context(context))
     
             self.assertHTMLEqual(
                 tpl,
                 wrap_adapter(request, adapters[8], {})
             )
-    
+
+        def test_render_related_field(self):
+            request = self.request_factory.get(
+                self.get_editable_url(
+                    self.basic_model.pk, self.basic_model._meta.app_label, self.basic_model._meta.model_name,
+                )
+            )
+            request.user = self.admin_user
+            setattr(
+                request,
+                FEDIT_PREVIEW_VAR,
+                True,
+            )
+            template = Template(
+                "{% load fedit %}"
+                "{% fedit test_field object.related_field test=True id=8 as test %}"
+                "{{ test }}"
+            )
+
+            context = {
+                "object": self.basic_model,
+                "request": request,
+            }
+    
+            tpl = template.render(Context(context))
+    
+            self.assertHTMLEqual(
+                tpl,
+                wrap_adapter(request, adapters[8], {})
+            )
+
+class TestModelAdapter(BaseFEditTest):
+    
+        def test_render(self):
+            request = self.request_factory.get(
+                self.get_editable_url(
+                    self.basic_model.pk, self.basic_model._meta.app_label, self.basic_model._meta.model_name,
+                )
+            )
+            request.user = self.admin_user
+            setattr(
+                request,
+                FEDIT_PREVIEW_VAR,
+                True,
+            )
+            template = Template(
+                "{% load fedit %}"
+                "{% fedit test_model object test=True id=9 %}"
+            )
+    
+            context = {
+                "object": self.basic_model,
+                "request": request,
+            }
+    
+            tpl = template.render(Context(context))
+    
+            self.assertHTMLEqual(
+                tpl,
+                wrap_adapter(request, adapters[9], {})
+            )
+    
+        def test_render_as_var(self):
+            request = self.request_factory.get(
+                self.get_editable_url(
+                    self.basic_model.pk, self.basic_model._meta.app_label, self.basic_model._meta.model_name,
+                )
+            )
+            request.user = self.admin_user
+            setattr(
+                request,
+                FEDIT_PREVIEW_VAR,
+                True,
+            )
+            template = Template(
+                "{% load fedit %}"
+                "{% fedit test_model object test=True id=10 as test %}"
+                "{{ test }}"
+            )
+    
+            context = {
+                "object": self.basic_model,
+                "request": request,
+            }
+    
+            tpl = template.render(Context(context))
+    
+            self.assertHTMLEqual(
+                tpl,
+                wrap_adapter(request, adapters[10], {})
+            )
+    
+        def test_render_from_context(self):
+            request = self.request_factory.get(
+                self.get_editable_url(
+                    self.basic_model.pk, self.basic_model._meta.app_label, self.basic_model._meta.model_name,
+                )
+            )
+            request.user = self.admin_user
+            setattr(
+                request,
+                FEDIT_PREVIEW_VAR,
+                True,
+            )
+            template = Template(
+                "{% load fedit %}"
+                "{% fedit test_model from_context test=True id=11 %}"
+            )
+    
+            context = {
+                "object": self.basic_model,
+                "request": request,
+                "wagtail_fedit_instance": self.basic_model,
+            }
+    
+            tpl = template.render(Context(context))
+    
+            self.assertHTMLEqual(
+                tpl,
+                wrap_adapter(request, adapters[11], context)
+            )
```

### Comparing `wagtail_fedit-1.5.3rc8/wagtail_fedit/test/core/tests/test_block_edit.py` & `wagtail_fedit-1.5.3rc9/wagtail_fedit/test/core/tests/test_block_edit.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc8/wagtail_fedit/test/core/tests/test_blocks.py` & `wagtail_fedit-1.5.3rc9/wagtail_fedit/test/core/tests/test_blocks.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc8/wagtail_fedit/test/core/tests/test_field_edit.py` & `wagtail_fedit-1.5.3rc9/wagtail_fedit/test/core/tests/test_field_edit.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc8/wagtail_fedit/test/core/tests/test_generic.py` & `wagtail_fedit-1.5.3rc9/wagtail_fedit/test/core/tests/test_generic.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc8/wagtail_fedit/test/core/tests/test_revision.py` & `wagtail_fedit-1.5.3rc9/wagtail_fedit/test/core/tests/test_revision.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc8/wagtail_fedit/test/core/tests/test_submit.py` & `wagtail_fedit-1.5.3rc9/wagtail_fedit/test/core/tests/test_submit.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc8/wagtail_fedit/test/manage.py` & `wagtail_fedit-1.5.3rc9/wagtail_fedit/test/manage.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc8/wagtail_fedit/test/testapp/settings.py` & `wagtail_fedit-1.5.3rc9/wagtail_fedit/test/testapp/settings.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc8/wagtail_fedit/test/testapp/urls.py` & `wagtail_fedit-1.5.3rc9/wagtail_fedit/test/testapp/urls.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc8/wagtail_fedit/toolbar.py` & `wagtail_fedit-1.5.3rc9/wagtail_fedit/toolbar.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc8/wagtail_fedit/urls.py` & `wagtail_fedit-1.5.3rc9/wagtail_fedit/urls.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,14 +5,18 @@
 
 urlpatterns = [
     # Frontend Editing
     path(
         "edit/<str:adapter_id>/<str:app_label>/<str:model_name>/<str:model_id>/<str:field_name>/", 
         views.EditAdapterView.as_view(), name="edit"
     ),
+    path(
+        "edit/<str:adapter_id>/<str:app_label>/<str:model_name>/<str:model_id>/", 
+        views.EditAdapterView.as_view(), name="edit"
+    ),
 ]
 
 model_based_views = (
     ("editable", views.FEditableView),
     ("publish", views.PublishView),
     ("submit", views.SubmitView),
     ("unpublish", views.UnpublishView),
```

### Comparing `wagtail_fedit-1.5.3rc8/wagtail_fedit/utils.py` & `wagtail_fedit-1.5.3rc9/wagtail_fedit/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -468,30 +468,33 @@
         hook(items=items, adapter=adapter)
 
     items = [item.render() for item in items]
     items = list(filter(None, items))
 
     reverse_kwargs = {
         "adapter_id": adapter.identifier,
-        "field_name": adapter.field_name,
         "app_label": adapter.object._meta.app_label,
         "model_name": adapter.object._meta.model_name,
         "model_id": adapter.object.pk,
     }
 
+    if adapter.field_name is not None:
+        reverse_kwargs["field_name"] = adapter.field_name
+
     shared = adapter.encode_shared_context()
     js_constructor = adapter.get_js_constructor()
     
     return render_to_string(
         "wagtail_fedit/content/editable_adapter.html",
         {
             "identifier": adapter.identifier,
             "adapter": adapter,
             "buttons": items,
             "shared": shared,
+            "unique_id": adapter.get_element_id(),
             "js_constructor": js_constructor,
             "shared_context": adapter.kwargs,
             "parent_context": context,
             "edit_url": reverse(
                 "wagtail_fedit:edit",
                 kwargs=reverse_kwargs,
             ),
```

### Comparing `wagtail_fedit-1.5.3rc8/wagtail_fedit/views/adapters.py` & `wagtail_fedit-1.5.3rc9/wagtail_fedit/views/adapters.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,35 +21,35 @@
 from wagtail.admin.views.generic import WagtailAdminTemplateMixin
 
 from ..adapters import (
     adapter_registry,
     BaseAdapter,
     RegistryLookUpError,
 )
-from ..templatetags.fedit import (
-    wrap_adapter,
-)
 from ..utils import (
     FeditPermissionCheck,
     FeditIFrameMixin,
     FEDIT_PREVIEW_VAR,
     lock_info,
 )
+from .mixins import (
+    LocaleMixin,
+)
 
 @method_decorator(xframe_options_sameorigin, name="dispatch")
 class BaseAdapterView(FeditIFrameMixin, FeditPermissionCheck, WagtailAdminTemplateMixin, View):
     ERROR_TITLE = _("Validation Errors")
 
     def dispatch(self, 
             request:    HttpRequest,
             adapter_id: str = None,
-            field_name: str = None,
             app_label:  str = None,
             model_name: str = None,
             model_id:   Any = None,
+            field_name: str = None,
         ) -> None:
 
         # Fetch the adapter class from the registry
         try:
             self.adapter_class: BaseAdapter = adapter_registry[adapter_id]
         except RegistryLookUpError:
             return HttpResponseBadRequest("Invalid adapter ID")
@@ -66,17 +66,21 @@
         # If not; it will be automatically created by the form.
         model_instance = self.model._default_manager.get(pk=model_id)
         if isinstance(model_instance, RevisionMixin) and model_instance.latest_revision_id:
             self.instance = model_instance.latest_revision.as_object()
         else:
             self.instance = model_instance
 
-        if not hasattr(self.instance, field_name):
-            return HttpResponseBadRequest("Invalid field name for object")
+        LocaleMixin.setup_locale(self.instance)
 
+        if not field_name and self.adapter_class.field_required:
+            return HttpResponseBadRequest("Field name is required for object")
+
+        if field_name and not hasattr(self.instance, field_name) and self.adapter_class.field_required:
+            return HttpResponseBadRequest("Invalid field name for object")
 
         shared_context = request.GET.get("shared_context")
         if shared_context:
             self.shared_context = self.adapter_class.decode_shared_context(
                 request,
                 self.instance,
                 field_name,
@@ -99,15 +103,20 @@
         setattr(
             self.request,
             FEDIT_PREVIEW_VAR,
             True,
         )
 
         return super().dispatch(
-            request, adapter_id, field_name, app_label, model_name, model_id,
+            request,
+            adapter_id=adapter_id,
+            field_name=field_name,
+            app_label=app_label,
+            model_name=model_name,
+            model_id=model_id,
         )
     
     @property
     def template_name(self):
         return self.adapter.get_template_names()
     
     def render_to_response(self, context: dict[str, Any], success: bool = True, extra: dict = None, **response_kwargs: Any) -> HttpResponse:
@@ -134,21 +143,33 @@
     
     def get_context_data(self, **kwargs):
         shared_context = None
         if self.shared_context:
             shared_context =\
                 self.request.GET["shared_context"]
 
+        verbose_name = self.model._meta.verbose_name
+        if self.adapter.field_required:
+            verbose_name = self.adapter.meta_field.verbose_name
+
+        extra = {}
+        if "form" in kwargs:
+            extra.update(
+                self.adapter.get_form_context(
+                    **kwargs,
+                ),
+            )
+
         return super().get_context_data(**kwargs) | {
-            "meta_field": self.adapter.meta_field,
-            "field_name": self.adapter.field_name,
+            "verbose_name": verbose_name,
             "locked_for_user": self.locked_for_user,
             "shared_context": shared_context,
             "form_attrs": self.adapter.get_form_attrs(),
             "locked": self.lock is not None,
+            **extra,
         }
 
 class EditAdapterView(BaseAdapterView):
     def get(self, request: HttpRequest, *args: Any, **kwargs: Any) -> HttpResponse:
         # Can omit data from context - we are not rendering the content.
         form = self.adapter.get_form()
```

### Comparing `wagtail_fedit-1.5.3rc8/wagtail_fedit/views/editable.py` & `wagtail_fedit-1.5.3rc9/wagtail_fedit/views/editable.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from typing import Any
 from django.db import models
 from django.conf import settings
 from django.contrib.contenttypes.models import ContentType
 from django.utils.translation import gettext_lazy as _
-from django.views.generic import TemplateView
-from django.shortcuts import redirect
+from django.utils import translation
 from django.urls import reverse
+from django.shortcuts import redirect
+from django.views.generic import TemplateView
 from django.http import (
     HttpRequest,
     HttpResponseBadRequest,
     HttpResponseForbidden,
     HttpResponse,
 )
 from wagtail.admin import messages
@@ -43,14 +44,15 @@
     # user_can_submit_for_moderation,
     # lock_info,
 )
 
 from .mixins import (
     ObjectViewMixin,
     LockViewMixin,
+    LocaleMixin,
 )
 
 
 MAX_LOG_ENTRIES_DISPLAYED = 5
 
 
 def get_unpublish_action(object):
@@ -61,15 +63,15 @@
 
 def get_publish_action(object):
     if isinstance(object, Page):
         return PublishPageRevisionAction
     return PublishRevisionAction
 
 
-class BaseFeditView(ObjectViewMixin, FeditPermissionCheck, TemplateView):
+class BaseFeditView(LocaleMixin, ObjectViewMixin, FeditPermissionCheck, TemplateView):
     def dispatch(self, request: HttpRequest, object_id: Any, app_label: str, model_name: str) -> HttpResponse:
         if self.error_response:
             return self.error_response
 
         if not self.has_perms(request, self.object):
             return HttpResponseForbidden("You do not have permission to view this page")
```

### Comparing `wagtail_fedit-1.5.3rc8/wagtail_fedit/views/mixins.py` & `wagtail_fedit-1.5.3rc9/wagtail_fedit/views/mixins.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from typing import Any
-from django.utils.translation import gettext_lazy as _
+from django.utils import translation
 from django.apps import apps
 from django.http import (
     HttpRequest,
     HttpResponseBadRequest,
     HttpResponse,
 )
 from ..utils import (
@@ -37,7 +37,24 @@
     def setup(self, request: HttpRequest, object_id: Any, app_label: str, model_name: str) -> HttpResponse:
         super().setup(request, object_id, app_label, model_name)
 
         self.lock, self.locked_for_user = lock_info(
             self.object, request.user,
         )
 
+
+class LocaleMixin:
+    def setup(self, *args, **kwargs) -> None:
+        super().setup(*args, **kwargs)
+        self.setup_locale(self.object)
+
+    @staticmethod
+    def setup_locale(object):
+        if hasattr(object, "get_locale"):
+            locale = object.get_locale()
+        elif hasattr(object, "locale"):
+            locale = object.locale
+        else:
+            locale = None
+
+        if locale:
+            translation.activate(locale.language_code)
```

### Comparing `wagtail_fedit-1.5.3rc8/wagtail_fedit/wagtail_hooks/action_menu.py` & `wagtail_fedit-1.5.3rc9/wagtail_fedit/wagtail_hooks/action_menu.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc8/wagtail_fedit/wagtail_hooks/adapter_hooks.py` & `wagtail_fedit-1.5.3rc9/wagtail_fedit/wagtail_hooks/adapter_hooks.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc8/wagtail_fedit/wagtail_hooks/log_actions.py` & `wagtail_fedit-1.5.3rc9/wagtail_fedit/wagtail_hooks/log_actions.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc8/wagtail_fedit/wagtail_hooks/userbar.py` & `wagtail_fedit-1.5.3rc9/wagtail_fedit/wagtail_hooks/userbar.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.3rc8/wagtail_fedit.egg-info/PKG-INFO` & `wagtail_fedit-1.5.3rc9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wagtail_fedit
-Version: 1.5.3rc8
+Version: 1.5.3rc9
 Summary: Frontend editing for your Wagtail site
 Home-page: https://github.com/Nigel2392/wagtail_fedit
 Author: Nigel
 Author-email: nigel@goodadvice.it
 License: GPL-2.0-only
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
@@ -23,16 +23,14 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: Django>=4.2
-Requires-Dist: Wagtail>=5.2
 
 wagtail_fedit
 =============
 
 ![Wagtail FEdit Example](https://github.com/Nigel2392/wagtail_fedit/blob/main/.github/images/wagtail_fedit_example.png?raw=true)
 
 Wagtail FEdit is a library to allow your Wagtail pages and content-blocks to be edited on the frontend.
@@ -79,17 +77,24 @@
    ]
    ```
 2. Run `py ./manage.py collectstatic`.
 3. Run `py ./manage.py adapter_help` to see all your options and their requirements.
 
 ## Getting Editing!
 
-1. Make sure the models you wish to edit inherit from PreviewableMixin.
+1. If you want to get into the frontend-editing interface for a model it must inherit from `PreviewableMixin`.
 
    **This is a requirement.**
+
+   It is however not always required for your model to inherit from `PreviewableMixin`.
+
+   **Any model can be edited**; you just can't access the specific frontend editing interface URL for that model if it does not inherit from `PreviewableMixin`.
+
+   I.E: If a random model which does not inherit from `PreviewableMixin` appears on an editable page; **you will be able to edit it.**
+
 2. Define a template for your model.
 
    Example:
 
    ```django-html
    {% load fedit static wagtailuserbar %} {# Load the required template tag libraries #}
    <!DOCTYPE html>
@@ -339,15 +344,15 @@
     def __init__(self, object, field_name: str, request: HttpRequest, **kwargs):
         kwargs["name"] = "myColorizerJavascriptFunction"
         super().__init__(object, field_name, request, **kwargs)
 
     def render_content(self, parent_context=None):
         # This is not required; we will replace a CSS variable; thus we are not returning any actual content.
         return ""
-    
+  
     def get_response_data(self, parent_context=None):
         """
         Return the data to be sent to the frontend adapter.
         """
         data = super().get_response_data(parent_context)
         return data | {
             "color": self.field_value,
@@ -479,15 +484,24 @@
 
 Register a custom JS file to be included when the utils.FEDIT_PREVIEW_VAR is set to True.
 
 This can be used to register custom adapter JS.
 
 Example of how this hook is used in wagtail_hooks.py:
 
-    ``python     @hooks.register(REGISTER_JS)     def register_js(request):         return [             format_html(                 '<script src="{0}"></script>',                 static('js/custom.js')             ),         ]     ``
+```python
+@hooks.register(REGISTER_JS)
+def register_js(request):
+    return [
+        format_html(
+            '<script src="{0}"></script>',
+            static('js/custom.js')
+        ),
+    ]
+```
 
 ### wagtail_fedit.register_field_renderer
 
 Register a custom renderer for a field.
 
 Example of how this type of renderer is used in wagtail_hooks/renderers.py:
 
@@ -498,18 +512,19 @@
     # This is a custom renderer for RichText fields.
     # It will render the RichText field as a RichText block.
     renderer_map[RichTextField] =\
         lambda request, context, instance, value: richtext(value)
 ```
 
 ### wagtail_fedit.register_field_widgets
+
 Register a custom widget for a field.
 
 Example of how this hook is used in wagtail_hooks.py:
-    
+
 ```python
 @hooks.register(REGISTER_FIELD_WIDGETS)
 def register_field_widgets(widgets):
     widgets[RichTextField] = AdminRichTextField
     return widgets
 ```
```

#### html2text {}

```diff
@@ -1,25 +1,24 @@
-Metadata-Version: 2.1 Name: wagtail_fedit Version: 1.5.3rc8 Summary: Frontend
+Metadata-Version: 2.1 Name: wagtail_fedit Version: 1.5.3rc9 Summary: Frontend
 editing for your Wagtail site Home-page: https://github.com/Nigel2392/
 wagtail_fedit Author: Nigel Author-email: nigel@goodadvice.it License: GPL-2.0-
 only Classifier: Environment :: Web Environment Classifier: Framework :: Django
 Classifier: Framework :: Django :: 4.2 Classifier: Framework :: Wagtail
 Classifier: Framework :: Wagtail :: 5 Classifier: Framework :: Wagtail :: 6
 Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
 :: GNU General Public License v2 or later (GPLv2+) Classifier: Operating System
 :: OS Independent Classifier: Programming Language :: Python Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3 :: Only Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
 Topic :: Internet :: WWW/HTTP Classifier: Topic :: Internet :: WWW/HTTP ::
 Dynamic Content Requires-Python: >=3.8 Description-Content-Type: text/markdown
-License-File: LICENSE Requires-Dist: Django>=4.2 Requires-Dist: Wagtail>=5.2
-wagtail_fedit ============= ![Wagtail FEdit Example](https://github.com/
-Nigel2392/wagtail_fedit/blob/main/.github/images/
+License-File: LICENSE wagtail_fedit ============= ![Wagtail FEdit Example]
+(https://github.com/Nigel2392/wagtail_fedit/blob/main/.github/images/
 wagtail_fedit_example.png?raw=true) Wagtail FEdit is a library to allow your
 Wagtail pages and content-blocks to be edited on the frontend. # Table of
 Contents - [Getting Started](#getting-started) - [Getting Editing!](#getting-
 editing) - [Permissions](#permissions) - [Revisions](#revisions) - [Workflows]
 (#workflows) - [Logs](#logs) - [Caveats](#caveats) - [Adapters](#adapters) -
 [Adapters Python](#adapters-python) - [Adapters Javascript](#adapters-
 javascript) - [Hooks](#hooks) - [Construct Adapter Toolbar]
@@ -35,18 +34,23 @@
 Sessions](#wagtail_fedit_share_with_sessions) - [Use Adapter Session ID]
 (#wagtail_fedit_use_adapter_session_id) - [How your content is rendered](#how-
 your-content-is-rendered) - [Rendered output HTML](#rendered-editable-output-
 html) - [Implemented](#implemented) Getting Started --------------- 1. Add
 'wagtail_fedit' to your INSTALLED_APPS setting like this: ``` INSTALLED_APPS =
 [ ..., 'wagtail_fedit', ] ``` 2. Run `py ./manage.py collectstatic`. 3. Run `py
 ./manage.py adapter_help` to see all your options and their requirements. ##
-Getting Editing! 1. Make sure the models you wish to edit inherit from
-PreviewableMixin. **This is a requirement.** 2. Define a template for your
-model. Example: ```django-html {% load fedit static wagtailuserbar %} {# Load
-the required template tag libraries #}
+Getting Editing! 1. If you want to get into the frontend-editing interface for
+a model it must inherit from `PreviewableMixin`. **This is a requirement.** It
+is however not always required for your model to inherit from
+`PreviewableMixin`. **Any model can be edited**; you just can't access the
+specific frontend editing interface URL for that model if it does not inherit
+from `PreviewableMixin`. I.E: If a random model which does not inherit from
+`PreviewableMixin` appears on an editable page; **you will be able to edit
+it.** 2. Define a template for your model. Example: ```django-html {% load
+fedit static wagtailuserbar %} {# Load the required template tag libraries #}
 {# Load all registered CSS required for the adapters. Only included inside edit
 view! #} {% fedit_scripts "css" %}
 {# Adress the model.field or model.my.related.field you wish to edit. #} {# For
 help on arguments for the adapters please run the adapter_help command. #} {#
 Example: `python3 ./manage.py adapter_help` #}
 ************ {{%% ffeeddiitt ffiieelldd sseellff..ttiittllee iinnlliinnee %%}} ************
 {% fedit field self.content %} {% wagtailuserbar %} {# Load all registered
@@ -195,17 +199,17 @@
 ', static('css/custom.css') ), ] ``` ### wagtail_fedit.field_editor_size
 Control the size of the editor for the given model-field type. Example of how
 this hook is called: ```python for hook in hooks.get_hooks
 (FEDIT_FIELD_EDITOR_SIZE): size = hook(model_instance, model_field) if size:
 return size ``` ### wagtail_fedit.register_js Register a custom JS file to be
 included when the utils.FEDIT_PREVIEW_VAR is set to True. This can be used to
 register custom adapter JS. Example of how this hook is used in
-wagtail_hooks.py: ``python @hooks.register(REGISTER_JS) def register_js
+wagtail_hooks.py: ```python @hooks.register(REGISTER_JS) def register_js
 (request): return [ format_html( '
-', static('js/custom.js') ), ] `` ### wagtail_fedit.register_field_renderer
+', static('js/custom.js') ), ] ``` ### wagtail_fedit.register_field_renderer
 Register a custom renderer for a field. Example of how this type of renderer is
 used in wagtail_hooks/renderers.py: ```python @hooks.register
 (REGISTER_FIELD_RENDERER) def register_renderers(renderer_map): # This is a
 custom renderer for RichText fields. # It will render the RichText field as a
 RichText block. renderer_map[RichTextField] =\ lambda request, context,
 instance, value: richtext(value) ``` ### wagtail_fedit.register_field_widgets
 Register a custom widget for a field. Example of how this hook is used in
```

### Comparing `wagtail_fedit-1.5.3rc8/wagtail_fedit.egg-info/SOURCES.txt` & `wagtail_fedit-1.5.3rc9/wagtail_fedit.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 wagtail_fedit.egg-info/top_level.txt
 wagtail_fedit/adapters/__init__.py
 wagtail_fedit/adapters/base.py
 wagtail_fedit/adapters/block.py
 wagtail_fedit/adapters/field.py
 wagtail_fedit/adapters/funcs.py
 wagtail_fedit/adapters/misc.py
+wagtail_fedit/adapters/models.py
 wagtail_fedit/adapters/registry.py
 wagtail_fedit/forms/__init__.py
 wagtail_fedit/forms/blocks.py
 wagtail_fedit/forms/fields.py
 wagtail_fedit/locale/nl/LC_MESSAGES/django.mo
 wagtail_fedit/locale/nl/LC_MESSAGES/django.po
 wagtail_fedit/migrations/__init__.py
@@ -37,14 +38,16 @@
 wagtail_fedit/static/wagtail_fedit/js/frontend.js
 wagtail_fedit/templates/wagtail_fedit/_hook_output.html
 wagtail_fedit/templates/wagtail_fedit/content/editable_adapter.html
 wagtail_fedit/templates/wagtail_fedit/content/buttons/admin_link.html
 wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_adapter.html
 wagtail_fedit/templates/wagtail_fedit/editor/action_confirm.html
 wagtail_fedit/templates/wagtail_fedit/editor/action_publish_confirm.html
+wagtail_fedit/templates/wagtail_fedit/editor/adapter_edit_handler.html
+wagtail_fedit/templates/wagtail_fedit/editor/adapter_edit_handler_form.html
 wagtail_fedit/templates/wagtail_fedit/editor/adapter_form.html
 wagtail_fedit/templates/wagtail_fedit/editor/adapter_form_errors.html
 wagtail_fedit/templates/wagtail_fedit/editor/adapter_iframe.html
 wagtail_fedit/templates/wagtail_fedit/editor/base_iframe.html
 wagtail_fedit/templates/wagtail_fedit/editor/field.html
 wagtail_fedit/templates/wagtail_fedit/icons/fedit-check-list.svg
 wagtail_fedit/templates/wagtail_fedit/icons/fedit-eye-closed.svg
@@ -62,14 +65,15 @@
 wagtail_fedit/test/__init__.py
 wagtail_fedit/test/manage.py
 wagtail_fedit/test/core/__init__.py
 wagtail_fedit/test/core/apps.py
 wagtail_fedit/test/core/context_processors.py
 wagtail_fedit/test/core/models.py
 wagtail_fedit/test/core/migrations/0001_initial.py
+wagtail_fedit/test/core/migrations/0002_basicmodel_related_field.py
 wagtail_fedit/test/core/migrations/__init__.py
 wagtail_fedit/test/core/tests/__init__.py
 wagtail_fedit/test/core/tests/base.py
 wagtail_fedit/test/core/tests/test_adapters.py
 wagtail_fedit/test/core/tests/test_block_edit.py
 wagtail_fedit/test/core/tests/test_blocks.py
 wagtail_fedit/test/core/tests/test_field_edit.py
```

