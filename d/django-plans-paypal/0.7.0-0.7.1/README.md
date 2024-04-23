# Comparing `tmp/django-plans-paypal-0.7.0.tar.gz` & `tmp/django-plans-paypal-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-plans-paypal-0.7.0.tar", last modified: Fri Apr 12 13:13:10 2024, max compression
+gzip compressed data, was "django-plans-paypal-0.7.1.tar", last modified: Tue Apr 23 10:10:26 2024, max compression
```

## Comparing `django-plans-paypal-0.7.0.tar` & `django-plans-paypal-0.7.1.tar`

### file list

```diff
@@ -1,70 +1,70 @@
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-12 13:13:10.478720 django-plans-paypal-0.7.0/
--rw-rw-r--   0 petr      (1000) petr      (1000)      229 2024-04-12 13:13:10.000000 django-plans-paypal-0.7.0/.coveragerc
--rw-rw-r--   0 petr      (1000) petr      (1000)      331 2024-04-12 13:13:10.000000 django-plans-paypal-0.7.0/.editorconfig
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-12 13:13:10.470719 django-plans-paypal-0.7.0/.github/
--rw-rw-r--   0 petr      (1000) petr      (1000)      348 2024-04-12 13:13:10.000000 django-plans-paypal-0.7.0/.github/ISSUE_TEMPLATE.md
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-12 13:13:10.470719 django-plans-paypal-0.7.0/.github/workflows/
--rw-rw-r--   0 petr      (1000) petr      (1000)     3177 2024-04-12 13:13:10.000000 django-plans-paypal-0.7.0/.github/workflows/main.yml
--rw-rw-r--   0 petr      (1000) petr      (1000)      432 2024-04-12 13:13:10.000000 django-plans-paypal-0.7.0/.gitignore
--rw-rw-r--   0 petr      (1000) petr      (1000)      469 2024-04-12 13:13:10.000000 django-plans-paypal-0.7.0/.travis.yml
--rw-rw-r--   0 petr      (1000) petr      (1000)      161 2024-04-12 13:13:10.000000 django-plans-paypal-0.7.0/AUTHORS.rst
--rw-rw-r--   0 petr      (1000) petr      (1000)     3306 2024-04-12 13:13:10.000000 django-plans-paypal-0.7.0/CONTRIBUTING.rst
--rw-rw-r--   0 petr      (1000) petr      (1000)     2742 2024-04-12 13:13:10.000000 django-plans-paypal-0.7.0/HISTORY.rst
--rw-rw-r--   0 petr      (1000) petr      (1000)     1075 2024-04-12 13:13:10.000000 django-plans-paypal-0.7.0/LICENSE
--rw-rw-r--   0 petr      (1000) petr      (1000)      179 2024-04-12 13:13:10.000000 django-plans-paypal-0.7.0/MANIFEST.in
--rw-rw-r--   0 petr      (1000) petr      (1000)     1549 2024-04-12 13:13:10.000000 django-plans-paypal-0.7.0/Makefile
--rw-rw-r--   0 petr      (1000) petr      (1000)     6975 2024-04-12 13:13:10.478720 django-plans-paypal-0.7.0/PKG-INFO
--rw-rw-r--   0 petr      (1000) petr      (1000)     3358 2024-04-12 13:13:10.000000 django-plans-paypal-0.7.0/README.rst
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-12 13:13:10.474719 django-plans-paypal-0.7.0/django_plans_paypal.egg-info/
--rw-rw-r--   0 petr      (1000) petr      (1000)     6975 2024-04-12 13:13:10.000000 django-plans-paypal-0.7.0/django_plans_paypal.egg-info/PKG-INFO
--rw-rw-r--   0 petr      (1000) petr      (1000)     1314 2024-04-12 13:13:10.000000 django-plans-paypal-0.7.0/django_plans_paypal.egg-info/SOURCES.txt
--rw-rw-r--   0 petr      (1000) petr      (1000)        1 2024-04-12 13:13:10.000000 django-plans-paypal-0.7.0/django_plans_paypal.egg-info/dependency_links.txt
--rw-rw-r--   0 petr      (1000) petr      (1000)        1 2024-04-12 13:13:10.000000 django-plans-paypal-0.7.0/django_plans_paypal.egg-info/not-zip-safe
--rw-rw-r--   0 petr      (1000) petr      (1000)       87 2024-04-12 13:13:10.000000 django-plans-paypal-0.7.0/django_plans_paypal.egg-info/requires.txt
--rw-rw-r--   0 petr      (1000) petr      (1000)       19 2024-04-12 13:13:10.000000 django-plans-paypal-0.7.0/django_plans_paypal.egg-info/top_level.txt
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-12 13:13:10.474719 django-plans-paypal-0.7.0/docs/
--rw-rw-r--   0 petr      (1000) petr      (1000)     6778 2024-04-12 13:13:10.000000 django-plans-paypal-0.7.0/docs/Makefile
--rw-rw-r--   0 petr      (1000) petr      (1000)       28 2024-04-12 13:13:10.000000 django-plans-paypal-0.7.0/docs/authors.rst
--rw-rw-r--   0 petr      (1000) petr      (1000)     8421 2024-04-12 13:13:10.000000 django-plans-paypal-0.7.0/docs/conf.py
--rw-rw-r--   0 petr      (1000) petr      (1000)       33 2024-04-12 13:13:10.000000 django-plans-paypal-0.7.0/docs/contributing.rst
--rw-rw-r--   0 petr      (1000) petr      (1000)       28 2024-04-12 13:13:10.000000 django-plans-paypal-0.7.0/docs/history.rst
--rw-rw-r--   0 petr      (1000) petr      (1000)      450 2024-04-12 13:13:10.000000 django-plans-paypal-0.7.0/docs/index.rst
--rw-rw-r--   0 petr      (1000) petr      (1000)      227 2024-04-12 13:13:10.000000 django-plans-paypal-0.7.0/docs/installation.rst
--rw-rw-r--   0 petr      (1000) petr      (1000)     6467 2024-04-12 13:13:10.000000 django-plans-paypal-0.7.0/docs/make.bat
--rw-rw-r--   0 petr      (1000) petr      (1000)       27 2024-04-12 13:13:10.000000 django-plans-paypal-0.7.0/docs/readme.rst
--rw-rw-r--   0 petr      (1000) petr      (1000)      438 2024-04-12 13:13:10.000000 django-plans-paypal-0.7.0/docs/usage.rst
--rw-rw-r--   0 petr      (1000) petr      (1000)      330 2024-04-12 13:13:10.000000 django-plans-paypal-0.7.0/manage.py
--rw-rw-r--   0 petr      (1000) petr      (1000)      195 2024-04-12 13:13:10.000000 django-plans-paypal-0.7.0/mypy.ini
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-12 13:13:10.474719 django-plans-paypal-0.7.0/plans_paypal/
--rw-rw-r--   0 petr      (1000) petr      (1000)       22 2024-04-12 13:13:10.000000 django-plans-paypal-0.7.0/plans_paypal/__init__.py
--rw-rw-r--   0 petr      (1000) petr      (1000)      721 2024-04-12 13:13:10.000000 django-plans-paypal-0.7.0/plans_paypal/admin.py
--rw-rw-r--   0 petr      (1000) petr      (1000)      162 2024-04-12 13:13:10.000000 django-plans-paypal-0.7.0/plans_paypal/apps.py
--rw-rw-r--   0 petr      (1000) petr      (1000)     4532 2024-04-12 13:13:10.000000 django-plans-paypal-0.7.0/plans_paypal/hooks.py
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-12 13:13:10.474719 django-plans-paypal-0.7.0/plans_paypal/migrations/
--rw-rw-r--   0 petr      (1000) petr      (1000)     1392 2024-04-12 13:13:10.000000 django-plans-paypal-0.7.0/plans_paypal/migrations/0001_initial.py
--rw-rw-r--   0 petr      (1000) petr      (1000)     2002 2024-04-12 13:13:10.000000 django-plans-paypal-0.7.0/plans_paypal/migrations/0002_auto_20211130_1117.py
--rw-rw-r--   0 petr      (1000) petr      (1000)     2146 2024-04-12 13:13:10.000000 django-plans-paypal-0.7.0/plans_paypal/migrations/0003_recurringuserplan_renewal_triggered_by_task_to_other.py
--rw-rw-r--   0 petr      (1000) petr      (1000)        0 2024-04-12 13:13:10.000000 django-plans-paypal-0.7.0/plans_paypal/migrations/__init__.py
--rw-rw-r--   0 petr      (1000) petr      (1000)      618 2024-04-12 13:13:10.000000 django-plans-paypal-0.7.0/plans_paypal/models.py
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-12 13:13:10.466719 django-plans-paypal-0.7.0/plans_paypal/templates/
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-12 13:13:10.474719 django-plans-paypal-0.7.0/plans_paypal/templates/paypal_payments/
--rw-rw-r--   0 petr      (1000) petr      (1000)      157 2024-04-12 13:13:10.000000 django-plans-paypal-0.7.0/plans_paypal/templates/paypal_payments/payment.html
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-12 13:13:10.474719 django-plans-paypal-0.7.0/plans_paypal/tests/
--rw-rw-r--   0 petr      (1000) petr      (1000)        0 2024-04-12 13:13:10.000000 django-plans-paypal-0.7.0/plans_paypal/tests/__init__.py
--rw-rw-r--   0 petr      (1000) petr      (1000)    10620 2024-04-12 13:13:10.000000 django-plans-paypal-0.7.0/plans_paypal/tests/test_hooks.py
--rw-rw-r--   0 petr      (1000) petr      (1000)     2141 2024-04-12 13:13:10.000000 django-plans-paypal-0.7.0/plans_paypal/tests/test_views.py
--rw-rw-r--   0 petr      (1000) petr      (1000)      594 2024-04-12 13:13:10.000000 django-plans-paypal-0.7.0/plans_paypal/urls.py
--rw-rw-r--   0 petr      (1000) petr      (1000)     4289 2024-04-12 13:13:10.000000 django-plans-paypal-0.7.0/plans_paypal/views.py
--rw-rw-r--   0 petr      (1000) petr      (1000)      123 2024-04-12 13:13:10.000000 django-plans-paypal-0.7.0/requirements.txt
--rw-rw-r--   0 petr      (1000) petr      (1000)       34 2024-04-12 13:13:10.000000 django-plans-paypal-0.7.0/requirements_dev.txt
--rw-rw-r--   0 petr      (1000) petr      (1000)      150 2024-04-12 13:13:10.000000 django-plans-paypal-0.7.0/requirements_test.txt
--rw-rw-r--   0 petr      (1000) petr      (1000)      575 2024-04-12 13:13:10.000000 django-plans-paypal-0.7.0/runtests.py
--rw-rw-r--   0 petr      (1000) petr      (1000)      419 2024-04-12 13:13:10.478720 django-plans-paypal-0.7.0/setup.cfg
--rwxrwxr-x   0 petr      (1000) petr      (1000)     2827 2024-04-12 13:13:10.000000 django-plans-paypal-0.7.0/setup.py
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-12 13:13:10.478720 django-plans-paypal-0.7.0/tests/
--rw-rw-r--   0 petr      (1000) petr      (1000)        0 2024-04-12 13:13:10.000000 django-plans-paypal-0.7.0/tests/__init__.py
--rw-rw-r--   0 petr      (1000) petr      (1000)     1659 2024-04-12 13:13:10.000000 django-plans-paypal-0.7.0/tests/settings.py
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-12 13:13:10.478720 django-plans-paypal-0.7.0/tests/templates/
--rw-rw-r--   0 petr      (1000) petr      (1000)       33 2024-04-12 13:13:10.000000 django-plans-paypal-0.7.0/tests/templates/base.html
--rw-rw-r--   0 petr      (1000) petr      (1000)      226 2024-04-12 13:13:10.000000 django-plans-paypal-0.7.0/tests/urls.py
--rw-rw-r--   0 petr      (1000) petr      (1000)      388 2024-04-12 13:13:10.000000 django-plans-paypal-0.7.0/tox.ini
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-23 10:10:26.254662 django-plans-paypal-0.7.1/
+-rw-rw-r--   0 petr      (1000) petr      (1000)      229 2024-04-23 10:10:25.000000 django-plans-paypal-0.7.1/.coveragerc
+-rw-rw-r--   0 petr      (1000) petr      (1000)      331 2024-04-23 10:10:25.000000 django-plans-paypal-0.7.1/.editorconfig
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-23 10:10:26.246662 django-plans-paypal-0.7.1/.github/
+-rw-rw-r--   0 petr      (1000) petr      (1000)      348 2024-04-23 10:10:25.000000 django-plans-paypal-0.7.1/.github/ISSUE_TEMPLATE.md
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-23 10:10:26.246662 django-plans-paypal-0.7.1/.github/workflows/
+-rw-rw-r--   0 petr      (1000) petr      (1000)     3177 2024-04-23 10:10:25.000000 django-plans-paypal-0.7.1/.github/workflows/main.yml
+-rw-rw-r--   0 petr      (1000) petr      (1000)      432 2024-04-23 10:10:25.000000 django-plans-paypal-0.7.1/.gitignore
+-rw-rw-r--   0 petr      (1000) petr      (1000)      469 2024-04-23 10:10:25.000000 django-plans-paypal-0.7.1/.travis.yml
+-rw-rw-r--   0 petr      (1000) petr      (1000)      161 2024-04-23 10:10:25.000000 django-plans-paypal-0.7.1/AUTHORS.rst
+-rw-rw-r--   0 petr      (1000) petr      (1000)     3306 2024-04-23 10:10:25.000000 django-plans-paypal-0.7.1/CONTRIBUTING.rst
+-rw-rw-r--   0 petr      (1000) petr      (1000)     2843 2024-04-23 10:10:25.000000 django-plans-paypal-0.7.1/HISTORY.rst
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1075 2024-04-23 10:10:25.000000 django-plans-paypal-0.7.1/LICENSE
+-rw-rw-r--   0 petr      (1000) petr      (1000)      179 2024-04-23 10:10:25.000000 django-plans-paypal-0.7.1/MANIFEST.in
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1549 2024-04-23 10:10:25.000000 django-plans-paypal-0.7.1/Makefile
+-rw-r--r--   0 petr      (1000) petr      (1000)     7238 2024-04-23 10:10:26.254662 django-plans-paypal-0.7.1/PKG-INFO
+-rw-rw-r--   0 petr      (1000) petr      (1000)     3358 2024-04-23 10:10:25.000000 django-plans-paypal-0.7.1/README.rst
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-23 10:10:26.254662 django-plans-paypal-0.7.1/django_plans_paypal.egg-info/
+-rw-r--r--   0 petr      (1000) petr      (1000)     7238 2024-04-23 10:10:25.000000 django-plans-paypal-0.7.1/django_plans_paypal.egg-info/PKG-INFO
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1314 2024-04-23 10:10:26.000000 django-plans-paypal-0.7.1/django_plans_paypal.egg-info/SOURCES.txt
+-rw-rw-r--   0 petr      (1000) petr      (1000)        1 2024-04-23 10:10:25.000000 django-plans-paypal-0.7.1/django_plans_paypal.egg-info/dependency_links.txt
+-rw-rw-r--   0 petr      (1000) petr      (1000)        1 2024-04-23 10:10:25.000000 django-plans-paypal-0.7.1/django_plans_paypal.egg-info/not-zip-safe
+-rw-rw-r--   0 petr      (1000) petr      (1000)       87 2024-04-23 10:10:25.000000 django-plans-paypal-0.7.1/django_plans_paypal.egg-info/requires.txt
+-rw-rw-r--   0 petr      (1000) petr      (1000)       19 2024-04-23 10:10:25.000000 django-plans-paypal-0.7.1/django_plans_paypal.egg-info/top_level.txt
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-23 10:10:26.250662 django-plans-paypal-0.7.1/docs/
+-rw-rw-r--   0 petr      (1000) petr      (1000)     6778 2024-04-23 10:10:25.000000 django-plans-paypal-0.7.1/docs/Makefile
+-rw-rw-r--   0 petr      (1000) petr      (1000)       28 2024-04-23 10:10:25.000000 django-plans-paypal-0.7.1/docs/authors.rst
+-rw-rw-r--   0 petr      (1000) petr      (1000)     8421 2024-04-23 10:10:25.000000 django-plans-paypal-0.7.1/docs/conf.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)       33 2024-04-23 10:10:25.000000 django-plans-paypal-0.7.1/docs/contributing.rst
+-rw-rw-r--   0 petr      (1000) petr      (1000)       28 2024-04-23 10:10:25.000000 django-plans-paypal-0.7.1/docs/history.rst
+-rw-rw-r--   0 petr      (1000) petr      (1000)      450 2024-04-23 10:10:25.000000 django-plans-paypal-0.7.1/docs/index.rst
+-rw-rw-r--   0 petr      (1000) petr      (1000)      227 2024-04-23 10:10:25.000000 django-plans-paypal-0.7.1/docs/installation.rst
+-rw-rw-r--   0 petr      (1000) petr      (1000)     6467 2024-04-23 10:10:25.000000 django-plans-paypal-0.7.1/docs/make.bat
+-rw-rw-r--   0 petr      (1000) petr      (1000)       27 2024-04-23 10:10:25.000000 django-plans-paypal-0.7.1/docs/readme.rst
+-rw-rw-r--   0 petr      (1000) petr      (1000)      438 2024-04-23 10:10:25.000000 django-plans-paypal-0.7.1/docs/usage.rst
+-rw-rw-r--   0 petr      (1000) petr      (1000)      330 2024-04-23 10:10:25.000000 django-plans-paypal-0.7.1/manage.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      195 2024-04-23 10:10:25.000000 django-plans-paypal-0.7.1/mypy.ini
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-23 10:10:26.250662 django-plans-paypal-0.7.1/plans_paypal/
+-rw-rw-r--   0 petr      (1000) petr      (1000)       22 2024-04-23 10:10:25.000000 django-plans-paypal-0.7.1/plans_paypal/__init__.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      721 2024-04-23 10:10:25.000000 django-plans-paypal-0.7.1/plans_paypal/admin.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      162 2024-04-23 10:10:25.000000 django-plans-paypal-0.7.1/plans_paypal/apps.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)     4532 2024-04-23 10:10:25.000000 django-plans-paypal-0.7.1/plans_paypal/hooks.py
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-23 10:10:26.250662 django-plans-paypal-0.7.1/plans_paypal/migrations/
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1392 2024-04-23 10:10:25.000000 django-plans-paypal-0.7.1/plans_paypal/migrations/0001_initial.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)     2002 2024-04-23 10:10:25.000000 django-plans-paypal-0.7.1/plans_paypal/migrations/0002_auto_20211130_1117.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)     2146 2024-04-23 10:10:25.000000 django-plans-paypal-0.7.1/plans_paypal/migrations/0003_recurringuserplan_renewal_triggered_by_task_to_other.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)        0 2024-04-23 10:10:25.000000 django-plans-paypal-0.7.1/plans_paypal/migrations/__init__.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      618 2024-04-23 10:10:25.000000 django-plans-paypal-0.7.1/plans_paypal/models.py
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-23 10:10:26.242662 django-plans-paypal-0.7.1/plans_paypal/templates/
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-23 10:10:26.250662 django-plans-paypal-0.7.1/plans_paypal/templates/paypal_payments/
+-rw-rw-r--   0 petr      (1000) petr      (1000)      157 2024-04-23 10:10:25.000000 django-plans-paypal-0.7.1/plans_paypal/templates/paypal_payments/payment.html
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-23 10:10:26.250662 django-plans-paypal-0.7.1/plans_paypal/tests/
+-rw-rw-r--   0 petr      (1000) petr      (1000)        0 2024-04-23 10:10:25.000000 django-plans-paypal-0.7.1/plans_paypal/tests/__init__.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)    10620 2024-04-23 10:10:25.000000 django-plans-paypal-0.7.1/plans_paypal/tests/test_hooks.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)     2561 2024-04-23 10:10:25.000000 django-plans-paypal-0.7.1/plans_paypal/tests/test_views.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      594 2024-04-23 10:10:25.000000 django-plans-paypal-0.7.1/plans_paypal/urls.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)     4483 2024-04-23 10:10:25.000000 django-plans-paypal-0.7.1/plans_paypal/views.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      123 2024-04-23 10:10:25.000000 django-plans-paypal-0.7.1/requirements.txt
+-rw-rw-r--   0 petr      (1000) petr      (1000)       34 2024-04-23 10:10:25.000000 django-plans-paypal-0.7.1/requirements_dev.txt
+-rw-rw-r--   0 petr      (1000) petr      (1000)      150 2024-04-23 10:10:25.000000 django-plans-paypal-0.7.1/requirements_test.txt
+-rw-rw-r--   0 petr      (1000) petr      (1000)      575 2024-04-23 10:10:25.000000 django-plans-paypal-0.7.1/runtests.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      419 2024-04-23 10:10:26.254662 django-plans-paypal-0.7.1/setup.cfg
+-rwxrwxr-x   0 petr      (1000) petr      (1000)     2827 2024-04-23 10:10:25.000000 django-plans-paypal-0.7.1/setup.py
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-23 10:10:26.250662 django-plans-paypal-0.7.1/tests/
+-rw-rw-r--   0 petr      (1000) petr      (1000)        0 2024-04-23 10:10:25.000000 django-plans-paypal-0.7.1/tests/__init__.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1659 2024-04-23 10:10:25.000000 django-plans-paypal-0.7.1/tests/settings.py
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-23 10:10:26.250662 django-plans-paypal-0.7.1/tests/templates/
+-rw-rw-r--   0 petr      (1000) petr      (1000)       33 2024-04-23 10:10:25.000000 django-plans-paypal-0.7.1/tests/templates/base.html
+-rw-rw-r--   0 petr      (1000) petr      (1000)      226 2024-04-23 10:10:25.000000 django-plans-paypal-0.7.1/tests/urls.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      388 2024-04-23 10:10:25.000000 django-plans-paypal-0.7.1/tox.ini
```

### Comparing `django-plans-paypal-0.7.0/.github/workflows/main.yml` & `django-plans-paypal-0.7.1/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `django-plans-paypal-0.7.0/CONTRIBUTING.rst` & `django-plans-paypal-0.7.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `django-plans-paypal-0.7.0/HISTORY.rst` & `django-plans-paypal-0.7.1/HISTORY.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,16 @@
 .. :changelog:
 
 History
 -------
 
