# Comparing `tmp/pipecraft-0.1.0.tar.gz` & `tmp/pipecraft-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pipecraft-0.1.0.tar", max compression
+gzip compressed data, was "pipecraft-0.2.0.tar", max compression
```

## Comparing `pipecraft-0.1.0.tar` & `pipecraft-0.2.0.tar`

### file list

```diff
@@ -1,4 +1,8 @@
--rw-r--r--   0        0        0        0 2024-03-13 16:24:21.750569 pipecraft-0.1.0/README.md
--rw-r--r--   0        0        0      313 2024-03-13 16:24:21.751569 pipecraft-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-03-13 16:24:21.750569 pipecraft-0.1.0/src/pipecraft/__init__.py
--rw-r--r--   0        0        0      332 1970-01-01 00:00:00.000000 pipecraft-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-03-13 16:24:21.750569 pipecraft-0.2.0/README.md
+-rw-r--r--   0        0        0      371 2024-04-22 22:27:16.783983 pipecraft-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0       94 2024-03-13 18:55:41.032631 pipecraft-0.2.0/src/pipecraft/__init__.py
+-rw-r--r--   0        0        0     2190 2024-03-18 23:06:32.098131 pipecraft-0.2.0/src/pipecraft/backend.py
+-rw-r--r--   0        0        0        0 2024-03-13 18:54:29.572655 pipecraft-0.2.0/src/pipecraft/pcpimage.py
+-rw-r--r--   0        0        0     6598 2024-03-18 19:50:22.640008 pipecraft-0.2.0/src/pipecraft/pipeline.py
+-rw-r--r--   0        0        0      521 2024-04-01 16:00:19.772489 pipecraft-0.2.0/src/pipecraft/utils.py
+-rw-r--r--   0        0        0      496 1970-01-01 00:00:00.000000 pipecraft-0.2.0/PKG-INFO
```

