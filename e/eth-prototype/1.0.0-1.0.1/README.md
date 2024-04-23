# Comparing `tmp/eth-prototype-1.0.0.tar.gz` & `tmp/eth_prototype-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eth-prototype-1.0.0.tar", last modified: Thu Feb 15 22:29:46 2024, max compression
+gzip compressed data, was "eth_prototype-1.0.1.tar", last modified: Tue Apr 23 15:55:34 2024, max compression
```

## Comparing `eth-prototype-1.0.0.tar` & `eth_prototype-1.0.1.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 22:29:46.138220 eth-prototype-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)      591 2024-02-15 22:29:33.000000 eth-prototype-1.0.0/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 22:29:46.122220 eth-prototype-1.0.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 22:29:46.126220 eth-prototype-1.0.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-02-15 22:29:33.000000 eth-prototype-1.0.0/.github/workflows/publish.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      765 2024-02-15 22:29:33.000000 eth-prototype-1.0.0/.github/workflows/test.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      675 2024-02-15 22:29:33.000000 eth-prototype-1.0.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-02-15 22:29:33.000000 eth-prototype-1.0.0/.isort.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-02-15 22:29:33.000000 eth-prototype-1.0.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      461 2024-02-15 22:29:33.000000 eth-prototype-1.0.0/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-02-15 22:29:33.000000 eth-prototype-1.0.0/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-02-15 22:29:33.000000 eth-prototype-1.0.0/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-02-15 22:29:33.000000 eth-prototype-1.0.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2648 2024-02-15 22:29:46.138220 eth-prototype-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-02-15 22:29:33.000000 eth-prototype-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 22:29:46.130220 eth-prototype-1.0.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-02-15 22:29:33.000000 eth-prototype-1.0.0/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 22:29:46.130220 eth-prototype-1.0.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-02-15 22:29:33.000000 eth-prototype-1.0.0/docs/_static/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-02-15 22:29:33.000000 eth-prototype-1.0.0/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-02-15 22:29:33.000000 eth-prototype-1.0.0/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (127)     9506 2024-02-15 22:29:33.000000 eth-prototype-1.0.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     2266 2024-02-15 22:29:33.000000 eth-prototype-1.0.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-02-15 22:29:33.000000 eth-prototype-1.0.0/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-02-15 22:29:33.000000 eth-prototype-1.0.0/docs/readme.rst
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-02-15 22:29:33.000000 eth-prototype-1.0.0/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      343 2024-02-15 22:29:33.000000 eth-prototype-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1398 2024-02-15 22:29:46.138220 eth-prototype-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      710 2024-02-15 22:29:33.000000 eth-prototype-1.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 22:29:46.122220 eth-prototype-1.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 22:29:46.138220 eth-prototype-1.0.0/src/eth_prototype.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2648 2024-02-15 22:29:46.000000 eth-prototype-1.0.0/src/eth_prototype.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1642 2024-02-15 22:29:46.000000 eth-prototype-1.0.0/src/eth_prototype.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-15 22:29:46.000000 eth-prototype-1.0.0/src/eth_prototype.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-15 22:29:45.000000 eth-prototype-1.0.0/src/eth_prototype.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      231 2024-02-15 22:29:46.000000 eth-prototype-1.0.0/src/eth_prototype.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-02-15 22:29:46.000000 eth-prototype-1.0.0/src/eth_prototype.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 22:29:46.130220 eth-prototype-1.0.0/src/ethproto/
--rw-r--r--   0 runner    (1001) docker     (127)      579 2024-02-15 22:29:33.000000 eth-prototype-1.0.0/src/ethproto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5578 2024-02-15 22:29:33.000000 eth-prototype-1.0.0/src/ethproto/build_artifacts.py
--rw-r--r--   0 runner    (1001) docker     (127)    18662 2024-02-15 22:29:33.000000 eth-prototype-1.0.0/src/ethproto/contracts.py
--rw-r--r--   0 runner    (1001) docker     (127)     1777 2024-02-15 22:29:33.000000 eth-prototype-1.0.0/src/ethproto/defender_relay.py
--rw-r--r--   0 runner    (1001) docker     (127)    20445 2024-02-15 22:29:33.000000 eth-prototype-1.0.0/src/ethproto/w3wrappers.py
--rw-r--r--   0 runner    (1001) docker     (127)     8262 2024-02-15 22:29:33.000000 eth-prototype-1.0.0/src/ethproto/wadray.py
--rw-r--r--   0 runner    (1001) docker     (127)    17448 2024-02-15 22:29:33.000000 eth-prototype-1.0.0/src/ethproto/wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 22:29:46.134220 eth-prototype-1.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-02-15 22:29:33.000000 eth-prototype-1.0.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 22:29:46.134220 eth-prototype-1.0.0/tests/hardhat-project/
--rw-r--r--   0 runner    (1001) docker     (127)      352 2024-02-15 22:29:33.000000 eth-prototype-1.0.0/tests/hardhat-project/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 22:29:46.122220 eth-prototype-1.0.0/tests/hardhat-project/artifacts2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 22:29:46.134220 eth-prototype-1.0.0/tests/hardhat-project/artifacts2/TestCurrency.sol/
--rw-r--r--   0 runner    (1001) docker     (127)    29097 2024-02-15 22:29:33.000000 eth-prototype-1.0.0/tests/hardhat-project/artifacts2/TestCurrency.sol/TestCurrency.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 22:29:46.134220 eth-prototype-1.0.0/tests/hardhat-project/contracts/
--rw-r--r--   0 runner    (1001) docker     (127)      340 2024-02-15 22:29:33.000000 eth-prototype-1.0.0/tests/hardhat-project/contracts/Count.sol
--rw-r--r--   0 runner    (1001) docker     (127)      319 2024-02-15 22:29:33.000000 eth-prototype-1.0.0/tests/hardhat-project/contracts/Counter.sol
--rw-r--r--   0 runner    (1001) docker     (127)      822 2024-02-15 22:29:33.000000 eth-prototype-1.0.0/tests/hardhat-project/contracts/CounterUpgradeable.sol
--rw-r--r--   0 runner    (1001) docker     (127)      995 2024-02-15 22:29:33.000000 eth-prototype-1.0.0/tests/hardhat-project/contracts/CounterUpgradeableWithLibrary.sol
--rw-r--r--   0 runner    (1001) docker     (127)      523 2024-02-15 22:29:33.000000 eth-prototype-1.0.0/tests/hardhat-project/contracts/CounterWithLibrary.sol
--rw-r--r--   0 runner    (1001) docker     (127)      365 2024-02-15 22:29:33.000000 eth-prototype-1.0.0/tests/hardhat-project/contracts/Datatypes.sol
--rw-r--r--   0 runner    (1001) docker     (127)      713 2024-02-15 22:29:33.000000 eth-prototype-1.0.0/tests/hardhat-project/contracts/TestCurrency.sol
--rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-02-15 22:29:33.000000 eth-prototype-1.0.0/tests/hardhat-project/contracts/TestCurrencyUUPS.sol
--rw-r--r--   0 runner    (1001) docker     (127)      657 2024-02-15 22:29:33.000000 eth-prototype-1.0.0/tests/hardhat-project/contracts/TestNFT.sol
--rw-r--r--   0 runner    (1001) docker     (127)      376 2024-02-15 22:29:33.000000 eth-prototype-1.0.0/tests/hardhat-project/hardhat.config.js
--rw-r--r--   0 runner    (1001) docker     (127)   631590 2024-02-15 22:29:33.000000 eth-prototype-1.0.0/tests/hardhat-project/package-lock.json
--rw-r--r--   0 runner    (1001) docker     (127)      650 2024-02-15 22:29:33.000000 eth-prototype-1.0.0/tests/hardhat-project/package.json
--rw-r--r--   0 runner    (1001) docker     (127)     4472 2024-02-15 22:29:33.000000 eth-prototype-1.0.0/tests/test_build_artifacts.py
--rw-r--r--   0 runner    (1001) docker     (127)    10408 2024-02-15 22:29:33.000000 eth-prototype-1.0.0/tests/test_contracts.py
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-02-15 22:29:33.000000 eth-prototype-1.0.0/tests/test_defender.py
--rw-r--r--   0 runner    (1001) docker     (127)      480 2024-02-15 22:29:33.000000 eth-prototype-1.0.0/tests/test_time_control.py
--rw-r--r--   0 runner    (1001) docker     (127)     2214 2024-02-15 22:29:33.000000 eth-prototype-1.0.0/tests/test_w3.py
--rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-02-15 22:29:33.000000 eth-prototype-1.0.0/tests/test_wadray.py
--rw-r--r--   0 runner    (1001) docker     (127)     2555 2024-02-15 22:29:33.000000 eth-prototype-1.0.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 15:55:34.456576 eth_prototype-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      591 2024-04-23 15:55:28.000000 eth_prototype-1.0.1/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 15:55:34.440576 eth_prototype-1.0.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 15:55:34.444576 eth_prototype-1.0.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-04-23 15:55:28.000000 eth_prototype-1.0.1/.github/workflows/publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      759 2024-04-23 15:55:28.000000 eth_prototype-1.0.1/.github/workflows/test.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      675 2024-04-23 15:55:28.000000 eth_prototype-1.0.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-23 15:55:28.000000 eth_prototype-1.0.1/.isort.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-04-23 15:55:28.000000 eth_prototype-1.0.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      461 2024-04-23 15:55:28.000000 eth_prototype-1.0.1/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-23 15:55:28.000000 eth_prototype-1.0.1/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-23 15:55:28.000000 eth_prototype-1.0.1/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-04-23 15:55:28.000000 eth_prototype-1.0.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2654 2024-04-23 15:55:34.456576 eth_prototype-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-04-23 15:55:28.000000 eth_prototype-1.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 15:55:34.448576 eth_prototype-1.0.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-04-23 15:55:28.000000 eth_prototype-1.0.1/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 15:55:34.448576 eth_prototype-1.0.1/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-23 15:55:28.000000 eth_prototype-1.0.1/docs/_static/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-23 15:55:28.000000 eth_prototype-1.0.1/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-23 15:55:28.000000 eth_prototype-1.0.1/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     9506 2024-04-23 15:55:28.000000 eth_prototype-1.0.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2266 2024-04-23 15:55:28.000000 eth_prototype-1.0.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-23 15:55:28.000000 eth_prototype-1.0.1/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-23 15:55:28.000000 eth_prototype-1.0.1/docs/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-04-23 15:55:28.000000 eth_prototype-1.0.1/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2024-04-23 15:55:28.000000 eth_prototype-1.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1404 2024-04-23 15:55:34.456576 eth_prototype-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      710 2024-04-23 15:55:28.000000 eth_prototype-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 15:55:34.440576 eth_prototype-1.0.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 15:55:34.452576 eth_prototype-1.0.1/src/eth_prototype.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2654 2024-04-23 15:55:34.000000 eth_prototype-1.0.1/src/eth_prototype.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1642 2024-04-23 15:55:34.000000 eth_prototype-1.0.1/src/eth_prototype.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 15:55:34.000000 eth_prototype-1.0.1/src/eth_prototype.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 15:55:34.000000 eth_prototype-1.0.1/src/eth_prototype.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-04-23 15:55:34.000000 eth_prototype-1.0.1/src/eth_prototype.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-23 15:55:34.000000 eth_prototype-1.0.1/src/eth_prototype.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 15:55:34.448576 eth_prototype-1.0.1/src/ethproto/
+-rw-r--r--   0 runner    (1001) docker     (127)      579 2024-04-23 15:55:28.000000 eth_prototype-1.0.1/src/ethproto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5578 2024-04-23 15:55:28.000000 eth_prototype-1.0.1/src/ethproto/build_artifacts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18662 2024-04-23 15:55:28.000000 eth_prototype-1.0.1/src/ethproto/contracts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1777 2024-04-23 15:55:28.000000 eth_prototype-1.0.1/src/ethproto/defender_relay.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20607 2024-04-23 15:55:28.000000 eth_prototype-1.0.1/src/ethproto/w3wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8262 2024-04-23 15:55:28.000000 eth_prototype-1.0.1/src/ethproto/wadray.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17307 2024-04-23 15:55:28.000000 eth_prototype-1.0.1/src/ethproto/wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 15:55:34.448576 eth_prototype-1.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-04-23 15:55:28.000000 eth_prototype-1.0.1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 15:55:34.452576 eth_prototype-1.0.1/tests/hardhat-project/
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2024-04-23 15:55:28.000000 eth_prototype-1.0.1/tests/hardhat-project/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 15:55:34.440576 eth_prototype-1.0.1/tests/hardhat-project/artifacts2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 15:55:34.452576 eth_prototype-1.0.1/tests/hardhat-project/artifacts2/TestCurrency.sol/
+-rw-r--r--   0 runner    (1001) docker     (127)    29097 2024-04-23 15:55:28.000000 eth_prototype-1.0.1/tests/hardhat-project/artifacts2/TestCurrency.sol/TestCurrency.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 15:55:34.452576 eth_prototype-1.0.1/tests/hardhat-project/contracts/
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-04-23 15:55:28.000000 eth_prototype-1.0.1/tests/hardhat-project/contracts/Count.sol
+-rw-r--r--   0 runner    (1001) docker     (127)      319 2024-04-23 15:55:28.000000 eth_prototype-1.0.1/tests/hardhat-project/contracts/Counter.sol
+-rw-r--r--   0 runner    (1001) docker     (127)      822 2024-04-23 15:55:28.000000 eth_prototype-1.0.1/tests/hardhat-project/contracts/CounterUpgradeable.sol
+-rw-r--r--   0 runner    (1001) docker     (127)      995 2024-04-23 15:55:28.000000 eth_prototype-1.0.1/tests/hardhat-project/contracts/CounterUpgradeableWithLibrary.sol
+-rw-r--r--   0 runner    (1001) docker     (127)      523 2024-04-23 15:55:28.000000 eth_prototype-1.0.1/tests/hardhat-project/contracts/CounterWithLibrary.sol
+-rw-r--r--   0 runner    (1001) docker     (127)      365 2024-04-23 15:55:28.000000 eth_prototype-1.0.1/tests/hardhat-project/contracts/Datatypes.sol
+-rw-r--r--   0 runner    (1001) docker     (127)      713 2024-04-23 15:55:28.000000 eth_prototype-1.0.1/tests/hardhat-project/contracts/TestCurrency.sol
+-rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-04-23 15:55:28.000000 eth_prototype-1.0.1/tests/hardhat-project/contracts/TestCurrencyUUPS.sol
+-rw-r--r--   0 runner    (1001) docker     (127)      657 2024-04-23 15:55:28.000000 eth_prototype-1.0.1/tests/hardhat-project/contracts/TestNFT.sol
+-rw-r--r--   0 runner    (1001) docker     (127)      376 2024-04-23 15:55:28.000000 eth_prototype-1.0.1/tests/hardhat-project/hardhat.config.js
+-rw-r--r--   0 runner    (1001) docker     (127)   631590 2024-04-23 15:55:28.000000 eth_prototype-1.0.1/tests/hardhat-project/package-lock.json
+-rw-r--r--   0 runner    (1001) docker     (127)      650 2024-04-23 15:55:28.000000 eth_prototype-1.0.1/tests/hardhat-project/package.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4472 2024-04-23 15:55:28.000000 eth_prototype-1.0.1/tests/test_build_artifacts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10408 2024-04-23 15:55:28.000000 eth_prototype-1.0.1/tests/test_contracts.py
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-04-23 15:55:28.000000 eth_prototype-1.0.1/tests/test_defender.py
+-rw-r--r--   0 runner    (1001) docker     (127)      480 2024-04-23 15:55:28.000000 eth_prototype-1.0.1/tests/test_time_control.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2214 2024-04-23 15:55:28.000000 eth_prototype-1.0.1/tests/test_w3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-04-23 15:55:28.000000 eth_prototype-1.0.1/tests/test_wadray.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2523 2024-04-23 15:55:28.000000 eth_prototype-1.0.1/tox.ini
```

### Comparing `eth-prototype-1.0.0/.coveragerc` & `eth_prototype-1.0.1/.coveragerc`

 * *Files identical despite different names*

### Comparing `eth-prototype-1.0.0/.github/workflows/publish.yaml` & `eth_prototype-1.0.1/.github/workflows/publish.yaml`

 * *Files identical despite different names*

### Comparing `eth-prototype-1.0.0/.github/workflows/test.yaml` & `eth_prototype-1.0.1/.github/workflows/test.yaml`

 * *Files 21% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     branches: ["main"]
 
 jobs:
   build:
     runs-on: ubuntu-latest
     strategy:
       matrix:
-        python-version: ["3.7", "3.8", "3.9"]
+        python-version: ["3.9", "3.10"]
 
     steps:
       - uses: actions/checkout@v3
       - name: Set up Python ${{ matrix.python-version }}
         uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python-version }}
```

