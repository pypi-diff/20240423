# Comparing `tmp/django-bootstrap5-24.1.tar.gz` & `tmp/django_bootstrap5-24.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-bootstrap5-24.1.tar", last modified: Fri Apr 12 08:20:08 2024, max compression
+gzip compressed data, was "django_bootstrap5-24.2.tar", last modified: Tue Apr 23 05:00:47 2024, max compression
```

## Comparing `django-bootstrap5-24.1.tar` & `django_bootstrap5-24.2.tar`

### file list

```diff
@@ -1,131 +1,127 @@
-drwxr-xr-x   0 dylan      (501) staff       (20)        0 2024-04-12 08:20:08.774009 django-bootstrap5-24.1/
-drwxr-xr-x   0 dylan      (501) staff       (20)        0 2024-04-12 08:20:08.755661 django-bootstrap5-24.1/.github/
--rw-r--r--   0 dylan      (501) staff       (20)      441 2021-12-12 13:22:34.000000 django-bootstrap5-24.1/.github/dependabot.yml
-drwxr-xr-x   0 dylan      (501) staff       (20)        0 2024-04-12 08:20:08.756079 django-bootstrap5-24.1/.github/workflows/
--rw-r--r--   0 dylan      (501) staff       (20)     1525 2024-04-12 08:10:50.000000 django-bootstrap5-24.1/.github/workflows/dependabot-auto-approve-and-merge.yml
--rw-r--r--   0 dylan      (501) staff       (20)     2967 2023-12-29 08:22:50.000000 django-bootstrap5-24.1/.github/workflows/test.yml
--rw-r--r--   0 dylan      (501) staff       (20)      587 2021-12-12 13:22:34.000000 django-bootstrap5-24.1/.gitignore
--rw-r--r--   0 dylan      (501) staff       (20)      206 2023-12-29 08:22:50.000000 django-bootstrap5-24.1/.readthedocs.yml
--rw-r--r--   0 dylan      (501) staff       (20)      757 2021-12-12 13:22:34.000000 django-bootstrap5-24.1/AUTHORS
--rw-r--r--   0 dylan      (501) staff       (20)     5411 2024-04-12 08:19:55.000000 django-bootstrap5-24.1/CHANGELOG.md
--rw-r--r--   0 dylan      (501) staff       (20)     2348 2023-12-29 08:22:50.000000 django-bootstrap5-24.1/CONTRIBUTING.md
--rw-r--r--   0 dylan      (501) staff       (20)     1533 2021-12-12 13:22:34.000000 django-bootstrap5-24.1/LICENSE
--rw-r--r--   0 dylan      (501) staff       (20)     1151 2021-12-12 13:22:34.000000 django-bootstrap5-24.1/MIGRATE.md
--rw-r--r--   0 dylan      (501) staff       (20)     1090 2023-12-29 08:22:50.000000 django-bootstrap5-24.1/Makefile
--rw-r--r--   0 dylan      (501) staff       (20)     5570 2024-04-12 08:20:08.773780 django-bootstrap5-24.1/PKG-INFO
--rw-r--r--   0 dylan      (501) staff       (20)     2346 2023-12-29 08:22:50.000000 django-bootstrap5-24.1/README.md
-drwxr-xr-x   0 dylan      (501) staff       (20)        0 2024-04-12 08:20:08.757995 django-bootstrap5-24.1/docs/
--rw-r--r--   0 dylan      (501) staff       (20)       30 2021-12-12 13:22:34.000000 django-bootstrap5-24.1/docs/changelog.rst
--rw-r--r--   0 dylan      (501) staff       (20)      566 2023-12-29 08:22:50.000000 django-bootstrap5-24.1/docs/conf.py
--rw-r--r--   0 dylan      (501) staff       (20)       34 2023-06-03 11:33:19.000000 django-bootstrap5-24.1/docs/contributing.rst
--rw-r--r--   0 dylan      (501) staff       (20)      577 2021-12-12 13:22:34.000000 django-bootstrap5-24.1/docs/example_template.rst
--rw-r--r--   0 dylan      (501) staff       (20)     3276 2021-12-12 13:22:34.000000 django-bootstrap5-24.1/docs/forms.rst
--rw-r--r--   0 dylan      (501) staff       (20)      265 2023-06-03 14:37:18.000000 django-bootstrap5-24.1/docs/index.rst
--rw-r--r--   0 dylan      (501) staff       (20)      585 2021-12-12 13:22:34.000000 django-bootstrap5-24.1/docs/installation.rst
--rw-r--r--   0 dylan      (501) staff       (20)       28 2021-12-12 13:22:34.000000 django-bootstrap5-24.1/docs/migrate.rst
--rw-r--r--   0 dylan      (501) staff       (20)      665 2021-12-12 13:22:34.000000 django-bootstrap5-24.1/docs/quickstart.rst
--rw-r--r--   0 dylan      (501) staff       (20)       55 2024-04-12 08:13:48.000000 django-bootstrap5-24.1/docs/requirements.txt
--rw-r--r--   0 dylan      (501) staff       (20)     3275 2023-12-29 08:24:07.000000 django-bootstrap5-24.1/docs/settings.rst
--rw-r--r--   0 dylan      (501) staff       (20)     1364 2021-12-12 13:22:34.000000 django-bootstrap5-24.1/docs/templates.rst
--rw-r--r--   0 dylan      (501) staff       (20)     2217 2021-12-12 13:22:34.000000 django-bootstrap5-24.1/docs/templatetags.rst
--rw-r--r--   0 dylan      (501) staff       (20)      799 2023-06-03 13:26:35.000000 django-bootstrap5-24.1/docs/widgets.rst
-drwxr-xr-x   0 dylan      (501) staff       (20)        0 2024-04-12 08:20:08.758584 django-bootstrap5-24.1/example/
--rw-r--r--   0 dylan      (501) staff       (20)        0 2021-12-12 13:22:34.000000 django-bootstrap5-24.1/example/__init__.py
-drwxr-xr-x   0 dylan      (501) staff       (20)        0 2024-04-12 08:20:08.759143 django-bootstrap5-24.1/example/app/
--rw-r--r--   0 dylan      (501) staff       (20)        0 2021-12-12 13:22:34.000000 django-bootstrap5-24.1/example/app/__init__.py
--rw-r--r--   0 dylan      (501) staff       (20)     4215 2021-12-12 13:22:34.000000 django-bootstrap5-24.1/example/app/forms.py
--rw-r--r--   0 dylan      (501) staff       (20)     2785 2022-02-27 06:07:14.000000 django-bootstrap5-24.1/example/app/views.py
--rwxr-xr-x   0 dylan      (501) staff       (20)      242 2021-12-12 13:22:34.000000 django-bootstrap5-24.1/example/manage.py
--rw-r--r--   0 dylan      (501) staff       (20)     5231 2021-12-12 13:22:34.000000 django-bootstrap5-24.1/example/settings.py
-drwxr-xr-x   0 dylan      (501) staff       (20)        0 2024-04-12 08:20:08.752555 django-bootstrap5-24.1/example/templates/
-drwxr-xr-x   0 dylan      (501) staff       (20)        0 2024-04-12 08:20:08.761206 django-bootstrap5-24.1/example/templates/app/
--rw-r--r--   0 dylan      (501) staff       (20)     1327 2021-12-12 13:22:34.000000 django-bootstrap5-24.1/example/templates/app/base.html
--rw-r--r--   0 dylan      (501) staff       (20)      125 2021-12-12 13:22:34.000000 django-bootstrap5-24.1/example/templates/app/bootstrap.html
--rw-r--r--   0 dylan      (501) staff       (20)      397 2021-12-12 13:22:34.000000 django-bootstrap5-24.1/example/templates/app/form.html
--rw-r--r--   0 dylan      (501) staff       (20)      549 2021-12-12 13:22:34.000000 django-bootstrap5-24.1/example/templates/app/form_by_field.html
--rw-r--r--   0 dylan      (501) staff       (20)      429 2021-12-12 13:22:34.000000 django-bootstrap5-24.1/example/templates/app/form_horizontal.html
--rw-r--r--   0 dylan      (501) staff       (20)      441 2021-12-12 13:22:34.000000 django-bootstrap5-24.1/example/templates/app/form_inline.html
--rw-r--r--   0 dylan      (501) staff       (20)      417 2021-12-12 13:22:34.000000 django-bootstrap5-24.1/example/templates/app/form_with_files.html
--rw-r--r--   0 dylan      (501) staff       (20)      443 2021-12-12 13:22:34.000000 django-bootstrap5-24.1/example/templates/app/formset.html
--rw-r--r--   0 dylan      (501) staff       (20)      205 2021-12-12 13:22:34.000000 django-bootstrap5-24.1/example/templates/app/home.html
--rw-r--r--   0 dylan      (501) staff       (20)      274 2021-12-12 13:22:34.000000 django-bootstrap5-24.1/example/templates/app/misc.html
--rw-r--r--   0 dylan      (501) staff       (20)      489 2021-12-12 13:22:34.000000 django-bootstrap5-24.1/example/templates/app/pagination.html
--rw-r--r--   0 dylan      (501) staff       (20)      898 2023-04-23 11:11:29.000000 django-bootstrap5-24.1/example/urls.py
--rwxr-xr-x   0 dylan      (501) staff       (20)      252 2021-12-12 13:22:34.000000 django-bootstrap5-24.1/manage.py
--rw-r--r--   0 dylan      (501) staff       (20)     2565 2024-04-12 08:19:55.000000 django-bootstrap5-24.1/pyproject.toml
--rw-r--r--   0 dylan      (501) staff       (20)      117 2024-04-12 08:19:55.000000 django-bootstrap5-24.1/requirements-dev.txt
--rw-r--r--   0 dylan      (501) staff       (20)       78 2024-04-12 08:19:55.000000 django-bootstrap5-24.1/requirements-test.txt
--rw-r--r--   0 dylan      (501) staff       (20)       38 2024-04-12 08:20:08.774050 django-bootstrap5-24.1/setup.cfg
-drwxr-xr-x   0 dylan      (501) staff       (20)        0 2024-04-12 08:20:08.752745 django-bootstrap5-24.1/src/
-drwxr-xr-x   0 dylan      (501) staff       (20)        0 2024-04-12 08:20:08.763904 django-bootstrap5-24.1/src/django_bootstrap5/
--rw-r--r--   0 dylan      (501) staff       (20)       93 2023-12-29 08:22:50.000000 django-bootstrap5-24.1/src/django_bootstrap5/__about__.py
--rw-r--r--   0 dylan      (501) staff       (20)       69 2023-06-03 11:33:19.000000 django-bootstrap5-24.1/src/django_bootstrap5/__init__.py
--rw-r--r--   0 dylan      (501) staff       (20)     2351 2022-08-05 14:34:59.000000 django-bootstrap5-24.1/src/django_bootstrap5/components.py
--rw-r--r--   0 dylan      (501) staff       (20)     2692 2023-12-29 08:24:07.000000 django-bootstrap5-24.1/src/django_bootstrap5/core.py
--rw-r--r--   0 dylan      (501) staff       (20)      621 2021-12-12 13:22:34.000000 django-bootstrap5-24.1/src/django_bootstrap5/css.py
--rw-r--r--   0 dylan      (501) staff       (20)     1482 2022-10-15 06:32:49.000000 django-bootstrap5-24.1/src/django_bootstrap5/forms.py
--rw-r--r--   0 dylan      (501) staff       (20)      870 2021-12-12 13:22:34.000000 django-bootstrap5-24.1/src/django_bootstrap5/html.py
--rw-r--r--   0 dylan      (501) staff       (20)    21369 2024-04-12 08:10:50.000000 django-bootstrap5-24.1/src/django_bootstrap5/renderers.py
--rw-r--r--   0 dylan      (501) staff       (20)      901 2021-12-12 13:22:34.000000 django-bootstrap5-24.1/src/django_bootstrap5/size.py
-drwxr-xr-x   0 dylan      (501) staff       (20)        0 2024-04-12 08:20:08.752873 django-bootstrap5-24.1/src/django_bootstrap5/templates/
-drwxr-xr-x   0 dylan      (501) staff       (20)        0 2024-04-12 08:20:08.765510 django-bootstrap5-24.1/src/django_bootstrap5/templates/django_bootstrap5/
--rw-r--r--   0 dylan      (501) staff       (20)     1079 2021-12-12 13:22:34.000000 django-bootstrap5-24.1/src/django_bootstrap5/templates/django_bootstrap5/bootstrap5.html
--rw-r--r--   0 dylan      (501) staff       (20)       95 2021-12-12 13:22:34.000000 django-bootstrap5-24.1/src/django_bootstrap5/templates/django_bootstrap5/field_errors.html
--rw-r--r--   0 dylan      (501) staff       (20)       79 2021-12-12 13:22:34.000000 django-bootstrap5-24.1/src/django_bootstrap5/templates/django_bootstrap5/field_help_text.html
--rw-r--r--   0 dylan      (501) staff       (20)      122 2021-12-12 13:22:34.000000 django-bootstrap5-24.1/src/django_bootstrap5/templates/django_bootstrap5/form_errors.html
--rw-r--r--   0 dylan      (501) staff       (20)      206 2021-12-12 13:22:34.000000 django-bootstrap5-24.1/src/django_bootstrap5/templates/django_bootstrap5/messages.html
--rw-r--r--   0 dylan      (501) staff       (20)     1762 2021-12-12 13:22:34.000000 django-bootstrap5-24.1/src/django_bootstrap5/templates/django_bootstrap5/pagination.html
-drwxr-xr-x   0 dylan      (501) staff       (20)        0 2024-04-12 08:20:08.766012 django-bootstrap5-24.1/src/django_bootstrap5/templates/django_bootstrap5/widgets/
--rw-r--r--   0 dylan      (501) staff       (20)      895 2021-12-12 13:22:34.000000 django-bootstrap5-24.1/src/django_bootstrap5/templates/django_bootstrap5/widgets/clearable_file_input.html
--rw-r--r--   0 dylan      (501) staff       (20)     1052 2021-12-12 13:22:34.000000 django-bootstrap5-24.1/src/django_bootstrap5/templates/django_bootstrap5/widgets/radio_select.html
--rw-r--r--   0 dylan      (501) staff       (20)      829 2024-04-12 08:10:50.000000 django-bootstrap5-24.1/src/django_bootstrap5/templates/django_bootstrap5/widgets/radio_select_button_group.html
-drwxr-xr-x   0 dylan      (501) staff       (20)        0 2024-04-12 08:20:08.766365 django-bootstrap5-24.1/src/django_bootstrap5/templatetags/
--rw-r--r--   0 dylan      (501) staff       (20)        0 2021-12-12 13:22:34.000000 django-bootstrap5-24.1/src/django_bootstrap5/templatetags/__init__.py
--rw-r--r--   0 dylan      (501) staff       (20)    19503 2023-12-29 08:22:50.000000 django-bootstrap5-24.1/src/django_bootstrap5/templatetags/django_bootstrap5.py
--rw-r--r--   0 dylan      (501) staff       (20)      467 2021-12-12 13:22:34.000000 django-bootstrap5-24.1/src/django_bootstrap5/text.py
--rw-r--r--   0 dylan      (501) staff       (20)     1497 2021-12-12 13:22:34.000000 django-bootstrap5-24.1/src/django_bootstrap5/utils.py
--rw-r--r--   0 dylan      (501) staff       (20)      745 2021-12-12 13:22:34.000000 django-bootstrap5-24.1/src/django_bootstrap5/widgets.py
-drwxr-xr-x   0 dylan      (501) staff       (20)        0 2024-04-12 08:20:08.773445 django-bootstrap5-24.1/src/django_bootstrap5.egg-info/
--rw-r--r--   0 dylan      (501) staff       (20)     5570 2024-04-12 08:20:08.000000 django-bootstrap5-24.1/src/django_bootstrap5.egg-info/PKG-INFO
--rw-r--r--   0 dylan      (501) staff       (20)     3510 2024-04-12 08:20:08.000000 django-bootstrap5-24.1/src/django_bootstrap5.egg-info/SOURCES.txt
--rw-r--r--   0 dylan      (501) staff       (20)        1 2024-04-12 08:20:08.000000 django-bootstrap5-24.1/src/django_bootstrap5.egg-info/dependency_links.txt
--rw-r--r--   0 dylan      (501) staff       (20)       12 2024-04-12 08:20:08.000000 django-bootstrap5-24.1/src/django_bootstrap5.egg-info/requires.txt
--rw-r--r--   0 dylan      (501) staff       (20)       18 2024-04-12 08:20:08.000000 django-bootstrap5-24.1/src/django_bootstrap5.egg-info/top_level.txt
-drwxr-xr-x   0 dylan      (501) staff       (20)        0 2024-04-12 08:20:08.772873 django-bootstrap5-24.1/tests/
--rw-r--r--   0 dylan      (501) staff       (20)        0 2021-12-12 13:22:34.000000 django-bootstrap5-24.1/tests/__init__.py
-drwxr-xr-x   0 dylan      (501) staff       (20)        0 2024-04-12 08:20:08.773251 django-bootstrap5-24.1/tests/app/
--rw-r--r--   0 dylan      (501) staff       (20)        0 2021-12-12 13:22:34.000000 django-bootstrap5-24.1/tests/app/__init__.py
--rw-r--r--   0 dylan      (501) staff       (20)     1703 2021-12-12 13:22:34.000000 django-bootstrap5-24.1/tests/app/settings.py
--rw-r--r--   0 dylan      (501) staff       (20)       17 2021-12-12 13:22:34.000000 django-bootstrap5-24.1/tests/app/urls.py
--rw-r--r--   0 dylan      (501) staff       (20)      549 2023-06-29 05:37:28.000000 django-bootstrap5-24.1/tests/base.py
--rw-r--r--   0 dylan      (501) staff       (20)     3439 2021-12-12 13:22:34.000000 django-bootstrap5-24.1/tests/image.py
--rw-r--r--   0 dylan      (501) staff       (20)     1595 2021-12-12 13:22:34.000000 django-bootstrap5-24.1/tests/test_bootstrap_alert.py
--rw-r--r--   0 dylan      (501) staff       (20)     2698 2021-12-12 13:22:34.000000 django-bootstrap5-24.1/tests/test_bootstrap_button.py
--rw-r--r--   0 dylan      (501) staff       (20)     2024 2021-12-12 13:22:34.000000 django-bootstrap5-24.1/tests/test_bootstrap_css_and_js_tags.py
--rw-r--r--   0 dylan      (501) staff       (20)     3282 2023-12-29 08:22:50.000000 django-bootstrap5-24.1/tests/test_bootstrap_field.py
--rw-r--r--   0 dylan      (501) staff       (20)     3343 2021-12-27 05:56:30.000000 django-bootstrap5-24.1/tests/test_bootstrap_field_datetime.py
--rw-r--r--   0 dylan      (501) staff       (20)     3797 2023-12-29 08:22:50.000000 django-bootstrap5-24.1/tests/test_bootstrap_field_input_checkbox.py
--rw-r--r--   0 dylan      (501) staff       (20)     2120 2023-06-29 05:47:36.000000 django-bootstrap5-24.1/tests/test_bootstrap_field_input_color.py
--rw-r--r--   0 dylan      (501) staff       (20)     3150 2021-12-12 13:22:34.000000 django-bootstrap5-24.1/tests/test_bootstrap_field_input_file.py
--rw-r--r--   0 dylan      (501) staff       (20)     2003 2021-12-12 13:22:34.000000 django-bootstrap5-24.1/tests/test_bootstrap_field_input_range.py
--rw-r--r--   0 dylan      (501) staff       (20)    12847 2023-12-29 08:22:50.000000 django-bootstrap5-24.1/tests/test_bootstrap_field_input_text.py
--rw-r--r--   0 dylan      (501) staff       (20)     3657 2023-04-23 08:55:44.000000 django-bootstrap5-24.1/tests/test_bootstrap_field_parameters.py
--rw-r--r--   0 dylan      (501) staff       (20)     4590 2021-12-12 13:22:34.000000 django-bootstrap5-24.1/tests/test_bootstrap_field_radio_select.py
--rw-r--r--   0 dylan      (501) staff       (20)     4545 2024-04-12 08:10:50.000000 django-bootstrap5-24.1/tests/test_bootstrap_field_radio_select_button_group.py
--rw-r--r--   0 dylan      (501) staff       (20)     2240 2023-06-29 05:55:16.000000 django-bootstrap5-24.1/tests/test_bootstrap_field_select.py
--rw-r--r--   0 dylan      (501) staff       (20)     1340 2021-12-12 13:22:34.000000 django-bootstrap5-24.1/tests/test_bootstrap_field_textarea.py
--rw-r--r--   0 dylan      (501) staff       (20)     8031 2023-12-29 08:24:07.000000 django-bootstrap5-24.1/tests/test_bootstrap_form.py
--rw-r--r--   0 dylan      (501) staff       (20)     1634 2021-12-12 13:22:34.000000 django-bootstrap5-24.1/tests/test_bootstrap_formset.py
--rw-r--r--   0 dylan      (501) staff       (20)      869 2022-10-15 06:31:02.000000 django-bootstrap5-24.1/tests/test_bootstrap_label.py
--rw-r--r--   0 dylan      (501) staff       (20)     2934 2022-08-05 14:34:59.000000 django-bootstrap5-24.1/tests/test_bootstrap_messages.py
--rw-r--r--   0 dylan      (501) staff       (20)     6807 2023-04-25 10:31:45.000000 django-bootstrap5-24.1/tests/test_bootstrap_pagination.py
--rw-r--r--   0 dylan      (501) staff       (20)     2600 2021-12-12 13:22:34.000000 django-bootstrap5-24.1/tests/test_components.py
--rw-r--r--   0 dylan      (501) staff       (20)      839 2021-12-12 13:22:34.000000 django-bootstrap5-24.1/tests/test_css.py
--rw-r--r--   0 dylan      (501) staff       (20)      511 2021-12-12 13:22:34.000000 django-bootstrap5-24.1/tests/test_html.py
--rw-r--r--   0 dylan      (501) staff       (20)      515 2021-12-12 13:22:34.000000 django-bootstrap5-24.1/tests/test_settings.py
--rw-r--r--   0 dylan      (501) staff       (20)     1149 2021-12-12 13:22:34.000000 django-bootstrap5-24.1/tests/test_size.py
--rw-r--r--   0 dylan      (501) staff       (20)      852 2021-12-12 13:22:34.000000 django-bootstrap5-24.1/tests/test_templates.py
--rw-r--r--   0 dylan      (501) staff       (20)      556 2021-12-12 13:22:34.000000 django-bootstrap5-24.1/tests/test_text.py
--rw-r--r--   0 dylan      (501) staff       (20)     1257 2023-04-23 08:55:44.000000 django-bootstrap5-24.1/tests/test_urls.py
--rw-r--r--   0 dylan      (501) staff       (20)      315 2021-12-12 13:22:34.000000 django-bootstrap5-24.1/tests/test_version.py
--rw-r--r--   0 dylan      (501) staff       (20)      983 2023-12-29 08:22:50.000000 django-bootstrap5-24.1/tox.ini
+drwxr-xr-x   0 dylan      (501) staff       (20)        0 2024-04-23 05:00:47.120102 django_bootstrap5-24.2/
+-rw-r--r--   0 dylan      (501) staff       (20)      299 2024-04-23 04:52:34.000000 django_bootstrap5-24.2/.editorconfig
+-rw-r--r--   0 dylan      (501) staff       (20)      333 2024-04-22 09:23:29.000000 django_bootstrap5-24.2/.readthedocs.yaml
+-rw-r--r--   0 dylan      (501) staff       (20)      757 2021-12-12 13:22:34.000000 django_bootstrap5-24.2/AUTHORS
+-rw-r--r--   0 dylan      (501) staff       (20)     5761 2024-04-23 05:00:31.000000 django_bootstrap5-24.2/CHANGELOG.md
+-rw-r--r--   0 dylan      (501) staff       (20)     2348 2024-04-18 06:47:16.000000 django_bootstrap5-24.2/CONTRIBUTING.md
+-rw-r--r--   0 dylan      (501) staff       (20)     1533 2021-12-12 13:22:34.000000 django_bootstrap5-24.2/LICENSE
+-rw-r--r--   0 dylan      (501) staff       (20)      329 2024-04-23 04:52:34.000000 django_bootstrap5-24.2/MANIFEST.in
+-rw-r--r--   0 dylan      (501) staff       (20)     1151 2021-12-12 13:22:34.000000 django_bootstrap5-24.2/MIGRATE.md
+-rw-r--r--   0 dylan      (501) staff       (20)     1155 2024-04-22 09:49:31.000000 django_bootstrap5-24.2/Makefile
+-rw-r--r--   0 dylan      (501) staff       (20)     5530 2024-04-23 05:00:47.119877 django_bootstrap5-24.2/PKG-INFO
+-rw-r--r--   0 dylan      (501) staff       (20)     2346 2023-12-29 08:22:50.000000 django_bootstrap5-24.2/README.md
+drwxr-xr-x   0 dylan      (501) staff       (20)        0 2024-04-23 05:00:47.103455 django_bootstrap5-24.2/docs/
+-rw-r--r--   0 dylan      (501) staff       (20)       61 2024-04-22 09:23:29.000000 django_bootstrap5-24.2/docs/changelog.rst
+-rw-r--r--   0 dylan      (501) staff       (20)      561 2024-04-22 09:23:29.000000 django_bootstrap5-24.2/docs/conf.py
+-rw-r--r--   0 dylan      (501) staff       (20)       64 2024-04-22 09:23:29.000000 django_bootstrap5-24.2/docs/contributing.rst
+-rw-r--r--   0 dylan      (501) staff       (20)      577 2021-12-12 13:22:34.000000 django_bootstrap5-24.2/docs/example_template.rst
+-rw-r--r--   0 dylan      (501) staff       (20)     3276 2021-12-12 13:22:34.000000 django_bootstrap5-24.2/docs/forms.rst
+-rw-r--r--   0 dylan      (501) staff       (20)      265 2023-06-03 14:37:18.000000 django_bootstrap5-24.2/docs/index.rst
+-rw-r--r--   0 dylan      (501) staff       (20)      585 2021-12-12 13:22:34.000000 django_bootstrap5-24.2/docs/installation.rst
+-rw-r--r--   0 dylan      (501) staff       (20)       59 2024-04-22 09:23:29.000000 django_bootstrap5-24.2/docs/migrate.rst
+-rw-r--r--   0 dylan      (501) staff       (20)      665 2021-12-12 13:22:34.000000 django_bootstrap5-24.2/docs/quickstart.rst
+-rw-r--r--   0 dylan      (501) staff       (20)       49 2024-04-22 09:23:29.000000 django_bootstrap5-24.2/docs/requirements.txt
+-rw-r--r--   0 dylan      (501) staff       (20)     3360 2024-04-23 04:42:32.000000 django_bootstrap5-24.2/docs/settings.rst
+-rw-r--r--   0 dylan      (501) staff       (20)     1364 2021-12-12 13:22:34.000000 django_bootstrap5-24.2/docs/templates.rst
+-rw-r--r--   0 dylan      (501) staff       (20)     2217 2021-12-12 13:22:34.000000 django_bootstrap5-24.2/docs/templatetags.rst
+-rw-r--r--   0 dylan      (501) staff       (20)      799 2023-06-03 13:26:35.000000 django_bootstrap5-24.2/docs/widgets.rst
+drwxr-xr-x   0 dylan      (501) staff       (20)        0 2024-04-23 05:00:47.104153 django_bootstrap5-24.2/example/
+-rw-r--r--   0 dylan      (501) staff       (20)        0 2021-12-12 13:22:34.000000 django_bootstrap5-24.2/example/__init__.py
+drwxr-xr-x   0 dylan      (501) staff       (20)        0 2024-04-23 05:00:47.104677 django_bootstrap5-24.2/example/app/
+-rw-r--r--   0 dylan      (501) staff       (20)        0 2021-12-12 13:22:34.000000 django_bootstrap5-24.2/example/app/__init__.py
+-rw-r--r--   0 dylan      (501) staff       (20)     4215 2021-12-12 13:22:34.000000 django_bootstrap5-24.2/example/app/forms.py
+-rw-r--r--   0 dylan      (501) staff       (20)     2785 2022-02-27 06:07:14.000000 django_bootstrap5-24.2/example/app/views.py
+-rwxr-xr-x   0 dylan      (501) staff       (20)      242 2021-12-12 13:22:34.000000 django_bootstrap5-24.2/example/manage.py
+-rw-r--r--   0 dylan      (501) staff       (20)     5292 2024-04-22 11:28:55.000000 django_bootstrap5-24.2/example/settings.py
+drwxr-xr-x   0 dylan      (501) staff       (20)        0 2024-04-23 05:00:47.098097 django_bootstrap5-24.2/example/templates/
+drwxr-xr-x   0 dylan      (501) staff       (20)        0 2024-04-23 05:00:47.106775 django_bootstrap5-24.2/example/templates/app/
+-rw-r--r--   0 dylan      (501) staff       (20)     1327 2021-12-12 13:22:34.000000 django_bootstrap5-24.2/example/templates/app/base.html
+-rw-r--r--   0 dylan      (501) staff       (20)      125 2021-12-12 13:22:34.000000 django_bootstrap5-24.2/example/templates/app/bootstrap.html
+-rw-r--r--   0 dylan      (501) staff       (20)      397 2021-12-12 13:22:34.000000 django_bootstrap5-24.2/example/templates/app/form.html
+-rw-r--r--   0 dylan      (501) staff       (20)      549 2021-12-12 13:22:34.000000 django_bootstrap5-24.2/example/templates/app/form_by_field.html
+-rw-r--r--   0 dylan      (501) staff       (20)      429 2021-12-12 13:22:34.000000 django_bootstrap5-24.2/example/templates/app/form_horizontal.html
+-rw-r--r--   0 dylan      (501) staff       (20)      441 2021-12-12 13:22:34.000000 django_bootstrap5-24.2/example/templates/app/form_inline.html
+-rw-r--r--   0 dylan      (501) staff       (20)      417 2021-12-12 13:22:34.000000 django_bootstrap5-24.2/example/templates/app/form_with_files.html
+-rw-r--r--   0 dylan      (501) staff       (20)      443 2021-12-12 13:22:34.000000 django_bootstrap5-24.2/example/templates/app/formset.html
+-rw-r--r--   0 dylan      (501) staff       (20)      205 2021-12-12 13:22:34.000000 django_bootstrap5-24.2/example/templates/app/home.html
+-rw-r--r--   0 dylan      (501) staff       (20)      274 2021-12-12 13:22:34.000000 django_bootstrap5-24.2/example/templates/app/misc.html
+-rw-r--r--   0 dylan      (501) staff       (20)      489 2021-12-12 13:22:34.000000 django_bootstrap5-24.2/example/templates/app/pagination.html
+-rw-r--r--   0 dylan      (501) staff       (20)      898 2023-04-23 11:11:29.000000 django_bootstrap5-24.2/example/urls.py
+-rwxr-xr-x   0 dylan      (501) staff       (20)      252 2021-12-12 13:22:34.000000 django_bootstrap5-24.2/manage.py
+-rw-r--r--   0 dylan      (501) staff       (20)     2568 2024-04-23 05:00:31.000000 django_bootstrap5-24.2/pyproject.toml
+-rw-r--r--   0 dylan      (501) staff       (20)      156 2024-04-22 09:23:29.000000 django_bootstrap5-24.2/requirements-dev.txt
+-rw-r--r--   0 dylan      (501) staff       (20)       78 2024-04-22 09:23:29.000000 django_bootstrap5-24.2/requirements-test.txt
+-rw-r--r--   0 dylan      (501) staff       (20)       38 2024-04-23 05:00:47.120139 django_bootstrap5-24.2/setup.cfg
+drwxr-xr-x   0 dylan      (501) staff       (20)        0 2024-04-23 05:00:47.098286 django_bootstrap5-24.2/src/
+drwxr-xr-x   0 dylan      (501) staff       (20)        0 2024-04-23 05:00:47.109437 django_bootstrap5-24.2/src/django_bootstrap5/
+-rw-r--r--   0 dylan      (501) staff       (20)       93 2023-12-29 08:22:50.000000 django_bootstrap5-24.2/src/django_bootstrap5/__about__.py
+-rw-r--r--   0 dylan      (501) staff       (20)       69 2023-06-03 11:33:19.000000 django_bootstrap5-24.2/src/django_bootstrap5/__init__.py
+-rw-r--r--   0 dylan      (501) staff       (20)     2351 2022-08-05 14:34:59.000000 django_bootstrap5-24.2/src/django_bootstrap5/components.py
+-rw-r--r--   0 dylan      (501) staff       (20)     2716 2024-04-22 11:28:55.000000 django_bootstrap5-24.2/src/django_bootstrap5/core.py
+-rw-r--r--   0 dylan      (501) staff       (20)      621 2021-12-12 13:22:34.000000 django_bootstrap5-24.2/src/django_bootstrap5/css.py
+-rw-r--r--   0 dylan      (501) staff       (20)     1482 2022-10-15 06:32:49.000000 django_bootstrap5-24.2/src/django_bootstrap5/forms.py
+-rw-r--r--   0 dylan      (501) staff       (20)      870 2021-12-12 13:22:34.000000 django_bootstrap5-24.2/src/django_bootstrap5/html.py
+-rw-r--r--   0 dylan      (501) staff       (20)    21369 2024-04-12 08:10:50.000000 django_bootstrap5-24.2/src/django_bootstrap5/renderers.py
+-rw-r--r--   0 dylan      (501) staff       (20)      901 2021-12-12 13:22:34.000000 django_bootstrap5-24.2/src/django_bootstrap5/size.py
+drwxr-xr-x   0 dylan      (501) staff       (20)        0 2024-04-23 05:00:47.098405 django_bootstrap5-24.2/src/django_bootstrap5/templates/
+drwxr-xr-x   0 dylan      (501) staff       (20)        0 2024-04-23 05:00:47.111047 django_bootstrap5-24.2/src/django_bootstrap5/templates/django_bootstrap5/
+-rw-r--r--   0 dylan      (501) staff       (20)     1220 2024-04-22 11:28:55.000000 django_bootstrap5-24.2/src/django_bootstrap5/templates/django_bootstrap5/bootstrap5.html
+-rw-r--r--   0 dylan      (501) staff       (20)       95 2021-12-12 13:22:34.000000 django_bootstrap5-24.2/src/django_bootstrap5/templates/django_bootstrap5/field_errors.html
+-rw-r--r--   0 dylan      (501) staff       (20)       79 2021-12-12 13:22:34.000000 django_bootstrap5-24.2/src/django_bootstrap5/templates/django_bootstrap5/field_help_text.html
+-rw-r--r--   0 dylan      (501) staff       (20)      122 2021-12-12 13:22:34.000000 django_bootstrap5-24.2/src/django_bootstrap5/templates/django_bootstrap5/form_errors.html
+-rw-r--r--   0 dylan      (501) staff       (20)      206 2021-12-12 13:22:34.000000 django_bootstrap5-24.2/src/django_bootstrap5/templates/django_bootstrap5/messages.html
+-rw-r--r--   0 dylan      (501) staff       (20)     1762 2021-12-12 13:22:34.000000 django_bootstrap5-24.2/src/django_bootstrap5/templates/django_bootstrap5/pagination.html
+drwxr-xr-x   0 dylan      (501) staff       (20)        0 2024-04-23 05:00:47.111494 django_bootstrap5-24.2/src/django_bootstrap5/templates/django_bootstrap5/widgets/
+-rw-r--r--   0 dylan      (501) staff       (20)      895 2021-12-12 13:22:34.000000 django_bootstrap5-24.2/src/django_bootstrap5/templates/django_bootstrap5/widgets/clearable_file_input.html
+-rw-r--r--   0 dylan      (501) staff       (20)     1052 2021-12-12 13:22:34.000000 django_bootstrap5-24.2/src/django_bootstrap5/templates/django_bootstrap5/widgets/radio_select.html
+-rw-r--r--   0 dylan      (501) staff       (20)      829 2024-04-12 08:10:50.000000 django_bootstrap5-24.2/src/django_bootstrap5/templates/django_bootstrap5/widgets/radio_select_button_group.html
+drwxr-xr-x   0 dylan      (501) staff       (20)        0 2024-04-23 05:00:47.111862 django_bootstrap5-24.2/src/django_bootstrap5/templatetags/
+-rw-r--r--   0 dylan      (501) staff       (20)        0 2021-12-12 13:22:34.000000 django_bootstrap5-24.2/src/django_bootstrap5/templatetags/__init__.py
+-rw-r--r--   0 dylan      (501) staff       (20)    19616 2024-04-22 11:28:55.000000 django_bootstrap5-24.2/src/django_bootstrap5/templatetags/django_bootstrap5.py
+-rw-r--r--   0 dylan      (501) staff       (20)      467 2021-12-12 13:22:34.000000 django_bootstrap5-24.2/src/django_bootstrap5/text.py
+-rw-r--r--   0 dylan      (501) staff       (20)     1497 2021-12-12 13:22:34.000000 django_bootstrap5-24.2/src/django_bootstrap5/utils.py
+-rw-r--r--   0 dylan      (501) staff       (20)      745 2021-12-12 13:22:34.000000 django_bootstrap5-24.2/src/django_bootstrap5/widgets.py
+drwxr-xr-x   0 dylan      (501) staff       (20)        0 2024-04-23 05:00:47.119586 django_bootstrap5-24.2/src/django_bootstrap5.egg-info/
+-rw-r--r--   0 dylan      (501) staff       (20)     5530 2024-04-23 05:00:47.000000 django_bootstrap5-24.2/src/django_bootstrap5.egg-info/PKG-INFO
+-rw-r--r--   0 dylan      (501) staff       (20)     3420 2024-04-23 05:00:47.000000 django_bootstrap5-24.2/src/django_bootstrap5.egg-info/SOURCES.txt
+-rw-r--r--   0 dylan      (501) staff       (20)        1 2024-04-23 05:00:47.000000 django_bootstrap5-24.2/src/django_bootstrap5.egg-info/dependency_links.txt
+-rw-r--r--   0 dylan      (501) staff       (20)       12 2024-04-23 05:00:47.000000 django_bootstrap5-24.2/src/django_bootstrap5.egg-info/requires.txt
+-rw-r--r--   0 dylan      (501) staff       (20)       18 2024-04-23 05:00:47.000000 django_bootstrap5-24.2/src/django_bootstrap5.egg-info/top_level.txt
+drwxr-xr-x   0 dylan      (501) staff       (20)        0 2024-04-23 05:00:47.119014 django_bootstrap5-24.2/tests/
+-rw-r--r--   0 dylan      (501) staff       (20)        0 2021-12-12 13:22:34.000000 django_bootstrap5-24.2/tests/__init__.py
+drwxr-xr-x   0 dylan      (501) staff       (20)        0 2024-04-23 05:00:47.119393 django_bootstrap5-24.2/tests/app/
+-rw-r--r--   0 dylan      (501) staff       (20)        0 2021-12-12 13:22:34.000000 django_bootstrap5-24.2/tests/app/__init__.py
+-rw-r--r--   0 dylan      (501) staff       (20)     1703 2021-12-12 13:22:34.000000 django_bootstrap5-24.2/tests/app/settings.py
+-rw-r--r--   0 dylan      (501) staff       (20)       17 2021-12-12 13:22:34.000000 django_bootstrap5-24.2/tests/app/urls.py
+-rw-r--r--   0 dylan      (501) staff       (20)      549 2023-06-29 05:37:28.000000 django_bootstrap5-24.2/tests/base.py
+-rw-r--r--   0 dylan      (501) staff       (20)     3439 2021-12-12 13:22:34.000000 django_bootstrap5-24.2/tests/image.py
+-rw-r--r--   0 dylan      (501) staff       (20)     1595 2021-12-12 13:22:34.000000 django_bootstrap5-24.2/tests/test_bootstrap_alert.py
+-rw-r--r--   0 dylan      (501) staff       (20)     2698 2021-12-12 13:22:34.000000 django_bootstrap5-24.2/tests/test_bootstrap_button.py
+-rw-r--r--   0 dylan      (501) staff       (20)     2186 2024-04-22 11:28:55.000000 django_bootstrap5-24.2/tests/test_bootstrap_css_and_js_tags.py
+-rw-r--r--   0 dylan      (501) staff       (20)     3282 2023-12-29 08:22:50.000000 django_bootstrap5-24.2/tests/test_bootstrap_field.py
+-rw-r--r--   0 dylan      (501) staff       (20)     3099 2024-04-23 04:42:32.000000 django_bootstrap5-24.2/tests/test_bootstrap_field_datetime.py
+-rw-r--r--   0 dylan      (501) staff       (20)     3797 2023-12-29 08:22:50.000000 django_bootstrap5-24.2/tests/test_bootstrap_field_input_checkbox.py
+-rw-r--r--   0 dylan      (501) staff       (20)     2120 2023-06-29 05:47:36.000000 django_bootstrap5-24.2/tests/test_bootstrap_field_input_color.py
+-rw-r--r--   0 dylan      (501) staff       (20)     3150 2021-12-12 13:22:34.000000 django_bootstrap5-24.2/tests/test_bootstrap_field_input_file.py
+-rw-r--r--   0 dylan      (501) staff       (20)     2003 2021-12-12 13:22:34.000000 django_bootstrap5-24.2/tests/test_bootstrap_field_input_range.py
+-rw-r--r--   0 dylan      (501) staff       (20)    12847 2023-12-29 08:22:50.000000 django_bootstrap5-24.2/tests/test_bootstrap_field_input_text.py
+-rw-r--r--   0 dylan      (501) staff       (20)     3657 2023-04-23 08:55:44.000000 django_bootstrap5-24.2/tests/test_bootstrap_field_parameters.py
+-rw-r--r--   0 dylan      (501) staff       (20)     4590 2024-04-22 11:35:51.000000 django_bootstrap5-24.2/tests/test_bootstrap_field_radio_select.py
+-rw-r--r--   0 dylan      (501) staff       (20)     4545 2024-04-22 11:35:51.000000 django_bootstrap5-24.2/tests/test_bootstrap_field_radio_select_button_group.py
+-rw-r--r--   0 dylan      (501) staff       (20)     2240 2023-06-29 05:55:16.000000 django_bootstrap5-24.2/tests/test_bootstrap_field_select.py
+-rw-r--r--   0 dylan      (501) staff       (20)     1340 2021-12-12 13:22:34.000000 django_bootstrap5-24.2/tests/test_bootstrap_field_textarea.py
+-rw-r--r--   0 dylan      (501) staff       (20)     8031 2023-12-29 08:24:07.000000 django_bootstrap5-24.2/tests/test_bootstrap_form.py
+-rw-r--r--   0 dylan      (501) staff       (20)     1634 2021-12-12 13:22:34.000000 django_bootstrap5-24.2/tests/test_bootstrap_formset.py
+-rw-r--r--   0 dylan      (501) staff       (20)      869 2022-10-15 06:31:02.000000 django_bootstrap5-24.2/tests/test_bootstrap_label.py
+-rw-r--r--   0 dylan      (501) staff       (20)     2934 2022-08-05 14:34:59.000000 django_bootstrap5-24.2/tests/test_bootstrap_messages.py
+-rw-r--r--   0 dylan      (501) staff       (20)     6807 2023-04-25 10:31:45.000000 django_bootstrap5-24.2/tests/test_bootstrap_pagination.py
+-rw-r--r--   0 dylan      (501) staff       (20)     2600 2021-12-12 13:22:34.000000 django_bootstrap5-24.2/tests/test_components.py
+-rw-r--r--   0 dylan      (501) staff       (20)      839 2021-12-12 13:22:34.000000 django_bootstrap5-24.2/tests/test_css.py
+-rw-r--r--   0 dylan      (501) staff       (20)      511 2021-12-12 13:22:34.000000 django_bootstrap5-24.2/tests/test_html.py
+-rw-r--r--   0 dylan      (501) staff       (20)      515 2021-12-12 13:22:34.000000 django_bootstrap5-24.2/tests/test_settings.py
+-rw-r--r--   0 dylan      (501) staff       (20)     1149 2021-12-12 13:22:34.000000 django_bootstrap5-24.2/tests/test_size.py
+-rw-r--r--   0 dylan      (501) staff       (20)     1366 2024-04-22 11:28:55.000000 django_bootstrap5-24.2/tests/test_templates.py
+-rw-r--r--   0 dylan      (501) staff       (20)      556 2021-12-12 13:22:34.000000 django_bootstrap5-24.2/tests/test_text.py
+-rw-r--r--   0 dylan      (501) staff       (20)     1257 2023-04-23 08:55:44.000000 django_bootstrap5-24.2/tests/test_urls.py
+-rw-r--r--   0 dylan      (501) staff       (20)      315 2021-12-12 13:22:34.000000 django_bootstrap5-24.2/tests/test_version.py
+-rw-r--r--   0 dylan      (501) staff       (20)      866 2024-04-23 04:42:32.000000 django_bootstrap5-24.2/tox.ini
```

### Comparing `django-bootstrap5-24.1/AUTHORS` & `django_bootstrap5-24.2/AUTHORS`

 * *Files identical despite different names*

### Comparing `django-bootstrap5-24.1/CHANGELOG.md` & `django_bootstrap5-24.2/CHANGELOG.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,20 @@
 # Changelog
 