+0.7.1 (2024-04-23)
+++++++++++++++++++
+* fail if PaymentFailureView is requested on completed orders
+
 0.7.0 (2024-04-12)
 ++++++++++++++++++
 * migrate code to RecurringUserPlan.renewal_triggered_by
 * migrate data of RecurringUserPlans with payment_provider="paypal-recurring" and renewal_triggered_by=TASK to renewal_triggered_by=OTHER
 
 0.6.0 (2023-03-22)
 +++++++++++++++++++
```

### Comparing `django-plans-paypal-0.7.0/LICENSE` & `django-plans-paypal-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django-plans-paypal-0.7.0/Makefile` & `django-plans-paypal-0.7.1/Makefile`

 * *Files identical despite different names*

### Comparing `django-plans-paypal-0.7.0/PKG-INFO` & `django-plans-paypal-0.7.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-plans-paypal
-Version: 0.7.0
+Version: 0.7.1
 Summary: Integration between django-plans and django-paypal.
 Home-page: https://github.com/PetrDlouhy/django-plans-paypal
 Author: Petr Dlouhý
 Author-email: petr.dlouhy@email.cz
 License: MIT
 Keywords: django-plans-paypal
 Classifier: Development Status :: 3 - Alpha
@@ -17,14 +17,19 @@
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 License-File: LICENSE
 License-File: AUTHORS.rst
