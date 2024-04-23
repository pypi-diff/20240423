# Comparing `tmp/wagtail_fedit-1.5.4rc5.tar.gz` & `tmp/wagtail_fedit-1.5.4rc6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wagtail_fedit-1.5.4rc5.tar", last modified: Tue Apr 23 19:08:00 2024, max compression
+gzip compressed data, was "wagtail_fedit-1.5.4rc6.tar", last modified: Tue Apr 23 20:07:16 2024, max compression
```

## Comparing `wagtail_fedit-1.5.4rc5.tar` & `wagtail_fedit-1.5.4rc6.tar`

### file list

```diff
@@ -1,137 +1,137 @@
-drwxrwxrwx   0        0        0        0 2024-04-23 19:08:00.002390 wagtail_fedit-1.5.4rc5/
--rw-rw-rw-   0        0        0    18429 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.4rc5/LICENSE
--rw-rw-rw-   0        0        0      257 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.4rc5/MANIFEST.in
--rw-rw-rw-   0        0        0    21651 2024-04-23 19:08:00.003394 wagtail_fedit-1.5.4rc5/PKG-INFO
--rw-rw-rw-   0        0        0    20450 2024-04-23 11:23:03.000000 wagtail_fedit-1.5.4rc5/README.md
--rw-rw-rw-   0        0        0       90 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.4rc5/pyproject.toml
--rw-rw-rw-   0        0        0     1189 2024-04-23 19:08:00.016049 wagtail_fedit-1.5.4rc5/setup.cfg
--rw-rw-rw-   0        0        0       39 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.4rc5/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-23 19:07:59.758360 wagtail_fedit-1.5.4rc5/wagtail_fedit/
--rw-rw-rw-   0        0        0        0 2024-03-29 20:13:25.000000 wagtail_fedit-1.5.4rc5/wagtail_fedit/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-23 19:07:59.845970 wagtail_fedit-1.5.4rc5/wagtail_fedit/adapters/
--rw-rw-rw-   0        0        0      532 2024-04-22 21:01:35.000000 wagtail_fedit-1.5.4rc5/wagtail_fedit/adapters/__init__.py
--rw-rw-rw-   0        0        0    14330 2024-04-23 15:34:38.000000 wagtail_fedit-1.5.4rc5/wagtail_fedit/adapters/base.py
--rw-rw-rw-   0        0        0     6570 2024-04-23 19:07:14.000000 wagtail_fedit-1.5.4rc5/wagtail_fedit/adapters/block.py
--rw-rw-rw-   0        0        0     8652 2024-04-23 18:12:26.000000 wagtail_fedit-1.5.4rc5/wagtail_fedit/adapters/field.py
--rw-rw-rw-   0        0        0     2671 2024-04-22 20:52:19.000000 wagtail_fedit-1.5.4rc5/wagtail_fedit/adapters/funcs.py
--rw-rw-rw-   0        0        0     2739 2024-04-23 14:30:53.000000 wagtail_fedit-1.5.4rc5/wagtail_fedit/adapters/misc.py
--rw-rw-rw-   0        0        0     4632 2024-04-23 15:46:14.000000 wagtail_fedit-1.5.4rc5/wagtail_fedit/adapters/models.py
--rw-rw-rw-   0        0        0     1595 2024-04-18 20:22:37.000000 wagtail_fedit-1.5.4rc5/wagtail_fedit/adapters/registry.py
--rw-rw-rw-   0        0        0      163 2024-03-29 20:13:25.000000 wagtail_fedit-1.5.4rc5/wagtail_fedit/apps.py
-drwxrwxrwx   0        0        0        0 2024-04-23 19:07:59.857925 wagtail_fedit-1.5.4rc5/wagtail_fedit/forms/
--rw-rw-rw-   0        0        0      215 2024-04-23 13:02:23.000000 wagtail_fedit-1.5.4rc5/wagtail_fedit/forms/__init__.py
--rw-rw-rw-   0        0        0     2881 2024-04-18 20:27:35.000000 wagtail_fedit-1.5.4rc5/wagtail_fedit/forms/blocks.py
--rw-rw-rw-   0        0        0     3269 2024-04-23 13:28:56.000000 wagtail_fedit-1.5.4rc5/wagtail_fedit/forms/fields.py
--rw-rw-rw-   0        0        0     4617 2024-04-21 02:08:33.000000 wagtail_fedit-1.5.4rc5/wagtail_fedit/hooks.py
-drwxrwxrwx   0        0        0        0 2024-04-23 19:07:59.714242 wagtail_fedit-1.5.4rc5/wagtail_fedit/locale/
-drwxrwxrwx   0        0        0        0 2024-04-23 19:07:59.715243 wagtail_fedit-1.5.4rc5/wagtail_fedit/locale/nl/
-drwxrwxrwx   0        0        0        0 2024-04-23 19:07:59.867608 wagtail_fedit-1.5.4rc5/wagtail_fedit/locale/nl/LC_MESSAGES/
--rw-rw-rw-   0        0        0     7262 2024-04-23 15:50:58.000000 wagtail_fedit-1.5.4rc5/wagtail_fedit/locale/nl/LC_MESSAGES/django.mo
--rw-rw-rw-   0        0        0    13018 2024-04-23 15:50:49.000000 wagtail_fedit-1.5.4rc5/wagtail_fedit/locale/nl/LC_MESSAGES/django.po
-drwxrwxrwx   0        0        0        0 2024-04-23 19:07:59.869277 wagtail_fedit-1.5.4rc5/wagtail_fedit/migrations/
--rw-rw-rw-   0        0        0        0 2024-03-29 20:13:25.000000 wagtail_fedit-1.5.4rc5/wagtail_fedit/migrations/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-23 19:07:59.871406 wagtail_fedit-1.5.4rc5/wagtail_fedit/migrations/__pycache__/
--rw-rw-rw-   0        0        0      215 2024-03-29 21:05:00.000000 wagtail_fedit-1.5.4rc5/wagtail_fedit/migrations/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0        0        0     3170 2024-04-05 20:30:10.000000 wagtail_fedit-1.5.4rc5/wagtail_fedit/models.py
--rw-rw-rw-   0        0        0     1585 2024-04-23 15:56:07.000000 wagtail_fedit-1.5.4rc5/wagtail_fedit/settings.py
-drwxrwxrwx   0        0        0        0 2024-04-23 19:07:59.717463 wagtail_fedit-1.5.4rc5/wagtail_fedit/static/
-drwxrwxrwx   0        0        0        0 2024-04-23 19:07:59.718465 wagtail_fedit-1.5.4rc5/wagtail_fedit/static/wagtail_fedit/
-drwxrwxrwx   0        0        0        0 2024-04-23 19:07:59.889175 wagtail_fedit-1.5.4rc5/wagtail_fedit/static/wagtail_fedit/css/
--rw-rw-rw-   0        0        0     5791 2024-04-23 18:28:37.000000 wagtail_fedit-1.5.4rc5/wagtail_fedit/static/wagtail_fedit/css/frontend.css
--rw-rw-rw-   0        0        0     5098 2024-04-17 20:40:49.000000 wagtail_fedit-1.5.4rc5/wagtail_fedit/static/wagtail_fedit/css/furniture.css
--rw-rw-rw-   0        0        0     1266 2024-04-05 19:37:44.000000 wagtail_fedit-1.5.4rc5/wagtail_fedit/static/wagtail_fedit/css/userbar-menu.css
-drwxrwxrwx   0        0        0        0 2024-04-23 19:07:59.891184 wagtail_fedit-1.5.4rc5/wagtail_fedit/static/wagtail_fedit/js/
--rw-rw-rw-   0        0        0    22454 2024-04-23 18:08:58.000000 wagtail_fedit-1.5.4rc5/wagtail_fedit/static/wagtail_fedit/js/frontend.js
-drwxrwxrwx   0        0        0        0 2024-04-23 19:07:59.719464 wagtail_fedit-1.5.4rc5/wagtail_fedit/static/wagtail_fedit/vendor/
-drwxrwxrwx   0        0        0        0 2024-04-23 19:07:59.898632 wagtail_fedit-1.5.4rc5/wagtail_fedit/static/wagtail_fedit/vendor/tippy/
--rw-rw-rw-   0        0        0     1091 2024-04-23 15:39:19.000000 wagtail_fedit-1.5.4rc5/wagtail_fedit/static/wagtail_fedit/vendor/tippy/LICENSE
--rw-rw-rw-   0        0        0    20122 2024-04-23 14:51:23.000000 wagtail_fedit-1.5.4rc5/wagtail_fedit/static/wagtail_fedit/vendor/tippy/popper.min.js
--rw-rw-rw-   0        0        0    25717 2024-04-23 14:51:31.000000 wagtail_fedit-1.5.4rc5/wagtail_fedit/static/wagtail_fedit/vendor/tippy/tippy-bundle.min.js
-drwxrwxrwx   0        0        0        0 2024-04-23 19:07:59.720464 wagtail_fedit-1.5.4rc5/wagtail_fedit/templates/
-drwxrwxrwx   0        0        0        0 2024-04-23 19:07:59.900637 wagtail_fedit-1.5.4rc5/wagtail_fedit/templates/wagtail_fedit/
--rw-rw-rw-   0        0        0       56 2024-04-16 18:37:39.000000 wagtail_fedit-1.5.4rc5/wagtail_fedit/templates/wagtail_fedit/_hook_output.html
-drwxrwxrwx   0        0        0        0 2024-04-23 19:07:59.902124 wagtail_fedit-1.5.4rc5/wagtail_fedit/templates/wagtail_fedit/content/
-drwxrwxrwx   0        0        0        0 2024-04-23 19:07:59.905996 wagtail_fedit-1.5.4rc5/wagtail_fedit/templates/wagtail_fedit/content/buttons/
--rw-rw-rw-   0        0        0      929 2024-04-23 15:23:24.000000 wagtail_fedit-1.5.4rc5/wagtail_fedit/templates/wagtail_fedit/content/buttons/admin_link.html
--rw-rw-rw-   0        0        0      991 2024-04-23 15:27:54.000000 wagtail_fedit-1.5.4rc5/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_adapter.html
--rw-rw-rw-   0        0        0      571 2024-04-23 17:34:21.000000 wagtail_fedit-1.5.4rc5/wagtail_fedit/templates/wagtail_fedit/content/editable_adapter.html
-drwxrwxrwx   0        0        0        0 2024-04-23 19:07:59.920721 wagtail_fedit-1.5.4rc5/wagtail_fedit/templates/wagtail_fedit/editor/
--rw-rw-rw-   0        0        0     2259 2024-04-11 08:02:26.000000 wagtail_fedit-1.5.4rc5/wagtail_fedit/templates/wagtail_fedit/editor/action_confirm.html
--rw-rw-rw-   0        0        0     3699 2024-04-20 21:55:10.000000 wagtail_fedit-1.5.4rc5/wagtail_fedit/templates/wagtail_fedit/editor/action_publish_confirm.html
--rw-rw-rw-   0        0        0      266 2024-04-21 21:15:09.000000 wagtail_fedit-1.5.4rc5/wagtail_fedit/templates/wagtail_fedit/editor/adapter_edit_handler.html
--rw-rw-rw-   0        0        0      265 2024-04-21 21:23:24.000000 wagtail_fedit-1.5.4rc5/wagtail_fedit/templates/wagtail_fedit/editor/adapter_edit_handler_form.html
--rw-rw-rw-   0        0        0      555 2024-04-21 21:13:45.000000 wagtail_fedit-1.5.4rc5/wagtail_fedit/templates/wagtail_fedit/editor/adapter_form.html
--rw-rw-rw-   0        0        0      455 2024-04-21 00:11:35.000000 wagtail_fedit-1.5.4rc5/wagtail_fedit/templates/wagtail_fedit/editor/adapter_form_errors.html
--rw-rw-rw-   0        0        0      330 2024-04-21 00:12:14.000000 wagtail_fedit-1.5.4rc5/wagtail_fedit/templates/wagtail_fedit/editor/adapter_iframe.html
--rw-rw-rw-   0        0        0     5271 2024-04-21 00:11:24.000000 wagtail_fedit-1.5.4rc5/wagtail_fedit/templates/wagtail_fedit/editor/base_iframe.html
--rw-rw-rw-   0        0        0      496 2024-04-02 17:46:59.000000 wagtail_fedit-1.5.4rc5/wagtail_fedit/templates/wagtail_fedit/editor/field.html
-drwxrwxrwx   0        0        0        0 2024-04-23 19:07:59.929020 wagtail_fedit-1.5.4rc5/wagtail_fedit/templates/wagtail_fedit/icons/
--rw-rw-rw-   0        0        0      797 2024-04-11 08:36:19.000000 wagtail_fedit-1.5.4rc5/wagtail_fedit/templates/wagtail_fedit/icons/fedit-check-list.svg
--rw-rw-rw-   0        0        0      584 2024-04-11 08:36:55.000000 wagtail_fedit-1.5.4rc5/wagtail_fedit/templates/wagtail_fedit/icons/fedit-eye-closed.svg
--rw-rw-rw-   0        0        0      377 2024-04-11 08:23:07.000000 wagtail_fedit-1.5.4rc5/wagtail_fedit/templates/wagtail_fedit/icons/fedit-eye-open.svg
--rw-rw-rw-   0        0        0      725 2024-04-11 09:02:58.000000 wagtail_fedit-1.5.4rc5/wagtail_fedit/templates/wagtail_fedit/icons/fedit-save.svg
--rw-rw-rw-   0        0        0     1323 2024-04-11 08:36:52.000000 wagtail_fedit-1.5.4rc5/wagtail_fedit/templates/wagtail_fedit/icons/fedit-stop-sign.svg
-drwxrwxrwx   0        0        0        0 2024-04-23 19:07:59.932019 wagtail_fedit-1.5.4rc5/wagtail_fedit/templates/wagtail_fedit/userbar/
--rw-rw-rw-   0        0        0      867 2024-04-03 17:05:21.000000 wagtail_fedit-1.5.4rc5/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit.html
--rw-rw-rw-   0        0        0      876 2024-04-03 16:59:31.000000 wagtail_fedit-1.5.4rc5/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_view_live.html
-drwxrwxrwx   0        0        0        0 2024-04-23 19:07:59.936023 wagtail_fedit-1.5.4rc5/wagtail_fedit/templates/wagtail_fedit/userbar/publish/
--rw-rw-rw-   0        0        0      263 2024-04-11 08:24:35.000000 wagtail_fedit-1.5.4rc5/wagtail_fedit/templates/wagtail_fedit/userbar/publish/action_button.html
--rw-rw-rw-   0        0        0      967 2024-04-11 09:03:51.000000 wagtail_fedit-1.5.4rc5/wagtail_fedit/templates/wagtail_fedit/userbar/publish/item_fedit_publishing.html
-drwxrwxrwx   0        0        0        0 2024-04-23 19:07:59.939020 wagtail_fedit-1.5.4rc5/wagtail_fedit/templatetags/
--rw-rw-rw-   0        0        0        0 2024-03-29 20:13:42.000000 wagtail_fedit-1.5.4rc5/wagtail_fedit/templatetags/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-23 19:07:59.943603 wagtail_fedit-1.5.4rc5/wagtail_fedit/templatetags/__pycache__/
--rw-rw-rw-   0        0        0      217 2024-03-29 21:05:00.000000 wagtail_fedit-1.5.4rc5/wagtail_fedit/templatetags/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0        0        0    12579 2024-04-23 17:39:17.000000 wagtail_fedit-1.5.4rc5/wagtail_fedit/templatetags/__pycache__/fedit.cpython-311.pyc
--rw-rw-rw-   0        0        0     9556 2024-04-23 17:20:47.000000 wagtail_fedit-1.5.4rc5/wagtail_fedit/templatetags/fedit.py
-drwxrwxrwx   0        0        0        0 2024-04-23 19:07:59.945650 wagtail_fedit-1.5.4rc5/wagtail_fedit/test/
--rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.4rc5/wagtail_fedit/test/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-23 19:07:59.952439 wagtail_fedit-1.5.4rc5/wagtail_fedit/test/core/
--rw-rw-rw-   0        0        0      151 2024-04-05 07:59:49.000000 wagtail_fedit-1.5.4rc5/wagtail_fedit/test/core/__init__.py
--rw-rw-rw-   0        0        0      165 2024-04-05 08:41:40.000000 wagtail_fedit-1.5.4rc5/wagtail_fedit/test/core/apps.py
--rw-rw-rw-   0        0        0      130 2024-04-15 20:12:38.000000 wagtail_fedit-1.5.4rc5/wagtail_fedit/test/core/context_processors.py
-drwxrwxrwx   0        0        0        0 2024-04-23 19:07:59.958436 wagtail_fedit-1.5.4rc5/wagtail_fedit/test/core/migrations/
--rw-rw-rw-   0        0        0    12115 2024-04-20 22:33:35.000000 wagtail_fedit-1.5.4rc5/wagtail_fedit/test/core/migrations/0001_initial.py
--rw-rw-rw-   0        0        0      509 2024-04-21 18:41:55.000000 wagtail_fedit-1.5.4rc5/wagtail_fedit/test/core/migrations/0002_basicmodel_related_field.py
--rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.4rc5/wagtail_fedit/test/core/migrations/__init__.py
--rw-rw-rw-   0        0        0     6047 2024-04-23 13:09:46.000000 wagtail_fedit-1.5.4rc5/wagtail_fedit/test/core/models.py
-drwxrwxrwx   0        0        0        0 2024-04-23 19:07:59.976200 wagtail_fedit-1.5.4rc5/wagtail_fedit/test/core/tests/
--rw-rw-rw-   0        0        0        0 2024-04-05 07:59:29.000000 wagtail_fedit-1.5.4rc5/wagtail_fedit/test/core/tests/__init__.py
--rw-rw-rw-   0        0        0     8475 2024-04-23 13:35:29.000000 wagtail_fedit-1.5.4rc5/wagtail_fedit/test/core/tests/base.py
--rw-rw-rw-   0        0        0    22637 2024-04-23 12:36:52.000000 wagtail_fedit-1.5.4rc5/wagtail_fedit/test/core/tests/test_adapters.py
--rw-rw-rw-   0        0        0     4320 2024-04-06 22:44:26.000000 wagtail_fedit-1.5.4rc5/wagtail_fedit/test/core/tests/test_block_edit.py
--rw-rw-rw-   0        0        0     5664 2024-04-05 10:31:29.000000 wagtail_fedit-1.5.4rc5/wagtail_fedit/test/core/tests/test_blocks.py
--rw-rw-rw-   0        0        0     3642 2024-04-05 18:00:23.000000 wagtail_fedit-1.5.4rc5/wagtail_fedit/test/core/tests/test_field_edit.py
--rw-rw-rw-   0        0        0     3709 2024-04-10 13:03:30.000000 wagtail_fedit-1.5.4rc5/wagtail_fedit/test/core/tests/test_generic.py
--rw-rw-rw-   0        0        0     4865 2024-04-23 14:23:09.000000 wagtail_fedit-1.5.4rc5/wagtail_fedit/test/core/tests/test_model_edit.py
--rw-rw-rw-   0        0        0     1574 2024-04-20 20:49:12.000000 wagtail_fedit-1.5.4rc5/wagtail_fedit/test/core/tests/test_revision.py
--rw-rw-rw-   0        0        0     9545 2024-04-20 21:54:40.000000 wagtail_fedit-1.5.4rc5/wagtail_fedit/test/core/tests/test_submit.py
--rw-rw-rw-   0        0        0      704 2024-04-05 17:55:36.000000 wagtail_fedit-1.5.4rc5/wagtail_fedit/test/manage.py
-drwxrwxrwx   0        0        0        0 2024-04-23 19:07:59.982531 wagtail_fedit-1.5.4rc5/wagtail_fedit/test/testapp/
--rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.4rc5/wagtail_fedit/test/testapp/__init__.py
--rw-rw-rw-   0        0        0      407 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.4rc5/wagtail_fedit/test/testapp/asgi.py
--rw-rw-rw-   0        0        0     3625 2024-04-15 20:14:41.000000 wagtail_fedit-1.5.4rc5/wagtail_fedit/test/testapp/settings.py
--rw-rw-rw-   0        0        0      897 2024-04-05 08:04:53.000000 wagtail_fedit-1.5.4rc5/wagtail_fedit/test/testapp/urls.py
--rw-rw-rw-   0        0        0      407 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.4rc5/wagtail_fedit/test/testapp/wsgi.py
--rw-rw-rw-   0        0        0     2220 2024-04-23 14:21:34.000000 wagtail_fedit-1.5.4rc5/wagtail_fedit/toolbar.py
--rw-rw-rw-   0        0        0     1196 2024-04-23 17:25:08.000000 wagtail_fedit-1.5.4rc5/wagtail_fedit/urls.py
--rw-rw-rw-   0        0        0    17246 2024-04-23 17:23:14.000000 wagtail_fedit-1.5.4rc5/wagtail_fedit/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-23 19:07:59.989531 wagtail_fedit-1.5.4rc5/wagtail_fedit/views/
--rw-rw-rw-   0        0        0      215 2024-04-23 17:24:50.000000 wagtail_fedit-1.5.4rc5/wagtail_fedit/views/__init__.py
--rw-rw-rw-   0        0        0     7877 2024-04-23 17:24:01.000000 wagtail_fedit-1.5.4rc5/wagtail_fedit/views/adapters.py
--rw-rw-rw-   0        0        0    17563 2024-04-21 20:25:17.000000 wagtail_fedit-1.5.4rc5/wagtail_fedit/views/editable.py
--rw-rw-rw-   0        0        0     1923 2024-04-21 20:29:01.000000 wagtail_fedit-1.5.4rc5/wagtail_fedit/views/mixins.py
-drwxrwxrwx   0        0        0        0 2024-04-23 19:08:00.001389 wagtail_fedit-1.5.4rc5/wagtail_fedit/wagtail_hooks/
--rw-rw-rw-   0        0        0      184 2024-04-16 10:03:02.000000 wagtail_fedit-1.5.4rc5/wagtail_fedit/wagtail_hooks/__init__.py
--rw-rw-rw-   0        0        0     1748 2024-04-06 18:37:13.000000 wagtail_fedit-1.5.4rc5/wagtail_fedit/wagtail_hooks/action_menu.py
--rw-rw-rw-   0        0        0     2857 2024-04-23 15:56:51.000000 wagtail_fedit-1.5.4rc5/wagtail_fedit/wagtail_hooks/adapter_hooks.py
--rw-rw-rw-   0        0        0      328 2024-04-21 16:44:33.000000 wagtail_fedit-1.5.4rc5/wagtail_fedit/wagtail_hooks/adapter_registry.py
--rw-rw-rw-   0        0        0      398 2024-04-11 09:03:10.000000 wagtail_fedit-1.5.4rc5/wagtail_fedit/wagtail_hooks/icons.py
--rw-rw-rw-   0        0        0     2573 2024-04-11 07:39:50.000000 wagtail_fedit-1.5.4rc5/wagtail_fedit/wagtail_hooks/log_actions.py
--rw-rw-rw-   0        0        0      340 2024-03-30 17:10:05.000000 wagtail_fedit-1.5.4rc5/wagtail_fedit/wagtail_hooks/urls.py
--rw-rw-rw-   0        0        0     7630 2024-04-19 20:11:56.000000 wagtail_fedit-1.5.4rc5/wagtail_fedit/wagtail_hooks/userbar.py
-drwxrwxrwx   0        0        0        0 2024-04-23 19:07:59.806050 wagtail_fedit-1.5.4rc5/wagtail_fedit.egg-info/
--rw-rw-rw-   0        0        0    21651 2024-04-23 19:07:59.000000 wagtail_fedit-1.5.4rc5/wagtail_fedit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     4521 2024-04-23 19:07:59.000000 wagtail_fedit-1.5.4rc5/wagtail_fedit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-23 19:07:59.000000 wagtail_fedit-1.5.4rc5/wagtail_fedit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2024-04-23 19:07:59.000000 wagtail_fedit-1.5.4rc5/wagtail_fedit.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-04-23 19:07:59.000000 wagtail_fedit-1.5.4rc5/wagtail_fedit.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-23 20:07:16.981384 wagtail_fedit-1.5.4rc6/
+-rw-rw-rw-   0        0        0    18429 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.4rc6/LICENSE
+-rw-rw-rw-   0        0        0      257 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.4rc6/MANIFEST.in
+-rw-rw-rw-   0        0        0    21651 2024-04-23 20:07:16.981384 wagtail_fedit-1.5.4rc6/PKG-INFO
+-rw-rw-rw-   0        0        0    20450 2024-04-23 11:23:03.000000 wagtail_fedit-1.5.4rc6/README.md
+-rw-rw-rw-   0        0        0       90 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.4rc6/pyproject.toml
+-rw-rw-rw-   0        0        0     1189 2024-04-23 20:07:16.993927 wagtail_fedit-1.5.4rc6/setup.cfg
+-rw-rw-rw-   0        0        0       39 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.4rc6/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-23 20:07:16.313709 wagtail_fedit-1.5.4rc6/wagtail_fedit/
+-rw-rw-rw-   0        0        0        0 2024-03-29 20:13:25.000000 wagtail_fedit-1.5.4rc6/wagtail_fedit/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-23 20:07:16.405348 wagtail_fedit-1.5.4rc6/wagtail_fedit/adapters/
+-rw-rw-rw-   0        0        0      532 2024-04-22 21:01:35.000000 wagtail_fedit-1.5.4rc6/wagtail_fedit/adapters/__init__.py
+-rw-rw-rw-   0        0        0    14330 2024-04-23 15:34:38.000000 wagtail_fedit-1.5.4rc6/wagtail_fedit/adapters/base.py
+-rw-rw-rw-   0        0        0     6524 2024-04-23 20:05:52.000000 wagtail_fedit-1.5.4rc6/wagtail_fedit/adapters/block.py
+-rw-rw-rw-   0        0        0     8652 2024-04-23 18:12:26.000000 wagtail_fedit-1.5.4rc6/wagtail_fedit/adapters/field.py
+-rw-rw-rw-   0        0        0     2671 2024-04-22 20:52:19.000000 wagtail_fedit-1.5.4rc6/wagtail_fedit/adapters/funcs.py
+-rw-rw-rw-   0        0        0     2739 2024-04-23 14:30:53.000000 wagtail_fedit-1.5.4rc6/wagtail_fedit/adapters/misc.py
+-rw-rw-rw-   0        0        0     4632 2024-04-23 15:46:14.000000 wagtail_fedit-1.5.4rc6/wagtail_fedit/adapters/models.py
+-rw-rw-rw-   0        0        0     1595 2024-04-18 20:22:37.000000 wagtail_fedit-1.5.4rc6/wagtail_fedit/adapters/registry.py
+-rw-rw-rw-   0        0        0      163 2024-03-29 20:13:25.000000 wagtail_fedit-1.5.4rc6/wagtail_fedit/apps.py
+drwxrwxrwx   0        0        0        0 2024-04-23 20:07:16.422816 wagtail_fedit-1.5.4rc6/wagtail_fedit/forms/
+-rw-rw-rw-   0        0        0      215 2024-04-23 13:02:23.000000 wagtail_fedit-1.5.4rc6/wagtail_fedit/forms/__init__.py
+-rw-rw-rw-   0        0        0     2881 2024-04-18 20:27:35.000000 wagtail_fedit-1.5.4rc6/wagtail_fedit/forms/blocks.py
+-rw-rw-rw-   0        0        0     3269 2024-04-23 13:28:56.000000 wagtail_fedit-1.5.4rc6/wagtail_fedit/forms/fields.py
+-rw-rw-rw-   0        0        0     4617 2024-04-21 02:08:33.000000 wagtail_fedit-1.5.4rc6/wagtail_fedit/hooks.py
+drwxrwxrwx   0        0        0        0 2024-04-23 20:07:16.206837 wagtail_fedit-1.5.4rc6/wagtail_fedit/locale/
+drwxrwxrwx   0        0        0        0 2024-04-23 20:07:16.206837 wagtail_fedit-1.5.4rc6/wagtail_fedit/locale/nl/
+drwxrwxrwx   0        0        0        0 2024-04-23 20:07:16.444842 wagtail_fedit-1.5.4rc6/wagtail_fedit/locale/nl/LC_MESSAGES/
+-rw-rw-rw-   0        0        0     7262 2024-04-23 15:50:58.000000 wagtail_fedit-1.5.4rc6/wagtail_fedit/locale/nl/LC_MESSAGES/django.mo
+-rw-rw-rw-   0        0        0    13018 2024-04-23 15:50:49.000000 wagtail_fedit-1.5.4rc6/wagtail_fedit/locale/nl/LC_MESSAGES/django.po
+drwxrwxrwx   0        0        0        0 2024-04-23 20:07:16.445824 wagtail_fedit-1.5.4rc6/wagtail_fedit/migrations/
+-rw-rw-rw-   0        0        0        0 2024-03-29 20:13:25.000000 wagtail_fedit-1.5.4rc6/wagtail_fedit/migrations/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-23 20:07:16.447820 wagtail_fedit-1.5.4rc6/wagtail_fedit/migrations/__pycache__/
+-rw-rw-rw-   0        0        0      215 2024-03-29 21:05:00.000000 wagtail_fedit-1.5.4rc6/wagtail_fedit/migrations/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0     3170 2024-04-05 20:30:10.000000 wagtail_fedit-1.5.4rc6/wagtail_fedit/models.py
+-rw-rw-rw-   0        0        0     1585 2024-04-23 15:56:07.000000 wagtail_fedit-1.5.4rc6/wagtail_fedit/settings.py
+drwxrwxrwx   0        0        0        0 2024-04-23 20:07:16.208836 wagtail_fedit-1.5.4rc6/wagtail_fedit/static/
+drwxrwxrwx   0        0        0        0 2024-04-23 20:07:16.209837 wagtail_fedit-1.5.4rc6/wagtail_fedit/static/wagtail_fedit/
+drwxrwxrwx   0        0        0        0 2024-04-23 20:07:16.484325 wagtail_fedit-1.5.4rc6/wagtail_fedit/static/wagtail_fedit/css/
+-rw-rw-rw-   0        0        0     5791 2024-04-23 18:28:37.000000 wagtail_fedit-1.5.4rc6/wagtail_fedit/static/wagtail_fedit/css/frontend.css
+-rw-rw-rw-   0        0        0     5098 2024-04-17 20:40:49.000000 wagtail_fedit-1.5.4rc6/wagtail_fedit/static/wagtail_fedit/css/furniture.css
+-rw-rw-rw-   0        0        0     1266 2024-04-05 19:37:44.000000 wagtail_fedit-1.5.4rc6/wagtail_fedit/static/wagtail_fedit/css/userbar-menu.css
+drwxrwxrwx   0        0        0        0 2024-04-23 20:07:16.509465 wagtail_fedit-1.5.4rc6/wagtail_fedit/static/wagtail_fedit/js/
+-rw-rw-rw-   0        0        0    22454 2024-04-23 18:08:58.000000 wagtail_fedit-1.5.4rc6/wagtail_fedit/static/wagtail_fedit/js/frontend.js
+drwxrwxrwx   0        0        0        0 2024-04-23 20:07:16.211316 wagtail_fedit-1.5.4rc6/wagtail_fedit/static/wagtail_fedit/vendor/
+drwxrwxrwx   0        0        0        0 2024-04-23 20:07:16.608776 wagtail_fedit-1.5.4rc6/wagtail_fedit/static/wagtail_fedit/vendor/tippy/
+-rw-rw-rw-   0        0        0     1091 2024-04-23 15:39:19.000000 wagtail_fedit-1.5.4rc6/wagtail_fedit/static/wagtail_fedit/vendor/tippy/LICENSE
+-rw-rw-rw-   0        0        0    20122 2024-04-23 14:51:23.000000 wagtail_fedit-1.5.4rc6/wagtail_fedit/static/wagtail_fedit/vendor/tippy/popper.min.js
+-rw-rw-rw-   0        0        0    25717 2024-04-23 14:51:31.000000 wagtail_fedit-1.5.4rc6/wagtail_fedit/static/wagtail_fedit/vendor/tippy/tippy-bundle.min.js
+drwxrwxrwx   0        0        0        0 2024-04-23 20:07:16.212314 wagtail_fedit-1.5.4rc6/wagtail_fedit/templates/
+drwxrwxrwx   0        0        0        0 2024-04-23 20:07:16.616874 wagtail_fedit-1.5.4rc6/wagtail_fedit/templates/wagtail_fedit/
+-rw-rw-rw-   0        0        0       56 2024-04-16 18:37:39.000000 wagtail_fedit-1.5.4rc6/wagtail_fedit/templates/wagtail_fedit/_hook_output.html
+drwxrwxrwx   0        0        0        0 2024-04-23 20:07:16.618876 wagtail_fedit-1.5.4rc6/wagtail_fedit/templates/wagtail_fedit/content/
+drwxrwxrwx   0        0        0        0 2024-04-23 20:07:16.628155 wagtail_fedit-1.5.4rc6/wagtail_fedit/templates/wagtail_fedit/content/buttons/
+-rw-rw-rw-   0        0        0      929 2024-04-23 15:23:24.000000 wagtail_fedit-1.5.4rc6/wagtail_fedit/templates/wagtail_fedit/content/buttons/admin_link.html
+-rw-rw-rw-   0        0        0      991 2024-04-23 15:27:54.000000 wagtail_fedit-1.5.4rc6/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_adapter.html
+-rw-rw-rw-   0        0        0      571 2024-04-23 17:34:21.000000 wagtail_fedit-1.5.4rc6/wagtail_fedit/templates/wagtail_fedit/content/editable_adapter.html
+drwxrwxrwx   0        0        0        0 2024-04-23 20:07:16.669788 wagtail_fedit-1.5.4rc6/wagtail_fedit/templates/wagtail_fedit/editor/
+-rw-rw-rw-   0        0        0     2259 2024-04-11 08:02:26.000000 wagtail_fedit-1.5.4rc6/wagtail_fedit/templates/wagtail_fedit/editor/action_confirm.html
+-rw-rw-rw-   0        0        0     3699 2024-04-20 21:55:10.000000 wagtail_fedit-1.5.4rc6/wagtail_fedit/templates/wagtail_fedit/editor/action_publish_confirm.html
+-rw-rw-rw-   0        0        0      266 2024-04-21 21:15:09.000000 wagtail_fedit-1.5.4rc6/wagtail_fedit/templates/wagtail_fedit/editor/adapter_edit_handler.html
+-rw-rw-rw-   0        0        0      265 2024-04-21 21:23:24.000000 wagtail_fedit-1.5.4rc6/wagtail_fedit/templates/wagtail_fedit/editor/adapter_edit_handler_form.html
+-rw-rw-rw-   0        0        0      555 2024-04-21 21:13:45.000000 wagtail_fedit-1.5.4rc6/wagtail_fedit/templates/wagtail_fedit/editor/adapter_form.html
+-rw-rw-rw-   0        0        0      455 2024-04-21 00:11:35.000000 wagtail_fedit-1.5.4rc6/wagtail_fedit/templates/wagtail_fedit/editor/adapter_form_errors.html
+-rw-rw-rw-   0        0        0      330 2024-04-21 00:12:14.000000 wagtail_fedit-1.5.4rc6/wagtail_fedit/templates/wagtail_fedit/editor/adapter_iframe.html
+-rw-rw-rw-   0        0        0     5271 2024-04-21 00:11:24.000000 wagtail_fedit-1.5.4rc6/wagtail_fedit/templates/wagtail_fedit/editor/base_iframe.html
+-rw-rw-rw-   0        0        0      496 2024-04-02 17:46:59.000000 wagtail_fedit-1.5.4rc6/wagtail_fedit/templates/wagtail_fedit/editor/field.html
+drwxrwxrwx   0        0        0        0 2024-04-23 20:07:16.676103 wagtail_fedit-1.5.4rc6/wagtail_fedit/templates/wagtail_fedit/icons/
+-rw-rw-rw-   0        0        0      797 2024-04-11 08:36:19.000000 wagtail_fedit-1.5.4rc6/wagtail_fedit/templates/wagtail_fedit/icons/fedit-check-list.svg
+-rw-rw-rw-   0        0        0      584 2024-04-11 08:36:55.000000 wagtail_fedit-1.5.4rc6/wagtail_fedit/templates/wagtail_fedit/icons/fedit-eye-closed.svg
+-rw-rw-rw-   0        0        0      377 2024-04-11 08:23:07.000000 wagtail_fedit-1.5.4rc6/wagtail_fedit/templates/wagtail_fedit/icons/fedit-eye-open.svg
+-rw-rw-rw-   0        0        0      725 2024-04-11 09:02:58.000000 wagtail_fedit-1.5.4rc6/wagtail_fedit/templates/wagtail_fedit/icons/fedit-save.svg
+-rw-rw-rw-   0        0        0     1323 2024-04-11 08:36:52.000000 wagtail_fedit-1.5.4rc6/wagtail_fedit/templates/wagtail_fedit/icons/fedit-stop-sign.svg
+drwxrwxrwx   0        0        0        0 2024-04-23 20:07:16.694169 wagtail_fedit-1.5.4rc6/wagtail_fedit/templates/wagtail_fedit/userbar/
+-rw-rw-rw-   0        0        0      867 2024-04-03 17:05:21.000000 wagtail_fedit-1.5.4rc6/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit.html
+-rw-rw-rw-   0        0        0      876 2024-04-03 16:59:31.000000 wagtail_fedit-1.5.4rc6/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_view_live.html
+drwxrwxrwx   0        0        0        0 2024-04-23 20:07:16.712787 wagtail_fedit-1.5.4rc6/wagtail_fedit/templates/wagtail_fedit/userbar/publish/
+-rw-rw-rw-   0        0        0      263 2024-04-11 08:24:35.000000 wagtail_fedit-1.5.4rc6/wagtail_fedit/templates/wagtail_fedit/userbar/publish/action_button.html
+-rw-rw-rw-   0        0        0      967 2024-04-11 09:03:51.000000 wagtail_fedit-1.5.4rc6/wagtail_fedit/templates/wagtail_fedit/userbar/publish/item_fedit_publishing.html
+drwxrwxrwx   0        0        0        0 2024-04-23 20:07:16.715786 wagtail_fedit-1.5.4rc6/wagtail_fedit/templatetags/
+-rw-rw-rw-   0        0        0        0 2024-03-29 20:13:42.000000 wagtail_fedit-1.5.4rc6/wagtail_fedit/templatetags/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-23 20:07:16.719787 wagtail_fedit-1.5.4rc6/wagtail_fedit/templatetags/__pycache__/
+-rw-rw-rw-   0        0        0      217 2024-03-29 21:05:00.000000 wagtail_fedit-1.5.4rc6/wagtail_fedit/templatetags/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0    12928 2024-04-23 20:05:43.000000 wagtail_fedit-1.5.4rc6/wagtail_fedit/templatetags/__pycache__/fedit.cpython-311.pyc
+-rw-rw-rw-   0        0        0     9810 2024-04-23 20:05:23.000000 wagtail_fedit-1.5.4rc6/wagtail_fedit/templatetags/fedit.py
+drwxrwxrwx   0        0        0        0 2024-04-23 20:07:16.722319 wagtail_fedit-1.5.4rc6/wagtail_fedit/test/
+-rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.4rc6/wagtail_fedit/test/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-23 20:07:16.770749 wagtail_fedit-1.5.4rc6/wagtail_fedit/test/core/
+-rw-rw-rw-   0        0        0      151 2024-04-05 07:59:49.000000 wagtail_fedit-1.5.4rc6/wagtail_fedit/test/core/__init__.py
+-rw-rw-rw-   0        0        0      165 2024-04-05 08:41:40.000000 wagtail_fedit-1.5.4rc6/wagtail_fedit/test/core/apps.py
+-rw-rw-rw-   0        0        0      130 2024-04-15 20:12:38.000000 wagtail_fedit-1.5.4rc6/wagtail_fedit/test/core/context_processors.py
+drwxrwxrwx   0        0        0        0 2024-04-23 20:07:16.797824 wagtail_fedit-1.5.4rc6/wagtail_fedit/test/core/migrations/
+-rw-rw-rw-   0        0        0    12115 2024-04-20 22:33:35.000000 wagtail_fedit-1.5.4rc6/wagtail_fedit/test/core/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0      509 2024-04-21 18:41:55.000000 wagtail_fedit-1.5.4rc6/wagtail_fedit/test/core/migrations/0002_basicmodel_related_field.py
+-rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.4rc6/wagtail_fedit/test/core/migrations/__init__.py
+-rw-rw-rw-   0        0        0     6047 2024-04-23 13:09:46.000000 wagtail_fedit-1.5.4rc6/wagtail_fedit/test/core/models.py
+drwxrwxrwx   0        0        0        0 2024-04-23 20:07:16.896520 wagtail_fedit-1.5.4rc6/wagtail_fedit/test/core/tests/
+-rw-rw-rw-   0        0        0        0 2024-04-05 07:59:29.000000 wagtail_fedit-1.5.4rc6/wagtail_fedit/test/core/tests/__init__.py
+-rw-rw-rw-   0        0        0     8475 2024-04-23 13:35:29.000000 wagtail_fedit-1.5.4rc6/wagtail_fedit/test/core/tests/base.py
+-rw-rw-rw-   0        0        0    22637 2024-04-23 12:36:52.000000 wagtail_fedit-1.5.4rc6/wagtail_fedit/test/core/tests/test_adapters.py
+-rw-rw-rw-   0        0        0     4320 2024-04-06 22:44:26.000000 wagtail_fedit-1.5.4rc6/wagtail_fedit/test/core/tests/test_block_edit.py
+-rw-rw-rw-   0        0        0     5664 2024-04-05 10:31:29.000000 wagtail_fedit-1.5.4rc6/wagtail_fedit/test/core/tests/test_blocks.py
+-rw-rw-rw-   0        0        0     3642 2024-04-05 18:00:23.000000 wagtail_fedit-1.5.4rc6/wagtail_fedit/test/core/tests/test_field_edit.py
+-rw-rw-rw-   0        0        0     3709 2024-04-10 13:03:30.000000 wagtail_fedit-1.5.4rc6/wagtail_fedit/test/core/tests/test_generic.py
+-rw-rw-rw-   0        0        0     4865 2024-04-23 14:23:09.000000 wagtail_fedit-1.5.4rc6/wagtail_fedit/test/core/tests/test_model_edit.py
+-rw-rw-rw-   0        0        0     1574 2024-04-20 20:49:12.000000 wagtail_fedit-1.5.4rc6/wagtail_fedit/test/core/tests/test_revision.py
+-rw-rw-rw-   0        0        0     9545 2024-04-20 21:54:40.000000 wagtail_fedit-1.5.4rc6/wagtail_fedit/test/core/tests/test_submit.py
+-rw-rw-rw-   0        0        0      704 2024-04-05 17:55:36.000000 wagtail_fedit-1.5.4rc6/wagtail_fedit/test/manage.py
+drwxrwxrwx   0        0        0        0 2024-04-23 20:07:16.943858 wagtail_fedit-1.5.4rc6/wagtail_fedit/test/testapp/
+-rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.4rc6/wagtail_fedit/test/testapp/__init__.py
+-rw-rw-rw-   0        0        0      407 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.4rc6/wagtail_fedit/test/testapp/asgi.py
+-rw-rw-rw-   0        0        0     3625 2024-04-15 20:14:41.000000 wagtail_fedit-1.5.4rc6/wagtail_fedit/test/testapp/settings.py
+-rw-rw-rw-   0        0        0      897 2024-04-05 08:04:53.000000 wagtail_fedit-1.5.4rc6/wagtail_fedit/test/testapp/urls.py
+-rw-rw-rw-   0        0        0      407 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.4rc6/wagtail_fedit/test/testapp/wsgi.py
+-rw-rw-rw-   0        0        0     2220 2024-04-23 14:21:34.000000 wagtail_fedit-1.5.4rc6/wagtail_fedit/toolbar.py
+-rw-rw-rw-   0        0        0     1196 2024-04-23 17:25:08.000000 wagtail_fedit-1.5.4rc6/wagtail_fedit/urls.py
+-rw-rw-rw-   0        0        0    17246 2024-04-23 17:23:14.000000 wagtail_fedit-1.5.4rc6/wagtail_fedit/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-23 20:07:16.968338 wagtail_fedit-1.5.4rc6/wagtail_fedit/views/
+-rw-rw-rw-   0        0        0      215 2024-04-23 17:24:50.000000 wagtail_fedit-1.5.4rc6/wagtail_fedit/views/__init__.py
+-rw-rw-rw-   0        0        0     7388 2024-04-23 20:03:50.000000 wagtail_fedit-1.5.4rc6/wagtail_fedit/views/adapters.py
+-rw-rw-rw-   0        0        0    17563 2024-04-21 20:25:17.000000 wagtail_fedit-1.5.4rc6/wagtail_fedit/views/editable.py
+-rw-rw-rw-   0        0        0     1923 2024-04-21 20:29:01.000000 wagtail_fedit-1.5.4rc6/wagtail_fedit/views/mixins.py
+drwxrwxrwx   0        0        0        0 2024-04-23 20:07:16.979858 wagtail_fedit-1.5.4rc6/wagtail_fedit/wagtail_hooks/
+-rw-rw-rw-   0        0        0      184 2024-04-16 10:03:02.000000 wagtail_fedit-1.5.4rc6/wagtail_fedit/wagtail_hooks/__init__.py
+-rw-rw-rw-   0        0        0     1748 2024-04-06 18:37:13.000000 wagtail_fedit-1.5.4rc6/wagtail_fedit/wagtail_hooks/action_menu.py
+-rw-rw-rw-   0        0        0     2857 2024-04-23 15:56:51.000000 wagtail_fedit-1.5.4rc6/wagtail_fedit/wagtail_hooks/adapter_hooks.py
+-rw-rw-rw-   0        0        0      328 2024-04-21 16:44:33.000000 wagtail_fedit-1.5.4rc6/wagtail_fedit/wagtail_hooks/adapter_registry.py
+-rw-rw-rw-   0        0        0      398 2024-04-11 09:03:10.000000 wagtail_fedit-1.5.4rc6/wagtail_fedit/wagtail_hooks/icons.py
+-rw-rw-rw-   0        0        0     2573 2024-04-11 07:39:50.000000 wagtail_fedit-1.5.4rc6/wagtail_fedit/wagtail_hooks/log_actions.py
+-rw-rw-rw-   0        0        0      340 2024-03-30 17:10:05.000000 wagtail_fedit-1.5.4rc6/wagtail_fedit/wagtail_hooks/urls.py
+-rw-rw-rw-   0        0        0     7630 2024-04-19 20:11:56.000000 wagtail_fedit-1.5.4rc6/wagtail_fedit/wagtail_hooks/userbar.py
+drwxrwxrwx   0        0        0        0 2024-04-23 20:07:16.354778 wagtail_fedit-1.5.4rc6/wagtail_fedit.egg-info/
+-rw-rw-rw-   0        0        0    21651 2024-04-23 20:07:16.000000 wagtail_fedit-1.5.4rc6/wagtail_fedit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     4521 2024-04-23 20:07:16.000000 wagtail_fedit-1.5.4rc6/wagtail_fedit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-23 20:07:16.000000 wagtail_fedit-1.5.4rc6/wagtail_fedit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       25 2024-04-23 20:07:16.000000 wagtail_fedit-1.5.4rc6/wagtail_fedit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-04-23 20:07:16.000000 wagtail_fedit-1.5.4rc6/wagtail_fedit.egg-info/top_level.txt
```

### Comparing `wagtail_fedit-1.5.4rc5/LICENSE` & `wagtail_fedit-1.5.4rc6/LICENSE`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.4rc5/PKG-INFO` & `wagtail_fedit-1.5.4rc6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wagtail_fedit
-Version: 1.5.4rc5
+Version: 1.5.4rc6
 Summary: Frontend editing for your Wagtail site
 Home-page: https://github.com/Nigel2392/wagtail_fedit
 Author: Nigel
 Author-email: nigel@goodadvice.it
 License: GPL-2.0-only
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: wagtail_fedit Version: 1.5.4rc5 Summary: Frontend
+Metadata-Version: 2.1 Name: wagtail_fedit Version: 1.5.4rc6 Summary: Frontend
 editing for your Wagtail site Home-page: https://github.com/Nigel2392/
 wagtail_fedit Author: Nigel Author-email: nigel@goodadvice.it License: GPL-2.0-
 only Classifier: Environment :: Web Environment Classifier: Framework :: Django
 Classifier: Framework :: Django :: 4.2 Classifier: Framework :: Wagtail
 Classifier: Framework :: Wagtail :: 5 Classifier: Framework :: Wagtail :: 6
 Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
 :: GNU General Public License v2 or later (GPLv2+) Classifier: Operating System
```

