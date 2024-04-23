# Comparing `tmp/wagtail_fedit-1.5.4rc2.tar.gz` & `tmp/wagtail_fedit-1.5.4rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wagtail_fedit-1.5.4rc2.tar", last modified: Tue Apr 23 16:04:54 2024, max compression
+gzip compressed data, was "wagtail_fedit-1.5.4rc3.tar", last modified: Tue Apr 23 18:10:30 2024, max compression
```

## Comparing `wagtail_fedit-1.5.4rc2.tar` & `wagtail_fedit-1.5.4rc3.tar`

### file list

```diff
@@ -1,137 +1,137 @@
-drwxrwxrwx   0        0        0        0 2024-04-23 16:04:54.816361 wagtail_fedit-1.5.4rc2/
--rw-rw-rw-   0        0        0    18429 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.4rc2/LICENSE
--rw-rw-rw-   0        0        0      257 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.4rc2/MANIFEST.in
--rw-rw-rw-   0        0        0    21651 2024-04-23 16:04:54.816361 wagtail_fedit-1.5.4rc2/PKG-INFO
--rw-rw-rw-   0        0        0    20450 2024-04-23 11:23:03.000000 wagtail_fedit-1.5.4rc2/README.md
--rw-rw-rw-   0        0        0       90 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.4rc2/pyproject.toml
--rw-rw-rw-   0        0        0     1189 2024-04-23 16:04:54.829459 wagtail_fedit-1.5.4rc2/setup.cfg
--rw-rw-rw-   0        0        0       39 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.4rc2/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-23 16:04:54.643523 wagtail_fedit-1.5.4rc2/wagtail_fedit/
--rw-rw-rw-   0        0        0        0 2024-03-29 20:13:25.000000 wagtail_fedit-1.5.4rc2/wagtail_fedit/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-23 16:04:54.682786 wagtail_fedit-1.5.4rc2/wagtail_fedit/adapters/
--rw-rw-rw-   0        0        0      532 2024-04-22 21:01:35.000000 wagtail_fedit-1.5.4rc2/wagtail_fedit/adapters/__init__.py
--rw-rw-rw-   0        0        0    14330 2024-04-23 15:34:38.000000 wagtail_fedit-1.5.4rc2/wagtail_fedit/adapters/base.py
--rw-rw-rw-   0        0        0     6408 2024-04-23 15:37:06.000000 wagtail_fedit-1.5.4rc2/wagtail_fedit/adapters/block.py
--rw-rw-rw-   0        0        0     8508 2024-04-23 15:38:57.000000 wagtail_fedit-1.5.4rc2/wagtail_fedit/adapters/field.py
--rw-rw-rw-   0        0        0     2671 2024-04-22 20:52:19.000000 wagtail_fedit-1.5.4rc2/wagtail_fedit/adapters/funcs.py
--rw-rw-rw-   0        0        0     2739 2024-04-23 14:30:53.000000 wagtail_fedit-1.5.4rc2/wagtail_fedit/adapters/misc.py
--rw-rw-rw-   0        0        0     4632 2024-04-23 15:46:14.000000 wagtail_fedit-1.5.4rc2/wagtail_fedit/adapters/models.py
--rw-rw-rw-   0        0        0     1595 2024-04-18 20:22:37.000000 wagtail_fedit-1.5.4rc2/wagtail_fedit/adapters/registry.py
--rw-rw-rw-   0        0        0      163 2024-03-29 20:13:25.000000 wagtail_fedit-1.5.4rc2/wagtail_fedit/apps.py
-drwxrwxrwx   0        0        0        0 2024-04-23 16:04:54.684785 wagtail_fedit-1.5.4rc2/wagtail_fedit/forms/
--rw-rw-rw-   0        0        0      215 2024-04-23 13:02:23.000000 wagtail_fedit-1.5.4rc2/wagtail_fedit/forms/__init__.py
--rw-rw-rw-   0        0        0     2881 2024-04-18 20:27:35.000000 wagtail_fedit-1.5.4rc2/wagtail_fedit/forms/blocks.py
--rw-rw-rw-   0        0        0     3269 2024-04-23 13:28:56.000000 wagtail_fedit-1.5.4rc2/wagtail_fedit/forms/fields.py
--rw-rw-rw-   0        0        0     4617 2024-04-21 02:08:33.000000 wagtail_fedit-1.5.4rc2/wagtail_fedit/hooks.py
-drwxrwxrwx   0        0        0        0 2024-04-23 16:04:54.614603 wagtail_fedit-1.5.4rc2/wagtail_fedit/locale/
-drwxrwxrwx   0        0        0        0 2024-04-23 16:04:54.614603 wagtail_fedit-1.5.4rc2/wagtail_fedit/locale/nl/
-drwxrwxrwx   0        0        0        0 2024-04-23 16:04:54.685250 wagtail_fedit-1.5.4rc2/wagtail_fedit/locale/nl/LC_MESSAGES/
--rw-rw-rw-   0        0        0     7262 2024-04-23 15:50:58.000000 wagtail_fedit-1.5.4rc2/wagtail_fedit/locale/nl/LC_MESSAGES/django.mo
--rw-rw-rw-   0        0        0    13018 2024-04-23 15:50:49.000000 wagtail_fedit-1.5.4rc2/wagtail_fedit/locale/nl/LC_MESSAGES/django.po
-drwxrwxrwx   0        0        0        0 2024-04-23 16:04:54.685250 wagtail_fedit-1.5.4rc2/wagtail_fedit/migrations/
--rw-rw-rw-   0        0        0        0 2024-03-29 20:13:25.000000 wagtail_fedit-1.5.4rc2/wagtail_fedit/migrations/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-23 16:04:54.688137 wagtail_fedit-1.5.4rc2/wagtail_fedit/migrations/__pycache__/
--rw-rw-rw-   0        0        0      215 2024-03-29 21:05:00.000000 wagtail_fedit-1.5.4rc2/wagtail_fedit/migrations/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0        0        0     3170 2024-04-05 20:30:10.000000 wagtail_fedit-1.5.4rc2/wagtail_fedit/models.py
--rw-rw-rw-   0        0        0     1585 2024-04-23 15:56:07.000000 wagtail_fedit-1.5.4rc2/wagtail_fedit/settings.py
-drwxrwxrwx   0        0        0        0 2024-04-23 16:04:54.615718 wagtail_fedit-1.5.4rc2/wagtail_fedit/static/
-drwxrwxrwx   0        0        0        0 2024-04-23 16:04:54.615718 wagtail_fedit-1.5.4rc2/wagtail_fedit/static/wagtail_fedit/
-drwxrwxrwx   0        0        0        0 2024-04-23 16:04:54.691148 wagtail_fedit-1.5.4rc2/wagtail_fedit/static/wagtail_fedit/css/
--rw-rw-rw-   0        0        0     5750 2024-04-23 15:45:28.000000 wagtail_fedit-1.5.4rc2/wagtail_fedit/static/wagtail_fedit/css/frontend.css
--rw-rw-rw-   0        0        0     5098 2024-04-17 20:40:49.000000 wagtail_fedit-1.5.4rc2/wagtail_fedit/static/wagtail_fedit/css/furniture.css
--rw-rw-rw-   0        0        0     1266 2024-04-05 19:37:44.000000 wagtail_fedit-1.5.4rc2/wagtail_fedit/static/wagtail_fedit/css/userbar-menu.css
-drwxrwxrwx   0        0        0        0 2024-04-23 16:04:54.714475 wagtail_fedit-1.5.4rc2/wagtail_fedit/static/wagtail_fedit/js/
--rw-rw-rw-   0        0        0    21429 2024-04-23 15:58:28.000000 wagtail_fedit-1.5.4rc2/wagtail_fedit/static/wagtail_fedit/js/frontend.js
-drwxrwxrwx   0        0        0        0 2024-04-23 16:04:54.615718 wagtail_fedit-1.5.4rc2/wagtail_fedit/static/wagtail_fedit/vendor/
-drwxrwxrwx   0        0        0        0 2024-04-23 16:04:54.722605 wagtail_fedit-1.5.4rc2/wagtail_fedit/static/wagtail_fedit/vendor/tippy/
--rw-rw-rw-   0        0        0     1091 2024-04-23 15:39:19.000000 wagtail_fedit-1.5.4rc2/wagtail_fedit/static/wagtail_fedit/vendor/tippy/LICENSE
--rw-rw-rw-   0        0        0    20122 2024-04-23 14:51:23.000000 wagtail_fedit-1.5.4rc2/wagtail_fedit/static/wagtail_fedit/vendor/tippy/popper.min.js
--rw-rw-rw-   0        0        0    25717 2024-04-23 14:51:31.000000 wagtail_fedit-1.5.4rc2/wagtail_fedit/static/wagtail_fedit/vendor/tippy/tippy-bundle.min.js
-drwxrwxrwx   0        0        0        0 2024-04-23 16:04:54.618834 wagtail_fedit-1.5.4rc2/wagtail_fedit/templates/
-drwxrwxrwx   0        0        0        0 2024-04-23 16:04:54.723605 wagtail_fedit-1.5.4rc2/wagtail_fedit/templates/wagtail_fedit/
--rw-rw-rw-   0        0        0       56 2024-04-16 18:37:39.000000 wagtail_fedit-1.5.4rc2/wagtail_fedit/templates/wagtail_fedit/_hook_output.html
-drwxrwxrwx   0        0        0        0 2024-04-23 16:04:54.725603 wagtail_fedit-1.5.4rc2/wagtail_fedit/templates/wagtail_fedit/content/
-drwxrwxrwx   0        0        0        0 2024-04-23 16:04:54.728176 wagtail_fedit-1.5.4rc2/wagtail_fedit/templates/wagtail_fedit/content/buttons/
--rw-rw-rw-   0        0        0      929 2024-04-23 15:23:24.000000 wagtail_fedit-1.5.4rc2/wagtail_fedit/templates/wagtail_fedit/content/buttons/admin_link.html
--rw-rw-rw-   0        0        0      991 2024-04-23 15:27:54.000000 wagtail_fedit-1.5.4rc2/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_adapter.html
--rw-rw-rw-   0        0        0      534 2024-04-21 17:21:38.000000 wagtail_fedit-1.5.4rc2/wagtail_fedit/templates/wagtail_fedit/content/editable_adapter.html
-drwxrwxrwx   0        0        0        0 2024-04-23 16:04:54.737094 wagtail_fedit-1.5.4rc2/wagtail_fedit/templates/wagtail_fedit/editor/
--rw-rw-rw-   0        0        0     2259 2024-04-11 08:02:26.000000 wagtail_fedit-1.5.4rc2/wagtail_fedit/templates/wagtail_fedit/editor/action_confirm.html
--rw-rw-rw-   0        0        0     3699 2024-04-20 21:55:10.000000 wagtail_fedit-1.5.4rc2/wagtail_fedit/templates/wagtail_fedit/editor/action_publish_confirm.html
--rw-rw-rw-   0        0        0      266 2024-04-21 21:15:09.000000 wagtail_fedit-1.5.4rc2/wagtail_fedit/templates/wagtail_fedit/editor/adapter_edit_handler.html
--rw-rw-rw-   0        0        0      265 2024-04-21 21:23:24.000000 wagtail_fedit-1.5.4rc2/wagtail_fedit/templates/wagtail_fedit/editor/adapter_edit_handler_form.html
--rw-rw-rw-   0        0        0      555 2024-04-21 21:13:45.000000 wagtail_fedit-1.5.4rc2/wagtail_fedit/templates/wagtail_fedit/editor/adapter_form.html
--rw-rw-rw-   0        0        0      455 2024-04-21 00:11:35.000000 wagtail_fedit-1.5.4rc2/wagtail_fedit/templates/wagtail_fedit/editor/adapter_form_errors.html
--rw-rw-rw-   0        0        0      330 2024-04-21 00:12:14.000000 wagtail_fedit-1.5.4rc2/wagtail_fedit/templates/wagtail_fedit/editor/adapter_iframe.html
--rw-rw-rw-   0        0        0     5271 2024-04-21 00:11:24.000000 wagtail_fedit-1.5.4rc2/wagtail_fedit/templates/wagtail_fedit/editor/base_iframe.html
--rw-rw-rw-   0        0        0      496 2024-04-02 17:46:59.000000 wagtail_fedit-1.5.4rc2/wagtail_fedit/templates/wagtail_fedit/editor/field.html
-drwxrwxrwx   0        0        0        0 2024-04-23 16:04:54.743104 wagtail_fedit-1.5.4rc2/wagtail_fedit/templates/wagtail_fedit/icons/
--rw-rw-rw-   0        0        0      797 2024-04-11 08:36:19.000000 wagtail_fedit-1.5.4rc2/wagtail_fedit/templates/wagtail_fedit/icons/fedit-check-list.svg
--rw-rw-rw-   0        0        0      584 2024-04-11 08:36:55.000000 wagtail_fedit-1.5.4rc2/wagtail_fedit/templates/wagtail_fedit/icons/fedit-eye-closed.svg
--rw-rw-rw-   0        0        0      377 2024-04-11 08:23:07.000000 wagtail_fedit-1.5.4rc2/wagtail_fedit/templates/wagtail_fedit/icons/fedit-eye-open.svg
--rw-rw-rw-   0        0        0      725 2024-04-11 09:02:58.000000 wagtail_fedit-1.5.4rc2/wagtail_fedit/templates/wagtail_fedit/icons/fedit-save.svg
--rw-rw-rw-   0        0        0     1323 2024-04-11 08:36:52.000000 wagtail_fedit-1.5.4rc2/wagtail_fedit/templates/wagtail_fedit/icons/fedit-stop-sign.svg
-drwxrwxrwx   0        0        0        0 2024-04-23 16:04:54.743104 wagtail_fedit-1.5.4rc2/wagtail_fedit/templates/wagtail_fedit/userbar/
--rw-rw-rw-   0        0        0      867 2024-04-03 17:05:21.000000 wagtail_fedit-1.5.4rc2/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit.html
--rw-rw-rw-   0        0        0      876 2024-04-03 16:59:31.000000 wagtail_fedit-1.5.4rc2/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_view_live.html
-drwxrwxrwx   0        0        0        0 2024-04-23 16:04:54.743104 wagtail_fedit-1.5.4rc2/wagtail_fedit/templates/wagtail_fedit/userbar/publish/
--rw-rw-rw-   0        0        0      263 2024-04-11 08:24:35.000000 wagtail_fedit-1.5.4rc2/wagtail_fedit/templates/wagtail_fedit/userbar/publish/action_button.html
--rw-rw-rw-   0        0        0      967 2024-04-11 09:03:51.000000 wagtail_fedit-1.5.4rc2/wagtail_fedit/templates/wagtail_fedit/userbar/publish/item_fedit_publishing.html
-drwxrwxrwx   0        0        0        0 2024-04-23 16:04:54.749576 wagtail_fedit-1.5.4rc2/wagtail_fedit/templatetags/
--rw-rw-rw-   0        0        0        0 2024-03-29 20:13:42.000000 wagtail_fedit-1.5.4rc2/wagtail_fedit/templatetags/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-23 16:04:54.751579 wagtail_fedit-1.5.4rc2/wagtail_fedit/templatetags/__pycache__/
--rw-rw-rw-   0        0        0      217 2024-03-29 21:05:00.000000 wagtail_fedit-1.5.4rc2/wagtail_fedit/templatetags/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0        0        0    12420 2024-04-23 15:25:11.000000 wagtail_fedit-1.5.4rc2/wagtail_fedit/templatetags/__pycache__/fedit.cpython-311.pyc
--rw-rw-rw-   0        0        0     9470 2024-04-23 15:25:09.000000 wagtail_fedit-1.5.4rc2/wagtail_fedit/templatetags/fedit.py
-drwxrwxrwx   0        0        0        0 2024-04-23 16:04:54.752576 wagtail_fedit-1.5.4rc2/wagtail_fedit/test/
--rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.4rc2/wagtail_fedit/test/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-23 16:04:54.757794 wagtail_fedit-1.5.4rc2/wagtail_fedit/test/core/
--rw-rw-rw-   0        0        0      151 2024-04-05 07:59:49.000000 wagtail_fedit-1.5.4rc2/wagtail_fedit/test/core/__init__.py
--rw-rw-rw-   0        0        0      165 2024-04-05 08:41:40.000000 wagtail_fedit-1.5.4rc2/wagtail_fedit/test/core/apps.py
--rw-rw-rw-   0        0        0      130 2024-04-15 20:12:38.000000 wagtail_fedit-1.5.4rc2/wagtail_fedit/test/core/context_processors.py
-drwxrwxrwx   0        0        0        0 2024-04-23 16:04:54.762575 wagtail_fedit-1.5.4rc2/wagtail_fedit/test/core/migrations/
--rw-rw-rw-   0        0        0    12115 2024-04-20 22:33:35.000000 wagtail_fedit-1.5.4rc2/wagtail_fedit/test/core/migrations/0001_initial.py
--rw-rw-rw-   0        0        0      509 2024-04-21 18:41:55.000000 wagtail_fedit-1.5.4rc2/wagtail_fedit/test/core/migrations/0002_basicmodel_related_field.py
--rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.4rc2/wagtail_fedit/test/core/migrations/__init__.py
--rw-rw-rw-   0        0        0     6047 2024-04-23 13:09:46.000000 wagtail_fedit-1.5.4rc2/wagtail_fedit/test/core/models.py
-drwxrwxrwx   0        0        0        0 2024-04-23 16:04:54.772820 wagtail_fedit-1.5.4rc2/wagtail_fedit/test/core/tests/
--rw-rw-rw-   0        0        0        0 2024-04-05 07:59:29.000000 wagtail_fedit-1.5.4rc2/wagtail_fedit/test/core/tests/__init__.py
--rw-rw-rw-   0        0        0     8475 2024-04-23 13:35:29.000000 wagtail_fedit-1.5.4rc2/wagtail_fedit/test/core/tests/base.py
--rw-rw-rw-   0        0        0    22637 2024-04-23 12:36:52.000000 wagtail_fedit-1.5.4rc2/wagtail_fedit/test/core/tests/test_adapters.py
--rw-rw-rw-   0        0        0     4320 2024-04-06 22:44:26.000000 wagtail_fedit-1.5.4rc2/wagtail_fedit/test/core/tests/test_block_edit.py
--rw-rw-rw-   0        0        0     5664 2024-04-05 10:31:29.000000 wagtail_fedit-1.5.4rc2/wagtail_fedit/test/core/tests/test_blocks.py
--rw-rw-rw-   0        0        0     3642 2024-04-05 18:00:23.000000 wagtail_fedit-1.5.4rc2/wagtail_fedit/test/core/tests/test_field_edit.py
--rw-rw-rw-   0        0        0     3709 2024-04-10 13:03:30.000000 wagtail_fedit-1.5.4rc2/wagtail_fedit/test/core/tests/test_generic.py
--rw-rw-rw-   0        0        0     4865 2024-04-23 14:23:09.000000 wagtail_fedit-1.5.4rc2/wagtail_fedit/test/core/tests/test_model_edit.py
--rw-rw-rw-   0        0        0     1574 2024-04-20 20:49:12.000000 wagtail_fedit-1.5.4rc2/wagtail_fedit/test/core/tests/test_revision.py
--rw-rw-rw-   0        0        0     9545 2024-04-20 21:54:40.000000 wagtail_fedit-1.5.4rc2/wagtail_fedit/test/core/tests/test_submit.py
--rw-rw-rw-   0        0        0      704 2024-04-05 17:55:36.000000 wagtail_fedit-1.5.4rc2/wagtail_fedit/test/manage.py
-drwxrwxrwx   0        0        0        0 2024-04-23 16:04:54.776961 wagtail_fedit-1.5.4rc2/wagtail_fedit/test/testapp/
--rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.4rc2/wagtail_fedit/test/testapp/__init__.py
--rw-rw-rw-   0        0        0      407 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.4rc2/wagtail_fedit/test/testapp/asgi.py
--rw-rw-rw-   0        0        0     3625 2024-04-15 20:14:41.000000 wagtail_fedit-1.5.4rc2/wagtail_fedit/test/testapp/settings.py
--rw-rw-rw-   0        0        0      897 2024-04-05 08:04:53.000000 wagtail_fedit-1.5.4rc2/wagtail_fedit/test/testapp/urls.py
--rw-rw-rw-   0        0        0      407 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.4rc2/wagtail_fedit/test/testapp/wsgi.py
--rw-rw-rw-   0        0        0     2220 2024-04-23 14:21:34.000000 wagtail_fedit-1.5.4rc2/wagtail_fedit/toolbar.py
--rw-rw-rw-   0        0        0      934 2024-04-21 16:55:23.000000 wagtail_fedit-1.5.4rc2/wagtail_fedit/urls.py
--rw-rw-rw-   0        0        0    17111 2024-04-23 15:38:05.000000 wagtail_fedit-1.5.4rc2/wagtail_fedit/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-23 16:04:54.783038 wagtail_fedit-1.5.4rc2/wagtail_fedit/views/
--rw-rw-rw-   0        0        0      190 2024-04-13 19:36:44.000000 wagtail_fedit-1.5.4rc2/wagtail_fedit/views/__init__.py
--rw-rw-rw-   0        0        0     7220 2024-04-23 13:39:08.000000 wagtail_fedit-1.5.4rc2/wagtail_fedit/views/adapters.py
--rw-rw-rw-   0        0        0    17563 2024-04-21 20:25:17.000000 wagtail_fedit-1.5.4rc2/wagtail_fedit/views/editable.py
--rw-rw-rw-   0        0        0     1923 2024-04-21 20:29:01.000000 wagtail_fedit-1.5.4rc2/wagtail_fedit/views/mixins.py
-drwxrwxrwx   0        0        0        0 2024-04-23 16:04:54.816361 wagtail_fedit-1.5.4rc2/wagtail_fedit/wagtail_hooks/
--rw-rw-rw-   0        0        0      184 2024-04-16 10:03:02.000000 wagtail_fedit-1.5.4rc2/wagtail_fedit/wagtail_hooks/__init__.py
--rw-rw-rw-   0        0        0     1748 2024-04-06 18:37:13.000000 wagtail_fedit-1.5.4rc2/wagtail_fedit/wagtail_hooks/action_menu.py
--rw-rw-rw-   0        0        0     2857 2024-04-23 15:56:51.000000 wagtail_fedit-1.5.4rc2/wagtail_fedit/wagtail_hooks/adapter_hooks.py
--rw-rw-rw-   0        0        0      328 2024-04-21 16:44:33.000000 wagtail_fedit-1.5.4rc2/wagtail_fedit/wagtail_hooks/adapter_registry.py
--rw-rw-rw-   0        0        0      398 2024-04-11 09:03:10.000000 wagtail_fedit-1.5.4rc2/wagtail_fedit/wagtail_hooks/icons.py
--rw-rw-rw-   0        0        0     2573 2024-04-11 07:39:50.000000 wagtail_fedit-1.5.4rc2/wagtail_fedit/wagtail_hooks/log_actions.py
--rw-rw-rw-   0        0        0      340 2024-03-30 17:10:05.000000 wagtail_fedit-1.5.4rc2/wagtail_fedit/wagtail_hooks/urls.py
--rw-rw-rw-   0        0        0     7630 2024-04-19 20:11:56.000000 wagtail_fedit-1.5.4rc2/wagtail_fedit/wagtail_hooks/userbar.py
-drwxrwxrwx   0        0        0        0 2024-04-23 16:04:54.673377 wagtail_fedit-1.5.4rc2/wagtail_fedit.egg-info/
--rw-rw-rw-   0        0        0    21651 2024-04-23 16:04:54.000000 wagtail_fedit-1.5.4rc2/wagtail_fedit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     4521 2024-04-23 16:04:54.000000 wagtail_fedit-1.5.4rc2/wagtail_fedit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-23 16:04:54.000000 wagtail_fedit-1.5.4rc2/wagtail_fedit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2024-04-23 16:04:54.000000 wagtail_fedit-1.5.4rc2/wagtail_fedit.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-04-23 16:04:54.000000 wagtail_fedit-1.5.4rc2/wagtail_fedit.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-23 18:10:30.622337 wagtail_fedit-1.5.4rc3/
+-rw-rw-rw-   0        0        0    18429 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.4rc3/LICENSE
+-rw-rw-rw-   0        0        0      257 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.4rc3/MANIFEST.in
+-rw-rw-rw-   0        0        0    21651 2024-04-23 18:10:30.622337 wagtail_fedit-1.5.4rc3/PKG-INFO
+-rw-rw-rw-   0        0        0    20450 2024-04-23 11:23:03.000000 wagtail_fedit-1.5.4rc3/README.md
+-rw-rw-rw-   0        0        0       90 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.4rc3/pyproject.toml
+-rw-rw-rw-   0        0        0     1189 2024-04-23 18:10:30.632336 wagtail_fedit-1.5.4rc3/setup.cfg
+-rw-rw-rw-   0        0        0       39 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.4rc3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-23 18:10:30.211527 wagtail_fedit-1.5.4rc3/wagtail_fedit/
+-rw-rw-rw-   0        0        0        0 2024-03-29 20:13:25.000000 wagtail_fedit-1.5.4rc3/wagtail_fedit/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-23 18:10:30.304101 wagtail_fedit-1.5.4rc3/wagtail_fedit/adapters/
+-rw-rw-rw-   0        0        0      532 2024-04-22 21:01:35.000000 wagtail_fedit-1.5.4rc3/wagtail_fedit/adapters/__init__.py
+-rw-rw-rw-   0        0        0    14330 2024-04-23 15:34:38.000000 wagtail_fedit-1.5.4rc3/wagtail_fedit/adapters/base.py
+-rw-rw-rw-   0        0        0     6408 2024-04-23 15:37:06.000000 wagtail_fedit-1.5.4rc3/wagtail_fedit/adapters/block.py
+-rw-rw-rw-   0        0        0     8661 2024-04-23 18:05:30.000000 wagtail_fedit-1.5.4rc3/wagtail_fedit/adapters/field.py
+-rw-rw-rw-   0        0        0     2671 2024-04-22 20:52:19.000000 wagtail_fedit-1.5.4rc3/wagtail_fedit/adapters/funcs.py
+-rw-rw-rw-   0        0        0     2739 2024-04-23 14:30:53.000000 wagtail_fedit-1.5.4rc3/wagtail_fedit/adapters/misc.py
+-rw-rw-rw-   0        0        0     4632 2024-04-23 15:46:14.000000 wagtail_fedit-1.5.4rc3/wagtail_fedit/adapters/models.py
+-rw-rw-rw-   0        0        0     1595 2024-04-18 20:22:37.000000 wagtail_fedit-1.5.4rc3/wagtail_fedit/adapters/registry.py
+-rw-rw-rw-   0        0        0      163 2024-03-29 20:13:25.000000 wagtail_fedit-1.5.4rc3/wagtail_fedit/apps.py
+drwxrwxrwx   0        0        0        0 2024-04-23 18:10:30.308102 wagtail_fedit-1.5.4rc3/wagtail_fedit/forms/
+-rw-rw-rw-   0        0        0      215 2024-04-23 13:02:23.000000 wagtail_fedit-1.5.4rc3/wagtail_fedit/forms/__init__.py
+-rw-rw-rw-   0        0        0     2881 2024-04-18 20:27:35.000000 wagtail_fedit-1.5.4rc3/wagtail_fedit/forms/blocks.py
+-rw-rw-rw-   0        0        0     3269 2024-04-23 13:28:56.000000 wagtail_fedit-1.5.4rc3/wagtail_fedit/forms/fields.py
+-rw-rw-rw-   0        0        0     4617 2024-04-21 02:08:33.000000 wagtail_fedit-1.5.4rc3/wagtail_fedit/hooks.py
+drwxrwxrwx   0        0        0        0 2024-04-23 18:10:30.147585 wagtail_fedit-1.5.4rc3/wagtail_fedit/locale/
+drwxrwxrwx   0        0        0        0 2024-04-23 18:10:30.148296 wagtail_fedit-1.5.4rc3/wagtail_fedit/locale/nl/
+drwxrwxrwx   0        0        0        0 2024-04-23 18:10:30.326102 wagtail_fedit-1.5.4rc3/wagtail_fedit/locale/nl/LC_MESSAGES/
+-rw-rw-rw-   0        0        0     7262 2024-04-23 15:50:58.000000 wagtail_fedit-1.5.4rc3/wagtail_fedit/locale/nl/LC_MESSAGES/django.mo
+-rw-rw-rw-   0        0        0    13018 2024-04-23 15:50:49.000000 wagtail_fedit-1.5.4rc3/wagtail_fedit/locale/nl/LC_MESSAGES/django.po
+drwxrwxrwx   0        0        0        0 2024-04-23 18:10:30.328107 wagtail_fedit-1.5.4rc3/wagtail_fedit/migrations/
+-rw-rw-rw-   0        0        0        0 2024-03-29 20:13:25.000000 wagtail_fedit-1.5.4rc3/wagtail_fedit/migrations/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-23 18:10:30.330107 wagtail_fedit-1.5.4rc3/wagtail_fedit/migrations/__pycache__/
+-rw-rw-rw-   0        0        0      215 2024-03-29 21:05:00.000000 wagtail_fedit-1.5.4rc3/wagtail_fedit/migrations/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0     3170 2024-04-05 20:30:10.000000 wagtail_fedit-1.5.4rc3/wagtail_fedit/models.py
+-rw-rw-rw-   0        0        0     1585 2024-04-23 15:56:07.000000 wagtail_fedit-1.5.4rc3/wagtail_fedit/settings.py
+drwxrwxrwx   0        0        0        0 2024-04-23 18:10:30.150711 wagtail_fedit-1.5.4rc3/wagtail_fedit/static/
+drwxrwxrwx   0        0        0        0 2024-04-23 18:10:30.151717 wagtail_fedit-1.5.4rc3/wagtail_fedit/static/wagtail_fedit/
+drwxrwxrwx   0        0        0        0 2024-04-23 18:10:30.336975 wagtail_fedit-1.5.4rc3/wagtail_fedit/static/wagtail_fedit/css/
+-rw-rw-rw-   0        0        0     5750 2024-04-23 15:45:28.000000 wagtail_fedit-1.5.4rc3/wagtail_fedit/static/wagtail_fedit/css/frontend.css
+-rw-rw-rw-   0        0        0     5098 2024-04-17 20:40:49.000000 wagtail_fedit-1.5.4rc3/wagtail_fedit/static/wagtail_fedit/css/furniture.css
+-rw-rw-rw-   0        0        0     1266 2024-04-05 19:37:44.000000 wagtail_fedit-1.5.4rc3/wagtail_fedit/static/wagtail_fedit/css/userbar-menu.css
+drwxrwxrwx   0        0        0        0 2024-04-23 18:10:30.338969 wagtail_fedit-1.5.4rc3/wagtail_fedit/static/wagtail_fedit/js/
+-rw-rw-rw-   0        0        0    22454 2024-04-23 18:08:58.000000 wagtail_fedit-1.5.4rc3/wagtail_fedit/static/wagtail_fedit/js/frontend.js
+drwxrwxrwx   0        0        0        0 2024-04-23 18:10:30.151717 wagtail_fedit-1.5.4rc3/wagtail_fedit/static/wagtail_fedit/vendor/
+drwxrwxrwx   0        0        0        0 2024-04-23 18:10:30.444696 wagtail_fedit-1.5.4rc3/wagtail_fedit/static/wagtail_fedit/vendor/tippy/
+-rw-rw-rw-   0        0        0     1091 2024-04-23 15:39:19.000000 wagtail_fedit-1.5.4rc3/wagtail_fedit/static/wagtail_fedit/vendor/tippy/LICENSE
+-rw-rw-rw-   0        0        0    20122 2024-04-23 14:51:23.000000 wagtail_fedit-1.5.4rc3/wagtail_fedit/static/wagtail_fedit/vendor/tippy/popper.min.js
+-rw-rw-rw-   0        0        0    25717 2024-04-23 14:51:31.000000 wagtail_fedit-1.5.4rc3/wagtail_fedit/static/wagtail_fedit/vendor/tippy/tippy-bundle.min.js
+drwxrwxrwx   0        0        0        0 2024-04-23 18:10:30.152711 wagtail_fedit-1.5.4rc3/wagtail_fedit/templates/
+drwxrwxrwx   0        0        0        0 2024-04-23 18:10:30.447689 wagtail_fedit-1.5.4rc3/wagtail_fedit/templates/wagtail_fedit/
+-rw-rw-rw-   0        0        0       56 2024-04-16 18:37:39.000000 wagtail_fedit-1.5.4rc3/wagtail_fedit/templates/wagtail_fedit/_hook_output.html
+drwxrwxrwx   0        0        0        0 2024-04-23 18:10:30.449930 wagtail_fedit-1.5.4rc3/wagtail_fedit/templates/wagtail_fedit/content/
+drwxrwxrwx   0        0        0        0 2024-04-23 18:10:30.453033 wagtail_fedit-1.5.4rc3/wagtail_fedit/templates/wagtail_fedit/content/buttons/
+-rw-rw-rw-   0        0        0      929 2024-04-23 15:23:24.000000 wagtail_fedit-1.5.4rc3/wagtail_fedit/templates/wagtail_fedit/content/buttons/admin_link.html
+-rw-rw-rw-   0        0        0      991 2024-04-23 15:27:54.000000 wagtail_fedit-1.5.4rc3/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_adapter.html
+-rw-rw-rw-   0        0        0      571 2024-04-23 17:34:21.000000 wagtail_fedit-1.5.4rc3/wagtail_fedit/templates/wagtail_fedit/content/editable_adapter.html
+drwxrwxrwx   0        0        0        0 2024-04-23 18:10:30.498084 wagtail_fedit-1.5.4rc3/wagtail_fedit/templates/wagtail_fedit/editor/
+-rw-rw-rw-   0        0        0     2259 2024-04-11 08:02:26.000000 wagtail_fedit-1.5.4rc3/wagtail_fedit/templates/wagtail_fedit/editor/action_confirm.html
+-rw-rw-rw-   0        0        0     3699 2024-04-20 21:55:10.000000 wagtail_fedit-1.5.4rc3/wagtail_fedit/templates/wagtail_fedit/editor/action_publish_confirm.html
+-rw-rw-rw-   0        0        0      266 2024-04-21 21:15:09.000000 wagtail_fedit-1.5.4rc3/wagtail_fedit/templates/wagtail_fedit/editor/adapter_edit_handler.html
+-rw-rw-rw-   0        0        0      265 2024-04-21 21:23:24.000000 wagtail_fedit-1.5.4rc3/wagtail_fedit/templates/wagtail_fedit/editor/adapter_edit_handler_form.html
+-rw-rw-rw-   0        0        0      555 2024-04-21 21:13:45.000000 wagtail_fedit-1.5.4rc3/wagtail_fedit/templates/wagtail_fedit/editor/adapter_form.html
+-rw-rw-rw-   0        0        0      455 2024-04-21 00:11:35.000000 wagtail_fedit-1.5.4rc3/wagtail_fedit/templates/wagtail_fedit/editor/adapter_form_errors.html
+-rw-rw-rw-   0        0        0      330 2024-04-21 00:12:14.000000 wagtail_fedit-1.5.4rc3/wagtail_fedit/templates/wagtail_fedit/editor/adapter_iframe.html
+-rw-rw-rw-   0        0        0     5271 2024-04-21 00:11:24.000000 wagtail_fedit-1.5.4rc3/wagtail_fedit/templates/wagtail_fedit/editor/base_iframe.html
+-rw-rw-rw-   0        0        0      496 2024-04-02 17:46:59.000000 wagtail_fedit-1.5.4rc3/wagtail_fedit/templates/wagtail_fedit/editor/field.html
+drwxrwxrwx   0        0        0        0 2024-04-23 18:10:30.529448 wagtail_fedit-1.5.4rc3/wagtail_fedit/templates/wagtail_fedit/icons/
+-rw-rw-rw-   0        0        0      797 2024-04-11 08:36:19.000000 wagtail_fedit-1.5.4rc3/wagtail_fedit/templates/wagtail_fedit/icons/fedit-check-list.svg
+-rw-rw-rw-   0        0        0      584 2024-04-11 08:36:55.000000 wagtail_fedit-1.5.4rc3/wagtail_fedit/templates/wagtail_fedit/icons/fedit-eye-closed.svg
+-rw-rw-rw-   0        0        0      377 2024-04-11 08:23:07.000000 wagtail_fedit-1.5.4rc3/wagtail_fedit/templates/wagtail_fedit/icons/fedit-eye-open.svg
+-rw-rw-rw-   0        0        0      725 2024-04-11 09:02:58.000000 wagtail_fedit-1.5.4rc3/wagtail_fedit/templates/wagtail_fedit/icons/fedit-save.svg
+-rw-rw-rw-   0        0        0     1323 2024-04-11 08:36:52.000000 wagtail_fedit-1.5.4rc3/wagtail_fedit/templates/wagtail_fedit/icons/fedit-stop-sign.svg
+drwxrwxrwx   0        0        0        0 2024-04-23 18:10:30.545211 wagtail_fedit-1.5.4rc3/wagtail_fedit/templates/wagtail_fedit/userbar/
+-rw-rw-rw-   0        0        0      867 2024-04-03 17:05:21.000000 wagtail_fedit-1.5.4rc3/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit.html
+-rw-rw-rw-   0        0        0      876 2024-04-03 16:59:31.000000 wagtail_fedit-1.5.4rc3/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_view_live.html
+drwxrwxrwx   0        0        0        0 2024-04-23 18:10:30.550099 wagtail_fedit-1.5.4rc3/wagtail_fedit/templates/wagtail_fedit/userbar/publish/
+-rw-rw-rw-   0        0        0      263 2024-04-11 08:24:35.000000 wagtail_fedit-1.5.4rc3/wagtail_fedit/templates/wagtail_fedit/userbar/publish/action_button.html
+-rw-rw-rw-   0        0        0      967 2024-04-11 09:03:51.000000 wagtail_fedit-1.5.4rc3/wagtail_fedit/templates/wagtail_fedit/userbar/publish/item_fedit_publishing.html
+drwxrwxrwx   0        0        0        0 2024-04-23 18:10:30.564300 wagtail_fedit-1.5.4rc3/wagtail_fedit/templatetags/
+-rw-rw-rw-   0        0        0        0 2024-03-29 20:13:42.000000 wagtail_fedit-1.5.4rc3/wagtail_fedit/templatetags/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-23 18:10:30.568508 wagtail_fedit-1.5.4rc3/wagtail_fedit/templatetags/__pycache__/
+-rw-rw-rw-   0        0        0      217 2024-03-29 21:05:00.000000 wagtail_fedit-1.5.4rc3/wagtail_fedit/templatetags/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0    12579 2024-04-23 17:39:17.000000 wagtail_fedit-1.5.4rc3/wagtail_fedit/templatetags/__pycache__/fedit.cpython-311.pyc
+-rw-rw-rw-   0        0        0     9556 2024-04-23 17:20:47.000000 wagtail_fedit-1.5.4rc3/wagtail_fedit/templatetags/fedit.py
+drwxrwxrwx   0        0        0        0 2024-04-23 18:10:30.571307 wagtail_fedit-1.5.4rc3/wagtail_fedit/test/
+-rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.4rc3/wagtail_fedit/test/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-23 18:10:30.578316 wagtail_fedit-1.5.4rc3/wagtail_fedit/test/core/
+-rw-rw-rw-   0        0        0      151 2024-04-05 07:59:49.000000 wagtail_fedit-1.5.4rc3/wagtail_fedit/test/core/__init__.py
+-rw-rw-rw-   0        0        0      165 2024-04-05 08:41:40.000000 wagtail_fedit-1.5.4rc3/wagtail_fedit/test/core/apps.py
+-rw-rw-rw-   0        0        0      130 2024-04-15 20:12:38.000000 wagtail_fedit-1.5.4rc3/wagtail_fedit/test/core/context_processors.py
+drwxrwxrwx   0        0        0        0 2024-04-23 18:10:30.583348 wagtail_fedit-1.5.4rc3/wagtail_fedit/test/core/migrations/
+-rw-rw-rw-   0        0        0    12115 2024-04-20 22:33:35.000000 wagtail_fedit-1.5.4rc3/wagtail_fedit/test/core/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0      509 2024-04-21 18:41:55.000000 wagtail_fedit-1.5.4rc3/wagtail_fedit/test/core/migrations/0002_basicmodel_related_field.py
+-rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.4rc3/wagtail_fedit/test/core/migrations/__init__.py
+-rw-rw-rw-   0        0        0     6047 2024-04-23 13:09:46.000000 wagtail_fedit-1.5.4rc3/wagtail_fedit/test/core/models.py
+drwxrwxrwx   0        0        0        0 2024-04-23 18:10:30.599778 wagtail_fedit-1.5.4rc3/wagtail_fedit/test/core/tests/
+-rw-rw-rw-   0        0        0        0 2024-04-05 07:59:29.000000 wagtail_fedit-1.5.4rc3/wagtail_fedit/test/core/tests/__init__.py
+-rw-rw-rw-   0        0        0     8475 2024-04-23 13:35:29.000000 wagtail_fedit-1.5.4rc3/wagtail_fedit/test/core/tests/base.py
+-rw-rw-rw-   0        0        0    22637 2024-04-23 12:36:52.000000 wagtail_fedit-1.5.4rc3/wagtail_fedit/test/core/tests/test_adapters.py
+-rw-rw-rw-   0        0        0     4320 2024-04-06 22:44:26.000000 wagtail_fedit-1.5.4rc3/wagtail_fedit/test/core/tests/test_block_edit.py
+-rw-rw-rw-   0        0        0     5664 2024-04-05 10:31:29.000000 wagtail_fedit-1.5.4rc3/wagtail_fedit/test/core/tests/test_blocks.py
+-rw-rw-rw-   0        0        0     3642 2024-04-05 18:00:23.000000 wagtail_fedit-1.5.4rc3/wagtail_fedit/test/core/tests/test_field_edit.py
+-rw-rw-rw-   0        0        0     3709 2024-04-10 13:03:30.000000 wagtail_fedit-1.5.4rc3/wagtail_fedit/test/core/tests/test_generic.py
+-rw-rw-rw-   0        0        0     4865 2024-04-23 14:23:09.000000 wagtail_fedit-1.5.4rc3/wagtail_fedit/test/core/tests/test_model_edit.py
+-rw-rw-rw-   0        0        0     1574 2024-04-20 20:49:12.000000 wagtail_fedit-1.5.4rc3/wagtail_fedit/test/core/tests/test_revision.py
+-rw-rw-rw-   0        0        0     9545 2024-04-20 21:54:40.000000 wagtail_fedit-1.5.4rc3/wagtail_fedit/test/core/tests/test_submit.py
+-rw-rw-rw-   0        0        0      704 2024-04-05 17:55:36.000000 wagtail_fedit-1.5.4rc3/wagtail_fedit/test/manage.py
+drwxrwxrwx   0        0        0        0 2024-04-23 18:10:30.604980 wagtail_fedit-1.5.4rc3/wagtail_fedit/test/testapp/
+-rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.4rc3/wagtail_fedit/test/testapp/__init__.py
+-rw-rw-rw-   0        0        0      407 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.4rc3/wagtail_fedit/test/testapp/asgi.py
+-rw-rw-rw-   0        0        0     3625 2024-04-15 20:14:41.000000 wagtail_fedit-1.5.4rc3/wagtail_fedit/test/testapp/settings.py
+-rw-rw-rw-   0        0        0      897 2024-04-05 08:04:53.000000 wagtail_fedit-1.5.4rc3/wagtail_fedit/test/testapp/urls.py
+-rw-rw-rw-   0        0        0      407 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.4rc3/wagtail_fedit/test/testapp/wsgi.py
+-rw-rw-rw-   0        0        0     2220 2024-04-23 14:21:34.000000 wagtail_fedit-1.5.4rc3/wagtail_fedit/toolbar.py
+-rw-rw-rw-   0        0        0     1196 2024-04-23 17:25:08.000000 wagtail_fedit-1.5.4rc3/wagtail_fedit/urls.py
+-rw-rw-rw-   0        0        0    17246 2024-04-23 17:23:14.000000 wagtail_fedit-1.5.4rc3/wagtail_fedit/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-23 18:10:30.610983 wagtail_fedit-1.5.4rc3/wagtail_fedit/views/
+-rw-rw-rw-   0        0        0      215 2024-04-23 17:24:50.000000 wagtail_fedit-1.5.4rc3/wagtail_fedit/views/__init__.py
+-rw-rw-rw-   0        0        0     7877 2024-04-23 17:24:01.000000 wagtail_fedit-1.5.4rc3/wagtail_fedit/views/adapters.py
+-rw-rw-rw-   0        0        0    17563 2024-04-21 20:25:17.000000 wagtail_fedit-1.5.4rc3/wagtail_fedit/views/editable.py
+-rw-rw-rw-   0        0        0     1923 2024-04-21 20:29:01.000000 wagtail_fedit-1.5.4rc3/wagtail_fedit/views/mixins.py
+drwxrwxrwx   0        0        0        0 2024-04-23 18:10:30.621336 wagtail_fedit-1.5.4rc3/wagtail_fedit/wagtail_hooks/
+-rw-rw-rw-   0        0        0      184 2024-04-16 10:03:02.000000 wagtail_fedit-1.5.4rc3/wagtail_fedit/wagtail_hooks/__init__.py
+-rw-rw-rw-   0        0        0     1748 2024-04-06 18:37:13.000000 wagtail_fedit-1.5.4rc3/wagtail_fedit/wagtail_hooks/action_menu.py
+-rw-rw-rw-   0        0        0     2857 2024-04-23 15:56:51.000000 wagtail_fedit-1.5.4rc3/wagtail_fedit/wagtail_hooks/adapter_hooks.py
+-rw-rw-rw-   0        0        0      328 2024-04-21 16:44:33.000000 wagtail_fedit-1.5.4rc3/wagtail_fedit/wagtail_hooks/adapter_registry.py
+-rw-rw-rw-   0        0        0      398 2024-04-11 09:03:10.000000 wagtail_fedit-1.5.4rc3/wagtail_fedit/wagtail_hooks/icons.py
+-rw-rw-rw-   0        0        0     2573 2024-04-11 07:39:50.000000 wagtail_fedit-1.5.4rc3/wagtail_fedit/wagtail_hooks/log_actions.py
+-rw-rw-rw-   0        0        0      340 2024-03-30 17:10:05.000000 wagtail_fedit-1.5.4rc3/wagtail_fedit/wagtail_hooks/urls.py
+-rw-rw-rw-   0        0        0     7630 2024-04-19 20:11:56.000000 wagtail_fedit-1.5.4rc3/wagtail_fedit/wagtail_hooks/userbar.py
+drwxrwxrwx   0        0        0        0 2024-04-23 18:10:30.249369 wagtail_fedit-1.5.4rc3/wagtail_fedit.egg-info/
+-rw-rw-rw-   0        0        0    21651 2024-04-23 18:10:30.000000 wagtail_fedit-1.5.4rc3/wagtail_fedit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     4521 2024-04-23 18:10:30.000000 wagtail_fedit-1.5.4rc3/wagtail_fedit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-23 18:10:30.000000 wagtail_fedit-1.5.4rc3/wagtail_fedit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       25 2024-04-23 18:10:30.000000 wagtail_fedit-1.5.4rc3/wagtail_fedit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-04-23 18:10:30.000000 wagtail_fedit-1.5.4rc3/wagtail_fedit.egg-info/top_level.txt
```

### Comparing `wagtail_fedit-1.5.4rc2/LICENSE` & `wagtail_fedit-1.5.4rc3/LICENSE`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.4rc2/PKG-INFO` & `wagtail_fedit-1.5.4rc3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wagtail_fedit
-Version: 1.5.4rc2
+Version: 1.5.4rc3
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
-Metadata-Version: 2.1 Name: wagtail_fedit Version: 1.5.4rc2 Summary: Frontend
+Metadata-Version: 2.1 Name: wagtail_fedit Version: 1.5.4rc3 Summary: Frontend
 editing for your Wagtail site Home-page: https://github.com/Nigel2392/
 wagtail_fedit Author: Nigel Author-email: nigel@goodadvice.it License: GPL-2.0-
 only Classifier: Environment :: Web Environment Classifier: Framework :: Django
 Classifier: Framework :: Django :: 4.2 Classifier: Framework :: Wagtail
 Classifier: Framework :: Wagtail :: 5 Classifier: Framework :: Wagtail :: 6
 Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
 :: GNU General Public License v2 or later (GPLv2+) Classifier: Operating System
```

