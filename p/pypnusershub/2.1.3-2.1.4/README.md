# Comparing `tmp/pypnusershub-2.1.3.tar.gz` & `tmp/pypnusershub-2.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypnusershub-2.1.3.tar", last modified: Thu Feb 22 17:30:21 2024, max compression
+gzip compressed data, was "pypnusershub-2.1.4.tar", last modified: Tue Apr 23 12:23:07 2024, max compression
```

## Comparing `pypnusershub-2.1.3.tar` & `pypnusershub-2.1.4.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 17:30:21.212032 pypnusershub-2.1.3/
--rw-r--r--   0 runner    (1001) docker     (127)    35141 2024-02-22 17:30:13.000000 pypnusershub-2.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-02-22 17:30:13.000000 pypnusershub-2.1.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     9482 2024-02-22 17:30:21.212032 pypnusershub-2.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8264 2024-02-22 17:30:13.000000 pypnusershub-2.1.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-02-22 17:30:13.000000 pypnusershub-2.1.3/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-02-22 17:30:13.000000 pypnusershub-2.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-02-22 17:30:13.000000 pypnusershub-2.1.3/requirements-common.in
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-02-22 17:30:13.000000 pypnusershub-2.1.3/requirements-dependencies.in
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-22 17:30:21.212032 pypnusershub-2.1.3/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     1564 2024-02-22 17:30:13.000000 pypnusershub-2.1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 17:30:21.204032 pypnusershub-2.1.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 17:30:21.208032 pypnusershub-2.1.3/src/pypnusershub/
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-02-22 17:30:13.000000 pypnusershub-2.1.3/src/pypnusershub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2867 2024-02-22 17:30:13.000000 pypnusershub-2.1.3/src/pypnusershub/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 17:30:21.208032 pypnusershub-2.1.3/src/pypnusershub/db/
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-02-22 17:30:13.000000 pypnusershub-2.1.3/src/pypnusershub/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4424 2024-02-22 17:30:13.000000 pypnusershub-2.1.3/src/pypnusershub/db/fixtures.sql
--rw-r--r--   0 runner    (1001) docker     (127)    14767 2024-02-22 17:30:13.000000 pypnusershub-2.1.3/src/pypnusershub/db/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     4878 2024-02-22 17:30:13.000000 pypnusershub-2.1.3/src/pypnusershub/db/models_register.py
--rw-r--r--   0 runner    (1001) docker     (127)     3898 2024-02-22 17:30:13.000000 pypnusershub-2.1.3/src/pypnusershub/db/tools.py
--rw-r--r--   0 runner    (1001) docker     (127)      922 2024-02-22 17:30:13.000000 pypnusershub-2.1.3/src/pypnusershub/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)      788 2024-02-22 17:30:13.000000 pypnusershub-2.1.3/src/pypnusershub/env.py
--rw-r--r--   0 runner    (1001) docker     (127)     1191 2024-02-22 17:30:13.000000 pypnusershub-2.1.3/src/pypnusershub/login_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 17:30:21.208032 pypnusershub-2.1.3/src/pypnusershub/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-22 17:30:13.000000 pypnusershub-2.1.3/src/pypnusershub/migrations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 17:30:21.208032 pypnusershub-2.1.3/src/pypnusershub/migrations/data/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-22 17:30:13.000000 pypnusershub-2.1.3/src/pypnusershub/migrations/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3605 2024-02-22 17:30:13.000000 pypnusershub-2.1.3/src/pypnusershub/migrations/data/utilisateurs-samples.sql
--rw-r--r--   0 runner    (1001) docker     (127)    15812 2024-02-22 17:30:13.000000 pypnusershub-2.1.3/src/pypnusershub/migrations/data/utilisateurs.sql
--rw-r--r--   0 runner    (1001) docker     (127)     2158 2024-02-22 17:30:13.000000 pypnusershub-2.1.3/src/pypnusershub/migrations/env.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 17:30:21.212032 pypnusershub-2.1.3/src/pypnusershub/migrations/versions/
--rw-r--r--   0 runner    (1001) docker     (127)      821 2024-02-22 17:30:13.000000 pypnusershub-2.1.3/src/pypnusershub/migrations/versions/10e87bc144cd_get_id_role_by_name.py
--rw-r--r--   0 runner    (1001) docker     (127)      548 2024-02-22 17:30:13.000000 pypnusershub-2.1.3/src/pypnusershub/migrations/versions/112ccf1024ce_add_unique_constraint_on_t_roles_uuid.py
--rw-r--r--   0 runner    (1001) docker     (127)     5883 2024-02-22 17:30:13.000000 pypnusershub-2.1.3/src/pypnusershub/migrations/versions/5b334b77f5f5_fix_v_roleslist_forall_applications.py
--rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-02-22 17:30:13.000000 pypnusershub-2.1.3/src/pypnusershub/migrations/versions/72f227e37bdf_utilisateurs_sample_data.py
--rw-r--r--   0 runner    (1001) docker     (127)      640 2024-02-22 17:30:13.000000 pypnusershub-2.1.3/src/pypnusershub/migrations/versions/830cc8f4daef_add_additional_data_field_to_organism.py
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-02-22 17:30:13.000000 pypnusershub-2.1.3/src/pypnusershub/migrations/versions/951b8270a1cf_add_unique_constraint_on_uuid_organisme.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-22 17:30:13.000000 pypnusershub-2.1.3/src/pypnusershub/migrations/versions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      477 2024-02-22 17:30:13.000000 pypnusershub-2.1.3/src/pypnusershub/migrations/versions/f4bf21ac6238_fix_temp_user_organism_size.py
--rw-r--r--   0 runner    (1001) docker     (127)      686 2024-02-22 17:30:13.000000 pypnusershub-2.1.3/src/pypnusershub/migrations/versions/f9d3b95946cd_set_code_profil_in_integer.py
--rw-r--r--   0 runner    (1001) docker     (127)      567 2024-02-22 17:30:13.000000 pypnusershub-2.1.3/src/pypnusershub/migrations/versions/fa35dfe5ff27_create_utilisateurs_schema.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6691 2024-02-22 17:30:13.000000 pypnusershub-2.1.3/src/pypnusershub/routes.py
--rw-r--r--   0 runner    (1001) docker     (127)     7217 2024-02-22 17:30:13.000000 pypnusershub-2.1.3/src/pypnusershub/routes_register.py
--rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-02-22 17:30:13.000000 pypnusershub-2.1.3/src/pypnusershub/schemas.py
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-02-22 17:30:13.000000 pypnusershub-2.1.3/src/pypnusershub/test_settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 17:30:21.212032 pypnusershub-2.1.3/src/pypnusershub/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-22 17:30:13.000000 pypnusershub-2.1.3/src/pypnusershub/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      839 2024-02-22 17:30:13.000000 pypnusershub-2.1.3/src/pypnusershub/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2900 2024-02-22 17:30:13.000000 pypnusershub-2.1.3/src/pypnusershub/tests/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (127)     3409 2024-02-22 17:30:13.000000 pypnusershub-2.1.3/src/pypnusershub/tests/test_utilisateurs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-02-22 17:30:13.000000 pypnusershub-2.1.3/src/pypnusershub/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1579 2024-02-22 17:30:13.000000 pypnusershub-2.1.3/src/pypnusershub/tests/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3734 2024-02-22 17:30:13.000000 pypnusershub-2.1.3/src/pypnusershub/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 17:30:21.212032 pypnusershub-2.1.3/src/pypnusershub.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9482 2024-02-22 17:30:21.000000 pypnusershub-2.1.3/src/pypnusershub.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2067 2024-02-22 17:30:21.000000 pypnusershub-2.1.3/src/pypnusershub.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-22 17:30:21.000000 pypnusershub-2.1.3/src/pypnusershub.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-02-22 17:30:21.000000 pypnusershub-2.1.3/src/pypnusershub.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-02-22 17:30:21.000000 pypnusershub-2.1.3/src/pypnusershub.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-02-22 17:30:21.000000 pypnusershub-2.1.3/src/pypnusershub.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 12:23:07.468631 pypnusershub-2.1.4/
+-rw-r--r--   0 runner    (1001) docker     (127)    35141 2024-04-23 12:23:03.000000 pypnusershub-2.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-23 12:23:03.000000 pypnusershub-2.1.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     9482 2024-04-23 12:23:07.468631 pypnusershub-2.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8264 2024-04-23 12:23:03.000000 pypnusershub-2.1.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-23 12:23:03.000000 pypnusershub-2.1.4/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-23 12:23:03.000000 pypnusershub-2.1.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-04-23 12:23:03.000000 pypnusershub-2.1.4/requirements-common.in
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-23 12:23:03.000000 pypnusershub-2.1.4/requirements-dependencies.in
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 12:23:07.468631 pypnusershub-2.1.4/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1564 2024-04-23 12:23:03.000000 pypnusershub-2.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 12:23:07.460631 pypnusershub-2.1.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 12:23:07.464631 pypnusershub-2.1.4/src/pypnusershub/
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-23 12:23:03.000000 pypnusershub-2.1.4/src/pypnusershub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2867 2024-04-23 12:23:03.000000 pypnusershub-2.1.4/src/pypnusershub/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 12:23:07.464631 pypnusershub-2.1.4/src/pypnusershub/db/
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-23 12:23:03.000000 pypnusershub-2.1.4/src/pypnusershub/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4424 2024-04-23 12:23:03.000000 pypnusershub-2.1.4/src/pypnusershub/db/fixtures.sql
+-rw-r--r--   0 runner    (1001) docker     (127)    14767 2024-04-23 12:23:03.000000 pypnusershub-2.1.4/src/pypnusershub/db/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4878 2024-04-23 12:23:03.000000 pypnusershub-2.1.4/src/pypnusershub/db/models_register.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3898 2024-04-23 12:23:03.000000 pypnusershub-2.1.4/src/pypnusershub/db/tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)      922 2024-04-23 12:23:03.000000 pypnusershub-2.1.4/src/pypnusershub/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)      788 2024-04-23 12:23:03.000000 pypnusershub-2.1.4/src/pypnusershub/env.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1191 2024-04-23 12:23:03.000000 pypnusershub-2.1.4/src/pypnusershub/login_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 12:23:07.464631 pypnusershub-2.1.4/src/pypnusershub/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 12:23:03.000000 pypnusershub-2.1.4/src/pypnusershub/migrations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 12:23:07.464631 pypnusershub-2.1.4/src/pypnusershub/migrations/data/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 12:23:03.000000 pypnusershub-2.1.4/src/pypnusershub/migrations/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3605 2024-04-23 12:23:03.000000 pypnusershub-2.1.4/src/pypnusershub/migrations/data/utilisateurs-samples.sql
+-rw-r--r--   0 runner    (1001) docker     (127)    15812 2024-04-23 12:23:03.000000 pypnusershub-2.1.4/src/pypnusershub/migrations/data/utilisateurs.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     2158 2024-04-23 12:23:03.000000 pypnusershub-2.1.4/src/pypnusershub/migrations/env.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 12:23:07.468631 pypnusershub-2.1.4/src/pypnusershub/migrations/versions/
+-rw-r--r--   0 runner    (1001) docker     (127)      821 2024-04-23 12:23:03.000000 pypnusershub-2.1.4/src/pypnusershub/migrations/versions/10e87bc144cd_get_id_role_by_name.py
+-rw-r--r--   0 runner    (1001) docker     (127)      548 2024-04-23 12:23:03.000000 pypnusershub-2.1.4/src/pypnusershub/migrations/versions/112ccf1024ce_add_unique_constraint_on_t_roles_uuid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5883 2024-04-23 12:23:03.000000 pypnusershub-2.1.4/src/pypnusershub/migrations/versions/5b334b77f5f5_fix_v_roleslist_forall_applications.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-04-23 12:23:03.000000 pypnusershub-2.1.4/src/pypnusershub/migrations/versions/72f227e37bdf_utilisateurs_sample_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-04-23 12:23:03.000000 pypnusershub-2.1.4/src/pypnusershub/migrations/versions/830cc8f4daef_add_additional_data_field_to_organism.py
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-04-23 12:23:03.000000 pypnusershub-2.1.4/src/pypnusershub/migrations/versions/951b8270a1cf_add_unique_constraint_on_uuid_organisme.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 12:23:03.000000 pypnusershub-2.1.4/src/pypnusershub/migrations/versions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      477 2024-04-23 12:23:03.000000 pypnusershub-2.1.4/src/pypnusershub/migrations/versions/f4bf21ac6238_fix_temp_user_organism_size.py
+-rw-r--r--   0 runner    (1001) docker     (127)      686 2024-04-23 12:23:03.000000 pypnusershub-2.1.4/src/pypnusershub/migrations/versions/f9d3b95946cd_set_code_profil_in_integer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      567 2024-04-23 12:23:03.000000 pypnusershub-2.1.4/src/pypnusershub/migrations/versions/fa35dfe5ff27_create_utilisateurs_schema.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6956 2024-04-23 12:23:03.000000 pypnusershub-2.1.4/src/pypnusershub/routes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7217 2024-04-23 12:23:03.000000 pypnusershub-2.1.4/src/pypnusershub/routes_register.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-04-23 12:23:03.000000 pypnusershub-2.1.4/src/pypnusershub/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-23 12:23:03.000000 pypnusershub-2.1.4/src/pypnusershub/test_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 12:23:07.468631 pypnusershub-2.1.4/src/pypnusershub/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 12:23:03.000000 pypnusershub-2.1.4/src/pypnusershub/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      839 2024-04-23 12:23:03.000000 pypnusershub-2.1.4/src/pypnusershub/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2900 2024-04-23 12:23:03.000000 pypnusershub-2.1.4/src/pypnusershub/tests/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3409 2024-04-23 12:23:03.000000 pypnusershub-2.1.4/src/pypnusershub/tests/test_utilisateurs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-04-23 12:23:03.000000 pypnusershub-2.1.4/src/pypnusershub/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1579 2024-04-23 12:23:03.000000 pypnusershub-2.1.4/src/pypnusershub/tests/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3734 2024-04-23 12:23:03.000000 pypnusershub-2.1.4/src/pypnusershub/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 12:23:07.468631 pypnusershub-2.1.4/src/pypnusershub.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9482 2024-04-23 12:23:07.000000 pypnusershub-2.1.4/src/pypnusershub.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2067 2024-04-23 12:23:07.000000 pypnusershub-2.1.4/src/pypnusershub.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 12:23:07.000000 pypnusershub-2.1.4/src/pypnusershub.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-23 12:23:07.000000 pypnusershub-2.1.4/src/pypnusershub.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-04-23 12:23:07.000000 pypnusershub-2.1.4/src/pypnusershub.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-23 12:23:07.000000 pypnusershub-2.1.4/src/pypnusershub.egg-info/top_level.txt
```

### Comparing `pypnusershub-2.1.3/LICENSE` & `pypnusershub-2.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pypnusershub-2.1.3/PKG-INFO` & `pypnusershub-2.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypnusershub
-Version: 2.1.3
+Version: 2.1.4
 Summary: Python lib to authenticate using PN's UsersHub
 Home-page: https://github.com/PnX-SI/UsersHub-authentification-module
 Maintainer: Parcs nationaux des Écrins et des Cévennes
 Maintainer-email: geonature@ecrins-parcnational.fr
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
```

### Comparing `pypnusershub-2.1.3/README.md` & `pypnusershub-2.1.4/README.md`

 * *Files identical despite different names*

### Comparing `pypnusershub-2.1.3/setup.py` & `pypnusershub-2.1.4/setup.py`

 * *Files identical despite different names*

### Comparing `pypnusershub-2.1.3/src/pypnusershub/__main__.py` & `pypnusershub-2.1.4/src/pypnusershub/__main__.py`

 * *Files identical despite different names*

### Comparing `pypnusershub-2.1.3/src/pypnusershub/db/fixtures.sql` & `pypnusershub-2.1.4/src/pypnusershub/db/fixtures.sql`

 * *Files identical despite different names*

### Comparing `pypnusershub-2.1.3/src/pypnusershub/db/models.py` & `pypnusershub-2.1.4/src/pypnusershub/db/models.py`

 * *Files identical despite different names*

### Comparing `pypnusershub-2.1.3/src/pypnusershub/db/models_register.py` & `pypnusershub-2.1.4/src/pypnusershub/db/models_register.py`

 * *Files identical despite different names*

### Comparing `pypnusershub-2.1.3/src/pypnusershub/db/tools.py` & `pypnusershub-2.1.4/src/pypnusershub/db/tools.py`

 * *Files identical despite different names*

### Comparing `pypnusershub-2.1.3/src/pypnusershub/decorators.py` & `pypnusershub-2.1.4/src/pypnusershub/decorators.py`

 * *Files identical despite different names*

### Comparing `pypnusershub-2.1.3/src/pypnusershub/env.py` & `pypnusershub-2.1.4/src/pypnusershub/env.py`

 * *Files identical despite different names*

### Comparing `pypnusershub-2.1.3/src/pypnusershub/login_manager.py` & `pypnusershub-2.1.4/src/pypnusershub/login_manager.py`

 * *Files identical despite different names*

### Comparing `pypnusershub-2.1.3/src/pypnusershub/migrations/data/utilisateurs-samples.sql` & `pypnusershub-2.1.4/src/pypnusershub/migrations/data/utilisateurs-samples.sql`

 * *Files identical despite different names*

### Comparing `pypnusershub-2.1.3/src/pypnusershub/migrations/data/utilisateurs.sql` & `pypnusershub-2.1.4/src/pypnusershub/migrations/data/utilisateurs.sql`

 * *Files identical despite different names*

### Comparing `pypnusershub-2.1.3/src/pypnusershub/migrations/env.py` & `pypnusershub-2.1.4/src/pypnusershub/migrations/env.py`

 * *Files identical despite different names*

### Comparing `pypnusershub-2.1.3/src/pypnusershub/migrations/versions/10e87bc144cd_get_id_role_by_name.py` & `pypnusershub-2.1.4/src/pypnusershub/migrations/versions/10e87bc144cd_get_id_role_by_name.py`

 * *Files identical despite different names*

### Comparing `pypnusershub-2.1.3/src/pypnusershub/migrations/versions/112ccf1024ce_add_unique_constraint_on_t_roles_uuid.py` & `pypnusershub-2.1.4/src/pypnusershub/migrations/versions/112ccf1024ce_add_unique_constraint_on_t_roles_uuid.py`

 * *Files identical despite different names*

### Comparing `pypnusershub-2.1.3/src/pypnusershub/migrations/versions/5b334b77f5f5_fix_v_roleslist_forall_applications.py` & `pypnusershub-2.1.4/src/pypnusershub/migrations/versions/5b334b77f5f5_fix_v_roleslist_forall_applications.py`

 * *Files identical despite different names*

### Comparing `pypnusershub-2.1.3/src/pypnusershub/migrations/versions/72f227e37bdf_utilisateurs_sample_data.py` & `pypnusershub-2.1.4/src/pypnusershub/migrations/versions/72f227e37bdf_utilisateurs_sample_data.py`

 * *Files identical despite different names*

### Comparing `pypnusershub-2.1.3/src/pypnusershub/migrations/versions/830cc8f4daef_add_additional_data_field_to_organism.py` & `pypnusershub-2.1.4/src/pypnusershub/migrations/versions/830cc8f4daef_add_additional_data_field_to_organism.py`

 * *Files identical despite different names*

### Comparing `pypnusershub-2.1.3/src/pypnusershub/migrations/versions/951b8270a1cf_add_unique_constraint_on_uuid_organisme.py` & `pypnusershub-2.1.4/src/pypnusershub/migrations/versions/951b8270a1cf_add_unique_constraint_on_uuid_organisme.py`

 * *Files identical despite different names*

### Comparing `pypnusershub-2.1.3/src/pypnusershub/migrations/versions/f9d3b95946cd_set_code_profil_in_integer.py` & `pypnusershub-2.1.4/src/pypnusershub/migrations/versions/f9d3b95946cd_set_code_profil_in_integer.py`

 * *Files identical despite different names*

### Comparing `pypnusershub-2.1.3/src/pypnusershub/migrations/versions/fa35dfe5ff27_create_utilisateurs_schema.py` & `pypnusershub-2.1.4/src/pypnusershub/migrations/versions/fa35dfe5ff27_create_utilisateurs_schema.py`

 * *Files identical despite different names*

### Comparing `pypnusershub-2.1.3/src/pypnusershub/routes.py` & `pypnusershub-2.1.4/src/pypnusershub/routes.py`

 * *Files 6% similar despite different names*

```diff
@@ -61,21 +61,24 @@
 #    but the param is called 'INIT_APP_WITH_DB' and default to True.
 #  - the 'login' url must be configuratble. We provide this with the
 #    'LOGIN_ROUTE' param, but we still default to '/login' and POST.
 
 
 class ConfigurableBlueprint(Blueprint):
     def register(self, app, *args, **kwargs):