### Comparing `eth-prototype-1.0.0/.gitignore` & `eth_prototype-1.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `eth-prototype-1.0.0/.pre-commit-config.yaml` & `eth_prototype-1.0.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `eth-prototype-1.0.0/LICENSE.txt` & `eth_prototype-1.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `eth-prototype-1.0.0/PKG-INFO` & `eth_prototype-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eth-prototype
-Version: 1.0.0
+Version: 1.0.1
 Summary: Prototype Ethereum Smart Contracts in Python
 Home-page: https://github.com/gnarvaja/eth-prototype
 Author: Guillermo M. Narvaja
 Author-email: guillermo@ensuro.co
 License: MIT
 Project-URL: Documentation, https://pyscaffold.org/
 Platform: any
@@ -16,26 +16,26 @@
 License-File: AUTHORS.rst
 Requires-Dist: m9g
 Requires-Dist: environs
 Requires-Dist: requests
 Requires-Dist: hexbytes
 Requires-Dist: importlib-metadata; python_version < "3.8"
 Provides-Extra: web3
-Requires-Dist: web3; extra == "web3"
+Requires-Dist: web3>=6; extra == "web3"
 Provides-Extra: defender
 Requires-Dist: boto3; extra == "defender"
 Provides-Extra: gmpy2
 Requires-Dist: gmpy2; extra == "gmpy2"
 Provides-Extra: testing
 Requires-Dist: setuptools; extra == "testing"
 Requires-Dist: pytest; extra == "testing"
 Requires-Dist: gmpy2; extra == "testing"
 Requires-Dist: pytest-cov; extra == "testing"
 Provides-Extra: testing-w3
