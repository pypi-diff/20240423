# Comparing `tmp/lsst-rsp-0.5.1.tar.gz` & `tmp/lsst_rsp-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lsst-rsp-0.5.1.tar", last modified: Thu Apr 11 20:19:44 2024, max compression
+gzip compressed data, was "lsst_rsp-0.5.2.tar", last modified: Mon Apr 22 23:47:58 2024, max compression
```

## Comparing `lsst-rsp-0.5.1.tar` & `lsst_rsp-0.5.2.tar`

### file list

```diff
@@ -1,78 +1,78 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:19:44.649178 lsst-rsp-0.5.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:19:44.641178 lsst-rsp-0.5.1/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-11 20:19:39.000000 lsst-rsp-0.5.1/.github/CODE_OF_CONDUCT
--rw-r--r--   0 runner    (1001) docker     (127)      675 2024-04-11 20:19:39.000000 lsst-rsp-0.5.1/.github/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-04-11 20:19:39.000000 lsst-rsp-0.5.1/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:19:44.641178 lsst-rsp-0.5.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2260 2024-04-11 20:19:39.000000 lsst-rsp-0.5.1/.github/workflows/ci.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      995 2024-04-11 20:19:39.000000 lsst-rsp-0.5.1/.github/workflows/periodic-ci.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1836 2024-04-11 20:19:39.000000 lsst-rsp-0.5.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      528 2024-04-11 20:19:39.000000 lsst-rsp-0.5.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      649 2024-04-11 20:19:39.000000 lsst-rsp-0.5.1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-04-11 20:19:39.000000 lsst-rsp-0.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 20:19:39.000000 lsst-rsp-0.5.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      374 2024-04-11 20:19:39.000000 lsst-rsp-0.5.1/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     5444 2024-04-11 20:19:44.649178 lsst-rsp-0.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2814 2024-04-11 20:19:39.000000 lsst-rsp-0.5.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:19:44.641178 lsst-rsp-0.5.1/changelog.d/
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-11 20:19:39.000000 lsst-rsp-0.5.1/changelog.d/_template.md.jinja
--rw-r--r--   0 runner    (1001) docker     (127)     8309 2024-04-11 20:19:39.000000 lsst-rsp-0.5.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 20:19:44.649178 lsst-rsp-0.5.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:19:44.637178 lsst-rsp-0.5.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:19:44.641178 lsst-rsp-0.5.1/src/lsst/
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-11 20:19:39.000000 lsst-rsp-0.5.1/src/lsst/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:19:44.641178 lsst-rsp-0.5.1/src/lsst/rsp/
--rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-04-11 20:19:39.000000 lsst-rsp-0.5.1/src/lsst/rsp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2438 2024-04-11 20:19:39.000000 lsst-rsp-0.5.1/src/lsst/rsp/catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     3496 2024-04-11 20:19:39.000000 lsst-rsp-0.5.1/src/lsst/rsp/log.py
--rw-r--r--   0 runner    (1001) docker     (127)      800 2024-04-11 20:19:39.000000 lsst-rsp-0.5.1/src/lsst/rsp/service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:19:44.645178 lsst-rsp-0.5.1/src/lsst/rsp/startup/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 20:19:39.000000 lsst-rsp-0.5.1/src/lsst/rsp/startup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-04-11 20:19:39.000000 lsst-rsp-0.5.1/src/lsst/rsp/startup/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-04-11 20:19:39.000000 lsst-rsp-0.5.1/src/lsst/rsp/startup/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-04-11 20:19:39.000000 lsst-rsp-0.5.1/src/lsst/rsp/startup/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:19:44.645178 lsst-rsp-0.5.1/src/lsst/rsp/startup/models/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 20:19:39.000000 lsst-rsp-0.5.1/src/lsst/rsp/startup/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-04-11 20:19:39.000000 lsst-rsp-0.5.1/src/lsst/rsp/startup/models/noninteractive.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:19:44.645178 lsst-rsp-0.5.1/src/lsst/rsp/startup/services/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 20:19:39.000000 lsst-rsp-0.5.1/src/lsst/rsp/startup/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    27724 2024-04-11 20:19:39.000000 lsst-rsp-0.5.1/src/lsst/rsp/startup/services/labrunner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:19:44.645178 lsst-rsp-0.5.1/src/lsst/rsp/startup/storage/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 20:19:39.000000 lsst-rsp-0.5.1/src/lsst/rsp/startup/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4717 2024-04-11 20:19:39.000000 lsst-rsp-0.5.1/src/lsst/rsp/startup/storage/command.py
--rw-r--r--   0 runner    (1001) docker     (127)     3067 2024-04-11 20:19:39.000000 lsst-rsp-0.5.1/src/lsst/rsp/startup/storage/logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     5240 2024-04-11 20:19:39.000000 lsst-rsp-0.5.1/src/lsst/rsp/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:19:44.649178 lsst-rsp-0.5.1/src/lsst_rsp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5444 2024-04-11 20:19:44.000000 lsst-rsp-0.5.1/src/lsst_rsp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1669 2024-04-11 20:19:44.000000 lsst-rsp-0.5.1/src/lsst_rsp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 20:19:44.000000 lsst-rsp-0.5.1/src/lsst_rsp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-11 20:19:44.000000 lsst-rsp-0.5.1/src/lsst_rsp.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-04-11 20:19:44.000000 lsst-rsp-0.5.1/src/lsst_rsp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-11 20:19:44.000000 lsst-rsp-0.5.1/src/lsst_rsp.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:19:44.645178 lsst-rsp-0.5.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-11 20:19:39.000000 lsst-rsp-0.5.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2379 2024-04-11 20:19:39.000000 lsst-rsp-0.5.1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)    10807 2024-04-11 20:19:39.000000 lsst-rsp-0.5.1/tests/startup_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:19:44.637178 lsst-rsp-0.5.1/tests/support/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:19:44.645178 lsst-rsp-0.5.1/tests/support/files/
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-11 20:19:39.000000 lsst-rsp-0.5.1/tests/support/files/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:19:44.645178 lsst-rsp-0.5.1/tests/support/files/etc/
--rw-r--r--   0 runner    (1001) docker     (127)    10287 2024-04-11 20:19:39.000000 lsst-rsp-0.5.1/tests/support/files/etc/dircolors.ansi-universal
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:19:44.645178 lsst-rsp-0.5.1/tests/support/files/etc/skel/
--rw-r--r--   0 runner    (1001) docker     (127)      213 2024-04-11 20:19:39.000000 lsst-rsp-0.5.1/tests/support/files/etc/skel/.gitconfig
--rw-r--r--   0 runner    (1001) docker     (127)      359 2024-04-11 20:19:39.000000 lsst-rsp-0.5.1/tests/support/files/etc/skel/.pythonrc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:19:44.645178 lsst-rsp-0.5.1/tests/support/files/etc/skel/notebooks/
--rw-r--r--   0 runner    (1001) docker     (127)      376 2024-04-11 20:19:39.000000 lsst-rsp-0.5.1/tests/support/files/etc/skel/notebooks/.user_setups
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:19:44.637178 lsst-rsp-0.5.1/tests/support/files/homedir/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:19:44.649178 lsst-rsp-0.5.1/tests/support/files/homedir/.lsst/
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-11 20:19:39.000000 lsst-rsp-0.5.1/tests/support/files/homedir/.lsst/aws-credentials.ini
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-11 20:19:39.000000 lsst-rsp-0.5.1/tests/support/files/homedir/.lsst/postgres-credentials.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:19:44.637178 lsst-rsp-0.5.1/tests/support/files/stack_top/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:19:44.649178 lsst-rsp-0.5.1/tests/support/files/stack_top/jupyterlab/
--rw-r--r--   0 runner    (1001) docker     (127)     1833 2024-04-11 20:19:39.000000 lsst-rsp-0.5.1/tests/support/files/stack_top/jupyterlab/20-logging.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:19:44.649178 lsst-rsp-0.5.1/tests/support/files/stack_top/jupyterlab/secrets/
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-11 20:19:39.000000 lsst-rsp-0.5.1/tests/support/files/stack_top/jupyterlab/secrets/aws-credentials.ini
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-11 20:19:39.000000 lsst-rsp-0.5.1/tests/support/files/stack_top/jupyterlab/secrets/postgres-credentials.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-04-11 20:19:39.000000 lsst-rsp-0.5.1/tests/utils_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      297 2024-04-11 20:19:39.000000 lsst-rsp-0.5.1/tests/version_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      644 2024-04-11 20:19:39.000000 lsst-rsp-0.5.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:47:58.076074 lsst_rsp-0.5.2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:47:58.068073 lsst_rsp-0.5.2/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-22 23:47:53.000000 lsst_rsp-0.5.2/.github/CODE_OF_CONDUCT
+-rw-r--r--   0 runner    (1001) docker     (127)      675 2024-04-22 23:47:53.000000 lsst_rsp-0.5.2/.github/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-04-22 23:47:53.000000 lsst_rsp-0.5.2/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:47:58.068073 lsst_rsp-0.5.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2260 2024-04-22 23:47:53.000000 lsst_rsp-0.5.2/.github/workflows/ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      995 2024-04-22 23:47:53.000000 lsst_rsp-0.5.2/.github/workflows/periodic-ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1836 2024-04-22 23:47:53.000000 lsst_rsp-0.5.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      528 2024-04-22 23:47:53.000000 lsst_rsp-0.5.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      794 2024-04-22 23:47:53.000000 lsst_rsp-0.5.2/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-04-22 23:47:53.000000 lsst_rsp-0.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 23:47:53.000000 lsst_rsp-0.5.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-04-22 23:47:53.000000 lsst_rsp-0.5.2/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     5444 2024-04-22 23:47:58.076074 lsst_rsp-0.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2814 2024-04-22 23:47:53.000000 lsst_rsp-0.5.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:47:58.068073 lsst_rsp-0.5.2/changelog.d/
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-22 23:47:53.000000 lsst_rsp-0.5.2/changelog.d/_template.md.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)     8309 2024-04-22 23:47:53.000000 lsst_rsp-0.5.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 23:47:58.076074 lsst_rsp-0.5.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:47:58.064073 lsst_rsp-0.5.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:47:58.068073 lsst_rsp-0.5.2/src/lsst/
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-22 23:47:53.000000 lsst_rsp-0.5.2/src/lsst/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:47:58.072073 lsst_rsp-0.5.2/src/lsst/rsp/
+-rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-04-22 23:47:53.000000 lsst_rsp-0.5.2/src/lsst/rsp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2438 2024-04-22 23:47:53.000000 lsst_rsp-0.5.2/src/lsst/rsp/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3496 2024-04-22 23:47:53.000000 lsst_rsp-0.5.2/src/lsst/rsp/log.py
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2024-04-22 23:47:53.000000 lsst_rsp-0.5.2/src/lsst/rsp/service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:47:58.072073 lsst_rsp-0.5.2/src/lsst/rsp/startup/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 23:47:53.000000 lsst_rsp-0.5.2/src/lsst/rsp/startup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-04-22 23:47:53.000000 lsst_rsp-0.5.2/src/lsst/rsp/startup/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-04-22 23:47:53.000000 lsst_rsp-0.5.2/src/lsst/rsp/startup/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-04-22 23:47:53.000000 lsst_rsp-0.5.2/src/lsst/rsp/startup/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:47:58.072073 lsst_rsp-0.5.2/src/lsst/rsp/startup/models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 23:47:53.000000 lsst_rsp-0.5.2/src/lsst/rsp/startup/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-04-22 23:47:53.000000 lsst_rsp-0.5.2/src/lsst/rsp/startup/models/noninteractive.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:47:58.072073 lsst_rsp-0.5.2/src/lsst/rsp/startup/services/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 23:47:53.000000 lsst_rsp-0.5.2/src/lsst/rsp/startup/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27930 2024-04-22 23:47:53.000000 lsst_rsp-0.5.2/src/lsst/rsp/startup/services/labrunner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:47:58.072073 lsst_rsp-0.5.2/src/lsst/rsp/startup/storage/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 23:47:53.000000 lsst_rsp-0.5.2/src/lsst/rsp/startup/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4717 2024-04-22 23:47:53.000000 lsst_rsp-0.5.2/src/lsst/rsp/startup/storage/command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3067 2024-04-22 23:47:53.000000 lsst_rsp-0.5.2/src/lsst/rsp/startup/storage/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5240 2024-04-22 23:47:53.000000 lsst_rsp-0.5.2/src/lsst/rsp/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:47:58.076074 lsst_rsp-0.5.2/src/lsst_rsp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5444 2024-04-22 23:47:58.000000 lsst_rsp-0.5.2/src/lsst_rsp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1669 2024-04-22 23:47:58.000000 lsst_rsp-0.5.2/src/lsst_rsp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 23:47:58.000000 lsst_rsp-0.5.2/src/lsst_rsp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-22 23:47:58.000000 lsst_rsp-0.5.2/src/lsst_rsp.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-04-22 23:47:58.000000 lsst_rsp-0.5.2/src/lsst_rsp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-22 23:47:58.000000 lsst_rsp-0.5.2/src/lsst_rsp.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:47:58.076074 lsst_rsp-0.5.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-22 23:47:53.000000 lsst_rsp-0.5.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2379 2024-04-22 23:47:53.000000 lsst_rsp-0.5.2/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11534 2024-04-22 23:47:53.000000 lsst_rsp-0.5.2/tests/startup_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:47:58.064073 lsst_rsp-0.5.2/tests/support/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:47:58.076074 lsst_rsp-0.5.2/tests/support/files/
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-22 23:47:53.000000 lsst_rsp-0.5.2/tests/support/files/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:47:58.076074 lsst_rsp-0.5.2/tests/support/files/etc/
+-rw-r--r--   0 runner    (1001) docker     (127)    10287 2024-04-22 23:47:53.000000 lsst_rsp-0.5.2/tests/support/files/etc/dircolors.ansi-universal
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:47:58.076074 lsst_rsp-0.5.2/tests/support/files/etc/skel/
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-04-22 23:47:53.000000 lsst_rsp-0.5.2/tests/support/files/etc/skel/.gitconfig
+-rw-r--r--   0 runner    (1001) docker     (127)      359 2024-04-22 23:47:53.000000 lsst_rsp-0.5.2/tests/support/files/etc/skel/.pythonrc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:47:58.076074 lsst_rsp-0.5.2/tests/support/files/etc/skel/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (127)      376 2024-04-22 23:47:53.000000 lsst_rsp-0.5.2/tests/support/files/etc/skel/notebooks/.user_setups
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:47:58.064073 lsst_rsp-0.5.2/tests/support/files/homedir/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:47:58.076074 lsst_rsp-0.5.2/tests/support/files/homedir/.lsst/
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-22 23:47:53.000000 lsst_rsp-0.5.2/tests/support/files/homedir/.lsst/aws-credentials.ini
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-22 23:47:53.000000 lsst_rsp-0.5.2/tests/support/files/homedir/.lsst/postgres-credentials.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:47:58.068073 lsst_rsp-0.5.2/tests/support/files/stack_top/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:47:58.076074 lsst_rsp-0.5.2/tests/support/files/stack_top/jupyterlab/
+-rw-r--r--   0 runner    (1001) docker     (127)     1833 2024-04-22 23:47:53.000000 lsst_rsp-0.5.2/tests/support/files/stack_top/jupyterlab/20-logging.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:47:58.076074 lsst_rsp-0.5.2/tests/support/files/stack_top/jupyterlab/secrets/
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-22 23:47:53.000000 lsst_rsp-0.5.2/tests/support/files/stack_top/jupyterlab/secrets/aws-credentials.ini
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-22 23:47:53.000000 lsst_rsp-0.5.2/tests/support/files/stack_top/jupyterlab/secrets/postgres-credentials.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-04-22 23:47:53.000000 lsst_rsp-0.5.2/tests/utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      297 2024-04-22 23:47:53.000000 lsst_rsp-0.5.2/tests/version_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      644 2024-04-22 23:47:53.000000 lsst_rsp-0.5.2/tox.ini
```

### Comparing `lsst-rsp-0.5.1/.github/CONTRIBUTING.md` & `lsst_rsp-0.5.2/.github/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `lsst-rsp-0.5.1/.github/workflows/ci.yaml` & `lsst_rsp-0.5.2/.github/workflows/ci.yaml`

 * *Files identical despite different names*

