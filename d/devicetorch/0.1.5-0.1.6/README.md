# Comparing `tmp/devicetorch-0.1.5.tar.gz` & `tmp/devicetorch-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "devicetorch-0.1.5.tar", last modified: Mon Apr 22 08:20:19 2024, max compression
+gzip compressed data, was "devicetorch-0.1.6.tar", last modified: Mon Apr 22 22:50:08 2024, max compression
```

## Comparing `devicetorch-0.1.5.tar` & `devicetorch-0.1.6.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 x          (501) staff       (20)        0 2024-04-22 08:20:19.339613 devicetorch-0.1.5/
--rw-r--r--   0 x          (501) staff       (20)       55 2024-04-22 08:20:19.339434 devicetorch-0.1.5/PKG-INFO
--rw-r--r--   0 x          (501) staff       (20)      344 2024-04-20 22:15:20.000000 devicetorch-0.1.5/README.md
-drwxr-xr-x   0 x          (501) staff       (20)        0 2024-04-22 08:20:19.338702 devicetorch-0.1.5/devicetorch/
--rw-r--r--   0 x          (501) staff       (20)      305 2024-04-22 08:19:40.000000 devicetorch-0.1.5/devicetorch/__init__.py
-drwxr-xr-x   0 x          (501) staff       (20)        0 2024-04-22 08:20:19.339214 devicetorch-0.1.5/devicetorch.egg-info/
--rw-r--r--   0 x          (501) staff       (20)       55 2024-04-22 08:20:19.000000 devicetorch-0.1.5/devicetorch.egg-info/PKG-INFO
--rw-r--r--   0 x          (501) staff       (20)      182 2024-04-22 08:20:19.000000 devicetorch-0.1.5/devicetorch.egg-info/SOURCES.txt
--rw-r--r--   0 x          (501) staff       (20)        1 2024-04-22 08:20:19.000000 devicetorch-0.1.5/devicetorch.egg-info/dependency_links.txt
--rw-r--r--   0 x          (501) staff       (20)       12 2024-04-22 08:20:19.000000 devicetorch-0.1.5/devicetorch.egg-info/top_level.txt
--rw-r--r--   0 x          (501) staff       (20)       38 2024-04-22 08:20:19.339659 devicetorch-0.1.5/setup.cfg
--rw-r--r--   0 x          (501) staff       (20)      128 2024-04-22 08:19:56.000000 devicetorch-0.1.5/setup.py
+drwxr-xr-x   0 x          (501) staff       (20)        0 2024-04-22 22:50:08.353872 devicetorch-0.1.6/
+-rw-r--r--   0 x          (501) staff       (20)       55 2024-04-22 22:50:08.353714 devicetorch-0.1.6/PKG-INFO
+-rw-r--r--   0 x          (501) staff       (20)      344 2024-04-20 22:15:20.000000 devicetorch-0.1.6/README.md
+drwxr-xr-x   0 x          (501) staff       (20)        0 2024-04-22 22:50:08.352955 devicetorch-0.1.6/devicetorch/
+-rw-r--r--   0 x          (501) staff       (20)      481 2024-04-22 22:49:44.000000 devicetorch-0.1.6/devicetorch/__init__.py
+drwxr-xr-x   0 x          (501) staff       (20)        0 2024-04-22 22:50:08.353545 devicetorch-0.1.6/devicetorch.egg-info/
+-rw-r--r--   0 x          (501) staff       (20)       55 2024-04-22 22:50:08.000000 devicetorch-0.1.6/devicetorch.egg-info/PKG-INFO
+-rw-r--r--   0 x          (501) staff       (20)      182 2024-04-22 22:50:08.000000 devicetorch-0.1.6/devicetorch.egg-info/SOURCES.txt
+-rw-r--r--   0 x          (501) staff       (20)        1 2024-04-22 22:50:08.000000 devicetorch-0.1.6/devicetorch.egg-info/dependency_links.txt
+-rw-r--r--   0 x          (501) staff       (20)       12 2024-04-22 22:50:08.000000 devicetorch-0.1.6/devicetorch.egg-info/top_level.txt
+-rw-r--r--   0 x          (501) staff       (20)       38 2024-04-22 22:50:08.353962 devicetorch-0.1.6/setup.cfg
+-rw-r--r--   0 x          (501) staff       (20)      128 2024-04-22 22:50:02.000000 devicetorch-0.1.6/setup.py
```

