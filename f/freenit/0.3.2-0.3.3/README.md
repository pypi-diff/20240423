# Comparing `tmp/freenit-0.3.2.tar.gz` & `tmp/freenit-0.3.3.tar.gz`

## Comparing `freenit-0.3.2.tar` & `freenit-0.3.3.tar`

### file list

```diff
@@ -1,108 +1,108 @@
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 freenit-0.3.2/.pylintrc
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 freenit-0.3.2/MANIFEST.in
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 freenit-0.3.2/Makefile
--rw-r--r--   0        0        0     2146 2020-02-02 00:00:00.000000 freenit-0.3.2/alembic.ini
--rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 freenit-0.3.2/main.py
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 freenit-0.3.2/name.py
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 freenit-0.3.2/provisioners.mk
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 freenit-0.3.2/pytest.ini
--rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 freenit-0.3.2/requirements.yml
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 freenit-0.3.2/setup.cfg
--rw-r--r--   0        0        0     2435 2020-02-02 00:00:00.000000 freenit-0.3.2/setup.py
--rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 freenit-0.3.2/.github/workflows/pythonapp.yml
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 freenit-0.3.2/alembic/README
--rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 freenit-0.3.2/alembic/env.py
--rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 freenit-0.3.2/alembic/script.py.mako
--rw-r--r--   0        0        0     3029 2020-02-02 00:00:00.000000 freenit-0.3.2/alembic/versions/06a043f2516a_initial.py
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 freenit-0.3.2/ansible/group_vars/.keep
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 freenit-0.3.2/ansible/inventory/.keep
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 freenit-0.3.2/ansible/roles/.keep
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 freenit-0.3.2/ansible/roles/devel/tasks/main.yml
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 freenit-0.3.2/ansible/roles/devel/vars/main.yml
--rwxr-xr-x   0        0        0      202 2020-02-02 00:00:00.000000 freenit-0.3.2/bin/build.sh
--rw-r--r--   0        0        0     1024 2020-02-02 00:00:00.000000 freenit-0.3.2/bin/common.sh
--rwxr-xr-x   0        0        0      335 2020-02-02 00:00:00.000000 freenit-0.3.2/bin/devel.sh
--rwxr-xr-x   0        0        0    12122 2020-02-02 00:00:00.000000 freenit-0.3.2/bin/freenit.sh
--rwxr-xr-x   0        0        0       95 2020-02-02 00:00:00.000000 freenit-0.3.2/bin/init.sh
--rwxr-xr-x   0        0        0      183 2020-02-02 00:00:00.000000 freenit-0.3.2/bin/publish.sh
--rwxr-xr-x   0        0        0      163 2020-02-02 00:00:00.000000 freenit-0.3.2/bin/security.sh
--rwxr-xr-x   0        0        0      129 2020-02-02 00:00:00.000000 freenit-0.3.2/bin/test.sh
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 freenit-0.3.2/freenit/__init__.py
--rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 freenit-0.3.2/freenit/app.py
--rw-r--r--   0        0        0     2898 2020-02-02 00:00:00.000000 freenit-0.3.2/freenit/auth.py
--rw-r--r--   0        0        0     3062 2020-02-02 00:00:00.000000 freenit-0.3.2/freenit/base_config.py
--rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 freenit-0.3.2/freenit/cli.py
--rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 freenit-0.3.2/freenit/config.py
--rw-r--r--   0        0        0     2087 2020-02-02 00:00:00.000000 freenit-0.3.2/freenit/decorators.py
--rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 freenit-0.3.2/freenit/mail.py
--rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 freenit-0.3.2/freenit/migration.py
--rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 freenit-0.3.2/freenit/permissions.py
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 freenit-0.3.2/freenit/api/__init__.py
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 freenit-0.3.2/freenit/api/router.py
--rw-r--r--   0        0        0     2656 2020-02-02 00:00:00.000000 freenit-0.3.2/freenit/api/theme.py
--rw-r--r--   0        0        0     3221 2020-02-02 00:00:00.000000 freenit-0.3.2/freenit/api/auth/__init__.py
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 freenit-0.3.2/freenit/api/role/__init__.py
--rw-r--r--   0        0        0     2913 2020-02-02 00:00:00.000000 freenit-0.3.2/freenit/api/role/ldap.py
--rw-r--r--   0        0        0     3670 2020-02-02 00:00:00.000000 freenit-0.3.2/freenit/api/role/sql.py
--rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 freenit-0.3.2/freenit/api/user/__init__.py
--rw-r--r--   0        0        0     3154 2020-02-02 00:00:00.000000 freenit-0.3.2/freenit/api/user/ldap.py
--rw-r--r--   0        0        0     2450 2020-02-02 00:00:00.000000 freenit-0.3.2/freenit/api/user/sql.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 freenit-0.3.2/freenit/models/__init__.py
--rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 freenit-0.3.2/freenit/models/pagination.py
--rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 freenit-0.3.2/freenit/models/role.py
--rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 freenit-0.3.2/freenit/models/safe.py
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 freenit-0.3.2/freenit/models/theme.py
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 freenit-0.3.2/freenit/models/user.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 freenit-0.3.2/freenit/models/ldap/__init__.py
--rw-r--r--   0        0        0     3025 2020-02-02 00:00:00.000000 freenit-0.3.2/freenit/models/ldap/base.py
--rw-r--r--   0        0        0     4166 2020-02-02 00:00:00.000000 freenit-0.3.2/freenit/models/ldap/role.py
--rw-r--r--   0        0        0     3966 2020-02-02 00:00:00.000000 freenit-0.3.2/freenit/models/ldap/user.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 freenit-0.3.2/freenit/models/sql/__init__.py
--rw-r--r--   0        0        0     1111 2020-02-02 00:00:00.000000 freenit-0.3.2/freenit/models/sql/base.py
--rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 freenit-0.3.2/freenit/models/sql/role.py
--rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 freenit-0.3.2/freenit/models/sql/theme.py
--rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 freenit-0.3.2/freenit/models/sql/user.py
--rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 freenit-0.3.2/freenit/project/.gitignore
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 freenit-0.3.2/freenit/project/LICENSE
--rw-r--r--   0        0        0     2154 2020-02-02 00:00:00.000000 freenit-0.3.2/freenit/project/alembic.ini
--rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 freenit-0.3.2/freenit/project/main.py
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 freenit-0.3.2/freenit/project/provisioners.mk
--rw-r--r--   0        0        0      879 2020-02-02 00:00:00.000000 freenit-0.3.2/freenit/project/pyproject.toml
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 freenit-0.3.2/freenit/project/requirements.yml
--rw-r--r--   0        0        0     1301 2020-02-02 00:00:00.000000 freenit-0.3.2/freenit/project/setup.py
--rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 freenit-0.3.2/freenit/project/alembic/script.py.mako
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 freenit-0.3.2/freenit/project/ansible/group_vars/.keep
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 freenit-0.3.2/freenit/project/ansible/inventory/.keep
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 freenit-0.3.2/freenit/project/ansible/roles/devel/tasks/main.yml
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 freenit-0.3.2/freenit/project/ansible/roles/devel/vars/main.yml
--rw-r--r--   0        0        0      928 2020-02-02 00:00:00.000000 freenit-0.3.2/freenit/project/bin/common.sh
--rwxr-xr-x   0        0        0      309 2020-02-02 00:00:00.000000 freenit-0.3.2/freenit/project/bin/devel.sh
--rwxr-xr-x   0        0        0       95 2020-02-02 00:00:00.000000 freenit-0.3.2/freenit/project/bin/init.sh
--rwxr-xr-x   0        0        0       99 2020-02-02 00:00:00.000000 freenit-0.3.2/freenit/project/bin/test.sh
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 freenit-0.3.2/freenit/project/project/__init__.py
--rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 freenit-0.3.2/freenit/project/project/app.py
--rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 freenit-0.3.2/freenit/project/project/base_config.py
--rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 freenit-0.3.2/freenit/project/project/config.py
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 freenit-0.3.2/freenit/project/project/api/__init__.py
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 freenit-0.3.2/freenit/project/project/api/router.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 freenit-0.3.2/freenit/project/project/models/__init__.py
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 freenit-0.3.2/freenit/project/templates/site.yml.tpl
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 freenit-0.3.2/freenit/project/tests/__init__.py
--rw-r--r--   0        0        0     1318 2020-02-02 00:00:00.000000 freenit-0.3.2/freenit/project/tests/client.py
--rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 freenit-0.3.2/freenit/project/tests/conftest.py
--rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 freenit-0.3.2/freenit/project/tests/factories.py
--rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 freenit-0.3.2/freenit/project/tests/test_user.py
--rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 freenit-0.3.2/templates/site.yml.tpl
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 freenit-0.3.2/tests/__init__.py
--rw-r--r--   0        0        0     1185 2020-02-02 00:00:00.000000 freenit-0.3.2/tests/client.py
--rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 freenit-0.3.2/tests/conftest.py
--rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 freenit-0.3.2/tests/factories.py
--rw-r--r--   0        0        0      787 2020-02-02 00:00:00.000000 freenit-0.3.2/tests/test_auth.py
--rw-r--r--   0        0        0     2157 2020-02-02 00:00:00.000000 freenit-0.3.2/tests/test_permission.py
--rw-r--r--   0        0        0     2281 2020-02-02 00:00:00.000000 freenit-0.3.2/tests/test_role.py
--rw-r--r--   0        0        0     1944 2020-02-02 00:00:00.000000 freenit-0.3.2/tests/test_user.py
--rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 freenit-0.3.2/.gitignore
--rw-r--r--   0        0        0     1322 2020-02-02 00:00:00.000000 freenit-0.3.2/LICENSE
--rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 freenit-0.3.2/README.md
--rw-r--r--   0        0        0     1548 2020-02-02 00:00:00.000000 freenit-0.3.2/pyproject.toml
--rw-r--r--   0        0        0     3845 2020-02-02 00:00:00.000000 freenit-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 freenit-0.3.3/.pylintrc
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 freenit-0.3.3/MANIFEST.in
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 freenit-0.3.3/Makefile
+-rw-r--r--   0        0        0     2146 2020-02-02 00:00:00.000000 freenit-0.3.3/alembic.ini
+-rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 freenit-0.3.3/main.py
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 freenit-0.3.3/name.py
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 freenit-0.3.3/provisioners.mk
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 freenit-0.3.3/pytest.ini
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 freenit-0.3.3/requirements.yml
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 freenit-0.3.3/setup.cfg
+-rw-r--r--   0        0        0     2435 2020-02-02 00:00:00.000000 freenit-0.3.3/setup.py
+-rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 freenit-0.3.3/.github/workflows/pythonapp.yml
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 freenit-0.3.3/alembic/README
+-rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 freenit-0.3.3/alembic/env.py
+-rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 freenit-0.3.3/alembic/script.py.mako
+-rw-r--r--   0        0        0     3029 2020-02-02 00:00:00.000000 freenit-0.3.3/alembic/versions/06a043f2516a_initial.py
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 freenit-0.3.3/ansible/group_vars/.keep
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 freenit-0.3.3/ansible/inventory/.keep
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 freenit-0.3.3/ansible/roles/.keep
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 freenit-0.3.3/ansible/roles/devel/tasks/main.yml
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 freenit-0.3.3/ansible/roles/devel/vars/main.yml
+-rwxr-xr-x   0        0        0      202 2020-02-02 00:00:00.000000 freenit-0.3.3/bin/build.sh
+-rw-r--r--   0        0        0     1024 2020-02-02 00:00:00.000000 freenit-0.3.3/bin/common.sh
+-rwxr-xr-x   0        0        0      335 2020-02-02 00:00:00.000000 freenit-0.3.3/bin/devel.sh
+-rwxr-xr-x   0        0        0    12122 2020-02-02 00:00:00.000000 freenit-0.3.3/bin/freenit.sh
+-rwxr-xr-x   0        0        0       95 2020-02-02 00:00:00.000000 freenit-0.3.3/bin/init.sh
+-rwxr-xr-x   0        0        0      183 2020-02-02 00:00:00.000000 freenit-0.3.3/bin/publish.sh
+-rwxr-xr-x   0        0        0      163 2020-02-02 00:00:00.000000 freenit-0.3.3/bin/security.sh
+-rwxr-xr-x   0        0        0      129 2020-02-02 00:00:00.000000 freenit-0.3.3/bin/test.sh
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 freenit-0.3.3/freenit/__init__.py
+-rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 freenit-0.3.3/freenit/app.py
+-rw-r--r--   0        0        0     2898 2020-02-02 00:00:00.000000 freenit-0.3.3/freenit/auth.py
+-rw-r--r--   0        0        0     3207 2020-02-02 00:00:00.000000 freenit-0.3.3/freenit/base_config.py
+-rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 freenit-0.3.3/freenit/cli.py
+-rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 freenit-0.3.3/freenit/config.py
+-rw-r--r--   0        0        0     2087 2020-02-02 00:00:00.000000 freenit-0.3.3/freenit/decorators.py
+-rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 freenit-0.3.3/freenit/mail.py
+-rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 freenit-0.3.3/freenit/migration.py
+-rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 freenit-0.3.3/freenit/permissions.py
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 freenit-0.3.3/freenit/api/__init__.py
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 freenit-0.3.3/freenit/api/router.py
+-rw-r--r--   0        0        0     2656 2020-02-02 00:00:00.000000 freenit-0.3.3/freenit/api/theme.py
+-rw-r--r--   0        0        0     3221 2020-02-02 00:00:00.000000 freenit-0.3.3/freenit/api/auth/__init__.py
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 freenit-0.3.3/freenit/api/role/__init__.py
+-rw-r--r--   0        0        0     2913 2020-02-02 00:00:00.000000 freenit-0.3.3/freenit/api/role/ldap.py
+-rw-r--r--   0        0        0     3670 2020-02-02 00:00:00.000000 freenit-0.3.3/freenit/api/role/sql.py
+-rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 freenit-0.3.3/freenit/api/user/__init__.py
+-rw-r--r--   0        0        0     3154 2020-02-02 00:00:00.000000 freenit-0.3.3/freenit/api/user/ldap.py
+-rw-r--r--   0        0        0     2450 2020-02-02 00:00:00.000000 freenit-0.3.3/freenit/api/user/sql.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 freenit-0.3.3/freenit/models/__init__.py
+-rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 freenit-0.3.3/freenit/models/pagination.py
+-rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 freenit-0.3.3/freenit/models/role.py
+-rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 freenit-0.3.3/freenit/models/safe.py
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 freenit-0.3.3/freenit/models/theme.py
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 freenit-0.3.3/freenit/models/user.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 freenit-0.3.3/freenit/models/ldap/__init__.py
+-rw-r--r--   0        0        0     3025 2020-02-02 00:00:00.000000 freenit-0.3.3/freenit/models/ldap/base.py
+-rw-r--r--   0        0        0     4166 2020-02-02 00:00:00.000000 freenit-0.3.3/freenit/models/ldap/role.py
+-rw-r--r--   0        0        0     3966 2020-02-02 00:00:00.000000 freenit-0.3.3/freenit/models/ldap/user.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 freenit-0.3.3/freenit/models/sql/__init__.py
+-rw-r--r--   0        0        0     1111 2020-02-02 00:00:00.000000 freenit-0.3.3/freenit/models/sql/base.py
+-rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 freenit-0.3.3/freenit/models/sql/role.py
+-rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 freenit-0.3.3/freenit/models/sql/theme.py
+-rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 freenit-0.3.3/freenit/models/sql/user.py
+-rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 freenit-0.3.3/freenit/project/.gitignore
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 freenit-0.3.3/freenit/project/LICENSE
+-rw-r--r--   0        0        0     2154 2020-02-02 00:00:00.000000 freenit-0.3.3/freenit/project/alembic.ini
+-rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 freenit-0.3.3/freenit/project/main.py
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 freenit-0.3.3/freenit/project/provisioners.mk
+-rw-r--r--   0        0        0      879 2020-02-02 00:00:00.000000 freenit-0.3.3/freenit/project/pyproject.toml
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 freenit-0.3.3/freenit/project/requirements.yml
+-rw-r--r--   0        0        0     1301 2020-02-02 00:00:00.000000 freenit-0.3.3/freenit/project/setup.py
+-rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 freenit-0.3.3/freenit/project/alembic/script.py.mako
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 freenit-0.3.3/freenit/project/ansible/group_vars/.keep
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 freenit-0.3.3/freenit/project/ansible/inventory/.keep
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 freenit-0.3.3/freenit/project/ansible/roles/devel/tasks/main.yml
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 freenit-0.3.3/freenit/project/ansible/roles/devel/vars/main.yml
+-rw-r--r--   0        0        0      928 2020-02-02 00:00:00.000000 freenit-0.3.3/freenit/project/bin/common.sh
+-rwxr-xr-x   0        0        0      309 2020-02-02 00:00:00.000000 freenit-0.3.3/freenit/project/bin/devel.sh
+-rwxr-xr-x   0        0        0       95 2020-02-02 00:00:00.000000 freenit-0.3.3/freenit/project/bin/init.sh
+-rwxr-xr-x   0        0        0       99 2020-02-02 00:00:00.000000 freenit-0.3.3/freenit/project/bin/test.sh
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 freenit-0.3.3/freenit/project/project/__init__.py
+-rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 freenit-0.3.3/freenit/project/project/app.py
+-rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 freenit-0.3.3/freenit/project/project/base_config.py
+-rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 freenit-0.3.3/freenit/project/project/config.py
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 freenit-0.3.3/freenit/project/project/api/__init__.py
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 freenit-0.3.3/freenit/project/project/api/router.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 freenit-0.3.3/freenit/project/project/models/__init__.py
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 freenit-0.3.3/freenit/project/templates/site.yml.tpl
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 freenit-0.3.3/freenit/project/tests/__init__.py
+-rw-r--r--   0        0        0     1318 2020-02-02 00:00:00.000000 freenit-0.3.3/freenit/project/tests/client.py
+-rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 freenit-0.3.3/freenit/project/tests/conftest.py
+-rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 freenit-0.3.3/freenit/project/tests/factories.py
+-rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 freenit-0.3.3/freenit/project/tests/test_user.py
+-rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 freenit-0.3.3/templates/site.yml.tpl
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 freenit-0.3.3/tests/__init__.py
+-rw-r--r--   0        0        0     1185 2020-02-02 00:00:00.000000 freenit-0.3.3/tests/client.py
+-rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 freenit-0.3.3/tests/conftest.py
+-rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 freenit-0.3.3/tests/factories.py
+-rw-r--r--   0        0        0      787 2020-02-02 00:00:00.000000 freenit-0.3.3/tests/test_auth.py
+-rw-r--r--   0        0        0     2157 2020-02-02 00:00:00.000000 freenit-0.3.3/tests/test_permission.py
+-rw-r--r--   0        0        0     2281 2020-02-02 00:00:00.000000 freenit-0.3.3/tests/test_role.py
+-rw-r--r--   0        0        0     1944 2020-02-02 00:00:00.000000 freenit-0.3.3/tests/test_user.py
+-rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 freenit-0.3.3/.gitignore
+-rw-r--r--   0        0        0     1322 2020-02-02 00:00:00.000000 freenit-0.3.3/LICENSE
+-rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 freenit-0.3.3/README.md
+-rw-r--r--   0        0        0     1548 2020-02-02 00:00:00.000000 freenit-0.3.3/pyproject.toml
+-rw-r--r--   0        0        0     3845 2020-02-02 00:00:00.000000 freenit-0.3.3/PKG-INFO
```