### Comparing `lsst-rsp-0.5.1/.github/workflows/periodic-ci.yaml` & `lsst_rsp-0.5.2/.github/workflows/periodic-ci.yaml`

 * *Files identical despite different names*

### Comparing `lsst-rsp-0.5.1/.gitignore` & `lsst_rsp-0.5.2/.gitignore`

 * *Files identical despite different names*

### Comparing `lsst-rsp-0.5.1/.pre-commit-config.yaml` & `lsst_rsp-0.5.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `lsst-rsp-0.5.1/CHANGELOG.md` & `lsst_rsp-0.5.2/CHANGELOG.md`

 * *Files 26% similar despite different names*

```diff
@@ -2,14 +2,21 @@
 
 lsst-rsp is versioned with [semver](https://semver.org/).
 
 Find changes for the upcoming release in the project's [changelog.d directory](https://github.com/lsst-sqre/lsst-rsp/tree/main/changelog.d/).
 
 <!-- scriv-insert-here -->
 
+<a id='changelog-0.5.2'></a>
+## 0.5.2 (2024-04-22)
+
+### Bug fixes
+
+- If the user credentials directory `$HOME/.lsst` does not exist, create it.
+
 <a id='changelog-0.4.3'></a>
 ## 0.4.3 (2024-03-22)
 
 ### Bug fixes
 
 - Raise `ValueError` for invalid arguments to utility functions rather than bare `Exception`.
```