+Requires-Dist: django-author>=1.0.3
+Requires-Dist: django-extensions
+Requires-Dist: django-plans
+Requires-Dist: django-paypal
+Requires-Dist: django-related-admin
 
 =============================
 Django plans paypal
 =============================
 
 .. image:: https://badge.fury.io/py/django-plans-paypal.svg
     :target: https://badge.fury.io/py/django-plans-paypal
@@ -147,14 +152,18 @@
 
 
 
 
 History
 -------
 
+0.7.1 (2024-04-23)
+++++++++++++++++++
+* fail if PaymentFailureView is requested on completed orders
+
 0.7.0 (2024-04-12)
 ++++++++++++++++++
 * migrate code to RecurringUserPlan.renewal_triggered_by
 * migrate data of RecurringUserPlans with payment_provider="paypal-recurring" and renewal_triggered_by=TASK to renewal_triggered_by=OTHER
 
 0.6.0 (2023-03-22)
 +++++++++++++++++++
```

### Comparing `django-plans-paypal-0.7.0/README.rst` & `django-plans-paypal-0.7.1/README.rst`

 * *Files identical despite different names*

### Comparing `django-plans-paypal-0.7.0/django_plans_paypal.egg-info/PKG-INFO` & `django-plans-paypal-0.7.1/django_plans_paypal.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-plans-paypal
-Version: 0.7.0
+Version: 0.7.1
 Summary: Integration between django-plans and django-paypal.
 Home-page: https://github.com/PetrDlouhy/django-plans-paypal
 Author: Petr Dlouhý
 Author-email: petr.dlouhy@email.cz
 License: MIT
 Keywords: django-plans-paypal
 Classifier: Development Status :: 3 - Alpha