-        # set cookie autorenew
         app.config["PASS_METHOD"] = app.config.get("PASS_METHOD", "hash")
 
         app.config["REMEMBER_COOKIE_NAME"] = app.config.get(
             "REMEMBER_COOKIE_NAME", "token"
         )
-
+        # retro-compat set COOKIE_EXPIRATION in REMEMBER_COOKIE_DURATION
+        # (Flask Login parameter, default 1 year)
+        app.config["REMEMBER_COOKIE_DURATION"] = app.config.get(
+            "COOKIE_EXPIRATION", 31557600
+        )
         parent = super(ConfigurableBlueprint, self)
         parent.register(app, *args, **kwargs)
 
         @app.before_request
         def load_current_user():
             g.current_user = current_user
 
@@ -124,19 +127,21 @@
         return Response(msg, status=status_code)
 
     if not user.check_password(user_data["password"]):
         msg = json.dumps({"type": "password", "msg": "Mot de passe invalide"})
         log.info(msg)
         status_code = current_app.config.get("BAD_LOGIN_STATUS_CODE", 490)
         return Response(msg, status=status_code)
-    login_user(user)
+    login_user(user, remember=True)
     # Génération d'un token
     token = encode_token(user_dict)
     token_exp = datetime.datetime.now(datetime.timezone.utc)