-Requires-Dist: web3[tester]; extra == "testing-w3"
+Requires-Dist: web3[tester]>=6; extra == "testing-w3"
 Requires-Dist: setuptools; extra == "testing-w3"
 Requires-Dist: pytest; extra == "testing-w3"
 Requires-Dist: pytest-cov; extra == "testing-w3"
 Requires-Dist: boto3; extra == "testing-w3"
 
 # eth-prototype
```

### Comparing `eth-prototype-1.0.0/README.md` & `eth_prototype-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `eth-prototype-1.0.0/docs/Makefile` & `eth_prototype-1.0.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `eth-prototype-1.0.0/docs/conf.py` & `eth_prototype-1.0.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `eth-prototype-1.0.0/docs/index.rst` & `eth_prototype-1.0.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `eth-prototype-1.0.0/setup.cfg` & `eth_prototype-1.0.1/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -31,26 +31,26 @@
 [options.packages.find]
 where = src
 exclude = 
 	tests
 
 [options.extras_require]
 web3 = 
-	web3
+	web3>=6
 defender = 
 	boto3
 gmpy2 = 
 	gmpy2
 testing = 
 	setuptools
 	pytest
 	gmpy2
 	pytest-cov
 testing-w3 = 
-	web3[tester]
+	web3[tester]>=6
 	setuptools
 	pytest
 	pytest-cov
 	boto3
 
 [options.entry_points]
