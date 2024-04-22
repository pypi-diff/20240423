# Comparing `tmp/adafruit_circuitpython_wiznet5k-5.1.0.tar.gz` & `tmp/adafruit_circuitpython_wiznet5k-5.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit_circuitpython_wiznet5k-5.1.0.tar", last modified: Mon Apr 22 16:52:38 2024, max compression
+gzip compressed data, was "adafruit_circuitpython_wiznet5k-5.1.1.tar", last modified: Mon Apr 22 20:40:10 2024, max compression
```

## Comparing `adafruit_circuitpython_wiznet5k-5.1.0.tar` & `adafruit_circuitpython_wiznet5k-5.1.1.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 16:52:38.476480 adafruit_circuitpython_wiznet5k-5.1.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 16:52:38.468480 adafruit_circuitpython_wiznet5k-5.1.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 16:52:38.468480 adafruit_circuitpython_wiznet5k-5.1.0/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      880 2024-04-22 16:52:27.000000 adafruit_circuitpython_wiznet5k-5.1.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 16:52:38.472480 adafruit_circuitpython_wiznet5k-5.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-22 16:52:27.000000 adafruit_circuitpython_wiznet5k-5.1.0/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (127)      479 2024-04-22 16:52:27.000000 adafruit_circuitpython_wiznet5k-5.1.0/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (127)      482 2024-04-22 16:52:27.000000 adafruit_circuitpython_wiznet5k-5.1.0/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (127)      475 2024-04-22 16:52:27.000000 adafruit_circuitpython_wiznet5k-5.1.0/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-04-22 16:52:27.000000 adafruit_circuitpython_wiznet5k-5.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-04-22 16:52:27.000000 adafruit_circuitpython_wiznet5k-5.1.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    13078 2024-04-22 16:52:27.000000 adafruit_circuitpython_wiznet5k-5.1.0/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (127)      388 2024-04-22 16:52:27.000000 adafruit_circuitpython_wiznet5k-5.1.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     6147 2024-04-22 16:52:27.000000 adafruit_circuitpython_wiznet5k-5.1.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)      750 2024-04-22 16:52:27.000000 adafruit_circuitpython_wiznet5k-5.1.0/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 16:52:38.472480 adafruit_circuitpython_wiznet5k-5.1.0/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (127)    16814 2024-04-22 16:52:27.000000 adafruit_circuitpython_wiznet5k-5.1.0/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-04-22 16:52:27.000000 adafruit_circuitpython_wiznet5k-5.1.0/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-04-22 16:52:27.000000 adafruit_circuitpython_wiznet5k-5.1.0/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (127)     7402 2024-04-22 16:52:38.476480 adafruit_circuitpython_wiznet5k-5.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6490 2024-04-22 16:52:27.000000 adafruit_circuitpython_wiznet5k-5.1.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-22 16:52:27.000000 adafruit_circuitpython_wiznet5k-5.1.0/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 16:52:38.476480 adafruit_circuitpython_wiznet5k-5.1.0/adafruit_circuitpython_wiznet5k.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7402 2024-04-22 16:52:38.000000 adafruit_circuitpython_wiznet5k-5.1.0/adafruit_circuitpython_wiznet5k.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-04-22 16:52:38.000000 adafruit_circuitpython_wiznet5k-5.1.0/adafruit_circuitpython_wiznet5k.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 16:52:38.000000 adafruit_circuitpython_wiznet5k-5.1.0/adafruit_circuitpython_wiznet5k.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-22 16:52:38.000000 adafruit_circuitpython_wiznet5k-5.1.0/adafruit_circuitpython_wiznet5k.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-22 16:52:38.000000 adafruit_circuitpython_wiznet5k-5.1.0/adafruit_circuitpython_wiznet5k.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 16:52:38.472480 adafruit_circuitpython_wiznet5k-5.1.0/adafruit_wiznet5k/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 16:52:35.000000 adafruit_circuitpython_wiznet5k-5.1.0/adafruit_wiznet5k/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    51901 2024-04-22 16:52:35.000000 adafruit_circuitpython_wiznet5k-5.1.0/adafruit_wiznet5k/adafruit_wiznet5k.py
--rw-r--r--   0 runner    (1001) docker     (127)     1360 2024-04-22 16:52:35.000000 adafruit_circuitpython_wiznet5k-5.1.0/adafruit_wiznet5k/adafruit_wiznet5k_debug.py
--rw-r--r--   0 runner    (1001) docker     (127)    26273 2024-04-22 16:52:35.000000 adafruit_circuitpython_wiznet5k-5.1.0/adafruit_wiznet5k/adafruit_wiznet5k_dhcp.py
--rw-r--r--   0 runner    (1001) docker     (127)    11431 2024-04-22 16:52:35.000000 adafruit_circuitpython_wiznet5k-5.1.0/adafruit_wiznet5k/adafruit_wiznet5k_dns.py
--rw-r--r--   0 runner    (1001) docker     (127)    28809 2024-04-22 16:52:35.000000 adafruit_circuitpython_wiznet5k-5.1.0/adafruit_wiznet5k/adafruit_wiznet5k_socket.py
--rw-r--r--   0 runner    (1001) docker     (127)     9002 2024-04-22 16:52:35.000000 adafruit_circuitpython_wiznet5k-5.1.0/adafruit_wiznet5k/adafruit_wiznet5k_wsgiserver.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 16:52:38.472480 adafruit_circuitpython_wiznet5k-5.1.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 16:52:38.476480 adafruit_circuitpython_wiznet5k-5.1.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)     4414 2024-04-22 16:52:27.000000 adafruit_circuitpython_wiznet5k-5.1.0/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-22 16:52:27.000000 adafruit_circuitpython_wiznet5k-5.1.0/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-22 16:52:27.000000 adafruit_circuitpython_wiznet5k-5.1.0/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-22 16:52:27.000000 adafruit_circuitpython_wiznet5k-5.1.0/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (127)     5541 2024-04-22 16:52:27.000000 adafruit_circuitpython_wiznet5k-5.1.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-22 16:52:27.000000 adafruit_circuitpython_wiznet5k-5.1.0/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-22 16:52:27.000000 adafruit_circuitpython_wiznet5k-5.1.0/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (127)      975 2024-04-22 16:52:27.000000 adafruit_circuitpython_wiznet5k-5.1.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-22 16:52:27.000000 adafruit_circuitpython_wiznet5k-5.1.0/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-22 16:52:27.000000 adafruit_circuitpython_wiznet5k-5.1.0/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 16:52:38.476480 adafruit_circuitpython_wiznet5k-5.1.0/examples/
--rw-r--r--   0 runner    (1001) docker     (127)     1356 2024-04-22 16:52:35.000000 adafruit_circuitpython_wiznet5k-5.1.0/examples/wiznet5k_aio_post.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2159 2024-04-22 16:52:35.000000 adafruit_circuitpython_wiznet5k-5.1.0/examples/wiznet5k_cheerlights.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1085 2024-04-22 16:52:35.000000 adafruit_circuitpython_wiznet5k-5.1.0/examples/wiznet5k_cpython_client_for_simpleserver.py
--rw-r--r--   0 runner    (1001) docker     (127)      963 2024-04-22 16:52:35.000000 adafruit_circuitpython_wiznet5k-5.1.0/examples/wiznet5k_httpserver.py
--rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-04-22 16:52:35.000000 adafruit_circuitpython_wiznet5k-5.1.0/examples/wiznet5k_simpleserver.py
--rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-04-22 16:52:35.000000 adafruit_circuitpython_wiznet5k-5.1.0/examples/wiznet5k_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1435 2024-04-22 16:52:35.000000 adafruit_circuitpython_wiznet5k-5.1.0/examples/wiznet5k_simpletest_manual_network.py
--rw-r--r--   0 runner    (1001) docker     (127)     4193 2024-04-22 16:52:35.000000 adafruit_circuitpython_wiznet5k-5.1.0/examples/wiznet5k_wsgiserver.py
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-22 16:52:27.000000 adafruit_circuitpython_wiznet5k-5.1.0/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1270 2024-04-22 16:52:35.000000 adafruit_circuitpython_wiznet5k-5.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-22 16:52:27.000000 adafruit_circuitpython_wiznet5k-5.1.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 16:52:38.476480 adafruit_circuitpython_wiznet5k-5.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 20:40:10.821188 adafruit_circuitpython_wiznet5k-5.1.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 20:40:10.809188 adafruit_circuitpython_wiznet5k-5.1.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 20:40:10.813188 adafruit_circuitpython_wiznet5k-5.1.1/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      880 2024-04-22 20:40:01.000000 adafruit_circuitpython_wiznet5k-5.1.1/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 20:40:10.813188 adafruit_circuitpython_wiznet5k-5.1.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-22 20:40:01.000000 adafruit_circuitpython_wiznet5k-5.1.1/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-04-22 20:40:01.000000 adafruit_circuitpython_wiznet5k-5.1.1/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      482 2024-04-22 20:40:01.000000 adafruit_circuitpython_wiznet5k-5.1.1/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-04-22 20:40:01.000000 adafruit_circuitpython_wiznet5k-5.1.1/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-04-22 20:40:01.000000 adafruit_circuitpython_wiznet5k-5.1.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-04-22 20:40:01.000000 adafruit_circuitpython_wiznet5k-5.1.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    13078 2024-04-22 20:40:01.000000 adafruit_circuitpython_wiznet5k-5.1.1/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-04-22 20:40:01.000000 adafruit_circuitpython_wiznet5k-5.1.1/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     6147 2024-04-22 20:40:01.000000 adafruit_circuitpython_wiznet5k-5.1.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)      750 2024-04-22 20:40:01.000000 adafruit_circuitpython_wiznet5k-5.1.1/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 20:40:10.813188 adafruit_circuitpython_wiznet5k-5.1.1/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (127)    16814 2024-04-22 20:40:01.000000 adafruit_circuitpython_wiznet5k-5.1.1/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-04-22 20:40:01.000000 adafruit_circuitpython_wiznet5k-5.1.1/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-04-22 20:40:01.000000 adafruit_circuitpython_wiznet5k-5.1.1/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     7402 2024-04-22 20:40:10.821188 adafruit_circuitpython_wiznet5k-5.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6490 2024-04-22 20:40:01.000000 adafruit_circuitpython_wiznet5k-5.1.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-22 20:40:01.000000 adafruit_circuitpython_wiznet5k-5.1.1/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 20:40:10.821188 adafruit_circuitpython_wiznet5k-5.1.1/adafruit_circuitpython_wiznet5k.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7402 2024-04-22 20:40:10.000000 adafruit_circuitpython_wiznet5k-5.1.1/adafruit_circuitpython_wiznet5k.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-04-22 20:40:10.000000 adafruit_circuitpython_wiznet5k-5.1.1/adafruit_circuitpython_wiznet5k.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 20:40:10.000000 adafruit_circuitpython_wiznet5k-5.1.1/adafruit_circuitpython_wiznet5k.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-22 20:40:10.000000 adafruit_circuitpython_wiznet5k-5.1.1/adafruit_circuitpython_wiznet5k.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-22 20:40:10.000000 adafruit_circuitpython_wiznet5k-5.1.1/adafruit_circuitpython_wiznet5k.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 20:40:10.817188 adafruit_circuitpython_wiznet5k-5.1.1/adafruit_wiznet5k/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 20:40:08.000000 adafruit_circuitpython_wiznet5k-5.1.1/adafruit_wiznet5k/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51901 2024-04-22 20:40:08.000000 adafruit_circuitpython_wiznet5k-5.1.1/adafruit_wiznet5k/adafruit_wiznet5k.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1360 2024-04-22 20:40:08.000000 adafruit_circuitpython_wiznet5k-5.1.1/adafruit_wiznet5k/adafruit_wiznet5k_debug.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26273 2024-04-22 20:40:08.000000 adafruit_circuitpython_wiznet5k-5.1.1/adafruit_wiznet5k/adafruit_wiznet5k_dhcp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11431 2024-04-22 20:40:08.000000 adafruit_circuitpython_wiznet5k-5.1.1/adafruit_wiznet5k/adafruit_wiznet5k_dns.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28954 2024-04-22 20:40:08.000000 adafruit_circuitpython_wiznet5k-5.1.1/adafruit_wiznet5k/adafruit_wiznet5k_socket.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9002 2024-04-22 20:40:08.000000 adafruit_circuitpython_wiznet5k-5.1.1/adafruit_wiznet5k/adafruit_wiznet5k_wsgiserver.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 20:40:10.817188 adafruit_circuitpython_wiznet5k-5.1.1/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 20:40:10.817188 adafruit_circuitpython_wiznet5k-5.1.1/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)     4414 2024-04-22 20:40:01.000000 adafruit_circuitpython_wiznet5k-5.1.1/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-22 20:40:01.000000 adafruit_circuitpython_wiznet5k-5.1.1/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-22 20:40:01.000000 adafruit_circuitpython_wiznet5k-5.1.1/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-22 20:40:01.000000 adafruit_circuitpython_wiznet5k-5.1.1/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (127)     5541 2024-04-22 20:40:01.000000 adafruit_circuitpython_wiznet5k-5.1.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-22 20:40:01.000000 adafruit_circuitpython_wiznet5k-5.1.1/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-22 20:40:01.000000 adafruit_circuitpython_wiznet5k-5.1.1/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (127)      975 2024-04-22 20:40:01.000000 adafruit_circuitpython_wiznet5k-5.1.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-22 20:40:01.000000 adafruit_circuitpython_wiznet5k-5.1.1/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-22 20:40:01.000000 adafruit_circuitpython_wiznet5k-5.1.1/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 20:40:10.821188 adafruit_circuitpython_wiznet5k-5.1.1/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     1356 2024-04-22 20:40:08.000000 adafruit_circuitpython_wiznet5k-5.1.1/examples/wiznet5k_aio_post.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2159 2024-04-22 20:40:08.000000 adafruit_circuitpython_wiznet5k-5.1.1/examples/wiznet5k_cheerlights.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1085 2024-04-22 20:40:08.000000 adafruit_circuitpython_wiznet5k-5.1.1/examples/wiznet5k_cpython_client_for_simpleserver.py
+-rw-r--r--   0 runner    (1001) docker     (127)      963 2024-04-22 20:40:08.000000 adafruit_circuitpython_wiznet5k-5.1.1/examples/wiznet5k_httpserver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-04-22 20:40:08.000000 adafruit_circuitpython_wiznet5k-5.1.1/examples/wiznet5k_simpleserver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-04-22 20:40:08.000000 adafruit_circuitpython_wiznet5k-5.1.1/examples/wiznet5k_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1435 2024-04-22 20:40:08.000000 adafruit_circuitpython_wiznet5k-5.1.1/examples/wiznet5k_simpletest_manual_network.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4193 2024-04-22 20:40:08.000000 adafruit_circuitpython_wiznet5k-5.1.1/examples/wiznet5k_wsgiserver.py
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-22 20:40:01.000000 adafruit_circuitpython_wiznet5k-5.1.1/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1270 2024-04-22 20:40:08.000000 adafruit_circuitpython_wiznet5k-5.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-22 20:40:01.000000 adafruit_circuitpython_wiznet5k-5.1.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 20:40:10.821188 adafruit_circuitpython_wiznet5k-5.1.1/setup.cfg
```

### Comparing `adafruit_circuitpython_wiznet5k-5.1.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit_circuitpython_wiznet5k-5.1.1/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_wiznet5k-5.1.0/.gitignore` & `adafruit_circuitpython_wiznet5k-5.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_wiznet5k-5.1.0/.pre-commit-config.yaml` & `adafruit_circuitpython_wiznet5k-5.1.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_wiznet5k-5.1.0/.pylintrc` & `adafruit_circuitpython_wiznet5k-5.1.1/.pylintrc`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_wiznet5k-5.1.0/CODE_OF_CONDUCT.md` & `adafruit_circuitpython_wiznet5k-5.1.1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_wiznet5k-5.1.0/LICENSE` & `adafruit_circuitpython_wiznet5k-5.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_wiznet5k-5.1.0/LICENSES/CC-BY-4.0.txt` & `adafruit_circuitpython_wiznet5k-5.1.1/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_wiznet5k-5.1.0/LICENSES/MIT.txt` & `adafruit_circuitpython_wiznet5k-5.1.1/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_wiznet5k-5.1.0/LICENSES/Unlicense.txt` & `adafruit_circuitpython_wiznet5k-5.1.1/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_wiznet5k-5.1.0/PKG-INFO` & `adafruit_circuitpython_wiznet5k-5.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-wiznet5k
-Version: 5.1.0
+Version: 5.1.1
 Summary: Pure-Python interface for WIZNET 5k ethernet modules.
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_Wiznet5k
 Keywords: adafruit,blinka,circuitpython,micropython,wiznet5k,ethernet,,wiznet,,w5500,,w5200,,internet,,iot
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit_circuitpython_wiznet5k-5.1.0/README.rst` & `adafruit_circuitpython_wiznet5k-5.1.1/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_wiznet5k-5.1.0/adafruit_circuitpython_wiznet5k.egg-info/PKG-INFO` & `adafruit_circuitpython_wiznet5k-5.1.1/adafruit_circuitpython_wiznet5k.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-wiznet5k
-Version: 5.1.0
+Version: 5.1.1
 Summary: Pure-Python interface for WIZNET 5k ethernet modules.
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_Wiznet5k
 Keywords: adafruit,blinka,circuitpython,micropython,wiznet5k,ethernet,,wiznet,,w5500,,w5200,,internet,,iot
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit_circuitpython_wiznet5k-5.1.0/adafruit_circuitpython_wiznet5k.egg-info/SOURCES.txt` & `adafruit_circuitpython_wiznet5k-5.1.1/adafruit_circuitpython_wiznet5k.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_wiznet5k-5.1.0/adafruit_wiznet5k/adafruit_wiznet5k.py` & `adafruit_circuitpython_wiznet5k-5.1.1/adafruit_wiznet5k/adafruit_wiznet5k.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,15 +40,15 @@
         import digitalio
 
         IpAddress4Raw = Union[bytes, Tuple[int, int, int, int]]
         MacAddressRaw = Union[bytes, Tuple[int, int, int, int, int, int]]
 except ImportError:
     pass
 
-__version__ = "5.1.0"
+__version__ = "5.1.1"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_Wiznet5k.git"
 
 from random import randint
 import time
 import gc
 from micropython import const
 from adafruit_ticks import ticks_ms, ticks_diff
```