### Comparing `wagtail_fedit-1.5.4rc5/README.md` & `wagtail_fedit-1.5.4rc6/README.md`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.4rc5/setup.cfg` & `wagtail_fedit-1.5.4rc6/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2077 6167 7461 696c 5f66 6564 6974   = wagtail_fedit
 00000020: 0d0a 7665 7273 696f 6e20 3d20 312e 352e  ..version = 1.5.
-00000030: 3472 6335 0d0a 6465 7363 7269 7074 696f  4rc5..descriptio
+00000030: 3472 6336 0d0a 6465 7363 7269 7074 696f  4rc6..descriptio
 00000040: 6e20 3d20 4672 6f6e 7465 6e64 2065 6469  n = Frontend edi
 00000050: 7469 6e67 2066 6f72 2079 6f75 7220 5761  ting for your Wa
 00000060: 6774 6169 6c20 7369 7465 0d0a 6c6f 6e67  gtail site..long
 00000070: 5f64 6573 6372 6970 7469 6f6e 203d 2066  _description = f
 00000080: 696c 653a 2052 4541 444d 452e 6d64 0d0a  ile: README.md..
 00000090: 6c6f 6e67 5f64 6573 6372 6970 7469 6f6e  long_description
 000000a0: 5f63 6f6e 7465 6e74 5f74 7970 6520 3d20  _content_type =