### Comparing `wagtail_fedit-1.5.4rc2/README.md` & `wagtail_fedit-1.5.4rc3/README.md`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.4rc2/setup.cfg` & `wagtail_fedit-1.5.4rc3/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2077 6167 7461 696c 5f66 6564 6974   = wagtail_fedit
 00000020: 0d0a 7665 7273 696f 6e20 3d20 312e 352e  ..version = 1.5.
-00000030: 3472 6332 0d0a 6465 7363 7269 7074 696f  4rc2..descriptio
+00000030: 3472 6333 0d0a 6465 7363 7269 7074 696f  4rc3..descriptio
 00000040: 6e20 3d20 4672 6f6e 7465 6e64 2065 6469  n = Frontend edi
 00000050: 7469 6e67 2066 6f72 2079 6f75 7220 5761  ting for your Wa
 00000060: 6774 6169 6c20 7369 7465 0d0a 6c6f 6e67  gtail site..long
 00000070: 5f64 6573 6372 6970 7469 6f6e 203d 2066  _description = f
 00000080: 696c 653a 2052 4541 444d 452e 6d64 0d0a  ile: README.md..
 00000090: 6c6f 6e67 5f64 6573 6372 6970 7469 6f6e  long_description
 000000a0: 5f63 6f6e 7465 6e74 5f74 7970 6520 3d20  _content_type =
