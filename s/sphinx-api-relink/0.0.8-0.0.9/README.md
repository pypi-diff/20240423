# Comparing `tmp/sphinx-api-relink-0.0.8.tar.gz` & `tmp/sphinx_api_relink-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sphinx-api-relink-0.0.8.tar", last modified: Sat Dec  9 17:43:30 2023, max compression
+gzip compressed data, was "sphinx_api_relink-0.0.9.tar", last modified: Tue Apr 23 12:53:23 2024, max compression
```

## Comparing `sphinx-api-relink-0.0.8.tar` & `sphinx_api_relink-0.0.9.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-09 17:43:30.383425 sphinx-api-relink-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)      925 2023-12-09 17:43:17.000000 sphinx-api-relink-0.0.8/.cspell.json
--rw-r--r--   0 runner    (1001) docker     (127)      253 2023-12-09 17:43:17.000000 sphinx-api-relink-0.0.8/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-09 17:43:30.375425 sphinx-api-relink-0.0.8/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      909 2023-12-09 17:43:17.000000 sphinx-api-relink-0.0.8/.github/release-drafter.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-09 17:43:30.375425 sphinx-api-relink-0.0.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      526 2023-12-09 17:43:17.000000 sphinx-api-relink-0.0.8/.github/workflows/cd.yml
--rw-r--r--   0 runner    (1001) docker     (127)      620 2023-12-09 17:43:17.000000 sphinx-api-relink-0.0.8/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)      436 2023-12-09 17:43:17.000000 sphinx-api-relink-0.0.8/.github/workflows/clean-caches.yml
--rw-r--r--   0 runner    (1001) docker     (127)      979 2023-12-09 17:43:17.000000 sphinx-api-relink-0.0.8/.github/workflows/pr-linting.yml
--rw-r--r--   0 runner    (1001) docker     (127)      280 2023-12-09 17:43:17.000000 sphinx-api-relink-0.0.8/.github/workflows/release-drafter.yml
--rw-r--r--   0 runner    (1001) docker     (127)      650 2023-12-09 17:43:17.000000 sphinx-api-relink-0.0.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     2378 2023-12-09 17:43:17.000000 sphinx-api-relink-0.0.8/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)        8 2023-12-09 17:43:17.000000 sphinx-api-relink-0.0.8/.prettierignore
--rw-r--r--   0 runner    (1001) docker     (127)      275 2023-12-09 17:43:17.000000 sphinx-api-relink-0.0.8/.taplo.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-09 17:43:30.379425 sphinx-api-relink-0.0.8/.vscode/
--rw-r--r--   0 runner    (1001) docker     (127)      840 2023-12-09 17:43:17.000000 sphinx-api-relink-0.0.8/.vscode/extensions.json
--rw-r--r--   0 runner    (1001) docker     (127)      415 2023-12-09 17:43:17.000000 sphinx-api-relink-0.0.8/.vscode/launch.json
--rw-r--r--   0 runner    (1001) docker     (127)     1786 2023-12-09 17:43:17.000000 sphinx-api-relink-0.0.8/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (127)      423 2023-12-09 17:43:17.000000 sphinx-api-relink-0.0.8/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)     1536 2023-12-09 17:43:17.000000 sphinx-api-relink-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6807 2023-12-09 17:43:30.383425 sphinx-api-relink-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4633 2023-12-09 17:43:17.000000 sphinx-api-relink-0.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      152 2023-12-09 17:43:17.000000 sphinx-api-relink-0.0.8/environment.yml
--rw-r--r--   0 runner    (1001) docker     (127)     4492 2023-12-09 17:43:17.000000 sphinx-api-relink-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-09 17:43:30.383425 sphinx-api-relink-0.0.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-09 17:43:30.375425 sphinx-api-relink-0.0.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-09 17:43:30.379425 sphinx-api-relink-0.0.8/src/sphinx_api_relink/
--rw-r--r--   0 runner    (1001) docker     (127)     7986 2023-12-09 17:43:17.000000 sphinx-api-relink-0.0.8/src/sphinx_api_relink/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5215 2023-12-09 17:43:17.000000 sphinx-api-relink-0.0.8/src/sphinx_api_relink/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     5165 2023-12-09 17:43:17.000000 sphinx-api-relink-0.0.8/src/sphinx_api_relink/linkcode.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-09 17:43:17.000000 sphinx-api-relink-0.0.8/src/sphinx_api_relink/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-09 17:43:30.379425 sphinx-api-relink-0.0.8/src/sphinx_api_relink/templates/
--rw-r--r--   0 runner    (1001) docker     (127)      250 2023-12-09 17:43:17.000000 sphinx-api-relink-0.0.8/src/sphinx_api_relink/templates/module.rst_t
--rw-r--r--   0 runner    (1001) docker     (127)     1021 2023-12-09 17:43:17.000000 sphinx-api-relink-0.0.8/src/sphinx_api_relink/templates/package.rst_t
--rw-r--r--   0 runner    (1001) docker     (127)      125 2023-12-09 17:43:17.000000 sphinx-api-relink-0.0.8/src/sphinx_api_relink/templates/toc.rst_t
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-09 17:43:30.379425 sphinx-api-relink-0.0.8/src/sphinx_api_relink.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6807 2023-12-09 17:43:30.000000 sphinx-api-relink-0.0.8/src/sphinx_api_relink.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      893 2023-12-09 17:43:30.000000 sphinx-api-relink-0.0.8/src/sphinx_api_relink.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-09 17:43:30.000000 sphinx-api-relink-0.0.8/src/sphinx_api_relink.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      312 2023-12-09 17:43:30.000000 sphinx-api-relink-0.0.8/src/sphinx_api_relink.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2023-12-09 17:43:30.000000 sphinx-api-relink-0.0.8/src/sphinx_api_relink.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 12:53:23.209457 sphinx_api_relink-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)      965 2024-04-23 12:53:15.000000 sphinx_api_relink-0.0.9/.cspell.json
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-23 12:53:15.000000 sphinx_api_relink-0.0.9/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 12:53:23.205457 sphinx_api_relink-0.0.9/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      909 2024-04-23 12:53:15.000000 sphinx_api_relink-0.0.9/.github/release-drafter.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 12:53:23.205457 sphinx_api_relink-0.0.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      865 2024-04-23 12:53:15.000000 sphinx_api_relink-0.0.9/.github/workflows/cd.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      708 2024-04-23 12:53:15.000000 sphinx_api_relink-0.0.9/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      436 2024-04-23 12:53:15.000000 sphinx_api_relink-0.0.9/.github/workflows/clean-caches.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-04-23 12:53:15.000000 sphinx_api_relink-0.0.9/.github/workflows/pr-linting.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-23 12:53:15.000000 sphinx_api_relink-0.0.9/.github/workflows/release-drafter.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      650 2024-04-23 12:53:15.000000 sphinx_api_relink-0.0.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     2182 2024-04-23 12:53:15.000000 sphinx_api_relink-0.0.9/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-23 12:53:15.000000 sphinx_api_relink-0.0.9/.prettierignore
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-23 12:53:15.000000 sphinx_api_relink-0.0.9/.taplo.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 12:53:23.205457 sphinx_api_relink-0.0.9/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (127)      905 2024-04-23 12:53:15.000000 sphinx_api_relink-0.0.9/.vscode/extensions.json
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-04-23 12:53:15.000000 sphinx_api_relink-0.0.9/.vscode/launch.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2093 2024-04-23 12:53:15.000000 sphinx_api_relink-0.0.9/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (127)      386 2024-04-23 12:53:15.000000 sphinx_api_relink-0.0.9/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1536 2024-04-23 12:53:15.000000 sphinx_api_relink-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6500 2024-04-23 12:53:23.209457 sphinx_api_relink-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4520 2024-04-23 12:53:15.000000 sphinx_api_relink-0.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-23 12:53:15.000000 sphinx_api_relink-0.0.9/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     4311 2024-04-23 12:53:15.000000 sphinx_api_relink-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 12:53:23.209457 sphinx_api_relink-0.0.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 12:53:23.201457 sphinx_api_relink-0.0.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 12:53:23.205457 sphinx_api_relink-0.0.9/src/sphinx_api_relink/
+-rw-r--r--   0 runner    (1001) docker     (127)     8667 2024-04-23 12:53:15.000000 sphinx_api_relink-0.0.9/src/sphinx_api_relink/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5216 2024-04-23 12:53:15.000000 sphinx_api_relink-0.0.9/src/sphinx_api_relink/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5165 2024-04-23 12:53:15.000000 sphinx_api_relink-0.0.9/src/sphinx_api_relink/linkcode.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 12:53:15.000000 sphinx_api_relink-0.0.9/src/sphinx_api_relink/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 12:53:23.205457 sphinx_api_relink-0.0.9/src/sphinx_api_relink/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-04-23 12:53:15.000000 sphinx_api_relink-0.0.9/src/sphinx_api_relink/templates/module.rst_t
+-rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-04-23 12:53:15.000000 sphinx_api_relink-0.0.9/src/sphinx_api_relink/templates/package.rst_t
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-23 12:53:15.000000 sphinx_api_relink-0.0.9/src/sphinx_api_relink/templates/toc.rst_t
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 12:53:23.205457 sphinx_api_relink-0.0.9/src/sphinx_api_relink.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6500 2024-04-23 12:53:23.000000 sphinx_api_relink-0.0.9/src/sphinx_api_relink.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      893 2024-04-23 12:53:23.000000 sphinx_api_relink-0.0.9/src/sphinx_api_relink.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 12:53:23.000000 sphinx_api_relink-0.0.9/src/sphinx_api_relink.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-04-23 12:53:23.000000 sphinx_api_relink-0.0.9/src/sphinx_api_relink.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-23 12:53:23.000000 sphinx_api_relink-0.0.9/src/sphinx_api_relink.egg-info/top_level.txt
```

### Comparing `sphinx-api-relink-0.0.8/.cspell.json` & `sphinx_api_relink-0.0.9/.cspell.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9800754800754802%*

 * *Differences: {"'ignorePaths'": "{insert: [(2, '*.rst_t')]}",*

 * * "'ignoreWords'": "{insert: [(4, 'redef')]}",*

 * * "'words'": "{insert: [(8, 'PyPA')]}"}*