```

### Comparing `wagtail_fedit-1.5.4rc5/wagtail_fedit/adapters/__init__.py` & `wagtail_fedit-1.5.4rc6/wagtail_fedit/adapters/__init__.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.4rc5/wagtail_fedit/adapters/base.py` & `wagtail_fedit-1.5.4rc6/wagtail_fedit/adapters/base.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.4rc5/wagtail_fedit/adapters/block.py` & `wagtail_fedit-1.5.4rc6/wagtail_fedit/adapters/block.py`

 * *Files 2% similar despite different names*

```diff
@@ -179,11 +179,9 @@
         return block.render(context)
 
     def render_content(self, parent_context: dict = None) -> str:
         parent_context = parent_context or {}
         if hasattr(parent_context, "flatten"):
             parent_context = parent_context.flatten()
 
-        parent_context.update(self.kwargs)
-
         return self.block.render(parent_context)
```

### Comparing `wagtail_fedit-1.5.4rc5/wagtail_fedit/adapters/field.py` & `wagtail_fedit-1.5.4rc6/wagtail_fedit/adapters/field.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.4rc5/wagtail_fedit/adapters/funcs.py` & `wagtail_fedit-1.5.4rc6/wagtail_fedit/adapters/funcs.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.4rc5/wagtail_fedit/adapters/misc.py` & `wagtail_fedit-1.5.4rc6/wagtail_fedit/adapters/misc.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.4rc5/wagtail_fedit/adapters/models.py` & `wagtail_fedit-1.5.4rc6/wagtail_fedit/adapters/models.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.4rc5/wagtail_fedit/adapters/registry.py` & `wagtail_fedit-1.5.4rc6/wagtail_fedit/adapters/registry.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.4rc5/wagtail_fedit/forms/blocks.py` & `wagtail_fedit-1.5.4rc6/wagtail_fedit/forms/blocks.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.4rc5/wagtail_fedit/forms/fields.py` & `wagtail_fedit-1.5.4rc6/wagtail_fedit/forms/fields.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.4rc5/wagtail_fedit/hooks.py` & `wagtail_fedit-1.5.4rc6/wagtail_fedit/hooks.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.4rc5/wagtail_fedit/locale/nl/LC_MESSAGES/django.mo` & `wagtail_fedit-1.5.4rc6/wagtail_fedit/locale/nl/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.4rc5/wagtail_fedit/locale/nl/LC_MESSAGES/django.po` & `wagtail_fedit-1.5.4rc6/wagtail_fedit/locale/nl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.4rc5/wagtail_fedit/models.py` & `wagtail_fedit-1.5.4rc6/wagtail_fedit/models.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.4rc5/wagtail_fedit/settings.py` & `wagtail_fedit-1.5.4rc6/wagtail_fedit/settings.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.4rc5/wagtail_fedit/static/wagtail_fedit/css/frontend.css` & `wagtail_fedit-1.5.4rc6/wagtail_fedit/static/wagtail_fedit/css/frontend.css`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.4rc5/wagtail_fedit/static/wagtail_fedit/css/furniture.css` & `wagtail_fedit-1.5.4rc6/wagtail_fedit/static/wagtail_fedit/css/furniture.css`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.4rc5/wagtail_fedit/static/wagtail_fedit/css/userbar-menu.css` & `wagtail_fedit-1.5.4rc6/wagtail_fedit/static/wagtail_fedit/css/userbar-menu.css`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.4rc5/wagtail_fedit/static/wagtail_fedit/js/frontend.js` & `wagtail_fedit-1.5.4rc6/wagtail_fedit/static/wagtail_fedit/js/frontend.js`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.4rc5/wagtail_fedit/static/wagtail_fedit/vendor/tippy/LICENSE` & `wagtail_fedit-1.5.4rc6/wagtail_fedit/static/wagtail_fedit/vendor/tippy/LICENSE`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.4rc5/wagtail_fedit/static/wagtail_fedit/vendor/tippy/popper.min.js` & `wagtail_fedit-1.5.4rc6/wagtail_fedit/static/wagtail_fedit/vendor/tippy/popper.min.js`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.4rc5/wagtail_fedit/static/wagtail_fedit/vendor/tippy/tippy-bundle.min.js` & `wagtail_fedit-1.5.4rc6/wagtail_fedit/static/wagtail_fedit/vendor/tippy/tippy-bundle.min.js`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.4rc5/wagtail_fedit/templates/wagtail_fedit/content/buttons/admin_link.html` & `wagtail_fedit-1.5.4rc6/wagtail_fedit/templates/wagtail_fedit/content/buttons/admin_link.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.4rc5/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_adapter.html` & `wagtail_fedit-1.5.4rc6/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_adapter.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.4rc5/wagtail_fedit/templates/wagtail_fedit/content/editable_adapter.html` & `wagtail_fedit-1.5.4rc6/wagtail_fedit/templates/wagtail_fedit/content/editable_adapter.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.4rc5/wagtail_fedit/templates/wagtail_fedit/editor/action_confirm.html` & `wagtail_fedit-1.5.4rc6/wagtail_fedit/templates/wagtail_fedit/editor/action_confirm.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.4rc5/wagtail_fedit/templates/wagtail_fedit/editor/action_publish_confirm.html` & `wagtail_fedit-1.5.4rc6/wagtail_fedit/templates/wagtail_fedit/editor/action_publish_confirm.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.4rc5/wagtail_fedit/templates/wagtail_fedit/editor/adapter_form.html` & `wagtail_fedit-1.5.4rc6/wagtail_fedit/templates/wagtail_fedit/editor/adapter_form.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.4rc5/wagtail_fedit/templates/wagtail_fedit/editor/base_iframe.html` & `wagtail_fedit-1.5.4rc6/wagtail_fedit/templates/wagtail_fedit/editor/base_iframe.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.4rc5/wagtail_fedit/templates/wagtail_fedit/icons/fedit-check-list.svg` & `wagtail_fedit-1.5.4rc6/wagtail_fedit/templates/wagtail_fedit/icons/fedit-check-list.svg`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.4rc5/wagtail_fedit/templates/wagtail_fedit/icons/fedit-eye-closed.svg` & `wagtail_fedit-1.5.4rc6/wagtail_fedit/templates/wagtail_fedit/icons/fedit-eye-closed.svg`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.4rc5/wagtail_fedit/templates/wagtail_fedit/icons/fedit-save.svg` & `wagtail_fedit-1.5.4rc6/wagtail_fedit/templates/wagtail_fedit/icons/fedit-save.svg`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.4rc5/wagtail_fedit/templates/wagtail_fedit/icons/fedit-stop-sign.svg` & `wagtail_fedit-1.5.4rc6/wagtail_fedit/templates/wagtail_fedit/icons/fedit-stop-sign.svg`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.4rc5/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit.html` & `wagtail_fedit-1.5.4rc6/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.4rc5/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_view_live.html` & `wagtail_fedit-1.5.4rc6/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_view_live.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.4rc5/wagtail_fedit/templates/wagtail_fedit/userbar/publish/item_fedit_publishing.html` & `wagtail_fedit-1.5.4rc6/wagtail_fedit/templates/wagtail_fedit/userbar/publish/item_fedit_publishing.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.4rc5/wagtail_fedit/templatetags/__pycache__/fedit.cpython-311.pyc` & `wagtail_fedit-1.5.4rc6/wagtail_fedit/templatetags/__pycache__/fedit.cpython-311.pyc`

 * *Files 18% similar despite different names*

#### Python bytecode