### Comparing `freenit-0.3.2/alembic.ini` & `freenit-0.3.3/alembic.ini`

 * *Files identical despite different names*

### Comparing `freenit-0.3.2/setup.py` & `freenit-0.3.3/setup.py`

 * *Files identical despite different names*

### Comparing `freenit-0.3.2/alembic/versions/06a043f2516a_initial.py` & `freenit-0.3.3/alembic/versions/06a043f2516a_initial.py`

 * *Files identical despite different names*

### Comparing `freenit-0.3.2/bin/common.sh` & `freenit-0.3.3/bin/common.sh`

 * *Files identical despite different names*

### Comparing `freenit-0.3.2/bin/freenit.sh` & `freenit-0.3.3/bin/freenit.sh`

 * *Files identical despite different names*

### Comparing `freenit-0.3.2/freenit/auth.py` & `freenit-0.3.3/freenit/auth.py`

 * *Files identical despite different names*

### Comparing `freenit-0.3.2/freenit/base_config.py` & `freenit-0.3.3/freenit/base_config.py`

 * *Files 9% similar despite different names*

```diff
@@ -34,23 +34,27 @@
         user="user@example.com",
         password="Sekrit",  # nosec
         port=587,
         tls=True,
         from_addr="no-reply@mail.com",
         register_subject="[Freenit] User Registration",
         register_message=register_message,
+        master_user="dovecot@example.com",
+        master_pw="Sekrit",
     ) -> None:
         self.server = server
         self.user = user
         self.password = password
         self.port = port
         self.tls = tls
         self.from_addr = from_addr
         self.register_subject = register_subject
         self.register_message = register_message
+        self.master_user = master_user
+        self.master_pw = master_pw
 
 
 class LDAP:
     def __init__(
         self,
         host="ldap.example.com",
         tls=True,
```

