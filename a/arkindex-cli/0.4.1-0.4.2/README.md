# Comparing `tmp/arkindex-cli-0.4.1.tar.gz` & `tmp/arkindex-cli-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arkindex-cli-0.4.1.tar", last modified: Mon Mar 11 12:48:02 2024, max compression
+gzip compressed data, was "arkindex-cli-0.4.2.tar", last modified: Tue Apr 23 14:41:52 2024, max compression
```

## Comparing `arkindex-cli-0.4.1.tar` & `arkindex-cli-0.4.2.tar`

### file list

```diff
@@ -1,70 +1,71 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-11 12:48:02.214686 arkindex-cli-0.4.1/
--rw-rw-rw-   0 root         (0) root         (0)      104 2024-03-11 12:46:34.000000 arkindex-cli-0.4.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1342 2024-03-11 12:48:02.214686 arkindex-cli-0.4.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1062 2024-03-11 12:46:34.000000 arkindex-cli-0.4.1/README.md
--rw-rw-rw-   0 root         (0) root         (0)        6 2024-03-11 12:46:34.000000 arkindex-cli-0.4.1/VERSION
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-11 12:48:02.206687 arkindex-cli-0.4.1/arkindex_cli/
--rw-rw-rw-   0 root         (0) root         (0)      501 2024-03-11 12:46:34.000000 arkindex-cli-0.4.1/arkindex_cli/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1792 2024-03-11 12:46:34.000000 arkindex-cli-0.4.1/arkindex_cli/argtypes.py
--rw-rw-rw-   0 root         (0) root         (0)     6890 2024-03-11 12:46:34.000000 arkindex-cli-0.4.1/arkindex_cli/auth.py
--rw-rw-rw-   0 root         (0) root         (0)     2882 2024-03-11 12:46:34.000000 arkindex-cli-0.4.1/arkindex_cli/cli.py
--rw-rw-rw-   0 root         (0) root         (0)      658 2024-03-11 12:46:34.000000 arkindex-cli-0.4.1/arkindex_cli/client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-11 12:48:02.210687 arkindex-cli-0.4.1/arkindex_cli/commands/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-11 12:47:59.000000 arkindex-cli-0.4.1/arkindex_cli/commands/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2415 2024-03-11 12:46:34.000000 arkindex-cli-0.4.1/arkindex_cli/commands/benchmark.py
--rw-rw-rw-   0 root         (0) root         (0)     1901 2024-03-11 12:46:34.000000 arkindex-cli-0.4.1/arkindex_cli/commands/classes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-11 12:48:02.210687 arkindex-cli-0.4.1/arkindex_cli/commands/elements/
--rw-rw-rw-   0 root         (0) root         (0)     1005 2024-03-11 12:46:34.000000 arkindex-cli-0.4.1/arkindex_cli/commands/elements/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2855 2024-03-11 12:46:34.000000 arkindex-cli-0.4.1/arkindex_cli/commands/elements/link.py
--rw-rw-rw-   0 root         (0) root         (0)    11955 2024-03-11 12:46:34.000000 arkindex-cli-0.4.1/arkindex_cli/commands/elements/ml_splits.py
--rw-rw-rw-   0 root         (0) root         (0)     4832 2024-03-11 12:46:34.000000 arkindex-cli-0.4.1/arkindex_cli/commands/elements/page_copy.py
--rw-rw-rw-   0 root         (0) root         (0)     4772 2024-03-11 12:46:34.000000 arkindex-cli-0.4.1/arkindex_cli/commands/elements/reject_classifications.py
--rw-rw-rw-   0 root         (0) root         (0)     2666 2024-03-11 12:46:34.000000 arkindex-cli-0.4.1/arkindex_cli/commands/elements/unlink.py
--rw-rw-rw-   0 root         (0) root         (0)     5792 2024-03-11 12:46:34.000000 arkindex-cli-0.4.1/arkindex_cli/commands/elements/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-11 12:48:02.210687 arkindex-cli-0.4.1/arkindex_cli/commands/export/
--rw-rw-rw-   0 root         (0) root         (0)     1186 2024-03-11 12:46:34.000000 arkindex-cli-0.4.1/arkindex_cli/commands/export/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    17840 2024-03-11 12:46:34.000000 arkindex-cli-0.4.1/arkindex_cli/commands/export/alto.py
--rw-rw-rw-   0 root         (0) root         (0)    20772 2024-03-11 12:46:34.000000 arkindex-cli-0.4.1/arkindex_cli/commands/export/csv.py
--rw-rw-rw-   0 root         (0) root         (0)     8387 2024-03-11 12:46:34.000000 arkindex-cli-0.4.1/arkindex_cli/commands/export/docx.py
--rw-rw-rw-   0 root         (0) root         (0)     3222 2024-03-11 12:46:34.000000 arkindex-cli-0.4.1/arkindex_cli/commands/export/entities.py
--rw-rw-rw-   0 root         (0) root         (0)    13259 2024-03-11 12:46:34.000000 arkindex-cli-0.4.1/arkindex_cli/commands/export/pdf.py
--rw-rw-rw-   0 root         (0) root         (0)     2702 2024-03-11 12:46:34.000000 arkindex-cli-0.4.1/arkindex_cli/commands/export/utils.py
--rw-rw-rw-   0 root         (0) root         (0)     2294 2024-03-11 12:46:34.000000 arkindex-cli-0.4.1/arkindex_cli/commands/login.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-11 12:48:02.210687 arkindex-cli-0.4.1/arkindex_cli/commands/models/
--rw-rw-rw-   0 root         (0) root         (0)      531 2024-03-11 12:46:34.000000 arkindex-cli-0.4.1/arkindex_cli/commands/models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3805 2024-03-11 12:46:34.000000 arkindex-cli-0.4.1/arkindex_cli/commands/models/publish.py
--rw-rw-rw-   0 root         (0) root         (0)     6981 2024-03-11 12:46:34.000000 arkindex-cli-0.4.1/arkindex_cli/commands/models/utils.py
--rw-rw-rw-   0 root         (0) root         (0)     2577 2024-03-11 12:46:34.000000 arkindex-cli-0.4.1/arkindex_cli/commands/secrets.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-11 12:48:02.210687 arkindex-cli-0.4.1/arkindex_cli/commands/selection/
--rw-rw-rw-   0 root         (0) root         (0)      544 2024-03-11 12:46:34.000000 arkindex-cli-0.4.1/arkindex_cli/commands/selection/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3672 2024-03-11 12:46:34.000000 arkindex-cli-0.4.1/arkindex_cli/commands/selection/populate.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-11 12:48:02.210687 arkindex-cli-0.4.1/arkindex_cli/commands/upload/
--rw-rw-rw-   0 root         (0) root         (0)      960 2024-03-11 12:46:34.000000 arkindex-cli-0.4.1/arkindex_cli/commands/upload/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-11 12:48:02.210687 arkindex-cli-0.4.1/arkindex_cli/commands/upload/alto/
--rw-rw-rw-   0 root         (0) root         (0)    34603 2024-03-11 12:46:34.000000 arkindex-cli-0.4.1/arkindex_cli/commands/upload/alto/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     9305 2024-03-11 12:46:34.000000 arkindex-cli-0.4.1/arkindex_cli/commands/upload/alto/parser.py
--rw-rw-rw-   0 root         (0) root         (0)     9393 2024-03-11 12:46:34.000000 arkindex-cli-0.4.1/arkindex_cli/commands/upload/iiif.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-11 12:48:02.210687 arkindex-cli-0.4.1/arkindex_cli/commands/upload/mets/
--rw-rw-rw-   0 root         (0) root         (0)     5179 2024-03-11 12:46:34.000000 arkindex-cli-0.4.1/arkindex_cli/commands/upload/mets/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      872 2024-03-11 12:46:34.000000 arkindex-cli-0.4.1/arkindex_cli/commands/upload/mets/cache.py
--rw-rw-rw-   0 root         (0) root         (0)    15192 2024-03-11 12:46:34.000000 arkindex-cli-0.4.1/arkindex_cli/commands/upload/mets/parser.py
--rw-rw-rw-   0 root         (0) root         (0)     4308 2024-03-11 12:46:34.000000 arkindex-cli-0.4.1/arkindex_cli/commands/upload/minio_client.py
--rw-rw-rw-   0 root         (0) root         (0)     8125 2024-03-11 12:46:34.000000 arkindex-cli-0.4.1/arkindex_cli/commands/upload/page_xml_import.py
--rw-rw-rw-   0 root         (0) root         (0)     4270 2024-03-11 12:46:34.000000 arkindex-cli-0.4.1/arkindex_cli/commands/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-11 12:48:02.210687 arkindex-cli-0.4.1/arkindex_cli/commands/worker/
--rw-rw-rw-   0 root         (0) root         (0)      560 2024-03-11 12:46:34.000000 arkindex-cli-0.4.1/arkindex_cli/commands/worker/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4908 2024-03-11 12:46:34.000000 arkindex-cli-0.4.1/arkindex_cli/commands/worker/publish.py
--rw-rw-rw-   0 root         (0) root         (0)     3562 2024-03-11 12:46:34.000000 arkindex-cli-0.4.1/arkindex_cli/git.py
--rw-rw-rw-   0 root         (0) root         (0)      966 2024-03-11 12:46:34.000000 arkindex-cli-0.4.1/arkindex_cli/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-11 12:48:02.206687 arkindex-cli-0.4.1/arkindex_cli.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1342 2024-03-11 12:48:02.000000 arkindex-cli-0.4.1/arkindex_cli.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1929 2024-03-11 12:48:02.000000 arkindex-cli-0.4.1/arkindex_cli.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-11 12:48:02.000000 arkindex-cli-0.4.1/arkindex_cli.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       51 2024-03-11 12:48:02.000000 arkindex-cli-0.4.1/arkindex_cli.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      236 2024-03-11 12:48:02.000000 arkindex-cli-0.4.1/arkindex_cli.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2024-03-11 12:48:02.000000 arkindex-cli-0.4.1/arkindex_cli.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)       17 2024-03-11 12:46:34.000000 arkindex-cli-0.4.1/requirements-export.txt
--rw-rw-rw-   0 root         (0) root         (0)       58 2024-03-11 12:46:34.000000 arkindex-cli-0.4.1/requirements-tests.txt
--rw-rw-rw-   0 root         (0) root         (0)      209 2024-03-11 12:46:34.000000 arkindex-cli-0.4.1/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-03-11 12:48:02.214686 arkindex-cli-0.4.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1009 2024-03-11 12:46:34.000000 arkindex-cli-0.4.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 14:41:52.603089 arkindex-cli-0.4.2/
+-rw-rw-rw-   0 root         (0) root         (0)      104 2024-04-23 14:40:24.000000 arkindex-cli-0.4.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1342 2024-04-23 14:41:52.603089 arkindex-cli-0.4.2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1062 2024-04-23 14:40:24.000000 arkindex-cli-0.4.2/README.md
+-rw-rw-rw-   0 root         (0) root         (0)        6 2024-04-23 14:40:24.000000 arkindex-cli-0.4.2/VERSION
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 14:41:52.599089 arkindex-cli-0.4.2/arkindex_cli/
+-rw-rw-rw-   0 root         (0) root         (0)      979 2024-04-23 14:40:24.000000 arkindex-cli-0.4.2/arkindex_cli/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1792 2024-04-23 14:40:24.000000 arkindex-cli-0.4.2/arkindex_cli/argtypes.py
+-rw-rw-rw-   0 root         (0) root         (0)     6890 2024-04-23 14:40:24.000000 arkindex-cli-0.4.2/arkindex_cli/auth.py
+-rw-rw-rw-   0 root         (0) root         (0)     3126 2024-04-23 14:40:24.000000 arkindex-cli-0.4.2/arkindex_cli/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)      658 2024-04-23 14:40:24.000000 arkindex-cli-0.4.2/arkindex_cli/client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 14:41:52.599089 arkindex-cli-0.4.2/arkindex_cli/commands/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-23 14:41:50.000000 arkindex-cli-0.4.2/arkindex_cli/commands/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2415 2024-04-23 14:40:24.000000 arkindex-cli-0.4.2/arkindex_cli/commands/benchmark.py
+-rw-rw-rw-   0 root         (0) root         (0)     1901 2024-04-23 14:40:24.000000 arkindex-cli-0.4.2/arkindex_cli/commands/classes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 14:41:52.599089 arkindex-cli-0.4.2/arkindex_cli/commands/elements/
+-rw-rw-rw-   0 root         (0) root         (0)     1005 2024-04-23 14:40:24.000000 arkindex-cli-0.4.2/arkindex_cli/commands/elements/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2855 2024-04-23 14:40:24.000000 arkindex-cli-0.4.2/arkindex_cli/commands/elements/link.py
+-rw-rw-rw-   0 root         (0) root         (0)    11960 2024-04-23 14:40:24.000000 arkindex-cli-0.4.2/arkindex_cli/commands/elements/ml_splits.py
+-rw-rw-rw-   0 root         (0) root         (0)     4832 2024-04-23 14:40:24.000000 arkindex-cli-0.4.2/arkindex_cli/commands/elements/page_copy.py
+-rw-rw-rw-   0 root         (0) root         (0)     4772 2024-04-23 14:40:24.000000 arkindex-cli-0.4.2/arkindex_cli/commands/elements/reject_classifications.py
+-rw-rw-rw-   0 root         (0) root         (0)     2666 2024-04-23 14:40:24.000000 arkindex-cli-0.4.2/arkindex_cli/commands/elements/unlink.py
+-rw-rw-rw-   0 root         (0) root         (0)     5792 2024-04-23 14:40:24.000000 arkindex-cli-0.4.2/arkindex_cli/commands/elements/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 14:41:52.599089 arkindex-cli-0.4.2/arkindex_cli/commands/export/
+-rw-rw-rw-   0 root         (0) root         (0)     1186 2024-04-23 14:40:24.000000 arkindex-cli-0.4.2/arkindex_cli/commands/export/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    17840 2024-04-23 14:40:24.000000 arkindex-cli-0.4.2/arkindex_cli/commands/export/alto.py
+-rw-rw-rw-   0 root         (0) root         (0)    20772 2024-04-23 14:40:24.000000 arkindex-cli-0.4.2/arkindex_cli/commands/export/csv.py
+-rw-rw-rw-   0 root         (0) root         (0)     8387 2024-04-23 14:40:24.000000 arkindex-cli-0.4.2/arkindex_cli/commands/export/docx.py
+-rw-rw-rw-   0 root         (0) root         (0)     3222 2024-04-23 14:40:24.000000 arkindex-cli-0.4.2/arkindex_cli/commands/export/entities.py
+-rw-rw-rw-   0 root         (0) root         (0)    13259 2024-04-23 14:40:24.000000 arkindex-cli-0.4.2/arkindex_cli/commands/export/pdf.py
+-rw-rw-rw-   0 root         (0) root         (0)     2702 2024-04-23 14:40:24.000000 arkindex-cli-0.4.2/arkindex_cli/commands/export/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     2294 2024-04-23 14:40:24.000000 arkindex-cli-0.4.2/arkindex_cli/commands/login.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 14:41:52.599089 arkindex-cli-0.4.2/arkindex_cli/commands/models/
+-rw-rw-rw-   0 root         (0) root         (0)      531 2024-04-23 14:40:24.000000 arkindex-cli-0.4.2/arkindex_cli/commands/models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3822 2024-04-23 14:40:24.000000 arkindex-cli-0.4.2/arkindex_cli/commands/models/publish.py
+-rw-rw-rw-   0 root         (0) root         (0)     7008 2024-04-23 14:40:24.000000 arkindex-cli-0.4.2/arkindex_cli/commands/models/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     2577 2024-04-23 14:40:24.000000 arkindex-cli-0.4.2/arkindex_cli/commands/secrets.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 14:41:52.599089 arkindex-cli-0.4.2/arkindex_cli/commands/selection/
+-rw-rw-rw-   0 root         (0) root         (0)      544 2024-04-23 14:40:24.000000 arkindex-cli-0.4.2/arkindex_cli/commands/selection/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3672 2024-04-23 14:40:24.000000 arkindex-cli-0.4.2/arkindex_cli/commands/selection/populate.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 14:41:52.603089 arkindex-cli-0.4.2/arkindex_cli/commands/upload/
+-rw-rw-rw-   0 root         (0) root         (0)      960 2024-04-23 14:40:24.000000 arkindex-cli-0.4.2/arkindex_cli/commands/upload/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 14:41:52.603089 arkindex-cli-0.4.2/arkindex_cli/commands/upload/alto/
+-rw-rw-rw-   0 root         (0) root         (0)    28888 2024-04-23 14:40:24.000000 arkindex-cli-0.4.2/arkindex_cli/commands/upload/alto/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    13729 2024-04-23 14:40:24.000000 arkindex-cli-0.4.2/arkindex_cli/commands/upload/alto/parser.py
+-rw-rw-rw-   0 root         (0) root         (0)     1131 2024-04-23 14:40:24.000000 arkindex-cli-0.4.2/arkindex_cli/commands/upload/cache.py
+-rw-rw-rw-   0 root         (0) root         (0)      147 2024-04-23 14:40:24.000000 arkindex-cli-0.4.2/arkindex_cli/commands/upload/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     9393 2024-04-23 14:40:24.000000 arkindex-cli-0.4.2/arkindex_cli/commands/upload/iiif.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 14:41:52.603089 arkindex-cli-0.4.2/arkindex_cli/commands/upload/mets/
+-rw-rw-rw-   0 root         (0) root         (0)     5612 2024-04-23 14:40:24.000000 arkindex-cli-0.4.2/arkindex_cli/commands/upload/mets/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    18633 2024-04-23 14:40:24.000000 arkindex-cli-0.4.2/arkindex_cli/commands/upload/mets/parser.py
+-rw-rw-rw-   0 root         (0) root         (0)     4308 2024-04-23 14:40:24.000000 arkindex-cli-0.4.2/arkindex_cli/commands/upload/minio_client.py
+-rw-rw-rw-   0 root         (0) root         (0)     8128 2024-04-23 14:40:24.000000 arkindex-cli-0.4.2/arkindex_cli/commands/upload/page_xml_import.py
+-rw-rw-rw-   0 root         (0) root         (0)     4270 2024-04-23 14:40:24.000000 arkindex-cli-0.4.2/arkindex_cli/commands/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 14:41:52.603089 arkindex-cli-0.4.2/arkindex_cli/commands/worker/
+-rw-rw-rw-   0 root         (0) root         (0)      560 2024-04-23 14:40:24.000000 arkindex-cli-0.4.2/arkindex_cli/commands/worker/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4908 2024-04-23 14:40:24.000000 arkindex-cli-0.4.2/arkindex_cli/commands/worker/publish.py
+-rw-rw-rw-   0 root         (0) root         (0)     3576 2024-04-23 14:40:24.000000 arkindex-cli-0.4.2/arkindex_cli/git.py
+-rw-rw-rw-   0 root         (0) root         (0)      966 2024-04-23 14:40:24.000000 arkindex-cli-0.4.2/arkindex_cli/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 14:41:52.599089 arkindex-cli-0.4.2/arkindex_cli.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1342 2024-04-23 14:41:52.000000 arkindex-cli-0.4.2/arkindex_cli.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1967 2024-04-23 14:41:52.000000 arkindex-cli-0.4.2/arkindex_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-23 14:41:52.000000 arkindex-cli-0.4.2/arkindex_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       51 2024-04-23 14:41:52.000000 arkindex-cli-0.4.2/arkindex_cli.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      236 2024-04-23 14:41:52.000000 arkindex-cli-0.4.2/arkindex_cli.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2024-04-23 14:41:52.000000 arkindex-cli-0.4.2/arkindex_cli.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)       17 2024-04-23 14:40:24.000000 arkindex-cli-0.4.2/requirements-export.txt
+-rw-rw-rw-   0 root         (0) root         (0)       58 2024-04-23 14:40:24.000000 arkindex-cli-0.4.2/requirements-tests.txt
+-rw-rw-rw-   0 root         (0) root         (0)      209 2024-04-23 14:40:24.000000 arkindex-cli-0.4.2/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-23 14:41:52.603089 arkindex-cli-0.4.2/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1009 2024-04-23 14:40:24.000000 arkindex-cli-0.4.2/setup.py
```

### Comparing `arkindex-cli-0.4.1/PKG-INFO` & `arkindex-cli-0.4.2/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arkindex-cli
-Version: 0.4.1
+Version: 0.4.2
 Summary: Arkindex CLI client easy and sexy to use
 Home-page: https://arkindex.teklia.com
 Author: Teklia
 Author-email: contact@teklia.com
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: export
```

### Comparing `arkindex-cli-0.4.1/README.md` & `arkindex-cli-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `arkindex-cli-0.4.1/arkindex_cli/argtypes.py` & `arkindex-cli-0.4.2/arkindex_cli/argtypes.py`

 * *Files identical despite different names*