@@ -17,14 +17,19 @@
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 License-File: LICENSE
 License-File: AUTHORS.rst
+Requires-Dist: django-author>=1.0.3
+Requires-Dist: django-extensions
+Requires-Dist: django-plans
+Requires-Dist: django-paypal
+Requires-Dist: django-related-admin
 
 =============================
 Django plans paypal
 =============================
 
 .. image:: https://badge.fury.io/py/django-plans-paypal.svg
     :target: https://badge.fury.io/py/django-plans-paypal
@@ -147,14 +152,18 @@
 
 
 
 
 History
 -------
 
+0.7.1 (2024-04-23)
+++++++++++++++++++
+* fail if PaymentFailureView is requested on completed orders
+
 0.7.0 (2024-04-12)
 ++++++++++++++++++
 * migrate code to RecurringUserPlan.renewal_triggered_by
 * migrate data of RecurringUserPlans with payment_provider="paypal-recurring" and renewal_triggered_by=TASK to renewal_triggered_by=OTHER
 
 0.6.0 (2023-03-22)
 +++++++++++++++++++
```

### Comparing `django-plans-paypal-0.7.0/django_plans_paypal.egg-info/SOURCES.txt` & `django-plans-paypal-0.7.1/django_plans_paypal.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-plans-paypal-0.7.0/docs/Makefile` & `django-plans-paypal-0.7.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `django-plans-paypal-0.7.0/docs/conf.py` & `django-plans-paypal-0.7.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `django-plans-paypal-0.7.0/docs/make.bat` & `django-plans-paypal-0.7.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `django-plans-paypal-0.7.0/plans_paypal/admin.py` & `django-plans-paypal-0.7.1/plans_paypal/admin.py`

 * *Files identical despite different names*