```diff
@@ -17,26 +17,28 @@
         "parmater",
         "transision",
         "transisions"
     ],
     "ignorePaths": [
         "**/*.rst_t",
         "**/.cspell.json",
+        "*.rst_t",
         ".editorconfig",
         ".gitignore",
         ".pre-commit-config.yaml",
         ".prettierignore",
         ".vscode/*",
         "pyproject.toml"
     ],
     "ignoreWords": [
         "PyPI",
         "commitlint",
         "linkcode",
         "prereleased",
+        "redef",
         "refdomain",
         "refspecific",
         "reftarget",
         "reftype",
         "refuri",
         "rtfd",
         "srcdir",
@@ -49,11 +51,12 @@
         "apidoc",
         "autoapi",
         "autodoc",
         "ComPWA",
         "conda",
         "intersphinx",
         "mypy",
+        "PyPA",
         "PYTHONHASHSEED",
         "SymPy"
     ]
 }
```

### Comparing `sphinx-api-relink-0.0.8/.github/release-drafter.yml` & `sphinx_api_relink-0.0.9/.github/release-drafter.yml`

 * *Files identical despite different names*

### Comparing `sphinx-api-relink-0.0.8/.github/workflows/ci.yml` & `sphinx_api_relink-0.0.9/.github/workflows/ci.yml`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 name: CI
 
 concurrency:
   group: ${{ github.workflow }}-${{ github.ref }}
