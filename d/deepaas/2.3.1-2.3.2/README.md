# Comparing `tmp/deepaas-2.3.1.tar.gz` & `tmp/deepaas-2.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deepaas-2.3.1.tar", last modified: Tue Mar 26 13:00:01 2024, max compression
+gzip compressed data, was "deepaas-2.3.2.tar", last modified: Tue Apr 23 13:38:30 2024, max compression
```

## Comparing `deepaas-2.3.1.tar` & `deepaas-2.3.2.tar`

### file list

```diff
@@ -1,139 +1,139 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:00:01.329457 deepaas-2.3.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:00:01.313457 deepaas-2.3.1/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      308 2024-03-26 12:59:48.000000 deepaas-2.3.1/.github/ISSUE_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-03-26 12:59:48.000000 deepaas-2.3.1/.github/PULL_REQUEST_TEMPLATE.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:00:01.313457 deepaas-2.3.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      610 2024-03-26 12:59:48.000000 deepaas-2.3.1/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1409 2024-03-26 12:59:48.000000 deepaas-2.3.1/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1747 2024-03-26 12:59:48.000000 deepaas-2.3.1/.github/workflows/release-please.yml
--rw-r--r--   0 runner    (1001) docker     (127)      657 2024-03-26 12:59:48.000000 deepaas-2.3.1/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-03-26 12:59:48.000000 deepaas-2.3.1/.release-please-manifest.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:00:01.313457 deepaas-2.3.1/.sqa/
--rw-r--r--   0 runner    (1001) docker     (127)      816 2024-03-26 12:59:48.000000 deepaas-2.3.1/.sqa/config.yml
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-03-26 12:59:48.000000 deepaas-2.3.1/.sqa/docker-compose.yml
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-03-26 12:59:48.000000 deepaas-2.3.1/.stestr.conf
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-03-26 13:00:01.000000 deepaas-2.3.1/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (127)     2058 2024-03-26 12:59:48.000000 deepaas-2.3.1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     3231 2024-03-26 12:59:48.000000 deepaas-2.3.1/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)     5414 2024-03-26 12:59:48.000000 deepaas-2.3.1/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-03-26 13:00:01.000000 deepaas-2.3.1/ChangeLog
--rwxr-xr-x   0 runner    (1001) docker     (127)      530 2024-03-26 12:59:48.000000 deepaas-2.3.1/Jenkinsfile
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-03-26 12:59:48.000000 deepaas-2.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1858 2024-03-26 12:59:48.000000 deepaas-2.3.1/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     5479 2024-03-26 13:00:01.329457 deepaas-2.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3464 2024-03-26 12:59:48.000000 deepaas-2.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:00:01.313457 deepaas-2.3.1/deepaas/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-03-26 12:59:48.000000 deepaas-2.3.1/deepaas/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:00:01.317457 deepaas-2.3.1/deepaas/api/
--rw-r--r--   0 runner    (1001) docker     (127)     3300 2024-03-26 12:59:48.000000 deepaas-2.3.1/deepaas/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:00:01.317457 deepaas-2.3.1/deepaas/api/v2/
--rw-r--r--   0 runner    (1001) docker     (127)     2191 2024-03-26 12:59:48.000000 deepaas-2.3.1/deepaas/api/v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2815 2024-03-26 12:59:48.000000 deepaas-2.3.1/deepaas/api/v2/debug.py
--rw-r--r--   0 runner    (1001) docker     (127)     3312 2024-03-26 12:59:48.000000 deepaas-2.3.1/deepaas/api/v2/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     3437 2024-03-26 12:59:48.000000 deepaas-2.3.1/deepaas/api/v2/predict.py
--rw-r--r--   0 runner    (1001) docker     (127)     2611 2024-03-26 12:59:48.000000 deepaas-2.3.1/deepaas/api/v2/responses.py
--rw-r--r--   0 runner    (1001) docker     (127)     6327 2024-03-26 12:59:48.000000 deepaas-2.3.1/deepaas/api/v2/train.py
--rw-r--r--   0 runner    (1001) docker     (127)      823 2024-03-26 12:59:48.000000 deepaas-2.3.1/deepaas/api/v2/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2472 2024-03-26 12:59:48.000000 deepaas-2.3.1/deepaas/api/versions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:00:01.317457 deepaas-2.3.1/deepaas/cmd/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 12:59:48.000000 deepaas-2.3.1/deepaas/cmd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1262 2024-03-26 12:59:48.000000 deepaas-2.3.1/deepaas/cmd/_shutdown.py
--rw-r--r--   0 runner    (1001) docker     (127)    13629 2024-03-26 12:59:48.000000 deepaas-2.3.1/deepaas/cmd/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     4469 2024-03-26 12:59:48.000000 deepaas-2.3.1/deepaas/cmd/execute.py
--rw-r--r--   0 runner    (1001) docker     (127)     3119 2024-03-26 12:59:48.000000 deepaas-2.3.1/deepaas/cmd/run.py
--rw-r--r--   0 runner    (1001) docker     (127)     3753 2024-03-26 12:59:48.000000 deepaas-2.3.1/deepaas/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      704 2024-03-26 12:59:48.000000 deepaas-2.3.1/deepaas/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:00:01.317457 deepaas-2.3.1/deepaas/model/
--rw-r--r--   0 runner    (1001) docker     (127)      927 2024-03-26 12:59:48.000000 deepaas-2.3.1/deepaas/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1994 2024-03-26 12:59:48.000000 deepaas-2.3.1/deepaas/model/loading.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:00:01.317457 deepaas-2.3.1/deepaas/model/v2/
--rw-r--r--   0 runner    (1001) docker     (127)     2859 2024-03-26 12:59:48.000000 deepaas-2.3.1/deepaas/model/v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8887 2024-03-26 12:59:48.000000 deepaas-2.3.1/deepaas/model/v2/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     6725 2024-03-26 12:59:48.000000 deepaas-2.3.1/deepaas/model/v2/test.py
--rw-r--r--   0 runner    (1001) docker     (127)    13439 2024-03-26 12:59:48.000000 deepaas-2.3.1/deepaas/model/v2/wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)      817 2024-03-26 12:59:48.000000 deepaas-2.3.1/deepaas/opts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:00:01.321457 deepaas-2.3.1/deepaas/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 12:59:48.000000 deepaas-2.3.1/deepaas/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2564 2024-03-26 12:59:48.000000 deepaas-2.3.1/deepaas/tests/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2224 2024-03-26 12:59:48.000000 deepaas-2.3.1/deepaas/tests/fake_responses.py
--rw-r--r--   0 runner    (1001) docker     (127)     4188 2024-03-26 12:59:48.000000 deepaas-2.3.1/deepaas/tests/test_cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)     9525 2024-03-26 12:59:48.000000 deepaas-2.3.1/deepaas/tests/test_v2_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     8622 2024-03-26 12:59:48.000000 deepaas-2.3.1/deepaas/tests/test_v2_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-03-26 12:59:48.000000 deepaas-2.3.1/deepaas/tests/test_versions_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      796 2024-03-26 12:59:48.000000 deepaas-2.3.1/deepaas/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:00:01.329457 deepaas-2.3.1/deepaas.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5479 2024-03-26 13:00:01.000000 deepaas-2.3.1/deepaas.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3445 2024-03-26 13:00:01.000000 deepaas-2.3.1/deepaas.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-26 13:00:01.000000 deepaas-2.3.1/deepaas.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-03-26 13:00:01.000000 deepaas-2.3.1/deepaas.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-26 13:00:01.000000 deepaas-2.3.1/deepaas.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-03-26 13:00:01.000000 deepaas-2.3.1/deepaas.egg-info/pbr.json
--rw-r--r--   0 runner    (1001) docker     (127)      202 2024-03-26 13:00:01.000000 deepaas-2.3.1/deepaas.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-03-26 13:00:01.000000 deepaas-2.3.1/deepaas.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:00:01.321457 deepaas-2.3.1/doc/
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-03-26 12:59:48.000000 deepaas-2.3.1/doc/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:00:01.321457 deepaas-2.3.1/doc/source/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:00:01.321457 deepaas-2.3.1/doc/source/_static/
--rw-r--r--   0 runner    (1001) docker     (127)   109251 2024-03-26 12:59:48.000000 deepaas-2.3.1/doc/source/_static/logo-deep-solid-white.png
--rw-r--r--   0 runner    (1001) docker     (127)     9342 2024-03-26 12:59:48.000000 deepaas-2.3.1/doc/source/_static/logo.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:00:01.321457 deepaas-2.3.1/doc/source/_templates/
--rw-r--r--   0 runner    (1001) docker     (127)      282 2024-03-26 12:59:48.000000 deepaas-2.3.1/doc/source/_templates/sidebarfooter.html
--rw-r--r--   0 runner    (1001) docker     (127)      386 2024-03-26 12:59:48.000000 deepaas-2.3.1/doc/source/api.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:00:01.321457 deepaas-2.3.1/doc/source/cli/
--rw-r--r--   0 runner    (1001) docker     (127)     2358 2024-03-26 12:59:48.000000 deepaas-2.3.1/doc/source/cli/deepaas-cli.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1623 2024-03-26 12:59:48.000000 deepaas-2.3.1/doc/source/cli/deepaas-predict.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2437 2024-03-26 12:59:48.000000 deepaas-2.3.1/doc/source/cli/deepaas-run.rst
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-03-26 12:59:48.000000 deepaas-2.3.1/doc/source/cli/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     7822 2024-03-26 12:59:48.000000 deepaas-2.3.1/doc/source/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:00:01.321457 deepaas-2.3.1/doc/source/contributing/
--rw-r--r--   0 runner    (1001) docker     (127)     3231 2024-03-26 12:59:48.000000 deepaas-2.3.1/doc/source/contributing/code_of_conduct.md
--rw-r--r--   0 runner    (1001) docker     (127)     5414 2024-03-26 12:59:48.000000 deepaas-2.3.1/doc/source/contributing/contributing.md
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-03-26 12:59:48.000000 deepaas-2.3.1/doc/source/contributing/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1684 2024-03-26 12:59:48.000000 deepaas-2.3.1/doc/source/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:00:01.321457 deepaas-2.3.1/doc/source/install/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:00:01.321457 deepaas-2.3.1/doc/source/install/configuration/
--rw-r--r--   0 runner    (1001) docker     (127)      294 2024-03-26 12:59:48.000000 deepaas-2.3.1/doc/source/install/configuration/config.rst
--rw-r--r--   0 runner    (1001) docker     (127)      382 2024-03-26 12:59:48.000000 deepaas-2.3.1/doc/source/install/configuration/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      596 2024-03-26 12:59:48.000000 deepaas-2.3.1/doc/source/install/configuration/sample.rst
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-03-26 12:59:48.000000 deepaas-2.3.1/doc/source/install/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      709 2024-03-26 12:59:48.000000 deepaas-2.3.1/doc/source/install/installation.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:00:01.321457 deepaas-2.3.1/doc/source/install/releasenotes/
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-03-26 12:59:48.000000 deepaas-2.3.1/doc/source/install/releasenotes/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     7290 2024-03-26 12:59:48.000000 deepaas-2.3.1/doc/source/install/upgrade.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:00:01.325457 deepaas-2.3.1/doc/source/user/
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-03-26 12:59:48.000000 deepaas-2.3.1/doc/source/user/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      866 2024-03-26 12:59:48.000000 deepaas-2.3.1/doc/source/user/predict.rst
--rw-r--r--   0 runner    (1001) docker     (127)      723 2024-03-26 12:59:48.000000 deepaas-2.3.1/doc/source/user/quickstart.rst
--rw-r--r--   0 runner    (1001) docker     (127)     8236 2024-03-26 12:59:48.000000 deepaas-2.3.1/doc/source/user/v2-api.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:00:01.325457 deepaas-2.3.1/etc/
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-03-26 12:59:48.000000 deepaas-2.3.1/etc/deepaas-config-generator.conf
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-26 12:59:48.000000 deepaas-2.3.1/mypy.ini
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:00:01.325457 deepaas-2.3.1/paper/
--rw-r--r--   0 runner    (1001) docker     (127)    60694 2024-03-26 12:59:48.000000 deepaas-2.3.1/paper/deepaas.png
--rw-r--r--   0 runner    (1001) docker     (127)     2180 2024-03-26 12:59:48.000000 deepaas-2.3.1/paper/paper.bib
--rw-r--r--   0 runner    (1001) docker     (127)     4037 2024-03-26 12:59:48.000000 deepaas-2.3.1/paper/paper.md
--rw-r--r--   0 runner    (1001) docker     (127)      372 2024-03-26 12:59:48.000000 deepaas-2.3.1/release-please-config.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:00:01.309457 deepaas-2.3.1/releasenotes/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:00:01.329457 deepaas-2.3.1/releasenotes/notes/
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-03-26 12:59:48.000000 deepaas-2.3.1/releasenotes/notes/add-debug-endpoint-7b2f3ede199d74cc.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      267 2024-03-26 12:59:48.000000 deepaas-2.3.1/releasenotes/notes/add-new-cli-669061dfada81f5c.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      504 2024-03-26 12:59:48.000000 deepaas-2.3.1/releasenotes/notes/allow-passing-args-dbadafef832265e9.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      339 2024-03-26 12:59:48.000000 deepaas-2.3.1/releasenotes/notes/bug-fixes-73cfa32ffb5bdbb0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-03-26 12:59:48.000000 deepaas-2.3.1/releasenotes/notes/deepaas-cli-6e8a8689baab3277.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      465 2024-03-26 12:59:48.000000 deepaas-2.3.1/releasenotes/notes/deprecate-old-model-loading-27aa4485b2132da7.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-03-26 12:59:48.000000 deepaas-2.3.1/releasenotes/notes/deprecate-openwhisk-be449ddfb9fa554c.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      205 2024-03-26 12:59:48.000000 deepaas-2.3.1/releasenotes/notes/disable-v1-default-dc827ebdd0d90181.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-03-26 12:59:48.000000 deepaas-2.3.1/releasenotes/notes/initial-documentation-2584128b20eeb9d1.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      602 2024-03-26 12:59:48.000000 deepaas-2.3.1/releasenotes/notes/only-py3-support-928e43ebad4904da.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      652 2024-03-26 12:59:48.000000 deepaas-2.3.1/releasenotes/notes/openwish-proxy-c9c15eef91da0579.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      348 2024-03-26 12:59:48.000000 deepaas-2.3.1/releasenotes/notes/remove-deprecated-get-args-166d8535f5b23c1e.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-03-26 12:59:48.000000 deepaas-2.3.1/releasenotes/notes/remove-openwhisk-integration-f69978c2824221c3.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      343 2024-03-26 12:59:48.000000 deepaas-2.3.1/releasenotes/notes/remove-v1-api-93dbfcdc2f4beb1d.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      296 2024-03-26 12:59:48.000000 deepaas-2.3.1/releasenotes/notes/training-arguments-4e59dc2945a634a5.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-03-26 12:59:48.000000 deepaas-2.3.1/releasenotes/notes/unify-train-predict-261e92c21d9f47d1.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2088 2024-03-26 12:59:48.000000 deepaas-2.3.1/releasenotes/notes/v2-api-1bc54fcdb42f6c8b.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      812 2024-03-26 12:59:48.000000 deepaas-2.3.1/releasenotes/notes/versioned-api-endpoints-23bf76653d43f033.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      464 2024-03-26 12:59:48.000000 deepaas-2.3.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1807 2024-03-26 13:00:01.329457 deepaas-2.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      632 2024-03-26 12:59:48.000000 deepaas-2.3.1/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)     2929 2024-03-26 12:59:48.000000 deepaas-2.3.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:38:30.770416 deepaas-2.3.2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:38:30.754416 deepaas-2.3.2/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-04-23 13:38:11.000000 deepaas-2.3.2/.github/ISSUE_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-04-23 13:38:11.000000 deepaas-2.3.2/.github/PULL_REQUEST_TEMPLATE.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:38:30.754416 deepaas-2.3.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      610 2024-04-23 13:38:11.000000 deepaas-2.3.2/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1409 2024-04-23 13:38:11.000000 deepaas-2.3.2/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1747 2024-04-23 13:38:11.000000 deepaas-2.3.2/.github/workflows/release-please.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      657 2024-04-23 13:38:11.000000 deepaas-2.3.2/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-23 13:38:11.000000 deepaas-2.3.2/.release-please-manifest.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:38:30.754416 deepaas-2.3.2/.sqa/
+-rw-r--r--   0 runner    (1001) docker     (127)      816 2024-04-23 13:38:11.000000 deepaas-2.3.2/.sqa/config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-23 13:38:11.000000 deepaas-2.3.2/.sqa/docker-compose.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-23 13:38:11.000000 deepaas-2.3.2/.stestr.conf
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-23 13:38:30.000000 deepaas-2.3.2/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (127)     2323 2024-04-23 13:38:11.000000 deepaas-2.3.2/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3231 2024-04-23 13:38:11.000000 deepaas-2.3.2/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5414 2024-04-23 13:38:11.000000 deepaas-2.3.2/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-23 13:38:30.000000 deepaas-2.3.2/ChangeLog
+-rwxr-xr-x   0 runner    (1001) docker     (127)      530 2024-04-23 13:38:11.000000 deepaas-2.3.2/Jenkinsfile
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-23 13:38:11.000000 deepaas-2.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1858 2024-04-23 13:38:11.000000 deepaas-2.3.2/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     5479 2024-04-23 13:38:30.770416 deepaas-2.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3464 2024-04-23 13:38:11.000000 deepaas-2.3.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:38:30.754416 deepaas-2.3.2/deepaas/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-23 13:38:11.000000 deepaas-2.3.2/deepaas/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:38:30.754416 deepaas-2.3.2/deepaas/api/
+-rw-r--r--   0 runner    (1001) docker     (127)     3300 2024-04-23 13:38:11.000000 deepaas-2.3.2/deepaas/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:38:30.758416 deepaas-2.3.2/deepaas/api/v2/
+-rw-r--r--   0 runner    (1001) docker     (127)     2191 2024-04-23 13:38:11.000000 deepaas-2.3.2/deepaas/api/v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2815 2024-04-23 13:38:11.000000 deepaas-2.3.2/deepaas/api/v2/debug.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3312 2024-04-23 13:38:11.000000 deepaas-2.3.2/deepaas/api/v2/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3437 2024-04-23 13:38:11.000000 deepaas-2.3.2/deepaas/api/v2/predict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2611 2024-04-23 13:38:11.000000 deepaas-2.3.2/deepaas/api/v2/responses.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6327 2024-04-23 13:38:11.000000 deepaas-2.3.2/deepaas/api/v2/train.py
+-rw-r--r--   0 runner    (1001) docker     (127)      823 2024-04-23 13:38:11.000000 deepaas-2.3.2/deepaas/api/v2/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2472 2024-04-23 13:38:11.000000 deepaas-2.3.2/deepaas/api/versions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:38:30.758416 deepaas-2.3.2/deepaas/cmd/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 13:38:11.000000 deepaas-2.3.2/deepaas/cmd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1262 2024-04-23 13:38:11.000000 deepaas-2.3.2/deepaas/cmd/_shutdown.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13600 2024-04-23 13:38:11.000000 deepaas-2.3.2/deepaas/cmd/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4469 2024-04-23 13:38:11.000000 deepaas-2.3.2/deepaas/cmd/execute.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3119 2024-04-23 13:38:11.000000 deepaas-2.3.2/deepaas/cmd/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3753 2024-04-23 13:38:11.000000 deepaas-2.3.2/deepaas/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      704 2024-04-23 13:38:11.000000 deepaas-2.3.2/deepaas/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:38:30.758416 deepaas-2.3.2/deepaas/model/
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-04-23 13:38:11.000000 deepaas-2.3.2/deepaas/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1994 2024-04-23 13:38:11.000000 deepaas-2.3.2/deepaas/model/loading.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:38:30.758416 deepaas-2.3.2/deepaas/model/v2/
+-rw-r--r--   0 runner    (1001) docker     (127)     2859 2024-04-23 13:38:11.000000 deepaas-2.3.2/deepaas/model/v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8887 2024-04-23 13:38:11.000000 deepaas-2.3.2/deepaas/model/v2/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6725 2024-04-23 13:38:11.000000 deepaas-2.3.2/deepaas/model/v2/test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13439 2024-04-23 13:38:11.000000 deepaas-2.3.2/deepaas/model/v2/wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)      817 2024-04-23 13:38:11.000000 deepaas-2.3.2/deepaas/opts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:38:30.762416 deepaas-2.3.2/deepaas/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 13:38:11.000000 deepaas-2.3.2/deepaas/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2564 2024-04-23 13:38:11.000000 deepaas-2.3.2/deepaas/tests/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2224 2024-04-23 13:38:11.000000 deepaas-2.3.2/deepaas/tests/fake_responses.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4188 2024-04-23 13:38:11.000000 deepaas-2.3.2/deepaas/tests/test_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9525 2024-04-23 13:38:11.000000 deepaas-2.3.2/deepaas/tests/test_v2_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8622 2024-04-23 13:38:11.000000 deepaas-2.3.2/deepaas/tests/test_v2_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-04-23 13:38:11.000000 deepaas-2.3.2/deepaas/tests/test_versions_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      796 2024-04-23 13:38:11.000000 deepaas-2.3.2/deepaas/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:38:30.770416 deepaas-2.3.2/deepaas.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5479 2024-04-23 13:38:30.000000 deepaas-2.3.2/deepaas.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3445 2024-04-23 13:38:30.000000 deepaas-2.3.2/deepaas.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 13:38:30.000000 deepaas-2.3.2/deepaas.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-23 13:38:30.000000 deepaas-2.3.2/deepaas.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 13:38:30.000000 deepaas-2.3.2/deepaas.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-23 13:38:30.000000 deepaas-2.3.2/deepaas.egg-info/pbr.json
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-23 13:38:30.000000 deepaas-2.3.2/deepaas.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-23 13:38:30.000000 deepaas-2.3.2/deepaas.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:38:30.762416 deepaas-2.3.2/doc/
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-23 13:38:11.000000 deepaas-2.3.2/doc/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:38:30.762416 deepaas-2.3.2/doc/source/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:38:30.762416 deepaas-2.3.2/doc/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)   109251 2024-04-23 13:38:11.000000 deepaas-2.3.2/doc/source/_static/logo-deep-solid-white.png
+-rw-r--r--   0 runner    (1001) docker     (127)     9342 2024-04-23 13:38:11.000000 deepaas-2.3.2/doc/source/_static/logo.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:38:30.762416 deepaas-2.3.2/doc/source/_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      282 2024-04-23 13:38:11.000000 deepaas-2.3.2/doc/source/_templates/sidebarfooter.html
+-rw-r--r--   0 runner    (1001) docker     (127)      386 2024-04-23 13:38:11.000000 deepaas-2.3.2/doc/source/api.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:38:30.762416 deepaas-2.3.2/doc/source/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)     2358 2024-04-23 13:38:11.000000 deepaas-2.3.2/doc/source/cli/deepaas-cli.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1623 2024-04-23 13:38:11.000000 deepaas-2.3.2/doc/source/cli/deepaas-predict.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2437 2024-04-23 13:38:11.000000 deepaas-2.3.2/doc/source/cli/deepaas-run.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-23 13:38:11.000000 deepaas-2.3.2/doc/source/cli/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7822 2024-04-23 13:38:11.000000 deepaas-2.3.2/doc/source/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:38:30.762416 deepaas-2.3.2/doc/source/contributing/
+-rw-r--r--   0 runner    (1001) docker     (127)     3231 2024-04-23 13:38:11.000000 deepaas-2.3.2/doc/source/contributing/code_of_conduct.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5414 2024-04-23 13:38:11.000000 deepaas-2.3.2/doc/source/contributing/contributing.md
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-23 13:38:11.000000 deepaas-2.3.2/doc/source/contributing/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1684 2024-04-23 13:38:11.000000 deepaas-2.3.2/doc/source/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:38:30.762416 deepaas-2.3.2/doc/source/install/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:38:30.762416 deepaas-2.3.2/doc/source/install/configuration/
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-04-23 13:38:11.000000 deepaas-2.3.2/doc/source/install/configuration/config.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      382 2024-04-23 13:38:11.000000 deepaas-2.3.2/doc/source/install/configuration/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2024-04-23 13:38:11.000000 deepaas-2.3.2/doc/source/install/configuration/sample.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-23 13:38:11.000000 deepaas-2.3.2/doc/source/install/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-04-23 13:38:11.000000 deepaas-2.3.2/doc/source/install/installation.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:38:30.762416 deepaas-2.3.2/doc/source/install/releasenotes/
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-23 13:38:11.000000 deepaas-2.3.2/doc/source/install/releasenotes/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7290 2024-04-23 13:38:11.000000 deepaas-2.3.2/doc/source/install/upgrade.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:38:30.766416 deepaas-2.3.2/doc/source/user/
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-23 13:38:11.000000 deepaas-2.3.2/doc/source/user/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      866 2024-04-23 13:38:11.000000 deepaas-2.3.2/doc/source/user/predict.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      723 2024-04-23 13:38:11.000000 deepaas-2.3.2/doc/source/user/quickstart.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     8236 2024-04-23 13:38:11.000000 deepaas-2.3.2/doc/source/user/v2-api.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:38:30.766416 deepaas-2.3.2/etc/
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-23 13:38:11.000000 deepaas-2.3.2/etc/deepaas-config-generator.conf
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 13:38:11.000000 deepaas-2.3.2/mypy.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:38:30.766416 deepaas-2.3.2/paper/
+-rw-r--r--   0 runner    (1001) docker     (127)    60694 2024-04-23 13:38:11.000000 deepaas-2.3.2/paper/deepaas.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2180 2024-04-23 13:38:11.000000 deepaas-2.3.2/paper/paper.bib
+-rw-r--r--   0 runner    (1001) docker     (127)     4037 2024-04-23 13:38:11.000000 deepaas-2.3.2/paper/paper.md
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-04-23 13:38:11.000000 deepaas-2.3.2/release-please-config.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:38:30.750416 deepaas-2.3.2/releasenotes/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:38:30.770416 deepaas-2.3.2/releasenotes/notes/
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-04-23 13:38:11.000000 deepaas-2.3.2/releasenotes/notes/add-debug-endpoint-7b2f3ede199d74cc.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      267 2024-04-23 13:38:11.000000 deepaas-2.3.2/releasenotes/notes/add-new-cli-669061dfada81f5c.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-04-23 13:38:11.000000 deepaas-2.3.2/releasenotes/notes/allow-passing-args-dbadafef832265e9.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      339 2024-04-23 13:38:11.000000 deepaas-2.3.2/releasenotes/notes/bug-fixes-73cfa32ffb5bdbb0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-23 13:38:11.000000 deepaas-2.3.2/releasenotes/notes/deepaas-cli-6e8a8689baab3277.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      465 2024-04-23 13:38:11.000000 deepaas-2.3.2/releasenotes/notes/deprecate-old-model-loading-27aa4485b2132da7.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-23 13:38:11.000000 deepaas-2.3.2/releasenotes/notes/deprecate-openwhisk-be449ddfb9fa554c.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      205 2024-04-23 13:38:11.000000 deepaas-2.3.2/releasenotes/notes/disable-v1-default-dc827ebdd0d90181.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-23 13:38:11.000000 deepaas-2.3.2/releasenotes/notes/initial-documentation-2584128b20eeb9d1.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      602 2024-04-23 13:38:11.000000 deepaas-2.3.2/releasenotes/notes/only-py3-support-928e43ebad4904da.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      652 2024-04-23 13:38:11.000000 deepaas-2.3.2/releasenotes/notes/openwish-proxy-c9c15eef91da0579.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      348 2024-04-23 13:38:11.000000 deepaas-2.3.2/releasenotes/notes/remove-deprecated-get-args-166d8535f5b23c1e.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-23 13:38:11.000000 deepaas-2.3.2/releasenotes/notes/remove-openwhisk-integration-f69978c2824221c3.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2024-04-23 13:38:11.000000 deepaas-2.3.2/releasenotes/notes/remove-v1-api-93dbfcdc2f4beb1d.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2024-04-23 13:38:11.000000 deepaas-2.3.2/releasenotes/notes/training-arguments-4e59dc2945a634a5.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-04-23 13:38:11.000000 deepaas-2.3.2/releasenotes/notes/unify-train-predict-261e92c21d9f47d1.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2088 2024-04-23 13:38:11.000000 deepaas-2.3.2/releasenotes/notes/v2-api-1bc54fcdb42f6c8b.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      812 2024-04-23 13:38:11.000000 deepaas-2.3.2/releasenotes/notes/versioned-api-endpoints-23bf76653d43f033.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-04-23 13:38:11.000000 deepaas-2.3.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1807 2024-04-23 13:38:30.770416 deepaas-2.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2024-04-23 13:38:11.000000 deepaas-2.3.2/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2929 2024-04-23 13:38:11.000000 deepaas-2.3.2/tox.ini
```

### Comparing `deepaas-2.3.1/.github/PULL_REQUEST_TEMPLATE.md` & `deepaas-2.3.2/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `deepaas-2.3.1/.github/workflows/ci.yml` & `deepaas-2.3.2/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `deepaas-2.3.1/.github/workflows/python-publish.yml` & `deepaas-2.3.2/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `deepaas-2.3.1/.github/workflows/release-please.yml` & `deepaas-2.3.2/.github/workflows/release-please.yml`

 * *Files identical despite different names*