### Comparing `adafruit_circuitpython_wiznet5k-5.1.0/adafruit_wiznet5k/adafruit_wiznet5k_debug.py` & `adafruit_circuitpython_wiznet5k-5.1.1/adafruit_wiznet5k/adafruit_wiznet5k_debug.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_wiznet5k-5.1.0/adafruit_wiznet5k/adafruit_wiznet5k_dhcp.py` & `adafruit_circuitpython_wiznet5k-5.1.1/adafruit_wiznet5k/adafruit_wiznet5k_dhcp.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_wiznet5k-5.1.0/adafruit_wiznet5k/adafruit_wiznet5k_dns.py` & `adafruit_circuitpython_wiznet5k-5.1.1/adafruit_wiznet5k/adafruit_wiznet5k_dns.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_wiznet5k-5.1.0/adafruit_wiznet5k/adafruit_wiznet5k_socket.py` & `adafruit_circuitpython_wiznet5k-5.1.1/adafruit_wiznet5k/adafruit_wiznet5k_socket.py`

 * *Files 0% similar despite different names*

```diff
@@ -402,14 +402,17 @@
             wiznet5k.adafruit_wiznet5k.SNSR_SOCK_ESTABLISHED,
         ):
             if (
                 self._timeout
                 and 0 < self._timeout < ticks_diff(ticks_ms(), stamp) / 1000
             ):
                 raise TimeoutError("Failed to accept connection.")
+            if self._status == wiznet5k.adafruit_wiznet5k.SNSR_SOCK_CLOSE_WAIT:
+                self._disconnect()
+                self.listen()
             if self._status == wiznet5k.adafruit_wiznet5k.SNSR_SOCK_CLOSED:
                 self.close()
                 self.listen()
 
         _, addr = _the_interface.socket_accept(self._socknum)
         current_socknum = self._socknum
         # Create a new socket object and swap socket nums, so we can continue listening
```

