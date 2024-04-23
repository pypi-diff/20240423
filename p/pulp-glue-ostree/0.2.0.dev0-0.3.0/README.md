# Comparing `tmp/pulp-glue-ostree-0.2.0.dev0.tar.gz` & `tmp/pulp-glue-ostree-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulp-glue-ostree-0.2.0.dev0.tar", last modified: Mon Apr  3 11:54:53 2023, max compression
+gzip compressed data, was "pulp-glue-ostree-0.3.0.tar", last modified: Tue Apr 23 17:35:29 2024, max compression
```

## Comparing `pulp-glue-ostree-0.2.0.dev0.tar` & `pulp-glue-ostree-0.3.0.tar`

### file list

```diff
@@ -1,17 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 11:54:53.808955 pulp-glue-ostree-0.2.0.dev0/
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-04-03 11:54:53.808955 pulp-glue-ostree-0.2.0.dev0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-03 11:54:44.000000 pulp-glue-ostree-0.2.0.dev0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 11:54:53.804955 pulp-glue-ostree-0.2.0.dev0/pulp_glue/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 11:54:53.804955 pulp-glue-ostree-0.2.0.dev0/pulp_glue/ostree/
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-03 11:54:44.000000 pulp-glue-ostree-0.2.0.dev0/pulp_glue/ostree/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3908 2023-04-03 11:54:44.000000 pulp-glue-ostree-0.2.0.dev0/pulp_glue/ostree/context.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 11:54:44.000000 pulp-glue-ostree-0.2.0.dev0/pulp_glue/ostree/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 11:54:53.804955 pulp-glue-ostree-0.2.0.dev0/pulp_glue_ostree.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-04-03 11:54:53.000000 pulp-glue-ostree-0.2.0.dev0/pulp_glue_ostree.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-04-03 11:54:53.000000 pulp-glue-ostree-0.2.0.dev0/pulp_glue_ostree.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-03 11:54:53.000000 pulp-glue-ostree-0.2.0.dev0/pulp_glue_ostree.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-03 11:54:53.000000 pulp-glue-ostree-0.2.0.dev0/pulp_glue_ostree.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-03 11:54:53.000000 pulp-glue-ostree-0.2.0.dev0/pulp_glue_ostree.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-03 11:54:44.000000 pulp-glue-ostree-0.2.0.dev0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-03 11:54:53.808955 pulp-glue-ostree-0.2.0.dev0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-04-03 11:54:44.000000 pulp-glue-ostree-0.2.0.dev0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 17:35:29.827659 pulp-glue-ostree-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      887 2024-04-23 17:35:29.827659 pulp-glue-ostree-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-23 17:35:17.000000 pulp-glue-ostree-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 17:35:29.827659 pulp-glue-ostree-0.3.0/pulp_glue/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 17:35:29.827659 pulp-glue-ostree-0.3.0/pulp_glue/ostree/
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-23 17:35:17.000000 pulp-glue-ostree-0.3.0/pulp_glue/ostree/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3908 2024-04-23 17:35:17.000000 pulp-glue-ostree-0.3.0/pulp_glue/ostree/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 17:35:17.000000 pulp-glue-ostree-0.3.0/pulp_glue/ostree/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 17:35:29.827659 pulp-glue-ostree-0.3.0/pulp_glue_ostree.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      887 2024-04-23 17:35:29.000000 pulp-glue-ostree-0.3.0/pulp_glue_ostree.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      306 2024-04-23 17:35:29.000000 pulp-glue-ostree-0.3.0/pulp_glue_ostree.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 17:35:29.000000 pulp-glue-ostree-0.3.0/pulp_glue_ostree.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-23 17:35:29.000000 pulp-glue-ostree-0.3.0/pulp_glue_ostree.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-23 17:35:29.000000 pulp-glue-ostree-0.3.0/pulp_glue_ostree.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-04-23 17:35:17.000000 pulp-glue-ostree-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 17:35:29.827659 pulp-glue-ostree-0.3.0/setup.cfg
```

### Comparing `pulp-glue-ostree-0.2.0.dev0/pulp_glue/ostree/context.py` & `pulp-glue-ostree-0.3.0/pulp_glue/ostree/context.py`

 * *Files identical despite different names*

