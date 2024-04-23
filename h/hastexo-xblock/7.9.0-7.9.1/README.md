# Comparing `tmp/hastexo-xblock-7.9.0.tar.gz` & `tmp/hastexo-xblock-7.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hastexo-xblock-7.9.0.tar", last modified: Thu Jan 11 14:45:39 2024, max compression
+gzip compressed data, was "hastexo-xblock-7.9.1.tar", last modified: Wed Feb 14 14:44:41 2024, max compression
```

## Comparing `hastexo-xblock-7.9.0.tar` & `hastexo-xblock-7.9.1.tar`

### file list

```diff
@@ -1,185 +1,185 @@
-drwxr-xr-x   0 maaritamm   (501) staff       (20)        0 2024-01-11 14:45:39.089664 hastexo-xblock-7.9.0/
--rw-r--r--   0 maaritamm   (501) staff       (20)      358 2024-01-11 14:42:32.000000 hastexo-xblock-7.9.0/.bumpversion.cfg
-drwxr-xr-x   0 maaritamm   (501) staff       (20)        0 2024-01-11 14:45:39.010180 hastexo-xblock-7.9.0/.githooks/
--rwxr-xr-x   0 maaritamm   (501) staff       (20)       29 2024-01-10 14:30:32.000000 hastexo-xblock-7.9.0/.githooks/pre-commit
--rwxr-xr-x   0 maaritamm   (501) staff       (20)       19 2024-01-10 14:30:32.000000 hastexo-xblock-7.9.0/.githooks/pre-push
-drwxr-xr-x   0 maaritamm   (501) staff       (20)        0 2024-01-11 14:45:38.991016 hastexo-xblock-7.9.0/.github/
-drwxr-xr-x   0 maaritamm   (501) staff       (20)        0 2024-01-11 14:45:39.010892 hastexo-xblock-7.9.0/.github/workflows/
--rw-r--r--   0 maaritamm   (501) staff       (20)     1711 2024-01-10 14:30:32.000000 hastexo-xblock-7.9.0/.github/workflows/tox.yml
--rw-r--r--   0 maaritamm   (501) staff       (20)       58 2024-01-10 14:36:26.000000 hastexo-xblock-7.9.0/.gitignore
--rw-r--r--   0 maaritamm   (501) staff       (20)     1238 2024-01-10 14:30:32.000000 hastexo-xblock-7.9.0/.gitlab-ci.yml
--rw-r--r--   0 maaritamm   (501) staff       (20)    29618 2024-01-11 14:42:32.000000 hastexo-xblock-7.9.0/Changelog.md
--rw-r--r--   0 maaritamm   (501) staff       (20)     5452 2024-01-10 14:30:32.000000 hastexo-xblock-7.9.0/HACKING.md
--rw-r--r--   0 maaritamm   (501) staff       (20)    34520 2024-01-10 14:30:32.000000 hastexo-xblock-7.9.0/LICENSE
--rw-r--r--   0 maaritamm   (501) staff       (20)    30919 2024-01-11 14:45:39.089356 hastexo-xblock-7.9.0/PKG-INFO
--rw-r--r--   0 maaritamm   (501) staff       (20)    30187 2024-01-11 14:42:32.000000 hastexo-xblock-7.9.0/README.md
-drwxr-xr-x   0 maaritamm   (501) staff       (20)        0 2024-01-11 14:45:38.991690 hastexo-xblock-7.9.0/fake/
-drwxr-xr-x   0 maaritamm   (501) staff       (20)        0 2024-01-11 14:45:38.991422 hastexo-xblock-7.9.0/fake/common/
-drwxr-xr-x   0 maaritamm   (501) staff       (20)        0 2024-01-11 14:45:38.991528 hastexo-xblock-7.9.0/fake/common/djangoapps/
-drwxr-xr-x   0 maaritamm   (501) staff       (20)        0 2024-01-11 14:45:39.011763 hastexo-xblock-7.9.0/fake/common/djangoapps/student/
--rw-r--r--   0 maaritamm   (501) staff       (20)        0 2024-01-10 14:30:32.000000 hastexo-xblock-7.9.0/fake/common/djangoapps/student/__init__.py
--rw-r--r--   0 maaritamm   (501) staff       (20)      443 2024-01-10 14:30:32.000000 hastexo-xblock-7.9.0/fake/common/djangoapps/student/models.py
-drwxr-xr-x   0 maaritamm   (501) staff       (20)        0 2024-01-11 14:45:39.012298 hastexo-xblock-7.9.0/fake/course/
--rw-r--r--   0 maaritamm   (501) staff       (20)        0 2024-01-10 14:30:32.000000 hastexo-xblock-7.9.0/fake/course/__init__.py
-drwxr-xr-x   0 maaritamm   (501) staff       (20)        0 2024-01-11 14:45:39.019263 hastexo-xblock-7.9.0/hastexo/
--rw-r--r--   0 maaritamm   (501) staff       (20)      347 2024-01-10 14:30:32.000000 hastexo-xblock-7.9.0/hastexo/__init__.py
--rw-r--r--   0 maaritamm   (501) staff       (20)     4167 2024-01-10 14:30:32.000000 hastexo-xblock-7.9.0/hastexo/admin.py
--rw-r--r--   0 maaritamm   (501) staff       (20)    11496 2024-01-11 14:25:10.000000 hastexo-xblock-7.9.0/hastexo/common.py
--rw-r--r--   0 maaritamm   (501) staff       (20)     1560 2024-01-10 14:30:32.000000 hastexo-xblock-7.9.0/hastexo/gcloud.py
--rw-r--r--   0 maaritamm   (501) staff       (20)    44070 2024-01-11 14:25:10.000000 hastexo-xblock-7.9.0/hastexo/hastexo.py
--rw-r--r--   0 maaritamm   (501) staff       (20)     6099 2024-01-10 14:30:32.000000 hastexo-xblock-7.9.0/hastexo/jobs.py
-drwxr-xr-x   0 maaritamm   (501) staff       (20)        0 2024-01-11 14:45:39.020240 hastexo-xblock-7.9.0/hastexo/locale/
--rw-r--r--   0 maaritamm   (501) staff       (20)      341 2024-01-10 14:30:32.000000 hastexo-xblock-7.9.0/hastexo/locale/config.yaml
-drwxr-xr-x   0 maaritamm   (501) staff       (20)        0 2024-01-11 14:45:38.992306 hastexo-xblock-7.9.0/hastexo/locale/en/
-drwxr-xr-x   0 maaritamm   (501) staff       (20)        0 2024-01-11 14:45:39.020909 hastexo-xblock-7.9.0/hastexo/locale/en/LC_MESSAGES/
--rw-r--r--   0 maaritamm   (501) staff       (20)     3512 2024-01-10 14:30:32.000000 hastexo-xblock-7.9.0/hastexo/locale/en/LC_MESSAGES/django-partial.po
-drwxr-xr-x   0 maaritamm   (501) staff       (20)        0 2024-01-11 14:45:39.021494 hastexo-xblock-7.9.0/hastexo/management/
--rw-r--r--   0 maaritamm   (501) staff       (20)        0 2024-01-10 14:30:32.000000 hastexo-xblock-7.9.0/hastexo/management/__init__.py
-drwxr-xr-x   0 maaritamm   (501) staff       (20)        0 2024-01-11 14:45:39.021763 hastexo-xblock-7.9.0/hastexo/management/__pycache__/
--rw-r--r--   0 maaritamm   (501) staff       (20)      171 2024-01-10 14:32:28.000000 hastexo-xblock-7.9.0/hastexo/management/__pycache__/__init__.cpython-38.pyc
-drwxr-xr-x   0 maaritamm   (501) staff       (20)        0 2024-01-11 14:45:39.023293 hastexo-xblock-7.9.0/hastexo/management/commands/
--rw-r--r--   0 maaritamm   (501) staff       (20)        0 2024-01-10 14:30:32.000000 hastexo-xblock-7.9.0/hastexo/management/commands/__init__.py
-drwxr-xr-x   0 maaritamm   (501) staff       (20)        0 2024-01-11 14:45:39.025068 hastexo-xblock-7.9.0/hastexo/management/commands/__pycache__/
--rw-r--r--   0 maaritamm   (501) staff       (20)      180 2024-01-10 14:32:32.000000 hastexo-xblock-7.9.0/hastexo/management/commands/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 maaritamm   (501) staff       (20)     1007 2024-01-10 14:32:32.000000 hastexo-xblock-7.9.0/hastexo/management/commands/__pycache__/reaper.cpython-38.pyc
--rw-r--r--   0 maaritamm   (501) staff       (20)      938 2024-01-10 14:32:32.000000 hastexo-xblock-7.9.0/hastexo/management/commands/__pycache__/suspender.cpython-38.pyc
--rw-r--r--   0 maaritamm   (501) staff       (20)      708 2024-01-10 14:30:32.000000 hastexo-xblock-7.9.0/hastexo/management/commands/reaper.py
--rw-r--r--   0 maaritamm   (501) staff       (20)      639 2024-01-10 14:30:32.000000 hastexo-xblock-7.9.0/hastexo/management/commands/suspender.py
-drwxr-xr-x   0 maaritamm   (501) staff       (20)        0 2024-01-11 14:45:39.033512 hastexo-xblock-7.9.0/hastexo/migrations/
--rw-r--r--   0 maaritamm   (501) staff       (20)     1900 2024-01-10 14:30:32.000000 hastexo-xblock-7.9.0/hastexo/migrations/0001_initial.py
--rw-r--r--   0 maaritamm   (501) staff       (20)     2016 2024-01-10 14:30:32.000000 hastexo-xblock-7.9.0/hastexo/migrations/0002_stacklog.py
--rw-r--r--   0 maaritamm   (501) staff       (20)     2596 2024-01-10 14:30:32.000000 hastexo-xblock-7.9.0/hastexo/migrations/0003_blanks.py
--rw-r--r--   0 maaritamm   (501) staff       (20)      560 2024-01-10 14:30:32.000000 hastexo-xblock-7.9.0/hastexo/migrations/0004_auto_20190715_1053.py
--rw-r--r--   0 maaritamm   (501) staff       (20)     1647 2024-01-10 14:30:32.000000 hastexo-xblock-7.9.0/hastexo/migrations/0005_auto_20190811_1555.py
--rw-r--r--   0 maaritamm   (501) staff       (20)     1469 2024-01-10 14:30:32.000000 hastexo-xblock-7.9.0/hastexo/migrations/0006_auto_20200107_1332.py
--rw-r--r--   0 maaritamm   (501) staff       (20)     1034 2024-01-10 14:30:32.000000 hastexo-xblock-7.9.0/hastexo/migrations/0007_add_delete_by_and_delete_age.py
--rw-r--r--   0 maaritamm   (501) staff       (20)      581 2024-01-10 14:30:32.000000 hastexo-xblock-7.9.0/hastexo/migrations/0008_add_database_defaults_for_stack_key_and_password.py
--rw-r--r--   0 maaritamm   (501) staff       (20)      599 2024-01-10 14:30:32.000000 hastexo-xblock-7.9.0/hastexo/migrations/0009_add_null_true_for_key_and_password.py
--rw-r--r--   0 maaritamm   (501) staff       (20)     1748 2024-01-10 14:30:32.000000 hastexo-xblock-7.9.0/hastexo/migrations/0010_add_user_foreign_key.py
--rw-r--r--   0 maaritamm   (501) staff       (20)     1018 2024-01-10 14:30:32.000000 hastexo-xblock-7.9.0/hastexo/migrations/0011_allow_null_for_learner.py
--rw-r--r--   0 maaritamm   (501) staff       (20)      529 2024-01-10 14:30:32.000000 hastexo-xblock-7.9.0/hastexo/migrations/0012_add_suspend_by.py
--rw-r--r--   0 maaritamm   (501) staff       (20)        0 2024-01-10 14:30:32.000000 hastexo-xblock-7.9.0/hastexo/migrations/__init__.py
-drwxr-xr-x   0 maaritamm   (501) staff       (20)        0 2024-01-11 14:45:39.042155 hastexo-xblock-7.9.0/hastexo/migrations/__pycache__/
--rw-r--r--   0 maaritamm   (501) staff       (20)     1369 2024-01-10 14:32:28.000000 hastexo-xblock-7.9.0/hastexo/migrations/__pycache__/0001_initial.cpython-38.pyc
--rw-r--r--   0 maaritamm   (501) staff       (20)     1444 2024-01-10 14:32:28.000000 hastexo-xblock-7.9.0/hastexo/migrations/__pycache__/0002_stacklog.cpython-38.pyc
--rw-r--r--   0 maaritamm   (501) staff       (20)     1225 2024-01-10 14:32:28.000000 hastexo-xblock-7.9.0/hastexo/migrations/__pycache__/0003_blanks.cpython-38.pyc
--rw-r--r--   0 maaritamm   (501) staff       (20)      708 2024-01-10 14:32:28.000000 hastexo-xblock-7.9.0/hastexo/migrations/__pycache__/0004_auto_20190715_1053.cpython-38.pyc
--rw-r--r--   0 maaritamm   (501) staff       (20)     1047 2024-01-10 14:32:28.000000 hastexo-xblock-7.9.0/hastexo/migrations/__pycache__/0005_auto_20190811_1555.cpython-38.pyc
--rw-r--r--   0 maaritamm   (501) staff       (20)     1160 2024-01-10 14:32:28.000000 hastexo-xblock-7.9.0/hastexo/migrations/__pycache__/0006_auto_20200107_1332.cpython-38.pyc
--rw-r--r--   0 maaritamm   (501) staff       (20)      853 2024-01-10 14:32:28.000000 hastexo-xblock-7.9.0/hastexo/migrations/__pycache__/0007_add_delete_by_and_delete_age.cpython-38.pyc
--rw-r--r--   0 maaritamm   (501) staff       (20)      736 2024-01-10 14:32:28.000000 hastexo-xblock-7.9.0/hastexo/migrations/__pycache__/0008_add_database_defaults_for_stack_key_and_password.cpython-38.pyc
--rw-r--r--   0 maaritamm   (501) staff       (20)      737 2024-01-10 14:32:28.000000 hastexo-xblock-7.9.0/hastexo/migrations/__pycache__/0009_add_null_true_for_key_and_password.cpython-38.pyc
--rw-r--r--   0 maaritamm   (501) staff       (20)     1628 2024-01-10 14:32:28.000000 hastexo-xblock-7.9.0/hastexo/migrations/__pycache__/0010_add_user_foreign_key.cpython-38.pyc
--rw-r--r--   0 maaritamm   (501) staff       (20)      802 2024-01-10 14:32:28.000000 hastexo-xblock-7.9.0/hastexo/migrations/__pycache__/0011_allow_null_for_learner.cpython-38.pyc
--rw-r--r--   0 maaritamm   (501) staff       (20)      661 2024-01-10 14:32:28.000000 hastexo-xblock-7.9.0/hastexo/migrations/__pycache__/0012_add_suspend_by.cpython-38.pyc
--rw-r--r--   0 maaritamm   (501) staff       (20)      171 2024-01-10 14:32:28.000000 hastexo-xblock-7.9.0/hastexo/migrations/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 maaritamm   (501) staff       (20)     3644 2024-01-10 14:30:32.000000 hastexo-xblock-7.9.0/hastexo/models.py
--rw-r--r--   0 maaritamm   (501) staff       (20)     4614 2024-01-10 14:30:32.000000 hastexo-xblock-7.9.0/hastexo/openstack.py
--rw-r--r--   0 maaritamm   (501) staff       (20)    29112 2024-01-10 14:30:32.000000 hastexo-xblock-7.9.0/hastexo/provider.py
-drwxr-xr-x   0 maaritamm   (501) staff       (20)        0 2024-01-11 14:45:38.993680 hastexo-xblock-7.9.0/hastexo/public/
-drwxr-xr-x   0 maaritamm   (501) staff       (20)        0 2024-01-11 14:45:39.042801 hastexo-xblock-7.9.0/hastexo/public/css/
--rw-r--r--   0 maaritamm   (501) staff       (20)     3279 2024-01-10 14:30:32.000000 hastexo-xblock-7.9.0/hastexo/public/css/main.css
-drwxr-xr-x   0 maaritamm   (501) staff       (20)        0 2024-01-11 14:45:39.045416 hastexo-xblock-7.9.0/hastexo/public/js/
--rw-r--r--   0 maaritamm   (501) staff       (20)     7621 2024-01-10 14:30:32.000000 hastexo-xblock-7.9.0/hastexo/public/js/client.js
-drwxr-xr-x   0 maaritamm   (501) staff       (20)        0 2024-01-11 14:45:39.050413 hastexo-xblock-7.9.0/hastexo/public/js/guacamole-common-js/
--rw-r--r--   0 maaritamm   (501) staff       (20)    67952 2024-01-10 14:30:32.000000 hastexo-xblock-7.9.0/hastexo/public/js/guacamole-common-js/0.9.13-incubating-all.min.js
--rw-r--r--   0 maaritamm   (501) staff       (20)    70401 2024-01-10 14:30:32.000000 hastexo-xblock-7.9.0/hastexo/public/js/guacamole-common-js/1.4.0-all.min.js
--rw-r--r--   0 maaritamm   (501) staff       (20)    72449 2024-01-11 10:58:49.000000 hastexo-xblock-7.9.0/hastexo/public/js/guacamole-common-js/1.5.2-all.min.js
--rw-r--r--   0 maaritamm   (501) staff       (20)    72461 2024-01-11 14:25:10.000000 hastexo-xblock-7.9.0/hastexo/public/js/guacamole-common-js/1.5.4-all.min.js
--rw-r--r--   0 maaritamm   (501) staff       (20)    18617 2024-01-10 14:30:32.000000 hastexo-xblock-7.9.0/hastexo/public/js/main.js
--rw-r--r--   0 maaritamm   (501) staff       (20)     2344 2024-01-10 14:30:32.000000 hastexo-xblock-7.9.0/hastexo/public/js/plugins.js
-drwxr-xr-x   0 maaritamm   (501) staff       (20)        0 2024-01-11 14:45:38.995059 hastexo-xblock-7.9.0/hastexo/public/js/translations/
-drwxr-xr-x   0 maaritamm   (501) staff       (20)        0 2024-01-11 14:45:39.051757 hastexo-xblock-7.9.0/hastexo/public/js/translations/de-de/
--rw-r--r--   0 maaritamm   (501) staff       (20)     7160 2024-01-10 14:30:32.000000 hastexo-xblock-7.9.0/hastexo/public/js/translations/de-de/text.js
-drwxr-xr-x   0 maaritamm   (501) staff       (20)        0 2024-01-11 14:45:39.052619 hastexo-xblock-7.9.0/hastexo/public/js/translations/el/
--rw-r--r--   0 maaritamm   (501) staff       (20)    14190 2024-01-10 14:30:32.000000 hastexo-xblock-7.9.0/hastexo/public/js/translations/el/text.js
-drwxr-xr-x   0 maaritamm   (501) staff       (20)        0 2024-01-11 14:45:39.053232 hastexo-xblock-7.9.0/hastexo/public/js/translations/es-419/
--rw-r--r--   0 maaritamm   (501) staff       (20)     6916 2024-01-10 14:30:32.000000 hastexo-xblock-7.9.0/hastexo/public/js/translations/es-419/text.js
-drwxr-xr-x   0 maaritamm   (501) staff       (20)        0 2024-01-11 14:45:39.054082 hastexo-xblock-7.9.0/hastexo/public/js/translations/et-ee/
--rw-r--r--   0 maaritamm   (501) staff       (20)     7131 2024-01-10 14:30:32.000000 hastexo-xblock-7.9.0/hastexo/public/js/translations/et-ee/text.js
-drwxr-xr-x   0 maaritamm   (501) staff       (20)        0 2024-01-11 14:45:39.054666 hastexo-xblock-7.9.0/hastexo/public/js/translations/hi/
--rw-r--r--   0 maaritamm   (501) staff       (20)    12785 2024-01-10 14:30:32.000000 hastexo-xblock-7.9.0/hastexo/public/js/translations/hi/text.js
-drwxr-xr-x   0 maaritamm   (501) staff       (20)        0 2024-01-11 14:45:38.995389 hastexo-xblock-7.9.0/hastexo/static/
-drwxr-xr-x   0 maaritamm   (501) staff       (20)        0 2024-01-11 14:45:39.055930 hastexo-xblock-7.9.0/hastexo/static/html/
--rw-r--r--   0 maaritamm   (501) staff       (20)     3111 2024-01-10 14:30:32.000000 hastexo-xblock-7.9.0/hastexo/static/html/lab.html
--rw-r--r--   0 maaritamm   (501) staff       (20)     3445 2024-01-10 14:30:32.000000 hastexo-xblock-7.9.0/hastexo/static/html/main.html
--rw-r--r--   0 maaritamm   (501) staff       (20)    34877 2024-01-10 14:30:32.000000 hastexo-xblock-7.9.0/hastexo/tasks.py
-drwxr-xr-x   0 maaritamm   (501) staff       (20)        0 2024-01-11 14:45:38.997509 hastexo-xblock-7.9.0/hastexo/translations/
-drwxr-xr-x   0 maaritamm   (501) staff       (20)        0 2024-01-11 14:45:38.995786 hastexo-xblock-7.9.0/hastexo/translations/de_DE/
-drwxr-xr-x   0 maaritamm   (501) staff       (20)        0 2024-01-11 14:45:39.057192 hastexo-xblock-7.9.0/hastexo/translations/de_DE/LC_MESSAGES/
--rw-r--r--   0 maaritamm   (501) staff       (20)     4125 2024-01-10 14:30:32.000000 hastexo-xblock-7.9.0/hastexo/translations/de_DE/LC_MESSAGES/text.mo
--rw-r--r--   0 maaritamm   (501) staff       (20)     5146 2024-01-10 14:30:32.000000 hastexo-xblock-7.9.0/hastexo/translations/de_DE/LC_MESSAGES/text.po
-drwxr-xr-x   0 maaritamm   (501) staff       (20)        0 2024-01-11 14:45:38.996144 hastexo-xblock-7.9.0/hastexo/translations/el/
-drwxr-xr-x   0 maaritamm   (501) staff       (20)        0 2024-01-11 14:45:39.058640 hastexo-xblock-7.9.0/hastexo/translations/el/LC_MESSAGES/
--rw-r--r--   0 maaritamm   (501) staff       (20)     5594 2024-01-10 14:30:32.000000 hastexo-xblock-7.9.0/hastexo/translations/el/LC_MESSAGES/text.mo
--rw-r--r--   0 maaritamm   (501) staff       (20)     6657 2024-01-10 14:30:32.000000 hastexo-xblock-7.9.0/hastexo/translations/el/LC_MESSAGES/text.po
-drwxr-xr-x   0 maaritamm   (501) staff       (20)        0 2024-01-11 14:45:38.996538 hastexo-xblock-7.9.0/hastexo/translations/en/
-drwxr-xr-x   0 maaritamm   (501) staff       (20)        0 2024-01-11 14:45:39.060153 hastexo-xblock-7.9.0/hastexo/translations/en/LC_MESSAGES/
--rw-r--r--   0 maaritamm   (501) staff       (20)      380 2024-01-10 14:30:32.000000 hastexo-xblock-7.9.0/hastexo/translations/en/LC_MESSAGES/text.mo
--rw-r--r--   0 maaritamm   (501) staff       (20)     3512 2024-01-10 14:30:32.000000 hastexo-xblock-7.9.0/hastexo/translations/en/LC_MESSAGES/text.po
-drwxr-xr-x   0 maaritamm   (501) staff       (20)        0 2024-01-11 14:45:38.997010 hastexo-xblock-7.9.0/hastexo/translations/es_419/
-drwxr-xr-x   0 maaritamm   (501) staff       (20)        0 2024-01-11 14:45:39.061983 hastexo-xblock-7.9.0/hastexo/translations/es_419/LC_MESSAGES/
--rw-r--r--   0 maaritamm   (501) staff       (20)     4101 2024-01-10 14:30:32.000000 hastexo-xblock-7.9.0/hastexo/translations/es_419/LC_MESSAGES/text.mo
--rw-r--r--   0 maaritamm   (501) staff       (20)     5122 2024-01-10 14:30:32.000000 hastexo-xblock-7.9.0/hastexo/translations/es_419/LC_MESSAGES/text.po
-drwxr-xr-x   0 maaritamm   (501) staff       (20)        0 2024-01-11 14:45:38.997333 hastexo-xblock-7.9.0/hastexo/translations/et_EE/
-drwxr-xr-x   0 maaritamm   (501) staff       (20)        0 2024-01-11 14:45:39.063533 hastexo-xblock-7.9.0/hastexo/translations/et_EE/LC_MESSAGES/
--rw-r--r--   0 maaritamm   (501) staff       (20)     3926 2024-01-10 14:30:32.000000 hastexo-xblock-7.9.0/hastexo/translations/et_EE/LC_MESSAGES/text.mo
--rw-r--r--   0 maaritamm   (501) staff       (20)     4950 2024-01-10 14:30:32.000000 hastexo-xblock-7.9.0/hastexo/translations/et_EE/LC_MESSAGES/text.po
-drwxr-xr-x   0 maaritamm   (501) staff       (20)        0 2024-01-11 14:45:38.997651 hastexo-xblock-7.9.0/hastexo/translations/hi/
-drwxr-xr-x   0 maaritamm   (501) staff       (20)        0 2024-01-11 14:45:39.065074 hastexo-xblock-7.9.0/hastexo/translations/hi/LC_MESSAGES/
--rw-r--r--   0 maaritamm   (501) staff       (20)     6255 2024-01-10 14:30:32.000000 hastexo-xblock-7.9.0/hastexo/translations/hi/LC_MESSAGES/text.mo
--rw-r--r--   0 maaritamm   (501) staff       (20)     7294 2024-01-10 14:30:32.000000 hastexo-xblock-7.9.0/hastexo/translations/hi/LC_MESSAGES/text.po
-drwxr-xr-x   0 maaritamm   (501) staff       (20)        0 2024-01-11 14:45:39.067554 hastexo-xblock-7.9.0/hastexo_guacamole_client/
--rw-r--r--   0 maaritamm   (501) staff       (20)        0 2024-01-10 14:30:32.000000 hastexo-xblock-7.9.0/hastexo_guacamole_client/__init__.py
--rw-r--r--   0 maaritamm   (501) staff       (20)      896 2024-01-10 14:30:32.000000 hastexo-xblock-7.9.0/hastexo_guacamole_client/asgi.py
--rw-r--r--   0 maaritamm   (501) staff       (20)     3347 2024-01-10 14:30:32.000000 hastexo-xblock-7.9.0/hastexo_guacamole_client/consumers.py
--rw-r--r--   0 maaritamm   (501) staff       (20)     2742 2024-01-10 14:30:32.000000 hastexo-xblock-7.9.0/hastexo_guacamole_client/settings.py
-drwxr-xr-x   0 maaritamm   (501) staff       (20)        0 2024-01-11 14:45:39.069882 hastexo-xblock-7.9.0/hastexo_xblock.egg-info/
--rw-r--r--   0 maaritamm   (501) staff       (20)    30919 2024-01-11 14:45:38.000000 hastexo-xblock-7.9.0/hastexo_xblock.egg-info/PKG-INFO
--rw-r--r--   0 maaritamm   (501) staff       (20)     4988 2024-01-11 14:45:38.000000 hastexo-xblock-7.9.0/hastexo_xblock.egg-info/SOURCES.txt
--rw-r--r--   0 maaritamm   (501) staff       (20)        1 2024-01-11 14:45:38.000000 hastexo-xblock-7.9.0/hastexo_xblock.egg-info/dependency_links.txt
--rw-r--r--   0 maaritamm   (501) staff       (20)       52 2024-01-11 14:45:38.000000 hastexo-xblock-7.9.0/hastexo_xblock.egg-info/entry_points.txt
--rw-r--r--   0 maaritamm   (501) staff       (20)      138 2024-01-11 14:45:38.000000 hastexo-xblock-7.9.0/hastexo_xblock.egg-info/requires.txt
--rw-r--r--   0 maaritamm   (501) staff       (20)        8 2024-01-11 14:45:38.000000 hastexo-xblock-7.9.0/hastexo_xblock.egg-info/top_level.txt
-drwxr-xr-x   0 maaritamm   (501) staff       (20)        0 2024-01-11 14:45:39.072102 hastexo-xblock-7.9.0/requirements/
--rw-r--r--   0 maaritamm   (501) staff       (20)      690 2024-01-11 14:25:10.000000 hastexo-xblock-7.9.0/requirements/base.txt
--rw-r--r--   0 maaritamm   (501) staff       (20)        7 2024-01-10 14:30:32.000000 hastexo-xblock-7.9.0/requirements/flake8.txt
--rw-r--r--   0 maaritamm   (501) staff       (20)       41 2024-01-10 14:30:32.000000 hastexo-xblock-7.9.0/requirements/setup.txt
--rw-r--r--   0 maaritamm   (501) staff       (20)      359 2024-01-10 14:30:32.000000 hastexo-xblock-7.9.0/requirements/test.txt
--rw-r--r--   0 maaritamm   (501) staff       (20)      690 2024-01-11 14:25:10.000000 hastexo-xblock-7.9.0/requirements.txt
--rwxr-xr-x   0 maaritamm   (501) staff       (20)     2000 2024-01-10 14:30:32.000000 hastexo-xblock-7.9.0/run_tests.py
-drwxr-xr-x   0 maaritamm   (501) staff       (20)        0 2024-01-11 14:45:38.999081 hastexo-xblock-7.9.0/samples/
-drwxr-xr-x   0 maaritamm   (501) staff       (20)        0 2024-01-11 14:45:39.072829 hastexo-xblock-7.9.0/samples/gcloud/
--rw-r--r--   0 maaritamm   (501) staff       (20)     2198 2024-01-10 14:30:32.000000 hastexo-xblock-7.9.0/samples/gcloud/sample-template.yaml.jinja
-drwxr-xr-x   0 maaritamm   (501) staff       (20)        0 2024-01-11 14:45:39.073393 hastexo-xblock-7.9.0/samples/hot/
--rw-r--r--   0 maaritamm   (501) staff       (20)    13209 2024-01-10 14:30:32.000000 hastexo-xblock-7.9.0/samples/hot/sample-template.yaml
--rw-r--r--   0 maaritamm   (501) staff       (20)       38 2024-01-11 14:45:39.089751 hastexo-xblock-7.9.0/setup.cfg
--rwxr-xr-x   0 maaritamm   (501) staff       (20)     2372 2024-01-10 14:30:32.000000 hastexo-xblock-7.9.0/setup.py
-drwxr-xr-x   0 maaritamm   (501) staff       (20)        0 2024-01-11 14:45:39.074006 hastexo-xblock-7.9.0/src/
--rw-r--r--   0 maaritamm   (501) staff       (20)      185 2024-01-10 14:30:32.000000 hastexo-xblock-7.9.0/src/pip-delete-this-directory.txt
-drwxr-xr-x   0 maaritamm   (501) staff       (20)        0 2024-01-11 14:45:39.074577 hastexo-xblock-7.9.0/tests/
--rw-r--r--   0 maaritamm   (501) staff       (20)        0 2024-01-10 14:30:32.000000 hastexo-xblock-7.9.0/tests/__init__.py
-drwxr-xr-x   0 maaritamm   (501) staff       (20)        0 2024-01-11 14:45:39.000235 hastexo-xblock-7.9.0/tests/resources/
-drwxr-xr-x   0 maaritamm   (501) staff       (20)        0 2024-01-11 14:45:39.000346 hastexo-xblock-7.9.0/tests/resources/course/
-drwxr-xr-x   0 maaritamm   (501) staff       (20)        0 2024-01-11 14:45:39.079611 hastexo-xblock-7.9.0/tests/resources/course/hastexo/
--rw-r--r--   0 maaritamm   (501) staff       (20)      488 2024-01-10 14:30:32.000000 hastexo-xblock-7.9.0/tests/resources/course/hastexo/fake_lab_1.xml
--rw-r--r--   0 maaritamm   (501) staff       (20)      346 2024-01-10 14:30:32.000000 hastexo-xblock-7.9.0/tests/resources/course/hastexo/fake_lab_2.xml
--rw-r--r--   0 maaritamm   (501) staff       (20)       67 2024-01-10 14:30:32.000000 hastexo-xblock-7.9.0/tests/resources/course/hastexo/fake_lab_hook_events_1.xml
--rw-r--r--   0 maaritamm   (501) staff       (20)       69 2024-01-10 14:30:32.000000 hastexo-xblock-7.9.0/tests/resources/course/hastexo/fake_lab_hook_events_2.xml
--rw-r--r--   0 maaritamm   (501) staff       (20)       45 2024-01-10 14:30:32.000000 hastexo-xblock-7.9.0/tests/resources/course/hastexo/fake_lab_no_port_name.xml
--rw-r--r--   0 maaritamm   (501) staff       (20)       46 2024-01-10 14:30:32.000000 hastexo-xblock-7.9.0/tests/resources/course/hastexo/fake_lab_no_port_number.xml
--rw-r--r--   0 maaritamm   (501) staff       (20)      301 2024-01-10 14:30:32.000000 hastexo-xblock-7.9.0/tests/resources/course/hastexo/fake_lab_no_provider_capacity.xml
--rw-r--r--   0 maaritamm   (501) staff       (20)      101 2024-01-10 14:30:32.000000 hastexo-xblock-7.9.0/tests/resources/course/hastexo/fake_lab_no_provider_name.xml
-drwxr-xr-x   0 maaritamm   (501) staff       (20)        0 2024-01-11 14:45:39.087897 hastexo-xblock-7.9.0/tests/unit/
--rw-r--r--   0 maaritamm   (501) staff       (20)        0 2024-01-10 14:30:32.000000 hastexo-xblock-7.9.0/tests/unit/__init__.py
--rw-r--r--   0 maaritamm   (501) staff       (20)     5947 2024-01-10 14:30:32.000000 hastexo-xblock-7.9.0/tests/unit/test_admin.py
--rw-r--r--   0 maaritamm   (501) staff       (20)      976 2024-01-10 14:30:32.000000 hastexo-xblock-7.9.0/tests/unit/test_commands.py
--rw-r--r--   0 maaritamm   (501) staff       (20)     9618 2024-01-10 14:30:32.000000 hastexo-xblock-7.9.0/tests/unit/test_common.py
--rw-r--r--   0 maaritamm   (501) staff       (20)     5062 2024-01-10 14:30:32.000000 hastexo-xblock-7.9.0/tests/unit/test_gcloud.py
--rw-r--r--   0 maaritamm   (501) staff       (20)    63018 2024-01-10 14:30:32.000000 hastexo-xblock-7.9.0/tests/unit/test_hastexo.py
--rw-r--r--   0 maaritamm   (501) staff       (20)    21787 2024-01-10 14:30:32.000000 hastexo-xblock-7.9.0/tests/unit/test_jobs.py
--rw-r--r--   0 maaritamm   (501) staff       (20)     2623 2024-01-10 14:30:32.000000 hastexo-xblock-7.9.0/tests/unit/test_models.py
--rw-r--r--   0 maaritamm   (501) staff       (20)     6648 2024-01-10 14:30:32.000000 hastexo-xblock-7.9.0/tests/unit/test_openstack.py
--rw-r--r--   0 maaritamm   (501) staff       (20)    71703 2024-01-10 14:30:32.000000 hastexo-xblock-7.9.0/tests/unit/test_provider.py
--rw-r--r--   0 maaritamm   (501) staff       (20)    71832 2024-01-10 14:30:32.000000 hastexo-xblock-7.9.0/tests/unit/test_tasks.py
--rw-r--r--   0 maaritamm   (501) staff       (20)     1516 2024-01-10 14:30:32.000000 hastexo-xblock-7.9.0/tox.ini
+drwxr-xr-x   0 maaritamm   (501) staff       (20)        0 2024-02-14 14:44:41.144353 hastexo-xblock-7.9.1/
+-rw-r--r--   0 maaritamm   (501) staff       (20)      358 2024-02-14 14:39:58.000000 hastexo-xblock-7.9.1/.bumpversion.cfg
+drwxr-xr-x   0 maaritamm   (501) staff       (20)        0 2024-02-14 14:44:41.049739 hastexo-xblock-7.9.1/.githooks/
+-rwxr-xr-x   0 maaritamm   (501) staff       (20)       29 2024-01-10 14:30:32.000000 hastexo-xblock-7.9.1/.githooks/pre-commit
+-rwxr-xr-x   0 maaritamm   (501) staff       (20)       19 2024-01-10 14:30:32.000000 hastexo-xblock-7.9.1/.githooks/pre-push
+drwxr-xr-x   0 maaritamm   (501) staff       (20)        0 2024-02-14 14:44:41.024217 hastexo-xblock-7.9.1/.github/
+drwxr-xr-x   0 maaritamm   (501) staff       (20)        0 2024-02-14 14:44:41.050784 hastexo-xblock-7.9.1/.github/workflows/
+-rw-r--r--   0 maaritamm   (501) staff       (20)     1711 2024-01-10 14:30:32.000000 hastexo-xblock-7.9.1/.github/workflows/tox.yml
+-rw-r--r--   0 maaritamm   (501) staff       (20)       58 2024-01-10 14:36:26.000000 hastexo-xblock-7.9.1/.gitignore
+-rw-r--r--   0 maaritamm   (501) staff       (20)     1238 2024-01-10 14:30:32.000000 hastexo-xblock-7.9.1/.gitlab-ci.yml
+-rw-r--r--   0 maaritamm   (501) staff       (20)    29820 2024-02-14 14:39:58.000000 hastexo-xblock-7.9.1/Changelog.md
+-rw-r--r--   0 maaritamm   (501) staff       (20)     5452 2024-01-10 14:30:32.000000 hastexo-xblock-7.9.1/HACKING.md
+-rw-r--r--   0 maaritamm   (501) staff       (20)    34520 2024-01-10 14:30:32.000000 hastexo-xblock-7.9.1/LICENSE
+-rw-r--r--   0 maaritamm   (501) staff       (20)    30919 2024-02-14 14:44:41.143673 hastexo-xblock-7.9.1/PKG-INFO
+-rw-r--r--   0 maaritamm   (501) staff       (20)    30187 2024-02-14 14:39:58.000000 hastexo-xblock-7.9.1/README.md
+drwxr-xr-x   0 maaritamm   (501) staff       (20)        0 2024-02-14 14:44:41.024907 hastexo-xblock-7.9.1/fake/
+drwxr-xr-x   0 maaritamm   (501) staff       (20)        0 2024-02-14 14:44:41.024628 hastexo-xblock-7.9.1/fake/common/
+drwxr-xr-x   0 maaritamm   (501) staff       (20)        0 2024-02-14 14:44:41.024737 hastexo-xblock-7.9.1/fake/common/djangoapps/
+drwxr-xr-x   0 maaritamm   (501) staff       (20)        0 2024-02-14 14:44:41.052000 hastexo-xblock-7.9.1/fake/common/djangoapps/student/
+-rw-r--r--   0 maaritamm   (501) staff       (20)        0 2024-01-10 14:30:32.000000 hastexo-xblock-7.9.1/fake/common/djangoapps/student/__init__.py
+-rw-r--r--   0 maaritamm   (501) staff       (20)      443 2024-01-10 14:30:32.000000 hastexo-xblock-7.9.1/fake/common/djangoapps/student/models.py
+drwxr-xr-x   0 maaritamm   (501) staff       (20)        0 2024-02-14 14:44:41.052589 hastexo-xblock-7.9.1/fake/course/
+-rw-r--r--   0 maaritamm   (501) staff       (20)        0 2024-01-10 14:30:32.000000 hastexo-xblock-7.9.1/fake/course/__init__.py
+drwxr-xr-x   0 maaritamm   (501) staff       (20)        0 2024-02-14 14:44:41.059841 hastexo-xblock-7.9.1/hastexo/
+-rw-r--r--   0 maaritamm   (501) staff       (20)      347 2024-01-10 14:30:32.000000 hastexo-xblock-7.9.1/hastexo/__init__.py
+-rw-r--r--   0 maaritamm   (501) staff       (20)     4167 2024-01-10 14:30:32.000000 hastexo-xblock-7.9.1/hastexo/admin.py
+-rw-r--r--   0 maaritamm   (501) staff       (20)    11496 2024-02-12 13:10:32.000000 hastexo-xblock-7.9.1/hastexo/common.py
+-rw-r--r--   0 maaritamm   (501) staff       (20)     1560 2024-01-10 14:30:32.000000 hastexo-xblock-7.9.1/hastexo/gcloud.py
+-rw-r--r--   0 maaritamm   (501) staff       (20)    44179 2024-02-14 12:09:36.000000 hastexo-xblock-7.9.1/hastexo/hastexo.py
+-rw-r--r--   0 maaritamm   (501) staff       (20)     6099 2024-01-10 14:30:32.000000 hastexo-xblock-7.9.1/hastexo/jobs.py
+drwxr-xr-x   0 maaritamm   (501) staff       (20)        0 2024-02-14 14:44:41.060632 hastexo-xblock-7.9.1/hastexo/locale/
+-rw-r--r--   0 maaritamm   (501) staff       (20)      341 2024-01-10 14:30:32.000000 hastexo-xblock-7.9.1/hastexo/locale/config.yaml
+drwxr-xr-x   0 maaritamm   (501) staff       (20)        0 2024-02-14 14:44:41.025555 hastexo-xblock-7.9.1/hastexo/locale/en/
+drwxr-xr-x   0 maaritamm   (501) staff       (20)        0 2024-02-14 14:44:41.061600 hastexo-xblock-7.9.1/hastexo/locale/en/LC_MESSAGES/
+-rw-r--r--   0 maaritamm   (501) staff       (20)     3512 2024-01-10 14:30:32.000000 hastexo-xblock-7.9.1/hastexo/locale/en/LC_MESSAGES/django-partial.po
+drwxr-xr-x   0 maaritamm   (501) staff       (20)        0 2024-02-14 14:44:41.062470 hastexo-xblock-7.9.1/hastexo/management/
+-rw-r--r--   0 maaritamm   (501) staff       (20)        0 2024-01-10 14:30:32.000000 hastexo-xblock-7.9.1/hastexo/management/__init__.py
+drwxr-xr-x   0 maaritamm   (501) staff       (20)        0 2024-02-14 14:44:41.062977 hastexo-xblock-7.9.1/hastexo/management/__pycache__/
+-rw-r--r--   0 maaritamm   (501) staff       (20)      171 2024-01-10 14:32:28.000000 hastexo-xblock-7.9.1/hastexo/management/__pycache__/__init__.cpython-38.pyc
+drwxr-xr-x   0 maaritamm   (501) staff       (20)        0 2024-02-14 14:44:41.064842 hastexo-xblock-7.9.1/hastexo/management/commands/
+-rw-r--r--   0 maaritamm   (501) staff       (20)        0 2024-01-10 14:30:32.000000 hastexo-xblock-7.9.1/hastexo/management/commands/__init__.py
+drwxr-xr-x   0 maaritamm   (501) staff       (20)        0 2024-02-14 14:44:41.067301 hastexo-xblock-7.9.1/hastexo/management/commands/__pycache__/
+-rw-r--r--   0 maaritamm   (501) staff       (20)      180 2024-01-10 14:32:32.000000 hastexo-xblock-7.9.1/hastexo/management/commands/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 maaritamm   (501) staff       (20)     1007 2024-01-10 14:32:32.000000 hastexo-xblock-7.9.1/hastexo/management/commands/__pycache__/reaper.cpython-38.pyc
+-rw-r--r--   0 maaritamm   (501) staff       (20)      938 2024-01-10 14:32:32.000000 hastexo-xblock-7.9.1/hastexo/management/commands/__pycache__/suspender.cpython-38.pyc
+-rw-r--r--   0 maaritamm   (501) staff       (20)      708 2024-01-10 14:30:32.000000 hastexo-xblock-7.9.1/hastexo/management/commands/reaper.py
+-rw-r--r--   0 maaritamm   (501) staff       (20)      639 2024-01-10 14:30:32.000000 hastexo-xblock-7.9.1/hastexo/management/commands/suspender.py
+drwxr-xr-x   0 maaritamm   (501) staff       (20)        0 2024-02-14 14:44:41.075265 hastexo-xblock-7.9.1/hastexo/migrations/
+-rw-r--r--   0 maaritamm   (501) staff       (20)     1900 2024-01-10 14:30:32.000000 hastexo-xblock-7.9.1/hastexo/migrations/0001_initial.py
+-rw-r--r--   0 maaritamm   (501) staff       (20)     2016 2024-01-10 14:30:32.000000 hastexo-xblock-7.9.1/hastexo/migrations/0002_stacklog.py
+-rw-r--r--   0 maaritamm   (501) staff       (20)     2596 2024-01-10 14:30:32.000000 hastexo-xblock-7.9.1/hastexo/migrations/0003_blanks.py
+-rw-r--r--   0 maaritamm   (501) staff       (20)      560 2024-01-10 14:30:32.000000 hastexo-xblock-7.9.1/hastexo/migrations/0004_auto_20190715_1053.py
+-rw-r--r--   0 maaritamm   (501) staff       (20)     1647 2024-01-10 14:30:32.000000 hastexo-xblock-7.9.1/hastexo/migrations/0005_auto_20190811_1555.py
+-rw-r--r--   0 maaritamm   (501) staff       (20)     1469 2024-01-10 14:30:32.000000 hastexo-xblock-7.9.1/hastexo/migrations/0006_auto_20200107_1332.py
+-rw-r--r--   0 maaritamm   (501) staff       (20)     1034 2024-01-10 14:30:32.000000 hastexo-xblock-7.9.1/hastexo/migrations/0007_add_delete_by_and_delete_age.py
+-rw-r--r--   0 maaritamm   (501) staff       (20)      581 2024-01-10 14:30:32.000000 hastexo-xblock-7.9.1/hastexo/migrations/0008_add_database_defaults_for_stack_key_and_password.py
+-rw-r--r--   0 maaritamm   (501) staff       (20)      599 2024-01-10 14:30:32.000000 hastexo-xblock-7.9.1/hastexo/migrations/0009_add_null_true_for_key_and_password.py
+-rw-r--r--   0 maaritamm   (501) staff       (20)     1748 2024-01-10 14:30:32.000000 hastexo-xblock-7.9.1/hastexo/migrations/0010_add_user_foreign_key.py
+-rw-r--r--   0 maaritamm   (501) staff       (20)     1018 2024-01-10 14:30:32.000000 hastexo-xblock-7.9.1/hastexo/migrations/0011_allow_null_for_learner.py
+-rw-r--r--   0 maaritamm   (501) staff       (20)      529 2024-01-10 14:30:32.000000 hastexo-xblock-7.9.1/hastexo/migrations/0012_add_suspend_by.py
+-rw-r--r--   0 maaritamm   (501) staff       (20)        0 2024-01-10 14:30:32.000000 hastexo-xblock-7.9.1/hastexo/migrations/__init__.py
+drwxr-xr-x   0 maaritamm   (501) staff       (20)        0 2024-02-14 14:44:41.085290 hastexo-xblock-7.9.1/hastexo/migrations/__pycache__/
+-rw-r--r--   0 maaritamm   (501) staff       (20)     1369 2024-01-10 14:32:28.000000 hastexo-xblock-7.9.1/hastexo/migrations/__pycache__/0001_initial.cpython-38.pyc
+-rw-r--r--   0 maaritamm   (501) staff       (20)     1444 2024-01-10 14:32:28.000000 hastexo-xblock-7.9.1/hastexo/migrations/__pycache__/0002_stacklog.cpython-38.pyc
+-rw-r--r--   0 maaritamm   (501) staff       (20)     1225 2024-01-10 14:32:28.000000 hastexo-xblock-7.9.1/hastexo/migrations/__pycache__/0003_blanks.cpython-38.pyc
+-rw-r--r--   0 maaritamm   (501) staff       (20)      708 2024-01-10 14:32:28.000000 hastexo-xblock-7.9.1/hastexo/migrations/__pycache__/0004_auto_20190715_1053.cpython-38.pyc
+-rw-r--r--   0 maaritamm   (501) staff       (20)     1047 2024-01-10 14:32:28.000000 hastexo-xblock-7.9.1/hastexo/migrations/__pycache__/0005_auto_20190811_1555.cpython-38.pyc
+-rw-r--r--   0 maaritamm   (501) staff       (20)     1160 2024-01-10 14:32:28.000000 hastexo-xblock-7.9.1/hastexo/migrations/__pycache__/0006_auto_20200107_1332.cpython-38.pyc
+-rw-r--r--   0 maaritamm   (501) staff       (20)      853 2024-01-10 14:32:28.000000 hastexo-xblock-7.9.1/hastexo/migrations/__pycache__/0007_add_delete_by_and_delete_age.cpython-38.pyc
+-rw-r--r--   0 maaritamm   (501) staff       (20)      736 2024-01-10 14:32:28.000000 hastexo-xblock-7.9.1/hastexo/migrations/__pycache__/0008_add_database_defaults_for_stack_key_and_password.cpython-38.pyc
+-rw-r--r--   0 maaritamm   (501) staff       (20)      737 2024-01-10 14:32:28.000000 hastexo-xblock-7.9.1/hastexo/migrations/__pycache__/0009_add_null_true_for_key_and_password.cpython-38.pyc
+-rw-r--r--   0 maaritamm   (501) staff       (20)     1628 2024-01-10 14:32:28.000000 hastexo-xblock-7.9.1/hastexo/migrations/__pycache__/0010_add_user_foreign_key.cpython-38.pyc
+-rw-r--r--   0 maaritamm   (501) staff       (20)      802 2024-01-10 14:32:28.000000 hastexo-xblock-7.9.1/hastexo/migrations/__pycache__/0011_allow_null_for_learner.cpython-38.pyc
+-rw-r--r--   0 maaritamm   (501) staff       (20)      661 2024-01-10 14:32:28.000000 hastexo-xblock-7.9.1/hastexo/migrations/__pycache__/0012_add_suspend_by.cpython-38.pyc
+-rw-r--r--   0 maaritamm   (501) staff       (20)      171 2024-01-10 14:32:28.000000 hastexo-xblock-7.9.1/hastexo/migrations/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 maaritamm   (501) staff       (20)     3644 2024-01-10 14:30:32.000000 hastexo-xblock-7.9.1/hastexo/models.py
+-rw-r--r--   0 maaritamm   (501) staff       (20)     4614 2024-01-10 14:30:32.000000 hastexo-xblock-7.9.1/hastexo/openstack.py
+-rw-r--r--   0 maaritamm   (501) staff       (20)    29112 2024-01-10 14:30:32.000000 hastexo-xblock-7.9.1/hastexo/provider.py
+drwxr-xr-x   0 maaritamm   (501) staff       (20)        0 2024-02-14 14:44:41.027186 hastexo-xblock-7.9.1/hastexo/public/
+drwxr-xr-x   0 maaritamm   (501) staff       (20)        0 2024-02-14 14:44:41.086132 hastexo-xblock-7.9.1/hastexo/public/css/
+-rw-r--r--   0 maaritamm   (501) staff       (20)     3279 2024-01-10 14:30:32.000000 hastexo-xblock-7.9.1/hastexo/public/css/main.css
+drwxr-xr-x   0 maaritamm   (501) staff       (20)        0 2024-02-14 14:44:41.089290 hastexo-xblock-7.9.1/hastexo/public/js/
+-rw-r--r--   0 maaritamm   (501) staff       (20)     7621 2024-01-10 14:30:32.000000 hastexo-xblock-7.9.1/hastexo/public/js/client.js
+drwxr-xr-x   0 maaritamm   (501) staff       (20)        0 2024-02-14 14:44:41.095098 hastexo-xblock-7.9.1/hastexo/public/js/guacamole-common-js/
+-rw-r--r--   0 maaritamm   (501) staff       (20)    67952 2024-01-10 14:30:32.000000 hastexo-xblock-7.9.1/hastexo/public/js/guacamole-common-js/0.9.13-incubating-all.min.js
+-rw-r--r--   0 maaritamm   (501) staff       (20)    70401 2024-01-10 14:30:32.000000 hastexo-xblock-7.9.1/hastexo/public/js/guacamole-common-js/1.4.0-all.min.js
+-rw-r--r--   0 maaritamm   (501) staff       (20)    72449 2024-01-11 10:58:49.000000 hastexo-xblock-7.9.1/hastexo/public/js/guacamole-common-js/1.5.2-all.min.js
+-rw-r--r--   0 maaritamm   (501) staff       (20)    72461 2024-01-11 14:25:10.000000 hastexo-xblock-7.9.1/hastexo/public/js/guacamole-common-js/1.5.4-all.min.js
+-rw-r--r--   0 maaritamm   (501) staff       (20)    18617 2024-02-12 15:52:21.000000 hastexo-xblock-7.9.1/hastexo/public/js/main.js
+-rw-r--r--   0 maaritamm   (501) staff       (20)     2344 2024-01-10 14:30:32.000000 hastexo-xblock-7.9.1/hastexo/public/js/plugins.js
+drwxr-xr-x   0 maaritamm   (501) staff       (20)        0 2024-02-14 14:44:41.028848 hastexo-xblock-7.9.1/hastexo/public/js/translations/
+drwxr-xr-x   0 maaritamm   (501) staff       (20)        0 2024-02-14 14:44:41.096956 hastexo-xblock-7.9.1/hastexo/public/js/translations/de-de/
+-rw-r--r--   0 maaritamm   (501) staff       (20)     7160 2024-01-10 14:30:32.000000 hastexo-xblock-7.9.1/hastexo/public/js/translations/de-de/text.js
+drwxr-xr-x   0 maaritamm   (501) staff       (20)        0 2024-02-14 14:44:41.097897 hastexo-xblock-7.9.1/hastexo/public/js/translations/el/
+-rw-r--r--   0 maaritamm   (501) staff       (20)    14190 2024-01-10 14:30:32.000000 hastexo-xblock-7.9.1/hastexo/public/js/translations/el/text.js
+drwxr-xr-x   0 maaritamm   (501) staff       (20)        0 2024-02-14 14:44:41.098871 hastexo-xblock-7.9.1/hastexo/public/js/translations/es-419/
+-rw-r--r--   0 maaritamm   (501) staff       (20)     6916 2024-01-10 14:30:32.000000 hastexo-xblock-7.9.1/hastexo/public/js/translations/es-419/text.js
+drwxr-xr-x   0 maaritamm   (501) staff       (20)        0 2024-02-14 14:44:41.099572 hastexo-xblock-7.9.1/hastexo/public/js/translations/et-ee/
+-rw-r--r--   0 maaritamm   (501) staff       (20)     7131 2024-01-10 14:30:32.000000 hastexo-xblock-7.9.1/hastexo/public/js/translations/et-ee/text.js
+drwxr-xr-x   0 maaritamm   (501) staff       (20)        0 2024-02-14 14:44:41.100352 hastexo-xblock-7.9.1/hastexo/public/js/translations/hi/
+-rw-r--r--   0 maaritamm   (501) staff       (20)    12785 2024-01-10 14:30:32.000000 hastexo-xblock-7.9.1/hastexo/public/js/translations/hi/text.js
+drwxr-xr-x   0 maaritamm   (501) staff       (20)        0 2024-02-14 14:44:41.029396 hastexo-xblock-7.9.1/hastexo/static/
+drwxr-xr-x   0 maaritamm   (501) staff       (20)        0 2024-02-14 14:44:41.102128 hastexo-xblock-7.9.1/hastexo/static/html/
+-rw-r--r--   0 maaritamm   (501) staff       (20)     3111 2024-02-13 07:04:24.000000 hastexo-xblock-7.9.1/hastexo/static/html/lab.html
+-rw-r--r--   0 maaritamm   (501) staff       (20)     3445 2024-01-10 14:30:32.000000 hastexo-xblock-7.9.1/hastexo/static/html/main.html
+-rw-r--r--   0 maaritamm   (501) staff       (20)    34877 2024-01-10 14:30:32.000000 hastexo-xblock-7.9.1/hastexo/tasks.py
+drwxr-xr-x   0 maaritamm   (501) staff       (20)        0 2024-02-14 14:44:41.033294 hastexo-xblock-7.9.1/hastexo/translations/
+drwxr-xr-x   0 maaritamm   (501) staff       (20)        0 2024-02-14 14:44:41.030305 hastexo-xblock-7.9.1/hastexo/translations/de_DE/
+drwxr-xr-x   0 maaritamm   (501) staff       (20)        0 2024-02-14 14:44:41.103769 hastexo-xblock-7.9.1/hastexo/translations/de_DE/LC_MESSAGES/
+-rw-r--r--   0 maaritamm   (501) staff       (20)     4125 2024-01-10 14:30:32.000000 hastexo-xblock-7.9.1/hastexo/translations/de_DE/LC_MESSAGES/text.mo
+-rw-r--r--   0 maaritamm   (501) staff       (20)     5146 2024-01-10 14:30:32.000000 hastexo-xblock-7.9.1/hastexo/translations/de_DE/LC_MESSAGES/text.po
+drwxr-xr-x   0 maaritamm   (501) staff       (20)        0 2024-02-14 14:44:41.030920 hastexo-xblock-7.9.1/hastexo/translations/el/
+drwxr-xr-x   0 maaritamm   (501) staff       (20)        0 2024-02-14 14:44:41.105522 hastexo-xblock-7.9.1/hastexo/translations/el/LC_MESSAGES/
+-rw-r--r--   0 maaritamm   (501) staff       (20)     5594 2024-01-10 14:30:32.000000 hastexo-xblock-7.9.1/hastexo/translations/el/LC_MESSAGES/text.mo
+-rw-r--r--   0 maaritamm   (501) staff       (20)     6657 2024-01-10 14:30:32.000000 hastexo-xblock-7.9.1/hastexo/translations/el/LC_MESSAGES/text.po
+drwxr-xr-x   0 maaritamm   (501) staff       (20)        0 2024-02-14 14:44:41.031561 hastexo-xblock-7.9.1/hastexo/translations/en/
+drwxr-xr-x   0 maaritamm   (501) staff       (20)        0 2024-02-14 14:44:41.107482 hastexo-xblock-7.9.1/hastexo/translations/en/LC_MESSAGES/
+-rw-r--r--   0 maaritamm   (501) staff       (20)      380 2024-01-10 14:30:32.000000 hastexo-xblock-7.9.1/hastexo/translations/en/LC_MESSAGES/text.mo
+-rw-r--r--   0 maaritamm   (501) staff       (20)     3512 2024-01-10 14:30:32.000000 hastexo-xblock-7.9.1/hastexo/translations/en/LC_MESSAGES/text.po
+drwxr-xr-x   0 maaritamm   (501) staff       (20)        0 2024-02-14 14:44:41.032170 hastexo-xblock-7.9.1/hastexo/translations/es_419/
+drwxr-xr-x   0 maaritamm   (501) staff       (20)        0 2024-02-14 14:44:41.109181 hastexo-xblock-7.9.1/hastexo/translations/es_419/LC_MESSAGES/
+-rw-r--r--   0 maaritamm   (501) staff       (20)     4101 2024-01-10 14:30:32.000000 hastexo-xblock-7.9.1/hastexo/translations/es_419/LC_MESSAGES/text.mo
+-rw-r--r--   0 maaritamm   (501) staff       (20)     5122 2024-01-10 14:30:32.000000 hastexo-xblock-7.9.1/hastexo/translations/es_419/LC_MESSAGES/text.po
+drwxr-xr-x   0 maaritamm   (501) staff       (20)        0 2024-02-14 14:44:41.032826 hastexo-xblock-7.9.1/hastexo/translations/et_EE/
+drwxr-xr-x   0 maaritamm   (501) staff       (20)        0 2024-02-14 14:44:41.111374 hastexo-xblock-7.9.1/hastexo/translations/et_EE/LC_MESSAGES/
+-rw-r--r--   0 maaritamm   (501) staff       (20)     3926 2024-01-10 14:30:32.000000 hastexo-xblock-7.9.1/hastexo/translations/et_EE/LC_MESSAGES/text.mo
+-rw-r--r--   0 maaritamm   (501) staff       (20)     4950 2024-01-10 14:30:32.000000 hastexo-xblock-7.9.1/hastexo/translations/et_EE/LC_MESSAGES/text.po
+drwxr-xr-x   0 maaritamm   (501) staff       (20)        0 2024-02-14 14:44:41.033553 hastexo-xblock-7.9.1/hastexo/translations/hi/
+drwxr-xr-x   0 maaritamm   (501) staff       (20)        0 2024-02-14 14:44:41.114483 hastexo-xblock-7.9.1/hastexo/translations/hi/LC_MESSAGES/
+-rw-r--r--   0 maaritamm   (501) staff       (20)     6255 2024-01-10 14:30:32.000000 hastexo-xblock-7.9.1/hastexo/translations/hi/LC_MESSAGES/text.mo
+-rw-r--r--   0 maaritamm   (501) staff       (20)     7294 2024-01-10 14:30:32.000000 hastexo-xblock-7.9.1/hastexo/translations/hi/LC_MESSAGES/text.po
+drwxr-xr-x   0 maaritamm   (501) staff       (20)        0 2024-02-14 14:44:41.118155 hastexo-xblock-7.9.1/hastexo_guacamole_client/
+-rw-r--r--   0 maaritamm   (501) staff       (20)        0 2024-01-10 14:30:32.000000 hastexo-xblock-7.9.1/hastexo_guacamole_client/__init__.py
+-rw-r--r--   0 maaritamm   (501) staff       (20)      896 2024-01-10 14:30:32.000000 hastexo-xblock-7.9.1/hastexo_guacamole_client/asgi.py
+-rw-r--r--   0 maaritamm   (501) staff       (20)     3347 2024-01-10 14:30:32.000000 hastexo-xblock-7.9.1/hastexo_guacamole_client/consumers.py
+-rw-r--r--   0 maaritamm   (501) staff       (20)     2742 2024-01-10 14:30:32.000000 hastexo-xblock-7.9.1/hastexo_guacamole_client/settings.py
+drwxr-xr-x   0 maaritamm   (501) staff       (20)        0 2024-02-14 14:44:41.122088 hastexo-xblock-7.9.1/hastexo_xblock.egg-info/
+-rw-r--r--   0 maaritamm   (501) staff       (20)    30919 2024-02-14 14:44:40.000000 hastexo-xblock-7.9.1/hastexo_xblock.egg-info/PKG-INFO
+-rw-r--r--   0 maaritamm   (501) staff       (20)     4988 2024-02-14 14:44:40.000000 hastexo-xblock-7.9.1/hastexo_xblock.egg-info/SOURCES.txt
+-rw-r--r--   0 maaritamm   (501) staff       (20)        1 2024-02-14 14:44:40.000000 hastexo-xblock-7.9.1/hastexo_xblock.egg-info/dependency_links.txt
+-rw-r--r--   0 maaritamm   (501) staff       (20)       52 2024-02-14 14:44:40.000000 hastexo-xblock-7.9.1/hastexo_xblock.egg-info/entry_points.txt
+-rw-r--r--   0 maaritamm   (501) staff       (20)      138 2024-02-14 14:44:40.000000 hastexo-xblock-7.9.1/hastexo_xblock.egg-info/requires.txt
+-rw-r--r--   0 maaritamm   (501) staff       (20)        8 2024-02-14 14:44:40.000000 hastexo-xblock-7.9.1/hastexo_xblock.egg-info/top_level.txt
+drwxr-xr-x   0 maaritamm   (501) staff       (20)        0 2024-02-14 14:44:41.125161 hastexo-xblock-7.9.1/requirements/
+-rw-r--r--   0 maaritamm   (501) staff       (20)      690 2024-01-11 14:25:10.000000 hastexo-xblock-7.9.1/requirements/base.txt
+-rw-r--r--   0 maaritamm   (501) staff       (20)        7 2024-01-10 14:30:32.000000 hastexo-xblock-7.9.1/requirements/flake8.txt
+-rw-r--r--   0 maaritamm   (501) staff       (20)       41 2024-01-10 14:30:32.000000 hastexo-xblock-7.9.1/requirements/setup.txt
+-rw-r--r--   0 maaritamm   (501) staff       (20)      359 2024-01-10 14:30:32.000000 hastexo-xblock-7.9.1/requirements/test.txt
+-rw-r--r--   0 maaritamm   (501) staff       (20)      690 2024-01-11 14:25:10.000000 hastexo-xblock-7.9.1/requirements.txt
+-rwxr-xr-x   0 maaritamm   (501) staff       (20)     2000 2024-01-10 14:30:32.000000 hastexo-xblock-7.9.1/run_tests.py
+drwxr-xr-x   0 maaritamm   (501) staff       (20)        0 2024-02-14 14:44:41.035366 hastexo-xblock-7.9.1/samples/
+drwxr-xr-x   0 maaritamm   (501) staff       (20)        0 2024-02-14 14:44:41.125900 hastexo-xblock-7.9.1/samples/gcloud/
+-rw-r--r--   0 maaritamm   (501) staff       (20)     2198 2024-01-10 14:30:32.000000 hastexo-xblock-7.9.1/samples/gcloud/sample-template.yaml.jinja
+drwxr-xr-x   0 maaritamm   (501) staff       (20)        0 2024-02-14 14:44:41.126874 hastexo-xblock-7.9.1/samples/hot/
+-rw-r--r--   0 maaritamm   (501) staff       (20)    13209 2024-01-10 14:30:32.000000 hastexo-xblock-7.9.1/samples/hot/sample-template.yaml
+-rw-r--r--   0 maaritamm   (501) staff       (20)       38 2024-02-14 14:44:41.144551 hastexo-xblock-7.9.1/setup.cfg
+-rwxr-xr-x   0 maaritamm   (501) staff       (20)     2372 2024-01-10 14:30:32.000000 hastexo-xblock-7.9.1/setup.py
+drwxr-xr-x   0 maaritamm   (501) staff       (20)        0 2024-02-14 14:44:41.128117 hastexo-xblock-7.9.1/src/
+-rw-r--r--   0 maaritamm   (501) staff       (20)      185 2024-01-10 14:30:32.000000 hastexo-xblock-7.9.1/src/pip-delete-this-directory.txt
+drwxr-xr-x   0 maaritamm   (501) staff       (20)        0 2024-02-14 14:44:41.128832 hastexo-xblock-7.9.1/tests/
+-rw-r--r--   0 maaritamm   (501) staff       (20)        0 2024-01-10 14:30:32.000000 hastexo-xblock-7.9.1/tests/__init__.py
+drwxr-xr-x   0 maaritamm   (501) staff       (20)        0 2024-02-14 14:44:41.036491 hastexo-xblock-7.9.1/tests/resources/
+drwxr-xr-x   0 maaritamm   (501) staff       (20)        0 2024-02-14 14:44:41.036677 hastexo-xblock-7.9.1/tests/resources/course/
+drwxr-xr-x   0 maaritamm   (501) staff       (20)        0 2024-02-14 14:44:41.135448 hastexo-xblock-7.9.1/tests/resources/course/hastexo/
+-rw-r--r--   0 maaritamm   (501) staff       (20)      488 2024-01-10 14:30:32.000000 hastexo-xblock-7.9.1/tests/resources/course/hastexo/fake_lab_1.xml
+-rw-r--r--   0 maaritamm   (501) staff       (20)      346 2024-01-10 14:30:32.000000 hastexo-xblock-7.9.1/tests/resources/course/hastexo/fake_lab_2.xml
+-rw-r--r--   0 maaritamm   (501) staff       (20)       67 2024-01-10 14:30:32.000000 hastexo-xblock-7.9.1/tests/resources/course/hastexo/fake_lab_hook_events_1.xml
+-rw-r--r--   0 maaritamm   (501) staff       (20)       69 2024-01-10 14:30:32.000000 hastexo-xblock-7.9.1/tests/resources/course/hastexo/fake_lab_hook_events_2.xml
+-rw-r--r--   0 maaritamm   (501) staff       (20)       45 2024-01-10 14:30:32.000000 hastexo-xblock-7.9.1/tests/resources/course/hastexo/fake_lab_no_port_name.xml
+-rw-r--r--   0 maaritamm   (501) staff       (20)       46 2024-01-10 14:30:32.000000 hastexo-xblock-7.9.1/tests/resources/course/hastexo/fake_lab_no_port_number.xml
+-rw-r--r--   0 maaritamm   (501) staff       (20)      301 2024-01-10 14:30:32.000000 hastexo-xblock-7.9.1/tests/resources/course/hastexo/fake_lab_no_provider_capacity.xml
+-rw-r--r--   0 maaritamm   (501) staff       (20)      101 2024-01-10 14:30:32.000000 hastexo-xblock-7.9.1/tests/resources/course/hastexo/fake_lab_no_provider_name.xml
+drwxr-xr-x   0 maaritamm   (501) staff       (20)        0 2024-02-14 14:44:41.142408 hastexo-xblock-7.9.1/tests/unit/
+-rw-r--r--   0 maaritamm   (501) staff       (20)        0 2024-01-10 14:30:32.000000 hastexo-xblock-7.9.1/tests/unit/__init__.py
+-rw-r--r--   0 maaritamm   (501) staff       (20)     5947 2024-01-10 14:30:32.000000 hastexo-xblock-7.9.1/tests/unit/test_admin.py
+-rw-r--r--   0 maaritamm   (501) staff       (20)      976 2024-01-10 14:30:32.000000 hastexo-xblock-7.9.1/tests/unit/test_commands.py
+-rw-r--r--   0 maaritamm   (501) staff       (20)     9618 2024-01-10 14:30:32.000000 hastexo-xblock-7.9.1/tests/unit/test_common.py
+-rw-r--r--   0 maaritamm   (501) staff       (20)     5062 2024-01-10 14:30:32.000000 hastexo-xblock-7.9.1/tests/unit/test_gcloud.py
+-rw-r--r--   0 maaritamm   (501) staff       (20)    63482 2024-02-14 12:09:36.000000 hastexo-xblock-7.9.1/tests/unit/test_hastexo.py
+-rw-r--r--   0 maaritamm   (501) staff       (20)    21787 2024-01-10 14:30:32.000000 hastexo-xblock-7.9.1/tests/unit/test_jobs.py
+-rw-r--r--   0 maaritamm   (501) staff       (20)     2623 2024-01-10 14:30:32.000000 hastexo-xblock-7.9.1/tests/unit/test_models.py
+-rw-r--r--   0 maaritamm   (501) staff       (20)     6648 2024-01-10 14:30:32.000000 hastexo-xblock-7.9.1/tests/unit/test_openstack.py
+-rw-r--r--   0 maaritamm   (501) staff       (20)    71703 2024-01-10 14:30:32.000000 hastexo-xblock-7.9.1/tests/unit/test_provider.py
+-rw-r--r--   0 maaritamm   (501) staff       (20)    71832 2024-01-10 14:30:32.000000 hastexo-xblock-7.9.1/tests/unit/test_tasks.py
+-rw-r--r--   0 maaritamm   (501) staff       (20)     1516 2024-01-10 14:30:32.000000 hastexo-xblock-7.9.1/tox.ini
```

### Comparing `hastexo-xblock-7.9.0/.github/workflows/tox.yml` & `hastexo-xblock-7.9.1/.github/workflows/tox.yml`

 * *Files identical despite different names*

### Comparing `hastexo-xblock-7.9.0/.gitlab-ci.yml` & `hastexo-xblock-7.9.1/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `hastexo-xblock-7.9.0/Changelog.md` & `hastexo-xblock-7.9.1/Changelog.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+Version 7.9.1 (2024-02-14)
+-------------------------
+* [Bug fix] Don't allow accessing a fullscreen lab directly from a URL,
+  when the user is unauthenticated. Return a 401 right away when attempted.
+
 Version 7.9.0 (2024-01-11)
 -------------------------
 * [Enhancement] Add support for Apache Guacamole 1.5.4;
   make it the new default version.
 * [Enhancement] Update requirements for Open edX Quince release.
 
 Version 7.8.1 (2023-12-18)
```