```

### Comparing `wagtail_fedit-1.5.4rc2/wagtail_fedit/adapters/__init__.py` & `wagtail_fedit-1.5.4rc3/wagtail_fedit/adapters/__init__.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.4rc2/wagtail_fedit/adapters/base.py` & `wagtail_fedit-1.5.4rc3/wagtail_fedit/adapters/base.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.4rc2/wagtail_fedit/adapters/block.py` & `wagtail_fedit-1.5.4rc3/wagtail_fedit/adapters/block.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.4rc2/wagtail_fedit/adapters/field.py` & `wagtail_fedit-1.5.4rc3/wagtail_fedit/adapters/field.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from django.utils import translation
 from django.utils.translation import gettext_lazy as _
 from django.utils.safestring import mark_safe
 from django.http import HttpRequest
 
 from wagtail.log_actions import log
 from wagtail.models import RevisionMixin
+from wagtail.fields import StreamField
 from wagtail import hooks
 
 from .base import (
     BlockFieldReplacementAdapter,
     VARIABLES,
 )
 from ..hooks import (
@@ -161,27 +162,30 @@
             field_forms.save_possible_revision(self.original_object, self.request)
 
         extra_log_kwargs = {}
         if isinstance(self.original_object, RevisionMixin):
             extra_log_kwargs["revision"] = self.original_object.latest_revision
 
         with translation.override(None):
+            old_new = {}
+            if not isinstance(self.meta_field, StreamField):
+                old_new = {
+                    "old": str(self.initial_field_value),
+                    "new": str(getattr(self.object, self.field_name)),
+                }
+
             data = {
                 "verbose_field_name": str(self.meta_field.verbose_name),
                 "field_name": self.field_name,
                 "model_id": self.object.pk,
                 "model_name": self.object._meta.model_name,
                 "app_label": self.object._meta.app_label,
                 "model_verbose": str(self.model._meta.verbose_name),
                 "model_string": str(get_model_string(self.original_object)),
-                "old": str(self.initial_field_value),
-                "new": str(getattr(
-                    self.original_object,
-                    self.field_name
-                )),
+                "old_new": old_new,
             }
 
             uid = uuid.uuid4()
             if self.original_object.pk != self.object.pk:
                 data.update({
                     "edited_model_string": str(get_model_string(self.object)),
                     "edited_model_verbose": str(self.object._meta.verbose_name),
```

### Comparing `wagtail_fedit-1.5.4rc2/wagtail_fedit/adapters/funcs.py` & `wagtail_fedit-1.5.4rc3/wagtail_fedit/adapters/funcs.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.4rc2/wagtail_fedit/adapters/misc.py` & `wagtail_fedit-1.5.4rc3/wagtail_fedit/adapters/misc.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.4rc2/wagtail_fedit/adapters/models.py` & `wagtail_fedit-1.5.4rc3/wagtail_fedit/adapters/models.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.4rc2/wagtail_fedit/adapters/registry.py` & `wagtail_fedit-1.5.4rc3/wagtail_fedit/adapters/registry.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.4rc2/wagtail_fedit/forms/blocks.py` & `wagtail_fedit-1.5.4rc3/wagtail_fedit/forms/blocks.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.4rc2/wagtail_fedit/forms/fields.py` & `wagtail_fedit-1.5.4rc3/wagtail_fedit/forms/fields.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.4rc2/wagtail_fedit/hooks.py` & `wagtail_fedit-1.5.4rc3/wagtail_fedit/hooks.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.4rc2/wagtail_fedit/locale/nl/LC_MESSAGES/django.mo` & `wagtail_fedit-1.5.4rc3/wagtail_fedit/locale/nl/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.4rc2/wagtail_fedit/locale/nl/LC_MESSAGES/django.po` & `wagtail_fedit-1.5.4rc3/wagtail_fedit/locale/nl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.4rc2/wagtail_fedit/models.py` & `wagtail_fedit-1.5.4rc3/wagtail_fedit/models.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.4rc2/wagtail_fedit/settings.py` & `wagtail_fedit-1.5.4rc3/wagtail_fedit/settings.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.4rc2/wagtail_fedit/static/wagtail_fedit/css/frontend.css` & `wagtail_fedit-1.5.4rc3/wagtail_fedit/static/wagtail_fedit/css/frontend.css`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.4rc2/wagtail_fedit/static/wagtail_fedit/css/furniture.css` & `wagtail_fedit-1.5.4rc3/wagtail_fedit/static/wagtail_fedit/css/furniture.css`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.4rc2/wagtail_fedit/static/wagtail_fedit/css/userbar-menu.css` & `wagtail_fedit-1.5.4rc3/wagtail_fedit/static/wagtail_fedit/css/userbar-menu.css`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.4rc2/wagtail_fedit/static/wagtail_fedit/js/frontend.js` & `wagtail_fedit-1.5.4rc3/wagtail_fedit/static/wagtail_fedit/js/frontend.js`

 * *Files 3% similar despite different names*

#### js-beautify {}

```diff
@@ -172,14 +172,18 @@
         if (typeof html === "function") {
             this.#editor.wrapperElement.editorAPI = this;
             html(update);
             return;
         }
     }
 
+    refetch() {
+        this.#editor.refetch();
+    }
+
     execRelated(func) {
         for (const wrapper of this.#editor.relatedWrappers) {
             func(wrapper.editorAPI);
         }
     }
 }
 
@@ -206,31 +210,64 @@
             this.makeModal();
             this.focus();
         }
     }
 
     get relatedWrappers() {
         const wrapperId = this.wrapperElement.dataset.wrapperId;
-        return document.querySelectorAll(`[data-wrapper-id="${wrapperId}"]`);
+        const filterFn = (el) => el !== this.wrapperElement
+        const elements = document.querySelectorAll(`[data-wrapper-id="${wrapperId}"]`)
+        return Array.from(elements).filter(filterFn);
     }
 
     focus() {
         this.wrapperElement.focus();
     }
 
+    get editUrl() {
+        return this.wrapperElement.dataset.editUrl;
+    }
+
+    get refetchUrl() {
+        return this.wrapperElement.dataset.refetchUrl;
+    }
+
+    refetch() {
+        fetch(this.getRefetchUrl()).then((response) => {
+            response = response.json();
+            return response;
+        }).then((response) => {
+            if (!response.success) {
+                console.error("Errors rendering response", response);
+                return;
+            }
+            this.onResponse(response);
+        });
+    }
+
     getEditUrl() {
         // build the edit url from relative edit url
         const url = new URL(window.location.href);
         url.pathname = this.editUrl;
         if (this.sharedContext) {
             url.searchParams.set("shared_context", this.sharedContext);
         }
         return url.toString();
     }
 
+    getRefetchUrl() {
+        // build the edit url from relative edit url
+        const url = new URL(window.location.href);
+        url.pathname = this.refetchUrl;
+        if (this.sharedContext) {
+            url.searchParams.set("shared_context", this.sharedContext);
+        }
+        return url.toString();
+    }
+
     async makeModal() {
         this.modalWrapper.innerHTML = this.modalHtml;
         this.modal = this.modalWrapper.querySelector(".wagtail-fedit-modal");
 
         this.iframe = new iFrame({
             url: this.getEditUrl(),
             id: "wagtail-fedit-iframe",
@@ -339,18 +376,14 @@
         const wrapper = document.createElement("div");
         wrapper.id = "wagtail-fedit-modal-wrapper";
         wrapper.classList.add("wagtail-fedit-modal-wrapper");
         document.body.appendChild(wrapper);
         return wrapper;
     }
 
-    get editUrl() {
-        return this.wrapperElement.dataset.editUrl;
-    }
-
     init() {
         this.sharedContext = this.wrapperElement.dataset.sharedContext;
         this.modalHtml = modalHtml.replace("__ID__", this.wrapperElement.dataset.id);
         this.editBtn = this.wrapperElement.querySelector(".wagtail-fedit-edit-button");
 
         this.wrapperElement.editorAPI = this.api;
 
@@ -425,46 +458,49 @@
         return window.wagtailFedit.funcs;
     }
 }
 
 
 class BlockFieldEditor extends BaseWagtailFeditEditor {
     onResponse(response) {
-        const html = response.html;
-        for (const wrapper of this.relatedWrappers) {
-            wrapper.editorAPI.updateHtml((update) => {
-                // Fade out the old block
-                const anim = wrapper.animate([{
-                    opacity: 1
-                }, {
+        this.api.updateHtml((update) => {
+            // Fade out the old block
+            const anim = this.wrapperElement.animate([{
+                opacity: 1
+            }, {
+                opacity: 0
+            }, ], {
+                duration: 350,
+                easing: "ease-in-out",
+            });
+
+            anim.onfinish = () => {
+
+                const blockWrapper = update(response.html);
+
+                if (!response.refetch) {
+                    for (const wrapper of this.relatedWrappers) {
+                        wrapper.editorAPI.refetch();
+                    }
+                }
+
+                // Fade in the new block
+                const anim = blockWrapper.animate([{
                     opacity: 0
+                }, {
+                    opacity: 1
                 }, ], {
                     duration: 350,
                     easing: "ease-in-out",
                 });
-
                 anim.onfinish = () => {
-
-                    const blockWrapper = update(html);
-
-                    // Fade in the new block
-                    const anim = blockWrapper.animate([{
-                        opacity: 0
-                    }, {
-                        opacity: 1
-                    }, ], {
-                        duration: 350,
-                        easing: "ease-in-out",
-                    });
-                    anim.onfinish = () => {
-                        blockWrapper.style.opacity = 1;
-                    };
-                }
-            });
-        }
+                    blockWrapper.style.opacity = 1;
+                };
+            }
+        });
     }
 }
 
 
 class WagtailFeditPublishMenu {
     constructor(publishButton) {
         this.publishButton = publishButton;
```

### Comparing `wagtail_fedit-1.5.4rc2/wagtail_fedit/static/wagtail_fedit/vendor/tippy/LICENSE` & `wagtail_fedit-1.5.4rc3/wagtail_fedit/static/wagtail_fedit/vendor/tippy/LICENSE`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.4rc2/wagtail_fedit/static/wagtail_fedit/vendor/tippy/popper.min.js` & `wagtail_fedit-1.5.4rc3/wagtail_fedit/static/wagtail_fedit/vendor/tippy/popper.min.js`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.4rc2/wagtail_fedit/static/wagtail_fedit/vendor/tippy/tippy-bundle.min.js` & `wagtail_fedit-1.5.4rc3/wagtail_fedit/static/wagtail_fedit/vendor/tippy/tippy-bundle.min.js`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.4rc2/wagtail_fedit/templates/wagtail_fedit/content/buttons/admin_link.html` & `wagtail_fedit-1.5.4rc3/wagtail_fedit/templates/wagtail_fedit/content/buttons/admin_link.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.4rc2/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_adapter.html` & `wagtail_fedit-1.5.4rc3/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_adapter.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.4rc2/wagtail_fedit/templates/wagtail_fedit/content/editable_adapter.html` & `wagtail_fedit-1.5.4rc3/wagtail_fedit/templates/wagtail_fedit/content/editable_adapter.html`

 * *Files 26% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-{% load fedit %}<div id="{{ unique_id }}" data-wrapper-id="{{ unique_id }}" class="wagtail-fedit-adapter-wrapper{% if shared_context.inline or adapter.inline %} wagtail-fedit-inline{%endif%} wagtail-fedit-{{ identifier }}" data-fedit-constructor="{{ js_constructor }}" {% if shared %} data-shared-context="{{ shared }}"{%endif%} data-edit-url="{{ edit_url }}">
+{% load fedit %}<div id="{{ unique_id }}" data-wrapper-id="{{ unique_id }}" class="wagtail-fedit-adapter-wrapper{% if shared_context.inline or adapter.inline %} wagtail-fedit-inline{%endif%} wagtail-fedit-{{ identifier }}" data-fedit-constructor="{{ js_constructor }}" {% if shared %} data-shared-context="{{ shared }}"{%endif%} data-edit-url="{{ edit_url }}" data-refetch-url="{{ refetch_url }}">
     <div class="wagtail-fedit-buttons">
         {% for button in buttons %}
             {{ button }}
         {% endfor %}
     </div>{% render_adapter adapter %}
 </div>
```

### Comparing `wagtail_fedit-1.5.4rc2/wagtail_fedit/templates/wagtail_fedit/editor/action_confirm.html` & `wagtail_fedit-1.5.4rc3/wagtail_fedit/templates/wagtail_fedit/editor/action_confirm.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.4rc2/wagtail_fedit/templates/wagtail_fedit/editor/action_publish_confirm.html` & `wagtail_fedit-1.5.4rc3/wagtail_fedit/templates/wagtail_fedit/editor/action_publish_confirm.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.4rc2/wagtail_fedit/templates/wagtail_fedit/editor/adapter_form.html` & `wagtail_fedit-1.5.4rc3/wagtail_fedit/templates/wagtail_fedit/editor/adapter_form.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.4rc2/wagtail_fedit/templates/wagtail_fedit/editor/base_iframe.html` & `wagtail_fedit-1.5.4rc3/wagtail_fedit/templates/wagtail_fedit/editor/base_iframe.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.4rc2/wagtail_fedit/templates/wagtail_fedit/icons/fedit-check-list.svg` & `wagtail_fedit-1.5.4rc3/wagtail_fedit/templates/wagtail_fedit/icons/fedit-check-list.svg`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.4rc2/wagtail_fedit/templates/wagtail_fedit/icons/fedit-eye-closed.svg` & `wagtail_fedit-1.5.4rc3/wagtail_fedit/templates/wagtail_fedit/icons/fedit-eye-closed.svg`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.4rc2/wagtail_fedit/templates/wagtail_fedit/icons/fedit-save.svg` & `wagtail_fedit-1.5.4rc3/wagtail_fedit/templates/wagtail_fedit/icons/fedit-save.svg`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.4rc2/wagtail_fedit/templates/wagtail_fedit/icons/fedit-stop-sign.svg` & `wagtail_fedit-1.5.4rc3/wagtail_fedit/templates/wagtail_fedit/icons/fedit-stop-sign.svg`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.4rc2/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit.html` & `wagtail_fedit-1.5.4rc3/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.4rc2/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_view_live.html` & `wagtail_fedit-1.5.4rc3/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_view_live.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.4rc2/wagtail_fedit/templates/wagtail_fedit/userbar/publish/item_fedit_publishing.html` & `wagtail_fedit-1.5.4rc3/wagtail_fedit/templates/wagtail_fedit/userbar/publish/item_fedit_publishing.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.4rc2/wagtail_fedit/templatetags/__pycache__/fedit.cpython-311.pyc` & `wagtail_fedit-1.5.4rc3/wagtail_fedit/templatetags/__pycache__/fedit.cpython-311.pyc`

 * *Files 9% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0xd5d22766 (Tue Apr 23 15:25:09 2024 UTC)
-files sz: 9470
+moddate:  0xefed2766 (Tue Apr 23 17:20:47 2024 UTC)
+files sz: 9556
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 13
    flags     : 0
    code
       0x9700640064016c006d015a016d025a020100640064026c036d045a046d
@@ -185,99 +185,99 @@
                282 MAKE_FUNCTION            0
                284 LOAD_CONST              24 ('AdapterNode')
                286 LOAD_NAME                5 (Node)
                288 PRECALL                  3
                292 CALL                     3
                302 STORE_NAME              44 (AdapterNode)
    
-   140         304 LOAD_NAME               39 (register)
+   141         304 LOAD_NAME               39 (register)
                306 LOAD_METHOD             45 (tag)
                328 LOAD_NAME               35 (TEMPLATE_TAG_NAME)
                330 KW_NAMES                25
                332 PRECALL                  1
                336 CALL                     1
    
-   141         346 LOAD_CONST              26 ('parser')
+   142         346 LOAD_CONST              26 ('parser')
                348 LOAD_NAME               10 (Parser)
                350 LOAD_CONST              27 ('token')
                352 LOAD_NAME               11 (Token)
                354 BUILD_TUPLE              4
-               356 LOAD_CONST              28 (<code object do_render_fedit, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 140>)
+               356 LOAD_CONST              28 (<code object do_render_fedit, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 141>)
                358 MAKE_FUNCTION            4 (annotations)
    
-   140         360 PRECALL                  0
+   141         360 PRECALL                  0
                364 CALL                     0
    
-   141         374 STORE_NAME              46 (do_render_fedit)
+   142         374 STORE_NAME              46 (do_render_fedit)
    
-   198         376 LOAD_NAME               39 (register)
+   199         376 LOAD_NAME               39 (register)
                378 LOAD_METHOD             47 (simple_tag)
                400 LOAD_CONST              29 (True)
                402 KW_NAMES                30
                404 PRECALL                  1
                408 CALL                     1
    
-   199         418 LOAD_CONST              19 ('context')
+   200         418 LOAD_CONST              19 ('context')
                420 LOAD_NAME                8 (Context)
                422 LOAD_CONST              31 ('adapter')
                424 LOAD_NAME               29 (BaseAdapter)
                426 LOAD_CONST              21 ('return')
                428 LOAD_NAME               42 (str)
                430 BUILD_TUPLE              6
-               432 LOAD_CONST              32 (<code object render_adapter, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 198>)
+               432 LOAD_CONST              32 (<code object render_adapter, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 199>)
                434 MAKE_FUNCTION            4 (annotations)
    
-   198         436 PRECALL                  0
+   199         436 PRECALL                  0
                440 CALL                     0
    
-   199         450 STORE_NAME              48 (render_adapter)
+   200         450 STORE_NAME              48 (render_adapter)
    
-   215         452 LOAD_NAME               39 (register)
+   218         452 LOAD_NAME               39 (register)
                454 LOAD_METHOD             49 (inclusion_tag)
                476 LOAD_CONST              33 ('wagtail_fedit/_hook_output.html')
                478 LOAD_CONST              34 ('fedit_scripts')
                480 LOAD_CONST              29 (True)
                482 KW_NAMES                35
                484 PRECALL                  3
                488 CALL                     3
    
-   216         498 LOAD_CONST              21 ('return')
+   219         498 LOAD_CONST              21 ('return')
                500 LOAD_NAME               50 (dict)
                502 BUILD_TUPLE              2
-               504 LOAD_CONST              36 (<code object static_hook_output, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 215>)
+               504 LOAD_CONST              36 (<code object static_hook_output, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 218>)
                506 MAKE_FUNCTION            4 (annotations)
    
-   215         508 PRECALL                  0
+   218         508 PRECALL                  0
                512 CALL                     0
    
-   216         522 STORE_NAME              51 (static_hook_output)
+   219         522 STORE_NAME              51 (static_hook_output)
    
-   245         524 LOAD_NAME               39 (register)
+   248         524 LOAD_NAME               39 (register)
                526 LOAD_METHOD             47 (simple_tag)
                548 LOAD_CONST              37 (False)
                550 LOAD_CONST              38 ('tooltip')
                552 KW_NAMES                39
                554 PRECALL                  2
                558 CALL                     2
    
-   246         568 LOAD_CONST              47 ((None,))
+   249         568 LOAD_CONST              47 ((None,))
                570 LOAD_CONST              40 ('wrapping')
                572 LOAD_NAME               42 (str)
                574 LOAD_CONST              21 ('return')
                576 LOAD_NAME               42 (str)
                578 BUILD_TUPLE              4
-               580 LOAD_CONST              41 (<code object tooltip, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 245>)
+               580 LOAD_CONST              41 (<code object tooltip, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 248>)
                582 MAKE_FUNCTION            5 (defaults, annotations)
    
-   245         584 PRECALL                  0
+   248         584 PRECALL                  0
                588 CALL                     0
    
-   246         598 STORE_NAME              52 (tooltip)
+   249         598 STORE_NAME              52 (tooltip)
    
-   261         600 LOAD_CONST              48 ((None, None, None))
+   264         600 LOAD_CONST              48 ((None, None, None))
                602 LOAD_CONST              26 ('parser')
                604 LOAD_NAME               10 (Parser)
                606 LOAD_CONST              42 ('tokens')
                608 LOAD_NAME               53 (list)
                610 LOAD_NAME               42 (str)
                612 BINARY_SUBSCR
                622 LOAD_CONST              43 ('kwarg_list')
@@ -293,15 +293,15 @@
                658 LOAD_NAME               42 (str)
                660 LOAD_NAME                2 (Any)
                662 BUILD_TUPLE              2
                664 BINARY_SUBSCR
                674 LOAD_CONST              21 ('return')
                676 LOAD_NAME               50 (dict)
                678 BUILD_TUPLE             12
-               680 LOAD_CONST              46 (<code object get_kwargs, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 261>)
+               680 LOAD_CONST              46 (<code object get_kwargs, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 264>)
                682 MAKE_FUNCTION            5 (defaults, annotations)
                684 STORE_NAME              54 (get_kwargs)
                686 LOAD_CONST              11 (None)
                688 RETURN_VALUE
    consts
       0
       ('Type', 'Any')
@@ -560,20 +560,22 @@
                   20010074290000000000000000000064057c026a1500000000000000006a
                   0900000000000000009b0064067c099b009d04a6010000ab010000000000
                   000000820177007803590077017c01a01600000000000000000000000000
                   000000000000006407a6010000ab0100000000000000007d0a02007c006a
                   04000000000000000064097c067c057c0a64089c037c04a4018e017d0b7c
                   0ba0170000000000000000000000000000000000000000a6000000ab0000
                   0000000000000072107431000000000000000000007c0a7c06a6020000ab
-                  02000000000000000073297419000000000000000000007c006a0c000000
-                  00000000007c017c0ba01900000000000000000000000000000000000000
-                  007c01a6010000ab010000000000000000a6030000ab0300000000000000
-                  0053007419000000000000000000007c006a0c00000000000000007c0174
-                  35000000000000000000007c0a7c0b7c01a6030000ab0300000000000000
-                  00a6030000ab0300000000000000005300
+                  02000000000000000073437c01a019000000000000000000000000000000
+                  00000000007c0b6a030000000000000000a6010000ab0100000000000000
+                  0001007419000000000000000000007c006a0c00000000000000007c017c
+                  0ba01a00000000000000000000000000000000000000007c01a6010000ab
+                  010000000000000000a6030000ab03000000000000000053007419000000
+                  000000000000007c006a0c00000000000000007c01743700000000000000
+                  0000007c0a7c0b7c01a6030000ab030000000000000000a6030000ab0300
+                  000000000000005300
                 74           0 RESUME                   0
                
                 75           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (model)
                             14 STORE_FAST               2 (model)
                
                 76          16 LOAD_FAST                0 (self)
@@ -835,42 +837,50 @@
                
                134         908 LOAD_GLOBAL             49 (NULL + _can_edit)
                            920 LOAD_FAST               10 (request)
                            922 LOAD_FAST                6 (obj)
                            924 PRECALL                  2
                            928 CALL                     2
                
-               133         938 POP_JUMP_FORWARD_IF_TRUE    41 (to 1022)
+               133         938 POP_JUMP_FORWARD_IF_TRUE    67 (to 1074)
                
-               135     >>  940 LOAD_GLOBAL             25 (NULL + as_var)
-                           952 LOAD_FAST                0 (self)
-                           954 LOAD_ATTR               12 (as_var)
-                           964 LOAD_FAST                1 (context)
-                           966 LOAD_FAST               11 (adapter)
-                           968 LOAD_METHOD             25 (render_content)
-                           990 LOAD_FAST                1 (context)
-                           992 PRECALL                  1
-                           996 CALL                     1
-                          1006 PRECALL                  3
-                          1010 CALL                     3
-                          1020 RETURN_VALUE
-               
-               137     >> 1022 LOAD_GLOBAL             25 (NULL + as_var)
-                          1034 LOAD_FAST                0 (self)
-                          1036 LOAD_ATTR               12 (as_var)
-                          1046 LOAD_FAST                1 (context)
-                          1048 LOAD_GLOBAL             53 (NULL + wrap_adapter)
-                          1060 LOAD_FAST               10 (request)
-                          1062 LOAD_FAST               11 (adapter)
-                          1064 LOAD_FAST                1 (context)
-                          1066 PRECALL                  3
-                          1070 CALL                     3
-                          1080 PRECALL                  3
-                          1084 CALL                     3
-                          1094 RETURN_VALUE
+               135     >>  940 LOAD_FAST                1 (context)
+                           942 LOAD_METHOD             25 (update)
+                           964 LOAD_FAST               11 (adapter)
+                           966 LOAD_ATTR                3 (kwargs)
+                           976 PRECALL                  1
+                           980 CALL                     1
+                           990 POP_TOP
+               
+               136         992 LOAD_GLOBAL             25 (NULL + as_var)
+                          1004 LOAD_FAST                0 (self)
+                          1006 LOAD_ATTR               12 (as_var)
+                          1016 LOAD_FAST                1 (context)
+                          1018 LOAD_FAST               11 (adapter)
+                          1020 LOAD_METHOD             26 (render_content)
+                          1042 LOAD_FAST                1 (context)
+                          1044 PRECALL                  1
+                          1048 CALL                     1
+                          1058 PRECALL                  3
+                          1062 CALL                     3
+                          1072 RETURN_VALUE
+               
+               138     >> 1074 LOAD_GLOBAL             25 (NULL + as_var)
+                          1086 LOAD_FAST                0 (self)
+                          1088 LOAD_ATTR               12 (as_var)
+                          1098 LOAD_FAST                1 (context)
+                          1100 LOAD_GLOBAL             55 (NULL + wrap_adapter)
+                          1112 LOAD_FAST               10 (request)
+                          1114 LOAD_FAST               11 (adapter)
+                          1116 LOAD_FAST                1 (context)
+                          1118 PRECALL                  3
+                          1122 CALL                     3
+                          1132 PRECALL                  3
+                          1136 CALL                     3
+                          1146 RETURN_VALUE
                ExceptionTable:
                  354 to 428 -> 432 [0]
                  432 to 450 -> 518 [1] lasti
                  452 to 506 -> 508 [1] lasti
                  508 to 516 -> 518 [1] lasti
                  668 to 698 -> 702 [1]
                  702 to 784 -> 786 [2] lasti
@@ -881,26 +891,27 @@
                   'object'
                   1
                   'Object '
                   ' does not have attribute '
                   'request'
                   ('object', 'field_name', 'request')
                   ()
-               names      ('model', 'getters', '_resolve_expressions', 'kwargs', 'adapter', 'field_required', 'warnings', 'warn', 'WARNING_MODEL_INSTANCE_NOT_AVAILABLE', '__name__', 'RuntimeWarning', 'flatten', 'as_var', 'render_from_kwargs', 'AdapterError', 'TemplateSyntaxError', 'str', 'len', 'range', 'getattr', 'AttributeError', '__class__', 'get', 'check_permissions', '_can_edit', 'render_content', 'wrap_adapter')
+               names      ('model', 'getters', '_resolve_expressions', 'kwargs', 'adapter', 'field_required', 'warnings', 'warn', 'WARNING_MODEL_INSTANCE_NOT_AVAILABLE', '__name__', 'RuntimeWarning', 'flatten', 'as_var', 'render_from_kwargs', 'AdapterError', 'TemplateSyntaxError', 'str', 'len', 'range', 'getattr', 'AttributeError', '__class__', 'get', 'check_permissions', '_can_edit', 'update', 'render_content', 'wrap_adapter')
                varnames   ('self', 'context', 'model', 'getters', 'kwargs', 'field_name', 'obj', 'e', 'i', 'getter', 'request', 'adapter')
                freevars   ()
                cellvars   ()
                filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\tester\\wagtail_fedit\\templatetags\\fedit.py'
                name       'render'
                firstlineno 74
                lnotab
                   0x02010e010e020e0104ff04010cff0c040801080102ff020116ff020310
                   011402240110010804040116010c0118ff06030cfc100728020201320102
                   ff040102ff1603120140ff08030401040104013002420110010201240112
-                  013eff08042a0110010201020102fd040402fc060728011eff02025202
+                  013eff08042a0110010201020102fd040402fc060728011eff0202340152
+                  02
             (None,)
          names      ('__name__', '__module__', '__qualname__', 'signing', 'TimestampSigner', 'signer', 'Type', 'BaseAdapter', 'FilterExpression', 'list', 'str', '__init__', '_resolve_expressions', 'render')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\tester\\wagtail_fedit\\templatetags\\fedit.py'
          name       'AdapterNode'
@@ -942,219 +953,219 @@
             01000000000000000064097a0a0000a6010000ab0100000000000000007d
             097c02a0010000000000000000000000000000000000000000740d000000
             000000000000007c02a6010000ab01000000000000000064097a0a0000a6
             010000ab01000000000000000001007413000000000000000000007c007c
             027c056a0a00000000000000007c056a0b00000000000000007c056a0c00
             00000000000000a6050000ab0500000000000000007d0a741b0000000000
             0000000000640c7c057c067c077c09640b9c047c0aa4018e015300
-         140           0 RESUME                   0
+         141           0 RESUME                   0
          
-         143           2 LOAD_FAST                1 (token)
+         144           2 LOAD_FAST                1 (token)
                        4 LOAD_METHOD              0 (split_contents)
                       26 PRECALL                  0
                       30 CALL                     0
                       40 STORE_FAST               2 (tokens)
          
-         145          42 LOAD_FAST                2 (tokens)
+         146          42 LOAD_FAST                2 (tokens)
                       44 LOAD_METHOD              1 (pop)
                       66 LOAD_CONST               1 (0)
                       68 PRECALL                  1
                       72 CALL                     1
                       82 STORE_FAST               3 (_)
          
-         146          84 LOAD_FAST                2 (tokens)
+         147          84 LOAD_FAST                2 (tokens)
                       86 LOAD_METHOD              1 (pop)
                      108 LOAD_CONST               1 (0)
                      110 PRECALL                  1
                      114 CALL                     1
                      124 STORE_FAST               4 (adapter_id)
          
-         148         126 NOP
+         149         126 NOP
          
-         149         128 LOAD_GLOBAL              4 (adapter_registry)
+         150         128 LOAD_GLOBAL              4 (adapter_registry)
                      140 LOAD_FAST                4 (adapter_id)
                      142 BINARY_SUBSCR
                      152 STORE_FAST               5 (adapter)
                      154 JUMP_FORWARD            33 (to 222)
                  >>  156 PUSH_EXC_INFO
          
-         150         158 LOAD_GLOBAL              6 (RegistryLookUpError)
+         151         158 LOAD_GLOBAL              6 (RegistryLookUpError)
                      170 CHECK_EXC_MATCH
                      172 POP_JUMP_FORWARD_IF_FALSE    20 (to 214)
                      174 POP_TOP
          
-         151         176 LOAD_GLOBAL              9 (NULL + TemplateSyntaxError)
+         152         176 LOAD_GLOBAL              9 (NULL + TemplateSyntaxError)
                      188 LOAD_CONST               2 ("No adapter found with identifier '")
                      190 LOAD_FAST                4 (adapter_id)
                      192 FORMAT_VALUE             0
                      194 LOAD_CONST               3 ("'")
                      196 BUILD_STRING             3
                      198 PRECALL                  1
                      202 CALL                     1
                      212 RAISE_VARARGS            1
          
-         150     >>  214 RERAISE                  0
+         151     >>  214 RERAISE                  0
                  >>  216 COPY                     3
                      218 POP_EXCEPT
                      220 RERAISE                  1
          
-         153     >>  222 LOAD_CONST               4 ((None, None))
+         154     >>  222 LOAD_CONST               4 ((None, None))
                      224 UNPACK_SEQUENCE          2
                      228 STORE_FAST               6 (model)
                      230 STORE_FAST               7 (model_tokens)
          
-         154         232 LOAD_FAST                2 (tokens)
+         155         232 LOAD_FAST                2 (tokens)
                      234 POP_JUMP_FORWARD_IF_FALSE   173 (to 582)
          
-         155         236 LOAD_FAST                2 (tokens)
+         156         236 LOAD_FAST                2 (tokens)
                      238 LOAD_METHOD              1 (pop)
                      260 LOAD_CONST               1 (0)
                      262 PRECALL                  1
                      266 CALL                     1
                      276 STORE_FAST               8 (model__field)
          
-         156         278 LOAD_FAST                8 (model__field)
+         157         278 LOAD_FAST                8 (model__field)
                      280 LOAD_METHOD              5 (split)
                      302 LOAD_CONST               5 ('.')
                      304 PRECALL                  1
                      308 CALL                     1
                      318 STORE_FAST               7 (model_tokens)
          
-         160         320 LOAD_GLOBAL             13 (NULL + len)
+         161         320 LOAD_GLOBAL             13 (NULL + len)
                      332 LOAD_FAST                7 (model_tokens)
                      334 PRECALL                  1
                      338 CALL                     1
                      348 LOAD_CONST               6 (2)
                      350 COMPARE_OP               0 (<)
                      356 POP_JUMP_FORWARD_IF_FALSE    34 (to 426)
          
-         161         358 LOAD_FAST                7 (model_tokens)
+         162         358 LOAD_FAST                7 (model_tokens)
                      360 LOAD_CONST               1 (0)
                      362 BINARY_SUBSCR
                      372 LOAD_CONST               7 ('from_context')
                      374 COMPARE_OP               3 (!=)
                      380 POP_JUMP_FORWARD_IF_FALSE    22 (to 426)
                      382 LOAD_FAST                5 (adapter)
                      384 LOAD_ATTR                7 (field_required)
                      394 POP_JUMP_FORWARD_IF_FALSE    15 (to 426)
          
-         162         396 LOAD_GLOBAL              9 (NULL + TemplateSyntaxError)
+         163         396 LOAD_GLOBAL              9 (NULL + TemplateSyntaxError)
          
-         163         408 LOAD_CONST               8 ("Model and field name are required: 'mymodel.myfield' or 'from_context'")
+         164         408 LOAD_CONST               8 ("Model and field name are required: 'mymodel.myfield' or 'from_context'")
          
-         162         410 PRECALL                  1
+         163         410 PRECALL                  1
                      414 CALL                     1
                      424 RAISE_VARARGS            1
          
-         167     >>  426 LOAD_GLOBAL             13 (NULL + len)
+         168     >>  426 LOAD_GLOBAL             13 (NULL + len)
                      438 LOAD_FAST                7 (model_tokens)
                      440 PRECALL                  1
                      444 CALL                     1
                      454 LOAD_CONST               9 (1)
                      456 COMPARE_OP               4 (>)
                      462 POP_JUMP_FORWARD_IF_TRUE    19 (to 502)
          
-         168         464 LOAD_FAST                7 (model_tokens)
+         169         464 LOAD_FAST                7 (model_tokens)
                      466 LOAD_CONST               1 (0)
                      468 BINARY_SUBSCR
                      478 LOAD_CONST               7 ('from_context')
                      480 COMPARE_OP               3 (!=)
                      486 POP_JUMP_FORWARD_IF_FALSE    47 (to 582)
                      488 LOAD_FAST                5 (adapter)
                      490 LOAD_ATTR                7 (field_required)
                      500 POP_JUMP_FORWARD_IF_TRUE    40 (to 582)
          
-         173     >>  502 LOAD_FAST                0 (parser)
+         174     >>  502 LOAD_FAST                0 (parser)
                      504 LOAD_METHOD              8 (compile_filter)
                      526 LOAD_FAST                7 (model_tokens)
                      528 LOAD_METHOD              1 (pop)
                      550 LOAD_CONST               1 (0)
                      552 PRECALL                  1
                      556 CALL                     1
                      566 PRECALL                  1
                      570 CALL                     1
                      580 STORE_FAST               6 (model)
          
-         175     >>  582 LOAD_CONST               0 (None)
+         176     >>  582 LOAD_CONST               0 (None)
                      584 STORE_FAST               9 (as_var)
          
-         176         586 LOAD_FAST                2 (tokens)
+         177         586 LOAD_FAST                2 (tokens)
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
          
-         177         646 LOAD_FAST                2 (tokens)
+         178         646 LOAD_FAST                2 (tokens)
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
          
-         178         720 LOAD_FAST                2 (tokens)
+         179         720 LOAD_FAST                2 (tokens)
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
          
-         180     >>  794 LOAD_GLOBAL             19 (NULL + get_kwargs)
+         181     >>  794 LOAD_GLOBAL             19 (NULL + get_kwargs)
          
-         181         806 LOAD_FAST                0 (parser)
+         182         806 LOAD_FAST                0 (parser)
          
-         182         808 LOAD_FAST                2 (tokens)
+         183         808 LOAD_FAST                2 (tokens)
          
-         183         810 LOAD_FAST                5 (adapter)
+         184         810 LOAD_FAST                5 (adapter)
                      812 LOAD_ATTR               10 (required_kwargs)
          
-         184         822 LOAD_FAST                5 (adapter)
+         185         822 LOAD_FAST                5 (adapter)
                      824 LOAD_ATTR               11 (absolute_tokens)
          
-         185         834 LOAD_FAST                5 (adapter)
+         186         834 LOAD_FAST                5 (adapter)
                      836 LOAD_ATTR               12 (optional_kwargs)
          
-         180         846 PRECALL                  5
+         181         846 PRECALL                  5
                      850 CALL                     5
                      860 STORE_FAST              10 (kwargs)
          
-         188         862 LOAD_GLOBAL             27 (NULL + AdapterNode)
+         189         862 LOAD_GLOBAL             27 (NULL + AdapterNode)
                      874 LOAD_CONST              12 (())
          
-         189         876 LOAD_FAST                5 (adapter)
+         190         876 LOAD_FAST                5 (adapter)
          
-         190         878 LOAD_FAST                6 (model)
+         191         878 LOAD_FAST                6 (model)
          
-         191         880 LOAD_FAST                7 (model_tokens)
+         192         880 LOAD_FAST                7 (model_tokens)
          
-         192         882 LOAD_FAST                9 (as_var)
+         193         882 LOAD_FAST                9 (as_var)
          
-         188         884 LOAD_CONST              11 (('adapter', 'model', 'getters', 'as_var'))
+         189         884 LOAD_CONST              11 (('adapter', 'model', 'getters', 'as_var'))
                      886 BUILD_CONST_KEY_MAP      4
          
-         193         888 LOAD_FAST               10 (kwargs)
+         194         888 LOAD_FAST               10 (kwargs)
          
-         188         890 DICT_MERGE               1
+         189         890 DICT_MERGE               1
                      892 CALL_FUNCTION_EX         1
                      894 RETURN_VALUE
          ExceptionTable:
            128 to 152 -> 156 [0]
            156 to 214 -> 216 [1] lasti
          consts
             None
@@ -1172,15 +1183,15 @@
             ()
          names      ('split_contents', 'pop', 'adapter_registry', 'RegistryLookUpError', 'TemplateSyntaxError', 'split', 'len', 'field_required', 'compile_filter', 'get_kwargs', 'required_kwargs', 'absolute_tokens', 'optional_kwargs', 'AdapterNode')
          varnames   ('parser', 'token', 'tokens', '_', 'adapter_id', 'adapter', 'model', 'model_tokens', 'model__field', 'as_var', 'kwargs')
          freevars   ()
          cellvars   ()
          filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\tester\\wagtail_fedit\\templatetags\\fedit.py'
          name       'do_render_fedit'
-         firstlineno 140
+         firstlineno 141
          lnotab
             0x020328022a012a0202011e01120126ff08030a0104012a012a04260126
             010c0102ff100526012605500204013c014a014a020c01020102010c010c
             010cfb10080e0102010201020102fc040502fb
       True
       ('takes_context',)
       'adapter'
@@ -1190,81 +1201,90 @@
          stacksize : 3
          flags     : 3
          code
             0x970069007d0264017c007600720b7c006401190000000000000000007d
             027c0064013d007c00a00000000000000000000000000000000000000000
             007c02a6010000ab01000000000000000001007c016a0100000000000000
             007c0064023c0000007c016a0200000000000000007c0064033c0000007c
-            016a0300000000000000007c0064043c0000007c01a00400000000000000
-            000000000000000000000000007c00a6010000ab01000000000000000053
-            00
-         198           0 RESUME                   0
+            016a0300000000000000007c0064043c0000007c00a00000000000000000
+            000000000000000000000000007c016a040000000000000000a6010000ab
+            01000000000000000001007c01a005000000000000000000000000000000
+            00000000007c00a6010000ab0100000000000000005300
+         199           0 RESUME                   0
          
-         200           2 BUILD_MAP                0
+         201           2 BUILD_MAP                0
                        4 STORE_FAST               2 (parent_context)
          
-         202           6 LOAD_CONST               1 ('parent_context')
+         203           6 LOAD_CONST               1 ('parent_context')
                        8 LOAD_FAST                0 (context)
                       10 CONTAINS_OP              0
                       12 POP_JUMP_FORWARD_IF_FALSE    11 (to 36)
          
-         203          14 LOAD_FAST                0 (context)
+         204          14 LOAD_FAST                0 (context)
                       16 LOAD_CONST               1 ('parent_context')
                       18 BINARY_SUBSCR
                       28 STORE_FAST               2 (parent_context)
          
-         204          30 LOAD_FAST                0 (context)
+         205          30 LOAD_FAST                0 (context)
                       32 LOAD_CONST               1 ('parent_context')
                       34 DELETE_SUBSCR
          
-         206     >>   36 LOAD_FAST                0 (context)
+         207     >>   36 LOAD_FAST                0 (context)
                       38 LOAD_METHOD              0 (update)
                       60 LOAD_FAST                2 (parent_context)
                       62 PRECALL                  1
                       66 CALL                     1
                       76 POP_TOP
          
-         208          78 LOAD_FAST                1 (adapter)
+         209          78 LOAD_FAST                1 (adapter)
                       80 LOAD_ATTR                1 (field_name)
                       90 LOAD_FAST                0 (context)
                       92 LOAD_CONST               2 ('wagtail_fedit_field')
                       94 STORE_SUBSCR
          
-         209          98 LOAD_FAST                1 (adapter)
+         210          98 LOAD_FAST                1 (adapter)
                      100 LOAD_ATTR                2 (object)
                      110 LOAD_FAST                0 (context)
                      112 LOAD_CONST               3 ('wagtail_fedit_instance')
                      114 STORE_SUBSCR
          
-         210         118 LOAD_FAST                1 (adapter)
+         211         118 LOAD_FAST                1 (adapter)
                      120 LOAD_ATTR                3 (request)
                      130 LOAD_FAST                0 (context)
                      132 LOAD_CONST               4 ('request')
                      134 STORE_SUBSCR
          
-         212         138 LOAD_FAST                1 (adapter)
-                     140 LOAD_METHOD              4 (render_content)
-                     162 LOAD_FAST                0 (context)
-                     164 PRECALL                  1
-                     168 CALL                     1
-                     178 RETURN_VALUE
+         213         138 LOAD_FAST                0 (context)
+                     140 LOAD_METHOD              0 (update)
+                     162 LOAD_FAST                1 (adapter)
+                     164 LOAD_ATTR                4 (kwargs)
+                     174 PRECALL                  1
+                     178 CALL                     1
+                     188 POP_TOP
+         
+         215         190 LOAD_FAST                1 (adapter)
+                     192 LOAD_METHOD              5 (render_content)
+                     214 LOAD_FAST                0 (context)
+                     216 PRECALL                  1
+                     220 CALL                     1
+                     230 RETURN_VALUE
          consts
             None
             'parent_context'
             'wagtail_fedit_field'
             'wagtail_fedit_instance'
             'request'
-         names      ('update', 'field_name', 'object', 'request', 'render_content')
+         names      ('update', 'field_name', 'object', 'request', 'kwargs', 'render_content')
          varnames   ('context', 'adapter', 'parent_context')
          freevars   ()
          cellvars   ()
          filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\tester\\wagtail_fedit\\templatetags\\fedit.py'
          name       'render_adapter'
-         firstlineno 198
-         lnotab 0x020204020801100106022a02140114011402
+         firstlineno 199
+         lnotab 0x020204020801100106022a021401140114023402
       'wagtail_fedit/_hook_output.html'
       'fedit_scripts'
       ('name', 'takes_context')
       code
          argcount  : 2
          nlocals   : 7
          stacksize : 6
@@ -1280,107 +1300,107 @@
             00530067007d04740f000000000000000000006a0800000000000000007c
             03a6010000ab01000000000000000044005d417d0502007c057c02a60100
             00ab0100000000000000007d067413000000000000000000007c06741400
             0000000000000000007416000000000000000000006602a6020000ab0200
             0000000000000073037c0667017d067c04a00c0000000000000000000000
             0000000000000000007c06a6010000ab01000000000000000001008c4264
             067c0469015300
-         215           0 RESUME                   0
+         218           0 RESUME                   0
          
-         217           2 LOAD_FAST                1 (css_or_js)
+         220           2 LOAD_FAST                1 (css_or_js)
                        4 LOAD_METHOD              0 (lower)
                       26 PRECALL                  0
                       30 CALL                     0
                       40 STORE_FAST               1 (css_or_js)
          
-         219          42 LOAD_FAST                1 (css_or_js)
+         222          42 LOAD_FAST                1 (css_or_js)
                       44 LOAD_CONST               1 (('css', 'js'))
                       46 CONTAINS_OP              1
                       48 POP_JUMP_FORWARD_IF_FALSE    15 (to 80)
          
-         220          50 LOAD_GLOBAL              3 (NULL + ValueError)
+         223          50 LOAD_GLOBAL              3 (NULL + ValueError)
                       62 LOAD_CONST               2 ("Invalid argument, must be 'css' or 'js'")
                       64 PRECALL                  1
                       68 CALL                     1
                       78 RAISE_VARARGS            1
          
-         222     >>   80 LOAD_FAST                0 (context)
+         225     >>   80 LOAD_FAST                0 (context)
                       82 LOAD_METHOD              2 (get)
                      104 LOAD_CONST               3 ('request')
                      106 PRECALL                  1
                      110 CALL                     1
                      120 STORE_FAST               2 (request)
          
-         224         122 LOAD_FAST                1 (css_or_js)
+         227         122 LOAD_FAST                1 (css_or_js)
                      124 LOAD_CONST               4 ('css')
                      126 COMPARE_OP               2 (==)
                      132 POP_JUMP_FORWARD_IF_FALSE     8 (to 150)
          
-         225         134 LOAD_GLOBAL              6 (REGISTER_CSS)
+         228         134 LOAD_GLOBAL              6 (REGISTER_CSS)
                      146 STORE_FAST               3 (hook_name)
                      148 JUMP_FORWARD             7 (to 164)
          
-         227     >>  150 LOAD_GLOBAL              8 (REGISTER_JS)
+         230     >>  150 LOAD_GLOBAL              8 (REGISTER_JS)
                      162 STORE_FAST               3 (hook_name)
          
-         229     >>  164 LOAD_GLOBAL             11 (NULL + getattr)
+         232     >>  164 LOAD_GLOBAL             11 (NULL + getattr)
                      176 LOAD_FAST                2 (request)
                      178 LOAD_GLOBAL             12 (FEDIT_PREVIEW_VAR)
                      190 LOAD_CONST               5 (False)
                      192 PRECALL                  3
                      196 CALL                     3
                      206 POP_JUMP_FORWARD_IF_TRUE     2 (to 212)
          
-         230         208 BUILD_MAP                0
+         233         208 BUILD_MAP                0
                      210 RETURN_VALUE
          
-         232     >>  212 BUILD_LIST               0
+         235     >>  212 BUILD_LIST               0
                      214 STORE_FAST               4 (files)
          
-         233         216 LOAD_GLOBAL             15 (NULL + hooks)
+         236         216 LOAD_GLOBAL             15 (NULL + hooks)
                      228 LOAD_ATTR                8 (get_hooks)
                      238 LOAD_FAST                3 (hook_name)
                      240 PRECALL                  1
                      244 CALL                     1
                      254 GET_ITER
                  >>  256 FOR_ITER                65 (to 388)
                      258 STORE_FAST               5 (hook)
          
-         234         260 PUSH_NULL
+         237         260 PUSH_NULL
                      262 LOAD_FAST                5 (hook)
                      264 LOAD_FAST                2 (request)
                      266 PRECALL                  1
                      270 CALL                     1
                      280 STORE_FAST               6 (ret)
          
-         236         282 LOAD_GLOBAL             19 (NULL + isinstance)
+         239         282 LOAD_GLOBAL             19 (NULL + isinstance)
                      294 LOAD_FAST                6 (ret)
                      296 LOAD_GLOBAL             20 (list)
                      308 LOAD_GLOBAL             22 (tuple)
                      320 BUILD_TUPLE              2
                      322 PRECALL                  2
                      326 CALL                     2
                      336 POP_JUMP_FORWARD_IF_TRUE     3 (to 344)
          
-         237         338 LOAD_FAST                6 (ret)
+         240         338 LOAD_FAST                6 (ret)
                      340 BUILD_LIST               1
                      342 STORE_FAST               6 (ret)
          
-         239     >>  344 LOAD_FAST                4 (files)
+         242     >>  344 LOAD_FAST                4 (files)
                      346 LOAD_METHOD             12 (extend)
                      368 LOAD_FAST                6 (ret)
                      370 PRECALL                  1
                      374 CALL                     1
                      384 POP_TOP
                      386 JUMP_BACKWARD           66 (to 256)
          
-         242     >>  388 LOAD_CONST               6 ('hook_output')
+         245     >>  388 LOAD_CONST               6 ('hook_output')
                      390 LOAD_FAST                4 (files)
          
-         241         392 BUILD_MAP                1
+         244         392 BUILD_MAP                1
                      394 RETURN_VALUE
          consts
             None
             ('css', 'js')
             "Invalid argument, must be 'css' or 'js'"
             'request'
             'css'
@@ -1388,15 +1408,15 @@
             'hook_output'
          names      ('lower', 'ValueError', 'get', 'REGISTER_CSS', 'REGISTER_JS', 'getattr', 'FEDIT_PREVIEW_VAR', 'hooks', 'get_hooks', 'isinstance', 'list', 'tuple', 'extend')
          varnames   ('context', 'css_or_js', 'request', 'hook_name', 'files', 'hook', 'ret')
          freevars   ()
          cellvars   ()
          filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\tester\\wagtail_fedit\\templatetags\\fedit.py'
          name       'static_hook_output'
-         firstlineno 215
+         firstlineno 218
          lnotab
             0x0202280208011e022a020c0110020e022c01040204012c011602380106
             022c0304ff
       False
       'tooltip'
       ('takes_context', 'name')
       'wrapping'
@@ -1412,37 +1432,37 @@
             00000064037c049b0064047405000000000000000000007c05a6010000ab
             0100000000000000009b0064059d05a6010000ab01000000000000000001
             008c2f6406a00300000000000000000000000000000000000000007c03a6
             010000ab0100000000000000007d067c01730f7409000000000000000000
             007c06a6010000ab01000000000000000053007409000000000000000000
             0064077c069b0064087c019b0064099d05a6010000ab0100000000000000
             005300
-         245           0 RESUME                   0
+         248           0 RESUME                   0
          
-         247           2 LOAD_FAST                0 (content)
+         250           2 LOAD_FAST                0 (content)
                        4 LOAD_FAST                2 (kwargs)
                        6 LOAD_CONST               1 ('content')
                        8 STORE_SUBSCR
          
-         249          12 LOAD_CONST               2 ("data-tooltip='true'")
+         252          12 LOAD_CONST               2 ("data-tooltip='true'")
          
-         248          14 BUILD_LIST               1
+         251          14 BUILD_LIST               1
                       16 STORE_FAST               3 (s)
          
-         251          18 LOAD_FAST                2 (kwargs)
+         254          18 LOAD_FAST                2 (kwargs)
                       20 LOAD_METHOD              0 (items)
                       42 PRECALL                  0
                       46 CALL                     0
                       56 GET_ITER
                  >>   58 FOR_ITER                46 (to 152)
                       60 UNPACK_SEQUENCE          2
                       64 STORE_FAST               4 (key)
                       66 STORE_FAST               5 (value)
          
-         252          68 LOAD_FAST                3 (s)
+         255          68 LOAD_FAST                3 (s)
                       70 LOAD_METHOD              1 (append)
                       92 LOAD_CONST               3 ('data-tooltip-')
                       94 LOAD_FAST                4 (key)
                       96 FORMAT_VALUE             0
                       98 LOAD_CONST               4 ("='")
                      100 LOAD_GLOBAL              5 (NULL + escape)
                      112 LOAD_FAST                5 (value)
@@ -1452,31 +1472,31 @@
                      130 LOAD_CONST               5 ("'")
                      132 BUILD_STRING             5
                      134 PRECALL                  1
                      138 CALL                     1
                      148 POP_TOP
                      150 JUMP_BACKWARD           47 (to 58)
          
-         253     >>  152 LOAD_CONST               6 (' ')
+         256     >>  152 LOAD_CONST               6 (' ')
                      154 LOAD_METHOD              3 (join)
                      176 LOAD_FAST                3 (s)
                      178 PRECALL                  1
                      182 CALL                     1
                      192 STORE_FAST               6 (attrs)
          
-         255         194 LOAD_FAST                1 (wrapping)
+         258         194 LOAD_FAST                1 (wrapping)
                      196 POP_JUMP_FORWARD_IF_TRUE    15 (to 228)
          
-         256         198 LOAD_GLOBAL              9 (NULL + mark_safe)
+         259         198 LOAD_GLOBAL              9 (NULL + mark_safe)
                      210 LOAD_FAST                6 (attrs)
                      212 PRECALL                  1
                      216 CALL                     1
                      226 RETURN_VALUE
          
-         258     >>  228 LOAD_GLOBAL              9 (NULL + mark_safe)
+         261     >>  228 LOAD_GLOBAL              9 (NULL + mark_safe)
                      240 LOAD_CONST               7 ('<span ')
                      242 LOAD_FAST                6 (attrs)
                      244 FORMAT_VALUE             0
                      246 LOAD_CONST               8 ('>')
                      248 LOAD_FAST                1 (wrapping)
                      250 FORMAT_VALUE             0
                      252 LOAD_CONST               9 ('</span>')
@@ -1497,15 +1517,15 @@
             '</span>'
          names      ('items', 'append', 'escape', 'join', 'mark_safe')
          varnames   ('content', 'wrapping', 'kwargs', 's', 'key', 'value', 'attrs')
          freevars   ()
          cellvars   ()
          filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\tester\\wagtail_fedit\\templatetags\\fedit.py'
          name       'tooltip'
-         firstlineno 245
+         firstlineno 248
          lnotab 0x02020a0202ff0403320154012a0204011e02
       'tokens'
       'kwarg_list'
       'absolute_tokens'
       'optional_tokens'
       code
          argcount  : 5
@@ -1536,235 +1556,235 @@
             0500000000000000000000000000000000000000007c0964031900000000
             0000000000a6010000ab0100000000000000007c067c0a3c00000064057d
             0590018c147c0244005d187d0c7c0c7c0676017212740d00000000000000
             00000064097c0c9b009d02a6010000ab01000000000000000082018c197c
             04a0070000000000000000000000000000000000000000a6000000ab0000
             0000000000000044005d0e5c0200007d0a7d0b7c0a7c06760172057c0b7c
             067c0a3c0000008c0f7c065300
-         261           0 RESUME                   0
+         264           0 RESUME                   0
          
-         262           2 LOAD_CONST               1 (False)
+         265           2 LOAD_CONST               1 (False)
                        4 STORE_FAST               5 (had_kwargs)
          
-         263           6 BUILD_MAP                0
+         266           6 BUILD_MAP                0
                        8 STORE_FAST               6 (kwargs)
          
-         265          10 LOAD_FAST                2 (kwarg_list)
+         268          10 LOAD_FAST                2 (kwarg_list)
                       12 POP_JUMP_FORWARD_IF_TRUE    14 (to 42)
          
-         266          14 LOAD_GLOBAL              1 (NULL + tuple)
+         269          14 LOAD_GLOBAL              1 (NULL + tuple)
                       26 PRECALL                  0
                       30 CALL                     0
                       40 STORE_FAST               2 (kwarg_list)
          
-         268     >>   42 LOAD_FAST                3 (absolute_tokens)
+         271     >>   42 LOAD_FAST                3 (absolute_tokens)
                       44 POP_JUMP_FORWARD_IF_TRUE    14 (to 74)
          
-         269          46 LOAD_GLOBAL              1 (NULL + tuple)
+         272          46 LOAD_GLOBAL              1 (NULL + tuple)
                       58 PRECALL                  0
                       62 CALL                     0
                       72 STORE_FAST               3 (absolute_tokens)
          
-         271     >>   74 LOAD_FAST                4 (optional_tokens)
+         274     >>   74 LOAD_FAST                4 (optional_tokens)
                       76 POP_JUMP_FORWARD_IF_TRUE     2 (to 82)
          
-         272          78 BUILD_MAP                0
+         275          78 BUILD_MAP                0
                       80 STORE_FAST               4 (optional_tokens)
          
-         274     >>   82 LOAD_GLOBAL              3 (NULL + enumerate)
+         277     >>   82 LOAD_GLOBAL              3 (NULL + enumerate)
                       94 LOAD_FAST                1 (tokens)
                       96 PRECALL                  1
                      100 CALL                     1
                      110 GET_ITER
                  >>  112 EXTENDED_ARG             1
                      114 FOR_ITER               274 (to 664)
                      116 UNPACK_SEQUENCE          2
                      120 STORE_FAST               7 (i)
                      122 STORE_FAST               8 (token)
          
-         275         124 LOAD_FAST                8 (token)
+         278         124 LOAD_FAST                8 (token)
                      126 LOAD_METHOD              2 (split)
                      148 LOAD_CONST               2 ('=')
                      150 PRECALL                  1
                      154 CALL                     1
                      164 STORE_FAST               9 (split)
          
-         276         166 LOAD_GLOBAL              7 (NULL + len)
+         279         166 LOAD_GLOBAL              7 (NULL + len)
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
          
-         277         242 LOAD_FAST                9 (split)
+         280         242 LOAD_FAST                9 (split)
                      244 LOAD_CONST               4 (0)
                      246 BINARY_SUBSCR
                      256 LOAD_FAST                3 (absolute_tokens)
                      258 CONTAINS_OP              0
                      260 POP_JUMP_FORWARD_IF_FALSE    12 (to 286)
          
-         278         262 LOAD_CONST               5 (True)
+         281         262 LOAD_CONST               5 (True)
                      264 LOAD_FAST                6 (kwargs)
                      266 LOAD_FAST                9 (split)
                      268 LOAD_CONST               4 (0)
                      270 BINARY_SUBSCR
                      280 STORE_SUBSCR
          
-         279         284 JUMP_BACKWARD           87 (to 112)
+         282         284 JUMP_BACKWARD           87 (to 112)
          
-         281     >>  286 LOAD_FAST                5 (had_kwargs)
+         284     >>  286 LOAD_FAST                5 (had_kwargs)
                      288 POP_JUMP_FORWARD_IF_FALSE    15 (to 320)
          
-         282         290 LOAD_GLOBAL              9 (NULL + ValueError)
+         285         290 LOAD_GLOBAL              9 (NULL + ValueError)
                      302 LOAD_CONST               6 ('Unexpected positional argument after keyword argument')
                      304 PRECALL                  1
                      308 CALL                     1
                      318 RAISE_VARARGS            1
          
-         284     >>  320 LOAD_FAST                0 (parser)
+         287     >>  320 LOAD_FAST                0 (parser)
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
          
-         285     >>  382 LOAD_GLOBAL              7 (NULL + len)
+         288     >>  382 LOAD_GLOBAL              7 (NULL + len)
                      394 LOAD_FAST                9 (split)
                      396 PRECALL                  1
                      400 CALL                     1
                      410 LOAD_CONST               3 (1)
                      412 COMPARE_OP               2 (==)
                      418 POP_JUMP_FORWARD_IF_FALSE    57 (to 534)
          
-         286         420 LOAD_FAST                9 (split)
+         289         420 LOAD_FAST                9 (split)
                      422 LOAD_CONST               4 (0)
                      424 BINARY_SUBSCR
                      434 LOAD_FAST                3 (absolute_tokens)
                      436 CONTAINS_OP              0
                      438 POP_JUMP_FORWARD_IF_FALSE    12 (to 464)
          
-         287         440 LOAD_CONST               5 (True)
+         290         440 LOAD_CONST               5 (True)
                      442 LOAD_FAST                6 (kwargs)
                      444 LOAD_FAST                9 (split)
                      446 LOAD_CONST               4 (0)
                      448 BINARY_SUBSCR
                      458 STORE_SUBSCR
          
-         288         462 JUMP_BACKWARD          176 (to 112)
+         291         462 JUMP_BACKWARD          176 (to 112)
          
-         290     >>  464 LOAD_FAST                9 (split)
+         293     >>  464 LOAD_FAST                9 (split)
                      466 LOAD_CONST               4 (0)
                      468 BINARY_SUBSCR
                      478 STORE_FAST              10 (key)
          
-         291         480 LOAD_FAST                0 (parser)
+         294         480 LOAD_FAST                0 (parser)
                      482 LOAD_METHOD              5 (compile_filter)
                      504 LOAD_FAST               10 (key)
                      506 PRECALL                  1
                      510 CALL                     1
                      520 STORE_FAST              11 (value)
          
-         292         522 LOAD_FAST               11 (value)
+         295         522 LOAD_FAST               11 (value)
                      524 LOAD_FAST                6 (kwargs)
                      526 LOAD_FAST               10 (key)
                      528 STORE_SUBSCR
                      532 JUMP_BACKWARD          211 (to 112)
          
-         294     >>  534 LOAD_FAST                9 (split)
+         297     >>  534 LOAD_FAST                9 (split)
                      536 LOAD_CONST               4 (0)
                      538 BINARY_SUBSCR
                      548 STORE_FAST              10 (key)
          
-         297         550 LOAD_FAST               10 (key)
+         300         550 LOAD_FAST               10 (key)
                      552 LOAD_FAST                3 (absolute_tokens)
                      554 CONTAINS_OP              0
                      556 POP_JUMP_FORWARD_IF_FALSE    19 (to 596)
          
-         298         558 LOAD_GLOBAL              9 (NULL + ValueError)
+         301         558 LOAD_GLOBAL              9 (NULL + ValueError)
                      570 LOAD_CONST               7 ('Keyword argument ')
                      572 LOAD_FAST               10 (key)
                      574 FORMAT_VALUE             0
                      576 LOAD_CONST               8 (' cannot be resolved; it will not be parsed as a variable.')
                      578 BUILD_STRING             3
                      580 PRECALL                  1
                      584 CALL                     1
                      594 RAISE_VARARGS            1
          
-         300     >>  596 LOAD_FAST                0 (parser)
+         303     >>  596 LOAD_FAST                0 (parser)
                      598 LOAD_METHOD              5 (compile_filter)
                      620 LOAD_FAST                9 (split)
                      622 LOAD_CONST               3 (1)
                      624 BINARY_SUBSCR
                      634 PRECALL                  1
                      638 CALL                     1
                      648 LOAD_FAST                6 (kwargs)
                      650 LOAD_FAST               10 (key)
                      652 STORE_SUBSCR
          
-         301         656 LOAD_CONST               5 (True)
+         304         656 LOAD_CONST               5 (True)
                      658 STORE_FAST               5 (had_kwargs)
                      660 EXTENDED_ARG             1
                      662 JUMP_BACKWARD          276 (to 112)
          
-         303     >>  664 LOAD_FAST                2 (kwarg_list)
+         306     >>  664 LOAD_FAST                2 (kwarg_list)
                      666 GET_ITER
                  >>  668 FOR_ITER                24 (to 718)
                      670 STORE_FAST              12 (kwarg)
          
-         304         672 LOAD_FAST               12 (kwarg)
+         307         672 LOAD_FAST               12 (kwarg)
                      674 LOAD_FAST                6 (kwargs)
                      676 CONTAINS_OP              1
                      678 POP_JUMP_FORWARD_IF_FALSE    18 (to 716)
          
-         305         680 LOAD_GLOBAL             13 (NULL + TemplateSyntaxError)
+         308         680 LOAD_GLOBAL             13 (NULL + TemplateSyntaxError)
                      692 LOAD_CONST               9 ('Missing required keyword argument ')
                      694 LOAD_FAST               12 (kwarg)
                      696 FORMAT_VALUE             0
                      698 BUILD_STRING             2
                      700 PRECALL                  1
                      704 CALL                     1
                      714 RAISE_VARARGS            1
          
-         304     >>  716 JUMP_BACKWARD           25 (to 668)
+         307     >>  716 JUMP_BACKWARD           25 (to 668)
          
-         307     >>  718 LOAD_FAST                4 (optional_tokens)
+         310     >>  718 LOAD_FAST                4 (optional_tokens)
                      720 LOAD_METHOD              7 (items)
                      742 PRECALL                  0
                      746 CALL                     0
                      756 GET_ITER
                  >>  758 FOR_ITER                14 (to 788)
                      760 UNPACK_SEQUENCE          2
                      764 STORE_FAST              10 (key)
                      766 STORE_FAST              11 (value)
          
-         308         768 LOAD_FAST               10 (key)
+         311         768 LOAD_FAST               10 (key)
                      770 LOAD_FAST                6 (kwargs)
                      772 CONTAINS_OP              1
                      774 POP_JUMP_FORWARD_IF_FALSE     5 (to 786)
          
-         309         776 LOAD_FAST               11 (value)
+         312         776 LOAD_FAST               11 (value)
                      778 LOAD_FAST                6 (kwargs)
                      780 LOAD_FAST               10 (key)
                      782 STORE_SUBSCR
                  >>  786 JUMP_BACKWARD           15 (to 758)
          
-         311     >>  788 LOAD_FAST                6 (kwargs)
+         314     >>  788 LOAD_FAST                6 (kwargs)
                      790 RETURN_VALUE
          consts
             None
             False
             '='
             1
             0
@@ -1775,15 +1795,15 @@
             'Missing required keyword argument '
          names      ('tuple', 'enumerate', 'split', 'len', 'ValueError', 'compile_filter', 'TemplateSyntaxError', 'items')
          varnames   ('parser', 'tokens', 'kwarg_list', 'absolute_tokens', 'optional_tokens', 'had_kwargs', 'kwargs', 'i', 'token', 'split', 'key', 'value', 'kwarg')
          freevars   ()
          cellvars   ()
          filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\tester\\wagtail_fedit\\templatetags\\fedit.py'
          name       'get_kwargs'
-         firstlineno 261
+         firstlineno 264
          lnotab
             0x02010401040204011c0204011c02040104022a012a014c011401160102
             0204011e023e01260114011601020210012a010c021003080126023c0108
             020801080124ff0203320108010c02
       (None,)
       (None, None, None)
    names      ('typing', 'Type', 'Any', 'django.template', 'library', 'Node', 'TemplateSyntaxError', 'django.template.context', 'Context', 'django.template.base', 'Parser', 'Token', 'FilterExpression', 'django.http', 'HttpRequest', 'django.utils.html', 'escape', 'django.utils.safestring', 'mark_safe', 'django.urls', 'reverse', 'django.core', 'signing', 'wagtail', 'hooks', 'warnings', 'adapters', 'adapter_registry', 'RegistryLookUpError', 'BaseAdapter', 'AdapterError', 'utils', 'wrap_adapter', '_can_edit', 'FEDIT_PREVIEW_VAR', 'TEMPLATE_TAG_NAME', 'REGISTER_CSS', 'REGISTER_JS', 'Library', 'register', 'WARNING_FIELD_NAME_NOT_AVAILABLE', 'WARNING_MODEL_INSTANCE_NOT_AVAILABLE', 'str', 'as_var', 'AdapterNode', 'tag', 'do_render_fedit', 'simple_tag', 'render_adapter', 'inclusion_tag', 'dict', 'static_hook_output', 'tooltip', 'list', 'get_kwargs')
@@ -1791,9 +1811,9 @@
    freevars   ()
    cellvars   ()
    filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\tester\\wagtail_fedit\\templatetags\\fedit.py'
    name       '<module>'
    firstlineno 1
    lnotab
       0x00ff0201100114030c0314040c010c010c010c010c020c020802180618
-      0610061e030401040318071c562a010eff0e0102392a0112ff0e0102102e
+      0610061e030401040318071c572a010eff0e0102392a0112ff0e0102122e
       010aff0e01021d2c0110ff0e01020f
```

### Comparing `wagtail_fedit-1.5.4rc2/wagtail_fedit/templatetags/fedit.py` & `wagtail_fedit-1.5.4rc3/wagtail_fedit/templatetags/fedit.py`

 * *Files 1% similar despite different names*

```diff
@@ -128,14 +128,15 @@
             field_name=field_name,
             request=request,
             **kwargs,
         )
 
         if not adapter.check_permissions()\
           or not _can_edit(request, obj):
+            context.update(adapter.kwargs)
             return as_var(self.as_var, context, adapter.render_content(context))
 
         return as_var(self.as_var, context, wrap_adapter(request, adapter, context))
 
 
 @register.tag(name=TEMPLATE_TAG_NAME)
 def do_render_fedit(parser: Parser, token: Token):
@@ -204,14 +205,16 @@
         del context["parent_context"]
 
     context.update(parent_context)
 
     context["wagtail_fedit_field"]    = adapter.field_name
     context["wagtail_fedit_instance"] = adapter.object
     context["request"]                = adapter.request
+    
+    context.update(adapter.kwargs)
 
     return adapter.render_content(context)
 
 
 @register.inclusion_tag("wagtail_fedit/_hook_output.html", name="fedit_scripts", takes_context=True)
 def static_hook_output(context, css_or_js) -> dict:
     css_or_js = css_or_js.lower()
```

### Comparing `wagtail_fedit-1.5.4rc2/wagtail_fedit/test/core/migrations/0001_initial.py` & `wagtail_fedit-1.5.4rc3/wagtail_fedit/test/core/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.4rc2/wagtail_fedit/test/core/models.py` & `wagtail_fedit-1.5.4rc3/wagtail_fedit/test/core/models.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.4rc2/wagtail_fedit/test/core/tests/base.py` & `wagtail_fedit-1.5.4rc3/wagtail_fedit/test/core/tests/base.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.4rc2/wagtail_fedit/test/core/tests/test_adapters.py` & `wagtail_fedit-1.5.4rc3/wagtail_fedit/test/core/tests/test_adapters.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.4rc2/wagtail_fedit/test/core/tests/test_block_edit.py` & `wagtail_fedit-1.5.4rc3/wagtail_fedit/test/core/tests/test_block_edit.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.4rc2/wagtail_fedit/test/core/tests/test_blocks.py` & `wagtail_fedit-1.5.4rc3/wagtail_fedit/test/core/tests/test_blocks.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.4rc2/wagtail_fedit/test/core/tests/test_field_edit.py` & `wagtail_fedit-1.5.4rc3/wagtail_fedit/test/core/tests/test_field_edit.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.4rc2/wagtail_fedit/test/core/tests/test_generic.py` & `wagtail_fedit-1.5.4rc3/wagtail_fedit/test/core/tests/test_generic.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.4rc2/wagtail_fedit/test/core/tests/test_model_edit.py` & `wagtail_fedit-1.5.4rc3/wagtail_fedit/test/core/tests/test_model_edit.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.4rc2/wagtail_fedit/test/core/tests/test_revision.py` & `wagtail_fedit-1.5.4rc3/wagtail_fedit/test/core/tests/test_revision.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.4rc2/wagtail_fedit/test/core/tests/test_submit.py` & `wagtail_fedit-1.5.4rc3/wagtail_fedit/test/core/tests/test_submit.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.4rc2/wagtail_fedit/test/manage.py` & `wagtail_fedit-1.5.4rc3/wagtail_fedit/test/manage.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.4rc2/wagtail_fedit/test/testapp/settings.py` & `wagtail_fedit-1.5.4rc3/wagtail_fedit/test/testapp/settings.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.4rc2/wagtail_fedit/test/testapp/urls.py` & `wagtail_fedit-1.5.4rc3/wagtail_fedit/test/testapp/urls.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.4rc2/wagtail_fedit/toolbar.py` & `wagtail_fedit-1.5.4rc3/wagtail_fedit/toolbar.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.4rc2/wagtail_fedit/urls.py` & `wagtail_fedit-1.5.4rc3/wagtail_fedit/urls.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,31 @@
 from django.urls import path
 from . import views
 
 app_name = "wagtail_fedit"
 
-urlpatterns = [
-    # Frontend Editing
-    path(
-        "edit/<str:adapter_id>/<str:app_label>/<str:model_name>/<str:model_id>/<str:field_name>/", 
-        views.EditAdapterView.as_view(), name="edit"
-    ),
-    path(
-        "edit/<str:adapter_id>/<str:app_label>/<str:model_name>/<str:model_id>/", 
-        views.EditAdapterView.as_view(), name="edit"
-    ),
-]
+urlpatterns = []
 
+adapter_based_views = (
+    ("edit", views.EditAdapterView),
+    ("refetch", views.AdapterRefetchView),
+)
+
+for name, view in adapter_based_views:
+    view.url_name = f"wagtail_fedit:{name}"
+    view.url_pattern = f"{name}/<str:adapter_id>/<str:app_label>/<str:model_name>/<str:model_id>/<str:field_name>/"
+    urlpatterns.append(
+        path(view.url_pattern, view.as_view(), name=name)
+    )
+    view.url_pattern = f"{name}/<str:adapter_id>/<str:app_label>/<str:model_name>/<str:model_id>/"
+    urlpatterns.append(
+        path(view.url_pattern, view.as_view(), name=name)
+    )
+
+# Model based views
 model_based_views = (
     ("editable", views.FEditableView),
     ("publish", views.PublishView),
     ("submit", views.SubmitView),
     ("unpublish", views.UnpublishView),
     ("cancel", views.CancelView),
 )
```

### Comparing `wagtail_fedit-1.5.4rc2/wagtail_fedit/utils.py` & `wagtail_fedit-1.5.4rc3/wagtail_fedit/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -501,10 +501,14 @@
             "js_constructor": js_constructor,
             "shared_context": adapter.kwargs,
             "parent_context": context,
             "edit_url": reverse(
                 "wagtail_fedit:edit",
                 kwargs=reverse_kwargs,
             ),
+            "refetch_url": reverse(
+                "wagtail_fedit:refetch",
+                kwargs=reverse_kwargs,
+            ),
         },
         request=request if run_context_processors else None,
     )
```

### Comparing `wagtail_fedit-1.5.4rc2/wagtail_fedit/views/adapters.py` & `wagtail_fedit-1.5.4rc3/wagtail_fedit/views/adapters.py`

 * *Files 2% similar despite different names*

```diff
@@ -163,14 +163,31 @@
             "verbose_name": verbose_name,
             "locked_for_user": self.locked_for_user,
             "shared_context": shared_context,
             "form_attrs": self.adapter.get_form_attrs(),
             "locked": self.lock is not None,
             **extra,
         }