-  cancel-in-progress: true
+  cancel-in-progress: |-
+    ${{ github.ref != format('refs/heads/{0}', github.event.repository.default_branch) }}
 
 env:
   PYTHONHASHSEED: "0"
 
 on:
   push:
     branches:
```

### Comparing `sphinx-api-relink-0.0.8/.gitignore` & `sphinx_api_relink-0.0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `sphinx-api-relink-0.0.8/.pre-commit-config.yaml` & `sphinx_api_relink-0.0.9/.pre-commit-config.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -9,14 +9,21 @@
 
 repos:
   - repo: meta
     hooks:
       - id: check-hooks-apply
       - id: check-useless-excludes
 
+  - repo: https://github.com/astral-sh/ruff-pre-commit
+    rev: v0.3.5
+    hooks:
+      - id: ruff
+        args: [--fix]
+      - id: ruff-format
+
   - repo: https://github.com/pre-commit/pre-commit-hooks
     rev: v4.5.0
     hooks:
       - id: check-ast
       - id: check-case-conflict
       - id: check-json
       - id: check-merge-conflict
@@ -30,37 +37,44 @@
             .*\.bib|
             .*\.svg|
             \.cspell\.json
           )$
       - id: mixed-line-ending
       - id: trailing-whitespace
 
-  - repo: https://github.com/psf/black-pre-commit-mirror
-    rev: 23.11.0
+  - repo: https://github.com/pre-commit/mirrors-prettier
+    rev: v4.0.0-alpha.8
     hooks:
-      - id: black
+      - id: prettier
 
-  - repo: https://github.com/asottile/blacken-docs
-    rev: 1.16.0
+  - repo: https://github.com/ComPWA/mirrors-taplo
+    rev: v0.8.1
     hooks:
-      - id: blacken-docs
+      - id: taplo
 
-  - repo: https://github.com/ComPWA/repo-maintenance
-    rev: 0.1.9
+  - repo: https://github.com/pappasam/toml-sort
+    rev: v0.23.1
+    hooks:
+      - id: toml-sort
+        args:
+          - --in-place
+
+  - repo: https://github.com/ComPWA/policy
+    rev: 0.3.4
     hooks:
       - id: check-dev-files
         args:
           - --no-gitpod
           - --no-notebooks
           - --no-prettierrc
           - --repo-name=sphinx-api-relink
           - --repo-title=sphinx-api-relink
 
   - repo: https://github.com/streetsidesoftware/cspell-cli
-    rev: v8.1.1
+    rev: v8.6.1
     hooks:
       - id: cspell
 
   - repo: https://github.com/editorconfig-checker/editorconfig-checker.python
     rev: 2.7.3
     hooks:
       - id: editorconfig-checker
@@ -76,34 +90,11 @@
       - id: mypy
         name: mypy
         entry: mypy
         language: system
         types:
           - python
 
-  - repo: https://github.com/pre-commit/mirrors-prettier
-    rev: v4.0.0-alpha.3-1
-    hooks:
-      - id: prettier
-
   - repo: https://github.com/ComPWA/mirrors-pyright
-    rev: v1.1.339
+    rev: v1.1.357
     hooks:
       - id: pyright
-
-  - repo: https://github.com/astral-sh/ruff-pre-commit
-    rev: v0.1.7
-    hooks:
-      - id: ruff
-        args: [--fix]
-
-  - repo: https://github.com/ComPWA/mirrors-taplo
-    rev: v0.8.1
-    hooks:
-      - id: taplo
-
-  - repo: https://github.com/pappasam/toml-sort
-    rev: v0.23.1
-    hooks:
-      - id: toml-sort
-        args:
-          - --in-place
```

### Comparing `sphinx-api-relink-0.0.8/.vscode/extensions.json` & `sphinx_api_relink-0.0.9/.vscode/extensions.json`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8541666666666666%*

 * *Differences: {"'recommendations'": "{insert: [(11, 'soulcode.vscode-unwanted-extensions'), (15, "*

 * *                      "'wholroyd.jinja')], delete: [16, 7, 5]}",*

 * * "'unwantedRecommendations'": "{insert: [(2, 'garaioag.garaio-vscode-unwanted-recommendations'), "*

 * *                              "(3, 'ms-python.black-formatter'), (8, 'tyriar.sort-lines')]}"}*

