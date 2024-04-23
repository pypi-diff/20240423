# Comparing `tmp/toolshop-0.1.0.tar.gz` & `tmp/toolshop-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "toolshop-0.1.0.tar", max compression
+gzip compressed data, was "toolshop-0.1.1.tar", max compression
```

## Comparing `toolshop-0.1.0.tar` & `toolshop-0.1.1.tar`

### file list

```diff
@@ -1,4 +1,14 @@
--rw-r--r--   0        0        0        0 2024-04-14 23:27:47.894973 toolshop-0.1.0/README.md
--rw-r--r--   0        0        0      279 2024-04-14 23:27:47.898824 toolshop-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-14 23:27:47.894864 toolshop-0.1.0/toolshop/__init__.py
--rw-r--r--   0        0        0      349 1970-01-01 00:00:00.000000 toolshop-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     2357 2024-04-23 01:03:03.896488 toolshop-0.1.1/README.md
+-rw-r--r--   0        0        0      564 2024-04-23 01:06:05.878315 toolshop-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      288 2024-04-23 00:19:36.662327 toolshop-0.1.1/toolshop/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-18 02:04:46.117267 toolshop-0.1.1/toolshop/agent/__init__.py
+-rw-r--r--   0        0        0      511 2024-04-18 23:41:11.447749 toolshop-0.1.1/toolshop/agent/cli.py
+-rw-r--r--   0        0        0     3199 2024-04-21 01:37:50.945660 toolshop-0.1.1/toolshop/agent/coder.py
+-rw-r--r--   0        0        0     2352 2024-04-21 00:55:42.160724 toolshop-0.1.1/toolshop/agent/instructions.py
+-rw-r--r--   0        0        0     3716 2024-04-23 00:36:13.636544 toolshop-0.1.1/toolshop/base.py
+-rw-r--r--   0        0        0     2917 2024-04-23 00:00:55.778882 toolshop-0.1.1/toolshop/data.py
+-rw-r--r--   0        0        0    15899 2024-04-23 00:17:14.969939 toolshop-0.1.1/toolshop/file.py
+-rw-r--r--   0        0        0     2870 2024-04-23 00:30:16.785113 toolshop-0.1.1/toolshop/gcp.py
+-rw-r--r--   0        0        0     1007 2024-04-17 03:55:18.212948 toolshop-0.1.1/toolshop/logging.py
+-rw-r--r--   0        0        0     2745 2024-04-23 00:03:33.566457 toolshop-0.1.1/toolshop/terminal.py
+-rw-r--r--   0        0        0     3019 1970-01-01 00:00:00.000000 toolshop-0.1.1/PKG-INFO
```