```diff
@@ -1,40 +1,40 @@
 magic:    0xa70d0d0a
-moddate:  0xefed2766 (Tue Apr 23 17:20:47 2024 UTC)
-files sz: 9556
+moddate:  0x83142866 (Tue Apr 23 20:05:23 2024 UTC)
+files sz: 9810
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 13
    flags     : 0
    code
       0x9700640064016c006d015a016d025a020100640064026c036d045a046d
       055a056d065a060100640064036c076d085a080100640064046c096d0a5a
       0a6d0b5a0b6d0c5a0c0100640064056c0d6d0e5a0e0100640064066c0f6d
       105a100100640064076c116d125a120100640064086c136d145a14010064
-      0064096c156d165a1601006400640a6c176d185a1801006400640b6c195a
-      19640c640d6c1a6d1b5a1b6d1c5a1c6d1d5a1d6d1e5a1e0100640c640e6c
-      1f6d205a206d215a216d225a226d235a230100640c640f6c186d245a246d
-      255a250100020065046a260000000000000000a6000000ab000000000000
-      0000005a2764105a2864115a296412652a641365086414652a6415652a66
-      08641684045a2b020047006417840064186505a6030000ab030000000000
-      0000005a2c6527a02d000000000000000000000000000000000000000065
-      23ac19a6010000ab010000000000000000641a650a641b650b6604641c84
-      04a6000000ab0000000000000000005a2e6527a02f000000000000000000
-      0000000000000000000000641dac1ea6010000ab01000000000000000064
-      136508641f651d6415652a660664208404a6000000ab0000000000000000
-      005a306527a0310000000000000000000000000000000000000000642164
-      22641dac23a6030000ab03000000000000000064156532660264248404a6
-      000000ab0000000000000000005a336527a02f0000000000000000000000
-      00000000000000000064256426ac27a6020000ab02000000000000000064
-      2f6428652a6415652a660464298405a6000000ab0000000000000000005a
-      346430641a650a642a6535652a19000000000000000000642b6535652a19
-      000000000000000000642c6535652a19000000000000000000642d653265
-      2a650266021900000000000000000064156532660c642e84055a36640b53
-      00
+      0064096c156d165a1601006400640a6c176d185a1801006400640b6c196d
+      1a5a1a6d1b5a1b01006400640c6c1c5a1c640d640e6c1d6d1e5a1e6d1f5a
+      1f6d205a206d215a210100640d640f6c226d235a236d245a246d255a256d
+      265a260100640d64106c186d275a276d285a280100020065046a29000000
+      0000000000a6000000ab0000000000000000005a2a64115a2b64125a2c64
+      13652d641465086415652d6416652d6608641784045a2e02004700641884
+      0064196505a6030000ab0300000000000000005a2f652aa0300000000000
+      0000000000000000000000000000006526ac1aa6010000ab010000000000
+      000000641b650a641c650b6604641d8404a6000000ab0000000000000000
+      005a31652aa0320000000000000000000000000000000000000000641eac
+      1fa6010000ab01000000000000000064146508642065206416652d660664
+      218404a6000000ab0000000000000000005a33652aa03400000000000000
+      0000000000000000000000000064226423641eac24a6030000ab03000000
+      000000000064166535660264258404a6000000ab0000000000000000005a
+      36652aa032000000000000000000000000000000000000000064266427ac
+      28a6020000ab02000000000000000064306429652d6416652d6604642a84
+      05a6000000ab0000000000000000005a376431641b650a642b6538652d19
+      000000000000000000642c6538652d19000000000000000000642d653865
+      2d19000000000000000000642e6535652d65026602190000000000000000
+      0064166535660c642f84055a39640c5300
      0           0 RESUME                   0
    
      1           2 LOAD_CONST               0 (0)
                  4 LOAD_CONST               1 (('Type', 'Any'))
                  6 IMPORT_NAME              0 (typing)
                  8 IMPORT_FROM              1 (Type)
                 10 STORE_NAME               1 (Type)
@@ -109,215 +109,225 @@
     18         130 LOAD_CONST               0 (0)
                132 LOAD_CONST              10 (('hooks',))
                134 IMPORT_NAME             23 (wagtail)
                136 IMPORT_FROM             24 (hooks)
                138 STORE_NAME              24 (hooks)
                140 POP_TOP
    
-    20         142 LOAD_CONST               0 (0)
-               144 LOAD_CONST              11 (None)
-               146 IMPORT_NAME             25 (warnings)
-               148 STORE_NAME              25 (warnings)
-   
-    22         150 LOAD_CONST              12 (2)
-               152 LOAD_CONST              13 (('adapter_registry', 'RegistryLookUpError', 'BaseAdapter', 'AdapterError'))
-               154 IMPORT_NAME             26 (adapters)
-               156 IMPORT_FROM             27 (adapter_registry)
-               158 STORE_NAME              27 (adapter_registry)
-               160 IMPORT_FROM             28 (RegistryLookUpError)
-               162 STORE_NAME              28 (RegistryLookUpError)
-               164 IMPORT_FROM             29 (BaseAdapter)
-               166 STORE_NAME              29 (BaseAdapter)
-               168 IMPORT_FROM             30 (AdapterError)
-               170 STORE_NAME              30 (AdapterError)
-               172 POP_TOP
-   
-    28         174 LOAD_CONST              12 (2)
-               176 LOAD_CONST              14 (('wrap_adapter', '_can_edit', 'FEDIT_PREVIEW_VAR', 'TEMPLATE_TAG_NAME'))
-               178 IMPORT_NAME             31 (utils)
-               180 IMPORT_FROM             32 (wrap_adapter)
-               182 STORE_NAME              32 (wrap_adapter)
-               184 IMPORT_FROM             33 (_can_edit)
-               186 STORE_NAME              33 (_can_edit)
-               188 IMPORT_FROM             34 (FEDIT_PREVIEW_VAR)
-               190 STORE_NAME              34 (FEDIT_PREVIEW_VAR)
-               192 IMPORT_FROM             35 (TEMPLATE_TAG_NAME)
-               194 STORE_NAME              35 (TEMPLATE_TAG_NAME)
-               196 POP_TOP
-   
-    34         198 LOAD_CONST              12 (2)
-               200 LOAD_CONST              15 (('REGISTER_CSS', 'REGISTER_JS'))
-               202 IMPORT_NAME             24 (hooks)
-               204 IMPORT_FROM             36 (REGISTER_CSS)
-               206 STORE_NAME              36 (REGISTER_CSS)
-               208 IMPORT_FROM             37 (REGISTER_JS)
-               210 STORE_NAME              37 (REGISTER_JS)
+    19         142 LOAD_CONST               0 (0)
+               144 LOAD_CONST              11 (('Page', 'PAGE_TEMPLATE_VAR'))
+               146 IMPORT_NAME             25 (wagtail.models)
+               148 IMPORT_FROM             26 (Page)
+               150 STORE_NAME              26 (Page)
+               152 IMPORT_FROM             27 (PAGE_TEMPLATE_VAR)
+               154 STORE_NAME              27 (PAGE_TEMPLATE_VAR)
+               156 POP_TOP
+   
+    24         158 LOAD_CONST               0 (0)
+               160 LOAD_CONST              12 (None)
+               162 IMPORT_NAME             28 (warnings)
+               164 STORE_NAME              28 (warnings)
+   
+    26         166 LOAD_CONST              13 (2)
+               168 LOAD_CONST              14 (('adapter_registry', 'RegistryLookUpError', 'BaseAdapter', 'AdapterError'))
+               170 IMPORT_NAME             29 (adapters)
+               172 IMPORT_FROM             30 (adapter_registry)
+               174 STORE_NAME              30 (adapter_registry)
+               176 IMPORT_FROM             31 (RegistryLookUpError)
+               178 STORE_NAME              31 (RegistryLookUpError)
+               180 IMPORT_FROM             32 (BaseAdapter)
+               182 STORE_NAME              32 (BaseAdapter)
+               184 IMPORT_FROM             33 (AdapterError)
+               186 STORE_NAME              33 (AdapterError)
+               188 POP_TOP
+   
+    32         190 LOAD_CONST              13 (2)
+               192 LOAD_CONST              15 (('wrap_adapter', '_can_edit', 'FEDIT_PREVIEW_VAR', 'TEMPLATE_TAG_NAME'))
+               194 IMPORT_NAME             34 (utils)
+               196 IMPORT_FROM             35 (wrap_adapter)
+               198 STORE_NAME              35 (wrap_adapter)
+               200 IMPORT_FROM             36 (_can_edit)
+               202 STORE_NAME              36 (_can_edit)
+               204 IMPORT_FROM             37 (FEDIT_PREVIEW_VAR)
+               206 STORE_NAME              37 (FEDIT_PREVIEW_VAR)
+               208 IMPORT_FROM             38 (TEMPLATE_TAG_NAME)
+               210 STORE_NAME              38 (TEMPLATE_TAG_NAME)
                212 POP_TOP
    
-    40         214 PUSH_NULL
-               216 LOAD_NAME                4 (library)
-               218 LOAD_ATTR               38 (Library)
-               228 PRECALL                  0
-               232 CALL                     0
-               242 STORE_NAME              39 (register)
-   
-    43         244 LOAD_CONST              16 ('Field name is not available in the context for %(object)s.')
-               246 STORE_NAME              40 (WARNING_FIELD_NAME_NOT_AVAILABLE)
-   
-    44         248 LOAD_CONST              17 ('Model instance is not available in the context for %(object)s.')
-               250 STORE_NAME              41 (WARNING_MODEL_INSTANCE_NOT_AVAILABLE)
-   
-    47         252 LOAD_CONST              18 ('var')
-               254 LOAD_NAME               42 (str)
-               256 LOAD_CONST              19 ('context')
-               258 LOAD_NAME                8 (Context)
-               260 LOAD_CONST              20 ('value')
-               262 LOAD_NAME               42 (str)
-               264 LOAD_CONST              21 ('return')
-               266 LOAD_NAME               42 (str)
-               268 BUILD_TUPLE              8
-               270 LOAD_CONST              22 (<code object as_var, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 47>)
-               272 MAKE_FUNCTION            4 (annotations)
-               274 STORE_NAME              43 (as_var)
-   
-    54         276 PUSH_NULL
-               278 LOAD_BUILD_CLASS
-               280 LOAD_CONST              23 (<code object AdapterNode, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 54>)
-               282 MAKE_FUNCTION            0
-               284 LOAD_CONST              24 ('AdapterNode')
-               286 LOAD_NAME                5 (Node)
-               288 PRECALL                  3
-               292 CALL                     3
-               302 STORE_NAME              44 (AdapterNode)
-   
-   141         304 LOAD_NAME               39 (register)
-               306 LOAD_METHOD             45 (tag)
-               328 LOAD_NAME               35 (TEMPLATE_TAG_NAME)
-               330 KW_NAMES                25
-               332 PRECALL                  1
-               336 CALL                     1
-   
-   142         346 LOAD_CONST              26 ('parser')
-               348 LOAD_NAME               10 (Parser)
-               350 LOAD_CONST              27 ('token')
-               352 LOAD_NAME               11 (Token)
-               354 BUILD_TUPLE              4
-               356 LOAD_CONST              28 (<code object do_render_fedit, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 141>)
-               358 MAKE_FUNCTION            4 (annotations)
-   
-   141         360 PRECALL                  0
-               364 CALL                     0
-   
-   142         374 STORE_NAME              46 (do_render_fedit)
-   
-   199         376 LOAD_NAME               39 (register)
-               378 LOAD_METHOD             47 (simple_tag)
-               400 LOAD_CONST              29 (True)
-               402 KW_NAMES                30
-               404 PRECALL                  1
-               408 CALL                     1
-   
-   200         418 LOAD_CONST              19 ('context')
-               420 LOAD_NAME                8 (Context)
-               422 LOAD_CONST              31 ('adapter')
-               424 LOAD_NAME               29 (BaseAdapter)
-               426 LOAD_CONST              21 ('return')
-               428 LOAD_NAME               42 (str)
-               430 BUILD_TUPLE              6
-               432 LOAD_CONST              32 (<code object render_adapter, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 199>)
-               434 MAKE_FUNCTION            4 (annotations)
-   
-   199         436 PRECALL                  0
-               440 CALL                     0
-   
-   200         450 STORE_NAME              48 (render_adapter)
-   
-   218         452 LOAD_NAME               39 (register)
-               454 LOAD_METHOD             49 (inclusion_tag)
-               476 LOAD_CONST              33 ('wagtail_fedit/_hook_output.html')
-               478 LOAD_CONST              34 ('fedit_scripts')
-               480 LOAD_CONST              29 (True)
-               482 KW_NAMES                35
-               484 PRECALL                  3
-               488 CALL                     3
-   
-   219         498 LOAD_CONST              21 ('return')
-               500 LOAD_NAME               50 (dict)
-               502 BUILD_TUPLE              2
-               504 LOAD_CONST              36 (<code object static_hook_output, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 218>)
-               506 MAKE_FUNCTION            4 (annotations)
-   
-   218         508 PRECALL                  0
-               512 CALL                     0
-   
-   219         522 STORE_NAME              51 (static_hook_output)
-   
-   248         524 LOAD_NAME               39 (register)
-               526 LOAD_METHOD             47 (simple_tag)
-               548 LOAD_CONST              37 (False)
-               550 LOAD_CONST              38 ('tooltip')
-               552 KW_NAMES                39
-               554 PRECALL                  2
-               558 CALL                     2
-   
-   249         568 LOAD_CONST              47 ((None,))
-               570 LOAD_CONST              40 ('wrapping')
-               572 LOAD_NAME               42 (str)
-               574 LOAD_CONST              21 ('return')
-               576 LOAD_NAME               42 (str)
-               578 BUILD_TUPLE              4
-               580 LOAD_CONST              41 (<code object tooltip, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 248>)
-               582 MAKE_FUNCTION            5 (defaults, annotations)
-   
-   248         584 PRECALL                  0
-               588 CALL                     0
-   
-   249         598 STORE_NAME              52 (tooltip)
-   
-   264         600 LOAD_CONST              48 ((None, None, None))
-               602 LOAD_CONST              26 ('parser')
-               604 LOAD_NAME               10 (Parser)
-               606 LOAD_CONST              42 ('tokens')
-               608 LOAD_NAME               53 (list)
-               610 LOAD_NAME               42 (str)
-               612 BINARY_SUBSCR
-               622 LOAD_CONST              43 ('kwarg_list')
-               624 LOAD_NAME               53 (list)
-               626 LOAD_NAME               42 (str)
+    38         214 LOAD_CONST              13 (2)
+               216 LOAD_CONST              16 (('REGISTER_CSS', 'REGISTER_JS'))
+               218 IMPORT_NAME             24 (hooks)
+               220 IMPORT_FROM             39 (REGISTER_CSS)
+               222 STORE_NAME              39 (REGISTER_CSS)
+               224 IMPORT_FROM             40 (REGISTER_JS)
+               226 STORE_NAME              40 (REGISTER_JS)
+               228 POP_TOP
+   
+    44         230 PUSH_NULL
+               232 LOAD_NAME                4 (library)
+               234 LOAD_ATTR               41 (Library)
+               244 PRECALL                  0
+               248 CALL                     0
+               258 STORE_NAME              42 (register)
+   
+    47         260 LOAD_CONST              17 ('Field name is not available in the context for %(object)s.')
+               262 STORE_NAME              43 (WARNING_FIELD_NAME_NOT_AVAILABLE)
+   
+    48         264 LOAD_CONST              18 ('Model instance is not available in the context for %(object)s.')
+               266 STORE_NAME              44 (WARNING_MODEL_INSTANCE_NOT_AVAILABLE)
+   
+    51         268 LOAD_CONST              19 ('var')
+               270 LOAD_NAME               45 (str)
+               272 LOAD_CONST              20 ('context')
+               274 LOAD_NAME                8 (Context)
+               276 LOAD_CONST              21 ('value')
+               278 LOAD_NAME               45 (str)
+               280 LOAD_CONST              22 ('return')
+               282 LOAD_NAME               45 (str)
+               284 BUILD_TUPLE              8
+               286 LOAD_CONST              23 (<code object as_var, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Packages\wagtail_fedit\wagtail_fedit\templatetags\fedit.py", line 51>)
+               288 MAKE_FUNCTION            4 (annotations)
+               290 STORE_NAME              46 (as_var)
+   
+    58         292 PUSH_NULL
+               294 LOAD_BUILD_CLASS
+               296 LOAD_CONST              24 (<code object AdapterNode, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Packages\wagtail_fedit\wagtail_fedit\templatetags\fedit.py", line 58>)
+               298 MAKE_FUNCTION            0
+               300 LOAD_CONST              25 ('AdapterNode')
+               302 LOAD_NAME                5 (Node)
+               304 PRECALL                  3
+               308 CALL                     3
+               318 STORE_NAME              47 (AdapterNode)
+   
+   149         320 LOAD_NAME               42 (register)
+               322 LOAD_METHOD             48 (tag)
+               344 LOAD_NAME               38 (TEMPLATE_TAG_NAME)
+               346 KW_NAMES                26
+               348 PRECALL                  1
+               352 CALL                     1
+   
+   150         362 LOAD_CONST              27 ('parser')
+               364 LOAD_NAME               10 (Parser)
+               366 LOAD_CONST              28 ('token')
+               368 LOAD_NAME               11 (Token)
+               370 BUILD_TUPLE              4
+               372 LOAD_CONST              29 (<code object do_render_fedit, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Packages\wagtail_fedit\wagtail_fedit\templatetags\fedit.py", line 149>)
+               374 MAKE_FUNCTION            4 (annotations)
+   
+   149         376 PRECALL                  0
+               380 CALL                     0
+   
+   150         390 STORE_NAME              49 (do_render_fedit)
+   
+   207         392 LOAD_NAME               42 (register)
+               394 LOAD_METHOD             50 (simple_tag)
+               416 LOAD_CONST              30 (True)
+               418 KW_NAMES                31
+               420 PRECALL                  1
+               424 CALL                     1
+   
+   208         434 LOAD_CONST              20 ('context')
+               436 LOAD_NAME                8 (Context)
+               438 LOAD_CONST              32 ('adapter')
+               440 LOAD_NAME               32 (BaseAdapter)
+               442 LOAD_CONST              22 ('return')
+               444 LOAD_NAME               45 (str)
+               446 BUILD_TUPLE              6
+               448 LOAD_CONST              33 (<code object render_adapter, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Packages\wagtail_fedit\wagtail_fedit\templatetags\fedit.py", line 207>)
+               450 MAKE_FUNCTION            4 (annotations)
+   
+   207         452 PRECALL                  0
+               456 CALL                     0
+   
+   208         466 STORE_NAME              51 (render_adapter)
+   
+   229         468 LOAD_NAME               42 (register)
+               470 LOAD_METHOD             52 (inclusion_tag)
+               492 LOAD_CONST              34 ('wagtail_fedit/_hook_output.html')
+               494 LOAD_CONST              35 ('fedit_scripts')
+               496 LOAD_CONST              30 (True)
+               498 KW_NAMES                36
+               500 PRECALL                  3
+               504 CALL                     3
+   
+   230         514 LOAD_CONST              22 ('return')
+               516 LOAD_NAME               53 (dict)
+               518 BUILD_TUPLE              2
+               520 LOAD_CONST              37 (<code object static_hook_output, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Packages\wagtail_fedit\wagtail_fedit\templatetags\fedit.py", line 229>)
+               522 MAKE_FUNCTION            4 (annotations)
+   
+   229         524 PRECALL                  0
+               528 CALL                     0
+   
+   230         538 STORE_NAME              54 (static_hook_output)
+   
+   259         540 LOAD_NAME               42 (register)
+               542 LOAD_METHOD             50 (simple_tag)
+               564 LOAD_CONST              38 (False)
+               566 LOAD_CONST              39 ('tooltip')
+               568 KW_NAMES                40
+               570 PRECALL                  2
+               574 CALL                     2
+   
+   260         584 LOAD_CONST              48 ((None,))
+               586 LOAD_CONST              41 ('wrapping')
+               588 LOAD_NAME               45 (str)
+               590 LOAD_CONST              22 ('return')
+               592 LOAD_NAME               45 (str)
+               594 BUILD_TUPLE              4
+               596 LOAD_CONST              42 (<code object tooltip, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Packages\wagtail_fedit\wagtail_fedit\templatetags\fedit.py", line 259>)
+               598 MAKE_FUNCTION            5 (defaults, annotations)
+   
+   259         600 PRECALL                  0
+               604 CALL                     0
+   
+   260         614 STORE_NAME              55 (tooltip)
+   
+   275         616 LOAD_CONST              49 ((None, None, None))
+               618 LOAD_CONST              27 ('parser')
+               620 LOAD_NAME               10 (Parser)
+               622 LOAD_CONST              43 ('tokens')
+               624 LOAD_NAME               56 (list)
+               626 LOAD_NAME               45 (str)
                628 BINARY_SUBSCR
-               638 LOAD_CONST              44 ('absolute_tokens')
-               640 LOAD_NAME               53 (list)
-               642 LOAD_NAME               42 (str)
+               638 LOAD_CONST              44 ('kwarg_list')
+               640 LOAD_NAME               56 (list)
+               642 LOAD_NAME               45 (str)
                644 BINARY_SUBSCR
-               654 LOAD_CONST              45 ('optional_tokens')
-               656 LOAD_NAME               50 (dict)
-               658 LOAD_NAME               42 (str)
-               660 LOAD_NAME                2 (Any)
-               662 BUILD_TUPLE              2
-               664 BINARY_SUBSCR
-               674 LOAD_CONST              21 ('return')
-               676 LOAD_NAME               50 (dict)
-               678 BUILD_TUPLE             12
-               680 LOAD_CONST              46 (<code object get_kwargs, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 264>)
-               682 MAKE_FUNCTION            5 (defaults, annotations)
-               684 STORE_NAME              54 (get_kwargs)
-               686 LOAD_CONST              11 (None)
-               688 RETURN_VALUE
+               654 LOAD_CONST              45 ('absolute_tokens')
+               656 LOAD_NAME               56 (list)
+               658 LOAD_NAME               45 (str)
+               660 BINARY_SUBSCR
+               670 LOAD_CONST              46 ('optional_tokens')
+               672 LOAD_NAME               53 (dict)
+               674 LOAD_NAME               45 (str)
+               676 LOAD_NAME                2 (Any)
+               678 BUILD_TUPLE              2
+               680 BINARY_SUBSCR
+               690 LOAD_CONST              22 ('return')
+               692 LOAD_NAME               53 (dict)
+               694 BUILD_TUPLE             12
+               696 LOAD_CONST              47 (<code object get_kwargs, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Packages\wagtail_fedit\wagtail_fedit\templatetags\fedit.py", line 275>)
+               698 MAKE_FUNCTION            5 (defaults, annotations)
+               700 STORE_NAME              57 (get_kwargs)
+               702 LOAD_CONST              12 (None)
+               704 RETURN_VALUE
    consts
       0
       ('Type', 'Any')
       ('library', 'Node', 'TemplateSyntaxError')
       ('Context',)
       ('Parser', 'Token', 'FilterExpression')
       ('HttpRequest',)
       ('escape',)
       ('mark_safe',)
       ('reverse',)
       ('signing',)
       ('hooks',)
+      ('Page', 'PAGE_TEMPLATE_VAR')
       None
       2
       ('adapter_registry', 'RegistryLookUpError', 'BaseAdapter', 'AdapterError')
       ('wrap_adapter', '_can_edit', 'FEDIT_PREVIEW_VAR', 'TEMPLATE_TAG_NAME')
       ('REGISTER_CSS', 'REGISTER_JS')
       'Field name is not available in the context for %(object)s.'
       'Model instance is not available in the context for %(object)s.'
@@ -327,86 +337,86 @@
       'return'
       code
          argcount  : 3
          nlocals   : 3
          stacksize : 3
          flags     : 3
          code 0x97007c0073027c0253007c027c017c003c00000064015300
-          47           0 RESUME                   0
+          51           0 RESUME                   0
          
-          48           2 LOAD_FAST                0 (var)
+          52           2 LOAD_FAST                0 (var)
                        4 POP_JUMP_FORWARD_IF_TRUE     2 (to 10)
          
-          49           6 LOAD_FAST                2 (value)
+          53           6 LOAD_FAST                2 (value)
                        8 RETURN_VALUE
          
-          51     >>   10 LOAD_FAST                2 (value)
+          55     >>   10 LOAD_FAST                2 (value)
                       12 LOAD_FAST                1 (context)
                       14 LOAD_FAST                0 (var)
                       16 STORE_SUBSCR
          
-          52          20 LOAD_CONST               1 ('')
+          56          20 LOAD_CONST               1 ('')
                       22 RETURN_VALUE
          consts
             None
             ''
          names      ()
          varnames   ('var', 'context', 'value')
          freevars   ()
          cellvars   ()
-         filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\tester\\wagtail_fedit\\templatetags\\fedit.py'
+         filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Packages\\wagtail_fedit\\wagtail_fedit\\templatetags\\fedit.py'
          name       'as_var'
-         firstlineno 47
+         firstlineno 51
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
-          54           0 RESUME                   0
+          58           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('AdapterNode')
                        8 STORE_NAME               2 (__qualname__)
          
-          55          10 PUSH_NULL
+          59          10 PUSH_NULL
                       12 LOAD_NAME                3 (signing)
                       14 LOAD_ATTR                4 (TimestampSigner)
                       24 PRECALL                  0
                       28 CALL                     0
                       38 STORE_NAME               5 (signer)
          
-          57          40 LOAD_CONST               9 ((None,))
+          61          40 LOAD_CONST               9 ((None,))
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
-                      84 LOAD_CONST               6 (<code object __init__, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 57>)
+                      84 LOAD_CONST               6 (<code object __init__, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Packages\wagtail_fedit\wagtail_fedit\templatetags\fedit.py", line 61>)
                       86 MAKE_FUNCTION            5 (defaults, annotations)
                       88 STORE_NAME              11 (__init__)
          
-          64          90 LOAD_CONST               7 (<code object _resolve_expressions, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 64>)
+          68          90 LOAD_CONST               7 (<code object _resolve_expressions, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Packages\wagtail_fedit\wagtail_fedit\templatetags\fedit.py", line 68>)
                       92 MAKE_FUNCTION            0
                       94 STORE_NAME              12 (_resolve_expressions)
          
-          74          96 LOAD_CONST               8 (<code object render, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 74>)
+          78          96 LOAD_CONST               8 (<code object render, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Packages\wagtail_fedit\wagtail_fedit\templatetags\fedit.py", line 78>)
                       98 MAKE_FUNCTION            0
                      100 STORE_NAME              13 (render)
                      102 LOAD_CONST               1 (None)
                      104 RETURN_VALUE
          consts
             'AdapterNode'
             None
@@ -419,46 +429,46 @@
                nlocals   : 6
                stacksize : 2
                flags     : 11
                code
                   0x97007c017c005f0000000000000000007c027c005f0100000000000000
                   007c037c005f0200000000000000007c057c005f0300000000000000007c
                   047c005f04000000000000000064005300
-                57           0 RESUME                   0
+                61           0 RESUME                   0
                
-                58           2 LOAD_FAST                1 (adapter)
+                62           2 LOAD_FAST                1 (adapter)
                              4 LOAD_FAST                0 (self)
                              6 STORE_ATTR               0 (adapter)
                
-                59          16 LOAD_FAST                2 (model)
+                63          16 LOAD_FAST                2 (model)
                             18 LOAD_FAST                0 (self)
                             20 STORE_ATTR               1 (model)
                
-                60          30 LOAD_FAST                3 (getters)
+                64          30 LOAD_FAST                3 (getters)
                             32 LOAD_FAST                0 (self)
                             34 STORE_ATTR               2 (getters)
                
-                61          44 LOAD_FAST                5 (kwargs)
+                65          44 LOAD_FAST                5 (kwargs)
                             46 LOAD_FAST                0 (self)
                             48 STORE_ATTR               3 (kwargs)
                
-                62          58 LOAD_FAST                4 (as_var)
+                66          58 LOAD_FAST                4 (as_var)
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
-               filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\tester\\wagtail_fedit\\templatetags\\fedit.py'
+               filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Packages\\wagtail_fedit\\wagtail_fedit\\templatetags\\fedit.py'
                name       '__init__'
-               firstlineno 57
+               firstlineno 61
                lnotab 0x02010e010e010e010e01
             code
                argcount  : 3
                nlocals   : 6
                stacksize : 5
                flags     : 11
                code
@@ -466,70 +476,70 @@
                   00ab00000000000000000044005d325c0200007d047d0574030000000000
                   00000000007c05740400000000000000000000a6020000ab020000000000
                   00000072187c05a00300000000000000000000000000000000000000007c
                   01a6010000ab0100000000000000007c037c043c0000008c337403000000
                   000000000000007c02740400000000000000000000a6020000ab02000000
                   000000000072157c02a00300000000000000000000000000000000000000
                   007c01a6010000ab0100000000000000007d027c027c0366025300
-                64           0 RESUME                   0
+                68           0 RESUME                   0
                
-                65           2 LOAD_FAST                3 (kwargs)
+                69           2 LOAD_FAST                3 (kwargs)
                              4 LOAD_METHOD              0 (items)
                             26 PRECALL                  0
                             30 CALL                     0
                             40 GET_ITER
                        >>   42 FOR_ITER                50 (to 144)
                             44 UNPACK_SEQUENCE          2
                             48 STORE_FAST               4 (k)
                             50 STORE_FAST               5 (v)
                
-                66          52 LOAD_GLOBAL              3 (NULL + isinstance)
+                70          52 LOAD_GLOBAL              3 (NULL + isinstance)
                             64 LOAD_FAST                5 (v)
                             66 LOAD_GLOBAL              4 (FilterExpression)
                             78 PRECALL                  2
                             82 CALL                     2
                             92 POP_JUMP_FORWARD_IF_FALSE    24 (to 142)
                
-                67          94 LOAD_FAST                5 (v)
+                71          94 LOAD_FAST                5 (v)
                             96 LOAD_METHOD              3 (resolve)
                            118 LOAD_FAST                1 (context)
                            120 PRECALL                  1
                            124 CALL                     1
                            134 LOAD_FAST                3 (kwargs)
                            136 LOAD_FAST                4 (k)
                            138 STORE_SUBSCR
                        >>  142 JUMP_BACKWARD           51 (to 42)
                
-                69     >>  144 LOAD_GLOBAL              3 (NULL + isinstance)
+                73     >>  144 LOAD_GLOBAL              3 (NULL + isinstance)
                            156 LOAD_FAST                2 (model)
                            158 LOAD_GLOBAL              4 (FilterExpression)
                            170 PRECALL                  2
                            174 CALL                     2
                            184 POP_JUMP_FORWARD_IF_FALSE    21 (to 228)
                
-                70         186 LOAD_FAST                2 (model)
+                74         186 LOAD_FAST                2 (model)
                            188 LOAD_METHOD              3 (resolve)
                            210 LOAD_FAST                1 (context)
                            212 PRECALL                  1
                            216 CALL                     1
                            226 STORE_FAST               2 (model)
                
-                72     >>  228 LOAD_FAST                2 (model)
+                76     >>  228 LOAD_FAST                2 (model)
                            230 LOAD_FAST                3 (kwargs)
                            232 BUILD_TUPLE              2
                            234 RETURN_VALUE
                consts
                   None
                names      ('items', 'isinstance', 'FilterExpression', 'resolve')
                varnames   ('self', 'context', 'model', 'kwargs', 'k', 'v')
                freevars   ()
                cellvars   ()
-               filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\tester\\wagtail_fedit\\templatetags\\fedit.py'
+               filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Packages\\wagtail_fedit\\wagtail_fedit\\templatetags\\fedit.py'
                name       '_resolve_expressions'
-               firstlineno 64
+               firstlineno 68
                lnotab 0x020132012a0132022a012a02
             code
                argcount  : 2
                nlocals   : 12
                stacksize : 9
                flags     : 3
                code
@@ -560,327 +570,341 @@
                   20010074290000000000000000000064057c026a1500000000000000006a
                   0900000000000000009b0064067c099b009d04a6010000ab010000000000
                   000000820177007803590077017c01a01600000000000000000000000000
                   000000000000006407a6010000ab0100000000000000007d0a02007c006a
                   04000000000000000064097c067c057c0a64089c037c04a4018e017d0b7c
                   0ba0170000000000000000000000000000000000000000a6000000ab0000
                   0000000000000072107431000000000000000000007c0a7c06a6020000ab
-                  02000000000000000073437c01a019000000000000000000000000000000
+                  02000000000000000073627c01a019000000000000000000000000000000
                   00000000007c0b6a030000000000000000a6010000ab0100000000000000
-                  0001007419000000000000000000007c006a0c00000000000000007c017c
-                  0ba01a00000000000000000000000000000000000000007c01a6010000ab
-                  010000000000000000a6030000ab03000000000000000053007419000000
-                  000000000000007c006a0c00000000000000007c01743700000000000000
-                  0000007c0a7c0b7c01a6030000ab030000000000000000a6030000ab0300
-                  000000000000005300
-                74           0 RESUME                   0
+                  0001007435000000000000000000007c06743600000000000000000000a6
+                  020000ab020000000000000000720a7c067c017438000000000000000000
+                  003c0000007419000000000000000000007c006a0c00000000000000007c
+                  017c0ba01d00000000000000000000000000000000000000007c01a60100
+                  00ab010000000000000000a6030000ab0300000000000000005300741900
+                  0000000000000000007c006a0c00000000000000007c01743d0000000000
+                  00000000007c0a7c0b7c01a6030000ab030000000000000000a6030000ab
+                  0300000000000000005300
+                78           0 RESUME                   0
                
-                75           2 LOAD_FAST                0 (self)
+                79           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (model)
                             14 STORE_FAST               2 (model)
                
-                76          16 LOAD_FAST                0 (self)
+                80          16 LOAD_FAST                0 (self)
                             18 LOAD_ATTR                1 (getters)
                             28 STORE_FAST               3 (getters)
                
-                78          30 PUSH_NULL
+                82          30 PUSH_NULL
                             32 LOAD_FAST                0 (self)
                             34 LOAD_ATTR                2 (_resolve_expressions)
                
-                79          44 LOAD_FAST                1 (context)
+                83          44 LOAD_FAST                1 (context)
                             46 LOAD_FAST                2 (model)
                
-                78          48 BUILD_TUPLE              2
+                82          48 BUILD_TUPLE              2
                             50 BUILD_MAP                0
                
-                79          52 LOAD_FAST                0 (self)
+                83          52 LOAD_FAST                0 (self)
                             54 LOAD_ATTR                3 (kwargs)
                
-                78          64 DICT_MERGE               1
+                82          64 DICT_MERGE               1
                             66 CALL_FUNCTION_EX         1
                             68 UNPACK_SEQUENCE          2
                             72 STORE_FAST               2 (model)
                             74 STORE_FAST               4 (kwargs)
                
-                82          76 LOAD_CONST               1 ('wagtail_fedit_field')
+                86          76 LOAD_CONST               1 ('wagtail_fedit_field')
                             78 LOAD_FAST                1 (context)
                             80 CONTAINS_OP              0
                             82 POP_JUMP_FORWARD_IF_FALSE    36 (to 156)
                
-                83          84 LOAD_CONST               2 ('wagtail_fedit_instance')
+                87          84 LOAD_CONST               2 ('wagtail_fedit_instance')
                             86 LOAD_FAST                1 (context)
                             88 CONTAINS_OP              0
                             90 POP_JUMP_FORWARD_IF_FALSE    32 (to 156)
                
-                84          92 LOAD_FAST                2 (model)
+                88          92 LOAD_FAST                2 (model)
                
-                83          94 POP_JUMP_FORWARD_IF_TRUE    30 (to 156)
+                87          94 POP_JUMP_FORWARD_IF_TRUE    30 (to 156)
                
-                84          96 LOAD_FAST                0 (self)
+                88          96 LOAD_FAST                0 (self)
                             98 LOAD_ATTR                4 (adapter)
                            108 LOAD_ATTR                5 (field_required)
                
-                83         118 POP_JUMP_FORWARD_IF_FALSE    18 (to 156)
+                87         118 POP_JUMP_FORWARD_IF_FALSE    18 (to 156)
                
-                86         120 LOAD_FAST                1 (context)
+                90         120 LOAD_FAST                1 (context)
                            122 LOAD_CONST               1 ('wagtail_fedit_field')
                            124 BINARY_SUBSCR
                            134 STORE_FAST               5 (field_name)
                
-                87         136 LOAD_FAST                1 (context)
+                91         136 LOAD_FAST                1 (context)
                            138 LOAD_CONST               2 ('wagtail_fedit_instance')
                            140 BINARY_SUBSCR
                            150 STORE_FAST               6 (obj)
                            152 EXTENDED_ARG             1
                            154 JUMP_FORWARD           318 (to 792)
                
-                89     >>  156 LOAD_FAST                2 (model)
+                93     >>  156 LOAD_FAST                2 (model)
                            158 POP_JUMP_FORWARD_IF_TRUE    28 (to 216)
                            160 LOAD_CONST               2 ('wagtail_fedit_instance')
                            162 LOAD_FAST                1 (context)
                            164 CONTAINS_OP              0
                            166 POP_JUMP_FORWARD_IF_FALSE    24 (to 216)
                            168 LOAD_FAST                0 (self)
                            170 LOAD_ATTR                4 (adapter)
                            180 LOAD_ATTR                5 (field_required)
                            190 POP_JUMP_FORWARD_IF_TRUE    12 (to 216)
                
-                90         192 LOAD_FAST                1 (context)
+                94         192 LOAD_FAST                1 (context)
                            194 LOAD_CONST               2 ('wagtail_fedit_instance')
                            196 BINARY_SUBSCR
                            206 STORE_FAST               6 (obj)
                
-                91         208 LOAD_CONST               0 (None)
+                95         208 LOAD_CONST               0 (None)
                            210 STORE_FAST               5 (field_name)
                            212 EXTENDED_ARG             1
                            214 JUMP_FORWARD           288 (to 792)
                
-                95     >>  216 LOAD_FAST                2 (model)
+                99     >>  216 LOAD_FAST                2 (model)
                            218 POP_JUMP_FORWARD_IF_TRUE   152 (to 524)
                
-                96         220 LOAD_GLOBAL             13 (NULL + warnings)
+               100         220 LOAD_GLOBAL             13 (NULL + warnings)
                            232 LOAD_ATTR                7 (warn)
                
-                97         242 LOAD_GLOBAL             16 (WARNING_MODEL_INSTANCE_NOT_AVAILABLE)
+               101         242 LOAD_GLOBAL             16 (WARNING_MODEL_INSTANCE_NOT_AVAILABLE)
                
-                98         254 LOAD_CONST               3 ('object')
+               102         254 LOAD_CONST               3 ('object')
                            256 LOAD_FAST                0 (self)
                            258 LOAD_ATTR                4 (adapter)
                            268 LOAD_ATTR                9 (__name__)
                
-                97         278 BUILD_MAP                1
+               101         278 BUILD_MAP                1
                            280 BINARY_OP                6 (%)
                
-               100         284 LOAD_GLOBAL             20 (RuntimeWarning)
+               104         284 LOAD_GLOBAL             20 (RuntimeWarning)
                
-                96         296 PRECALL                  2
+               100         296 PRECALL                  2
                            300 CALL                     2
                            310 POP_TOP
                
-               103         312 LOAD_FAST                1 (context)
+               107         312 LOAD_FAST                1 (context)
                            314 LOAD_METHOD             11 (flatten)
                            336 PRECALL                  0
                            340 CALL                     0
                            350 STORE_FAST               1 (context)
                
-               105         352 NOP
+               109         352 NOP
                
-               106         354 LOAD_GLOBAL             25 (NULL + as_var)
+               110         354 LOAD_GLOBAL             25 (NULL + as_var)
                            366 LOAD_FAST                0 (self)
                            368 LOAD_ATTR               12 (as_var)
                            378 LOAD_FAST                1 (context)
                            380 PUSH_NULL
                            382 LOAD_FAST                0 (self)
                            384 LOAD_ATTR                4 (adapter)
                            394 LOAD_ATTR               13 (render_from_kwargs)
                
-               107         404 LOAD_FAST                1 (context)
+               111         404 LOAD_FAST                1 (context)
                
-               106         406 BUILD_TUPLE              1
+               110         406 BUILD_TUPLE              1
                            408 BUILD_MAP                0
                
-               107         410 LOAD_FAST                4 (kwargs)
+               111         410 LOAD_FAST                4 (kwargs)
                
-               106         412 DICT_MERGE               1
+               110         412 DICT_MERGE               1
                            414 CALL_FUNCTION_EX         1
                            416 PRECALL                  3
                            420 CALL                     3
                            430 RETURN_VALUE
                        >>  432 PUSH_EXC_INFO
                
-               109         434 LOAD_GLOBAL             28 (AdapterError)
+               113         434 LOAD_GLOBAL             28 (AdapterError)
                            446 CHECK_EXC_MATCH
                            448 POP_JUMP_FORWARD_IF_FALSE    33 (to 516)
                            450 STORE_FAST               7 (e)
                
-               110         452 LOAD_GLOBAL             31 (NULL + TemplateSyntaxError)
+               114         452 LOAD_GLOBAL             31 (NULL + TemplateSyntaxError)
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
                
-               109     >>  516 RERAISE                  0
+               113     >>  516 RERAISE                  0
                        >>  518 COPY                     3
                            520 POP_EXCEPT
                            522 RERAISE                  1
                
-               112     >>  524 LOAD_CONST               0 (None)
+               116     >>  524 LOAD_CONST               0 (None)
                            526 STORE_FAST               5 (field_name)
                
-               113         528 LOAD_FAST                2 (model)
+               117         528 LOAD_FAST                2 (model)
                            530 STORE_FAST               6 (obj)
                
-               114         532 LOAD_FAST                3 (getters)
+               118         532 LOAD_FAST                3 (getters)
                            534 POP_JUMP_FORWARD_IF_FALSE   128 (to 792)
                
-               115         536 LOAD_FAST                3 (getters)
+               119         536 LOAD_FAST                3 (getters)
                            538 LOAD_GLOBAL             35 (NULL + len)
                            550 LOAD_FAST                3 (getters)
                            552 PRECALL                  1
                            556 CALL                     1
                            566 LOAD_CONST               4 (1)
                            568 BINARY_OP               10 (-)
                            572 BINARY_SUBSCR
                            582 STORE_FAST               5 (field_name)
                
-               117         584 LOAD_GLOBAL             37 (NULL + range)
+               121         584 LOAD_GLOBAL             37 (NULL + range)
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
                
-               118         650 LOAD_FAST                3 (getters)
+               122         650 LOAD_FAST                3 (getters)
                            652 LOAD_FAST                8 (i)
                            654 BINARY_SUBSCR
                            664 STORE_FAST               9 (getter)
                
-               119         666 NOP
+               123         666 NOP
                
-               120         668 LOAD_GLOBAL             39 (NULL + getattr)
+               124         668 LOAD_GLOBAL             39 (NULL + getattr)
                            680 LOAD_FAST                6 (obj)
                            682 LOAD_FAST                9 (getter)
                            684 PRECALL                  2
                            688 CALL                     2
                            698 STORE_FAST               6 (obj)
                            700 JUMP_BACKWARD           28 (to 646)
                        >>  702 PUSH_EXC_INFO
                
-               121         704 LOAD_GLOBAL             40 (AttributeError)
+               125         704 LOAD_GLOBAL             40 (AttributeError)
                            716 CHECK_EXC_MATCH
                            718 POP_JUMP_FORWARD_IF_FALSE    32 (to 784)
                            720 POP_TOP
                
-               122         722 LOAD_GLOBAL             41 (NULL + AttributeError)
+               126         722 LOAD_GLOBAL             41 (NULL + AttributeError)
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
                
-               121     >>  784 RERAISE                  0
+               125     >>  784 RERAISE                  0
                        >>  786 COPY                     3
                            788 POP_EXCEPT
                            790 RERAISE                  1
                
-               125     >>  792 LOAD_FAST                1 (context)
+               129     >>  792 LOAD_FAST                1 (context)
                            794 LOAD_METHOD             22 (get)
                            816 LOAD_CONST               7 ('request')
                            818 PRECALL                  1
                            822 CALL                     1
                            832 STORE_FAST              10 (request)
                
-               126         834 PUSH_NULL
+               130         834 PUSH_NULL
                            836 LOAD_FAST                0 (self)
                            838 LOAD_ATTR                4 (adapter)
                            848 LOAD_CONST               9 (())
                
-               127         850 LOAD_FAST                6 (obj)
+               131         850 LOAD_FAST                6 (obj)
                
-               128         852 LOAD_FAST                5 (field_name)
+               132         852 LOAD_FAST                5 (field_name)
                
-               129         854 LOAD_FAST               10 (request)
+               133         854 LOAD_FAST               10 (request)
                
-               126         856 LOAD_CONST               8 (('object', 'field_name', 'request'))
+               130         856 LOAD_CONST               8 (('object', 'field_name', 'request'))
                            858 BUILD_CONST_KEY_MAP      3
                
-               130         860 LOAD_FAST                4 (kwargs)
+               134         860 LOAD_FAST                4 (kwargs)
                
-               126         862 DICT_MERGE               1
+               130         862 DICT_MERGE               1
                            864 CALL_FUNCTION_EX         1
                            866 STORE_FAST              11 (adapter)
                
-               133         868 LOAD_FAST               11 (adapter)
+               137         868 LOAD_FAST               11 (adapter)
                            870 LOAD_METHOD             23 (check_permissions)
                            892 PRECALL                  0
                            896 CALL                     0
                            906 POP_JUMP_FORWARD_IF_FALSE    16 (to 940)
                
-               134         908 LOAD_GLOBAL             49 (NULL + _can_edit)
+               138         908 LOAD_GLOBAL             49 (NULL + _can_edit)
                            920 LOAD_FAST               10 (request)
                            922 LOAD_FAST                6 (obj)
                            924 PRECALL                  2
                            928 CALL                     2
                
-               133         938 POP_JUMP_FORWARD_IF_TRUE    67 (to 1074)
+               137         938 POP_JUMP_FORWARD_IF_TRUE    98 (to 1136)
                
-               135     >>  940 LOAD_FAST                1 (context)
+               139     >>  940 LOAD_FAST                1 (context)
                            942 LOAD_METHOD             25 (update)
                            964 LOAD_FAST               11 (adapter)
                            966 LOAD_ATTR                3 (kwargs)
                            976 PRECALL                  1
                            980 CALL                     1
                            990 POP_TOP
                
-               136         992 LOAD_GLOBAL             25 (NULL + as_var)
-                          1004 LOAD_FAST                0 (self)
-                          1006 LOAD_ATTR               12 (as_var)
-                          1016 LOAD_FAST                1 (context)
-                          1018 LOAD_FAST               11 (adapter)
-                          1020 LOAD_METHOD             26 (render_content)
-                          1042 LOAD_FAST                1 (context)
-                          1044 PRECALL                  1
-                          1048 CALL                     1
-                          1058 PRECALL                  3
-                          1062 CALL                     3
-                          1072 RETURN_VALUE
-               
-               138     >> 1074 LOAD_GLOBAL             25 (NULL + as_var)
-                          1086 LOAD_FAST                0 (self)
-                          1088 LOAD_ATTR               12 (as_var)
-                          1098 LOAD_FAST                1 (context)
-                          1100 LOAD_GLOBAL             55 (NULL + wrap_adapter)
-                          1112 LOAD_FAST               10 (request)
-                          1114 LOAD_FAST               11 (adapter)
-                          1116 LOAD_FAST                1 (context)
-                          1118 PRECALL                  3
-                          1122 CALL                     3
-                          1132 PRECALL                  3
-                          1136 CALL                     3
-                          1146 RETURN_VALUE
+               141         992 LOAD_GLOBAL             53 (NULL + isinstance)
+                          1004 LOAD_FAST                6 (obj)
+                          1006 LOAD_GLOBAL             54 (Page)
+                          1018 PRECALL                  2
+                          1022 CALL                     2
+                          1032 POP_JUMP_FORWARD_IF_FALSE    10 (to 1054)
+               
+               142        1034 LOAD_FAST                6 (obj)
+                          1036 LOAD_FAST                1 (context)
+                          1038 LOAD_GLOBAL             56 (PAGE_TEMPLATE_VAR)
+                          1050 STORE_SUBSCR
+               
+               144     >> 1054 LOAD_GLOBAL             25 (NULL + as_var)
+                          1066 LOAD_FAST                0 (self)
+                          1068 LOAD_ATTR               12 (as_var)
+                          1078 LOAD_FAST                1 (context)
+                          1080 LOAD_FAST               11 (adapter)
+                          1082 LOAD_METHOD             29 (render_content)
+                          1104 LOAD_FAST                1 (context)
+                          1106 PRECALL                  1
+                          1110 CALL                     1
+                          1120 PRECALL                  3
+                          1124 CALL                     3
+                          1134 RETURN_VALUE
+               
+               146     >> 1136 LOAD_GLOBAL             25 (NULL + as_var)
+                          1148 LOAD_FAST                0 (self)
+                          1150 LOAD_ATTR               12 (as_var)
+                          1160 LOAD_FAST                1 (context)
+                          1162 LOAD_GLOBAL             61 (NULL + wrap_adapter)
+                          1174 LOAD_FAST               10 (request)
+                          1176 LOAD_FAST               11 (adapter)
+                          1178 LOAD_FAST                1 (context)
+                          1180 PRECALL                  3
+                          1184 CALL                     3
+                          1194 PRECALL                  3
+                          1198 CALL                     3
+                          1208 RETURN_VALUE
                ExceptionTable:
                  354 to 428 -> 432 [0]
                  432 to 450 -> 518 [1] lasti
                  452 to 506 -> 508 [1] lasti
                  508 to 516 -> 518 [1] lasti
                  668 to 698 -> 702 [1]
                  702 to 784 -> 786 [2] lasti
@@ -891,35 +915,35 @@
                   'object'
                   1
                   'Object '
                   ' does not have attribute '
                   'request'
                   ('object', 'field_name', 'request')
                   ()
-               names      ('model', 'getters', '_resolve_expressions', 'kwargs', 'adapter', 'field_required', 'warnings', 'warn', 'WARNING_MODEL_INSTANCE_NOT_AVAILABLE', '__name__', 'RuntimeWarning', 'flatten', 'as_var', 'render_from_kwargs', 'AdapterError', 'TemplateSyntaxError', 'str', 'len', 'range', 'getattr', 'AttributeError', '__class__', 'get', 'check_permissions', '_can_edit', 'update', 'render_content', 'wrap_adapter')
+               names      ('model', 'getters', '_resolve_expressions', 'kwargs', 'adapter', 'field_required', 'warnings', 'warn', 'WARNING_MODEL_INSTANCE_NOT_AVAILABLE', '__name__', 'RuntimeWarning', 'flatten', 'as_var', 'render_from_kwargs', 'AdapterError', 'TemplateSyntaxError', 'str', 'len', 'range', 'getattr', 'AttributeError', '__class__', 'get', 'check_permissions', '_can_edit', 'update', 'isinstance', 'Page', 'PAGE_TEMPLATE_VAR', 'render_content', 'wrap_adapter')
                varnames   ('self', 'context', 'model', 'getters', 'kwargs', 'field_name', 'obj', 'e', 'i', 'getter', 'request', 'adapter')
                freevars   ()
                cellvars   ()
-               filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\tester\\wagtail_fedit\\templatetags\\fedit.py'
+               filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Packages\\wagtail_fedit\\wagtail_fedit\\templatetags\\fedit.py'
                name       'render'
-               firstlineno 74
+               firstlineno 78
                lnotab
                   0x02010e010e020e0104ff04010cff0c040801080102ff020116ff020310
                   011402240110010804040116010c0118ff06030cfc100728020201320102
                   ff040102ff1603120140ff08030401040104013002420110010201240112
-                  013eff08042a0110010201020102fd040402fc060728011eff0202340152
-                  02
+                  013eff08042a0110010201020102fd040402fc060728011eff020234022a
+                  0114025202
             (None,)
          names      ('__name__', '__module__', '__qualname__', 'signing', 'TimestampSigner', 'signer', 'Type', 'BaseAdapter', 'FilterExpression', 'list', 'str', '__init__', '_resolve_expressions', 'render')
          varnames   ()
          freevars   ()
          cellvars   ()
-         filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\tester\\wagtail_fedit\\templatetags\\fedit.py'
+         filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Packages\\wagtail_fedit\\wagtail_fedit\\templatetags\\fedit.py'
          name       'AdapterNode'
-         firstlineno 54
+         firstlineno 58
          lnotab 0x0a011e023207060a
       'AdapterNode'
       ('name',)
       'parser'
       'token'
       code
          argcount  : 2
@@ -953,219 +977,219 @@
             01000000000000000064097a0a0000a6010000ab0100000000000000007d
             097c02a0010000000000000000000000000000000000000000740d000000
             000000000000007c02a6010000ab01000000000000000064097a0a0000a6
             010000ab01000000000000000001007413000000000000000000007c007c
             027c056a0a00000000000000007c056a0b00000000000000007c056a0c00
             00000000000000a6050000ab0500000000000000007d0a741b0000000000
             0000000000640c7c057c067c077c09640b9c047c0aa4018e015300
-         141           0 RESUME                   0
+         149           0 RESUME                   0
          
-         144           2 LOAD_FAST                1 (token)
+         152           2 LOAD_FAST                1 (token)
                        4 LOAD_METHOD              0 (split_contents)
                       26 PRECALL                  0
                       30 CALL                     0
                       40 STORE_FAST               2 (tokens)
          
-         146          42 LOAD_FAST                2 (tokens)
+         154          42 LOAD_FAST                2 (tokens)
                       44 LOAD_METHOD              1 (pop)
                       66 LOAD_CONST               1 (0)
                       68 PRECALL                  1
                       72 CALL                     1
                       82 STORE_FAST               3 (_)
          
-         147          84 LOAD_FAST                2 (tokens)
+         155          84 LOAD_FAST                2 (tokens)
                       86 LOAD_METHOD              1 (pop)
                      108 LOAD_CONST               1 (0)
                      110 PRECALL                  1
                      114 CALL                     1
                      124 STORE_FAST               4 (adapter_id)
          
-         149         126 NOP
+         157         126 NOP
          
-         150         128 LOAD_GLOBAL              4 (adapter_registry)
+         158         128 LOAD_GLOBAL              4 (adapter_registry)
                      140 LOAD_FAST                4 (adapter_id)
                      142 BINARY_SUBSCR
                      152 STORE_FAST               5 (adapter)
                      154 JUMP_FORWARD            33 (to 222)
                  >>  156 PUSH_EXC_INFO
          
-         151         158 LOAD_GLOBAL              6 (RegistryLookUpError)
+         159         158 LOAD_GLOBAL              6 (RegistryLookUpError)
                      170 CHECK_EXC_MATCH
                      172 POP_JUMP_FORWARD_IF_FALSE    20 (to 214)
                      174 POP_TOP
          
-         152         176 LOAD_GLOBAL              9 (NULL + TemplateSyntaxError)
+         160         176 LOAD_GLOBAL              9 (NULL + TemplateSyntaxError)
                      188 LOAD_CONST               2 ("No adapter found with identifier '")
                      190 LOAD_FAST                4 (adapter_id)
                      192 FORMAT_VALUE             0
                      194 LOAD_CONST               3 ("'")
                      196 BUILD_STRING             3
                      198 PRECALL                  1
                      202 CALL                     1
                      212 RAISE_VARARGS            1
          
-         151     >>  214 RERAISE                  0
+         159     >>  214 RERAISE                  0
                  >>  216 COPY                     3
                      218 POP_EXCEPT
                      220 RERAISE                  1
          
-         154     >>  222 LOAD_CONST               4 ((None, None))
+         162     >>  222 LOAD_CONST               4 ((None, None))
                      224 UNPACK_SEQUENCE          2
                      228 STORE_FAST               6 (model)
                      230 STORE_FAST               7 (model_tokens)
          
-         155         232 LOAD_FAST                2 (tokens)
+         163         232 LOAD_FAST                2 (tokens)
                      234 POP_JUMP_FORWARD_IF_FALSE   173 (to 582)
          
-         156         236 LOAD_FAST                2 (tokens)
+         164         236 LOAD_FAST                2 (tokens)
                      238 LOAD_METHOD              1 (pop)
                      260 LOAD_CONST               1 (0)
                      262 PRECALL                  1
                      266 CALL                     1
                      276 STORE_FAST               8 (model__field)
          
-         157         278 LOAD_FAST                8 (model__field)
+         165         278 LOAD_FAST                8 (model__field)
                      280 LOAD_METHOD              5 (split)
                      302 LOAD_CONST               5 ('.')
                      304 PRECALL                  1
                      308 CALL                     1
                      318 STORE_FAST               7 (model_tokens)
          
-         161         320 LOAD_GLOBAL             13 (NULL + len)
+         169         320 LOAD_GLOBAL             13 (NULL + len)
                      332 LOAD_FAST                7 (model_tokens)
                      334 PRECALL                  1
                      338 CALL                     1
                      348 LOAD_CONST               6 (2)
                      350 COMPARE_OP               0 (<)
                      356 POP_JUMP_FORWARD_IF_FALSE    34 (to 426)
          
-         162         358 LOAD_FAST                7 (model_tokens)
+         170         358 LOAD_FAST                7 (model_tokens)
                      360 LOAD_CONST               1 (0)
                      362 BINARY_SUBSCR
                      372 LOAD_CONST               7 ('from_context')
                      374 COMPARE_OP               3 (!=)
                      380 POP_JUMP_FORWARD_IF_FALSE    22 (to 426)
                      382 LOAD_FAST                5 (adapter)
                      384 LOAD_ATTR                7 (field_required)
                      394 POP_JUMP_FORWARD_IF_FALSE    15 (to 426)
          
-         163         396 LOAD_GLOBAL              9 (NULL + TemplateSyntaxError)
+         171         396 LOAD_GLOBAL              9 (NULL + TemplateSyntaxError)
          
-         164         408 LOAD_CONST               8 ("Model and field name are required: 'mymodel.myfield' or 'from_context'")
+         172         408 LOAD_CONST               8 ("Model and field name are required: 'mymodel.myfield' or 'from_context'")
          
-         163         410 PRECALL                  1
+         171         410 PRECALL                  1
                      414 CALL                     1
                      424 RAISE_VARARGS            1
          
-         168     >>  426 LOAD_GLOBAL             13 (NULL + len)
+         176     >>  426 LOAD_GLOBAL             13 (NULL + len)
                      438 LOAD_FAST                7 (model_tokens)
                      440 PRECALL                  1
                      444 CALL                     1
                      454 LOAD_CONST               9 (1)
                      456 COMPARE_OP               4 (>)
                      462 POP_JUMP_FORWARD_IF_TRUE    19 (to 502)
          
-         169         464 LOAD_FAST                7 (model_tokens)
+         177         464 LOAD_FAST                7 (model_tokens)
                      466 LOAD_CONST               1 (0)
                      468 BINARY_SUBSCR
                      478 LOAD_CONST               7 ('from_context')
                      480 COMPARE_OP               3 (!=)
                      486 POP_JUMP_FORWARD_IF_FALSE    47 (to 582)
                      488 LOAD_FAST                5 (adapter)
                      490 LOAD_ATTR                7 (field_required)
                      500 POP_JUMP_FORWARD_IF_TRUE    40 (to 582)
          
-         174     >>  502 LOAD_FAST                0 (parser)
+         182     >>  502 LOAD_FAST                0 (parser)
                      504 LOAD_METHOD              8 (compile_filter)
                      526 LOAD_FAST                7 (model_tokens)
                      528 LOAD_METHOD              1 (pop)
                      550 LOAD_CONST               1 (0)
                      552 PRECALL                  1
                      556 CALL                     1
                      566 PRECALL                  1
                      570 CALL                     1
                      580 STORE_FAST               6 (model)
          
-         176     >>  582 LOAD_CONST               0 (None)
+         184     >>  582 LOAD_CONST               0 (None)
                      584 STORE_FAST               9 (as_var)
          
-         177         586 LOAD_FAST                2 (tokens)
+         185         586 LOAD_FAST                2 (tokens)
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
          
-         178         646 LOAD_FAST                2 (tokens)
+         186         646 LOAD_FAST                2 (tokens)
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
          
-         179         720 LOAD_FAST                2 (tokens)
+         187         720 LOAD_FAST                2 (tokens)
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
          
-         181     >>  794 LOAD_GLOBAL             19 (NULL + get_kwargs)
+         189     >>  794 LOAD_GLOBAL             19 (NULL + get_kwargs)
          
-         182         806 LOAD_FAST                0 (parser)
+         190         806 LOAD_FAST                0 (parser)
          
-         183         808 LOAD_FAST                2 (tokens)
+         191         808 LOAD_FAST                2 (tokens)
          
-         184         810 LOAD_FAST                5 (adapter)
+         192         810 LOAD_FAST                5 (adapter)
                      812 LOAD_ATTR               10 (required_kwargs)
          
-         185         822 LOAD_FAST                5 (adapter)
+         193         822 LOAD_FAST                5 (adapter)
                      824 LOAD_ATTR               11 (absolute_tokens)
          
-         186         834 LOAD_FAST                5 (adapter)
+         194         834 LOAD_FAST                5 (adapter)
                      836 LOAD_ATTR               12 (optional_kwargs)
          
-         181         846 PRECALL                  5
+         189         846 PRECALL                  5
                      850 CALL                     5
                      860 STORE_FAST              10 (kwargs)
          
-         189         862 LOAD_GLOBAL             27 (NULL + AdapterNode)
+         197         862 LOAD_GLOBAL             27 (NULL + AdapterNode)
                      874 LOAD_CONST              12 (())
          
-         190         876 LOAD_FAST                5 (adapter)
+         198         876 LOAD_FAST                5 (adapter)
          
-         191         878 LOAD_FAST                6 (model)
+         199         878 LOAD_FAST                6 (model)
          
-         192         880 LOAD_FAST                7 (model_tokens)
+         200         880 LOAD_FAST                7 (model_tokens)
          
-         193         882 LOAD_FAST                9 (as_var)
+         201         882 LOAD_FAST                9 (as_var)
          
-         189         884 LOAD_CONST              11 (('adapter', 'model', 'getters', 'as_var'))
+         197         884 LOAD_CONST              11 (('adapter', 'model', 'getters', 'as_var'))
                      886 BUILD_CONST_KEY_MAP      4
          
-         194         888 LOAD_FAST               10 (kwargs)
+         202         888 LOAD_FAST               10 (kwargs)
          
-         189         890 DICT_MERGE               1
+         197         890 DICT_MERGE               1
                      892 CALL_FUNCTION_EX         1
                      894 RETURN_VALUE
          ExceptionTable:
            128 to 152 -> 156 [0]
            156 to 214 -> 216 [1] lasti
          consts
             None
@@ -1181,110 +1205,127 @@
             'as'
             ('adapter', 'model', 'getters', 'as_var')
             ()
          names      ('split_contents', 'pop', 'adapter_registry', 'RegistryLookUpError', 'TemplateSyntaxError', 'split', 'len', 'field_required', 'compile_filter', 'get_kwargs', 'required_kwargs', 'absolute_tokens', 'optional_kwargs', 'AdapterNode')
          varnames   ('parser', 'token', 'tokens', '_', 'adapter_id', 'adapter', 'model', 'model_tokens', 'model__field', 'as_var', 'kwargs')
          freevars   ()
          cellvars   ()
-         filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\tester\\wagtail_fedit\\templatetags\\fedit.py'
+         filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Packages\\wagtail_fedit\\wagtail_fedit\\templatetags\\fedit.py'
          name       'do_render_fedit'
-         firstlineno 141
+         firstlineno 149
          lnotab
             0x020328022a012a0202011e01120126ff08030a0104012a012a04260126
             010c0102ff100526012605500204013c014a014a020c01020102010c010c
             010cfb10080e0102010201020102fc040502fb
       True
       ('takes_context',)
       'adapter'
       code
          argcount  : 2
          nlocals   : 3
-         stacksize : 3
+         stacksize : 4
          flags     : 3
          code
             0x970069007d0264017c007600720b7c006401190000000000000000007d
             027c0064013d007c00a00000000000000000000000000000000000000000
             007c02a6010000ab01000000000000000001007c016a0100000000000000
             007c0064023c0000007c016a0200000000000000007c0064033c0000007c
             016a0300000000000000007c0064043c0000007c00a00000000000000000
             000000000000000000000000007c016a040000000000000000a6010000ab
-            01000000000000000001007c01a005000000000000000000000000000000
-            00000000007c00a6010000ab0100000000000000005300
-         199           0 RESUME                   0
+            0100000000000000000100740b000000000000000000007c016a02000000
+            0000000000740c00000000000000000000a6020000ab0200000000000000
+            00720f7c016a0200000000000000007c00740e000000000000000000003c
+            0000007c01a00800000000000000000000000000000000000000007c00a6
+            010000ab0100000000000000005300
+         207           0 RESUME                   0
          
-         201           2 BUILD_MAP                0
+         209           2 BUILD_MAP                0
                        4 STORE_FAST               2 (parent_context)
          
-         203           6 LOAD_CONST               1 ('parent_context')
+         211           6 LOAD_CONST               1 ('parent_context')
                        8 LOAD_FAST                0 (context)
                       10 CONTAINS_OP              0
                       12 POP_JUMP_FORWARD_IF_FALSE    11 (to 36)
          
-         204          14 LOAD_FAST                0 (context)
+         212          14 LOAD_FAST                0 (context)
                       16 LOAD_CONST               1 ('parent_context')
                       18 BINARY_SUBSCR
                       28 STORE_FAST               2 (parent_context)
          
-         205          30 LOAD_FAST                0 (context)
+         213          30 LOAD_FAST                0 (context)
                       32 LOAD_CONST               1 ('parent_context')
                       34 DELETE_SUBSCR
          
-         207     >>   36 LOAD_FAST                0 (context)
+         215     >>   36 LOAD_FAST                0 (context)
                       38 LOAD_METHOD              0 (update)
                       60 LOAD_FAST                2 (parent_context)
                       62 PRECALL                  1
                       66 CALL                     1
                       76 POP_TOP
          
-         209          78 LOAD_FAST                1 (adapter)
+         217          78 LOAD_FAST                1 (adapter)
                       80 LOAD_ATTR                1 (field_name)
                       90 LOAD_FAST                0 (context)
                       92 LOAD_CONST               2 ('wagtail_fedit_field')
                       94 STORE_SUBSCR
          
-         210          98 LOAD_FAST                1 (adapter)
+         218          98 LOAD_FAST                1 (adapter)
                      100 LOAD_ATTR                2 (object)
                      110 LOAD_FAST                0 (context)
                      112 LOAD_CONST               3 ('wagtail_fedit_instance')
                      114 STORE_SUBSCR
          
-         211         118 LOAD_FAST                1 (adapter)
+         219         118 LOAD_FAST                1 (adapter)
                      120 LOAD_ATTR                3 (request)
                      130 LOAD_FAST                0 (context)
                      132 LOAD_CONST               4 ('request')
                      134 STORE_SUBSCR
          
-         213         138 LOAD_FAST                0 (context)
+         221         138 LOAD_FAST                0 (context)
                      140 LOAD_METHOD              0 (update)
                      162 LOAD_FAST                1 (adapter)
                      164 LOAD_ATTR                4 (kwargs)
                      174 PRECALL                  1
                      178 CALL                     1
                      188 POP_TOP
          
-         215         190 LOAD_FAST                1 (adapter)
-                     192 LOAD_METHOD              5 (render_content)
-                     214 LOAD_FAST                0 (context)
-                     216 PRECALL                  1
-                     220 CALL                     1
-                     230 RETURN_VALUE
+         223         190 LOAD_GLOBAL             11 (NULL + isinstance)
+                     202 LOAD_FAST                1 (adapter)
+                     204 LOAD_ATTR                2 (object)
+                     214 LOAD_GLOBAL             12 (Page)
+                     226 PRECALL                  2
+                     230 CALL                     2
+                     240 POP_JUMP_FORWARD_IF_FALSE    15 (to 272)
+         
+         224         242 LOAD_FAST                1 (adapter)
+                     244 LOAD_ATTR                2 (object)
+                     254 LOAD_FAST                0 (context)
+                     256 LOAD_GLOBAL             14 (PAGE_TEMPLATE_VAR)
+                     268 STORE_SUBSCR
+         
+         226     >>  272 LOAD_FAST                1 (adapter)
+                     274 LOAD_METHOD              8 (render_content)
+                     296 LOAD_FAST                0 (context)
+                     298 PRECALL                  1
+                     302 CALL                     1
+                     312 RETURN_VALUE
          consts
             None
             'parent_context'
             'wagtail_fedit_field'
             'wagtail_fedit_instance'
             'request'
-         names      ('update', 'field_name', 'object', 'request', 'kwargs', 'render_content')
+         names      ('update', 'field_name', 'object', 'request', 'kwargs', 'isinstance', 'Page', 'PAGE_TEMPLATE_VAR', 'render_content')
          varnames   ('context', 'adapter', 'parent_context')
          freevars   ()
          cellvars   ()
-         filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\tester\\wagtail_fedit\\templatetags\\fedit.py'
+         filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Packages\\wagtail_fedit\\wagtail_fedit\\templatetags\\fedit.py'
          name       'render_adapter'
-         firstlineno 199
-         lnotab 0x020204020801100106022a021401140114023402
+         firstlineno 207
+         lnotab 0x020204020801100106022a02140114011402340234011e02
       'wagtail_fedit/_hook_output.html'
       'fedit_scripts'
       ('name', 'takes_context')
       code
          argcount  : 2
          nlocals   : 7
          stacksize : 6
@@ -1300,123 +1341,123 @@
             00530067007d04740f000000000000000000006a0800000000000000007c
             03a6010000ab01000000000000000044005d417d0502007c057c02a60100
             00ab0100000000000000007d067413000000000000000000007c06741400
             0000000000000000007416000000000000000000006602a6020000ab0200
             0000000000000073037c0667017d067c04a00c0000000000000000000000
             0000000000000000007c06a6010000ab01000000000000000001008c4264
             067c0469015300
-         218           0 RESUME                   0
+         229           0 RESUME                   0
          
-         220           2 LOAD_FAST                1 (css_or_js)
+         231           2 LOAD_FAST                1 (css_or_js)
                        4 LOAD_METHOD              0 (lower)
                       26 PRECALL                  0
                       30 CALL                     0
                       40 STORE_FAST               1 (css_or_js)
          
-         222          42 LOAD_FAST                1 (css_or_js)
+         233          42 LOAD_FAST                1 (css_or_js)
                       44 LOAD_CONST               1 (('css', 'js'))
                       46 CONTAINS_OP              1
                       48 POP_JUMP_FORWARD_IF_FALSE    15 (to 80)
          
-         223          50 LOAD_GLOBAL              3 (NULL + ValueError)
+         234          50 LOAD_GLOBAL              3 (NULL + ValueError)
                       62 LOAD_CONST               2 ("Invalid argument, must be 'css' or 'js'")
                       64 PRECALL                  1
                       68 CALL                     1
                       78 RAISE_VARARGS            1
          
-         225     >>   80 LOAD_FAST                0 (context)
+         236     >>   80 LOAD_FAST                0 (context)
                       82 LOAD_METHOD              2 (get)
                      104 LOAD_CONST               3 ('request')
                      106 PRECALL                  1
                      110 CALL                     1
                      120 STORE_FAST               2 (request)
          
-         227         122 LOAD_FAST                1 (css_or_js)
+         238         122 LOAD_FAST                1 (css_or_js)
                      124 LOAD_CONST               4 ('css')
                      126 COMPARE_OP               2 (==)
                      132 POP_JUMP_FORWARD_IF_FALSE     8 (to 150)
          
-         228         134 LOAD_GLOBAL              6 (REGISTER_CSS)
+         239         134 LOAD_GLOBAL              6 (REGISTER_CSS)
                      146 STORE_FAST               3 (hook_name)
                      148 JUMP_FORWARD             7 (to 164)
          
-         230     >>  150 LOAD_GLOBAL              8 (REGISTER_JS)
+         241     >>  150 LOAD_GLOBAL              8 (REGISTER_JS)
                      162 STORE_FAST               3 (hook_name)
          
-         232     >>  164 LOAD_GLOBAL             11 (NULL + getattr)
+         243     >>  164 LOAD_GLOBAL             11 (NULL + getattr)
                      176 LOAD_FAST                2 (request)
                      178 LOAD_GLOBAL             12 (FEDIT_PREVIEW_VAR)
                      190 LOAD_CONST               5 (False)
                      192 PRECALL                  3
                      196 CALL                     3
                      206 POP_JUMP_FORWARD_IF_TRUE     2 (to 212)
          
-         233         208 BUILD_MAP                0
+         244         208 BUILD_MAP                0
                      210 RETURN_VALUE
          
-         235     >>  212 BUILD_LIST               0
+         246     >>  212 BUILD_LIST               0
                      214 STORE_FAST               4 (files)
          
-         236         216 LOAD_GLOBAL             15 (NULL + hooks)
+         247         216 LOAD_GLOBAL             15 (NULL + hooks)
                      228 LOAD_ATTR                8 (get_hooks)
                      238 LOAD_FAST                3 (hook_name)
                      240 PRECALL                  1
                      244 CALL                     1
                      254 GET_ITER
                  >>  256 FOR_ITER                65 (to 388)
                      258 STORE_FAST               5 (hook)
          
-         237         260 PUSH_NULL
+         248         260 PUSH_NULL
                      262 LOAD_FAST                5 (hook)
                      264 LOAD_FAST                2 (request)
                      266 PRECALL                  1
                      270 CALL                     1
                      280 STORE_FAST               6 (ret)
          
-         239         282 LOAD_GLOBAL             19 (NULL + isinstance)
+         250         282 LOAD_GLOBAL             19 (NULL + isinstance)
                      294 LOAD_FAST                6 (ret)
                      296 LOAD_GLOBAL             20 (list)
                      308 LOAD_GLOBAL             22 (tuple)
                      320 BUILD_TUPLE              2
                      322 PRECALL                  2
                      326 CALL                     2
                      336 POP_JUMP_FORWARD_IF_TRUE     3 (to 344)
          
-         240         338 LOAD_FAST                6 (ret)
+         251         338 LOAD_FAST                6 (ret)
                      340 BUILD_LIST               1
                      342 STORE_FAST               6 (ret)
          
-         242     >>  344 LOAD_FAST                4 (files)
+         253     >>  344 LOAD_FAST                4 (files)
                      346 LOAD_METHOD             12 (extend)
                      368 LOAD_FAST                6 (ret)
                      370 PRECALL                  1
                      374 CALL                     1
                      384 POP_TOP
                      386 JUMP_BACKWARD           66 (to 256)
          
-         245     >>  388 LOAD_CONST               6 ('hook_output')
+         256     >>  388 LOAD_CONST               6 ('hook_output')
                      390 LOAD_FAST                4 (files)
          
-         244         392 BUILD_MAP                1
+         255         392 BUILD_MAP                1
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
-         filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\tester\\wagtail_fedit\\templatetags\\fedit.py'
+         filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Packages\\wagtail_fedit\\wagtail_fedit\\templatetags\\fedit.py'
          name       'static_hook_output'
-         firstlineno 218
+         firstlineno 229
          lnotab
             0x0202280208011e022a020c0110020e022c01040204012c011602380106
             022c0304ff
       False
       'tooltip'
       ('takes_context', 'name')
       'wrapping'
@@ -1432,37 +1473,37 @@
             00000064037c049b0064047405000000000000000000007c05a6010000ab
             0100000000000000009b0064059d05a6010000ab01000000000000000001
             008c2f6406a00300000000000000000000000000000000000000007c03a6
             010000ab0100000000000000007d067c01730f7409000000000000000000
             007c06a6010000ab01000000000000000053007409000000000000000000
             0064077c069b0064087c019b0064099d05a6010000ab0100000000000000
             005300
-         248           0 RESUME                   0
+         259           0 RESUME                   0
          
-         250           2 LOAD_FAST                0 (content)
+         261           2 LOAD_FAST                0 (content)
                        4 LOAD_FAST                2 (kwargs)
                        6 LOAD_CONST               1 ('content')
                        8 STORE_SUBSCR
          
-         252          12 LOAD_CONST               2 ("data-tooltip='true'")
+         263          12 LOAD_CONST               2 ("data-tooltip='true'")
          
-         251          14 BUILD_LIST               1
+         262          14 BUILD_LIST               1
                       16 STORE_FAST               3 (s)
          
-         254          18 LOAD_FAST                2 (kwargs)
+         265          18 LOAD_FAST                2 (kwargs)
                       20 LOAD_METHOD              0 (items)
                       42 PRECALL                  0
                       46 CALL                     0
                       56 GET_ITER
                  >>   58 FOR_ITER                46 (to 152)
                       60 UNPACK_SEQUENCE          2
                       64 STORE_FAST               4 (key)
                       66 STORE_FAST               5 (value)
          
-         255          68 LOAD_FAST                3 (s)
+         266          68 LOAD_FAST                3 (s)
                       70 LOAD_METHOD              1 (append)
                       92 LOAD_CONST               3 ('data-tooltip-')
                       94 LOAD_FAST                4 (key)
                       96 FORMAT_VALUE             0
                       98 LOAD_CONST               4 ("='")
                      100 LOAD_GLOBAL              5 (NULL + escape)
                      112 LOAD_FAST                5 (value)
@@ -1472,31 +1513,31 @@
                      130 LOAD_CONST               5 ("'")
                      132 BUILD_STRING             5
                      134 PRECALL                  1
                      138 CALL                     1
                      148 POP_TOP
                      150 JUMP_BACKWARD           47 (to 58)
          
-         256     >>  152 LOAD_CONST               6 (' ')
+         267     >>  152 LOAD_CONST               6 (' ')
                      154 LOAD_METHOD              3 (join)
                      176 LOAD_FAST                3 (s)
                      178 PRECALL                  1
                      182 CALL                     1
                      192 STORE_FAST               6 (attrs)
          
-         258         194 LOAD_FAST                1 (wrapping)
+         269         194 LOAD_FAST                1 (wrapping)
                      196 POP_JUMP_FORWARD_IF_TRUE    15 (to 228)
          
-         259         198 LOAD_GLOBAL              9 (NULL + mark_safe)
+         270         198 LOAD_GLOBAL              9 (NULL + mark_safe)
                      210 LOAD_FAST                6 (attrs)
                      212 PRECALL                  1
                      216 CALL                     1
                      226 RETURN_VALUE
          
-         261     >>  228 LOAD_GLOBAL              9 (NULL + mark_safe)
+         272     >>  228 LOAD_GLOBAL              9 (NULL + mark_safe)
                      240 LOAD_CONST               7 ('<span ')
                      242 LOAD_FAST                6 (attrs)
                      244 FORMAT_VALUE             0
                      246 LOAD_CONST               8 ('>')
                      248 LOAD_FAST                1 (wrapping)
                      250 FORMAT_VALUE             0
                      252 LOAD_CONST               9 ('</span>')
@@ -1515,17 +1556,17 @@
             '<span '
             '>'
             '</span>'
          names      ('items', 'append', 'escape', 'join', 'mark_safe')
          varnames   ('content', 'wrapping', 'kwargs', 's', 'key', 'value', 'attrs')
          freevars   ()
          cellvars   ()
-         filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\tester\\wagtail_fedit\\templatetags\\fedit.py'
+         filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Packages\\wagtail_fedit\\wagtail_fedit\\templatetags\\fedit.py'
          name       'tooltip'
-         firstlineno 248
+         firstlineno 259
          lnotab 0x02020a0202ff0403320154012a0204011e02
       'tokens'
       'kwarg_list'
       'absolute_tokens'
       'optional_tokens'
       code
          argcount  : 5
@@ -1556,235 +1597,235 @@
             0500000000000000000000000000000000000000007c0964031900000000
             0000000000a6010000ab0100000000000000007c067c0a3c00000064057d
             0590018c147c0244005d187d0c7c0c7c0676017212740d00000000000000
             00000064097c0c9b009d02a6010000ab01000000000000000082018c197c
             04a0070000000000000000000000000000000000000000a6000000ab0000
             0000000000000044005d0e5c0200007d0a7d0b7c0a7c06760172057c0b7c
             067c0a3c0000008c0f7c065300
-         264           0 RESUME                   0
+         275           0 RESUME                   0
          
-         265           2 LOAD_CONST               1 (False)
+         276           2 LOAD_CONST               1 (False)
                        4 STORE_FAST               5 (had_kwargs)
          
-         266           6 BUILD_MAP                0
+         277           6 BUILD_MAP                0
                        8 STORE_FAST               6 (kwargs)
          
-         268          10 LOAD_FAST                2 (kwarg_list)
+         279          10 LOAD_FAST                2 (kwarg_list)
                       12 POP_JUMP_FORWARD_IF_TRUE    14 (to 42)
          
-         269          14 LOAD_GLOBAL              1 (NULL + tuple)
+         280          14 LOAD_GLOBAL              1 (NULL + tuple)
                       26 PRECALL                  0
                       30 CALL                     0
                       40 STORE_FAST               2 (kwarg_list)
          
-         271     >>   42 LOAD_FAST                3 (absolute_tokens)
+         282     >>   42 LOAD_FAST                3 (absolute_tokens)
                       44 POP_JUMP_FORWARD_IF_TRUE    14 (to 74)
          
-         272          46 LOAD_GLOBAL              1 (NULL + tuple)
+         283          46 LOAD_GLOBAL              1 (NULL + tuple)
                       58 PRECALL                  0
                       62 CALL                     0
                       72 STORE_FAST               3 (absolute_tokens)
          
-         274     >>   74 LOAD_FAST                4 (optional_tokens)
+         285     >>   74 LOAD_FAST                4 (optional_tokens)
                       76 POP_JUMP_FORWARD_IF_TRUE     2 (to 82)
          
-         275          78 BUILD_MAP                0
+         286          78 BUILD_MAP                0
                       80 STORE_FAST               4 (optional_tokens)
          
-         277     >>   82 LOAD_GLOBAL              3 (NULL + enumerate)
+         288     >>   82 LOAD_GLOBAL              3 (NULL + enumerate)
                       94 LOAD_FAST                1 (tokens)
                       96 PRECALL                  1
                      100 CALL                     1
                      110 GET_ITER
                  >>  112 EXTENDED_ARG             1
                      114 FOR_ITER               274 (to 664)
                      116 UNPACK_SEQUENCE          2
                      120 STORE_FAST               7 (i)
                      122 STORE_FAST               8 (token)
          
-         278         124 LOAD_FAST                8 (token)
+         289         124 LOAD_FAST                8 (token)
                      126 LOAD_METHOD              2 (split)
                      148 LOAD_CONST               2 ('=')
                      150 PRECALL                  1
                      154 CALL                     1
                      164 STORE_FAST               9 (split)
          
-         279         166 LOAD_GLOBAL              7 (NULL + len)
+         290         166 LOAD_GLOBAL              7 (NULL + len)
                      178 LOAD_FAST                9 (split)
                      180 PRECALL                  1
                      184 CALL                     1
                      194 LOAD_CONST               3 (1)
                      196 COMPARE_OP               2 (==)
                      202 POP_JUMP_FORWARD_IF_FALSE    89 (to 382)
                      204 LOAD_GLOBAL              7 (NULL + len)
                      216 LOAD_FAST                2 (kwarg_list)
                      218 PRECALL                  1
                      222 CALL                     1
                      232 LOAD_FAST                7 (i)
                      234 COMPARE_OP               4 (>)
                      240 POP_JUMP_FORWARD_IF_FALSE    70 (to 382)
          
-         280         242 LOAD_FAST                9 (split)
+         291         242 LOAD_FAST                9 (split)
                      244 LOAD_CONST               4 (0)
                      246 BINARY_SUBSCR
                      256 LOAD_FAST                3 (absolute_tokens)
                      258 CONTAINS_OP              0
                      260 POP_JUMP_FORWARD_IF_FALSE    12 (to 286)
          
-         281         262 LOAD_CONST               5 (True)
+         292         262 LOAD_CONST               5 (True)
                      264 LOAD_FAST                6 (kwargs)
                      266 LOAD_FAST                9 (split)
                      268 LOAD_CONST               4 (0)
                      270 BINARY_SUBSCR
                      280 STORE_SUBSCR
          
-         282         284 JUMP_BACKWARD           87 (to 112)
+         293         284 JUMP_BACKWARD           87 (to 112)
          
-         284     >>  286 LOAD_FAST                5 (had_kwargs)
+         295     >>  286 LOAD_FAST                5 (had_kwargs)
                      288 POP_JUMP_FORWARD_IF_FALSE    15 (to 320)
          
-         285         290 LOAD_GLOBAL              9 (NULL + ValueError)
+         296         290 LOAD_GLOBAL              9 (NULL + ValueError)
                      302 LOAD_CONST               6 ('Unexpected positional argument after keyword argument')
                      304 PRECALL                  1
                      308 CALL                     1
                      318 RAISE_VARARGS            1
          
-         287     >>  320 LOAD_FAST                0 (parser)
+         298     >>  320 LOAD_FAST                0 (parser)
                      322 LOAD_METHOD              5 (compile_filter)
                      344 LOAD_FAST                8 (token)
                      346 PRECALL                  1
                      350 CALL                     1
                      360 LOAD_FAST                6 (kwargs)
                      362 LOAD_FAST                2 (kwarg_list)
                      364 LOAD_FAST                7 (i)
                      366 BINARY_SUBSCR
                      376 STORE_SUBSCR
                      380 JUMP_BACKWARD          135 (to 112)
          
-         288     >>  382 LOAD_GLOBAL              7 (NULL + len)
+         299     >>  382 LOAD_GLOBAL              7 (NULL + len)
                      394 LOAD_FAST                9 (split)
                      396 PRECALL                  1
                      400 CALL                     1
                      410 LOAD_CONST               3 (1)
                      412 COMPARE_OP               2 (==)
                      418 POP_JUMP_FORWARD_IF_FALSE    57 (to 534)
          
-         289         420 LOAD_FAST                9 (split)
+         300         420 LOAD_FAST                9 (split)
                      422 LOAD_CONST               4 (0)
                      424 BINARY_SUBSCR
                      434 LOAD_FAST                3 (absolute_tokens)
                      436 CONTAINS_OP              0
                      438 POP_JUMP_FORWARD_IF_FALSE    12 (to 464)
          
-         290         440 LOAD_CONST               5 (True)
+         301         440 LOAD_CONST               5 (True)
                      442 LOAD_FAST                6 (kwargs)
                      444 LOAD_FAST                9 (split)
                      446 LOAD_CONST               4 (0)
                      448 BINARY_SUBSCR
                      458 STORE_SUBSCR
          
-         291         462 JUMP_BACKWARD          176 (to 112)
+         302         462 JUMP_BACKWARD          176 (to 112)
          
-         293     >>  464 LOAD_FAST                9 (split)
+         304     >>  464 LOAD_FAST                9 (split)
                      466 LOAD_CONST               4 (0)
                      468 BINARY_SUBSCR
                      478 STORE_FAST              10 (key)
          
-         294         480 LOAD_FAST                0 (parser)
+         305         480 LOAD_FAST                0 (parser)
                      482 LOAD_METHOD              5 (compile_filter)
                      504 LOAD_FAST               10 (key)
                      506 PRECALL                  1
                      510 CALL                     1
                      520 STORE_FAST              11 (value)
          
-         295         522 LOAD_FAST               11 (value)
+         306         522 LOAD_FAST               11 (value)
                      524 LOAD_FAST                6 (kwargs)
                      526 LOAD_FAST               10 (key)
                      528 STORE_SUBSCR
                      532 JUMP_BACKWARD          211 (to 112)
          
-         297     >>  534 LOAD_FAST                9 (split)
+         308     >>  534 LOAD_FAST                9 (split)
                      536 LOAD_CONST               4 (0)
                      538 BINARY_SUBSCR
                      548 STORE_FAST              10 (key)
          
-         300         550 LOAD_FAST               10 (key)
+         311         550 LOAD_FAST               10 (key)
                      552 LOAD_FAST                3 (absolute_tokens)
                      554 CONTAINS_OP              0
                      556 POP_JUMP_FORWARD_IF_FALSE    19 (to 596)
          
-         301         558 LOAD_GLOBAL              9 (NULL + ValueError)
+         312         558 LOAD_GLOBAL              9 (NULL + ValueError)
                      570 LOAD_CONST               7 ('Keyword argument ')
                      572 LOAD_FAST               10 (key)
                      574 FORMAT_VALUE             0
                      576 LOAD_CONST               8 (' cannot be resolved; it will not be parsed as a variable.')
                      578 BUILD_STRING             3
                      580 PRECALL                  1
                      584 CALL                     1
                      594 RAISE_VARARGS            1
          
-         303     >>  596 LOAD_FAST                0 (parser)
+         314     >>  596 LOAD_FAST                0 (parser)
                      598 LOAD_METHOD              5 (compile_filter)
                      620 LOAD_FAST                9 (split)
                      622 LOAD_CONST               3 (1)
                      624 BINARY_SUBSCR
                      634 PRECALL                  1
                      638 CALL                     1
                      648 LOAD_FAST                6 (kwargs)
                      650 LOAD_FAST               10 (key)
                      652 STORE_SUBSCR
          
-         304         656 LOAD_CONST               5 (True)
+         315         656 LOAD_CONST               5 (True)
                      658 STORE_FAST               5 (had_kwargs)
                      660 EXTENDED_ARG             1
                      662 JUMP_BACKWARD          276 (to 112)
          
-         306     >>  664 LOAD_FAST                2 (kwarg_list)
+         317     >>  664 LOAD_FAST                2 (kwarg_list)
                      666 GET_ITER
                  >>  668 FOR_ITER                24 (to 718)
                      670 STORE_FAST              12 (kwarg)
          
-         307         672 LOAD_FAST               12 (kwarg)
+         318         672 LOAD_FAST               12 (kwarg)
                      674 LOAD_FAST                6 (kwargs)
                      676 CONTAINS_OP              1
                      678 POP_JUMP_FORWARD_IF_FALSE    18 (to 716)
          
-         308         680 LOAD_GLOBAL             13 (NULL + TemplateSyntaxError)
+         319         680 LOAD_GLOBAL             13 (NULL + TemplateSyntaxError)
                      692 LOAD_CONST               9 ('Missing required keyword argument ')
                      694 LOAD_FAST               12 (kwarg)
                      696 FORMAT_VALUE             0
                      698 BUILD_STRING             2
                      700 PRECALL                  1
                      704 CALL                     1
                      714 RAISE_VARARGS            1
          
-         307     >>  716 JUMP_BACKWARD           25 (to 668)
+         318     >>  716 JUMP_BACKWARD           25 (to 668)
          
-         310     >>  718 LOAD_FAST                4 (optional_tokens)
+         321     >>  718 LOAD_FAST                4 (optional_tokens)
                      720 LOAD_METHOD              7 (items)
                      742 PRECALL                  0
                      746 CALL                     0
                      756 GET_ITER
                  >>  758 FOR_ITER                14 (to 788)
                      760 UNPACK_SEQUENCE          2
                      764 STORE_FAST              10 (key)
                      766 STORE_FAST              11 (value)
          
-         311         768 LOAD_FAST               10 (key)
+         322         768 LOAD_FAST               10 (key)
                      770 LOAD_FAST                6 (kwargs)
                      772 CONTAINS_OP              1
                      774 POP_JUMP_FORWARD_IF_FALSE     5 (to 786)
          
-         312         776 LOAD_FAST               11 (value)
+         323         776 LOAD_FAST               11 (value)
                      778 LOAD_FAST                6 (kwargs)
                      780 LOAD_FAST               10 (key)
                      782 STORE_SUBSCR
                  >>  786 JUMP_BACKWARD           15 (to 758)
          
-         314     >>  788 LOAD_FAST                6 (kwargs)
+         325     >>  788 LOAD_FAST                6 (kwargs)
                      790 RETURN_VALUE
          consts
             None
             False
             '='
             1
             0
@@ -1793,27 +1834,27 @@
             'Keyword argument '
             ' cannot be resolved; it will not be parsed as a variable.'
             'Missing required keyword argument '
          names      ('tuple', 'enumerate', 'split', 'len', 'ValueError', 'compile_filter', 'TemplateSyntaxError', 'items')
          varnames   ('parser', 'tokens', 'kwarg_list', 'absolute_tokens', 'optional_tokens', 'had_kwargs', 'kwargs', 'i', 'token', 'split', 'key', 'value', 'kwarg')
          freevars   ()
          cellvars   ()
-         filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\tester\\wagtail_fedit\\templatetags\\fedit.py'
+         filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Packages\\wagtail_fedit\\wagtail_fedit\\templatetags\\fedit.py'
          name       'get_kwargs'
-         firstlineno 264
+         firstlineno 275
          lnotab
             0x02010401040204011c0204011c02040104022a012a014c011401160102
             0204011e023e01260114011601020210012a010c021003080126023c0108
             020801080124ff0203320108010c02
       (None,)
       (None, None, None)
-   names      ('typing', 'Type', 'Any', 'django.template', 'library', 'Node', 'TemplateSyntaxError', 'django.template.context', 'Context', 'django.template.base', 'Parser', 'Token', 'FilterExpression', 'django.http', 'HttpRequest', 'django.utils.html', 'escape', 'django.utils.safestring', 'mark_safe', 'django.urls', 'reverse', 'django.core', 'signing', 'wagtail', 'hooks', 'warnings', 'adapters', 'adapter_registry', 'RegistryLookUpError', 'BaseAdapter', 'AdapterError', 'utils', 'wrap_adapter', '_can_edit', 'FEDIT_PREVIEW_VAR', 'TEMPLATE_TAG_NAME', 'REGISTER_CSS', 'REGISTER_JS', 'Library', 'register', 'WARNING_FIELD_NAME_NOT_AVAILABLE', 'WARNING_MODEL_INSTANCE_NOT_AVAILABLE', 'str', 'as_var', 'AdapterNode', 'tag', 'do_render_fedit', 'simple_tag', 'render_adapter', 'inclusion_tag', 'dict', 'static_hook_output', 'tooltip', 'list', 'get_kwargs')
+   names      ('typing', 'Type', 'Any', 'django.template', 'library', 'Node', 'TemplateSyntaxError', 'django.template.context', 'Context', 'django.template.base', 'Parser', 'Token', 'FilterExpression', 'django.http', 'HttpRequest', 'django.utils.html', 'escape', 'django.utils.safestring', 'mark_safe', 'django.urls', 'reverse', 'django.core', 'signing', 'wagtail', 'hooks', 'wagtail.models', 'Page', 'PAGE_TEMPLATE_VAR', 'warnings', 'adapters', 'adapter_registry', 'RegistryLookUpError', 'BaseAdapter', 'AdapterError', 'utils', 'wrap_adapter', '_can_edit', 'FEDIT_PREVIEW_VAR', 'TEMPLATE_TAG_NAME', 'REGISTER_CSS', 'REGISTER_JS', 'Library', 'register', 'WARNING_FIELD_NAME_NOT_AVAILABLE', 'WARNING_MODEL_INSTANCE_NOT_AVAILABLE', 'str', 'as_var', 'AdapterNode', 'tag', 'do_render_fedit', 'simple_tag', 'render_adapter', 'inclusion_tag', 'dict', 'static_hook_output', 'tooltip', 'list', 'get_kwargs')
    varnames   ()
    freevars   ()
    cellvars   ()
-   filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\tester\\wagtail_fedit\\templatetags\\fedit.py'
+   filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Packages\\wagtail_fedit\\wagtail_fedit\\templatetags\\fedit.py'
    name       '<module>'
    firstlineno 1
    lnotab
-      0x00ff0201100114030c0314040c010c010c010c010c020c020802180618
-      0610061e030401040318071c572a010eff0e0102392a0112ff0e0102122e
-      010aff0e01021d2c0110ff0e01020f
+      0x00ff0201100114030c0314040c010c010c010c010c020c011005080218
+      06180610061e030401040318071c5b2a010eff0e0102392a0112ff0e0102
+      152e010aff0e01021d2c0110ff0e01020f
```