### Comparing `freenit-0.3.2/freenit/config.py` & `freenit-0.3.3/freenit/config.py`

 * *Files identical despite different names*

### Comparing `freenit-0.3.2/freenit/decorators.py` & `freenit-0.3.3/freenit/decorators.py`

 * *Files identical despite different names*

### Comparing `freenit-0.3.2/freenit/migration.py` & `freenit-0.3.3/freenit/migration.py`

 * *Files identical despite different names*

### Comparing `freenit-0.3.2/freenit/api/theme.py` & `freenit-0.3.3/freenit/api/theme.py`

 * *Files identical despite different names*

### Comparing `freenit-0.3.2/freenit/api/auth/__init__.py` & `freenit-0.3.3/freenit/api/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `freenit-0.3.2/freenit/api/role/ldap.py` & `freenit-0.3.3/freenit/api/role/ldap.py`

 * *Files identical despite different names*

### Comparing `freenit-0.3.2/freenit/api/role/sql.py` & `freenit-0.3.3/freenit/api/role/sql.py`

 * *Files identical despite different names*

### Comparing `freenit-0.3.2/freenit/api/user/ldap.py` & `freenit-0.3.3/freenit/api/user/ldap.py`

 * *Files identical despite different names*

### Comparing `freenit-0.3.2/freenit/api/user/sql.py` & `freenit-0.3.3/freenit/api/user/sql.py`

 * *Files identical despite different names*

