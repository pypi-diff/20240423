# Comparing `tmp/invenio-alma-0.9.0.tar.gz` & `tmp/invenio-alma-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "invenio-alma-0.9.0.tar", last modified: Fri May 26 09:10:31 2023, max compression
+gzip compressed data, was "invenio-alma-0.9.1.tar", last modified: Fri May 26 12:13:20 2023, max compression
```

## Comparing `invenio-alma-0.9.0.tar` & `invenio-alma-0.9.1.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:10:31.776546 invenio-alma-0.9.0/
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-26 09:10:22.000000 invenio-alma-0.9.0/.dockerignore
--rw-r--r--   0 runner    (1001) docker     (123)      823 2023-05-26 09:10:22.000000 invenio-alma-0.9.0/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-05-26 09:10:22.000000 invenio-alma-0.9.0/.ruff.toml
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-05-26 09:10:22.000000 invenio-alma-0.9.0/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3002 2023-05-26 09:10:22.000000 invenio-alma-0.9.0/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3502 2023-05-26 09:10:22.000000 invenio-alma-0.9.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-26 09:10:22.000000 invenio-alma-0.9.0/INSTALL.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-05-26 09:10:22.000000 invenio-alma-0.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-05-26 09:10:22.000000 invenio-alma-0.9.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4553 2023-05-26 09:10:31.776546 invenio-alma-0.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      992 2023-05-26 09:10:22.000000 invenio-alma-0.9.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:10:31.772546 invenio-alma-0.9.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     7433 2023-05-26 09:10:22.000000 invenio-alma-0.9.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-05-26 09:10:22.000000 invenio-alma-0.9.0/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-05-26 09:10:22.000000 invenio-alma-0.9.0/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-05-26 09:10:22.000000 invenio-alma-0.9.0/docs/changes.rst
--rw-r--r--   0 runner    (1001) docker     (123)    10422 2023-05-26 09:10:22.000000 invenio-alma-0.9.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-05-26 09:10:22.000000 invenio-alma-0.9.0/docs/configuration.rst
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-05-26 09:10:22.000000 invenio-alma-0.9.0/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      816 2023-05-26 09:10:22.000000 invenio-alma-0.9.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-05-26 09:10:22.000000 invenio-alma-0.9.0/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-05-26 09:10:22.000000 invenio-alma-0.9.0/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6993 2023-05-26 09:10:22.000000 invenio-alma-0.9.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-26 09:10:22.000000 invenio-alma-0.9.0/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-05-26 09:10:22.000000 invenio-alma-0.9.0/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:10:31.772546 invenio-alma-0.9.0/invenio_alma/
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-05-26 09:10:22.000000 invenio-alma-0.9.0/invenio_alma/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4594 2023-05-26 09:10:22.000000 invenio-alma-0.9.0/invenio_alma/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6923 2023-05-26 09:10:22.000000 invenio-alma-0.9.0/invenio_alma/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-05-26 09:10:22.000000 invenio-alma-0.9.0/invenio_alma/click_param_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-05-26 09:10:22.000000 invenio-alma-0.9.0/invenio_alma/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-05-26 09:10:22.000000 invenio-alma-0.9.0/invenio_alma/ext.py
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-05-26 09:10:22.000000 invenio-alma-0.9.0/invenio_alma/proxies.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:10:31.772546 invenio-alma-0.9.0/invenio_alma/resources/
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-05-26 09:10:22.000000 invenio-alma-0.9.0/invenio_alma/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-05-26 09:10:22.000000 invenio-alma-0.9.0/invenio_alma/resources/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-05-26 09:10:22.000000 invenio-alma-0.9.0/invenio_alma/resources/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:10:31.776546 invenio-alma-0.9.0/invenio_alma/services/
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-05-26 09:10:22.000000 invenio-alma-0.9.0/invenio_alma/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2329 2023-05-26 09:10:22.000000 invenio-alma-0.9.0/invenio_alma/services/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-05-26 09:10:22.000000 invenio-alma-0.9.0/invenio_alma/services/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      935 2023-05-26 09:10:22.000000 invenio-alma-0.9.0/invenio_alma/services/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     5997 2023-05-26 09:10:22.000000 invenio-alma-0.9.0/invenio_alma/services/rest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2420 2023-05-26 09:10:22.000000 invenio-alma-0.9.0/invenio_alma/services/sru.py
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-05-26 09:10:22.000000 invenio-alma-0.9.0/invenio_alma/services/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2885 2023-05-26 09:10:22.000000 invenio-alma-0.9.0/invenio_alma/tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-05-26 09:10:22.000000 invenio-alma-0.9.0/invenio_alma/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-05-26 09:10:22.000000 invenio-alma-0.9.0/invenio_alma/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:10:31.772546 invenio-alma-0.9.0/invenio_alma.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4553 2023-05-26 09:10:31.000000 invenio-alma-0.9.0/invenio_alma.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-05-26 09:10:31.000000 invenio-alma-0.9.0/invenio_alma.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 09:10:31.000000 invenio-alma-0.9.0/invenio_alma.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-05-26 09:10:31.000000 invenio-alma-0.9.0/invenio_alma.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 09:10:31.000000 invenio-alma-0.9.0/invenio_alma.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-05-26 09:10:31.000000 invenio-alma-0.9.0/invenio_alma.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-26 09:10:31.000000 invenio-alma-0.9.0/invenio_alma.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-26 09:10:22.000000 invenio-alma-0.9.0/pyproject.toml
--rwxr-xr-x   0 runner    (1001) docker     (123)      527 2023-05-26 09:10:22.000000 invenio-alma-0.9.0/run-tests.sh
--rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-05-26 09:10:31.776546 invenio-alma-0.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-05-26 09:10:22.000000 invenio-alma-0.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:10:31.776546 invenio-alma-0.9.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      986 2023-05-26 09:10:22.000000 invenio-alma-0.9.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-05-26 09:10:22.000000 invenio-alma-0.9.0/tests/test_invenio_alma.py
--rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-05-26 09:10:22.000000 invenio-alma-0.9.0/tests/test_invenio_alma_service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:13:20.520159 invenio-alma-0.9.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-26 12:13:15.000000 invenio-alma-0.9.1/.dockerignore
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-05-26 12:13:15.000000 invenio-alma-0.9.1/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-05-26 12:13:15.000000 invenio-alma-0.9.1/.ruff.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-05-26 12:13:15.000000 invenio-alma-0.9.1/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3072 2023-05-26 12:13:15.000000 invenio-alma-0.9.1/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3502 2023-05-26 12:13:15.000000 invenio-alma-0.9.1/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-26 12:13:15.000000 invenio-alma-0.9.1/INSTALL.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-05-26 12:13:15.000000 invenio-alma-0.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-05-26 12:13:15.000000 invenio-alma-0.9.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4623 2023-05-26 12:13:20.520159 invenio-alma-0.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      992 2023-05-26 12:13:15.000000 invenio-alma-0.9.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:13:20.516159 invenio-alma-0.9.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     7433 2023-05-26 12:13:15.000000 invenio-alma-0.9.1/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-05-26 12:13:15.000000 invenio-alma-0.9.1/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-05-26 12:13:15.000000 invenio-alma-0.9.1/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-05-26 12:13:15.000000 invenio-alma-0.9.1/docs/changes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10422 2023-05-26 12:13:15.000000 invenio-alma-0.9.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-05-26 12:13:15.000000 invenio-alma-0.9.1/docs/configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-05-26 12:13:15.000000 invenio-alma-0.9.1/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-05-26 12:13:15.000000 invenio-alma-0.9.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-05-26 12:13:15.000000 invenio-alma-0.9.1/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-05-26 12:13:15.000000 invenio-alma-0.9.1/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6993 2023-05-26 12:13:15.000000 invenio-alma-0.9.1/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-26 12:13:15.000000 invenio-alma-0.9.1/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-05-26 12:13:15.000000 invenio-alma-0.9.1/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:13:20.520159 invenio-alma-0.9.1/invenio_alma/
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-05-26 12:13:15.000000 invenio-alma-0.9.1/invenio_alma/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4594 2023-05-26 12:13:15.000000 invenio-alma-0.9.1/invenio_alma/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7070 2023-05-26 12:13:15.000000 invenio-alma-0.9.1/invenio_alma/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-05-26 12:13:15.000000 invenio-alma-0.9.1/invenio_alma/click_param_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-05-26 12:13:15.000000 invenio-alma-0.9.1/invenio_alma/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-05-26 12:13:15.000000 invenio-alma-0.9.1/invenio_alma/ext.py
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-05-26 12:13:15.000000 invenio-alma-0.9.1/invenio_alma/proxies.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:13:20.520159 invenio-alma-0.9.1/invenio_alma/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-05-26 12:13:15.000000 invenio-alma-0.9.1/invenio_alma/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-05-26 12:13:15.000000 invenio-alma-0.9.1/invenio_alma/resources/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-05-26 12:13:15.000000 invenio-alma-0.9.1/invenio_alma/resources/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:13:20.520159 invenio-alma-0.9.1/invenio_alma/services/
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-05-26 12:13:15.000000 invenio-alma-0.9.1/invenio_alma/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2329 2023-05-26 12:13:15.000000 invenio-alma-0.9.1/invenio_alma/services/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-05-26 12:13:15.000000 invenio-alma-0.9.1/invenio_alma/services/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-05-26 12:13:15.000000 invenio-alma-0.9.1/invenio_alma/services/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5997 2023-05-26 12:13:15.000000 invenio-alma-0.9.1/invenio_alma/services/rest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2420 2023-05-26 12:13:15.000000 invenio-alma-0.9.1/invenio_alma/services/sru.py
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-05-26 12:13:15.000000 invenio-alma-0.9.1/invenio_alma/services/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2885 2023-05-26 12:13:15.000000 invenio-alma-0.9.1/invenio_alma/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-05-26 12:13:15.000000 invenio-alma-0.9.1/invenio_alma/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-05-26 12:13:15.000000 invenio-alma-0.9.1/invenio_alma/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:13:20.520159 invenio-alma-0.9.1/invenio_alma.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4623 2023-05-26 12:13:20.000000 invenio-alma-0.9.1/invenio_alma.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-05-26 12:13:20.000000 invenio-alma-0.9.1/invenio_alma.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 12:13:20.000000 invenio-alma-0.9.1/invenio_alma.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-05-26 12:13:20.000000 invenio-alma-0.9.1/invenio_alma.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 12:13:20.000000 invenio-alma-0.9.1/invenio_alma.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-05-26 12:13:20.000000 invenio-alma-0.9.1/invenio_alma.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-26 12:13:20.000000 invenio-alma-0.9.1/invenio_alma.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-26 12:13:15.000000 invenio-alma-0.9.1/pyproject.toml
+-rwxr-xr-x   0 runner    (1001) docker     (123)      527 2023-05-26 12:13:15.000000 invenio-alma-0.9.1/run-tests.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-05-26 12:13:20.520159 invenio-alma-0.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-05-26 12:13:15.000000 invenio-alma-0.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:13:20.520159 invenio-alma-0.9.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-05-26 12:13:15.000000 invenio-alma-0.9.1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-05-26 12:13:15.000000 invenio-alma-0.9.1/tests/test_invenio_alma.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-05-26 12:13:15.000000 invenio-alma-0.9.1/tests/test_invenio_alma_service.py
```

### Comparing `invenio-alma-0.9.0/.editorconfig` & `invenio-alma-0.9.1/.editorconfig`

 * *Files identical despite different names*

### Comparing `invenio-alma-0.9.0/CHANGES.rst` & `invenio-alma-0.9.1/CHANGES.rst`

 * *Files 4% similar despite different names*

```diff
@@ -3,14 +3,19 @@
 
     invenio-alma is free software; you can redistribute it and/or modify it
     under the terms of the MIT License; see LICENSE file for more details.
 
 Changes
 =======
 
