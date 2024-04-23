# Comparing `tmp/mb_pytorch_lightning-1.0.10.tar.gz` & `tmp/mb_pytorch_lightning-1.0.11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mb_pytorch_lightning-1.0.10.tar", last modified: Tue Apr 23 15:46:00 2024, max compression
+gzip compressed data, was "mb_pytorch_lightning-1.0.11.tar", last modified: Tue Apr 23 16:23:50 2024, max compression
```

## Comparing `mb_pytorch_lightning-1.0.10.tar` & `mb_pytorch_lightning-1.0.11.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxr-x   0 winnow    (1000) winnow    (1000)        0 2024-04-23 15:46:00.347295 mb_pytorch_lightning-1.0.10/
--rw-r--r--   0 winnow    (1000) winnow    (1000)      186 2024-04-23 15:46:00.347295 mb_pytorch_lightning-1.0.10/PKG-INFO
--rw-rw-r--   0 winnow    (1000) winnow    (1000)       44 2024-04-23 15:19:59.000000 mb_pytorch_lightning-1.0.10/README.md
-drwxrwxr-x   0 winnow    (1000) winnow    (1000)        0 2024-04-23 15:46:00.347295 mb_pytorch_lightning-1.0.10/mb_pytorch_lightning.egg-info/
--rw-r--r--   0 winnow    (1000) winnow    (1000)      186 2024-04-23 15:46:00.000000 mb_pytorch_lightning-1.0.10/mb_pytorch_lightning.egg-info/PKG-INFO
--rw-rw-r--   0 winnow    (1000) winnow    (1000)      252 2024-04-23 15:46:00.000000 mb_pytorch_lightning-1.0.10/mb_pytorch_lightning.egg-info/SOURCES.txt
--rw-rw-r--   0 winnow    (1000) winnow    (1000)        1 2024-04-23 15:46:00.000000 mb_pytorch_lightning-1.0.10/mb_pytorch_lightning.egg-info/dependency_links.txt
--rw-rw-r--   0 winnow    (1000) winnow    (1000)        8 2024-04-23 15:46:00.000000 mb_pytorch_lightning-1.0.10/mb_pytorch_lightning.egg-info/requires.txt
--rw-rw-r--   0 winnow    (1000) winnow    (1000)        1 2024-04-23 15:46:00.000000 mb_pytorch_lightning-1.0.10/mb_pytorch_lightning.egg-info/top_level.txt
--rw-rw-r--   0 winnow    (1000) winnow    (1000)       81 2024-04-23 15:27:02.000000 mb_pytorch_lightning-1.0.10/pyproject.toml
--rw-rw-r--   0 winnow    (1000) winnow    (1000)       38 2024-04-23 15:46:00.347295 mb_pytorch_lightning-1.0.10/setup.cfg
--rwxrwxr-x   0 winnow    (1000) winnow    (1000)      807 2024-04-23 15:45:16.000000 mb_pytorch_lightning-1.0.10/setup.py
+drwxrwxr-x   0 winnow    (1000) winnow    (1000)        0 2024-04-23 16:23:50.052241 mb_pytorch_lightning-1.0.11/
+-rw-r--r--   0 winnow    (1000) winnow    (1000)      243 2024-04-23 16:23:50.052241 mb_pytorch_lightning-1.0.11/PKG-INFO
+-rw-rw-r--   0 winnow    (1000) winnow    (1000)       44 2024-04-23 15:19:59.000000 mb_pytorch_lightning-1.0.11/README.md
+drwxrwxr-x   0 winnow    (1000) winnow    (1000)        0 2024-04-23 16:23:50.052241 mb_pytorch_lightning-1.0.11/mb_pytorch_lightning.egg-info/
+-rw-r--r--   0 winnow    (1000) winnow    (1000)      243 2024-04-23 16:23:50.000000 mb_pytorch_lightning-1.0.11/mb_pytorch_lightning.egg-info/PKG-INFO
+-rw-rw-r--   0 winnow    (1000) winnow    (1000)      252 2024-04-23 16:23:50.000000 mb_pytorch_lightning-1.0.11/mb_pytorch_lightning.egg-info/SOURCES.txt
+-rw-rw-r--   0 winnow    (1000) winnow    (1000)        1 2024-04-23 16:23:50.000000 mb_pytorch_lightning-1.0.11/mb_pytorch_lightning.egg-info/dependency_links.txt
+-rw-rw-r--   0 winnow    (1000) winnow    (1000)       35 2024-04-23 16:23:50.000000 mb_pytorch_lightning-1.0.11/mb_pytorch_lightning.egg-info/requires.txt
+-rw-rw-r--   0 winnow    (1000) winnow    (1000)        1 2024-04-23 16:23:50.000000 mb_pytorch_lightning-1.0.11/mb_pytorch_lightning.egg-info/top_level.txt
+-rw-rw-r--   0 winnow    (1000) winnow    (1000)       81 2024-04-23 15:27:02.000000 mb_pytorch_lightning-1.0.11/pyproject.toml
+-rw-rw-r--   0 winnow    (1000) winnow    (1000)       38 2024-04-23 16:23:50.052241 mb_pytorch_lightning-1.0.11/setup.cfg
+-rwxrwxr-x   0 winnow    (1000) winnow    (1000)      856 2024-04-23 15:56:44.000000 mb_pytorch_lightning-1.0.11/setup.py
```

### Comparing `mb_pytorch_lightning-1.0.10/setup.py` & `mb_pytorch_lightning-1.0.11/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,15 +10,17 @@
     name="mb_pytorch_lightning",
     description="Production Planing functions package",
     author=["Malav Bateriwala"],
     packages=find_packages(),
     #packages=find_packages(),
     scripts=[],
     install_requires=[
-        "mb_base",],
+        "mb_base",
+        "mb_utils",
+        "pytorch_lightning",],
     setup_requires=["setuptools-git-versioning<2"],
     python_requires='>=3.8',
     setuptools_git_versioning={
         "enabled": True,
         "version_file": VERSION_FILE,
         "count_commits_from_version_file": True,
         "template": "{tag}",
```