+## 24.2 (2024-04-23)
+
+- Add .editorconfig (#598).
+- Remove support for Django 4.1 (EOL) (#597).
+- Add support for color mode (#593).
+- Change bootstrap_setting from filter to tag (#595).
+- Remove support for Python 3.7 (EOL) (#588).
+- Remove support for Django 3.2 (EOL) (#583).
+- Update Bootstrap to 5.3.3 (#584).
+- Fix Read the Docs (#585, #587).
+
 ## 24.1 (2024-04-12)
 
 - Fix RadioSelectButtonGroup rendering and add 'disabled' attribute to radio button group template (#447).
 
 ## 23.4 (2023-12-28)
 
 - Use ruff instead of black for formatting (#536).
```

### Comparing `django-bootstrap5-24.1/CONTRIBUTING.md` & `django_bootstrap5-24.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `django-bootstrap5-24.1/LICENSE` & `django_bootstrap5-24.2/LICENSE`

 * *Files identical despite different names*

### Comparing `django-bootstrap5-24.1/MIGRATE.md` & `django_bootstrap5-24.2/MIGRATE.md`

 * *Files identical despite different names*

### Comparing `django-bootstrap5-24.1/Makefile` & `django_bootstrap5-24.2/Makefile`

 * *Files 10% similar despite different names*

```diff
@@ -8,19 +8,19 @@
 .PHONY: tests
 tests:
 	tox
 
 .PHONY: reformat
 reformat:
 	ruff format .
-	ruff --fix .
+	ruff check . --fix
 
 .PHONY: lint
 lint:
-	ruff .
+	ruff check .
 
 .PHONY: docs
 docs: clean
 	cd docs && sphinx-build -b html -d _build/doctrees . _build/html
 
 .PHONY: example
 example:
@@ -41,20 +41,23 @@
 	@echo "On branch main."
 else
 	@echo "Error - Not on branch main."
 	@exit 1;
 endif
 
 .PHONY: build
-build: docs
+build:
 	python -m build
+	twine check dist/*
+	check-manifest
+	pyroma .
+	check-wheel-contents dist
 
 .PHONY: publish
-publish: porcelain branch build
-	twine check dist/*
+publish: porcelain branch docs build
 	twine upload dist/*
 	git tag -a v${VERSION} -m "Release ${VERSION}"
 	git push origin --tags
 
 .PHONY: clean
 clean:
 	rm -rf build dist src/*.egg-info .coverage*
```

### Comparing `django-bootstrap5-24.1/PKG-INFO` & `django_bootstrap5-24.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-bootstrap5
-Version: 24.1
+Version: 24.2
 Summary: Bootstrap 5 for Django
 Author-email: Dylan Verheul <dylan@dyve.net>
 License: BSD 3-Clause License
         
         Copyright (c) Zostera B.V. and individual contributors
         All rights reserved.
         
@@ -33,19 +33,18 @@
         OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
         OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 Project-URL: Changelog, https://github.com/zostera/django-bootstrap5/blob/main/CHANGELOG.md
 Project-URL: Documentation, https://django-bootstrap5.readthedocs.io/
 Project-URL: Homepage, https://github.com/zostera/django-bootstrap5
 Project-URL: Issues, https://github.com/zostera/django-bootstrap5/issues
 Project-URL: Source, https://github.com/zostera/django-bootstrap5
+Keywords: django,bootstrap,bootstrap5
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 3.2
-Classifier: Framework :: Django :: 4.1
 Classifier: Framework :: Django :: 4.2
 Classifier: Framework :: Django :: 5.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -55,15 +54,15 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Utilities
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: AUTHORS
-Requires-Dist: Django>=3.2
+Requires-Dist: Django>=4.2
 
 # django-bootstrap5
 
 [![CI](https://github.com/zostera/django-bootstrap5/workflows/CI/badge.svg?branch=main)](https://github.com/zostera/django-bootstrap5/actions?workflow=CI)
 [![Coverage Status](https://coveralls.io/repos/github/zostera/django-bootstrap5/badge.svg?branch=main)](https://coveralls.io/github/zostera/django-bootstrap5?branch=main)
 [![Latest PyPI version](https://img.shields.io/pypi/v/django-bootstrap5.svg)](https://pypi.python.org/pypi/django-bootstrap5)
```

### Comparing `django-bootstrap5-24.1/README.md` & `django_bootstrap5-24.2/README.md`

 * *Files identical despite different names*

### Comparing `django-bootstrap5-24.1/docs/conf.py` & `django_bootstrap5-24.2/docs/conf.py`

 * *Files 20% similar despite different names*

```diff
@@ -11,13 +11,13 @@
 author = ", ".join(author["name"] for author in pyproject["project"]["authors"])
 year = datetime.now().year
 copyright = f"{year}, {author}"
 
 extensions = [
     "sphinx.ext.autodoc",
     "sphinx.ext.viewcode",
-    "sphinx_mdinclude",
+    "myst_parser",
 ]
 
 htmlhelp_basename = f"{project}-doc"
 html_theme = "furo"
 pygments_style = "sphinx"
```

### Comparing `django-bootstrap5-24.1/docs/example_template.rst` & `django_bootstrap5-24.2/docs/example_template.rst`

 * *Files identical despite different names*

### Comparing `django-bootstrap5-24.1/docs/forms.rst` & `django_bootstrap5-24.2/docs/forms.rst`

 * *Files identical despite different names*

### Comparing `django-bootstrap5-24.1/docs/installation.rst` & `django_bootstrap5-24.2/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `django-bootstrap5-24.1/docs/quickstart.rst` & `django_bootstrap5-24.2/docs/quickstart.rst`

 * *Files identical despite different names*

### Comparing `django-bootstrap5-24.1/docs/settings.rst` & `django_bootstrap5-24.2/docs/settings.rst`

 * *Files 3% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 .. code:: django
 
     # Default settings
     BOOTSTRAP5 = {
 
         # The complete URL to the Bootstrap CSS file.
         # Note that a URL can be either a string
-        # ("https://stackpath.bootstrapcdn.com/bootstrap/4.1.1/css/bootstrap.min.css"),
+        # ("https://cdn.jsdelivr.net/npm/bootstrap@5.2.0/dist/css/bootstrap.min.css"),
         # or a dict with keys `url`, `integrity` and `crossorigin` like the default value below.
         "css_url": {
             "url": "https://cdn.jsdelivr.net/npm/bootstrap@5.2.0/dist/css/bootstrap.min.css",
             "integrity": "sha384-gH2yIJqKdNHPEq0n4Mqa/HGKIhSkIHeL5AyhkYV8i59U5AR6csBvApHHNl/vI1Bx",
             "crossorigin": "anonymous",
         },
 
@@ -30,14 +30,17 @@
             "integrity": "sha384-A3rJD856KowSb7dwlZdYEkO39Gagi7vIsF0jrRAoQmDKKtQBHUuLZ9AsSv4jD4Xa",
             "crossorigin": "anonymous",
         },
 
         # The complete URL to the Bootstrap CSS theme file (None means no theme).
         "theme_url": None,
 
+        # Color mode (None means do not set color mode).
+        "color_mode": None,
+
         # Put JavaScript in the HEAD section of the HTML document (only relevant if you use bootstrap5.html).
         'javascript_in_head': False,
 
         # Wrapper class for non-inline fields.
         # The default value "mb-3" is the spacing as used by Bootstrap 5 example code.
         'wrapper_class': 'mb-3',
```

### Comparing `django-bootstrap5-24.1/docs/templates.rst` & `django_bootstrap5-24.2/docs/templates.rst`

 * *Files identical despite different names*

### Comparing `django-bootstrap5-24.1/docs/templatetags.rst` & `django_bootstrap5-24.2/docs/templatetags.rst`

 * *Files identical despite different names*

### Comparing `django-bootstrap5-24.1/docs/widgets.rst` & `django_bootstrap5-24.2/docs/widgets.rst`

 * *Files identical despite different names*

### Comparing `django-bootstrap5-24.1/example/app/forms.py` & `django_bootstrap5-24.2/example/app/forms.py`

 * *Files identical despite different names*

### Comparing `django-bootstrap5-24.1/example/app/views.py` & `django_bootstrap5-24.2/example/app/views.py`

 * *Files identical despite different names*

### Comparing `django-bootstrap5-24.1/example/settings.py` & `django_bootstrap5-24.2/example/settings.py`

 * *Files 4% similar despite different names*

```diff
@@ -137,15 +137,21 @@
     "handlers": {
         "mail_admins": {
             "level": "ERROR",
             "filters": ["require_debug_false"],
             "class": "django.utils.log.AdminEmailHandler",
         }
     },
-    "loggers": {"django.request": {"handlers": ["mail_admins"], "level": "ERROR", "propagate": True}},
+    "loggers": {
+        "django.request": {
+            "handlers": ["mail_admins"],
+            "level": "ERROR",
+            "propagate": True,
+        }
+    },
 }
 
 # Settings for django-bootstrap5
 BOOTSTRAP5 = {
     "error_css_class": "django_bootstrap5-error",
     "required_css_class": "django_bootstrap5-required",
     "javascript_in_head": True,
```

### Comparing `django-bootstrap5-24.1/example/templates/app/base.html` & `django_bootstrap5-24.2/example/templates/app/base.html`

 * *Files identical despite different names*

### Comparing `django-bootstrap5-24.1/example/templates/app/form_by_field.html` & `django_bootstrap5-24.2/example/templates/app/form_by_field.html`

 * *Files identical despite different names*

### Comparing `django-bootstrap5-24.1/example/urls.py` & `django_bootstrap5-24.2/example/urls.py`

 * *Files identical despite different names*

### Comparing `django-bootstrap5-24.1/pyproject.toml` & `django_bootstrap5-24.2/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,85 +1,86 @@
 [build-system]
 build-backend = "setuptools.build_meta"
-requires = ["setuptools>=64", "setuptools_scm>=8"]
+requires = ["setuptools>=64"]
 
 [project]
 authors = [
   {name = "Dylan Verheul", email = "dylan@dyve.net"},
 ]
 classifiers = [
   "Development Status :: 5 - Production/Stable",
   "Environment :: Web Environment",
   "Framework :: Django",
-  "Framework :: Django :: 3.2",
-  "Framework :: Django :: 4.1",
   "Framework :: Django :: 4.2",
   "Framework :: Django :: 5.0",
   "Intended Audience :: Developers",
   "License :: OSI Approved :: BSD License",
   "Operating System :: OS Independent",
   "Programming Language :: Python :: 3",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: 3.12",
   "Topic :: Software Development :: Libraries",
   "Topic :: Utilities",
 ]
-dependencies = ["Django>=3.2"]
+dependencies = ["Django>=4.2"]
 description = "Bootstrap 5 for Django"
+keywords = ["django", "bootstrap", "bootstrap5"]
 license = {file = "LICENSE"}
 name = "django-bootstrap5"
 readme = "README.md"
 requires-python = ">=3.8"
-version = "24.1"
+version = "24.2"
 
 [project.urls]
 Changelog = "https://github.com/zostera/django-bootstrap5/blob/main/CHANGELOG.md"
 Documentation = "https://django-bootstrap5.readthedocs.io/"
 Homepage = "https://github.com/zostera/django-bootstrap5"
 Issues = "https://github.com/zostera/django-bootstrap5/issues"
 Source = "https://github.com/zostera/django-bootstrap5"
 
 [tool.ruff]
 fix = false
+line-length = 120
+src = ["src"]
+target-version = "py38"
+
+[tool.ruff.lint]
 fixable = [
   "I001", # isort (sorting)
   "F", # flake8
   "D", # docformatter
   "UP", # pyupgrade
 ]
 ignore = [
   "D1", # D1: Missing docstring error codes (because not every function and class has a docstring)
   "D203", # D203: 1 blank line required before class docstring (conflicts with D211 and should be disabled, see https://github.com/PyCQA/pydocstyle/pull/91)
   "D212", # D212: Multi-line docstring summary should start at the first line
   "D301", # D301: Use r”“” if any backslashes in a docstring (unclear how else to handle backslashes in docstrings)
 ]
-line-length = 120
 select = [
   "D", # pydocstyle
   "E", # pycodestyle
   "F", # flake8
   "I", # isort
   "UP", # pyupgrade
 ]
-src = ["src"]
-target-version = "py38"
 unfixable = [
   "F8", # names in flake8, such as defined but unused variables
 ]
 
-[tool.ruff.isort]
-known-first-party = ["django_marina", "app"]
+[tool.ruff.lint.isort]
+known-first-party = ["django_bootstrap5", "app"]
 known-third-party = ["django"]
 
 [tool.coverage.run]
 branch = true
 source = ["src", "tests"]
 
 [tool.coverage.paths]
-package = ["src/django_marina", "*/django_marina/src/django_marina"]
+package = ["src/django_bootstrap5", "*/django_bootstrap5/src/django_bootstrap5"]
 
 [tool.coverage.report]
 show_missing = true
 skip_covered = true
```

### Comparing `django-bootstrap5-24.1/src/django_bootstrap5/components.py` & `django_bootstrap5-24.2/src/django_bootstrap5/components.py`

 * *Files identical despite different names*

### Comparing `django-bootstrap5-24.1/src/django_bootstrap5/core.py` & `django_bootstrap5-24.2/src/django_bootstrap5/core.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 from importlib import import_module
 
 from django.conf import settings
 
 BOOTSTRAP5 = {"foo": "bar"}
 BOOTSTRAP5_DEFAULTS = {
     "css_url": {
-        "url": "https://cdn.jsdelivr.net/npm/bootstrap@5.2.3/dist/css/bootstrap.min.css",
-        "integrity": "sha384-rbsA2VBKQhggwzxH7pPCaAqO46MgnOM80zW1RWuH61DGLwZJEdK2Kadq2F9CUG65",
+        "url": "https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/css/bootstrap.min.css",
+        "integrity": "sha384-QWTKZyjpPEjISv5WaRU9OFeRpok6YctnYmDr5pNlyT2bRjXh0JMhjY6hW+ALEwIH",
         "crossorigin": "anonymous",
     },
     "javascript_url": {
-        "url": "https://cdn.jsdelivr.net/npm/bootstrap@5.2.3/dist/js/bootstrap.bundle.min.js",
-        "integrity": "sha384-kenU1KFdBIe4zVF0s0G1M5b4hcpxyD9F7jL+jjXkk+Q2h455rYXK/7HAuoJl+0I4",
+        "url": "https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/js/bootstrap.bundle.min.js",
+        "integrity": "sha384-YvpcrYf0tY3lHB60NNkmXc5s9fDVZLESaAA55NDzOxhy9GkcIdslK1eN7N6jIeHz",
         "crossorigin": "anonymous",
     },
     "theme_url": None,
+    "color_mode": None,
     "javascript_in_head": False,
     "wrapper_class": "mb-3",
     "inline_wrapper_class": "",
     "horizontal_label_class": "col-sm-2",
     "horizontal_field_class": "col-sm-10",
     "horizontal_field_offset_class": "offset-sm-2",
     "set_placeholder": True,
```

### Comparing `django-bootstrap5-24.1/src/django_bootstrap5/css.py` & `django_bootstrap5-24.2/src/django_bootstrap5/css.py`

 * *Files identical despite different names*

### Comparing `django-bootstrap5-24.1/src/django_bootstrap5/forms.py` & `django_bootstrap5-24.2/src/django_bootstrap5/forms.py`

 * *Files identical despite different names*

### Comparing `django-bootstrap5-24.1/src/django_bootstrap5/html.py` & `django_bootstrap5-24.2/src/django_bootstrap5/html.py`

 * *Files identical despite different names*

### Comparing `django-bootstrap5-24.1/src/django_bootstrap5/renderers.py` & `django_bootstrap5-24.2/src/django_bootstrap5/renderers.py`

 * *Files identical despite different names*

### Comparing `django-bootstrap5-24.1/src/django_bootstrap5/size.py` & `django_bootstrap5-24.2/src/django_bootstrap5/size.py`

 * *Files identical despite different names*

### Comparing `django-bootstrap5-24.1/src/django_bootstrap5/templates/django_bootstrap5/bootstrap5.html` & `django_bootstrap5-24.2/src/django_bootstrap5/templates/django_bootstrap5/bootstrap5.html`

 * *Files 24% similar despite different names*

```diff
@@ -1,42 +1,32 @@
 <!DOCTYPE html>
 {% load django_bootstrap5 %}
 {% load i18n %}
 {% get_current_language as LANGUAGE_CODE %}
-<html lang="{{ LANGUAGE_CODE|default:'en_us' }}">
-
+{% bootstrap_setting "color_mode" as COLOR_MODE %}
+{% bootstrap_setting "javascript_in_head" as BOOTSTRAP_JAVASCRIPT_IN_HEAD %}
+<html lang="{{ LANGUAGE_CODE|default:'en_us' }}"{% if COLOR_MODE %} data-bs-theme="{{ COLOR_MODE }}"{% endif %}>
 <head>
-
     <!-- Required meta tags -->
     <meta charset="utf-8">
     <meta name="viewport" content="width=device-width, initial-scale=1, shrink-to-fit=no">
-
     <!-- Page title -->
     <title>{% block bootstrap5_title %}django-bootstrap5 template title{% endblock %}</title>
-
     <!-- Bootstrap CSS -->
     {% bootstrap_css %}
-
     <!-- Bootstrap JavaScript if it is in head -->
-    {% if 'javascript_in_head'|bootstrap_setting %}
-        {% bootstrap_javascript %}
-    {% endif %}
-
-    {% block bootstrap5_extra_head %}{% endblock %}
+    {% if BOOTSTRAP_JAVASCRIPT_IN_HEAD %}{% bootstrap_javascript %}{% endif %}
 
+  {% block bootstrap5_extra_head %}{% endblock %}
 </head>
 
 <body>
 {% block bootstrap5_before_content %}{% endblock %}
 {% block bootstrap5_content %} CONTENT {% endblock %}
 {% block bootstrap5_after_content %}{% endblock %}
-
 <!-- Bootstrap JavaScript if it is in body -->
-{% if not 'javascript_in_head'|bootstrap_setting %}
-    {% bootstrap_javascript %}
-{% endif %}
+{% if not BOOTSTRAP_JAVASCRIPT_IN_HEAD %}{% bootstrap_javascript %}{% endif %}
 
 {% block bootstrap5_extra_script %}{% endblock %}
-
 </body>
 
 </html>
```

#### html2text {}

```diff
@@ -1,9 +1,11 @@
 {% load django_bootstrap5 %} {% load i18n %} {% get_current_language as
-LANGUAGE_CODE %}
-{% bootstrap_css %} {% if 'javascript_in_head'|bootstrap_setting %} {%
-bootstrap_javascript %} {% endif %} {% block bootstrap5_extra_head %}{%
-endblock %}
+LANGUAGE_CODE %} {% bootstrap_setting "color_mode" as COLOR_MODE %} {%
+bootstrap_setting "javascript_in_head" as BOOTSTRAP_JAVASCRIPT_IN_HEAD %}
+% if COLOR_MODE %} data-bs-theme="{{ COLOR_MODE }}"{% endif %}>
+{% bootstrap_css %} {% if BOOTSTRAP_JAVASCRIPT_IN_HEAD %}{%
+bootstrap_javascript %}{% endif %} {% block bootstrap5_extra_head %}{% endblock
+%}
 {% block bootstrap5_before_content %}{% endblock %} {% block bootstrap5_content
 %} CONTENT {% endblock %} {% block bootstrap5_after_content %}{% endblock %} {%
-if not 'javascript_in_head'|bootstrap_setting %} {% bootstrap_javascript %} {%
-endif %} {% block bootstrap5_extra_script %}{% endblock %}
+if not BOOTSTRAP_JAVASCRIPT_IN_HEAD %}{% bootstrap_javascript %}{% endif %} {%
+block bootstrap5_extra_script %}{% endblock %}
```

### Comparing `django-bootstrap5-24.1/src/django_bootstrap5/templates/django_bootstrap5/pagination.html` & `django_bootstrap5-24.2/src/django_bootstrap5/templates/django_bootstrap5/pagination.html`

 * *Files identical despite different names*

### Comparing `django-bootstrap5-24.1/src/django_bootstrap5/templates/django_bootstrap5/widgets/clearable_file_input.html` & `django_bootstrap5-24.2/src/django_bootstrap5/templates/django_bootstrap5/widgets/clearable_file_input.html`

 * *Files identical despite different names*

### Comparing `django-bootstrap5-24.1/src/django_bootstrap5/templates/django_bootstrap5/widgets/radio_select.html` & `django_bootstrap5-24.2/src/django_bootstrap5/templates/django_bootstrap5/widgets/radio_select.html`

 * *Files identical despite different names*

### Comparing `django-bootstrap5-24.1/src/django_bootstrap5/templates/django_bootstrap5/widgets/radio_select_button_group.html` & `django_bootstrap5-24.2/src/django_bootstrap5/templates/django_bootstrap5/widgets/radio_select_button_group.html`

 * *Files identical despite different names*

### Comparing `django-bootstrap5-24.1/src/django_bootstrap5/templatetags/django_bootstrap5.py` & `django_bootstrap5-24.2/src/django_bootstrap5/templatetags/django_bootstrap5.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,22 @@
 from django.template import Context
 from django.utils.http import urlencode
 from django.utils.safestring import mark_safe
 
 from ..components import render_alert, render_button
 from ..core import css_url, get_bootstrap_setting, javascript_url, theme_url
 from ..css import _css_class_list, merge_css_classes
-from ..forms import render_field, render_form, render_form_errors, render_formset, render_formset_errors, render_label
+from ..forms import (
+    render_field,
+    render_form,
+    render_form_errors,
+    render_formset,
+    render_formset_errors,
+    render_label,
+)
 from ..html import render_link_tag, render_script_tag
 from ..size import get_size_class
 from ..utils import render_template_file, url_replace_param
 
 MESSAGE_ALERT_TYPES = {
     message_constants.DEBUG: "warning",
     message_constants.INFO: "info",
@@ -22,20 +29,20 @@
     message_constants.WARNING: "warning",
     message_constants.ERROR: "danger",
 }
 
 register = template.Library()
 
 
-@register.filter
+@register.simple_tag
 def bootstrap_setting(value):
     """
     Return django-bootstrap5 setting for use in in a template.
 
-    Please consider this filter private, do not use it in your own templates.
+    Please consider this tag private, do not use it in your own templates.
     """
     return get_bootstrap_setting(value)
 
 
 @register.simple_tag
 def bootstrap_server_side_validation_class(widget):
     """
@@ -771,15 +778,22 @@
         pages_shown.append(i)
 
     parts = urlparse(url or "")
     params = parse_qs(parts.query)
     if extra:
         params.update(parse_qs(extra))
     url = urlunparse(
-        [parts.scheme, parts.netloc, parts.path, parts.params, urlencode(params, doseq=True), parts.fragment]
+        [
+            parts.scheme,
+            parts.netloc,
+            parts.path,
+            parts.params,
+            urlencode(params, doseq=True),
+            parts.fragment,
+        ]
     )
 
     pagination_css_classes = ["pagination"]
     if size:
         pagination_size_class = get_size_class(size, prefix="pagination", skip="md")
         if pagination_size_class:
             pagination_css_classes.append(pagination_size_class)
```

### Comparing `django-bootstrap5-24.1/src/django_bootstrap5/utils.py` & `django_bootstrap5-24.2/src/django_bootstrap5/utils.py`

 * *Files identical despite different names*

### Comparing `django-bootstrap5-24.1/src/django_bootstrap5/widgets.py` & `django_bootstrap5-24.2/src/django_bootstrap5/widgets.py`

 * *Files identical despite different names*

### Comparing `django-bootstrap5-24.1/src/django_bootstrap5.egg-info/PKG-INFO` & `django_bootstrap5-24.2/src/django_bootstrap5.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-bootstrap5
-Version: 24.1
+Version: 24.2
 Summary: Bootstrap 5 for Django
 Author-email: Dylan Verheul <dylan@dyve.net>
 License: BSD 3-Clause License
         
         Copyright (c) Zostera B.V. and individual contributors
         All rights reserved.
         
@@ -33,19 +33,18 @@
         OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
         OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 Project-URL: Changelog, https://github.com/zostera/django-bootstrap5/blob/main/CHANGELOG.md
 Project-URL: Documentation, https://django-bootstrap5.readthedocs.io/
 Project-URL: Homepage, https://github.com/zostera/django-bootstrap5
 Project-URL: Issues, https://github.com/zostera/django-bootstrap5/issues
 Project-URL: Source, https://github.com/zostera/django-bootstrap5
+Keywords: django,bootstrap,bootstrap5
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 3.2
-Classifier: Framework :: Django :: 4.1
 Classifier: Framework :: Django :: 4.2
 Classifier: Framework :: Django :: 5.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -55,15 +54,15 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Utilities
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: AUTHORS
-Requires-Dist: Django>=3.2
+Requires-Dist: Django>=4.2
 
 # django-bootstrap5
 
 [![CI](https://github.com/zostera/django-bootstrap5/workflows/CI/badge.svg?branch=main)](https://github.com/zostera/django-bootstrap5/actions?workflow=CI)
 [![Coverage Status](https://coveralls.io/repos/github/zostera/django-bootstrap5/badge.svg?branch=main)](https://coveralls.io/github/zostera/django-bootstrap5?branch=main)
 [![Latest PyPI version](https://img.shields.io/pypi/v/django-bootstrap5.svg)](https://pypi.python.org/pypi/django-bootstrap5)
```

### Comparing `django-bootstrap5-24.1/src/django_bootstrap5.egg-info/SOURCES.txt` & `django_bootstrap5-24.2/src/django_bootstrap5.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,22 @@
-.gitignore
-.readthedocs.yml
+.editorconfig
+.readthedocs.yaml
 AUTHORS
 CHANGELOG.md
 CONTRIBUTING.md
 LICENSE
+MANIFEST.in
 MIGRATE.md
 Makefile
 README.md
 manage.py
 pyproject.toml
 requirements-dev.txt
 requirements-test.txt
 tox.ini
-.github/dependabot.yml
-.github/workflows/dependabot-auto-approve-and-merge.yml
-.github/workflows/test.yml
 docs/changelog.rst
 docs/conf.py
 docs/contributing.rst
 docs/example_template.rst
 docs/forms.rst
 docs/index.rst
 docs/installation.rst
```

### Comparing `django-bootstrap5-24.1/tests/app/settings.py` & `django_bootstrap5-24.2/tests/app/settings.py`

 * *Files identical despite different names*

### Comparing `django-bootstrap5-24.1/tests/base.py` & `django_bootstrap5-24.2/tests/base.py`

 * *Files identical despite different names*

### Comparing `django-bootstrap5-24.1/tests/image.py` & `django_bootstrap5-24.2/tests/image.py`

 * *Files identical despite different names*

### Comparing `django-bootstrap5-24.1/tests/test_bootstrap_alert.py` & `django_bootstrap5-24.2/tests/test_bootstrap_alert.py`

 * *Files identical despite different names*

### Comparing `django-bootstrap5-24.1/tests/test_bootstrap_button.py` & `django_bootstrap5-24.2/tests/test_bootstrap_button.py`

 * *Files identical despite different names*

### Comparing `django-bootstrap5-24.1/tests/test_bootstrap_css_and_js_tags.py` & `django_bootstrap5-24.2/tests/test_bootstrap_css_and_js_tags.py`

 * *Files 5% similar despite different names*

```diff
@@ -37,12 +37,19 @@
     def test_bootstrap_css_tag_with_theme(self):
         with self.settings(BOOTSTRAP5={"theme_url": "//example.com/theme.css"}):
             self.assertHTMLEqual(
                 self.render("{% bootstrap_css %}"),
                 self.expected_bootstrap_css + '<link rel="stylesheet" href="//example.com/theme.css">',
             )
 
-    def test_bootstrap_setting_filter(self):
-        self.assertEqual(self.render('{{ "required_css_class"|bootstrap_setting }}'), "django_bootstrap5-req")
+    def test_bootstrap_setting_tag(self):
         self.assertEqual(
-            self.render('{% if "javascript_in_head"|bootstrap_setting %}head{% else %}body{% endif %}'), "head"
+            self.render('{% bootstrap_setting "required_css_class" %}'),
+            "django_bootstrap5-req",
+        )
+        self.assertEqual(
+            self.render(
+                '{% bootstrap_setting "javascript_in_head" as BOOTSTRAP_JAVASCRIPT_IN_HEAD %}'
+                + "{% if BOOTSTRAP_JAVASCRIPT_IN_HEAD %}head{% else %}body{% endif %}"
+            ),
+            "head",
         )
```

### Comparing `django-bootstrap5-24.1/tests/test_bootstrap_field.py` & `django_bootstrap5-24.2/tests/test_bootstrap_field.py`

 * *Files identical despite different names*

### Comparing `django-bootstrap5-24.1/tests/test_bootstrap_field_datetime.py` & `django_bootstrap5-24.2/tests/test_bootstrap_field_datetime.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,81 +1,81 @@
 from django import forms
 from django.contrib.admin.widgets import AdminSplitDateTime
 
-from tests.base import DJANGO_VERSION, BootstrapTestCase
+from tests.base import BootstrapTestCase
 
 
 class DateTimeTestForm(forms.Form):
     test = forms.SplitDateTimeField(widget=AdminSplitDateTime())
 
 
 class DateTimeTestCase(BootstrapTestCase):
-    def fix_django41(self, html):
-        """Return expected HTML fixed for Django 4.1 if necessary."""
-        if DJANGO_VERSION >= "4.1":
-            html = html.replace(' for="id_test_0"', "")
-        return html
-
     def test_input_type_admin_split_date_time(self):
         """Test field with AdminSplitDateTime widget."""
         expected_html = (
             '<div class="django_bootstrap5-req mb-3">'
-            '<label class="form-label" for="id_test_0">Test</label>'
+            '<label class="form-label">Test</label>'
             '<p class="datetime">'
             "Date: "
             '<input type="text" name="test_0" class="form-control vDateField" size="10"'
             ' placeholder="Test" required id="id_test_0">'
             "<br>"
             "Time: "
             '<input type="text" name="test_1" class="form-control vTimeField" size="8"'
             ' placeholder="Test" required id="id_test_1">'
             "</p>"
             "</div>"
         )
         self.assertHTMLEqual(
             self.render("{% bootstrap_field form.test %}", context={"form": DateTimeTestForm()}),
-            self.fix_django41(expected_html),
+            expected_html,
         )
 
     def test_input_type_admin_split_date_time_horizontal(self):
         """Test field with AdminSplitDateTime widget with layout horizontal."""
         expected_html = (
             '<div class="django_bootstrap5-req row mb-3">'
-            '<label class="col-form-label col-sm-2" for="id_test_0">Test</label>'
+            '<label class="col-form-label col-sm-2">Test</label>'
             '<div class="col-sm-10">'
             '<p class="datetime">'
             "Date: "
             '<input type="text" name="test_0" class="form-control vDateField" size="10"'
             ' placeholder="Test" required id="id_test_0">'
             "<br>"
             "Time: "
             '<input type="text" name="test_1" class="form-control vTimeField" size="8"'
             ' placeholder="Test" required id="id_test_1">'
             "</p>"
             "</div>"
             "</div>"
         )
         self.assertHTMLEqual(
-            self.render('{% bootstrap_field form.test layout="horizontal" %}', context={"form": DateTimeTestForm()}),
-            self.fix_django41(expected_html),
+            self.render(
+                '{% bootstrap_field form.test layout="horizontal" %}',
+                context={"form": DateTimeTestForm()},
+            ),
+            expected_html,
         )
 
     def test_input_type_admin_split_date_time_floating(self):
         """Test field with AdminSplitDateTime widget with layout floating."""
         expected_html = (
             '<div class="django_bootstrap5-req mb-3">'
-            '<label class="form-label" for="id_test_0">Test</label>'
+            '<label class="form-label">Test</label>'
             '<p class="datetime">'
             "Date: "
             '<input type="text" name="test_0" class="form-control vDateField" size="10"'
             ' placeholder="Test" required id="id_test_0">'
             "<br>"
             "Time: "
             '<input type="text" name="test_1" class="form-control vTimeField" size="8"'
             ' placeholder="Test" required id="id_test_1">'
             "</p>"
             "</div>"
         )
         self.assertHTMLEqual(
-            self.render('{% bootstrap_field form.test layout="floating" %}', context={"form": DateTimeTestForm()}),
-            self.fix_django41(expected_html),
+            self.render(
+                '{% bootstrap_field form.test layout="floating" %}',
+                context={"form": DateTimeTestForm()},
+            ),
+            expected_html,
         )
```

### Comparing `django-bootstrap5-24.1/tests/test_bootstrap_field_input_checkbox.py` & `django_bootstrap5-24.2/tests/test_bootstrap_field_input_checkbox.py`

 * *Files identical despite different names*

### Comparing `django-bootstrap5-24.1/tests/test_bootstrap_field_input_color.py` & `django_bootstrap5-24.2/tests/test_bootstrap_field_input_color.py`

 * *Files identical despite different names*

### Comparing `django-bootstrap5-24.1/tests/test_bootstrap_field_input_file.py` & `django_bootstrap5-24.2/tests/test_bootstrap_field_input_file.py`

 * *Files identical despite different names*

### Comparing `django-bootstrap5-24.1/tests/test_bootstrap_field_input_range.py` & `django_bootstrap5-24.2/tests/test_bootstrap_field_input_range.py`

 * *Files identical despite different names*

### Comparing `django-bootstrap5-24.1/tests/test_bootstrap_field_input_text.py` & `django_bootstrap5-24.2/tests/test_bootstrap_field_input_text.py`

 * *Files identical despite different names*

### Comparing `django-bootstrap5-24.1/tests/test_bootstrap_field_parameters.py` & `django_bootstrap5-24.2/tests/test_bootstrap_field_parameters.py`

 * *Files identical despite different names*

### Comparing `django-bootstrap5-24.1/tests/test_bootstrap_field_radio_select.py` & `django_bootstrap5-24.2/tests/test_bootstrap_field_radio_select.py`

 * *Files identical despite different names*

### Comparing `django-bootstrap5-24.1/tests/test_bootstrap_field_radio_select_button_group.py` & `django_bootstrap5-24.2/tests/test_bootstrap_field_radio_select_button_group.py`

 * *Files identical despite different names*

### Comparing `django-bootstrap5-24.1/tests/test_bootstrap_field_select.py` & `django_bootstrap5-24.2/tests/test_bootstrap_field_select.py`

 * *Files identical despite different names*

### Comparing `django-bootstrap5-24.1/tests/test_bootstrap_field_textarea.py` & `django_bootstrap5-24.2/tests/test_bootstrap_field_textarea.py`

 * *Files identical despite different names*

### Comparing `django-bootstrap5-24.1/tests/test_bootstrap_form.py` & `django_bootstrap5-24.2/tests/test_bootstrap_form.py`

 * *Files identical despite different names*

### Comparing `django-bootstrap5-24.1/tests/test_bootstrap_formset.py` & `django_bootstrap5-24.2/tests/test_bootstrap_formset.py`

 * *Files identical despite different names*

### Comparing `django-bootstrap5-24.1/tests/test_bootstrap_label.py` & `django_bootstrap5-24.2/tests/test_bootstrap_label.py`

 * *Files identical despite different names*

### Comparing `django-bootstrap5-24.1/tests/test_bootstrap_messages.py` & `django_bootstrap5-24.2/tests/test_bootstrap_messages.py`

 * *Files identical despite different names*

### Comparing `django-bootstrap5-24.1/tests/test_bootstrap_pagination.py` & `django_bootstrap5-24.2/tests/test_bootstrap_pagination.py`

 * *Files identical despite different names*

### Comparing `django-bootstrap5-24.1/tests/test_components.py` & `django_bootstrap5-24.2/tests/test_components.py`

 * *Files identical despite different names*

### Comparing `django-bootstrap5-24.1/tests/test_css.py` & `django_bootstrap5-24.2/tests/test_css.py`

 * *Files identical despite different names*

### Comparing `django-bootstrap5-24.1/tests/test_settings.py` & `django_bootstrap5-24.2/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `django-bootstrap5-24.1/tests/test_size.py` & `django_bootstrap5-24.2/tests/test_size.py`

 * *Files identical despite different names*

### Comparing `django-bootstrap5-24.1/tests/test_templates.py` & `django_bootstrap5-24.2/tests/test_templates.py`

 * *Files 21% similar despite different names*

```diff
@@ -4,14 +4,27 @@
 class TemplateTestCase(BootstrapTestCase):
     def test_empty_template(self):
         self.assertEqual(self.render("").strip(), "")
 
     def test_text_template(self):
         self.assertEqual(self.render("some text").strip(), "some text")
 
+    def test_bootstrap5_html_template_color_mode(self):
+        html = self.render(
+            '{% extends "django_bootstrap5/bootstrap5.html" %}',
+            load_bootstrap=False,
+        )
+        self.assertNotIn("data-bs-theme", html)
+        with self.settings(BOOTSTRAP5={"color_mode": "dark"}):
+            html = self.render(
+                '{% extends "django_bootstrap5/bootstrap5.html" %}',
+                load_bootstrap=False,
+            )
+            self.assertIn('data-bs-theme="dark"', html)
+
     def test_bootstrap5_html_template_title(self):
         html = self.render(
             '{% extends "django_bootstrap5/bootstrap5.html" %}{% block bootstrap5_title %}x-title-x{% endblock %}',
             load_bootstrap=False,
         )
         self.assertIn("x-title-x", html)
```

### Comparing `django-bootstrap5-24.1/tests/test_text.py` & `django_bootstrap5-24.2/tests/test_text.py`

 * *Files identical despite different names*

### Comparing `django-bootstrap5-24.1/tests/test_urls.py` & `django_bootstrap5-24.2/tests/test_urls.py`

 * *Files identical despite different names*

### Comparing `django-bootstrap5-24.1/tox.ini` & `django_bootstrap5-24.2/tox.ini`

 * *Files 10% similar despite different names*

```diff
@@ -1,37 +1,33 @@
 [tox]
 args_are_paths = false
 envlist =
-    py38-{3.2,4.1,4.2},
-    py39-{3.2,4.1,4.2},
-    py310-{3.2,4.1,4.2,5.0,main},
-    py311-{4.1,4.2,5.0,main},
+    py38-{4.2},
+    py39-{4.2},
+    py310-{4.2,5.0,main},
+    py311-{4.2,5.0,main},
     py312-{4.2,5.0,main},
     docs,
     lint,
 
 [testenv]
 basepython =
-    py37: python3.7
     py38: python3.8
     py39: python3.9
     py310: python3.10
     py311: python3.11
     py312: python3.12
 usedevelop = true
 pip_pre = true
 setenv =
     PYTHONPATH={toxinidir}
     PYTHONWARNINGS=all
 commands =
     python manage.py test {posargs}
 deps =
-    3.2: Django==3.2.*
-    4.0: Django==4.0.*
-    4.1: Django==4.1.*
     4.2: Django==4.2.*
     5.0: Django==5.0.*
     main: https://github.com/django/django/archive/main.tar.gz
     -r{toxinidir}/requirements-test.txt
 
 [testenv:ruff]
 basepython = python3.11
```