```

### Comparing `eth-prototype-1.0.0/setup.py` & `eth_prototype-1.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `eth-prototype-1.0.0/src/eth_prototype.egg-info/PKG-INFO` & `eth_prototype-1.0.1/src/eth_prototype.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eth-prototype
-Version: 1.0.0
+Version: 1.0.1
 Summary: Prototype Ethereum Smart Contracts in Python
 Home-page: https://github.com/gnarvaja/eth-prototype
 Author: Guillermo M. Narvaja
 Author-email: guillermo@ensuro.co
 License: MIT
 Project-URL: Documentation, https://pyscaffold.org/
 Platform: any
@@ -16,26 +16,26 @@
 License-File: AUTHORS.rst
 Requires-Dist: m9g
 Requires-Dist: environs
 Requires-Dist: requests
 Requires-Dist: hexbytes
 Requires-Dist: importlib-metadata; python_version < "3.8"
 Provides-Extra: web3
-Requires-Dist: web3; extra == "web3"
+Requires-Dist: web3>=6; extra == "web3"
 Provides-Extra: defender
 Requires-Dist: boto3; extra == "defender"
 Provides-Extra: gmpy2
 Requires-Dist: gmpy2; extra == "gmpy2"
 Provides-Extra: testing
 Requires-Dist: setuptools; extra == "testing"
 Requires-Dist: pytest; extra == "testing"
 Requires-Dist: gmpy2; extra == "testing"
 Requires-Dist: pytest-cov; extra == "testing"
 Provides-Extra: testing-w3
-Requires-Dist: web3[tester]; extra == "testing-w3"
+Requires-Dist: web3[tester]>=6; extra == "testing-w3"
 Requires-Dist: setuptools; extra == "testing-w3"
 Requires-Dist: pytest; extra == "testing-w3"
 Requires-Dist: pytest-cov; extra == "testing-w3"
 Requires-Dist: boto3; extra == "testing-w3"
 
 # eth-prototype
```