### Comparing `lsst-rsp-0.5.1/LICENSE` & `lsst_rsp-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `lsst-rsp-0.5.1/PKG-INFO` & `lsst_rsp-0.5.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lsst-rsp
-Version: 0.5.1
+Version: 0.5.2
 Summary: Utility functions for the Rubin Science Platform
 Author-email: "Association of Universities for Research in Astronomy, Inc. (AURA)" <sqre-admin@lists.lsst.org>
 License: MIT License
         
         Copyright (c) 2021-2024 Association of Universities for Research in Astronomy, Inc. (AURA)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `lsst-rsp-0.5.1/README.md` & `lsst_rsp-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `lsst-rsp-0.5.1/pyproject.toml` & `lsst_rsp-0.5.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `lsst-rsp-0.5.1/src/lsst/rsp/__init__.py` & `lsst_rsp-0.5.2/src/lsst/rsp/__init__.py`

 * *Files identical despite different names*

### Comparing `lsst-rsp-0.5.1/src/lsst/rsp/catalog.py` & `lsst_rsp-0.5.2/src/lsst/rsp/catalog.py`

 * *Files identical despite different names*

### Comparing `lsst-rsp-0.5.1/src/lsst/rsp/log.py` & `lsst_rsp-0.5.2/src/lsst/rsp/log.py`

 * *Files identical despite different names*