### Comparing `wagtail_fedit-1.5.4rc5/wagtail_fedit/templatetags/fedit.py` & `wagtail_fedit-1.5.4rc6/wagtail_fedit/templatetags/fedit.py`

 * *Files 14% similar despite different names*

```diff
@@ -12,14 +12,18 @@
 from django.http import HttpRequest
 from django.utils.html import escape
 from django.utils.safestring import mark_safe
 from django.urls import reverse
 from django.core import signing
 
 from wagtail import hooks
+from wagtail.models import (
+    Page,
+    PAGE_TEMPLATE_VAR,
+)
 
 import warnings
 
 from ..adapters import (
     adapter_registry,
     RegistryLookUpError,
     BaseAdapter,
@@ -129,14 +133,18 @@
             request=request,
             **kwargs,
         )
 
         if not adapter.check_permissions()\
           or not _can_edit(request, obj):
             context.update(adapter.kwargs)
+
+            if isinstance(obj, Page):
+                context[PAGE_TEMPLATE_VAR] = obj
+
             return as_var(self.as_var, context, adapter.render_content(context))
 
         return as_var(self.as_var, context, wrap_adapter(request, adapter, context))
 
 
 @register.tag(name=TEMPLATE_TAG_NAME)
 def do_render_fedit(parser: Parser, token: Token):
@@ -205,17 +213,20 @@
         del context["parent_context"]
 
     context.update(parent_context)
 
     context["wagtail_fedit_field"]    = adapter.field_name
     context["wagtail_fedit_instance"] = adapter.object
     context["request"]                = adapter.request
-    
+
     context.update(adapter.kwargs)
 
+    if isinstance(adapter.object, Page):
+        context[PAGE_TEMPLATE_VAR] = adapter.object
+
     return adapter.render_content(context)
 
 
 @register.inclusion_tag("wagtail_fedit/_hook_output.html", name="fedit_scripts", takes_context=True)
 def static_hook_output(context, css_or_js) -> dict:
     css_or_js = css_or_js.lower()
```