+Version v0.9.1 (release 2023-05-26)
+
+- fix: changed api not applied
+
+
 Version v0.9.0 (release 2023-05-26)
 
 - ruff: add to ignore
 - cli: make update func customizable
 
 
 Version v0.8.2 (release 2023-05-01)
```

### Comparing `invenio-alma-0.9.0/CONTRIBUTING.rst` & `invenio-alma-0.9.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `invenio-alma-0.9.0/LICENSE` & `invenio-alma-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `invenio-alma-0.9.0/MANIFEST.in` & `invenio-alma-0.9.1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `invenio-alma-0.9.0/PKG-INFO` & `invenio-alma-0.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invenio-alma
-Version: 0.9.0
+Version: 0.9.1
 Summary: "Provides API for Alma."
 Home-page: https://github.com/tu-graz-library/invenio-alma
 Author: Graz University of Technology.
 Author-email: info@inveniosoftware.org
 License: MIT
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
@@ -48,14 +48,19 @@
 
     invenio-alma is free software; you can redistribute it and/or modify it
     under the terms of the MIT License; see LICENSE file for more details.
 
 Changes
 =======
 
+Version v0.9.1 (release 2023-05-26)
+
+- fix: changed api not applied
+
+
 Version v0.9.0 (release 2023-05-26)
 
 - ruff: add to ignore
 - cli: make update func customizable
 
 
 Version v0.8.2 (release 2023-05-01)
```