### Comparing `lsst-rsp-0.5.1/src/lsst/rsp/service.py` & `lsst_rsp-0.5.2/src/lsst/rsp/service.py`

 * *Files identical despite different names*

### Comparing `lsst-rsp-0.5.1/src/lsst/rsp/startup/constants.py` & `lsst_rsp-0.5.2/src/lsst/rsp/startup/constants.py`

 * *Files identical despite different names*

### Comparing `lsst-rsp-0.5.1/src/lsst/rsp/startup/exceptions.py` & `lsst_rsp-0.5.2/src/lsst/rsp/startup/exceptions.py`

 * *Files identical despite different names*

### Comparing `lsst-rsp-0.5.1/src/lsst/rsp/startup/models/noninteractive.py` & `lsst_rsp-0.5.2/src/lsst/rsp/startup/models/noninteractive.py`

 * *Files identical despite different names*

### Comparing `lsst-rsp-0.5.1/src/lsst/rsp/startup/services/labrunner.py` & `lsst_rsp-0.5.2/src/lsst/rsp/startup/services/labrunner.py`

 * *Files 2% similar despite different names*

```diff
@@ -256,14 +256,16 @@
         #
         # Merge the config in the original credentials file and the one
         # in our homedir.  For any given section, we assume that the
         # information in the container ("original credentials files")
         # is correct, but leave any other user config alone.
         #
         hc_path = Path(self._env["AWS_SHARED_CREDENTIALS_FILE"])
+        if not hc_path.parent.exists():
+            hc_path.parent.mkdir(mode=0o700, parents=True)
         hc_path.touch(mode=0o600, exist_ok=True)
         home_config = configparser.ConfigParser()
         home_config.read(str(hc_path))
         ro_config = configparser.ConfigParser()
         ro_config.read(self._env["ORIG_AWS_SHARED_CREDENTIALS_FILE"])
         for sect in ro_config.sections():
             home_config[sect] = ro_config[sect]
@@ -273,14 +275,16 @@
     def _merge_pgpass(self) -> None:
         #
         # Same as above, but for pgpass files.
         #
         config = {}
         # Get current config from homedir
         home_pgpass = Path(self._env["PGPASSFILE"])
+        if not home_pgpass.parent.exists():
+            home_pgpass.parent.mkdir(mode=0o700, parents=True)
         home_pgpass.touch(mode=0o600, exist_ok=True)
         lines = home_pgpass.read_text().splitlines()
         for line in lines:
             if ":" not in line:
                 continue
             connection, passwd = line.rsplit(":", maxsplit=1)
             config[connection] = passwd.rstrip()
```