### Comparing `arkindex-cli-0.4.1/arkindex_cli/auth.py` & `arkindex-cli-0.4.2/arkindex_cli/auth.py`

 * *Files identical despite different names*

### Comparing `arkindex-cli-0.4.1/arkindex_cli/cli.py` & `arkindex-cli-0.4.2/arkindex_cli/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # -*- coding: utf-8 -*-
 import argparse
 import errno
 import warnings
 from pathlib import Path
 
+from arkindex_cli import enable_verbose_mode
 from arkindex_cli.commands.benchmark import add_benchmark_parser
 from arkindex_cli.commands.classes import add_classes_parser
 from arkindex_cli.commands.elements import add_elements_parser
 from arkindex_cli.commands.export import add_export_parser
 from arkindex_cli.commands.login import add_login_parser
 from arkindex_cli.commands.models import add_models_parser
 from arkindex_cli.commands.secrets import add_secrets_parser
@@ -41,14 +42,21 @@
     )
     parser.add_argument(
         "--gitlab-secure-file",
         help="Path to a GitLab Secure File to load Arkindex profiles to use.",
         type=Path,
     )
 
+    parser.add_argument(
+        "-v",
+        "--verbose",
+        action="store_true",
+        help="Enable verbose mode",
+    )
+
     version = get_version()
     if version:
         parser.add_argument(
             "-V",
             "--version",
             action="version",
             version=f"%(prog)s {version}",
@@ -74,14 +82,18 @@
     # Ignore the deprecation warnings of the SQLite export functions, which are only intended for other scripts.
     warnings.filterwarnings(
         action="ignore", category=FutureWarning, module="arkindex_cli.commands.export"
     )
 
     parser = get_parser()
     args = vars(parser.parse_args())
+
+    if args.pop("verbose", False):
+        enable_verbose_mode()
+
     if "func" in args:
         # Run the subcommand's function
         try:
             status = args.pop("func")(**args)
             parser.exit(status=status)
         except KeyboardInterrupt:
             # Just quit silently on ^C instead of displaying a long traceback
```

### Comparing `arkindex-cli-0.4.1/arkindex_cli/client.py` & `arkindex-cli-0.4.2/arkindex_cli/client.py`

 * *Files identical despite different names*

### Comparing `arkindex-cli-0.4.1/arkindex_cli/commands/benchmark.py` & `arkindex-cli-0.4.2/arkindex_cli/commands/benchmark.py`

 * *Files identical despite different names*

### Comparing `arkindex-cli-0.4.1/arkindex_cli/commands/classes.py` & `arkindex-cli-0.4.2/arkindex_cli/commands/classes.py`

 * *Files identical despite different names*

### Comparing `arkindex-cli-0.4.1/arkindex_cli/commands/elements/__init__.py` & `arkindex-cli-0.4.2/arkindex_cli/commands/elements/__init__.py`

 * *Files identical despite different names*

### Comparing `arkindex-cli-0.4.1/arkindex_cli/commands/elements/link.py` & `arkindex-cli-0.4.2/arkindex_cli/commands/elements/link.py`

 * *Files identical despite different names*

### Comparing `arkindex-cli-0.4.1/arkindex_cli/commands/elements/ml_splits.py` & `arkindex-cli-0.4.2/arkindex_cli/commands/elements/ml_splits.py`

 * *Files 0% similar despite different names*

```diff
@@ -188,15 +188,15 @@
         try:
             dataset = self.api_client.request(
                 "CreateDataset",
                 id=self.project_id,
                 body={
                     "name": self.dataset_name,
                     "description": "Dataset created with the CLI command",
-                    "sets": list(splits),
+                    "set_names": list(splits),
                 },
             )
         except ErrorResponse as e:
             raise ValueError(
                 f"Failed creating dataset: {e.status_code} -- {e.content}"
             ) from e
         return dataset
```

### Comparing `arkindex-cli-0.4.1/arkindex_cli/commands/elements/page_copy.py` & `arkindex-cli-0.4.2/arkindex_cli/commands/elements/page_copy.py`

 * *Files identical despite different names*

### Comparing `arkindex-cli-0.4.1/arkindex_cli/commands/elements/reject_classifications.py` & `arkindex-cli-0.4.2/arkindex_cli/commands/elements/reject_classifications.py`

 * *Files identical despite different names*

### Comparing `arkindex-cli-0.4.1/arkindex_cli/commands/elements/unlink.py` & `arkindex-cli-0.4.2/arkindex_cli/commands/elements/unlink.py`

 * *Files identical despite different names*

### Comparing `arkindex-cli-0.4.1/arkindex_cli/commands/elements/utils.py` & `arkindex-cli-0.4.2/arkindex_cli/commands/elements/utils.py`

 * *Files identical despite different names*

### Comparing `arkindex-cli-0.4.1/arkindex_cli/commands/export/__init__.py` & `arkindex-cli-0.4.2/arkindex_cli/commands/export/__init__.py`

 * *Files identical despite different names*

### Comparing `arkindex-cli-0.4.1/arkindex_cli/commands/export/alto.py` & `arkindex-cli-0.4.2/arkindex_cli/commands/export/alto.py`

 * *Files identical despite different names*

### Comparing `arkindex-cli-0.4.1/arkindex_cli/commands/export/csv.py` & `arkindex-cli-0.4.2/arkindex_cli/commands/export/csv.py`

 * *Files identical despite different names*

### Comparing `arkindex-cli-0.4.1/arkindex_cli/commands/export/docx.py` & `arkindex-cli-0.4.2/arkindex_cli/commands/export/docx.py`

 * *Files identical despite different names*

### Comparing `arkindex-cli-0.4.1/arkindex_cli/commands/export/entities.py` & `arkindex-cli-0.4.2/arkindex_cli/commands/export/entities.py`

 * *Files identical despite different names*

### Comparing `arkindex-cli-0.4.1/arkindex_cli/commands/export/pdf.py` & `arkindex-cli-0.4.2/arkindex_cli/commands/export/pdf.py`

 * *Files identical despite different names*

### Comparing `arkindex-cli-0.4.1/arkindex_cli/commands/export/utils.py` & `arkindex-cli-0.4.2/arkindex_cli/commands/export/utils.py`

 * *Files identical despite different names*

### Comparing `arkindex-cli-0.4.1/arkindex_cli/commands/login.py` & `arkindex-cli-0.4.2/arkindex_cli/commands/login.py`

 * *Files identical despite different names*

### Comparing `arkindex-cli-0.4.1/arkindex_cli/commands/models/__init__.py` & `arkindex-cli-0.4.2/arkindex_cli/commands/models/__init__.py`

 * *Files identical despite different names*

### Comparing `arkindex-cli-0.4.1/arkindex_cli/commands/models/publish.py` & `arkindex-cli-0.4.2/arkindex_cli/commands/models/publish.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 # -*- coding: utf-8 -*-
 import logging
 import os
 from pathlib import Path
 from typing import Optional
 from uuid import UUID
 
-from arkindex import ArkindexClient
 from rich.progress import Progress
 
 from arkindex_cli.auth import Profiles
+from arkindex_cli.client import ArkindexAPIClient
 from arkindex_cli.commands.models.utils import (
     create_archive,
     create_model_version,
     create_or_retrieve_model,
     find_model_path,
     upload_to_s3,
     validate_model_version,
@@ -29,15 +29,15 @@
         description="Publish every ML models of this git repository.",
         help="Publish ML models to Arkindex.",
     )
     publish_parser.set_defaults(func=run)
 
 
 def publish_model(
-    client: ArkindexClient,
+    client: ArkindexAPIClient,
     name: str,
     model_path: Path,
     configuration: dict,
     tag: Optional[str],
     description_path: Optional[Path],
     parent: Optional[UUID],
 ) -> None:
```

### Comparing `arkindex-cli-0.4.1/arkindex_cli/commands/models/utils.py` & `arkindex-cli-0.4.2/arkindex_cli/commands/models/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,16 @@
 from typing import NewType, Optional, Tuple, Union
 from uuid import UUID
 
 import apistar
 import requests
 import zstandard as zstd
 from apistar.exceptions import ErrorResponse
-from arkindex import ArkindexClient
+
+from arkindex_cli.client import ArkindexAPIClient
 
 logger = logging.getLogger(__name__)
 CHUNK_SIZE = 1024
 
 
 FilePath = NewType("FilePath", Path)
 Hash = NewType("Hash", str)
@@ -115,15 +116,15 @@
 
     yield path_to_zst_archive, hash, size, archive_hash
 
     # Remove the zstd archive
     os.remove(path_to_zst_archive)
 
 
-def create_or_retrieve_model(client: ArkindexClient, name: str):
+def create_or_retrieve_model(client: ArkindexAPIClient, name: str):
     """Create a new model or retrieve the id of the existing one (with the same name)"""
     try:
         r = client.request("CreateModel", body={"name": name})
         # New model was created
         return r["id"]
     except apistar.exceptions.ErrorResponse as e:
         r = e.content
@@ -135,15 +136,15 @@
             # Model exists but user has no access to it, raise
             raise Exception(f"Permission denied to publish {name}")
         else:
             raise
 
 
 def create_model_version(
-    client: ArkindexClient,
+    client: ArkindexAPIClient,
     model_id: str,
     tag: Optional[str] = None,
     description_path: Optional[Path] = None,
     configuration: Optional[dict] = {},
     parent: Optional[UUID] = None,
 ) -> dict:
     model_version_body = build_clean_payload(
@@ -175,15 +176,15 @@
             data=archive,
             headers={"Content-Type": "application/zstd"},
         )
     r.raise_for_status()
 
 
 def validate_model_version(
-    client: ArkindexClient,
+    client: ArkindexAPIClient,
     model_version_id: Union[str, UUID],
     hash: str,
     size: int,
     archive_hash: str,
 ) -> dict:
     # Sets the model version as `Available`, once its archive has been uploaded to S3.
     logger.info("Validating the model version...")
@@ -201,15 +202,15 @@
             destroy_model_version(client=client, model_version_id=model_version_id)
             return e.content
         logger.error(f"Failed to update model version: {msg}")
         raise e
 
 
 def destroy_model_version(
-    client: ArkindexClient,
+    client: ArkindexAPIClient,
     model_version_id: Union[str, UUID],
 ) -> None:
     logger.info("Deleting the model version...")
     try:
         client.request(
             "DestroyModelVersion",
             id=model_version_id,
```

### Comparing `arkindex-cli-0.4.1/arkindex_cli/commands/secrets.py` & `arkindex-cli-0.4.2/arkindex_cli/commands/secrets.py`

 * *Files identical despite different names*

### Comparing `arkindex-cli-0.4.1/arkindex_cli/commands/selection/__init__.py` & `arkindex-cli-0.4.2/arkindex_cli/commands/selection/__init__.py`

 * *Files identical despite different names*

### Comparing `arkindex-cli-0.4.1/arkindex_cli/commands/selection/populate.py` & `arkindex-cli-0.4.2/arkindex_cli/commands/selection/populate.py`

 * *Files identical despite different names*

### Comparing `arkindex-cli-0.4.1/arkindex_cli/commands/upload/__init__.py` & `arkindex-cli-0.4.2/arkindex_cli/commands/upload/__init__.py`

 * *Files identical despite different names*

### Comparing `arkindex-cli-0.4.1/arkindex_cli/commands/upload/alto/__init__.py` & `arkindex-cli-0.4.2/arkindex_cli/commands/upload/alto/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,225 +1,157 @@
 # -*- coding: utf-8 -*-
 import csv
 import errno
 import itertools
-import json
 import logging
 import re
+from itertools import filterfalse
 from operator import itemgetter
 from pathlib import Path
-from typing import Dict, List, Optional, Union
+from typing import List, Optional, Union
 from uuid import UUID
 
 from apistar.exceptions import ErrorResponse
-from arkindex import ArkindexClient
 from lxml import etree as ET
 from lxml import objectify
 from requests.compat import quote
 from rich.progress import Progress, track
 
 from arkindex_cli.argtypes import URLArgument
 from arkindex_cli.auth import Profiles
-from arkindex_cli.commands.upload.alto.parser import AltoElement, RootAltoElement
+from arkindex_cli.client import ArkindexAPIClient
+from arkindex_cli.commands.upload.alto.parser import (
+    AltoElement,
+    AltoMetadata,
+    RootAltoElement,
+)
+from arkindex_cli.commands.upload.cache import Cache, save_cache
+from arkindex_cli.commands.upload.exceptions import UploadProcessingError
 
 REGEX_IMAGE_ID = re.compile(r"0+(\d+)")
+REGEX_METADATA_ERROR = re.compile(
+    r"Metadata ({.*}) already exist\(s\) on this element\."
+)
 
 logger = logging.getLogger(__name__)
 
 
-def add_alto_parser(subcommands):
-    gallica = subcommands.add_parser(
-        "gallica",
-        help="The images are on Gallica IIIF server.",
-    )
-    gallica.add_argument(
-        "--metadata-file",
-        help="CSV that contains the metadata related to the Gallica import.",
-        required=True,
-        type=Path,
-    )
-    gallica.add_argument(
+def add_alto_arguments(parser):
+    parser.add_argument(
         "--alto-namespace",
         help="Specify an Alto namespace to use.",
         required=False,
         type=str,
     )
-    gallica.add_argument(
+    parser.add_argument(
         "path",
         help="Path to a directory which contains ALTO XML documents. Defaults to the current working directory.",
         type=Path,
         default=Path.cwd(),
     )
-    gallica.add_argument(
-        "--mets",
-        help="Path to a METS file which contains ALTO XML documents order in its `fileSec::fileGrp` node.",
-        type=Path,
-        default=None,
-    )
-    gallica.add_argument(
+    parser.add_argument(
         "--iiif-base-url",
         help="Base URL for the IIIF images, which will be prepended to all source image file names.",
         type=URLArgument(allow_query=False),
         required=True,
     )
-    gallica.add_argument(
+    parser.add_argument(
         "--parent-id",
         help="UUID of a parent folder under which page elements will be created.",
         type=UUID,
         required=True,
     )
-    gallica.add_argument(
-        "--json-summary",
-        help="Build a JSON file creation report for each parsed ALTO file.",
+    parser.add_argument(
+        "--skip-metadata",
+        help="Skipping ALTO metadata publication, speeds up a lot the execution time",
         action="store_true",
     )
-    gallica.add_argument(
-        "--skip-metadatas",
-        help="Skipping Alto ID metadata publication speeds up a lot the execution time",
-        action="store_true",
-    )
-    gallica.add_argument(
+    parser.add_argument(
         "--worker-run-id",
-        help="Worker Run used to publish elements and transcriptions in bulk. This is required to use bulk endpoints and speed up publication.",
-        type=UUID,
-    )
-    types = gallica.add_mutually_exclusive_group(required=True)
-    types.add_argument(
-        "--create-types",
-        help="Create an element type in the Arkindex corpus for each element type in the ALTO files.",
-        action="store_true",
-    )
-    types.add_argument(
-        "--existing-types",
-        help='Specify correspondences between element types in the Arkindex corpus and in the ALTO files. Format: --existing-types="alto_type:arkindex_type alto_type_2:arkindex_type_2"',
-        type=str,
-    )
-    gallica.set_defaults(func=run_gallica)
-
-    alto = subcommands.add_parser(
-        "alto",
-        description="Upload ALTO XML documents to Arkindex.",
-        help="Upload ALTO XML documents to Arkindex.",
-    )
-    alto.add_argument(
-        "--alto-namespace",
-        help="Specify an Alto namespace to use.",
-        required=False,
-        type=str,
-    )
-    alto.add_argument(
-        "path",
-        help="Path to a directory which contains ALTO XML documents. Defaults to the current working directory.",
-        type=Path,
-        default=Path.cwd(),
-    )
-    alto.add_argument(
-        "--mets",
-        help="Path to a METS file which contains ALTO XML documents order in its `fileSec::fileGrp` node.",
-        type=Path,
-        default=None,
-    )
-    alto.add_argument(
-        "--iiif-base-url",
-        help="Base URL for the IIIF images, which will be prepended to all source image file names.",
-        type=URLArgument(allow_query=False),
-        required=True,
-    )
-    alto.add_argument(
-        "--parent-id",
-        help="UUID of a parent folder under which page elements will be created.",
+        help="Worker Run used to publish elements, transcriptions and metadata in bulk.",
         type=UUID,
         required=True,
     )
-    alto.add_argument(
-        "--skip-metadatas",
-        help="Skipping Alto ID metadata publication speeds up a lot the execution time",
-        action="store_true",
-    )
-    alto.add_argument(
-        "--worker-run-id",
-        help="Worker Run used to publish elements and transcriptions in bulk. This is required to use bulk endpoints and speed up publication.",
-        type=UUID,
-    )
-    alto.add_argument(
+    parser.add_argument(
         "--dpi-x",
         help="Horizontal resolution of the image, in dots per inch, to be used for ALTO files using coordinates in tenths of millimeters.\n"
         "Strictly positive integer. Ignored for files using coordinates in pixels.",
         type=int,
     )
-    alto.add_argument(
+    parser.add_argument(
         "--dpi-y",
         help="Vertical resolution of the image, in dots per inch, to be used for ALTO files using coordinates in tenths of millimeters.\n"
         "Strictly positive integer. Ignored for files using coordinates in pixels.",
         type=int,
     )
-    alto.add_argument(
-        "--json-summary",
-        help="Build a JSON file creation report for each parsed ALTO file.",
-        action="store_true",
-    )
-    types = alto.add_mutually_exclusive_group(required=True)
+    types = parser.add_mutually_exclusive_group(required=True)
     types.add_argument(
         "--create-types",
         help="Create an element type in the Arkindex corpus for each element type in the ALTO files.",
         action="store_true",
     )
     types.add_argument(
         "--existing-types",
         help='Specify correspondences between element types in the Arkindex corpus and in the ALTO files. Format: --existing-types="alto_type:arkindex_type alto_type_2:arkindex_type_2"',
         type=str,
     )
-    alto.set_defaults(func=run)
-
-
-def get_json_summary_elements(path: Path) -> dict | None:
-    if not path.exists():
-        return
 
-    return json.loads(path.read_text()).get("elements")
 
+def add_alto_parser(subcommands):
+    # Gallica parser
+    gallica = subcommands.add_parser(
+        "gallica",
+        help="The images are on Gallica IIIF server.",
+    )
+    gallica.add_argument(
+        "--metadata-file",
+        help="CSV that contains the metadata related to the Gallica import.",
+        required=True,
+        type=Path,
+    )
+    add_alto_arguments(gallica)
+    gallica.set_defaults(func=run_gallica)
 
-def bbox_area(polygon: List[List[int]]) -> int:
-    """
-    Get area of the polygon bounding box with (min_x, min_y, width, height)
-    """
-    # getting polygon coordinates
-    x_coords, y_coords = zip(*polygon)
-
-    # determining line box dimensions
-    min_x, min_y = min(x_coords), min(y_coords)
-    max_x, max_y = max(x_coords), max(y_coords)
-    width, height = max_x - min_x, max_y - min_y
-
-    return width * height
+    # Generic Alto parser
+    alto = subcommands.add_parser(
+        "alto",
+        description="Upload ALTO XML documents to Arkindex.",
+        help="Upload ALTO XML documents to Arkindex.",
+    )
+    add_alto_arguments(alto)
+    alto.set_defaults(func=run)
 
 
 def check_element_type(corpus: dict, type_slug: str) -> None:
     types = {type["slug"] for type in corpus["types"]}
     if type_slug not in types:
-        raise ValueError(f"Type {type_slug} not found.")
-    return True
+        logger.error(f"Type {type_slug} not found.")
+        raise UploadProcessingError
 
 
-def create_iiif_image(client: ArkindexClient, url: str) -> str:
+def create_iiif_image(client: ArkindexAPIClient, url: str) -> str:
+    logger.debug(f"Creating image from URL {url}…")
     try:
         image = client.request("CreateIIIFURL", body={"url": url})
         return image["id"]
     except ErrorResponse as e:
         # When the image already exists, its ID is returned in a HTTP 400
         if e.status_code == 400 and "id" in e.content:
             return e.content["id"]
-        raise
+        logger.error(
+            f"Failed to create image from target URL {url}: {e.status_code} - {e.content}"
+        )
+        raise UploadProcessingError
 
 
 _TYPES = {}
 
 
 def get_element_type(
-    client: ArkindexClient,
+    client: ArkindexAPIClient,
     corpus_id: UUID,
     node_name: str,
     types_dict: Optional[dict],
     create_types: bool = False,
 ):
     """
     Retrieve or create an alto node's corresponding Arkindex element type.
@@ -232,431 +164,399 @@
         _TYPES[corpus_id] = arkindex_corpus_types = [
             item["slug"]
             for item in client.request("RetrieveCorpus", id=corpus_id)["types"]
         ]
     else:
         arkindex_corpus_types = _TYPES[corpus_id]
 
+    if types_dict is None and not create_types:
+        logger.error(
+            f"No type can be found matching node {node_name} in corpus {corpus_id}. "
+            "Hint: either define types_dict or allow type creation."
+        )
+        raise UploadProcessingError
+
     if types_dict is not None:
         if node_name not in types_dict:
-            raise Exception(f"Alto element {node_name} not in given types dictionary.")
-        else:
-            return types_dict[node_name]
-    elif create_types:
-        if node_name not in arkindex_corpus_types:
-            logger.info(
-                f"Creating element type {node_name} in target corpus {corpus_id}…"
+            logger.error(f"Alto element {node_name} not in given types dictionary.")
+            raise UploadProcessingError
+        return types_dict[node_name]
+
+    if node_name in arkindex_corpus_types:
+        logger.debug(f"Element type {node_name} exists in target corpus {corpus_id}.")
+    else:
+        logger.debug(f"Creating element type {node_name} in target corpus {corpus_id}…")
+
+        try:
+            client.request(
+                "CreateElementType",
+                body={
+                    "slug": node_name,
+                    "display_name": node_name,
+                    "corpus": corpus_id,
+                },
             )
-            try:
-                client.request(
-                    "CreateElementType",
-                    body={
-                        "slug": node_name,
-                        "display_name": node_name,
-                        "corpus": corpus_id,
-                    },
-                )
-                _TYPES[corpus_id].append(node_name)
-            except ErrorResponse as e:
-                logger.error(
-                    f"Failed to create element type {node_name} in target corpus {corpus_id}."
-                )
-                raise Exception(e.content)
-        else:
-            logger.debug(
-                f"Element type {node_name} exists in target corpus {corpus_id}."
+            _TYPES[corpus_id].append(node_name)
+        except ErrorResponse as e:
+            logger.error(
+                f"Failed to create element type {node_name} in target corpus {corpus_id}: {e.status_code} - {e.content}."
             )
-        return node_name
-    raise ValueError(
-        f"No type can be found matching node {node_name} in corpus {corpus_id}. "
-        "Hint: either define types_dict or allow type creation."
-    )
+            raise UploadProcessingError
 
+    return node_name
 
-def get_child(
-    parent_id: str,
-    element_type: str,
-    polygon: List[List[int]],
-    children: List[dict],
-) -> Optional[dict]:
-    """
-    Find and return the first child that match the parent ID, element type and polygon.
-    Return None if no child was found.
-    """
-    return next(
-        filter(
-            lambda child: parent_id in child["parent_ids"]
-            and child["type"] == element_type
-            and child.get("zone", {}).get("polygon") == polygon,
-            children,
-        ),
-        None,
-    )
 
+def create_metadata(
+    client: ArkindexAPIClient,
+    element_id: str,
+    metadata_list: list[dict],
+    worker_run_id: UUID,
+    reraise: bool = False,
+) -> None:
+    if not metadata_list:
+        return
 
-def update_children(
-    client: ArkindexClient,
-    parent_id: str,
-    children: Dict[str, dict],
-):
-    """
-    Add the parent ID to its children to limit API calls instead of listing parents for each element.
-    `ListElementChildren` will list several children at once whereas `ListElementParent` will (often) only list one parent.
-    """
-    for child in client.paginate(
-        "ListElementChildren",
-        id=parent_id,
-        with_has_children=True,
-    ):
-        parents = children[child["id"]].get("parent_ids", [])
-        children[child["id"]]["parent_ids"] = parents + [parent_id]
+    try:
+        client.request(
+            "CreateMetaDataBulk",
+            id=element_id,
+            body={
+                "worker_run_id": str(worker_run_id),
+                "metadata_list": metadata_list,
+            },
+        )
+        logger.debug(f"Published {len(metadata_list)} metadata")
+    except ErrorResponse as e:
+        # Check if all metadata already exist
+        content = REGEX_METADATA_ERROR.fullmatch(
+            e.content.get("non_field_errors", [""])[0]
+        )
+        if (
+            reraise
+            or e.status_code != 400
+            or len(e.content.get("non_field_errors", [])) != 1
+            or not content
+        ):
+            logger.error(
+                f"Failed to create metadata on target element {element_id}: {e.status_code} - {e.content}."
+            )
+            raise UploadProcessingError
 
-        if child["has_children"]:
-            update_children(client=client, parent_id=child["id"], children=children)
+        # Ignore existing metadata
+        existing_metadatas = eval(content.group(1))
+        if len(metadata_list) == len(existing_metadatas):
+            return
+
+        # Try to publish missing metadata only
+        metadata_list = [
+            metadata
+            for metadata in metadata_list
+            if (metadata["name"], metadata["type"], metadata["value"])
+            not in existing_metadatas
+        ]
+        create_metadata(client, element_id, metadata_list, worker_run_id, reraise=True)
 
 
-def filter_children(
-    client: ArkindexClient,
-    parent_id: UUID,
-    image_id: str,
-    children_id: List[str],
-) -> List[dict]:
-    """
-    Filter existing children on this image and list their parents to:
-    - avoid element duplication
-    - keep existing paths
-    """
-    if not children_id:
-        return []
+def create_element_parent(
+    client: ArkindexAPIClient,
+    parent_id: str,
+    child_id: str,
+) -> None:
+    logger.debug(f"Linking element {child_id} to parent {parent_id}…")
+    try:
+        client.request(
+            "CreateElementParent",
+            parent=parent_id,
+            child=child_id,
+        )
+    except ErrorResponse as e:
+        # Ignore "already" errors
+        if e.status_code != 400 or all(
+            "is already a parent of" not in message
+            for message in e.content.get("parent", [])
+        ):
+            logger.error(
+                f"Failed to link target element {child_id} to parent {parent_id}: {e.status_code} - {e.content}."
+            )
+            raise UploadProcessingError
 
-    filtered_children = {
-        element["id"]: element
-        for element in filter(
-            lambda element: element["id"] in children_id,
-            client.paginate("ListImageElements", id=image_id),
-        )
-    }
-
-    for child in sorted(
-        filtered_children.values(),
-        key=lambda element: bbox_area(element.get("zone", []).get("polygon", [])),
-        reverse=True,
-    ):
-        # This child was already processed by its parent
-        if "parent_ids" in child:
-            continue
 
-        update_children(
-            client=client,
-            parent_id=child["id"],
-            children=filtered_children,
-        )
+def create_element_parents(
+    client: ArkindexAPIClient,
+    nodes: List[AltoElement],
+    parent_id: UUID,
+    cache: Cache,
+) -> None:
+    if not nodes:
+        return
 
-    for child in filtered_children.values():
-        # If the parent of this element is a folder, there may be several folders between this element and
-        # the parent passed as a parameter but we still want to avoid duplicating the element.
-        # So we mock the ID of the parent with the ID passed in parameter.
-        if "parent_ids" not in child:
-            child["parent_ids"] = [str(parent_id)]
+    # List children to link only the missing ones
+    try:
+        child_ids = set(
+            map(itemgetter("id"), client.paginate("ListElementChildren", id=parent_id))
+        )
+    except ErrorResponse as e:
+        logger.error(
+            f"Failed to retrieve children of target element {parent_id}: {e.status_code} - {e.content}"
+        )
+        raise UploadProcessingError
 
-    return filtered_children.values()
+    for node in nodes:
+        # Check if the child is already linked to the parent
+        arkindex_id = cache.get(node.id)
+        if arkindex_id in child_ids:
+            continue
+        create_element_parent(client, parent_id, child_id=arkindex_id)
 
 
+@save_cache
 def create_elements(
-    client: ArkindexClient,
+    client: ArkindexAPIClient,
     nodes: List[AltoElement],
     image_id: str,
     parent_id: UUID,
     corpus_id: str,
-    worker_run_id: Optional[UUID] = None,
+    worker_run_id: UUID,
+    cache: Cache,
     parent_node: Union[AltoElement, None] = None,
-    publish_metadatas: bool = True,
+    publish_metadata: bool = True,
     create_types: bool = True,
     types_dict: Optional[dict] = None,
-    children: Optional[List[dict]] = [],
-    # Mapping of Alto ID => existing Arkindex ID
-    elements: Optional[dict] = None,
-):
-    # Mapping of Alto ID => Arkindex ID
-    out = {}
+    metadata_list: Optional[list[AltoMetadata]] = [],
+) -> None:
+    # Update node's metadata before publishing them
+    if publish_metadata and metadata_list:
+        for node in nodes:
+            for alto_metadata in metadata_list:
+                node.metadata_list.extend(alto_metadata.get_metadata_list(node.content))
 
     # Cleanup nodes:
     # - no nodes without ID
     # - no nodes without polygon when parent has a polygon
     cleaned_nodes = [
         node for node in nodes if node.id and (parent_node is None or node.polygon)
     ]
     if not cleaned_nodes:
         # Do not create this node but iterate on their children
         for node in nodes:
             if not node.children:
                 continue
 
-            out.update(
-                create_elements(
-                    client,
-                    nodes=node.children,
-                    image_id=image_id,
-                    parent_id=parent_id,
-                    corpus_id=corpus_id,
-                    worker_run_id=worker_run_id,
-                    parent_node=node,
-                    publish_metadatas=publish_metadatas,
-                    types_dict=types_dict,
-                    create_types=create_types,
-                    children=children,
-                    elements=elements,
-                )
+            create_elements(
+                client,
+                nodes=node.children,
+                image_id=image_id,
+                parent_id=parent_id,
+                corpus_id=corpus_id,
+                worker_run_id=worker_run_id,
+                cache=cache,
+                parent_node=node,
+                publish_metadata=publish_metadata,
+                types_dict=types_dict,
+                create_types=create_types,
+                metadata_list=metadata_list,
             )
 
-        return out
+    def in_cache(node: AltoElement) -> bool:
+        return cache.get(node.id)
+
+    missing_nodes = list(filterfalse(in_cache, cleaned_nodes))
+    existing_nodes = list(filter(in_cache, cleaned_nodes))
+
+    # Try to link every existing nodes to the parent
+    create_element_parents(client, existing_nodes, parent_id, cache)
 
     # Create elements slowly one-by-one when
     # - parent is unknown, so probably without any polygon nor image
     # - parent is known but has not polygon
     # - all nodes without any zones
-    # - no worker run ID is set
-    distinctive_elts = [node for node in cleaned_nodes if not node.polygon]
-    if parent_node is None or not parent_node.polygon or not worker_run_id:
-        distinctive_elts += cleaned_nodes
+    distinctive_elts = (
+        missing_nodes
+        if parent_node is None or not parent_node.polygon
+        else [node for node in missing_nodes if not node.polygon]
+    )
 
     for node in distinctive_elts:
         body = {
             "corpus": corpus_id,
             "parent": str(parent_id),
             "type": get_element_type(
                 client,
                 corpus_id,
                 node.node_name,
                 types_dict=types_dict,
                 create_types=create_types,
             ),
             "name": node.name,
+            "worker_run_id": str(worker_run_id),
         }
 
         if image_id and node.polygon:
             body["polygon"] = node.polygon
             body["image"] = image_id
 
-        # Do no duplicate element
-        element_id = None
-        if elements is not None:
-            assert (
-                node.id in elements
-            ), f"Element for node {node.name} ({node.id}) not found in JSON summary"
-            element_id = elements[node.id]
-
-        # Link existing element to its parent
-        if element_id:
-            client.request(
-                "CreateElementParent",
-                parent=body["parent"],
-                child=element_id,
-            )
-
-        if not element_id:
-            element = get_child(
-                parent_id=body["parent"],
-                element_type=body["type"],
-                polygon=body.get("polygon"),
-                children=children,
-            )
-            element_id = element["id"] if element else None
-
-        # Create missing element
-        if not element_id:
+        try:
             element_id = client.request(
                 "CreateElement",
                 body=body,
             )["id"]
-
-        # Store the arkindex ID of the newly created element
-        out[node.id] = element_id
+        except ErrorResponse as e:
+            logger.error(
+                f"Failed to create element on target parent {body['parent']}: {e.status_code} - {e.content}."
+            )
+            raise UploadProcessingError
 
         # Build transcription when available
         if node.text:
-            client.request(
-                "CreateTranscription",
-                id=element_id,
-                body={"text": node.text},
-            )
+            try:
+                client.request(
+                    "CreateTranscription",
+                    id=element_id,
+                    body={
+                        "text": node.text,
+                        "confidence": node.confidence,
+                        "worker_run_id": str(worker_run_id),
+                    },
+                )
+            except ErrorResponse as e:
+                logger.error(
+                    f"Failed to create transcription on target element {element_id}: {e.status_code} - {e.content}."
+                )
+                raise UploadProcessingError
+
+        # Store the arkindex ID of the newly created element
+        cache.set(node.id, element_id)
 
     if distinctive_elts:
-        logger.info(f"Published {len(distinctive_elts)} elements distinctly")
+        logger.debug(f"Published {len(distinctive_elts)} elements distinctly")
 
     # Split remaining nodes with/without transcriptions
     # to take advantage of CreateElements & CreateElementTranscriptions
-    with_transcriptions = [
-        node for node in cleaned_nodes if node.text and node.id not in out
-    ]
-    without_transcriptions = [
-        node for node in cleaned_nodes if not node.text and node.id not in out
-    ]
+    missing_nodes = list(
+        filter(lambda node: node not in distinctive_elts, missing_nodes)
+    )
+    with_transcriptions = [node for node in missing_nodes if node.text]
+    without_transcriptions = [node for node in missing_nodes if not node.text]
 
     if without_transcriptions:
         try:
-            elements, to_create = [], []
-            for node in without_transcriptions:
-                element_type = get_element_type(
-                    client,
-                    corpus_id,
-                    node.node_name,
-                    types_dict=types_dict,
-                    create_types=create_types,
-                )
-
-                # Do no duplicate elements
-                if existing_element := get_child(
-                    parent_id=str(parent_id),
-                    element_type=element_type,
-                    polygon=node.polygon,
-                    children=children,
-                ):
-                    elements.append(existing_element)
-                else:
-                    to_create.append(
+            elements = client.request(
+                "CreateElements",
+                id=parent_id,
+                body={
+                    "worker_run_id": str(worker_run_id),
+                    "elements": [
                         {
                             "name": node.name,
-                            "type": element_type,
+                            "type": get_element_type(
+                                client,
+                                corpus_id,
+                                node.node_name,
+                                types_dict=types_dict,
+                                create_types=create_types,
+                            ),
                             "polygon": node.polygon,
                         }
-                    )
-
-            # Create missing elements
-            if to_create:
-                elements.extend(
-                    client.request(
-                        "CreateElements",
-                        id=parent_id,
-                        body={
-                            "worker_run_id": str(worker_run_id),
-                            "elements": to_create,
-                        },
-                    )
-                )
+                        for node in without_transcriptions
+                    ],
+                },
+            )
         except ErrorResponse as e:
-            logger.error(f"Failed to create elements: {e.content}")
-            raise
+            logger.error(
+                f"Failed to create elements on target parent {parent_id}: {e.status_code} - {e.content}"
+            )
+            raise UploadProcessingError
 
         # Store the arkindex ID of the newly created element
         node_ids = (node.id for node in without_transcriptions)
         arkindex_ids = (elt["id"] for elt in elements)
-        out.update(dict(zip(node_ids, arkindex_ids)))
+        for node_id, arkindex_id in zip(node_ids, arkindex_ids):
+            cache.set(node_id, arkindex_id)
 
-        logger.info(f"Published {len(without_transcriptions)} elements")
+        logger.debug(f"Published {len(without_transcriptions)} elements")
 
     if with_transcriptions:
 
         # To create elements and transcriptions, we first
         # need to group nodes by their types
         groups = itertools.groupby(
             sorted(with_transcriptions, key=lambda n: n.node_name),
             lambda n: n.node_name,
         )
 
         for node_name, node_group in groups:
             node_group = list(node_group)  # needed because we access it several times
             try:
-                element_type = get_element_type(
-                    client,
-                    corpus_id,
-                    node_name,
-                    types_dict=types_dict,
-                    create_types=create_types,
-                )
-
-                elements, to_create = [], []
-                for node in node_group:
-                    # Do no duplicate transcriptions
-                    if existing_element := get_child(
-                        parent_id=str(parent_id),
-                        element_type=element_type,
-                        polygon=node.polygon,
-                        children=children,
-                    ):
-                        existing_element["element_id"] = existing_element["id"]
-                        elements.append(existing_element)
-                    else:
-                        to_create.append(
+                elements = client.request(
+                    "CreateElementTranscriptions",
+                    id=parent_id,
+                    body={
+                        "element_type": get_element_type(
+                            client,
+                            corpus_id,
+                            node_name,
+                            types_dict=types_dict,
+                            create_types=create_types,
+                        ),
+                        "worker_run_id": str(worker_run_id),
+                        "return_elements": True,
+                        "transcriptions": [
                             {
                                 "polygon": node.polygon,
                                 "text": node.text,
-                                "confidence": 1.0,
+                                "confidence": node.confidence,
                             }
-                        )
-
-                # Create missing transcriptions
-                if to_create:
-                    elements.extend(
-                        client.request(
-                            "CreateElementTranscriptions",
-                            id=parent_id,
-                            body={
-                                "element_type": element_type,
-                                "worker_run_id": str(worker_run_id),
-                                "return_elements": True,
-                                "transcriptions": to_create,
-                            },
-                        )
-                    )
+                            for node in node_group
+                        ],
+                    },
+                )
             except ErrorResponse as e:
-                logger.error(f"Failed to create elements: {e.content}")
-                raise
+                logger.error(
+                    f"Failed to create elements with transcriptions on target element {parent_id}: {e.status_code} - {e.content}"
+                )
+                raise UploadProcessingError
 
             # Store the arkindex ID of the newly created element
             node_ids = (node.id for node in node_group)
             arkindex_ids = (elt["element_id"] for elt in elements)
-            out.update(dict(zip(node_ids, arkindex_ids)))
+            for node_id, arkindex_id in zip(node_ids, arkindex_ids):
+                cache.set(node_id, arkindex_id)
 
-        logger.info(
+        logger.debug(
             f"Published {len(with_transcriptions)} elements with transcriptions"
         )
 
-    # Publish metadatas slowly, there is no alternative here
-    if publish_metadatas:
+    # Publish metadata
+    if publish_metadata:
         for node in cleaned_nodes:
-            try:
-                client.request(
-                    "CreateMetaData",
-                    id=out[node.id],
-                    body={"name": "Alto ID", "value": node.id, "type": "reference"},
-                )
-            except ErrorResponse as e:
-                # This metadata already exists
-                if e.status_code == 400 and e.content.get("id"):
-                    continue
-                raise e
-
-        logger.info(f"Published {len(cleaned_nodes)} metadatas")
+            create_metadata(
+                client, cache.get(node.id), node.metadata_list, worker_run_id
+            )
 
     # All nodes are created at this point
     # we can directly iterate on their children
     for node in cleaned_nodes:
         if not node.children:
             continue
 
-        out.update(
-            create_elements(
-                client,
-                nodes=node.children,
-                image_id=image_id,
-                parent_id=out[node.id],
-                corpus_id=corpus_id,
-                worker_run_id=worker_run_id,
-                parent_node=node,
-                publish_metadatas=publish_metadatas,
-                types_dict=types_dict,
-                create_types=create_types,
-                children=children,
-                elements=elements,
-            )
+        create_elements(
+            client,
+            nodes=node.children,
+            image_id=image_id,
+            parent_id=cache.get(node.id),
+            corpus_id=corpus_id,
+            worker_run_id=worker_run_id,
+            cache=cache,
+            parent_node=node,
+            publish_metadata=publish_metadata,
+            types_dict=types_dict,
+            create_types=create_types,
+            metadata_list=metadata_list,
         )
 
-    return out
-
 
 def format_url(path: Path, iiif_base_url: str, folders_ark_id_dict: dict = None):
     """
     This function is used to create the url to get the image from the Gallica IIIF server
     """
     # The path.name looks like 18840615_1-0003.xml with the folder id being the 18840615 which we use to
     # find the ark_id in order to get the folder from the Gallica server in this case it is ark:/12148/bpt6k7155522
@@ -674,53 +574,77 @@
     ark_id = folders_ark_id_dict[folder_id]
     return f"{iiif_base_url}{ark_id}/f{parse_image_idx(image_id)}"
 
 
 def parse_image_idx(image_id):
     # Remove leading 0s
     image_idx = REGEX_IMAGE_ID.search(image_id)
-    assert image_idx, f"Could not parse the image IDX from `{image_id}`"
+    if not image_idx:
+        logger.error(f"Could not parse the image IDX from `{image_id}`")
+        raise UploadProcessingError
     return image_idx.group(1)
 
 
 def upload_alto_file(
     path: Path,
-    client: ArkindexClient,
+    client: ArkindexAPIClient,
     iiif_base_url: str,
     corpus: dict,
     parent_id: UUID,
     types_dict: Optional[dict],
     create_types: bool,
+    worker_run_id: UUID,
     dpi_x: Optional[int] = None,
     dpi_y: Optional[int] = None,
     gallica: bool = False,
     folders_ark_id_dict: dict = None,
     alto_namespace: str = None,
-    json_summary: bool = False,
-    worker_run_id: Optional[UUID] = None,
-    skip_metadatas: bool = False,
-    children_id: Optional[List[str]] = [],
+    skip_metadata: bool = False,
 ) -> None:
+    logger.info(f"Publishing ALTO file @ {path}…")
+
+    # Setup cache next to alto file
+    cache = Cache(path.with_suffix(".json"))
+
     with open(path) as file:
         # This ensures that comments in the XML files do not cause the
         # "no Alto namespace found" exception.
         parser = ET.XMLParser(remove_comments=True)
         tree = objectify.parse(file, parser=parser)
         root = RootAltoElement(
             tree.getroot(), alto_namespace=alto_namespace, dpi_x=dpi_x, dpi_y=dpi_y
         )
 
     # Skip empty files immediately
     if not len(root.content):
         logger.warning(f"No content found in file {path}")
         return
 
-    # Load existing JSON summary if exists
-    json_summary_path = path.with_suffix(".json")
-    json_summary_elements = get_json_summary_elements(json_summary_path)
+    # Parse styles and tags
+    metadata_list = [
+        AltoMetadata(
+            target=target,
+            metadata_list={
+                node.attrib["ID"]: [
+                    {
+                        "name": key.capitalize(),
+                        "value": value,
+                        "type": "numeric" if value.isdigit() else "text",
+                    }
+                    for key, value in node.attrib.items()
+                    if key != "ID"
+                ]
+                for node in root.content.findall(
+                    f".//{{*}}{tag}/*", namespaces=root.namespaces
+                )
+                if node.attrib.get("ID")
+            },
+        )
+        for tag, target in [("Styles", "STYLEREFS"), ("Tags", "TAGREFS")]
+    ]
 
     page_nodes = root.content.findall(".//{*}Page", namespaces=root.namespaces)
     if len(page_nodes) == 1:
         # We use + here and not urljoin or path.join to create image URLs
         # because the base URL could contain a portion of the identifier:
         # 'http://server/iiif/root%2Fdirectory'
         # urljoin or path.join would erase that identifier prefix.
@@ -732,44 +656,36 @@
                 # Use the file identifier by default
                 root.file_identifier
                 # or keep existing path if we upload file of a subfolder
                 or quote(str(path.parent / root.filename), safe="")
             )
             image_id = create_iiif_image(client, iiif_base_url + iiif_path)
 
-        children = filter_children(
-            client=client,
-            parent_id=parent_id,
-            image_id=image_id,
-            children_id=children_id,
-        )
-
         page_node = AltoElement(
             page_nodes[0],
             alto_namespace=alto_namespace,
             unit=root.unit,
             dpi_x=dpi_x,
             dpi_y=dpi_y,
         )
         page_node.parse_children()
-        elements = create_elements(
+        create_elements(
             client=client,
             nodes=[page_node],
             image_id=image_id,
             parent_id=parent_id,
             corpus_id=corpus["id"],
             worker_run_id=worker_run_id,
-            publish_metadatas=not skip_metadatas,
+            cache=cache,
+            publish_metadata=not skip_metadata,
             create_types=create_types,
             types_dict=types_dict,
-            children=children,
-            elements=json_summary_elements,
+            metadata_list=metadata_list,
         )
     elif len(page_nodes) > 1:
-        elements = {}
         for page_node in page_nodes:
             page_node = AltoElement(
                 page_node,
                 alto_namespace=alto_namespace,
                 unit=root.unit,
                 dpi_x=dpi_x,
                 dpi_y=dpi_y,
@@ -779,111 +695,67 @@
                     "Attribute PHYSICAL_IMG_NR was not set for this Page node. Skipping…"
                 )
                 return
             image_id = create_iiif_image(
                 client, iiif_base_url + page_node.page_image_id
             )
 
-            children = filter_children(
+            create_elements(
                 client=client,
-                parent_id=parent_id,
+                nodes=[page_node],
                 image_id=image_id,
-                children_id=children_id,
-            )
-
-            elements.update(
-                create_elements(
-                    client=client,
-                    nodes=[page_node],
-                    image_id=image_id,
-                    parent_id=parent_id,
-                    corpus_id=corpus["id"],
-                    worker_run_id=worker_run_id,
-                    publish_metadatas=not skip_metadatas,
-                    create_types=create_types,
-                    types_dict=types_dict,
-                    children=children,
-                    elements=json_summary_elements,
-                )
+                parent_id=parent_id,
+                corpus_id=corpus["id"],
+                worker_run_id=worker_run_id,
+                cache=cache,
+                publish_metadata=not skip_metadata,
+                create_types=create_types,
+                types_dict=types_dict,
+                metadata_list=metadata_list,
             )
     else:
         logger.warning(f"No Page node found in file {root.filename}. Skipping…")
         return
 
-    if json_summary:
-        json_summary_path.write_text(
-            json.dumps(
-                {
-                    "alto_file": str(path),
-                    "arkindex_api_url": client.document.url,
-                    "elements": elements,
-                },
-                sort_keys=True,
-                indent=4,
-            )
-        )
-
 
 def run_gallica(
-    path: Path,
-    iiif_base_url: str,
-    parent_id: UUID,
-    mets: Optional[Path] = None,
-    create_types: bool = False,
-    existing_types: Optional[str] = None,
     metadata_file: Optional[Path] = None,
-    json_summary: bool = False,
-    profile_slug: Optional[str] = None,
-    gitlab_secure_file: Optional[Path] = None,
-    alto_namespace: Optional[str] = None,
-    worker_run_id: Optional[UUID] = None,
-    skip_metadatas: bool = False,
+    *args,
+    **kwargs,
 ):
     # If this is a Gallica import, load the metadata CSV file
     folders_ark_id_dict = dict()
     with open(metadata_file, "r") as file:
         reader = csv.reader(file)
         # Create a dictionary with the folder name as the id and the Gallica Ark ID as the value
         folders_ark_id_dict = {row[0]: row[1] for row in reader}
 
     run(
-        path=path,
-        iiif_base_url=iiif_base_url,
-        parent_id=parent_id,
-        mets=mets,
-        create_types=create_types,
-        existing_types=existing_types,
         folders_ark_id_dict=folders_ark_id_dict,
         gallica=True,
-        profile_slug=profile_slug,
-        gitlab_secure_file=gitlab_secure_file,
-        alto_namespace=alto_namespace,
-        json_summary=json_summary,
-        worker_run_id=worker_run_id,
-        skip_metadatas=skip_metadatas,
+        *args,
+        **kwargs,
     )
 
 
 def run(
     path: Path,
     iiif_base_url: str,
     parent_id: UUID,
-    mets: Optional[Path] = None,
+    worker_run_id: UUID,
     dpi_x: Optional[int] = None,
     dpi_y: Optional[int] = None,
     create_types: bool = False,
     existing_types: Optional[str] = None,
     folders_ark_id_dict: Optional[dict] = None,
     profile_slug: Optional[str] = None,
     gitlab_secure_file: Optional[Path] = None,
     gallica: bool = False,
     alto_namespace: Optional[str] = None,
-    json_summary: bool = False,
-    worker_run_id: Optional[UUID] = None,
-    skip_metadatas: bool = False,
+    skip_metadata: bool = False,
 ) -> int:
     if (dpi_x is None) ^ (dpi_y is None):
         logger.error("--dpi-x and --dpi-y must be either both set or both unset.")
         return errno.EINVAL
 
     if dpi_x is not None and dpi_x <= 0:
         logger.error("--dpi-x must be a strictly positive integer.")
@@ -898,30 +770,14 @@
         return errno.ENOTDIR
 
     file_paths = list(path.rglob("*.xml"))
     if not file_paths:
         logger.error(f"No XML files found in {path}.")
         return errno.ENOENT
 
-    if mets:
-        # Circular dependencies
-        from arkindex_cli.commands.upload.mets.parser import RootMetsElement
-
-        if not mets.is_file():
-            logger.error(f"Cannot find METS at {mets}")
-            return errno.ENOENT
-
-        try:
-            root = RootMetsElement(mets, iiif_base_url, dpi_x=dpi_x, dpi_y=dpi_y)
-        except FileNotFoundError as e:
-            logger.error(f"ALTO file listed in the METS file not found: {e}")
-            return errno.ENOENT
-
-        file_paths = root.files_order
-
     with Progress(transient=True) as progress:
         progress.add_task(start=False, description="Loading API client")
         client = Profiles(gitlab_secure_file).get_api_client_or_exit(profile_slug)
 
     with Progress(transient=True) as progress:
         progress.add_task(start=False, description="Fetching parent element")
         try:
@@ -939,55 +795,30 @@
             corpus = client.request("RetrieveCorpus", id=corpus_id)
         except ErrorResponse as e:
             logger.error(
                 f"Could not retrieve corpus {corpus_id}: HTTP {e.status_code} - {e.content}"
             )
             return errno.EREMOTEIO
 
-    if not worker_run_id:
-        logger.info(
-            "Upload METS in slow mode (Set --worker-run-id to use bulk endpoints)"
-        )
-
     types_dict = None
     if existing_types:
         split_str = existing_types.split(" ")
         types_dict = {}
         for item in split_str:
             split_item = item.split(":")
             types_dict[str(split_item[0]).lower()] = str(split_item[1]).lower()
-        for key, arkindex_type in types_dict.items():
+        for arkindex_type in types_dict.values():
             try:
                 check_element_type(corpus, arkindex_type)
             except ValueError as e:
                 logger.error(str(e))
                 return errno.EINVAL
 
     failed = 0
 
-    try:
-        # List existing children to:
-        # - avoid element duplication
-        # - keep existing paths
-        children_id = list(
-            map(
-                itemgetter("id"),
-                client.paginate(
-                    "ListElementChildren",
-                    id=parent_id,
-                    recursive=True,
-                ),
-            )
-        )
-    except ErrorResponse as e:
-        logger.error(
-            f"Could not list children of parent element {parent_id}: HTTP {e.status_code} - {e.content}"
-        )
-        return 1
-
     for file_path in track(file_paths, description="Uploading"):
         try:
             upload_alto_file(
                 gallica=gallica,
                 folders_ark_id_dict=folders_ark_id_dict,
                 path=file_path,
                 client=client,
@@ -995,22 +826,15 @@
                 corpus=corpus,
                 parent_id=parent_id,
                 types_dict=types_dict,
                 create_types=create_types,
                 dpi_x=dpi_x,
                 dpi_y=dpi_y,
                 alto_namespace=alto_namespace,
-                json_summary=json_summary,
                 worker_run_id=worker_run_id,
-                skip_metadatas=skip_metadatas,
-                children_id=children_id,
+                skip_metadata=skip_metadata,
             )
-        except ErrorResponse as e:
-            logger.error(
-                f"Upload failed for file {file_path}: HTTP {e.status_code} - {e.content}"
-            )
-            failed += 1
-        except Exception as e:
-            logger.error(f"Upload failed for file {file_path}: {e}")
+        except UploadProcessingError:
+            logger.error(f"Failed to publish ALTO file @ {file_path}")
             failed += 1
     # Return a non-zero error code when all files have failed
     return failed >= len(file_paths)
```

### Comparing `arkindex-cli-0.4.1/arkindex_cli/commands/upload/iiif.py` & `arkindex-cli-0.4.2/arkindex_cli/commands/upload/iiif.py`

 * *Files identical despite different names*

### Comparing `arkindex-cli-0.4.1/arkindex_cli/commands/upload/mets/__init__.py` & `arkindex-cli-0.4.2/arkindex_cli/commands/upload/mets/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,19 +7,17 @@
 from uuid import UUID
 
 from apistar.exceptions import ErrorResponse
 from rich.progress import Progress
 
 from arkindex_cli.auth import Profiles
 from arkindex_cli.commands.upload.alto import get_element_type
-from arkindex_cli.commands.upload.mets.cache import Cache
-from arkindex_cli.commands.upload.mets.parser import (
-    MetsProcessingError,
-    RootMetsElement,
-)
+from arkindex_cli.commands.upload.cache import Cache
+from arkindex_cli.commands.upload.exceptions import UploadProcessingError
+from arkindex_cli.commands.upload.mets.parser import RootMetsElement
 
 logger = logging.getLogger(__name__)
 
 
 def trailing_slash_url(value):
     """Check an URL ends with a /"""
     assert isinstance(value, str)
@@ -81,52 +79,56 @@
     mets.add_argument(
         "--dpi-y",
         help="Vertical resolution of the image, in dots per inch, to be used for ALTO files using coordinates in tenths of millimeters.\n"
         "Strictly positive integer. Ignored for files using coordinates in pixels.",
         type=int,
     )
     mets.add_argument(
-        "--skip-metadatas",
-        help="Skipping Alto ID metadata publication speeds up a lot the execution time",
+        "--skip-metadata",
+        help="Skipping METS metadata publication, speeds up a lot the execution time",
         action="store_true",
     )
     mets.add_argument(
         "--worker-run-id",
-        help="Worker Run used to publish elements and transcriptions in bulk. This is required to use bulk endpoints and speed up publication.",
+        help="Worker Run used to publish elements, transcriptions and metadata in bulk.",
         type=UUID,
+        required=True,
+    )
+    mets.add_argument(
+        "--alto",
+        action="store_true",
+        help="Whether or not to publish ALTO files as well",
     )
     mets.set_defaults(func=run)
 
 
 def run(
     path: Path,
     corpus_id: UUID,
     element_id: UUID,
     iiif_base_url: str,
+    worker_run_id: UUID,
     iiif_prefix: Optional[str] = None,
     dpi_x: Optional[int] = None,
     dpi_y: Optional[int] = None,
-    worker_run_id: Optional[UUID] = None,
-    skip_metadatas: bool = False,
+    skip_metadata: bool = False,
+    alto: bool = False,
     profile_slug: Optional[str] = None,
     gitlab_secure_file: Optional[Path] = None,
 ):
     with Progress(transient=True) as progress:
         progress.add_task(start=False, description="Loading API client")
         client = Profiles(gitlab_secure_file).get_api_client_or_exit(profile_slug)
 
     # Parse TOC
-    assert path.exists(), f"Cannot find METS at {path}"
+    if not path.exists():
+        logger.error(f"Cannot find METS at {path}")
+        return errno.ENOENT
     root = RootMetsElement(path, iiif_base_url, iiif_prefix, dpi_x, dpi_y)
 
-    if not worker_run_id:
-        logger.info(
-            "Upload METS in slow mode (Set --worker-run-id to use bulk endpoints)"
-        )
-
     # Check the existence of the top element
     with Progress(transient=True) as progress:
         progress.add_task(start=False, description="Fetching parent element")
         try:
             client.request("RetrieveElement", id=element_id)
         except ErrorResponse as e:
             logger.error(
@@ -136,26 +138,37 @@
 
     # Check that every type used by the tree is available on the corpus
     for type_slug in root.list_required_types():
         get_element_type(
             client, corpus_id, type_slug, types_dict=None, create_types=True
         )
 
+    # Publish ALTO files
+    if alto:
+        try:
+            root.publish_alto(
+                arkindex_client=client,
+                parent_id=element_id,
+                corpus_id=corpus_id,
+                publish_metadata=not skip_metadata,
+                worker_run_id=worker_run_id,
+            )
+        except UploadProcessingError:
+            logger.error(f"Failed to publish ALTO file @ {path}")
+            return
+
     # Setup cache next to mets file
-    Cache(path.parent / f"{path.stem}_cache.json")
+    cache = Cache(path.with_suffix(".json"))
 
     # Publish all elements recursively starting from root
+    logger.info(f"Publishing METS file @ {path}…")
     try:
         root.publish(
+            cache=cache,
             arkindex_client=client,
             parent_id=element_id,
             corpus_id=corpus_id,
-            publish_metadatas=not skip_metadatas,
+            publish_metadata=not skip_metadata,
             worker_run_id=worker_run_id,
         )
-    except MetsProcessingError:
+    except UploadProcessingError:
         logger.error(f"Failed to publish METS file @ {path}")
-    except KeyboardInterrupt:
-        pass
-
-    # Make sure to save cache on keyboard interrupt
-    Cache._instance = None
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `arkindex-cli-0.4.1/arkindex_cli/commands/upload/mets/parser.py` & `arkindex-cli-0.4.2/arkindex_cli/commands/upload/mets/parser.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,89 +1,119 @@
 # -*- coding: utf-8 -*-
 import logging
 import urllib.parse
+from operator import itemgetter
 from pathlib import Path
+from uuid import UUID
 
 from apistar.exceptions import ErrorResponse
 from lxml import etree as ET
 from lxml import objectify
 
+from arkindex_cli.client import ArkindexAPIClient
 from arkindex_cli.commands.upload.alto import (
+    create_element_parent,
     create_elements,
     create_iiif_image,
-    get_json_summary_elements,
+    create_metadata,
+    upload_alto_file,
 )
-from arkindex_cli.commands.upload.alto.parser import AltoElement, RootAltoElement
-from arkindex_cli.commands.upload.mets.cache import Cache
+from arkindex_cli.commands.upload.alto.parser import (
+    AltoElement,
+    AltoMetadata,
+    RootAltoElement,
+)
+from arkindex_cli.commands.upload.cache import Cache, save_cache
+from arkindex_cli.commands.upload.exceptions import UploadProcessingError
+from dateutil.parser import parse
 
 logger = logging.getLogger(__name__)
 
 # Only need METS base support here
 METS_NS = {"mets": "http://www.loc.gov/METS/", "xlink": "http://www.w3.org/1999/xlink"}
 
 IMAGE_SUFFIXES = (".jpeg", ".jpg", ".png", ".tiff", ".tif")
 ALTO_SUFFIXES = (".xml",)
 
 
-class MetsProcessingError(Exception):
-    """
-    Raised when there has been an error in the Mets upload processing
-    """
+def get_metadata_type(value: str) -> str:
+    def is_valid_number(value: str) -> bool:
+        try:
+            float(value)
+        except Exception:
+            return False
+        return True
+
+    def is_valid_date(value: str) -> bool:
+        try:
+            parse(value)
+        except Exception:
+            return False
+        return True
+
+    if value.startswith("http"):
+        return "url"
+
+    if is_valid_number(value):
+        return "numeric"
+
+    if is_valid_date(value):
+        return "date"
+
+    return "text"
 
 
 class MetsImage(object):
     """
     A remote IIIF image
     """
 
-    def __init__(self, image_relative_path, iiif_base_url, iiif_prefix):
+    def __init__(self, image_relative_path: str, iiif_base_url: str, iiif_prefix: str):
         # Build IIIF url for the image
         # knowing only its relative path to the folder with METS file
         image_path = urllib.parse.urljoin(iiif_prefix, image_relative_path)
         self.url = iiif_base_url + urllib.parse.quote_plus(image_path)
 
         self.cache_key = f"image/{image_relative_path}"
 
-    def publish(self, arkindex_client):
-
+    def publish(self, cache: Cache, arkindex_client: ArkindexAPIClient):
         # Check cache
-        self.arkindex_id = Cache.get(self.cache_key)
+        self.arkindex_id = cache.get(self.cache_key)
         if self.arkindex_id is not None:
             return
 
         # Declare image on Arkindex
         self.arkindex_id = create_iiif_image(arkindex_client, self.url)
-        logger.info(f"Published image {self.arkindex_id}")
+        logger.debug(f"Published image {self.arkindex_id}")
 
         # Store in cache
-        Cache.set(self.cache_key, self.arkindex_id)
+        cache.set(self.cache_key, self.arkindex_id)
 
 
 class MetsAlto(object):
     """
     A local ALTO XML file
     """
 
-    def __init__(self, path, dpi_x=None, dpi_y=None):
+    def __init__(self, path: Path, dpi_x: int | None = None, dpi_y: int | None = None):
         self.path = path
 
         with open(path) as file:
             # This ensures that comments in the XML files do not cause the
             # "no Alto namespace found" exception.
             parser = ET.XMLParser(remove_comments=True)
             tree = objectify.parse(file, parser=parser)
             self.root = RootAltoElement(tree.getroot(), dpi_x=dpi_x, dpi_y=dpi_y)
 
     def __eq__(self, other):
         # Used in unit tests to compare 2 instances
         return self.path.absolute() == other.path.absolute()
 
-    def parse(self, target_id):
+    def parse(self, target_id: str):
         self.target_id = target_id
-        self.cache_key = f"alto/{self.path}/{self.target_id}"
 
         # Find element matching provided id
         xpath = f".//*[@ID='{target_id}']"
         xml_target = self.root.content.find(xpath)
         if xml_target is None:
             return
 
@@ -101,87 +131,78 @@
             dpi_x=self.root.dpi_x,
             dpi_y=self.root.dpi_y,
         )
         self.element.parse_children()
 
     def publish(
         self,
-        arkindex_client,
-        corpus_id,
-        parent_id=None,
-        image=None,
-        worker_run_id=None,
-        publish_metadatas=True,
+        arkindex_client: ArkindexAPIClient,
+        corpus_id: UUID,
+        worker_run_id: UUID,
+        parent_id: UUID | None = None,
+        image: MetsImage | None = None,
+        publish_metadata: bool = True,
     ):
         # Check cache
-        arkindex_id = Cache.get(self.cache_key)
+        cache = Cache(self.path.with_suffix(".json"))
+        arkindex_id = cache.get(self.target_id)
         if arkindex_id is not None:
-
             # Create parent link
             if parent_id is not None:
-                try:
-                    arkindex_client.request(
-                        "CreateElementParent",
-                        child=arkindex_id,
-                        parent=parent_id,
-                    )
-                except ErrorResponse as e:
-                    # link already exists when 400 is received
-                    if e.status_code != 400:
-                        raise Exception(
-                            f"Failed to create placeholder element: {e.content}"
-                        )
-
-            return arkindex_id
-
-        # Load existing JSON summary if exists
-        json_summary_elements = get_json_summary_elements(
-            self.path.with_suffix(".json")
-        )
+                create_element_parent(
+                    client=arkindex_client, parent_id=parent_id, child_id=arkindex_id
+                )
+            return
 
         image_id = image.arkindex_id if image is not None else None
-        try:
-            elements = create_elements(
-                client=arkindex_client,
-                nodes=[
-                    self.element,
-                ],
-                image_id=image_id,
-                corpus_id=str(corpus_id),
-                parent_id=parent_id,
-                worker_run_id=worker_run_id,
-                publish_metadatas=publish_metadatas,
-                elements=json_summary_elements,
-            )
-
-        except ErrorResponse as e:
-            logger.info(f"Failed to create elements: {e.content}")
-            raise
-
-        # ALTO processor builds Arkindex elements
-        # and returns a mapping of ALTO ID => Arkindex ID
-        assert (
-            self.target_id in elements
-        ), f"Missing ALTO element {self.target_id} in arkindex elements"
-
-        # Store in cache all elements
-        for key, value in elements.items():
-            Cache.set(f"alto/{self.path}/{key}", value)
-
-        return elements[self.target_id]
+        create_elements(
+            client=arkindex_client,
+            nodes=[
+                self.element,
+            ],
+            image_id=image_id,
+            corpus_id=str(corpus_id),
+            parent_id=parent_id,
+            worker_run_id=worker_run_id,
+            cache=cache,
+            publish_metadata=publish_metadata,
+        )
 
 
 class MetsElement:
-    def __init__(self, node, parent=None) -> None:
+    def __init__(
+        self, node: ET._Element | None, parent: "MetsElement | None" = None
+    ) -> None:
         self.node = node
         self.parent = parent
 
         # Populated during publication on Arkindex
         self.arkindex_id = None
 
+        # List of the metadata associated with the element
+        self.metadata_list = [
+            {"name": "METS ID", "value": self.id, "type": "reference"}
+        ]
+        if self.node is not None:
+            self.metadata_list.extend(
+                [
+                    {
+                        "name": key,
+                        "value": value.strip(),
+                        "type": get_metadata_type(value.strip()),
+                    }
+                    for key, value in self.node.attrib.items()
+                    if (
+                        key
+                        and value.strip()
+                        and key not in ["TYPE", "ID", "LABEL", "DMDID"]
+                    )
+                ]
+            )
+
     @property
     def parent_id(self):
         if self.parent is None:
             return
         return self.parent.arkindex_id
 
     @property
@@ -198,122 +219,133 @@
 
     @property
     def label(self):
         if self.node is None:
             return "METS Import"
         return self.node.attrib.get("LABEL", self.id)[:250]
 
-    def publish(self, arkindex_client, corpus_id):
+    def publish(
+        self,
+        cache: Cache,
+        arkindex_client: ArkindexAPIClient,
+        corpus_id: UUID,
+        worker_run_id: UUID,
+        publish_metadata: bool = False,
+    ):
         """
         Publish elements not linked to an image: every element mentioned in METS
         that is not described by an ALTO file
         """
         # Check cache
         cache_key = f"mets/{self.id}"
-        self.arkindex_id = Cache.get(cache_key)
+        self.arkindex_id = cache.get(cache_key)
         if self.arkindex_id is not None:
             return self.arkindex_id
 
         # Publish element without any link to an image
+        logger.debug(f"Creating {self.type} {self.label}…")
         try:
-            logger.info(f"Creating {self.type} {self.label}…")
             resp = arkindex_client.request(
                 "CreateElement",
                 body={
                     "name": self.label,
                     "type": self.type,
                     "corpus": str(corpus_id),
                     "parent": self.parent_id and str(self.parent_id) or None,
+                    "worker_run_id": str(worker_run_id),
                 },
             )
         except ErrorResponse as e:
-            raise Exception(f"Failed to create placeholder element: {e.content}")
+            logger.error(f"Failed to create placeholder element: {e.content}")
+            raise UploadProcessingError
 
         self.arkindex_id = resp["id"]
 
         # Publish METS ID as metadata for later reference
-        logger.info(f"Storing METS ID as metadata on {self.arkindex_id}…")
-        try:
-            arkindex_client.request(
-                "CreateMetaData",
-                id=self.arkindex_id,
-                body={
-                    "name": "METS ID",
-                    "value": self.id,
-                    "type": "reference",
-                },
+        if publish_metadata:
+            create_metadata(
+                arkindex_client, self.arkindex_id, self.metadata_list, worker_run_id
             )
 
-        except ErrorResponse as e:
-            logger.error(
-                f"Could not create metadata on element ({self.arkindex_id}): HTTP {e.status_code} - {e.content}"
-            )
-            raise MetsProcessingError
-
         # Store arkindex reference in cache
-        Cache.set(cache_key, self.arkindex_id)
+        cache.set(cache_key, self.arkindex_id)
 
 
 class RootMetsElement(object):
-    def __init__(self, path, iiif_base_url, iiif_prefix=None, dpi_x=None, dpi_y=None):
+    def __init__(
+        self,
+        path: Path,
+        iiif_base_url: str,
+        iiif_prefix: str | None = None,
+        dpi_x: int | None = None,
+        dpi_y: int | None = None,
+    ):
         self.files_mapping = {}
         """Mapping from file_ids (as defined in the METS) to tuple of
         - path to ALTO xml file,
         - Loaded Arkindex summary.
         """
         self.files_order = []
         """
         List of ordered local ALTO files path (as defined in the METS)
         """
+        self.metadata_list = {}
+        """
+        Mapping from node ID (as defined in the METS) to list of Arkindex metadata
+        """
 
         with path.open() as file:
             # This ensures that comments in the XML files do not cause the
             # "no Alto namespace found" exception.
             parser = ET.XMLParser(remove_comments=True)
             tree = objectify.parse(file, parser=parser)
             self.root = tree.getroot()
 
+        self.namespaces = {
+            **METS_NS,
+            # Empty namespace prefixes are not supported in XPath
+            **{name or "mets": ns for name, ns in self.root.nsmap.items()},
+        }
+
         self.iiif_base_url = iiif_base_url
         self.iiif_prefix = iiif_prefix
         self.dpi_x = dpi_x
         self.dpi_y = dpi_y
+
         self.parse_files(path)
+        self.parse_metadata()
 
     def parse_files(self, toc_file: Path):
         """
         Parse files listed in the METS file section,
         and extract its immediate child FLocat path
         and build a relevant high-level class to use the content of
         - remote images
         - local Alto file
         """
-
         # Iterate over <file> in any <filesec>
         for file in self.root.xpath(
-            "./mets:fileSec/mets:fileGrp/mets:file", namespaces=METS_NS
+            "./mets:fileSec/mets:fileGrp/mets:file", namespaces=self.namespaces
         ):
 
-            try:
-                location = file.find("mets:FLocat", namespaces=METS_NS)
-                assert (
-                    location is not None
-                ), f"Could not find location of file ({file.get('ID')}) in METS."
-                href = location.get("{" + METS_NS["xlink"] + "}href")
-
-                # Only support local files for now
-                if href.startswith("file://"):
-                    href = href[7:]
-                file_path = (toc_file.parent / href).resolve()
-
-                mime_type = file.attrib.get("MIMETYPE")
-            except AssertionError as e:
+            location = file.find("mets:FLocat", namespaces=self.namespaces)
+            if location is None:
                 logger.error(
-                    f"Could not parse file {file} ({file.get('ID')}): {str(e)}"
+                    f"Could not find location of file ({file.get('ID')}) in METS."
                 )
-                raise MetsProcessingError
+                raise UploadProcessingError
+
+            href = location.get("{" + self.namespaces["xlink"] + "}href")
+
+            # Only support local files for now
+            if href.startswith("file://"):
+                href = href[7:]
+            file_path = (toc_file.parent / href).resolve()
+
+            mime_type = file.attrib.get("MIMETYPE")
 
             # Build IIIF image using local path to an image (even when not present)
             if (
                 mime_type and mime_type.startswith("image/")
             ) or file_path.suffix.lower() in IMAGE_SUFFIXES:
                 relpath = str(file_path.relative_to(toc_file.parent.resolve()))
                 self.files_mapping[file.attrib["ID"]] = MetsImage(
@@ -330,77 +362,171 @@
                     file_path, self.dpi_x, self.dpi_y
                 )
                 self.files_order.append(file_path)
 
             else:
                 logger.warning(f"Unsupported file {file_path}")
 
+    def parse_metadata(self):
+        """
+        Parse metadata and store them with the corresponding node ID
+        """
+
+        def build_metadata(node: ET._Element) -> dict:
+            # Name without namespace
+            name = ET.QName(node).localname
+
+            # If has `xsi:type` attribute, use it instead
+            name = (
+                subname
+                if (subname := node.attrib.get(f"{{{self.namespaces['xsi']}}}type"))
+                else name.capitalize()
+            )
+
+            # Value
+            value = node.text.strip()
+
+            return {
+                "type": get_metadata_type(value),
+                "name": name.strip(),
+                "value": value,
+            }
+
+        # Iterate over <dmdSec> with <mdWrap> child with a `MDTYPE="DC"` attribute
+        for dmdSec in self.root.xpath(
+            './/mets:mdWrap[@MDTYPE="DC"]/parent::mets:dmdSec',
+            namespaces=self.namespaces,
+        ):
+            node_id = dmdSec.attrib.get("ID")
+            if not node_id:
+                continue
+
+            self.metadata_list = AltoMetadata(
+                target="DMDID",
+                metadata_list={
+                    node_id: list(
+                        filter(
+                            itemgetter("value"),
+                            map(
+                                build_metadata,
+                                dmdSec.xpath(".//dc:*", namespaces=self.namespaces),
+                            ),
+                        )
+                    )
+                },
+            )
+
     def list_required_types(self):
         # each <div> with a type will generate a new arkindex element
         return set(
-            self.root.xpath("./mets:structMap//mets:div/@TYPE", namespaces=METS_NS)
+            self.root.xpath(
+                "./mets:structMap//mets:div/@TYPE", namespaces=self.namespaces
+            )
         )
 
+    def publish_alto(
+        self,
+        arkindex_client: ArkindexAPIClient,
+        parent_id: UUID,
+        corpus_id: UUID,
+        worker_run_id: UUID,
+        publish_metadata: bool = True,
+    ):
+        for alto_file in self.files_order:
+            upload_alto_file(
+                path=alto_file,
+                client=arkindex_client,
+                iiif_base_url=self.iiif_base_url,
+                corpus={"id": str(corpus_id)},
+                parent_id=parent_id,
+                types_dict=None,
+                create_types=True,
+                dpi_x=self.dpi_x,
+                dpi_y=self.dpi_y,
+                gallica=False,
+                folders_ark_id_dict=None,
+                alto_namespace=None,
+                worker_run_id=worker_run_id,
+                skip_metadata=not publish_metadata,
+            )
+
+    @save_cache
     def publish(
         self,
-        arkindex_client,
-        parent_id,
-        corpus_id,
-        worker_run_id=None,
-        publish_metadatas=True,
+        cache: Cache,
+        arkindex_client: ArkindexAPIClient,
+        parent_id: UUID,
+        corpus_id: UUID,
+        worker_run_id: UUID,
+        publish_metadata: bool = True,
     ):
         """Build the hierarchy on Arkindex, browsing the tree in a breadth-first fashion
 
         :param arkindex_client: Arkindex API client.
         :param parent_id: Root element id on Arkindex.
         :param corpus_id: ID of the corpus where the element will be created
         """
         # Mock top element as it's already present in Arkindex and
         # has no real presence in the METS file
         top = MetsElement(None)
         top.arkindex_id = parent_id
 
         # Find all structure maps and process their children
-        for div in self.root.xpath("./mets:structMap/mets:div", namespaces=METS_NS):
+        for div in self.root.xpath(
+            "./mets:structMap/mets:div", namespaces=self.namespaces
+        ):
 
             # Convert XML node to MetsElement, linked to our top element
             element = MetsElement(div, parent=top)
-            logger.info(f"Build {element.type} {element.id} : {element.label}")
+            logger.debug(f"Build {element.type} {element.id}: {element.label}")
 
             self.publish_element(
-                arkindex_client, corpus_id, element, worker_run_id, publish_metadatas
+                cache,
+                arkindex_client,
+                corpus_id,
+                element,
+                worker_run_id,
+                publish_metadata,
             )
 
     def publish_element(
         self,
-        arkindex_client,
-        corpus_id,
+        cache: Cache,
+        arkindex_client: ArkindexAPIClient,
+        corpus_id: UUID,
         element: MetsElement,
-        worker_run_id=None,
-        publish_metadatas=True,
+        worker_run_id: UUID,
+        publish_metadata: bool = True,
     ):
         """
         Recursive method that process a METS structural node
         and publishes relevant parts on Arkindex (image or elements)
         """
+        # Create a placeholder element
+        element.metadata_list.extend(self.metadata_list.get_metadata_list(element.node))
+        element.publish(
+            cache, arkindex_client, corpus_id, worker_run_id, publish_metadata
+        )
+
         # Simple discovery algo where we only remember the first alto & image found
         data, images = [], []
 
         def add_image(mets_image: MetsImage) -> None:
             """
             Only add a MetsImage to the image list if it is not already there
             """
             existing_image = next(
                 (image for image in images if image.url == mets_image.url), None
             )
             if not existing_image:
                 images.append(mets_image)
 
-        image = None
-        for area in element.node.findall("./mets:fptr//mets:area", namespaces=METS_NS):
+        for area in element.node.findall(
+            "./mets:fptr//mets:area", namespaces=self.namespaces
+        ):
             file = self.files_mapping.get(area.attrib["FILEID"])
             if file is None:
                 continue
             if isinstance(file, MetsAlto):
                 alto = file
                 alto_begin = area.attrib.get("BEGIN")
                 data.append((alto, alto_begin))
@@ -412,44 +538,44 @@
                             iiif_base_url=self.iiif_base_url,
                             iiif_prefix=self.iiif_prefix,
                         )
                     )
             elif isinstance(file, MetsImage):
                 add_image(file)
 
+        image = None
         if images:
             # There should be only one image
-            assert len(images) == 1
+            if len(images) != 1:
+                logger.error("Found several images")
+                raise UploadProcessingError
             image = images.pop()
 
-        if not data:
-            # Simply create a placeholder element
-            element.publish(arkindex_client, corpus_id)
-        else:
-            for alto, alto_begin in data:
-                # Parse then publish on Arkindex
-                alto.parse(alto_begin)
-
-                # Publish IIIF image
-                if image:
-                    image.publish(arkindex_client)
-
-                # Store arkindex id on element
-                element.arkindex_id = alto.publish(
-                    arkindex_client,
-                    corpus_id,
-                    element.parent_id,
-                    image,
-                    worker_run_id,
-                    publish_metadatas,
-                )
+        for alto, alto_begin in data:
+            # Parse then publish on Arkindex
+            alto.parse(alto_begin)
+
+            # Publish IIIF image
+            if image:
+                image.publish(cache, arkindex_client)
+
+            # Store arkindex id on element
+            alto.publish(
+                arkindex_client,
+                corpus_id,
+                worker_run_id,
+                element.arkindex_id,
+                image,
+                publish_metadata,
+            )
 
         # Recursion
-        for child in element.node.findall("./mets:div", namespaces=METS_NS):
+        for child in element.node.findall("./mets:div", namespaces=self.namespaces):
             child_element = MetsElement(child, parent=element)
             self.publish_element(
+                cache,
                 arkindex_client,
                 corpus_id,
                 child_element,
                 worker_run_id,
-                publish_metadatas,
+                publish_metadata,
             )
```

### Comparing `arkindex-cli-0.4.1/arkindex_cli/commands/upload/minio_client.py` & `arkindex-cli-0.4.2/arkindex_cli/commands/upload/minio_client.py`

 * *Files identical despite different names*

### Comparing `arkindex-cli-0.4.1/arkindex_cli/commands/upload/page_xml_import.py` & `arkindex-cli-0.4.2/arkindex_cli/commands/upload/page_xml_import.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 import os
 from pathlib import Path
 from typing import Optional
 from uuid import UUID
 
 from apistar.exceptions import ErrorResponse
 from rich.progress import Progress
-from transkribus.pagexml import PageXmlPage
 
 from arkindex_cli.auth import Profiles
+from teklia_toolbox.pagexml import PageXmlPage
 
 logger = logging.getLogger(__name__)
 
 
 class PageXmlParser(object):
     def __init__(self, client, path_or_xml):
         self.pagexml_page = PageXmlPage(path_or_xml)
```

### Comparing `arkindex-cli-0.4.1/arkindex_cli/commands/utils.py` & `arkindex-cli-0.4.2/arkindex_cli/commands/utils.py`

 * *Files identical despite different names*

### Comparing `arkindex-cli-0.4.1/arkindex_cli/commands/worker/__init__.py` & `arkindex-cli-0.4.2/arkindex_cli/commands/worker/__init__.py`

 * *Files identical despite different names*

### Comparing `arkindex-cli-0.4.1/arkindex_cli/commands/worker/publish.py` & `arkindex-cli-0.4.2/arkindex_cli/commands/worker/publish.py`

 * *Files identical despite different names*

### Comparing `arkindex-cli-0.4.1/arkindex_cli/git.py` & `arkindex-cli-0.4.2/arkindex_cli/git.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import subprocess
 from functools import cached_property
 from urllib.parse import urljoin
 
 logging.basicConfig(level=logging.INFO, format="[%(levelname)s] %(message)s")
 logger = logging.getLogger(__name__)
 
-GIT_SSH_REMOTE = re.compile(r"git@(?P<base>.+):(?P<project>.+)\.git")
+GIT_SSH_REMOTE = re.compile(r"git@(?P<base>.+):(?P<project>((?!\.git).)+)(\.git)?")
 CI_AUTHOR_REGEX = re.compile(r"^(?P<name>.+) <(?P<email>.+)>$")
 
 
 class LocalGitRepository(object):
     """
     Helper class to retrieve the attributes of a git project locally
     by running commands via sub processes, or using GitLab CI variables.
```

### Comparing `arkindex-cli-0.4.1/arkindex_cli/utils.py` & `arkindex-cli-0.4.2/arkindex_cli/utils.py`

 * *Files identical despite different names*

### Comparing `arkindex-cli-0.4.1/arkindex_cli.egg-info/PKG-INFO` & `arkindex-cli-0.4.2/arkindex_cli.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arkindex-cli
-Version: 0.4.1
+Version: 0.4.2
 Summary: Arkindex CLI client easy and sexy to use
 Home-page: https://arkindex.teklia.com
 Author: Teklia
 Author-email: contact@teklia.com
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: export
```

### Comparing `arkindex-cli-0.4.1/arkindex_cli.egg-info/SOURCES.txt` & `arkindex-cli-0.4.2/arkindex_cli.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -40,17 +40,18 @@
 arkindex_cli/commands/export/utils.py
 arkindex_cli/commands/models/__init__.py
 arkindex_cli/commands/models/publish.py
 arkindex_cli/commands/models/utils.py
 arkindex_cli/commands/selection/__init__.py
 arkindex_cli/commands/selection/populate.py
 arkindex_cli/commands/upload/__init__.py
+arkindex_cli/commands/upload/cache.py
+arkindex_cli/commands/upload/exceptions.py
 arkindex_cli/commands/upload/iiif.py
 arkindex_cli/commands/upload/minio_client.py
 arkindex_cli/commands/upload/page_xml_import.py
 arkindex_cli/commands/upload/alto/__init__.py
 arkindex_cli/commands/upload/alto/parser.py
 arkindex_cli/commands/upload/mets/__init__.py
-arkindex_cli/commands/upload/mets/cache.py
 arkindex_cli/commands/upload/mets/parser.py
 arkindex_cli/commands/worker/__init__.py
 arkindex_cli/commands/worker/publish.py
```

### Comparing `arkindex-cli-0.4.1/setup.py` & `arkindex-cli-0.4.2/setup.py`

 * *Files identical despite different names*