### Comparing `django-plans-paypal-0.7.0/plans_paypal/hooks.py` & `django-plans-paypal-0.7.1/plans_paypal/hooks.py`

 * *Files identical despite different names*

### Comparing `django-plans-paypal-0.7.0/plans_paypal/migrations/0001_initial.py` & `django-plans-paypal-0.7.1/plans_paypal/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-plans-paypal-0.7.0/plans_paypal/migrations/0002_auto_20211130_1117.py` & `django-plans-paypal-0.7.1/plans_paypal/migrations/0002_auto_20211130_1117.py`

 * *Files identical despite different names*

### Comparing `django-plans-paypal-0.7.0/plans_paypal/migrations/0003_recurringuserplan_renewal_triggered_by_task_to_other.py` & `django-plans-paypal-0.7.1/plans_paypal/migrations/0003_recurringuserplan_renewal_triggered_by_task_to_other.py`

 * *Files identical despite different names*

### Comparing `django-plans-paypal-0.7.0/plans_paypal/models.py` & `django-plans-paypal-0.7.1/plans_paypal/models.py`

 * *Files identical despite different names*

### Comparing `django-plans-paypal-0.7.0/plans_paypal/tests/test_hooks.py` & `django-plans-paypal-0.7.1/plans_paypal/tests/test_hooks.py`

 * *Files identical despite different names*