### Comparing `freenit-0.3.2/freenit/models/pagination.py` & `freenit-0.3.3/freenit/models/pagination.py`

 * *Files identical despite different names*

### Comparing `freenit-0.3.2/freenit/models/ldap/base.py` & `freenit-0.3.3/freenit/models/ldap/base.py`

 * *Files identical despite different names*

### Comparing `freenit-0.3.2/freenit/models/ldap/role.py` & `freenit-0.3.3/freenit/models/ldap/role.py`

 * *Files identical despite different names*

### Comparing `freenit-0.3.2/freenit/models/ldap/user.py` & `freenit-0.3.3/freenit/models/ldap/user.py`

 * *Files identical despite different names*

### Comparing `freenit-0.3.2/freenit/models/sql/base.py` & `freenit-0.3.3/freenit/models/sql/base.py`

 * *Files identical despite different names*

### Comparing `freenit-0.3.2/freenit/models/sql/theme.py` & `freenit-0.3.3/freenit/models/sql/theme.py`

 * *Files identical despite different names*

### Comparing `freenit-0.3.2/freenit/models/sql/user.py` & `freenit-0.3.3/freenit/models/sql/user.py`

 * *Files identical despite different names*

### Comparing `freenit-0.3.2/freenit/project/alembic.ini` & `freenit-0.3.3/freenit/project/alembic.ini`

 * *Files identical despite different names*