### Comparing `eth-prototype-1.0.0/src/eth_prototype.egg-info/SOURCES.txt` & `eth_prototype-1.0.1/src/eth_prototype.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `eth-prototype-1.0.0/src/ethproto/__init__.py` & `eth_prototype-1.0.1/src/ethproto/__init__.py`

 * *Files identical despite different names*

### Comparing `eth-prototype-1.0.0/src/ethproto/build_artifacts.py` & `eth_prototype-1.0.1/src/ethproto/build_artifacts.py`

 * *Files identical despite different names*

### Comparing `eth-prototype-1.0.0/src/ethproto/contracts.py` & `eth_prototype-1.0.1/src/ethproto/contracts.py`

 * *Files identical despite different names*

### Comparing `eth-prototype-1.0.0/src/ethproto/defender_relay.py` & `eth_prototype-1.0.1/src/ethproto/defender_relay.py`

 * *Files identical despite different names*

### Comparing `eth-prototype-1.0.0/src/ethproto/w3wrappers.py` & `eth_prototype-1.0.1/src/ethproto/w3wrappers.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 from environs import Env
 from eth_account.account import Account, LocalAccount
 from eth_account.signers.base import BaseAccount
 from eth_utils.abi import event_abi_to_log_topic
 from hexbytes import HexBytes
 from web3.contract import Contract