-    token_exp += datetime.timedelta(seconds=current_app.config["COOKIE_EXPIRATION"])
+    token_exp += datetime.timedelta(
+        seconds=current_app.config["REMEMBER_COOKIE_DURATION"]
+    )
     return jsonify(
         {"user": user_dict, "expires": token_exp.isoformat(), "token": token.decode()}
     )
 
 
 @routes.route("/public_login", methods=["POST"])
 def public_login():
@@ -151,15 +156,17 @@
     ).scalar_one()
 
     user_dict = user.as_dict()
     login_user(user)
     # Génération d'un token
     token = encode_token(user_dict)
     token_exp = datetime.datetime.now(datetime.timezone.utc)
-    token_exp += datetime.timedelta(seconds=current_app.config["COOKIE_EXPIRATION"])
+    token_exp += datetime.timedelta(
+        seconds=current_app.config["REMEMBER_COOKIE_DURATION"]
+    )
 
     return jsonify(
         {"user": user_dict, "expires": token_exp.isoformat(), "token": token.decode()}
     )
 
 
 @routes.route("/logout", methods=["GET", "POST"])
```

### Comparing `pypnusershub-2.1.3/src/pypnusershub/routes_register.py` & `pypnusershub-2.1.4/src/pypnusershub/routes_register.py`

 * *Files identical despite different names*

### Comparing `pypnusershub-2.1.3/src/pypnusershub/schemas.py` & `pypnusershub-2.1.4/src/pypnusershub/schemas.py`

 * *Files identical despite different names*

### Comparing `pypnusershub-2.1.3/src/pypnusershub/tests/conftest.py` & `pypnusershub-2.1.4/src/pypnusershub/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pypnusershub-2.1.3/src/pypnusershub/tests/fixtures.py` & `pypnusershub-2.1.4/src/pypnusershub/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `pypnusershub-2.1.3/src/pypnusershub/tests/test_utilisateurs.py` & `pypnusershub-2.1.4/src/pypnusershub/tests/test_utilisateurs.py`

 * *Files identical despite different names*

