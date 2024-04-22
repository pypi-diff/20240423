# Comparing `tmp/devicetorch-0.1.4.tar.gz` & `tmp/devicetorch-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "devicetorch-0.1.4.tar", last modified: Sat Apr 20 21:19:32 2024, max compression
+gzip compressed data, was "devicetorch-0.1.5.tar", last modified: Mon Apr 22 08:20:19 2024, max compression
```

## Comparing `devicetorch-0.1.4.tar` & `devicetorch-0.1.5.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 x          (501) staff       (20)        0 2024-04-20 21:19:32.750687 devicetorch-0.1.4/
--rw-r--r--   0 x          (501) staff       (20)       55 2024-04-20 21:19:32.750540 devicetorch-0.1.4/PKG-INFO
--rw-r--r--   0 x          (501) staff       (20)      278 2024-04-20 21:16:18.000000 devicetorch-0.1.4/README.md
-drwxr-xr-x   0 x          (501) staff       (20)        0 2024-04-20 21:19:32.749850 devicetorch-0.1.4/devicetorch/
--rw-r--r--   0 x          (501) staff       (20)      150 2024-04-20 21:08:37.000000 devicetorch-0.1.4/devicetorch/__init__.py
-drwxr-xr-x   0 x          (501) staff       (20)        0 2024-04-20 21:19:32.750372 devicetorch-0.1.4/devicetorch.egg-info/
--rw-r--r--   0 x          (501) staff       (20)       55 2024-04-20 21:19:32.000000 devicetorch-0.1.4/devicetorch.egg-info/PKG-INFO
--rw-r--r--   0 x          (501) staff       (20)      182 2024-04-20 21:19:32.000000 devicetorch-0.1.4/devicetorch.egg-info/SOURCES.txt
--rw-r--r--   0 x          (501) staff       (20)        1 2024-04-20 21:19:32.000000 devicetorch-0.1.4/devicetorch.egg-info/dependency_links.txt
--rw-r--r--   0 x          (501) staff       (20)       12 2024-04-20 21:19:32.000000 devicetorch-0.1.4/devicetorch.egg-info/top_level.txt
--rw-r--r--   0 x          (501) staff       (20)       38 2024-04-20 21:19:32.750725 devicetorch-0.1.4/setup.cfg
--rw-r--r--   0 x          (501) staff       (20)      128 2024-04-20 21:18:47.000000 devicetorch-0.1.4/setup.py
+drwxr-xr-x   0 x          (501) staff       (20)        0 2024-04-22 08:20:19.339613 devicetorch-0.1.5/
+-rw-r--r--   0 x          (501) staff       (20)       55 2024-04-22 08:20:19.339434 devicetorch-0.1.5/PKG-INFO
+-rw-r--r--   0 x          (501) staff       (20)      344 2024-04-20 22:15:20.000000 devicetorch-0.1.5/README.md
+drwxr-xr-x   0 x          (501) staff       (20)        0 2024-04-22 08:20:19.338702 devicetorch-0.1.5/devicetorch/
+-rw-r--r--   0 x          (501) staff       (20)      305 2024-04-22 08:19:40.000000 devicetorch-0.1.5/devicetorch/__init__.py
+drwxr-xr-x   0 x          (501) staff       (20)        0 2024-04-22 08:20:19.339214 devicetorch-0.1.5/devicetorch.egg-info/
+-rw-r--r--   0 x          (501) staff       (20)       55 2024-04-22 08:20:19.000000 devicetorch-0.1.5/devicetorch.egg-info/PKG-INFO
+-rw-r--r--   0 x          (501) staff       (20)      182 2024-04-22 08:20:19.000000 devicetorch-0.1.5/devicetorch.egg-info/SOURCES.txt
+-rw-r--r--   0 x          (501) staff       (20)        1 2024-04-22 08:20:19.000000 devicetorch-0.1.5/devicetorch.egg-info/dependency_links.txt
+-rw-r--r--   0 x          (501) staff       (20)       12 2024-04-22 08:20:19.000000 devicetorch-0.1.5/devicetorch.egg-info/top_level.txt
+-rw-r--r--   0 x          (501) staff       (20)       38 2024-04-22 08:20:19.339659 devicetorch-0.1.5/setup.cfg
+-rw-r--r--   0 x          (501) staff       (20)      128 2024-04-22 08:19:56.000000 devicetorch-0.1.5/setup.py
```