### Comparing `adafruit_circuitpython_wiznet5k-5.1.0/adafruit_wiznet5k/adafruit_wiznet5k_wsgiserver.py` & `adafruit_circuitpython_wiznet5k-5.1.1/adafruit_wiznet5k/adafruit_wiznet5k_wsgiserver.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_wiznet5k-5.1.0/docs/_static/favicon.ico` & `adafruit_circuitpython_wiznet5k-5.1.1/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_wiznet5k-5.1.0/docs/api.rst` & `adafruit_circuitpython_wiznet5k-5.1.1/docs/api.rst`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_wiznet5k-5.1.0/docs/conf.py` & `adafruit_circuitpython_wiznet5k-5.1.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_wiznet5k-5.1.0/docs/index.rst` & `adafruit_circuitpython_wiznet5k-5.1.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_wiznet5k-5.1.0/examples/wiznet5k_aio_post.py` & `adafruit_circuitpython_wiznet5k-5.1.1/examples/wiznet5k_aio_post.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_wiznet5k-5.1.0/examples/wiznet5k_cheerlights.py` & `adafruit_circuitpython_wiznet5k-5.1.1/examples/wiznet5k_cheerlights.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_wiznet5k-5.1.0/examples/wiznet5k_cpython_client_for_simpleserver.py` & `adafruit_circuitpython_wiznet5k-5.1.1/examples/wiznet5k_cpython_client_for_simpleserver.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_wiznet5k-5.1.0/examples/wiznet5k_httpserver.py` & `adafruit_circuitpython_wiznet5k-5.1.1/examples/wiznet5k_httpserver.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_wiznet5k-5.1.0/examples/wiznet5k_simpleserver.py` & `adafruit_circuitpython_wiznet5k-5.1.1/examples/wiznet5k_simpleserver.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_wiznet5k-5.1.0/examples/wiznet5k_simpletest.py` & `adafruit_circuitpython_wiznet5k-5.1.1/examples/wiznet5k_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_wiznet5k-5.1.0/examples/wiznet5k_simpletest_manual_network.py` & `adafruit_circuitpython_wiznet5k-5.1.1/examples/wiznet5k_simpletest_manual_network.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_wiznet5k-5.1.0/examples/wiznet5k_wsgiserver.py` & `adafruit_circuitpython_wiznet5k-5.1.1/examples/wiznet5k_wsgiserver.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_wiznet5k-5.1.0/pyproject.toml` & `adafruit_circuitpython_wiznet5k-5.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-wiznet5k"
 description = "Pure-Python interface for WIZNET 5k ethernet modules."
-version = "5.1.0"
+version = "5.1.1"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_Wiznet5k"}
 keywords = [
     "adafruit",
```