```diff
@@ -1,30 +1,32 @@
 {
     "recommendations": [
         "charliermarsh.ruff",
         "christian-kohler.path-intellisense",
         "eamodio.gitlens",
         "editorconfig.editorconfig",
         "esbenp.prettier-vscode",
-        "garaioag.garaio-vscode-unwanted-recommendations",
         "github.vscode-github-actions",
-        "ms-python.black-formatter",
         "ms-python.mypy-type-checker",
         "ms-python.python",
         "ms-python.vscode-pylance",
         "redhat.vscode-yaml",
         "ryanluker.vscode-coverage-gutters",
+        "soulcode.vscode-unwanted-extensions",
         "stkb.rewrap",
         "streetsidesoftware.code-spell-checker",
         "tamasfe.even-better-toml",
-        "tyriar.sort-lines",
+        "wholroyd.jinja",
         "yzhang.markdown-all-in-one"
     ],
     "unwantedRecommendations": [
         "bungcip.better-toml",
         "davidanson.vscode-markdownlint",
+        "garaioag.garaio-vscode-unwanted-recommendations",
+        "ms-python.black-formatter",
         "ms-python.flake8",
         "ms-python.isort",
         "ms-python.pylint",
-        "travisillig.vscode-json-stable-stringify"
+        "travisillig.vscode-json-stable-stringify",
+        "tyriar.sort-lines"
     ]
 }
```