### Comparing `django-plans-paypal-0.7.0/plans_paypal/tests/test_views.py` & `django-plans-paypal-0.7.1/plans_paypal/tests/test_views.py`

 * *Files 16% similar despite different names*

```diff
@@ -23,14 +23,22 @@
         self.assertEqual(response.status_code, 404)
 
     def test_payment_failure_view_order_does_not_exist(self):
         self.client.force_login(baker.make("User"))
         response = self.client.get(reverse("paypal-payment-failure", args=[1]))
         self.assertEqual(response.status_code, 404)
 
+    def test_payment_failure_view_order_completed(self):
+        order = baker.make(Order, status=Order.STATUS.COMPLETED)
+        self.client.force_login(order.user)
+        with self.assertRaisesRegex(ValueError, r"^Invalid order status: 2"):
+            self.client.get(reverse("paypal-payment-failure", args=[order.id]))
+        order.refresh_from_db()
+        self.assertEqual(order.status, Order.STATUS.COMPLETED)
+
     def test_payment_failure_view_not_logged_in(self):
         order = baker.make(Order, user=baker.make("User"))
         response = self.client.get(reverse("paypal-payment-failure", args=[order.id]))
         self.assertRedirects(
             response,
             "/accounts/login/?next="
             + reverse("paypal-payment-failure", args=[order.id]),
```