### Comparing `invenio-alma-0.9.0/README.rst` & `invenio-alma-0.9.1/README.rst`

 * *Files identical despite different names*

### Comparing `invenio-alma-0.9.0/docs/Makefile` & `invenio-alma-0.9.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `invenio-alma-0.9.0/docs/conf.py` & `invenio-alma-0.9.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `invenio-alma-0.9.0/docs/index.rst` & `invenio-alma-0.9.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `invenio-alma-0.9.0/docs/make.bat` & `invenio-alma-0.9.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `invenio-alma-0.9.0/invenio_alma/api.py` & `invenio-alma-0.9.1/invenio_alma/api.py`

 * *Files identical despite different names*

### Comparing `invenio-alma-0.9.0/invenio_alma/cli.py` & `invenio-alma-0.9.1/invenio_alma/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,26 +70,32 @@
 
 
 @create.command("alma-record")
 @with_appcontext
 @click.option("--marc-id", type=click.STRING, required=True)
 @click.option("--user-email", type=click.STRING, default="alma@tugraz.at")
 @click.option("--api-key", type=click.STRING, required=True)
+@click.option("--api-host", type=click.STRING, required=True)
 @click.option("--cms-id", type=click.STRING, required=True)
 def cli_create_alma_record(
     marc_id: str,
     user_email: str,
     api_key: str,
+    api_host: str,
     cms_id: str,
 ) -> None:
     """Create alma record."""