### Comparing `freenit-0.3.2/freenit/project/pyproject.toml` & `freenit-0.3.3/freenit/project/pyproject.toml`

 * *Files identical despite different names*

### Comparing `freenit-0.3.2/freenit/project/setup.py` & `freenit-0.3.3/freenit/project/setup.py`

 * *Files identical despite different names*

### Comparing `freenit-0.3.2/freenit/project/bin/common.sh` & `freenit-0.3.3/freenit/project/bin/common.sh`

 * *Files identical despite different names*

### Comparing `freenit-0.3.2/freenit/project/project/config.py` & `freenit-0.3.3/freenit/project/project/config.py`

 * *Files identical despite different names*

### Comparing `freenit-0.3.2/freenit/project/tests/client.py` & `freenit-0.3.3/freenit/project/tests/client.py`

 * *Files identical despite different names*

### Comparing `freenit-0.3.2/freenit/project/tests/conftest.py` & `freenit-0.3.3/freenit/project/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `freenit-0.3.2/freenit/project/tests/factories.py` & `freenit-0.3.3/freenit/project/tests/factories.py`

 * *Files identical despite different names*

### Comparing `freenit-0.3.2/tests/client.py` & `freenit-0.3.3/tests/client.py`

 * *Files identical despite different names*

### Comparing `freenit-0.3.2/tests/conftest.py` & `freenit-0.3.3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `freenit-0.3.2/tests/factories.py` & `freenit-0.3.3/tests/factories.py`

 * *Files identical despite different names*

### Comparing `freenit-0.3.2/tests/test_auth.py` & `freenit-0.3.3/tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `freenit-0.3.2/tests/test_permission.py` & `freenit-0.3.3/tests/test_permission.py`

 * *Files identical despite different names*

### Comparing `freenit-0.3.2/tests/test_role.py` & `freenit-0.3.3/tests/test_role.py`

 * *Files identical despite different names*

### Comparing `freenit-0.3.2/tests/test_user.py` & `freenit-0.3.3/tests/test_user.py`

 * *Files identical despite different names*

### Comparing `freenit-0.3.2/LICENSE` & `freenit-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `freenit-0.3.2/pyproject.toml` & `freenit-0.3.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `freenit-0.3.2/PKG-INFO` & `freenit-0.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: freenit
-Version: 0.3.2
+Version: 0.3.3
 Summary: REST API framework based on FastAPI
 Project-URL: Homepage, https://freenit.org
 Project-URL: Repository, https://github.com/freenit-framework/backend
 Author-email: Goran Mekić <meka@tilda.center>
 License: BSD 2-Clause License
         
         Copyright (c) 2021, Goran Mekić
```