### Comparing `deepaas-2.3.1/.readthedocs.yml` & `deepaas-2.3.2/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `deepaas-2.3.1/.sqa/config.yml` & `deepaas-2.3.2/.sqa/config.yml`

 * *Files identical despite different names*

### Comparing `deepaas-2.3.1/CHANGELOG.md` & `deepaas-2.3.2/CHANGELOG.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,16 @@
 # Changelog
 
+## [2.3.2](https://github.com/ai4os/DEEPaaS/compare/v2.3.1...v2.3.2) (2024-04-23)
+
+
+### Bug Fixes
+
+* typo in import ([#149](https://github.com/ai4os/DEEPaaS/issues/149)) ([2c381dd](https://github.com/ai4os/DEEPaaS/commit/2c381dd1163a71e68cc5e38d4d8a98b85755813d))
+
 ## [2.3.1](https://github.com/ai4os/DEEPaaS/compare/v2.3.0...v2.3.1) (2024-03-26)
 
 
 ### Miscellaneous Chores
 
 * release 2.3.1 ([#147](https://github.com/ai4os/DEEPaaS/issues/147)) ([ea9fa64](https://github.com/ai4os/DEEPaaS/commit/ea9fa64a0a7254f94ce06836163ac8664c75d38d))
```

### Comparing `deepaas-2.3.1/CODE_OF_CONDUCT.md` & `deepaas-2.3.2/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `deepaas-2.3.1/CONTRIBUTING.md` & `deepaas-2.3.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `deepaas-2.3.1/Jenkinsfile` & `deepaas-2.3.2/Jenkinsfile`

 * *Files identical despite different names*

### Comparing `deepaas-2.3.1/LICENSE` & `deepaas-2.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `deepaas-2.3.1/Makefile` & `deepaas-2.3.2/Makefile`

 * *Files identical despite different names*

### Comparing `deepaas-2.3.1/PKG-INFO` & `deepaas-2.3.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deepaas
-Version: 2.3.1
+Version: 2.3.2
 Summary: DEEPaaS is a REST API to expose a machine learning model.
 Home-page: https://github.com/indigo-dc/deepaas
 Author: Alvaro Lopez Garcia
 Author-email: aloga@ifca.unican.es
 License: Apache-2
 Project-URL: Bug Tracker, https://github.com/indigo-dc/deepaas/issues
 Project-URL: Documentation, https://deepaas.readthedocs.io/
```

### Comparing `deepaas-2.3.1/README.md` & `deepaas-2.3.2/README.md`

 * *Files identical despite different names*

### Comparing `deepaas-2.3.1/deepaas/__init__.py` & `deepaas-2.3.2/deepaas/__init__.py`

 * *Files identical despite different names*

### Comparing `deepaas-2.3.1/deepaas/api/__init__.py` & `deepaas-2.3.2/deepaas/api/__init__.py`

 * *Files identical despite different names*

### Comparing `deepaas-2.3.1/deepaas/api/v2/__init__.py` & `deepaas-2.3.2/deepaas/api/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `deepaas-2.3.1/deepaas/api/v2/debug.py` & `deepaas-2.3.2/deepaas/api/v2/debug.py`

 * *Files identical despite different names*

### Comparing `deepaas-2.3.1/deepaas/api/v2/models.py` & `deepaas-2.3.2/deepaas/api/v2/models.py`

 * *Files identical despite different names*

### Comparing `deepaas-2.3.1/deepaas/api/v2/predict.py` & `deepaas-2.3.2/deepaas/api/v2/predict.py`

 * *Files identical despite different names*

### Comparing `deepaas-2.3.1/deepaas/api/v2/responses.py` & `deepaas-2.3.2/deepaas/api/v2/responses.py`

 * *Files identical despite different names*

### Comparing `deepaas-2.3.1/deepaas/api/v2/train.py` & `deepaas-2.3.2/deepaas/api/v2/train.py`

 * *Files identical despite different names*

### Comparing `deepaas-2.3.1/deepaas/api/v2/utils.py` & `deepaas-2.3.2/deepaas/api/v2/utils.py`

 * *Files identical despite different names*

### Comparing `deepaas-2.3.1/deepaas/api/versions.py` & `deepaas-2.3.2/deepaas/api/versions.py`

 * *Files identical despite different names*

### Comparing `deepaas-2.3.1/deepaas/cmd/_shutdown.py` & `deepaas-2.3.2/deepaas/cmd/_shutdown.py`

 * *Files identical despite different names*

### Comparing `deepaas-2.3.1/deepaas/cmd/cli.py` & `deepaas-2.3.2/deepaas/cmd/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,16 +29,15 @@
 import uuid
 
 from datetime import datetime
 from marshmallow import fields
 from oslo_config import cfg
 from oslo_log import log
 
-# from deepaas import config
-from deepass import config
+from deepaas import config
 from deepaas.model import loading
 from deepaas.model.v2 import wrapper as v2_wrapper
 
 CONF = config.CONF
 
 debug_cli = False
```

### Comparing `deepaas-2.3.1/deepaas/cmd/execute.py` & `deepaas-2.3.2/deepaas/cmd/execute.py`

 * *Files identical despite different names*

### Comparing `deepaas-2.3.1/deepaas/cmd/run.py` & `deepaas-2.3.2/deepaas/cmd/run.py`

 * *Files identical despite different names*

### Comparing `deepaas-2.3.1/deepaas/config.py` & `deepaas-2.3.2/deepaas/config.py`

 * *Files identical despite different names*

### Comparing `deepaas-2.3.1/deepaas/exceptions.py` & `deepaas-2.3.2/deepaas/exceptions.py`

 * *Files identical despite different names*

### Comparing `deepaas-2.3.1/deepaas/model/__init__.py` & `deepaas-2.3.2/deepaas/model/__init__.py`

 * *Files identical despite different names*

### Comparing `deepaas-2.3.1/deepaas/model/loading.py` & `deepaas-2.3.2/deepaas/model/loading.py`

 * *Files identical despite different names*

### Comparing `deepaas-2.3.1/deepaas/model/v2/__init__.py` & `deepaas-2.3.2/deepaas/model/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `deepaas-2.3.1/deepaas/model/v2/base.py` & `deepaas-2.3.2/deepaas/model/v2/base.py`

 * *Files identical despite different names*

### Comparing `deepaas-2.3.1/deepaas/model/v2/test.py` & `deepaas-2.3.2/deepaas/model/v2/test.py`

 * *Files identical despite different names*

### Comparing `deepaas-2.3.1/deepaas/model/v2/wrapper.py` & `deepaas-2.3.2/deepaas/model/v2/wrapper.py`

 * *Files identical despite different names*

### Comparing `deepaas-2.3.1/deepaas/opts.py` & `deepaas-2.3.2/deepaas/opts.py`

 * *Files identical despite different names*

### Comparing `deepaas-2.3.1/deepaas/tests/base.py` & `deepaas-2.3.2/deepaas/tests/base.py`

 * *Files identical despite different names*

### Comparing `deepaas-2.3.1/deepaas/tests/fake_responses.py` & `deepaas-2.3.2/deepaas/tests/fake_responses.py`

 * *Files identical despite different names*

### Comparing `deepaas-2.3.1/deepaas/tests/test_cmd.py` & `deepaas-2.3.2/deepaas/tests/test_cmd.py`

 * *Files identical despite different names*

### Comparing `deepaas-2.3.1/deepaas/tests/test_v2_api.py` & `deepaas-2.3.2/deepaas/tests/test_v2_api.py`

 * *Files identical despite different names*

### Comparing `deepaas-2.3.1/deepaas/tests/test_v2_models.py` & `deepaas-2.3.2/deepaas/tests/test_v2_models.py`

 * *Files identical despite different names*

### Comparing `deepaas-2.3.1/deepaas/tests/test_versions_api.py` & `deepaas-2.3.2/deepaas/tests/test_versions_api.py`

 * *Files identical despite different names*

### Comparing `deepaas-2.3.1/deepaas/version.py` & `deepaas-2.3.2/deepaas/version.py`

 * *Files identical despite different names*

### Comparing `deepaas-2.3.1/deepaas.egg-info/PKG-INFO` & `deepaas-2.3.2/deepaas.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deepaas
-Version: 2.3.1
+Version: 2.3.2
 Summary: DEEPaaS is a REST API to expose a machine learning model.
 Home-page: https://github.com/indigo-dc/deepaas
 Author: Alvaro Lopez Garcia
 Author-email: aloga@ifca.unican.es
 License: Apache-2
 Project-URL: Bug Tracker, https://github.com/indigo-dc/deepaas/issues
 Project-URL: Documentation, https://deepaas.readthedocs.io/
```

### Comparing `deepaas-2.3.1/deepaas.egg-info/SOURCES.txt` & `deepaas-2.3.2/deepaas.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `deepaas-2.3.1/doc/source/_static/logo-deep-solid-white.png` & `deepaas-2.3.2/doc/source/_static/logo-deep-solid-white.png`

 * *Files identical despite different names*

### Comparing `deepaas-2.3.1/doc/source/_static/logo.png` & `deepaas-2.3.2/doc/source/_static/logo.png`

 * *Files identical despite different names*

### Comparing `deepaas-2.3.1/doc/source/cli/deepaas-cli.rst` & `deepaas-2.3.2/doc/source/cli/deepaas-cli.rst`

 * *Files identical despite different names*

### Comparing `deepaas-2.3.1/doc/source/cli/deepaas-predict.rst` & `deepaas-2.3.2/doc/source/cli/deepaas-predict.rst`

 * *Files identical despite different names*

### Comparing `deepaas-2.3.1/doc/source/cli/deepaas-run.rst` & `deepaas-2.3.2/doc/source/cli/deepaas-run.rst`

 * *Files identical despite different names*

### Comparing `deepaas-2.3.1/doc/source/conf.py` & `deepaas-2.3.2/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `deepaas-2.3.1/doc/source/contributing/code_of_conduct.md` & `deepaas-2.3.2/doc/source/contributing/code_of_conduct.md`

 * *Files identical despite different names*

### Comparing `deepaas-2.3.1/doc/source/contributing/contributing.md` & `deepaas-2.3.2/doc/source/contributing/contributing.md`

 * *Files identical despite different names*

### Comparing `deepaas-2.3.1/doc/source/index.rst` & `deepaas-2.3.2/doc/source/index.rst`

 * *Files identical despite different names*

### Comparing `deepaas-2.3.1/doc/source/install/configuration/sample.rst` & `deepaas-2.3.2/doc/source/install/configuration/sample.rst`

 * *Files identical despite different names*

### Comparing `deepaas-2.3.1/doc/source/install/installation.rst` & `deepaas-2.3.2/doc/source/install/installation.rst`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 Installation
 ============
 
 The recommended way to install the DEEPaaS API is with ``pip``:
 
 .. code-block:: console
 
-   pip install deepass
+   pip install deepaas
 
 This way you will ensure that the stable version is fetched from pip, rather
 than development or unstable version
 
 Installing the development version
 ----------------------------------
```

### Comparing `deepaas-2.3.1/doc/source/install/upgrade.rst` & `deepaas-2.3.2/doc/source/install/upgrade.rst`

 * *Files identical despite different names*

### Comparing `deepaas-2.3.1/doc/source/user/predict.rst` & `deepaas-2.3.2/doc/source/user/predict.rst`

 * *Files identical despite different names*

### Comparing `deepaas-2.3.1/doc/source/user/quickstart.rst` & `deepaas-2.3.2/doc/source/user/quickstart.rst`

 * *Files identical despite different names*

### Comparing `deepaas-2.3.1/doc/source/user/v2-api.rst` & `deepaas-2.3.2/doc/source/user/v2-api.rst`

 * *Files identical despite different names*

### Comparing `deepaas-2.3.1/paper/deepaas.png` & `deepaas-2.3.2/paper/deepaas.png`

 * *Files identical despite different names*

### Comparing `deepaas-2.3.1/paper/paper.bib` & `deepaas-2.3.2/paper/paper.bib`

 * *Files identical despite different names*

### Comparing `deepaas-2.3.1/paper/paper.md` & `deepaas-2.3.2/paper/paper.md`

 * *Files identical despite different names*

### Comparing `deepaas-2.3.1/releasenotes/notes/only-py3-support-928e43ebad4904da.yaml` & `deepaas-2.3.2/releasenotes/notes/only-py3-support-928e43ebad4904da.yaml`

 * *Files identical despite different names*

### Comparing `deepaas-2.3.1/releasenotes/notes/openwish-proxy-c9c15eef91da0579.yaml` & `deepaas-2.3.2/releasenotes/notes/openwish-proxy-c9c15eef91da0579.yaml`

 * *Files identical despite different names*

### Comparing `deepaas-2.3.1/releasenotes/notes/v2-api-1bc54fcdb42f6c8b.yaml` & `deepaas-2.3.2/releasenotes/notes/v2-api-1bc54fcdb42f6c8b.yaml`

 * *Files identical despite different names*

### Comparing `deepaas-2.3.1/releasenotes/notes/versioned-api-endpoints-23bf76653d43f033.yaml` & `deepaas-2.3.2/releasenotes/notes/versioned-api-endpoints-23bf76653d43f033.yaml`

 * *Files identical despite different names*

### Comparing `deepaas-2.3.1/setup.cfg` & `deepaas-2.3.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `deepaas-2.3.1/setup.py` & `deepaas-2.3.2/setup.py`

 * *Files identical despite different names*

### Comparing `deepaas-2.3.1/tox.ini` & `deepaas-2.3.2/tox.ini`

 * *Files identical despite different names*