-from web3.exceptions import ExtraDataLengthError
+from web3.exceptions import ContractLogicError, ExtraDataLengthError
 from web3.middleware import geth_poa_middleware
 
 from .build_artifacts import ArtifactLibrary
 from .contracts import RevertError
 from .wrappers import (
     MAXUINT256,
     SKIP_PROXY,
@@ -93,27 +93,27 @@
         tx_kwargs = {**provider.tx_kwargs, **tx_kwargs}
         from_ = tx_kwargs.pop("from")
         if isinstance(from_, BaseAccount):
             tx_kwargs["from"] = from_.address
         else:  # it's a string, I try to get the PK from the environment
             from_ = provider.address_book.get_signer_account(from_)
             tx_kwargs["from"] = from_.address
-        tx = function.buildTransaction(
+        tx = function.build_transaction(
             {
                 **tx_kwargs,
                 **{"nonce": provider.w3.eth.get_transaction_count(from_.address)},
             }
         )
         signed_tx = from_.sign_transaction(tx)
         tx_hash = provider.w3.eth.send_raw_transaction(signed_tx.rawTransaction)
     elif W3_TRANSACT_MODE == "defender-async":
         from .defender_relay import send_transaction
 
         tx_kwargs = {**provider.tx_kwargs, **tx_kwargs}
-        tx = function.buildTransaction(tx_kwargs)
+        tx = function.build_transaction(tx_kwargs)
         return send_transaction(tx)
 
     return provider.w3.eth.wait_for_transaction_receipt(tx_hash)
 
 
 class W3AddressBook(AddressBook):
     def __init__(self, w3, eth_accounts=None):
@@ -364,16 +364,20 @@
 
     def normalize_receipt(self, wrapper, receipt):
         if W3_TRANSACT_MODE == "defender-async":
             return receipt  # Don't do anything because the receipt is just a dict of not-yet-mined tx
         return ReceiptWrapper(receipt, wrapper.contract)
 
     def _handle_exception(self, err):
-        if str(err).startswith("execution reverted: "):
-            raise RevertError(str(err)[len("execution reverted: ") :])
+        if isinstance(err, ContractLogicError):
+            raise RevertError(
+                err.message[len("execution reverted: ") :]
+                if err.message and err.message.startswith("execution reverted: ")
+                else err.message
+            )
         super()._handle_exception(err)
 
     @classmethod
     def parse(cls, wrapper, value_type, value):
         if value_type.startswith("(") and value_type.endswith(")"):
             # It's a tuple / struct
             value_types = [t.strip() for t in value_type.split(",")]
```

### Comparing `eth-prototype-1.0.0/src/ethproto/wadray.py` & `eth_prototype-1.0.1/src/ethproto/wadray.py`

 * *Files identical despite different names*

### Comparing `eth-prototype-1.0.0/src/ethproto/wrappers.py` & `eth_prototype-1.0.1/src/ethproto/wrappers.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,18 +45,14 @@
 
 
 def auto_register_provider(provider_key):
     if provider_key == "w3":
         from .w3wrappers import register_w3_provider
 
         register_w3_provider()
-    elif provider_key == "brownie":
-        from .brwrappers import BrownieProvider
-
-        register_provider("brownie", BrownieProvider())
     else:
         raise RuntimeError(f"Unknown provider {provider_key}")
 
 
 def register_provider(provider_key, provider):
     global _providers
     _providers[provider_key] = provider
```

### Comparing `eth-prototype-1.0.0/tests/conftest.py` & `eth_prototype-1.0.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `eth-prototype-1.0.0/tests/hardhat-project/artifacts2/TestCurrency.sol/TestCurrency.json` & `eth_prototype-1.0.1/tests/hardhat-project/artifacts2/TestCurrency.sol/TestCurrency.json`

 * *Files identical despite different names*

### Comparing `eth-prototype-1.0.0/tests/hardhat-project/contracts/CounterUpgradeable.sol` & `eth_prototype-1.0.1/tests/hardhat-project/contracts/CounterUpgradeable.sol`

 * *Files identical despite different names*

### Comparing `eth-prototype-1.0.0/tests/hardhat-project/contracts/CounterUpgradeableWithLibrary.sol` & `eth_prototype-1.0.1/tests/hardhat-project/contracts/CounterUpgradeableWithLibrary.sol`

 * *Files identical despite different names*

### Comparing `eth-prototype-1.0.0/tests/hardhat-project/contracts/CounterWithLibrary.sol` & `eth_prototype-1.0.1/tests/hardhat-project/contracts/CounterWithLibrary.sol`

 * *Files identical despite different names*

### Comparing `eth-prototype-1.0.0/tests/hardhat-project/contracts/TestCurrency.sol` & `eth_prototype-1.0.1/tests/hardhat-project/contracts/TestCurrency.sol`

 * *Files identical despite different names*

### Comparing `eth-prototype-1.0.0/tests/hardhat-project/contracts/TestCurrencyUUPS.sol` & `eth_prototype-1.0.1/tests/hardhat-project/contracts/TestCurrencyUUPS.sol`

 * *Files identical despite different names*

### Comparing `eth-prototype-1.0.0/tests/hardhat-project/contracts/TestNFT.sol` & `eth_prototype-1.0.1/tests/hardhat-project/contracts/TestNFT.sol`

 * *Files identical despite different names*

### Comparing `eth-prototype-1.0.0/tests/hardhat-project/package-lock.json` & `eth_prototype-1.0.1/tests/hardhat-project/package-lock.json`

 * *Files identical despite different names*

### Comparing `eth-prototype-1.0.0/tests/hardhat-project/package.json` & `eth_prototype-1.0.1/tests/hardhat-project/package.json`

 * *Files identical despite different names*

### Comparing `eth-prototype-1.0.0/tests/test_build_artifacts.py` & `eth_prototype-1.0.1/tests/test_build_artifacts.py`

 * *Files identical despite different names*

### Comparing `eth-prototype-1.0.0/tests/test_contracts.py` & `eth_prototype-1.0.1/tests/test_contracts.py`

 * *Files identical despite different names*

### Comparing `eth-prototype-1.0.0/tests/test_w3.py` & `eth_prototype-1.0.1/tests/test_w3.py`

 * *Files identical despite different names*

### Comparing `eth-prototype-1.0.0/tests/test_wadray.py` & `eth_prototype-1.0.1/tests/test_wadray.py`

 * *Files identical despite different names*

### Comparing `eth-prototype-1.0.0/tox.ini` & `eth_prototype-1.0.1/tox.ini`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 # Tox configuration file
 # Read more under https://tox.readthedocs.org/
 # THIS SCRIPT IS SUPPOSED TO BE AN EXAMPLE. MODIFY IT ACCORDING TO YOUR NEEDS!
 
 [tox]
 minversion = 3.15
-envlist = {py37,py38,py39}, {py37,py38,py39}-w3
+envlist = {py39,py310}, {py39,py310}-w3
 
 [gh-actions]
 python =
-    3.7: py37, py37-w3
-    3.8: py38, py38-w3
     3.9: py39, py39-w3
+    3.10: py310, py310-w3
 
 [testenv]
 description = invoke pytest to run automated tests
 isolated_build = True
 setenv =
     TOXINIDIR = {toxinidir}
     TEST_ENV = pure-python
@@ -23,15 +22,15 @@
     WADRAY_USE_GMPY2
 extras =
     testing
 commands =
     pytest {posargs}
 
 
-[testenv:{py37,py38,py39}-w3]
+[testenv:{py39,py310}-w3]
 description = invoke pytest to run automated tests
 isolated_build = True
 setenv =
     TOXINIDIR = {toxinidir}
     TEST_ENV = web3py
 passenv =
     HOME
```