+    
+class AdapterRefetchView(BaseAdapterView):
+    def get(self, request: HttpRequest, *args: Any, **kwargs: Any) -> HttpResponse:
+        context = self.get_context_data()
+        if isinstance(self.instance, Page):
+            # Add the page template variable to the context.
+            # Wagtail uses this internally; for example in `{% wagtailpagecache %}`
+            context[PAGE_TEMPLATE_VAR] = self.instance
+
+        return JsonResponse({
+            "success": True,
+            "refetch": True,
+            **self.adapter\
+              .get_response_data(
+                  self.get_context_data(),
+              ),
+        })
 
 class EditAdapterView(BaseAdapterView):
     def get(self, request: HttpRequest, *args: Any, **kwargs: Any) -> HttpResponse:
         # Can omit data from context - we are not rendering the content.
         form = self.adapter.get_form()
 
         return self.render_to_response(
```

### Comparing `wagtail_fedit-1.5.4rc2/wagtail_fedit/views/editable.py` & `wagtail_fedit-1.5.4rc3/wagtail_fedit/views/editable.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.4rc2/wagtail_fedit/views/mixins.py` & `wagtail_fedit-1.5.4rc3/wagtail_fedit/views/mixins.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.4rc2/wagtail_fedit/wagtail_hooks/action_menu.py` & `wagtail_fedit-1.5.4rc3/wagtail_fedit/wagtail_hooks/action_menu.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.4rc2/wagtail_fedit/wagtail_hooks/adapter_hooks.py` & `wagtail_fedit-1.5.4rc3/wagtail_fedit/wagtail_hooks/adapter_hooks.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.4rc2/wagtail_fedit/wagtail_hooks/log_actions.py` & `wagtail_fedit-1.5.4rc3/wagtail_fedit/wagtail_hooks/log_actions.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.4rc2/wagtail_fedit/wagtail_hooks/userbar.py` & `wagtail_fedit-1.5.4rc3/wagtail_fedit/wagtail_hooks/userbar.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.4rc2/wagtail_fedit.egg-info/PKG-INFO` & `wagtail_fedit-1.5.4rc3/wagtail_fedit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wagtail-fedit
-Version: 1.5.4rc2
+Version: 1.5.4rc3
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
-Metadata-Version: 2.1 Name: wagtail-fedit Version: 1.5.4rc2 Summary: Frontend
+Metadata-Version: 2.1 Name: wagtail-fedit Version: 1.5.4rc3 Summary: Frontend
 editing for your Wagtail site Home-page: https://github.com/Nigel2392/
 wagtail_fedit Author: Nigel Author-email: nigel@goodadvice.it License: GPL-2.0-
 only Classifier: Environment :: Web Environment Classifier: Framework :: Django
 Classifier: Framework :: Django :: 4.2 Classifier: Framework :: Wagtail
 Classifier: Framework :: Wagtail :: 5 Classifier: Framework :: Wagtail :: 6
 Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
 :: GNU General Public License v2 or later (GPLv2+) Classifier: Operating System
```

### Comparing `wagtail_fedit-1.5.4rc2/wagtail_fedit.egg-info/SOURCES.txt` & `wagtail_fedit-1.5.4rc3/wagtail_fedit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