### Comparing `django-plans-paypal-0.7.0/plans_paypal/urls.py` & `django-plans-paypal-0.7.1/plans_paypal/urls.py`

 * *Files identical despite different names*

### Comparing `django-plans-paypal-0.7.0/plans_paypal/views.py` & `django-plans-paypal-0.7.1/plans_paypal/views.py`

 * *Files 3% similar despite different names*

```diff
@@ -111,12 +111,15 @@
     context = {"form": form}
     return render(request, "paypal_payments/payment.html", context)
 
 
 class PaymentFailureView(LoginRequiredMixin, View):
     def get(self, request, *args, order_id=None, payment_variant=None):
         order = get_object_or_404(Order, pk=order_id, user=request.user)
+        # This view is meant to cancel the order before it is completed.
+        if order.status == Order.STATUS.COMPLETED:
+            raise ValueError(f"Invalid order status: {order.status}")
         order.status = Order.STATUS.CANCELED
         # In case django-simple-history is installed
         order._change_reason = "Django-payments-paypal: Payment failed by cancel view"
         order.save()
         return redirect(reverse("order_payment_failure", kwargs={"pk": order_id}))
```

### Comparing `django-plans-paypal-0.7.0/runtests.py` & `django-plans-paypal-0.7.1/runtests.py`

 * *Files identical despite different names*

### Comparing `django-plans-paypal-0.7.0/setup.py` & `django-plans-paypal-0.7.1/setup.py`

 * *Files identical despite different names*

### Comparing `django-plans-paypal-0.7.0/tests/settings.py` & `django-plans-paypal-0.7.1/tests/settings.py`

 * *Files identical despite different names*