### Comparing `wagtail_fedit-1.5.4rc5/wagtail_fedit/test/core/migrations/0001_initial.py` & `wagtail_fedit-1.5.4rc6/wagtail_fedit/test/core/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.4rc5/wagtail_fedit/test/core/models.py` & `wagtail_fedit-1.5.4rc6/wagtail_fedit/test/core/models.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.4rc5/wagtail_fedit/test/core/tests/base.py` & `wagtail_fedit-1.5.4rc6/wagtail_fedit/test/core/tests/base.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.4rc5/wagtail_fedit/test/core/tests/test_adapters.py` & `wagtail_fedit-1.5.4rc6/wagtail_fedit/test/core/tests/test_adapters.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.4rc5/wagtail_fedit/test/core/tests/test_block_edit.py` & `wagtail_fedit-1.5.4rc6/wagtail_fedit/test/core/tests/test_block_edit.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.4rc5/wagtail_fedit/test/core/tests/test_blocks.py` & `wagtail_fedit-1.5.4rc6/wagtail_fedit/test/core/tests/test_blocks.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.4rc5/wagtail_fedit/test/core/tests/test_field_edit.py` & `wagtail_fedit-1.5.4rc6/wagtail_fedit/test/core/tests/test_field_edit.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.4rc5/wagtail_fedit/test/core/tests/test_generic.py` & `wagtail_fedit-1.5.4rc6/wagtail_fedit/test/core/tests/test_generic.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.4rc5/wagtail_fedit/test/core/tests/test_model_edit.py` & `wagtail_fedit-1.5.4rc6/wagtail_fedit/test/core/tests/test_model_edit.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.4rc5/wagtail_fedit/test/core/tests/test_revision.py` & `wagtail_fedit-1.5.4rc6/wagtail_fedit/test/core/tests/test_revision.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.4rc5/wagtail_fedit/test/core/tests/test_submit.py` & `wagtail_fedit-1.5.4rc6/wagtail_fedit/test/core/tests/test_submit.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.4rc5/wagtail_fedit/test/manage.py` & `wagtail_fedit-1.5.4rc6/wagtail_fedit/test/manage.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.4rc5/wagtail_fedit/test/testapp/settings.py` & `wagtail_fedit-1.5.4rc6/wagtail_fedit/test/testapp/settings.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.4rc5/wagtail_fedit/test/testapp/urls.py` & `wagtail_fedit-1.5.4rc6/wagtail_fedit/test/testapp/urls.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.4rc5/wagtail_fedit/toolbar.py` & `wagtail_fedit-1.5.4rc6/wagtail_fedit/toolbar.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.4rc5/wagtail_fedit/urls.py` & `wagtail_fedit-1.5.4rc6/wagtail_fedit/urls.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.4rc5/wagtail_fedit/utils.py` & `wagtail_fedit-1.5.4rc6/wagtail_fedit/utils.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.4rc5/wagtail_fedit/views/adapters.py` & `wagtail_fedit-1.5.4rc6/wagtail_fedit/views/adapters.py`

 * *Files 2% similar despite different names*