### Comparing `sphinx-api-relink-0.0.8/.vscode/settings.json` & `sphinx_api_relink-0.0.9/.vscode/settings.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7685185185185186%*

 * *Differences: {"'[json]'": "{'editor.wordWrap': 'on'}",*

 * * "'[python]'": "{'editor.defaultFormatter': 'charliermarsh.ruff'}",*

 * * "'files.associations'": "OrderedDict([('*.rst_t', 'jinja')])",*

 * * "'gitlens.telemetry.enabled'": 'False',*

 * * "'notebook.codeActionsOnSave'": "OrderedDict([('notebook.source.organizeImports', 'explicit')])",*

 * * "'notebook.formatOnSave.enabled'": 'True',*

 * * "'redhat.telemetry.enabled'": 'False',*

 * * "'ruff.importStrategy'": "'fromEnvironment'",*

 * * "'telemetry.telemetryLevel'": "'off'",*

 * * 'delete': "['black-formatt […]*

```diff
@@ -5,63 +5,74 @@
     "[git-commit]": {
         "editor.rulers": [
             72
         ],
         "rewrap.wrappingColumn": 72
     },
     "[json]": {
-        "editor.defaultFormatter": "esbenp.prettier-vscode"
+        "editor.defaultFormatter": "esbenp.prettier-vscode",
+        "editor.wordWrap": "on"
     },
     "[jsonc]": {
         "editor.defaultFormatter": "esbenp.prettier-vscode"
     },
     "[markdown]": {
         "editor.defaultFormatter": "esbenp.prettier-vscode"
     },
     "[pip-requirements]": {
         "editor.wordWrap": "off"
     },
     "[python]": {
         "editor.codeActionsOnSave": {
             "source.organizeImports": "explicit"
         },
-        "editor.defaultFormatter": "ms-python.black-formatter",
+        "editor.defaultFormatter": "charliermarsh.ruff",
         "editor.rulers": [
             88
         ]
     },
     "[yaml]": {
         "editor.defaultFormatter": "esbenp.prettier-vscode"
     },
-    "black-formatter.importStrategy": "fromEnvironment",
     "cSpell.enabled": true,
     "coverage-gutters.coverageFileNames": [
         "coverage.xml"
     ],
     "coverage-gutters.coverageReportFileName": "**/htmlcov/index.html",
     "coverage-gutters.showGutterCoverage": false,
     "coverage-gutters.showLineCoverage": true,
     "diffEditor.experimental.showMoves": true,
     "editor.formatOnSave": true,
+    "files.associations": {
+        "*.rst_t": "jinja"
+    },
     "files.watcherExclude": {
         "**/*_cache/**": true,
         "**/.eggs/**": true,
         "**/.git/**": true,
         "**/.tox/**": true
     },
     "git.rebaseWhenSync": true,
     "github-actions.workflows.pinned.refresh.enabled": true,
     "github-actions.workflows.pinned.workflows": [
         ".github/workflows/ci.yml"
     ],
+    "gitlens.telemetry.enabled": false,
     "multiDiffEditor.experimental.enabled": true,
     "mypy-type-checker.args": [
         "--config-file=${workspaceFolder}/pyproject.toml"
     ],
     "mypy-type-checker.importStrategy": "fromEnvironment",
+    "notebook.codeActionsOnSave": {
+        "notebook.source.organizeImports": "explicit"
+    },
+    "notebook.formatOnSave.enabled": true,
     "python.analysis.autoImportCompletions": false,
     "python.analysis.typeCheckingMode": "strict",
     "python.testing.unittestEnabled": false,
+    "redhat.telemetry.enabled": false,
     "rewrap.wrappingColumn": 88,
     "ruff.enable": true,
-    "ruff.organizeImports": true
+    "ruff.importStrategy": "fromEnvironment",
+    "ruff.organizeImports": true,
+    "telemetry.telemetryLevel": "off"
 }
```

### Comparing `sphinx-api-relink-0.0.8/LICENSE` & `sphinx_api_relink-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `sphinx-api-relink-0.0.8/PKG-INFO` & `sphinx_api_relink-0.0.9/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sphinx-api-relink
-Version: 0.0.8
+Version: 0.0.9
 Summary: Relink type hints in your Sphinx API
 Author-email: Common Partial Wave Analysis <compwa-admin@ep1.rub.de>
 Maintainer-email: compwa-admin@ep1.rub.de
 License: BSD 3-Clause License
 Project-URL: Changelog, https://github.com/ComPWA/sphinx-api-relink/releases
 Project-URL: Documentation, https://github.com/ComPWA/sphinx-api-relink/blob/main/README.md
 Project-URL: Source, https://github.com/ComPWA/sphinx-api-relink
@@ -31,41 +31,35 @@
 Requires-Dist: Sphinx>=4.4
 Requires-Dist: colorama
 Requires-Dist: docutils
 Requires-Dist: importlib-metadata; python_version < "3.8.0"
 Requires-Dist: typing-extensions; python_version < "3.8.0"
 Provides-Extra: dev
 Requires-Dist: sphinx-api-relink[sty]; extra == "dev"
-Provides-Extra: format
-Requires-Dist: black; extra == "format"
-Provides-Extra: lint
-Requires-Dist: ruff; extra == "lint"
-Requires-Dist: sphinx-api-relink[mypy]; extra == "lint"
-Provides-Extra: mypy
-Requires-Dist: mypy; extra == "mypy"
-Requires-Dist: types-colorama; extra == "mypy"
-Requires-Dist: types-docutils; extra == "mypy"
-Requires-Dist: types-requests; extra == "mypy"
 Provides-Extra: sty
+Requires-Dist: mypy; extra == "sty"
 Requires-Dist: pre-commit>=1.4.0; extra == "sty"
-Requires-Dist: sphinx-api-relink[format]; extra == "sty"
-Requires-Dist: sphinx-api-relink[lint]; extra == "sty"
+Requires-Dist: ruff; extra == "sty"
+Requires-Dist: sphinx-api-relink[types]; extra == "sty"
+Provides-Extra: types
+Requires-Dist: types-colorama; extra == "types"
+Requires-Dist: types-docutils; extra == "types"
+Requires-Dist: types-requests; extra == "types"
 
 # `sphinx-api-relink`
 
 [![PyPI package](https://badge.fury.io/py/sphinx-api-relink.svg)](https://pypi.org/project/sphinx-api-relink)
 [![Supported Python versions](https://img.shields.io/pypi/pyversions/sphinx-api-relink)](https://pypi.org/project/sphinx-api-relink)
 [![BSD 3-Clause license](https://img.shields.io/badge/License-BSD_3--Clause-blue.svg)](https://opensource.org/licenses/BSD-3-Clause)
 [![Open in Visual Studio Code](https://img.shields.io/badge/vscode-open-blue?logo=visualstudiocode)](https://open.vscode.dev/ComPWA/sphinx-api-relink)
 [![CI status](https://github.com/ComPWA/sphinx-api-relink/workflows/CI/badge.svg)](https://github.com/ComPWA/sphinx-api-relink/actions?query=branch%3Amain+workflow%3ACI)
 [![Checked with mypy](http://www.mypy-lang.org/static/mypy_badge.svg)](https://mypy.readthedocs.io)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/ComPWA/sphinx-api-relink/main.svg)](https://results.pre-commit.ci/latest/github/ComPWA/sphinx-api-relink/main)
 [![Spelling checked](https://img.shields.io/badge/cspell-checked-brightgreen.svg)](https://github.com/streetsidesoftware/cspell/tree/master/packages/cspell)
 [![code style: prettier](https://img.shields.io/badge/code_style-prettier-ff69b4.svg?style=flat-square)](https://github.com/prettier/prettier)
-[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
 
 This package is a plugin for the [`sphinx.ext.autodoc`](https://www.sphinx-doc.org/en/master/usage/extensions/autodoc.html) extension. The [`autodoc_type_aliases`](https://www.sphinx-doc.org/en/master/usage/extensions/autodoc.html#confval-autodoc_type_aliases) configuration does not always work well when using postponed evaluation of annotations ([PEP 563](https://peps.python.org/pep-0563), i.e. `from __future__ import annotations`) or when importing through [`typing.TYPE_CHECKING`](https://docs.python.org/3/library/typing.html#typing.TYPE_CHECKING), because `sphinx.ext.autodoc` generates the API dynamically (not statically, as opposed to [`sphinx-autoapi`](https://github.com/readthedocs/sphinx-autoapi)).
 
 ## Installation
 
 Just install through [PyPI](https://pypi.org) with `pip`:
```

### Comparing `sphinx-api-relink-0.0.8/README.md` & `sphinx_api_relink-0.0.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 [![BSD 3-Clause license](https://img.shields.io/badge/License-BSD_3--Clause-blue.svg)](https://opensource.org/licenses/BSD-3-Clause)
 [![Open in Visual Studio Code](https://img.shields.io/badge/vscode-open-blue?logo=visualstudiocode)](https://open.vscode.dev/ComPWA/sphinx-api-relink)
 [![CI status](https://github.com/ComPWA/sphinx-api-relink/workflows/CI/badge.svg)](https://github.com/ComPWA/sphinx-api-relink/actions?query=branch%3Amain+workflow%3ACI)
 [![Checked with mypy](http://www.mypy-lang.org/static/mypy_badge.svg)](https://mypy.readthedocs.io)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/ComPWA/sphinx-api-relink/main.svg)](https://results.pre-commit.ci/latest/github/ComPWA/sphinx-api-relink/main)
 [![Spelling checked](https://img.shields.io/badge/cspell-checked-brightgreen.svg)](https://github.com/streetsidesoftware/cspell/tree/master/packages/cspell)
 [![code style: prettier](https://img.shields.io/badge/code_style-prettier-ff69b4.svg?style=flat-square)](https://github.com/prettier/prettier)
-[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
 
 This package is a plugin for the [`sphinx.ext.autodoc`](https://www.sphinx-doc.org/en/master/usage/extensions/autodoc.html) extension. The [`autodoc_type_aliases`](https://www.sphinx-doc.org/en/master/usage/extensions/autodoc.html#confval-autodoc_type_aliases) configuration does not always work well when using postponed evaluation of annotations ([PEP 563](https://peps.python.org/pep-0563), i.e. `from __future__ import annotations`) or when importing through [`typing.TYPE_CHECKING`](https://docs.python.org/3/library/typing.html#typing.TYPE_CHECKING), because `sphinx.ext.autodoc` generates the API dynamically (not statically, as opposed to [`sphinx-autoapi`](https://github.com/readthedocs/sphinx-autoapi)).
 
 ## Installation
 
 Just install through [PyPI](https://pypi.org) with `pip`:
```

### Comparing `sphinx-api-relink-0.0.8/pyproject.toml` & `sphinx_api_relink-0.0.9/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -42,30 +42,25 @@
 license = {text = "BSD 3-Clause License"}
 maintainers = [{email = "compwa-admin@ep1.rub.de"}]
 name = "sphinx-api-relink"
 requires-python = ">=3.7"
 
 [project.optional-dependencies]
 dev = ["sphinx-api-relink[sty]"]
-format = ["black"]
-lint = [
+sty = [
+    "mypy",
+    "pre-commit >=1.4.0",
     "ruff",
-    "sphinx-api-relink[mypy]",
+    "sphinx-api-relink[types]",
 ]
-mypy = [
-    "mypy",
+types = [
     "types-colorama",
     "types-docutils",
     "types-requests",
 ]
-sty = [
-    "pre-commit >=1.4.0",
-    "sphinx-api-relink[format]",
-    "sphinx-api-relink[lint]",
-]
 
 [project.readme]
 content-type = "text/markdown"
 file = "README.md"
 
 [project.urls]
 Changelog = "https://github.com/ComPWA/sphinx-api-relink/releases"
@@ -87,39 +82,14 @@
 [tool.setuptools.packages.find]
 namespaces = false
 where = ["src"]
 
 [tool.setuptools_scm]
 write_to = "src/version.py"
 
-[tool.black]
-exclude = '''
-/(
-    .*\.egg-info
-    | .*build
-    | \.eggs
-    | \.git
-    | \.pytest_cache
-    | \.tox
-    | \.venv
-    | \.vscode
-    | dist
-)/
-'''
-include = '\.pyi?$'
-preview = true
-target-version = [
-    "py310",
-    "py311",
-    "py312",
-    "py37",
-    "py38",
-    "py39",
-]
-
 [tool.coverage.run]
 branch = true
 source = ["src"]
 
 [tool.mypy]
 disallow_incomplete_defs = true
 disallow_untyped_defs = true
@@ -153,14 +123,24 @@
 reportUnusedClass = true
 reportUnusedFunction = true
 reportUnusedImport = true
 reportUnusedVariable = true
 typeCheckingMode = "strict"
 
 [tool.ruff]
+preview = true
+show-fixes = true
+src = ["src"]
+target-version = "py37"
+
+[tool.ruff.format]
+docstring-code-format = true
+line-ending = "lf"
+
+[tool.ruff.lint]
 extend-select = [
     "A",
     "B",
     "BLE",
     "C4",
     "C90",
     "D",
@@ -197,35 +177,38 @@
     "D105",
     "D107",
     "D203",
     "D213",
     "D407",
     "D416",
     "E501",
+    "ISC001",
+    "PLW1514",
     "PLW2901",
+    "S404",
     "SIM108",
     "UP036",
 ]
-show-fixes = true
-src = ["src"]
-target-version = "py37"
 task-tags = ["cspell"]
 
-[tool.ruff.per-file-ignores]
+[tool.ruff.lint.isort]
+split-on-trailing-comma = false
+
+[tool.ruff.lint.per-file-ignores]
 "setup.py" = ["D100"]
 "tests/*" = [
     "D",
     "INP001",
     "PGH001",
     "PLR0913",
     "PLR2004",
     "S101",
 ]
 
-[tool.ruff.pydocstyle]
+[tool.ruff.lint.pydocstyle]
 convention = "google"
 
 [tool.tomlsort]
 all = false
 ignore_case = true
 in_place = true
 sort_first = [
```

### Comparing `sphinx-api-relink-0.0.8/src/sphinx_api_relink/__init__.py` & `sphinx_api_relink-0.0.9/src/sphinx_api_relink/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,35 @@
+# pyright: reportAttributeAccessIssue=false
 from __future__ import annotations
 
 import shutil
+import sys
 from pathlib import Path
 from typing import TYPE_CHECKING, Any
 
 import sphinx.domains.python
 from docutils import nodes
 from sphinx.addnodes import pending_xref, pending_xref_condition
-from sphinx.domains.python import parse_reftarget
 from sphinx.ext.apidoc import main as sphinx_apidoc
 
 from sphinx_api_relink.linkcode import get_linkcode_resolve
 
+if sys.version_info < (3, 8):
+    from importlib_metadata import version
+else:
+    from importlib.metadata import version
+
+__SPHINX_VERSION = tuple(int(i) for i in version("sphinx").split(".") if i.isdigit())
+if __SPHINX_VERSION < (7, 3):
+    from sphinx.domains.python import parse_reftarget  # type:ignore[attr-defined]
+else:
+    from sphinx.domains.python._annotations import (  # type:ignore[import-not-found,no-redef]
+        parse_reftarget,  # noqa: PLC2701
+    )
+
 if TYPE_CHECKING:
     from docutils.parsers.rst.states import Inliner
     from sphinx.application import Sphinx
     from sphinx.environment import BuildEnvironment
     from sphinx.util.typing import RoleFunction
 
 
@@ -39,15 +53,15 @@
 
 
 def set_linkcode_resolve(app: Sphinx, _: BuildEnvironment) -> None:
     github_repo: str | None = app.config.api_github_repo
     if github_repo is None:
         return
     debug: bool = app.config.api_linkcode_debug
-    app.config.linkcode_resolve = get_linkcode_resolve(github_repo, debug)  # type: ignore[attr-defined]
+    app.config.linkcode_resolve = get_linkcode_resolve(github_repo, debug)  # type:ignore[attr-defined]
     app.setup_extension("sphinx.ext.linkcode")
 
 
 def generate_apidoc(app: Sphinx, _: BuildEnvironment) -> None:
     config_key = "generate_apidoc_package_path"
     package_path: list[str] | str | None = getattr(app.config, config_key, None)
     if package_path is None:
@@ -104,15 +118,15 @@
     ref_types = _get_target_types(app)
     ref_types.update({
         v[1]: v[0] for v in target_substitutions.values() if isinstance(v, tuple)
     })
 
     def _new_type_to_xref(
         target: str,
-        env: BuildEnvironment | None = None,  # type: ignore[assignment]
+        env: BuildEnvironment | None = None,  # type:ignore[assignment]
         suppress_prefix: bool = False,
     ) -> pending_xref:
         reftype, target, title, refspecific = parse_reftarget(target, suppress_prefix)
         target = ref_targets.get(target, target)
         reftype = ref_types.get(target, reftype)
         if env is None:
             msg = "Environment cannot be None"
@@ -123,15 +137,18 @@
             refdomain="py",
             reftype=reftype,
             reftarget=target,
             refspecific=refspecific,
             **_get_env_kwargs(env),
         )
 
-    sphinx.domains.python.type_to_xref = _new_type_to_xref
+    if __SPHINX_VERSION < (7, 3):
+        sphinx.domains.python.type_to_xref = _new_type_to_xref  # pyright:ignore[reportPrivateImportUsage]
+    else:
+        sphinx.domains.python._annotations.type_to_xref = _new_type_to_xref
 
 
 def _get_target_substitutions(app: Sphinx) -> dict[str, str | tuple[str, str]]:
     config_key = "api_target_substitutions"
     target_substitutions = getattr(app.config, config_key, {})
     if not isinstance(target_substitutions, dict):
         msg = f"{config_key} must be a dict, got {type(target_substitutions).__name__}"
@@ -189,15 +206,15 @@
             pending_xref_condition("", short_name, condition="resolved"),
             pending_xref_condition("", title, condition="*"),
         ]
     return [nodes.Text(short_name)]
 
 
 def wiki_role(pattern: str) -> RoleFunction:
-    def role(  # noqa: PLR0913
+    def role(  # noqa: PLR0913, PLR0917
         name: str,
         rawtext: str,
         text: str,
         lineno: int,
         inliner: Inliner,
         options: dict | None = None,
         content: list[str] | None = None,
@@ -206,8 +223,8 @@
         output_text = output_text.replace("_", " ")
         url = pattern % (text,)
         if options is None:
             options = {}
         reference_node = nodes.reference(rawtext, output_text, refuri=url, **options)
         return [reference_node], []
 
-    return role
+    return role  # type:ignore[return-value]
```

### Comparing `sphinx-api-relink-0.0.8/src/sphinx_api_relink/helpers.py` & `sphinx_api_relink-0.0.9/src/sphinx_api_relink/helpers.py`

 * *Files 0% similar despite different names*

```diff
@@ -100,15 +100,15 @@
     if matches is None:
         msg = f"Could not find documentation for {package_name} v{installed_version}"
         raise ValueError(msg)
     return matches[1]
 
 
 def set_intersphinx_version_remapping(
-    version_remapping: dict[str, dict[str, str]]
+    version_remapping: dict[str, dict[str, str]],
 ) -> None:
     if not isinstance(version_remapping, dict):
         msg = (
             "intersphinx_relink_versions must be a dict, got a"
             f" {type(version_remapping).__name__}"
         )
         raise TypeError(msg)
```

### Comparing `sphinx-api-relink-0.0.8/src/sphinx_api_relink/linkcode.py` & `sphinx_api_relink-0.0.9/src/sphinx_api_relink/linkcode.py`

 * *Files identical despite different names*

### Comparing `sphinx-api-relink-0.0.8/src/sphinx_api_relink/templates/package.rst_t` & `sphinx_api_relink-0.0.9/src/sphinx_api_relink/templates/package.rst_t`

 * *Files identical despite different names*

### Comparing `sphinx-api-relink-0.0.8/src/sphinx_api_relink.egg-info/PKG-INFO` & `sphinx_api_relink-0.0.9/src/sphinx_api_relink.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sphinx-api-relink
-Version: 0.0.8
+Version: 0.0.9
 Summary: Relink type hints in your Sphinx API
 Author-email: Common Partial Wave Analysis <compwa-admin@ep1.rub.de>
 Maintainer-email: compwa-admin@ep1.rub.de
 License: BSD 3-Clause License
 Project-URL: Changelog, https://github.com/ComPWA/sphinx-api-relink/releases
 Project-URL: Documentation, https://github.com/ComPWA/sphinx-api-relink/blob/main/README.md
 Project-URL: Source, https://github.com/ComPWA/sphinx-api-relink
@@ -31,41 +31,35 @@
 Requires-Dist: Sphinx>=4.4
 Requires-Dist: colorama
 Requires-Dist: docutils
 Requires-Dist: importlib-metadata; python_version < "3.8.0"
 Requires-Dist: typing-extensions; python_version < "3.8.0"
 Provides-Extra: dev
 Requires-Dist: sphinx-api-relink[sty]; extra == "dev"
-Provides-Extra: format
-Requires-Dist: black; extra == "format"
-Provides-Extra: lint
-Requires-Dist: ruff; extra == "lint"
-Requires-Dist: sphinx-api-relink[mypy]; extra == "lint"
-Provides-Extra: mypy
-Requires-Dist: mypy; extra == "mypy"
-Requires-Dist: types-colorama; extra == "mypy"
-Requires-Dist: types-docutils; extra == "mypy"
-Requires-Dist: types-requests; extra == "mypy"
 Provides-Extra: sty
+Requires-Dist: mypy; extra == "sty"
 Requires-Dist: pre-commit>=1.4.0; extra == "sty"
-Requires-Dist: sphinx-api-relink[format]; extra == "sty"
-Requires-Dist: sphinx-api-relink[lint]; extra == "sty"
+Requires-Dist: ruff; extra == "sty"
+Requires-Dist: sphinx-api-relink[types]; extra == "sty"
+Provides-Extra: types
+Requires-Dist: types-colorama; extra == "types"
+Requires-Dist: types-docutils; extra == "types"
+Requires-Dist: types-requests; extra == "types"
 
 # `sphinx-api-relink`
 
 [![PyPI package](https://badge.fury.io/py/sphinx-api-relink.svg)](https://pypi.org/project/sphinx-api-relink)
 [![Supported Python versions](https://img.shields.io/pypi/pyversions/sphinx-api-relink)](https://pypi.org/project/sphinx-api-relink)
 [![BSD 3-Clause license](https://img.shields.io/badge/License-BSD_3--Clause-blue.svg)](https://opensource.org/licenses/BSD-3-Clause)
 [![Open in Visual Studio Code](https://img.shields.io/badge/vscode-open-blue?logo=visualstudiocode)](https://open.vscode.dev/ComPWA/sphinx-api-relink)
 [![CI status](https://github.com/ComPWA/sphinx-api-relink/workflows/CI/badge.svg)](https://github.com/ComPWA/sphinx-api-relink/actions?query=branch%3Amain+workflow%3ACI)
 [![Checked with mypy](http://www.mypy-lang.org/static/mypy_badge.svg)](https://mypy.readthedocs.io)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/ComPWA/sphinx-api-relink/main.svg)](https://results.pre-commit.ci/latest/github/ComPWA/sphinx-api-relink/main)
 [![Spelling checked](https://img.shields.io/badge/cspell-checked-brightgreen.svg)](https://github.com/streetsidesoftware/cspell/tree/master/packages/cspell)
 [![code style: prettier](https://img.shields.io/badge/code_style-prettier-ff69b4.svg?style=flat-square)](https://github.com/prettier/prettier)
-[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
 
 This package is a plugin for the [`sphinx.ext.autodoc`](https://www.sphinx-doc.org/en/master/usage/extensions/autodoc.html) extension. The [`autodoc_type_aliases`](https://www.sphinx-doc.org/en/master/usage/extensions/autodoc.html#confval-autodoc_type_aliases) configuration does not always work well when using postponed evaluation of annotations ([PEP 563](https://peps.python.org/pep-0563), i.e. `from __future__ import annotations`) or when importing through [`typing.TYPE_CHECKING`](https://docs.python.org/3/library/typing.html#typing.TYPE_CHECKING), because `sphinx.ext.autodoc` generates the API dynamically (not statically, as opposed to [`sphinx-autoapi`](https://github.com/readthedocs/sphinx-autoapi)).
 
 ## Installation
 
 Just install through [PyPI](https://pypi.org) with `pip`:
```

### Comparing `sphinx-api-relink-0.0.8/src/sphinx_api_relink.egg-info/SOURCES.txt` & `sphinx_api_relink-0.0.9/src/sphinx_api_relink.egg-info/SOURCES.txt`

 * *Files identical despite different names*