-    records_service, alma_service, identity = preliminaries(user_email, use_rest=True)
-
-    alma_service.config.api_key = api_key
+    config = AlmaRESTConfig(api_key, api_host)
 
+    records_service, alma_service, identity = preliminaries(
+        user_email,
+        config,
+        use_rest=True,
+        use_sru=False,
+    )
     create_alma_record(records_service, alma_service, identity, marc_id, cms_id)
 
 
 @create.command("repository-record")
 @click.option("--mms-id", type=click.STRING, required=True)
 def create_repository_record(mms_id: str) -> None:  # noqa: ARG001
     """Create repository record."""
```

### Comparing `invenio-alma-0.9.0/invenio_alma/click_param_type.py` & `invenio-alma-0.9.1/invenio_alma/click_param_type.py`

 * *Files identical despite different names*

### Comparing `invenio-alma-0.9.0/invenio_alma/config.py` & `invenio-alma-0.9.1/invenio_alma/config.py`

 * *Files identical despite different names*

### Comparing `invenio-alma-0.9.0/invenio_alma/ext.py` & `invenio-alma-0.9.1/invenio_alma/ext.py`

 * *Files identical despite different names*

### Comparing `invenio-alma-0.9.0/invenio_alma/resources/config.py` & `invenio-alma-0.9.1/invenio_alma/resources/config.py`

 * *Files identical despite different names*

### Comparing `invenio-alma-0.9.0/invenio_alma/resources/resources.py` & `invenio-alma-0.9.1/invenio_alma/resources/resources.py`

 * *Files identical despite different names*

### Comparing `invenio-alma-0.9.0/invenio_alma/services/base.py` & `invenio-alma-0.9.1/invenio_alma/services/base.py`

 * *Files identical despite different names*

### Comparing `invenio-alma-0.9.0/invenio_alma/services/config.py` & `invenio-alma-0.9.1/invenio_alma/services/config.py`

 * *Files identical despite different names*

### Comparing `invenio-alma-0.9.0/invenio_alma/services/errors.py` & `invenio-alma-0.9.1/invenio_alma/services/errors.py`

 * *Files identical despite different names*

### Comparing `invenio-alma-0.9.0/invenio_alma/services/rest.py` & `invenio-alma-0.9.1/invenio_alma/services/rest.py`

 * *Files identical despite different names*

### Comparing `invenio-alma-0.9.0/invenio_alma/services/sru.py` & `invenio-alma-0.9.1/invenio_alma/services/sru.py`

 * *Files identical despite different names*

### Comparing `invenio-alma-0.9.0/invenio_alma/tasks.py` & `invenio-alma-0.9.1/invenio_alma/tasks.py`

 * *Files identical despite different names*

### Comparing `invenio-alma-0.9.0/invenio_alma/utils.py` & `invenio-alma-0.9.1/invenio_alma/utils.py`

 * *Files identical despite different names*

### Comparing `invenio-alma-0.9.0/invenio_alma/views.py` & `invenio-alma-0.9.1/invenio_alma/views.py`

 * *Files identical despite different names*

### Comparing `invenio-alma-0.9.0/invenio_alma.egg-info/PKG-INFO` & `invenio-alma-0.9.1/invenio_alma.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invenio-alma
-Version: 0.9.0
+Version: 0.9.1
 Summary: "Provides API for Alma."
 Home-page: https://github.com/tu-graz-library/invenio-alma
 Author: Graz University of Technology.
 Author-email: info@inveniosoftware.org
 License: MIT
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
@@ -48,14 +48,19 @@
 
     invenio-alma is free software; you can redistribute it and/or modify it
     under the terms of the MIT License; see LICENSE file for more details.
 
 Changes
 =======
 
+Version v0.9.1 (release 2023-05-26)
+
+- fix: changed api not applied
+
+
 Version v0.9.0 (release 2023-05-26)
 
 - ruff: add to ignore
 - cli: make update func customizable
 
 
 Version v0.8.2 (release 2023-05-01)
```

### Comparing `invenio-alma-0.9.0/invenio_alma.egg-info/SOURCES.txt` & `invenio-alma-0.9.1/invenio_alma.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `invenio-alma-0.9.0/run-tests.sh` & `invenio-alma-0.9.1/run-tests.sh`

 * *Files identical despite different names*

### Comparing `invenio-alma-0.9.0/setup.cfg` & `invenio-alma-0.9.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `invenio-alma-0.9.0/tests/conftest.py` & `invenio-alma-0.9.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `invenio-alma-0.9.0/tests/test_invenio_alma.py` & `invenio-alma-0.9.1/tests/test_invenio_alma.py`

 * *Files identical despite different names*

### Comparing `invenio-alma-0.9.0/tests/test_invenio_alma_service.py` & `invenio-alma-0.9.1/tests/test_invenio_alma_service.py`

 * *Files identical despite different names*