### Comparing `hastexo-xblock-7.9.0/HACKING.md` & `hastexo-xblock-7.9.1/HACKING.md`

 * *Files identical despite different names*

### Comparing `hastexo-xblock-7.9.0/LICENSE` & `hastexo-xblock-7.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hastexo-xblock-7.9.0/PKG-INFO` & `hastexo-xblock-7.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hastexo-xblock
-Version: 7.9.0
+Version: 7.9.1
 Summary: hastexo XBlock: Makes arbitrarily complex lab environments available on an Open edX LMS
 Home-page: https://github.com/hastexo/hastexo-xblock
 Author: hastexo
 Author-email: pypi@hastexo.com
 License: AGPL-3.0
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
@@ -82,15 +82,15 @@
 Running this XBlock with Tutor (for Open edX Maple and later) requires
 two steps:
 
 1. Install the XBlock to your Tutor environment by adding it to the
    `OPENEDX_EXTRA_PIP_REQUIREMENTS` list in `config.yml`:
    ```
    OPENEDX_EXTRA_PIP_REQUIREMENTS:
-     - "hastexo-xblock==7.9.0"
+     - "hastexo-xblock==7.9.1"
    ```
    For additional information, please refer to the [official
    documentation](https://docs.tutor.overhang.io/configuration.html#installing-extra-xblocks-and-requirements).
 
 
 2. Install and enable the `tutor-contrib-hastexo` plugin:
    ```
```

### Comparing `hastexo-xblock-7.9.0/README.md` & `hastexo-xblock-7.9.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -62,15 +62,15 @@
 Running this XBlock with Tutor (for Open edX Maple and later) requires
 two steps:
 
 1. Install the XBlock to your Tutor environment by adding it to the
    `OPENEDX_EXTRA_PIP_REQUIREMENTS` list in `config.yml`:
    ```
    OPENEDX_EXTRA_PIP_REQUIREMENTS:
-     - "hastexo-xblock==7.9.0"
+     - "hastexo-xblock==7.9.1"
    ```
    For additional information, please refer to the [official
    documentation](https://docs.tutor.overhang.io/configuration.html#installing-extra-xblocks-and-requirements).
 
 
 2. Install and enable the `tutor-contrib-hastexo` plugin:
    ```
```

### Comparing `hastexo-xblock-7.9.0/hastexo/admin.py` & `hastexo-xblock-7.9.1/hastexo/admin.py`

 * *Files identical despite different names*

### Comparing `hastexo-xblock-7.9.0/hastexo/common.py` & `hastexo-xblock-7.9.1/hastexo/common.py`

 * *Files identical despite different names*

### Comparing `hastexo-xblock-7.9.0/hastexo/gcloud.py` & `hastexo-xblock-7.9.1/hastexo/gcloud.py`

 * *Files identical despite different names*

### Comparing `hastexo-xblock-7.9.0/hastexo/hastexo.py` & `hastexo-xblock-7.9.1/hastexo/hastexo.py`

 * *Files 1% similar despite different names*

```diff
@@ -654,14 +654,17 @@
         return context
 
     @XBlock.handler
     def launch_new_window(self, request, suffix=''):
         """
         The fullscreen lab view, opened in a new browser window.
         """
+        if 'sessionid' not in request.cookies:
+            return Response(status=401, body="Unauthorized")
+
         # Get context
         context = self.get_context()
 
         # Pass the token (for keepalives)
         context["csrftoken"] = request.cookies.get('csrftoken')
 
         # Get the JavaScript urls
```

### Comparing `hastexo-xblock-7.9.0/hastexo/jobs.py` & `hastexo-xblock-7.9.1/hastexo/jobs.py`

 * *Files identical despite different names*

### Comparing `hastexo-xblock-7.9.0/hastexo/locale/en/LC_MESSAGES/django-partial.po` & `hastexo-xblock-7.9.1/hastexo/locale/en/LC_MESSAGES/django-partial.po`

 * *Files identical despite different names*

### Comparing `hastexo-xblock-7.9.0/hastexo/management/commands/__pycache__/reaper.cpython-38.pyc` & `hastexo-xblock-7.9.1/hastexo/management/commands/__pycache__/reaper.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `hastexo-xblock-7.9.0/hastexo/management/commands/__pycache__/suspender.cpython-38.pyc` & `hastexo-xblock-7.9.1/hastexo/management/commands/__pycache__/suspender.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `hastexo-xblock-7.9.0/hastexo/management/commands/reaper.py` & `hastexo-xblock-7.9.1/hastexo/management/commands/reaper.py`

 * *Files identical despite different names*

### Comparing `hastexo-xblock-7.9.0/hastexo/management/commands/suspender.py` & `hastexo-xblock-7.9.1/hastexo/management/commands/suspender.py`

 * *Files identical despite different names*

### Comparing `hastexo-xblock-7.9.0/hastexo/migrations/0001_initial.py` & `hastexo-xblock-7.9.1/hastexo/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `hastexo-xblock-7.9.0/hastexo/migrations/0002_stacklog.py` & `hastexo-xblock-7.9.1/hastexo/migrations/0002_stacklog.py`

 * *Files identical despite different names*

### Comparing `hastexo-xblock-7.9.0/hastexo/migrations/0003_blanks.py` & `hastexo-xblock-7.9.1/hastexo/migrations/0003_blanks.py`

 * *Files identical despite different names*

### Comparing `hastexo-xblock-7.9.0/hastexo/migrations/0004_auto_20190715_1053.py` & `hastexo-xblock-7.9.1/hastexo/migrations/0004_auto_20190715_1053.py`

 * *Files identical despite different names*

### Comparing `hastexo-xblock-7.9.0/hastexo/migrations/0005_auto_20190811_1555.py` & `hastexo-xblock-7.9.1/hastexo/migrations/0005_auto_20190811_1555.py`

 * *Files identical despite different names*

### Comparing `hastexo-xblock-7.9.0/hastexo/migrations/0006_auto_20200107_1332.py` & `hastexo-xblock-7.9.1/hastexo/migrations/0006_auto_20200107_1332.py`

 * *Files identical despite different names*

### Comparing `hastexo-xblock-7.9.0/hastexo/migrations/0007_add_delete_by_and_delete_age.py` & `hastexo-xblock-7.9.1/hastexo/migrations/0007_add_delete_by_and_delete_age.py`

 * *Files identical despite different names*

### Comparing `hastexo-xblock-7.9.0/hastexo/migrations/0008_add_database_defaults_for_stack_key_and_password.py` & `hastexo-xblock-7.9.1/hastexo/migrations/0008_add_database_defaults_for_stack_key_and_password.py`

 * *Files identical despite different names*

### Comparing `hastexo-xblock-7.9.0/hastexo/migrations/0009_add_null_true_for_key_and_password.py` & `hastexo-xblock-7.9.1/hastexo/migrations/0009_add_null_true_for_key_and_password.py`

 * *Files identical despite different names*

### Comparing `hastexo-xblock-7.9.0/hastexo/migrations/0010_add_user_foreign_key.py` & `hastexo-xblock-7.9.1/hastexo/migrations/0010_add_user_foreign_key.py`

 * *Files identical despite different names*

### Comparing `hastexo-xblock-7.9.0/hastexo/migrations/0011_allow_null_for_learner.py` & `hastexo-xblock-7.9.1/hastexo/migrations/0011_allow_null_for_learner.py`

 * *Files identical despite different names*

### Comparing `hastexo-xblock-7.9.0/hastexo/migrations/0012_add_suspend_by.py` & `hastexo-xblock-7.9.1/hastexo/migrations/0012_add_suspend_by.py`

 * *Files identical despite different names*

### Comparing `hastexo-xblock-7.9.0/hastexo/migrations/__pycache__/0001_initial.cpython-38.pyc` & `hastexo-xblock-7.9.1/hastexo/migrations/__pycache__/0001_initial.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `hastexo-xblock-7.9.0/hastexo/migrations/__pycache__/0002_stacklog.cpython-38.pyc` & `hastexo-xblock-7.9.1/hastexo/migrations/__pycache__/0002_stacklog.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `hastexo-xblock-7.9.0/hastexo/migrations/__pycache__/0003_blanks.cpython-38.pyc` & `hastexo-xblock-7.9.1/hastexo/migrations/__pycache__/0003_blanks.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `hastexo-xblock-7.9.0/hastexo/migrations/__pycache__/0004_auto_20190715_1053.cpython-38.pyc` & `hastexo-xblock-7.9.1/hastexo/migrations/__pycache__/0004_auto_20190715_1053.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `hastexo-xblock-7.9.0/hastexo/migrations/__pycache__/0005_auto_20190811_1555.cpython-38.pyc` & `hastexo-xblock-7.9.1/hastexo/migrations/__pycache__/0005_auto_20190811_1555.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `hastexo-xblock-7.9.0/hastexo/migrations/__pycache__/0006_auto_20200107_1332.cpython-38.pyc` & `hastexo-xblock-7.9.1/hastexo/migrations/__pycache__/0006_auto_20200107_1332.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `hastexo-xblock-7.9.0/hastexo/migrations/__pycache__/0007_add_delete_by_and_delete_age.cpython-38.pyc` & `hastexo-xblock-7.9.1/hastexo/migrations/__pycache__/0007_add_delete_by_and_delete_age.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `hastexo-xblock-7.9.0/hastexo/migrations/__pycache__/0008_add_database_defaults_for_stack_key_and_password.cpython-38.pyc` & `hastexo-xblock-7.9.1/hastexo/migrations/__pycache__/0008_add_database_defaults_for_stack_key_and_password.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `hastexo-xblock-7.9.0/hastexo/migrations/__pycache__/0009_add_null_true_for_key_and_password.cpython-38.pyc` & `hastexo-xblock-7.9.1/hastexo/migrations/__pycache__/0009_add_null_true_for_key_and_password.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `hastexo-xblock-7.9.0/hastexo/migrations/__pycache__/0010_add_user_foreign_key.cpython-38.pyc` & `hastexo-xblock-7.9.1/hastexo/migrations/__pycache__/0010_add_user_foreign_key.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `hastexo-xblock-7.9.0/hastexo/migrations/__pycache__/0011_allow_null_for_learner.cpython-38.pyc` & `hastexo-xblock-7.9.1/hastexo/migrations/__pycache__/0011_allow_null_for_learner.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `hastexo-xblock-7.9.0/hastexo/migrations/__pycache__/0012_add_suspend_by.cpython-38.pyc` & `hastexo-xblock-7.9.1/hastexo/migrations/__pycache__/0012_add_suspend_by.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `hastexo-xblock-7.9.0/hastexo/models.py` & `hastexo-xblock-7.9.1/hastexo/models.py`

 * *Files identical despite different names*

### Comparing `hastexo-xblock-7.9.0/hastexo/openstack.py` & `hastexo-xblock-7.9.1/hastexo/openstack.py`

 * *Files identical despite different names*

### Comparing `hastexo-xblock-7.9.0/hastexo/provider.py` & `hastexo-xblock-7.9.1/hastexo/provider.py`

 * *Files identical despite different names*

### Comparing `hastexo-xblock-7.9.0/hastexo/public/css/main.css` & `hastexo-xblock-7.9.1/hastexo/public/css/main.css`

 * *Files identical despite different names*

### Comparing `hastexo-xblock-7.9.0/hastexo/public/js/client.js` & `hastexo-xblock-7.9.1/hastexo/public/js/client.js`

 * *Files identical despite different names*

### Comparing `hastexo-xblock-7.9.0/hastexo/public/js/guacamole-common-js/0.9.13-incubating-all.min.js` & `hastexo-xblock-7.9.1/hastexo/public/js/guacamole-common-js/0.9.13-incubating-all.min.js`

 * *Files identical despite different names*

### Comparing `hastexo-xblock-7.9.0/hastexo/public/js/guacamole-common-js/1.4.0-all.min.js` & `hastexo-xblock-7.9.1/hastexo/public/js/guacamole-common-js/1.4.0-all.min.js`

 * *Files identical despite different names*

### Comparing `hastexo-xblock-7.9.0/hastexo/public/js/guacamole-common-js/1.5.2-all.min.js` & `hastexo-xblock-7.9.1/hastexo/public/js/guacamole-common-js/1.5.2-all.min.js`

 * *Files identical despite different names*

### Comparing `hastexo-xblock-7.9.0/hastexo/public/js/guacamole-common-js/1.5.4-all.min.js` & `hastexo-xblock-7.9.1/hastexo/public/js/guacamole-common-js/1.5.4-all.min.js`

 * *Files identical despite different names*

### Comparing `hastexo-xblock-7.9.0/hastexo/public/js/main.js` & `hastexo-xblock-7.9.1/hastexo/public/js/main.js`

 * *Files identical despite different names*

### Comparing `hastexo-xblock-7.9.0/hastexo/public/js/plugins.js` & `hastexo-xblock-7.9.1/hastexo/public/js/plugins.js`

 * *Files identical despite different names*

### Comparing `hastexo-xblock-7.9.0/hastexo/public/js/translations/de-de/text.js` & `hastexo-xblock-7.9.1/hastexo/public/js/translations/de-de/text.js`

 * *Files identical despite different names*

### Comparing `hastexo-xblock-7.9.0/hastexo/public/js/translations/el/text.js` & `hastexo-xblock-7.9.1/hastexo/public/js/translations/el/text.js`

 * *Files identical despite different names*

### Comparing `hastexo-xblock-7.9.0/hastexo/public/js/translations/es-419/text.js` & `hastexo-xblock-7.9.1/hastexo/public/js/translations/es-419/text.js`

 * *Files identical despite different names*

### Comparing `hastexo-xblock-7.9.0/hastexo/public/js/translations/et-ee/text.js` & `hastexo-xblock-7.9.1/hastexo/public/js/translations/et-ee/text.js`

 * *Files identical despite different names*

### Comparing `hastexo-xblock-7.9.0/hastexo/public/js/translations/hi/text.js` & `hastexo-xblock-7.9.1/hastexo/public/js/translations/hi/text.js`

 * *Files identical despite different names*

### Comparing `hastexo-xblock-7.9.0/hastexo/static/html/lab.html` & `hastexo-xblock-7.9.1/hastexo/static/html/lab.html`

 * *Files identical despite different names*

### Comparing `hastexo-xblock-7.9.0/hastexo/static/html/main.html` & `hastexo-xblock-7.9.1/hastexo/static/html/main.html`

 * *Files identical despite different names*

### Comparing `hastexo-xblock-7.9.0/hastexo/tasks.py` & `hastexo-xblock-7.9.1/hastexo/tasks.py`

 * *Files identical despite different names*

### Comparing `hastexo-xblock-7.9.0/hastexo/translations/de_DE/LC_MESSAGES/text.mo` & `hastexo-xblock-7.9.1/hastexo/translations/de_DE/LC_MESSAGES/text.mo`

 * *Files identical despite different names*

### Comparing `hastexo-xblock-7.9.0/hastexo/translations/de_DE/LC_MESSAGES/text.po` & `hastexo-xblock-7.9.1/hastexo/translations/de_DE/LC_MESSAGES/text.po`

 * *Files identical despite different names*

### Comparing `hastexo-xblock-7.9.0/hastexo/translations/el/LC_MESSAGES/text.mo` & `hastexo-xblock-7.9.1/hastexo/translations/el/LC_MESSAGES/text.mo`

 * *Files identical despite different names*

### Comparing `hastexo-xblock-7.9.0/hastexo/translations/el/LC_MESSAGES/text.po` & `hastexo-xblock-7.9.1/hastexo/translations/el/LC_MESSAGES/text.po`

 * *Files identical despite different names*

### Comparing `hastexo-xblock-7.9.0/hastexo/translations/en/LC_MESSAGES/text.po` & `hastexo-xblock-7.9.1/hastexo/translations/en/LC_MESSAGES/text.po`

 * *Files identical despite different names*

### Comparing `hastexo-xblock-7.9.0/hastexo/translations/es_419/LC_MESSAGES/text.mo` & `hastexo-xblock-7.9.1/hastexo/translations/es_419/LC_MESSAGES/text.mo`

 * *Files identical despite different names*

### Comparing `hastexo-xblock-7.9.0/hastexo/translations/es_419/LC_MESSAGES/text.po` & `hastexo-xblock-7.9.1/hastexo/translations/es_419/LC_MESSAGES/text.po`

 * *Files identical despite different names*

### Comparing `hastexo-xblock-7.9.0/hastexo/translations/et_EE/LC_MESSAGES/text.mo` & `hastexo-xblock-7.9.1/hastexo/translations/et_EE/LC_MESSAGES/text.mo`

 * *Files identical despite different names*

### Comparing `hastexo-xblock-7.9.0/hastexo/translations/et_EE/LC_MESSAGES/text.po` & `hastexo-xblock-7.9.1/hastexo/translations/et_EE/LC_MESSAGES/text.po`

 * *Files identical despite different names*

### Comparing `hastexo-xblock-7.9.0/hastexo/translations/hi/LC_MESSAGES/text.mo` & `hastexo-xblock-7.9.1/hastexo/translations/hi/LC_MESSAGES/text.mo`

 * *Files identical despite different names*

### Comparing `hastexo-xblock-7.9.0/hastexo/translations/hi/LC_MESSAGES/text.po` & `hastexo-xblock-7.9.1/hastexo/translations/hi/LC_MESSAGES/text.po`

 * *Files identical despite different names*

### Comparing `hastexo-xblock-7.9.0/hastexo_guacamole_client/asgi.py` & `hastexo-xblock-7.9.1/hastexo_guacamole_client/asgi.py`

 * *Files identical despite different names*

### Comparing `hastexo-xblock-7.9.0/hastexo_guacamole_client/consumers.py` & `hastexo-xblock-7.9.1/hastexo_guacamole_client/consumers.py`

 * *Files identical despite different names*

### Comparing `hastexo-xblock-7.9.0/hastexo_guacamole_client/settings.py` & `hastexo-xblock-7.9.1/hastexo_guacamole_client/settings.py`

 * *Files identical despite different names*

### Comparing `hastexo-xblock-7.9.0/hastexo_xblock.egg-info/PKG-INFO` & `hastexo-xblock-7.9.1/hastexo_xblock.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hastexo-xblock
-Version: 7.9.0
+Version: 7.9.1
 Summary: hastexo XBlock: Makes arbitrarily complex lab environments available on an Open edX LMS
 Home-page: https://github.com/hastexo/hastexo-xblock
 Author: hastexo
 Author-email: pypi@hastexo.com
 License: AGPL-3.0
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
@@ -82,15 +82,15 @@
 Running this XBlock with Tutor (for Open edX Maple and later) requires
 two steps:
 
 1. Install the XBlock to your Tutor environment by adding it to the
    `OPENEDX_EXTRA_PIP_REQUIREMENTS` list in `config.yml`:
    ```
    OPENEDX_EXTRA_PIP_REQUIREMENTS:
-     - "hastexo-xblock==7.9.0"
+     - "hastexo-xblock==7.9.1"
    ```
    For additional information, please refer to the [official
    documentation](https://docs.tutor.overhang.io/configuration.html#installing-extra-xblocks-and-requirements).
 
 
 2. Install and enable the `tutor-contrib-hastexo` plugin:
    ```
```

### Comparing `hastexo-xblock-7.9.0/hastexo_xblock.egg-info/SOURCES.txt` & `hastexo-xblock-7.9.1/hastexo_xblock.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hastexo-xblock-7.9.0/requirements/base.txt` & `hastexo-xblock-7.9.1/requirements/base.txt`

 * *Files identical despite different names*

### Comparing `hastexo-xblock-7.9.0/requirements.txt` & `hastexo-xblock-7.9.1/requirements.txt`

 * *Files identical despite different names*

### Comparing `hastexo-xblock-7.9.0/run_tests.py` & `hastexo-xblock-7.9.1/run_tests.py`

 * *Files identical despite different names*

### Comparing `hastexo-xblock-7.9.0/samples/gcloud/sample-template.yaml.jinja` & `hastexo-xblock-7.9.1/samples/gcloud/sample-template.yaml.jinja`

 * *Files identical despite different names*

### Comparing `hastexo-xblock-7.9.0/samples/hot/sample-template.yaml` & `hastexo-xblock-7.9.1/samples/hot/sample-template.yaml`

 * *Files identical despite different names*

### Comparing `hastexo-xblock-7.9.0/setup.py` & `hastexo-xblock-7.9.1/setup.py`

 * *Files identical despite different names*

### Comparing `hastexo-xblock-7.9.0/tests/unit/test_admin.py` & `hastexo-xblock-7.9.1/tests/unit/test_admin.py`

 * *Files identical despite different names*

### Comparing `hastexo-xblock-7.9.0/tests/unit/test_commands.py` & `hastexo-xblock-7.9.1/tests/unit/test_commands.py`

 * *Files identical despite different names*

### Comparing `hastexo-xblock-7.9.0/tests/unit/test_common.py` & `hastexo-xblock-7.9.1/tests/unit/test_common.py`

 * *Files identical despite different names*

### Comparing `hastexo-xblock-7.9.0/tests/unit/test_gcloud.py` & `hastexo-xblock-7.9.1/tests/unit/test_gcloud.py`

 * *Files identical despite different names*

### Comparing `hastexo-xblock-7.9.0/tests/unit/test_hastexo.py` & `hastexo-xblock-7.9.1/tests/unit/test_hastexo.py`

 * *Files 1% similar despite different names*

```diff
@@ -1650,19 +1650,32 @@
             self.assertNotIn('text_js_url', js_urls)
 
     def test_launch_new_window(self):
         self.init_block()
 
         with patch('webob.Request') as request:
             request.cookies = Mock()
-            request.cookies.get.return_value = 'fake_csrf_token'
+            request.cookies = {
+                'sessionid': 'fake_sessionid',
+                'csrftoken': 'fake_csrf_token'}
             response = self.block.launch_new_window(request)
 
             self.assertEqual("200 OK", response.status)
 
+    def test_launch_new_window_unauthorized(self):
+        self.init_block()
+
+        with patch('webob.Request') as request:
+            request.cookies = Mock()
+            request.cookies = {'fake': 'cookie'}
+            response = self.block.launch_new_window(request)
+
+            self.assertEqual("401 Unauthorized", response.status)
+            self.assertEqual(b'Unauthorized', response.body)
+
     def test_fullscreen_setting(self):
         self.init_block()
         settings = get_xblock_settings()
         enable_fullscreen = self.block.get_enable_fullscreen(settings)
 
         # by default the setting is to be inherited from global settings
         self.assertEqual("inherit", self.block.enable_fullscreen)
```

### Comparing `hastexo-xblock-7.9.0/tests/unit/test_jobs.py` & `hastexo-xblock-7.9.1/tests/unit/test_jobs.py`

 * *Files identical despite different names*

### Comparing `hastexo-xblock-7.9.0/tests/unit/test_models.py` & `hastexo-xblock-7.9.1/tests/unit/test_models.py`

 * *Files identical despite different names*

### Comparing `hastexo-xblock-7.9.0/tests/unit/test_openstack.py` & `hastexo-xblock-7.9.1/tests/unit/test_openstack.py`

 * *Files identical despite different names*

### Comparing `hastexo-xblock-7.9.0/tests/unit/test_provider.py` & `hastexo-xblock-7.9.1/tests/unit/test_provider.py`

 * *Files identical despite different names*

### Comparing `hastexo-xblock-7.9.0/tests/unit/test_tasks.py` & `hastexo-xblock-7.9.1/tests/unit/test_tasks.py`

 * *Files identical despite different names*

### Comparing `hastexo-xblock-7.9.0/tox.ini` & `hastexo-xblock-7.9.1/tox.ini`

 * *Files identical despite different names*