```diff
@@ -155,37 +155,38 @@
         if "form" in kwargs:
             extra.update(
                 self.adapter.get_form_context(
                     **kwargs,
                 ),
             )
 
+        if isinstance(self.instance, Page):
+            # Add the page template variable to the context.
+            # Wagtail uses this internally; for example in `{% wagtailpagecache %}`
+            extra[PAGE_TEMPLATE_VAR] = self.instance
+
         return super().get_context_data(**kwargs) | {
             "verbose_name": verbose_name,
             "locked_for_user": self.locked_for_user,
             "shared_context": shared_context,
             "form_attrs": self.adapter.get_form_attrs(),
             "locked": self.lock is not None,
             **extra,
         }
     
 class AdapterRefetchView(BaseAdapterView):
     def get(self, request: HttpRequest, *args: Any, **kwargs: Any) -> HttpResponse:
         context = self.get_context_data()
-        if isinstance(self.instance, Page):
-            # Add the page template variable to the context.
-            # Wagtail uses this internally; for example in `{% wagtailpagecache %}`
-            context[PAGE_TEMPLATE_VAR] = self.instance
 
         return JsonResponse({
             "success": True,
             "refetch": True,
             **self.adapter\
               .get_response_data(
-                  self.get_context_data(),
+                  context,
               ),
         })
 
 class EditAdapterView(BaseAdapterView):
     def get(self, request: HttpRequest, *args: Any, **kwargs: Any) -> HttpResponse:
         # Can omit data from context - we are not rendering the content.
         form = self.adapter.get_form()
@@ -217,26 +218,14 @@
                 )
             }, status=423 if self.locked_for_user else 400)
 
         
         self.adapter.form_valid(form)
 
         context = self.get_context_data()
-        if isinstance(self.instance, Page):
-            # Add the page template variable to the context.
-            # Wagtail uses this internally; for example in `{% wagtailpagecache %}`
-            context[PAGE_TEMPLATE_VAR] = self.instance
-
-        ## Render the frame HTML
-        #html = wrap_adapter(
-        #    request=self.request,
-        #    adapter=self.adapter,
-        #    context=context,
-        #    run_context_processors=True,
-        #)
 
         return JsonResponse({
             "success": True,
             **self.adapter\
               .get_response_data(context),
         })
```