### Comparing `pypnusershub-2.1.3/src/pypnusershub/tests/test_utils.py` & `pypnusershub-2.1.4/src/pypnusershub/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `pypnusershub-2.1.3/src/pypnusershub/tests/utils.py` & `pypnusershub-2.1.4/src/pypnusershub/tests/utils.py`

 * *Files identical despite different names*

### Comparing `pypnusershub-2.1.3/src/pypnusershub/utils.py` & `pypnusershub-2.1.4/src/pypnusershub/utils.py`

 * *Files identical despite different names*

### Comparing `pypnusershub-2.1.3/src/pypnusershub.egg-info/PKG-INFO` & `pypnusershub-2.1.4/src/pypnusershub.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypnusershub
-Version: 2.1.3
+Version: 2.1.4
 Summary: Python lib to authenticate using PN's UsersHub
 Home-page: https://github.com/PnX-SI/UsersHub-authentification-module
 Maintainer: Parcs nationaux des Écrins et des Cévennes
 Maintainer-email: geonature@ecrins-parcnational.fr
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
```

### Comparing `pypnusershub-2.1.3/src/pypnusershub.egg-info/SOURCES.txt` & `pypnusershub-2.1.4/src/pypnusershub.egg-info/SOURCES.txt`

 * *Files identical despite different names*