### Comparing `lsst-rsp-0.5.1/src/lsst/rsp/startup/storage/command.py` & `lsst_rsp-0.5.2/src/lsst/rsp/startup/storage/command.py`

 * *Files identical despite different names*

### Comparing `lsst-rsp-0.5.1/src/lsst/rsp/startup/storage/logging.py` & `lsst_rsp-0.5.2/src/lsst/rsp/startup/storage/logging.py`

 * *Files identical despite different names*

### Comparing `lsst-rsp-0.5.1/src/lsst/rsp/utils.py` & `lsst_rsp-0.5.2/src/lsst/rsp/utils.py`

 * *Files identical despite different names*

### Comparing `lsst-rsp-0.5.1/src/lsst_rsp.egg-info/PKG-INFO` & `lsst_rsp-0.5.2/src/lsst_rsp.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lsst-rsp
-Version: 0.5.1
+Version: 0.5.2
 Summary: Utility functions for the Rubin Science Platform
 Author-email: "Association of Universities for Research in Astronomy, Inc. (AURA)" <sqre-admin@lists.lsst.org>
 License: MIT License
         
         Copyright (c) 2021-2024 Association of Universities for Research in Astronomy, Inc. (AURA)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `lsst-rsp-0.5.1/src/lsst_rsp.egg-info/SOURCES.txt` & `lsst_rsp-0.5.2/src/lsst_rsp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lsst-rsp-0.5.1/tests/conftest.py` & `lsst_rsp-0.5.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `lsst-rsp-0.5.1/tests/startup_test.py` & `lsst_rsp-0.5.2/tests/startup_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Tests for startup object."""
 
 import configparser
 import json
 import os
+import shutil
 from collections.abc import Iterable
 from pathlib import Path
 
 import pytest
 import symbolicmode
 
 import lsst.rsp
@@ -142,14 +143,35 @@
 
 #
 # File manipulation tests
 #
 
 
 @pytest.mark.usefixtures("_rsp_env")
+def test_create_credential_dir(monkeypatch: pytest.MonkeyPatch) -> None:
+    td = lsst.rsp.startup.constants.TOP_DIR_PATH
+    secret_dir = td / "jupyterlab" / "secrets"
+    monkeypatch.setenv(
+        "AWS_SHARED_CREDENTIALS_FILE", str(secret_dir / "aws-credentials.ini")
+    )
+    monkeypatch.setenv(
+        "PGPASSFILE", str(secret_dir / "postgres-credentials.txt")
+    )
+    cred_dir = Path(os.environ["HOME"]) / ".lsst"
+    assert cred_dir.exists()
+    shutil.rmtree(cred_dir)
+    assert not cred_dir.exists()
+    lr = LabRunner()
+    lr._set_butler_credential_variables()
+    assert not cred_dir.exists()
+    lr._copy_butler_credentials()
+    assert cred_dir.exists()
+
+
+@pytest.mark.usefixtures("_rsp_env")
 def test_copy_butler_credentials(monkeypatch: pytest.MonkeyPatch) -> None:
     td = lsst.rsp.startup.constants.TOP_DIR_PATH
     secret_dir = td / "jupyterlab" / "secrets"
     monkeypatch.setenv(
         "AWS_SHARED_CREDENTIALS_FILE", str(secret_dir / "aws-credentials.ini")
     )
     monkeypatch.setenv(
```

### Comparing `lsst-rsp-0.5.1/tests/support/files/etc/dircolors.ansi-universal` & `lsst_rsp-0.5.2/tests/support/files/etc/dircolors.ansi-universal`

 * *Files identical despite different names*

### Comparing `lsst-rsp-0.5.1/tests/support/files/stack_top/jupyterlab/20-logging.py` & `lsst_rsp-0.5.2/tests/support/files/stack_top/jupyterlab/20-logging.py`

 * *Files identical despite different names*

### Comparing `lsst-rsp-0.5.1/tests/utils_test.py` & `lsst_rsp-0.5.2/tests/utils_test.py`

 * *Files identical despite different names*

### Comparing `lsst-rsp-0.5.1/tox.ini` & `lsst_rsp-0.5.2/tox.ini`

 * *Files identical despite different names*