### Comparing `wagtail_fedit-1.5.4rc5/wagtail_fedit/views/editable.py` & `wagtail_fedit-1.5.4rc6/wagtail_fedit/views/editable.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.4rc5/wagtail_fedit/views/mixins.py` & `wagtail_fedit-1.5.4rc6/wagtail_fedit/views/mixins.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.4rc5/wagtail_fedit/wagtail_hooks/action_menu.py` & `wagtail_fedit-1.5.4rc6/wagtail_fedit/wagtail_hooks/action_menu.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.4rc5/wagtail_fedit/wagtail_hooks/adapter_hooks.py` & `wagtail_fedit-1.5.4rc6/wagtail_fedit/wagtail_hooks/adapter_hooks.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.4rc5/wagtail_fedit/wagtail_hooks/log_actions.py` & `wagtail_fedit-1.5.4rc6/wagtail_fedit/wagtail_hooks/log_actions.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.4rc5/wagtail_fedit/wagtail_hooks/userbar.py` & `wagtail_fedit-1.5.4rc6/wagtail_fedit/wagtail_hooks/userbar.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.4rc5/wagtail_fedit.egg-info/PKG-INFO` & `wagtail_fedit-1.5.4rc6/wagtail_fedit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wagtail-fedit
-Version: 1.5.4rc5
+Version: 1.5.4rc6
 Summary: Frontend editing for your Wagtail site
 Home-page: https://github.com/Nigel2392/wagtail_fedit
 Author: Nigel
 Author-email: nigel@goodadvice.it
 License: GPL-2.0-only
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: wagtail-fedit Version: 1.5.4rc5 Summary: Frontend
+Metadata-Version: 2.1 Name: wagtail-fedit Version: 1.5.4rc6 Summary: Frontend
 editing for your Wagtail site Home-page: https://github.com/Nigel2392/
 wagtail_fedit Author: Nigel Author-email: nigel@goodadvice.it License: GPL-2.0-
 only Classifier: Environment :: Web Environment Classifier: Framework :: Django
 Classifier: Framework :: Django :: 4.2 Classifier: Framework :: Wagtail
 Classifier: Framework :: Wagtail :: 5 Classifier: Framework :: Wagtail :: 6
 Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
 :: GNU General Public License v2 or later (GPLv2+) Classifier: Operating System
```

### Comparing `wagtail_fedit-1.5.4rc5/wagtail_fedit.egg-info/SOURCES.txt` & `wagtail_fedit-1.5.4rc6/wagtail_fedit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

