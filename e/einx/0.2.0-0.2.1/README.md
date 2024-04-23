# Comparing `tmp/einx-0.2.0.tar.gz` & `tmp/einx-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "einx-0.2.0.tar", last modified: Thu Apr  4 18:43:18 2024, max compression
+gzip compressed data, was "einx-0.2.1.tar", last modified: Tue Apr 23 19:30:14 2024, max compression
```

## Comparing `einx-0.2.0.tar` & `einx-0.2.1.tar`

### file list

```diff
@@ -1,62 +1,67 @@
-drwxrwxr-x   0 ferflo    (1000) ferflo    (1000)        0 2024-04-04 18:43:18.670449 einx-0.2.0/
--rw-rw-r--   0 ferflo    (1000) ferflo    (1000)     1093 2024-01-17 12:19:00.000000 einx-0.2.0/LICENSE
--rw-rw-r--   0 ferflo    (1000) ferflo    (1000)     6628 2024-04-04 18:43:18.670449 einx-0.2.0/PKG-INFO
--rw-rw-r--   0 ferflo    (1000) ferflo    (1000)     6075 2024-04-03 18:50:31.000000 einx-0.2.0/README.md
-drwxrwxr-x   0 ferflo    (1000) ferflo    (1000)        0 2024-04-04 18:43:18.666448 einx-0.2.0/einx/
--rw-rw-r--   0 ferflo    (1000) ferflo    (1000)      203 2024-03-08 12:29:27.000000 einx-0.2.0/einx/__init__.py
-drwxrwxr-x   0 ferflo    (1000) ferflo    (1000)        0 2024-04-04 18:43:18.666448 einx-0.2.0/einx/backend/
--rw-rw-r--   0 ferflo    (1000) ferflo    (1000)     2722 2024-03-18 09:17:36.000000 einx-0.2.0/einx/backend/__init__.py
--rw-rw-r--   0 ferflo    (1000) ferflo    (1000)     3256 2024-04-04 08:32:06.000000 einx-0.2.0/einx/backend/_dask.py
--rw-rw-r--   0 ferflo    (1000) ferflo    (1000)     2649 2024-04-04 08:32:08.000000 einx-0.2.0/einx/backend/_jax.py
--rw-rw-r--   0 ferflo    (1000) ferflo    (1000)     4731 2024-04-04 08:32:13.000000 einx-0.2.0/einx/backend/_mlx.py
--rw-rw-r--   0 ferflo    (1000) ferflo    (1000)     4289 2024-04-04 08:32:16.000000 einx-0.2.0/einx/backend/_numpy.py
--rw-rw-r--   0 ferflo    (1000) ferflo    (1000)     7190 2024-04-04 08:32:20.000000 einx-0.2.0/einx/backend/_tensorflow.py
--rw-rw-r--   0 ferflo    (1000) ferflo    (1000)     8826 2024-04-04 12:37:53.000000 einx-0.2.0/einx/backend/_torch.py
--rw-rw-r--   0 ferflo    (1000) ferflo    (1000)      847 2024-04-04 08:33:01.000000 einx-0.2.0/einx/backend/base.py
--rw-rw-r--   0 ferflo    (1000) ferflo    (1000)    30761 2024-04-04 07:52:02.000000 einx-0.2.0/einx/backend/tracer.py
-drwxrwxr-x   0 ferflo    (1000) ferflo    (1000)        0 2024-04-04 18:43:18.666448 einx-0.2.0/einx/expr/
--rw-rw-r--   0 ferflo    (1000) ferflo    (1000)       59 2023-12-14 11:24:25.000000 einx-0.2.0/einx/expr/__init__.py
--rw-rw-r--   0 ferflo    (1000) ferflo    (1000)     9078 2024-03-08 18:36:53.000000 einx-0.2.0/einx/expr/solver.py
--rw-rw-r--   0 ferflo    (1000) ferflo    (1000)    27957 2024-03-29 10:45:00.000000 einx-0.2.0/einx/expr/stage1.py
--rw-rw-r--   0 ferflo    (1000) ferflo    (1000)    40301 2024-03-29 10:50:18.000000 einx-0.2.0/einx/expr/stage2.py
--rw-rw-r--   0 ferflo    (1000) ferflo    (1000)    17055 2024-03-09 11:58:53.000000 einx-0.2.0/einx/expr/stage3.py
--rw-rw-r--   0 ferflo    (1000) ferflo    (1000)     5152 2024-03-08 22:56:33.000000 einx-0.2.0/einx/expr/util.py
--rw-rw-r--   0 ferflo    (1000) ferflo    (1000)     5745 2024-04-03 21:49:58.000000 einx-0.2.0/einx/lru_cache.py
-drwxrwxr-x   0 ferflo    (1000) ferflo    (1000)        0 2024-04-04 18:43:18.666448 einx-0.2.0/einx/nn/
--rw-rw-r--   0 ferflo    (1000) ferflo    (1000)       56 2024-03-08 15:08:02.000000 einx-0.2.0/einx/nn/__init__.py
--rw-rw-r--   0 ferflo    (1000) ferflo    (1000)     7609 2024-03-29 10:45:00.000000 einx-0.2.0/einx/nn/equinox.py
--rw-rw-r--   0 ferflo    (1000) ferflo    (1000)    10042 2024-03-29 10:45:00.000000 einx-0.2.0/einx/nn/flax.py
--rw-rw-r--   0 ferflo    (1000) ferflo    (1000)      476 2024-03-08 15:13:23.000000 einx-0.2.0/einx/nn/framework.py
--rw-rw-r--   0 ferflo    (1000) ferflo    (1000)     8107 2024-04-04 12:39:18.000000 einx-0.2.0/einx/nn/haiku.py
--rw-rw-r--   0 ferflo    (1000) ferflo    (1000)     8968 2024-03-29 10:45:00.000000 einx-0.2.0/einx/nn/keras.py
--rw-rw-r--   0 ferflo    (1000) ferflo    (1000)     4880 2024-03-08 17:33:26.000000 einx-0.2.0/einx/nn/nn.py
--rw-rw-r--   0 ferflo    (1000) ferflo    (1000)     9182 2024-03-29 10:10:27.000000 einx-0.2.0/einx/nn/torch.py
-drwxrwxr-x   0 ferflo    (1000) ferflo    (1000)        0 2024-04-04 18:43:18.670449 einx-0.2.0/einx/op/
--rw-rw-r--   0 ferflo    (1000) ferflo    (1000)      207 2024-03-08 15:08:02.000000 einx-0.2.0/einx/op/__init__.py
--rw-rw-r--   0 ferflo    (1000) ferflo    (1000)     6532 2024-03-09 11:51:38.000000 einx-0.2.0/einx/op/arange.py
--rw-rw-r--   0 ferflo    (1000) ferflo    (1000)    10953 2024-03-29 10:45:00.000000 einx-0.2.0/einx/op/dot.py
--rw-rw-r--   0 ferflo    (1000) ferflo    (1000)    16678 2024-04-04 07:48:15.000000 einx-0.2.0/einx/op/elementwise.py
--rw-rw-r--   0 ferflo    (1000) ferflo    (1000)    20042 2024-03-29 10:10:27.000000 einx-0.2.0/einx/op/index.py
--rw-rw-r--   0 ferflo    (1000) ferflo    (1000)     6007 2024-04-03 21:50:06.000000 einx-0.2.0/einx/op/rearrange.py
--rw-rw-r--   0 ferflo    (1000) ferflo    (1000)    12644 2024-03-09 12:24:47.000000 einx-0.2.0/einx/op/reduce.py
--rw-rw-r--   0 ferflo    (1000) ferflo    (1000)     4943 2024-03-09 12:29:03.000000 einx-0.2.0/einx/op/solve.py
--rw-rw-r--   0 ferflo    (1000) ferflo    (1000)    10039 2024-04-03 21:49:55.000000 einx-0.2.0/einx/op/util.py
--rw-rw-r--   0 ferflo    (1000) ferflo    (1000)    14980 2024-03-09 20:06:11.000000 einx-0.2.0/einx/op/vmap.py
--rw-rw-r--   0 ferflo    (1000) ferflo    (1000)    12470 2024-03-29 11:52:50.000000 einx-0.2.0/einx/op/vmap_with_axis.py
--rw-rw-r--   0 ferflo    (1000) ferflo    (1000)     2512 2024-04-04 12:43:22.000000 einx-0.2.0/einx/param.py
--rw-rw-r--   0 ferflo    (1000) ferflo    (1000)     1795 2024-03-08 17:33:26.000000 einx-0.2.0/einx/traceback_util.py
--rw-rw-r--   0 ferflo    (1000) ferflo    (1000)     2384 2024-03-08 17:33:26.000000 einx-0.2.0/einx/tree_util.py
--rw-rw-r--   0 ferflo    (1000) ferflo    (1000)       98 2024-01-20 12:36:57.000000 einx-0.2.0/einx/types.py
-drwxrwxr-x   0 ferflo    (1000) ferflo    (1000)        0 2024-04-04 18:43:18.666448 einx-0.2.0/einx.egg-info/
--rw-rw-r--   0 ferflo    (1000) ferflo    (1000)     6628 2024-04-04 18:43:18.000000 einx-0.2.0/einx.egg-info/PKG-INFO
--rw-rw-r--   0 ferflo    (1000) ferflo    (1000)     1038 2024-04-04 18:43:18.000000 einx-0.2.0/einx.egg-info/SOURCES.txt
--rw-rw-r--   0 ferflo    (1000) ferflo    (1000)        1 2024-04-04 18:43:18.000000 einx-0.2.0/einx.egg-info/dependency_links.txt
--rw-rw-r--   0 ferflo    (1000) ferflo    (1000)       59 2024-04-04 18:43:18.000000 einx-0.2.0/einx.egg-info/requires.txt
--rw-rw-r--   0 ferflo    (1000) ferflo    (1000)        5 2024-04-04 18:43:18.000000 einx-0.2.0/einx.egg-info/top_level.txt
--rw-rw-r--   0 ferflo    (1000) ferflo    (1000)       79 2024-04-04 18:43:18.670449 einx-0.2.0/setup.cfg
--rw-rw-r--   0 ferflo    (1000) ferflo    (1000)      993 2024-04-04 18:39:13.000000 einx-0.2.0/setup.py
-drwxrwxr-x   0 ferflo    (1000) ferflo    (1000)        0 2024-04-04 18:43:18.670449 einx-0.2.0/test/
--rw-rw-r--   0 ferflo    (1000) ferflo    (1000)     2102 2024-03-09 20:06:07.000000 einx-0.2.0/test/test_compare_einops.py
--rw-rw-r--   0 ferflo    (1000) ferflo    (1000)    10724 2024-03-09 18:47:00.000000 einx-0.2.0/test/test_nn.py
--rw-rw-r--   0 ferflo    (1000) ferflo    (1000)    29230 2024-04-04 12:55:32.000000 einx-0.2.0/test/test_shapes.py
--rw-rw-r--   0 ferflo    (1000) ferflo    (1000)     5526 2024-03-18 09:21:31.000000 einx-0.2.0/test/test_values.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:30:14.767382 einx-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-04-23 19:30:09.000000 einx-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6759 2024-04-23 19:30:14.767382 einx-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6054 2024-04-23 19:30:09.000000 einx-0.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:30:14.755382 einx-0.2.1/einx/
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-04-23 19:30:09.000000 einx-0.2.1/einx/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:30:14.759382 einx-0.2.1/einx/backend/
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-04-23 19:30:09.000000 einx-0.2.1/einx/backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4192 2024-04-23 19:30:09.000000 einx-0.2.1/einx/backend/_dask.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4236 2024-04-23 19:30:09.000000 einx-0.2.1/einx/backend/_jax.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5451 2024-04-23 19:30:09.000000 einx-0.2.1/einx/backend/_mlx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3791 2024-04-23 19:30:09.000000 einx-0.2.1/einx/backend/_numpy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10275 2024-04-23 19:30:09.000000 einx-0.2.1/einx/backend/_tensorflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15560 2024-04-23 19:30:09.000000 einx-0.2.1/einx/backend/_torch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5644 2024-04-23 19:30:09.000000 einx-0.2.1/einx/backend/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3794 2024-04-23 19:30:09.000000 einx-0.2.1/einx/backend/register.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:30:14.759382 einx-0.2.1/einx/expr/
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-23 19:30:09.000000 einx-0.2.1/einx/expr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9078 2024-04-23 19:30:09.000000 einx-0.2.1/einx/expr/solver.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27957 2024-04-23 19:30:09.000000 einx-0.2.1/einx/expr/stage1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40301 2024-04-23 19:30:09.000000 einx-0.2.1/einx/expr/stage2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16950 2024-04-23 19:30:09.000000 einx-0.2.1/einx/expr/stage3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5152 2024-04-23 19:30:09.000000 einx-0.2.1/einx/expr/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:30:14.763382 einx-0.2.1/einx/nn/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-23 19:30:09.000000 einx-0.2.1/einx/nn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9311 2024-04-23 19:30:09.000000 einx-0.2.1/einx/nn/equinox.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12882 2024-04-23 19:30:09.000000 einx-0.2.1/einx/nn/flax.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10561 2024-04-23 19:30:09.000000 einx-0.2.1/einx/nn/haiku.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10736 2024-04-23 19:30:09.000000 einx-0.2.1/einx/nn/keras.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4986 2024-04-23 19:30:09.000000 einx-0.2.1/einx/nn/nn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11096 2024-04-23 19:30:09.000000 einx-0.2.1/einx/nn/torch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:30:14.763382 einx-0.2.1/einx/op/
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-04-23 19:30:09.000000 einx-0.2.1/einx/op/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6539 2024-04-23 19:30:09.000000 einx-0.2.1/einx/op/arange.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10766 2024-04-23 19:30:09.000000 einx-0.2.1/einx/op/dot.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16570 2024-04-23 19:30:09.000000 einx-0.2.1/einx/op/elementwise.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19942 2024-04-23 19:30:09.000000 einx-0.2.1/einx/op/index.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5921 2024-04-23 19:30:09.000000 einx-0.2.1/einx/op/rearrange.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12633 2024-04-23 19:30:09.000000 einx-0.2.1/einx/op/reduce.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4945 2024-04-23 19:30:09.000000 einx-0.2.1/einx/op/solve.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9592 2024-04-23 19:30:09.000000 einx-0.2.1/einx/op/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15807 2024-04-23 19:30:09.000000 einx-0.2.1/einx/op/vmap.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12859 2024-04-23 19:30:09.000000 einx-0.2.1/einx/op/vmap_with_axis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1795 2024-04-23 19:30:09.000000 einx-0.2.1/einx/traceback_util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:30:14.767382 einx-0.2.1/einx/tracer/
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-23 19:30:09.000000 einx-0.2.1/einx/tracer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19049 2024-04-23 19:30:09.000000 einx-0.2.1/einx/tracer/compile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7716 2024-04-23 19:30:09.000000 einx-0.2.1/einx/tracer/decorator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3339 2024-04-23 19:30:09.000000 einx-0.2.1/einx/tracer/input.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4416 2024-04-23 19:30:09.000000 einx-0.2.1/einx/tracer/optimize.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16072 2024-04-23 19:30:09.000000 einx-0.2.1/einx/tracer/tensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8430 2024-04-23 19:30:09.000000 einx-0.2.1/einx/tracer/tracer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2384 2024-04-23 19:30:09.000000 einx-0.2.1/einx/tree_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-23 19:30:09.000000 einx-0.2.1/einx/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:30:14.767382 einx-0.2.1/einx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6759 2024-04-23 19:30:14.000000 einx-0.2.1/einx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-04-23 19:30:14.000000 einx-0.2.1/einx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 19:30:14.000000 einx-0.2.1/einx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-23 19:30:14.000000 einx-0.2.1/einx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-23 19:30:14.000000 einx-0.2.1/einx.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-23 19:30:14.767382 einx-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      993 2024-04-23 19:30:09.000000 einx-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:30:14.767382 einx-0.2.1/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     2102 2024-04-23 19:30:09.000000 einx-0.2.1/test/test_compare_einops.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10566 2024-04-23 19:30:09.000000 einx-0.2.1/test/test_nn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31046 2024-04-23 19:30:09.000000 einx-0.2.1/test/test_shapes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5773 2024-04-23 19:30:09.000000 einx-0.2.1/test/test_values.py
```

### Comparing `einx-0.2.0/LICENSE` & `einx-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `einx-0.2.0/PKG-INFO` & `einx-0.2.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,29 @@
 Metadata-Version: 2.1
 Name: einx
-Version: 0.2.0
+Version: 0.2.1
 Summary: Tensor Operations Expressed in Einstein-Inspired Notation
 Home-page: https://github.com/fferflo/einx
 Author: Florian Fervers
 Author-email: florian.fervers@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: numpy
+Requires-Dist: sympy
+Requires-Dist: frozendict
 Provides-Extra: torch
+Requires-Dist: torch>=2; extra == "torch"
 Provides-Extra: keras
-License-File: LICENSE
+Requires-Dist: keras>=3; extra == "keras"
 
 # *einx* - Tensor Operations in Einstein-Inspired Notation
 
 [![pytest](https://github.com/fferflo/einx/actions/workflows/run_pytest.yml/badge.svg)](https://github.com/fferflo/einx/actions/workflows/run_pytest.yml)
 [![Documentation](https://img.shields.io/badge/documentation-link-blue.svg)](https://einx.readthedocs.io)
 [![PyPI version](https://badge.fury.io/py/einx.svg)](https://badge.fury.io/py/einx)
 [![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue.svg)](https://www.python.org/downloads/release/python-380/)
@@ -129,15 +134,15 @@
 
 einx traces the required backend operations for a given call into graph representation and just-in-time compiles them into a regular Python function using Python's [`exec()`](https://docs.python.org/3/library/functions.html#exec). This reduces overhead to a single cache lookup and allows inspecting the generated function. For example:
 
 ```python
 >>> x = np.zeros((3, 10, 10))
 >>> graph = einx.sum("... (g [c])", x, g=2, graph=True)
 >>> print(graph)
-# backend: einx.backend.numpy
+import numpy as np
 def op0(i0):
-    x1 = backend.reshape(i0, (3, 10, 2, 5))
-    x0 = backend.sum(x1, axis=3)
-    return x0
+    x0 = np.reshape(i0, (3, 10, 2, 5))
+    x1 = np.sum(x0, axis=3)
+    return x1
 ```
 
 See [Just-in-time compilation](https://einx.readthedocs.io/en/latest/gettingstarted/jit.html) for more details.
```

### Comparing `einx-0.2.0/README.md` & `einx-0.2.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -111,15 +111,15 @@
 
 einx traces the required backend operations for a given call into graph representation and just-in-time compiles them into a regular Python function using Python's [`exec()`](https://docs.python.org/3/library/functions.html#exec). This reduces overhead to a single cache lookup and allows inspecting the generated function. For example:
 
 ```python
 >>> x = np.zeros((3, 10, 10))
 >>> graph = einx.sum("... (g [c])", x, g=2, graph=True)
 >>> print(graph)
-# backend: einx.backend.numpy
+import numpy as np
 def op0(i0):
-    x1 = backend.reshape(i0, (3, 10, 2, 5))
-    x0 = backend.sum(x1, axis=3)
-    return x0
+    x0 = np.reshape(i0, (3, 10, 2, 5))
+    x1 = np.sum(x0, axis=3)
+    return x1
 ```
 
 See [Just-in-time compilation](https://einx.readthedocs.io/en/latest/gettingstarted/jit.html) for more details.
```

### Comparing `einx-0.2.0/einx/expr/solver.py` & `einx-0.2.1/einx/expr/solver.py`

 * *Files identical despite different names*

### Comparing `einx-0.2.0/einx/expr/stage1.py` & `einx-0.2.1/einx/expr/stage1.py`

 * *Files identical despite different names*

### Comparing `einx-0.2.0/einx/expr/stage2.py` & `einx-0.2.1/einx/expr/stage2.py`

 * *Files identical despite different names*

### Comparing `einx-0.2.0/einx/expr/stage3.py` & `einx-0.2.1/einx/expr/stage3.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import numpy as np
 from functools import partial
 import einx
 
 
 class Expression:
     def __init__(self, value):
-        if not isinstance(value, (int, np.int64, np.int32, np.int16, np.int8)):
+        if not isinstance(value, (int, np.integer)):
             raise TypeError(f"Expected int, got {type(value)}")
         self.value = int(value)
         self.parent = None
 
     @property
     def shape(self):
         return tuple(x.value for x in self)
@@ -106,17 +106,14 @@
 
 
 class Axis(Expression):
     def __init__(self, name, value):
         Expression.__init__(self, value)
         self.name = name if name is not None else f"unnamed.{id(self)}"
 
-    def __repr__(self):
-        return f"Axis({self.name}, {self.value})"
-
     def __str__(self):
         return self.name if not self.is_unnamed else str(self.value)
 
     def __len__(self):
         return 1
 
     def __iter__(self):
```

### Comparing `einx-0.2.0/einx/expr/util.py` & `einx-0.2.1/einx/expr/util.py`

 * *Files identical despite different names*

### Comparing `einx-0.2.0/einx/nn/equinox.py` & `einx-0.2.1/einx/nn/equinox.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,14 +3,103 @@
 import equinox as eqx
 from functools import partial
 import jax.numpy as jnp
 from typing import Optional, Callable, Any
 
 # TODO: type annotations
 
+tjax = einx.tracer.import_("jax")
+
+
+def create_or_retrieve(concrete, name, shape, dtype, init):
+    if name in vars(concrete.module) and vars(concrete.module)[name] is not None:
+        tensor = vars(concrete.module)[name]
+    else:
+        tensor = vars(concrete.module)[name] = init(concrete.rng, shape, dtype)
+    return tensor
+
+
+class ParamFactory:
+    class Concrete(einx.tracer.input.Input):
+        def __init__(self, module, name, init, dtype, rng):
+            self.module = module
+            self.name = name
+            self.init = init
+
+            if dtype is None:
+                if hasattr(module, "dtype"):
+                    dtype = module.dtype
+                else:
+                    dtype = "float32"
+            self.dtype = dtype
+
+            self.rng = rng
+
+        def to_value_and_key(self):
+            return self, ParamFactory.CacheKey(self.name, self.init, self.dtype)
+
+    class CacheKey(einx.tracer.input.CacheKey):
+        def __init__(self, name, init, dtype):
+            self.name = name
+            self.init = init
+            self.dtype = dtype
+
+        def __hash__(self):
+            return hash((self.name, self.init, self.dtype))
+
+        def __eq__(self, other):
+            return (
+                isinstance(other, ParamFactory.CacheKey)
+                and self.name == other.name
+                and self.init == other.init
+                and self.dtype == other.dtype
+            )
+
+        def to_tracer(self, backend, virtual_arg):
+            x = ParamFactory.Tracer(self.name, self.init, self.dtype)
+            return x, x
+
+    class Tracer(einx.tracer.TensorFactory):
+        def __init__(self, name, init, dtype):
+            self.name = name
+            self.init = init
+            self.dtype = dtype
+
+        def __call__(self, shape, kwargs):
+            name = self.name if not self.name is None else kwargs.get("name", None)
+            init = self.init if not self.init is None else kwargs.get("init", None)
+            dtype = self.dtype if not self.dtype is None else kwargs.get("dtype", None)
+
+            if name is None:
+                raise ValueError("Must specify name for tensor factory eqx.Module")
+
+            if init is None:
+                raise ValueError("Must specify init for tensor factory eqx.Module")
+            elif isinstance(init, str):
+                if init == "get_at" or init == "rearrange":
+                    init = tjax.nn.initializers.normal(stddev=0.02)
+                elif init == "add":
+                    init = tjax.nn.initializers.constant(0.0, dtype=dtype)
+                elif init == "multiply":
+                    init = tjax.nn.initializers.constant(1.0, dtype=dtype)
+                elif init == "dot":
+                    init = tjax.nn.initializers.lecun_normal(
+                        kwargs["in_axis"], kwargs["out_axis"], kwargs["batch_axis"]
+                    )
+                else:
+                    raise ValueError(f"Don't know which initializer to use for operation '{init}'")
+            elif isinstance(init, (int, float)):
+                init = tjax.nn.initializers.constant(init, dtype=dtype)
+
+            return einx.tracer.apply(
+                create_or_retrieve,  # TODO: make tracable
+                args=[self, name, shape, dtype, init],
+                output=einx.tracer.Tensor(shape),
+            )
+
 
 def param(module, name=None, init=None, dtype=None, rng=None):
     """Create a tensor factory for Equinox parameters.
 
     Args:
         module: The module to create the parameter in. Must be an instance of ``eqx.Module``.
         name: Name of the parameter. If ``None``, uses a default name determined from the calling
@@ -19,65 +108,15 @@
             from the calling operation. Defaults to ``None``.
         dtype: Data type of the parameter. If ``None``, uses the ``dtype`` member of the calling
             module or ``float32`` if it does not exist. Defaults to ``None``.
 
     Returns:
         A tensor factory with the given default parameters.
     """
-
-    name0 = name
-    init0 = init
-    dtype0 = dtype
-
-    def equinox_param_factory(shape, name=name, dtype=dtype, init=init, **kwargs):
-        if name0 is not None:
-            name = name0
-        if init0 is not None:
-            init = init0
-        if dtype0 is not None:
-            dtype = dtype0
-
-        if name is None:
-            raise ValueError("Must specify name for tensor factory eqx.Module")
-
-        if dtype is None:
-            if hasattr(module, "dtype"):
-                dtype = module.dtype
-            else:
-                dtype = "float32"
-
-        if init is None:
-            raise ValueError("Must specify init for tensor factory eqx.Module")
-        elif isinstance(init, str):
-            if init == "get_at" or init == "rearrange":
-                init = jax.nn.initializers.normal(stddev=0.02)
-            elif init == "add":
-                init = jax.nn.initializers.constant(0.0, dtype=dtype)
-            elif init == "multiply":
-                init = jax.nn.initializers.constant(1.0, dtype=dtype)
-            elif init == "dot":
-                init = jax.nn.initializers.lecun_normal(
-                    kwargs["in_axis"], kwargs["out_axis"], kwargs["batch_axis"]
-                )
-            else:
-                raise ValueError(f"Don't know which initializer to use for operation '{init}'")
-        elif isinstance(init, (int, float)):
-            init = jax.nn.initializers.constant(init, dtype=dtype)
-
-        if vars(module)[name] is not None:
-            tensor = vars(module)[name]
-        else:
-            tensor = vars(module)[name] = init(rng, shape, dtype)
-        return tensor
-
-    return equinox_param_factory
-
-
-def to_tensor_factory(x):
-    return None
+    return ParamFactory.Concrete(module, name, init, dtype, rng)
 
 
 class Norm(eqx.Module):
     """Normalization layer.
 
     Args:
         stats: Einstein string determining the axes along which mean and variance are computed.
```

### Comparing `einx-0.2.0/einx/nn/flax.py` & `einx-0.2.1/einx/nn/keras.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,176 +1,164 @@
-import flax.linen as nn
+import keras
 import einx
-import flax
-from functools import partial
-import jax.numpy as jnp
-from typing import Callable, Union, Optional, Any
+import inspect
+import numpy as np
+from typing import Any, Callable, Optional
+
+_version = tuple(int(i) for i in keras.__version__.split(".")[:2])
+if _version < (3, 0):
+    raise ImportError(f"einx.nn.keras requires Keras version >= 3, but found {keras.__version__}")
+
+
+tkeras = einx.tracer.import_("keras")
+
+
+def create_or_retrieve(layer, name, shape, dtype, init, trainable):
+    if name in vars(layer):
+        tensor = vars(layer)[name]
+    else:
+        tensor = vars(layer)[name] = layer.add_weight(
+            shape=shape,
+            dtype=dtype,
+            initializer=init,
+            name=name,
+            trainable=trainable,
+        )
+    return tensor
+
+
+class ParamFactory:
+    class Concrete(einx.tracer.input.Input):
+        def __init__(self, layer, name, init, dtype, trainable):
+            self.layer = layer
+            self.name = name
+            self.init = init
+
+            if dtype is None:
+                if hasattr(layer, "dtype"):
+                    dtype = layer.dtype
+                else:
+                    dtype = "float32"
+            self.dtype = dtype
+
+            self.trainable = trainable
+
+        def to_value_and_key(self):
+            return self.layer, ParamFactory.CacheKey(
+                self.name, self.init, self.dtype, self.trainable
+            )
+
+    class CacheKey(einx.tracer.input.CacheKey):
+        def __init__(self, name, init, dtype, trainable):
+            self.name = name
+            self.init = init
+            self.dtype = dtype
+            self.trainable = trainable
+
+        def __hash__(self):
+            return hash((self.name, self.init, self.dtype, self.trainable))
+
+        def __eq__(self, other):
+            return (
+                isinstance(other, ParamFactory.CacheKey)
+                and self.name == other.name
+                and self.init == other.init
+                and self.dtype == other.dtype
+                and self.trainable == other.trainable
+            )
+
+        def to_tracer(self, backend, virtual_arg):
+            x = ParamFactory.Tracer(self.name, self.init, self.dtype, self.trainable)
+            return x, x
+
+    class Tracer(einx.tracer.TensorFactory):
+        def __init__(self, name, init, dtype, trainable):
+            self.name = name
+            self.init = init
+            self.dtype = dtype
+            self.trainable = trainable
+
+        def __call__(self, shape, kwargs):
+            name = self.name if not self.name is None else kwargs.get("name", None)
+            init = self.init if not self.init is None else kwargs.get("init", None)
+            dtype = self.dtype if not self.dtype is None else kwargs.get("dtype", None)
+
+            if name is None:
+                raise ValueError("Must specify name for tensor factory keras.layers.Layer")
+
+            if init is None:
+                raise ValueError("Must specify init for tensor factory keras.layers.Layer")
+            elif isinstance(init, str):
+                if init == "get_at" or init == "rearrange":
+                    init = tkeras.initializers.TruncatedNormal(stddev=0.02)
+                elif init == "add":
+                    init = tkeras.initializers.Constant(0.0)
+                elif init == "multiply":
+                    init = tkeras.initializers.Constant(1.0)
+                elif init == "dot":
+                    fan_in = np.prod([shape[i] for i in kwargs["in_axis"]])
+                    std = np.sqrt(1.0 / fan_in) / 0.87962566103423978
+                    init = tkeras.initializers.TruncatedNormal(mean=0.0, stddev=std)
+                else:
+                    raise ValueError(f"Don't know which initializer to use for operation '{init}'")
+            elif isinstance(init, (int, float)):
+                init = tkeras.initializers.Constant(init)
+
+            return einx.tracer.apply(
+                create_or_retrieve,  # TODO: make tracable
+                args=[self, name, shape, dtype, init, self.trainable],
+                output=einx.tracer.Tensor(shape),
+            )
 
 
 def param(
-    bound_method: Union[Callable, nn.Module],
+    layer: keras.layers.Layer,
     name: Optional[str] = None,
     init: Optional[Any] = None,
-    dtype: Optional[nn.dtypes.Dtype] = None,
-    col: Optional[str] = None,
+    dtype: Optional[Any] = None,
+    trainable: bool = True,
 ):
-    """Create a tensor factory for Flax parameters.
+    """Create a tensor factory for Keras parameters.
 
     Args:
-        bound_method: The bound method of a Flax module, i.e. ``nn.Module.param`` or
-            ``nn.Module.variable``, or a module instance in which case its ``param`` method
-            is used.
-        name: Name of the parameter. If ``None``, uses a default name determined from the calling
-            operation. Defaults to ``None``.
+        layer: The layer to create the parameter in. Must be an instance of ``keras.layers.Layer``.
+        name: Name of the parameter. If ``None``, uses a default name determined from the
+            calling operation. Defaults to ``None``.
         init: Initializer for the parameter. If ``None``, uses a default init method determined
             from the calling operation. Defaults to ``None``.
         dtype: Data type of the parameter. If ``None``, uses the ``dtype`` member of the calling
             module or ``float32`` if it does not exist. Defaults to ``None``.
-        col: The collection name to use when ``bound_method`` is ``nn.Module.variable``.
+        trainable: Whether the parameter is trainable. Defaults to ``True``.
 
     Returns:
         A tensor factory with the given default parameters.
     """
-    if isinstance(bound_method, nn.Module):
-        bound_method = bound_method.param
+    return ParamFactory.Concrete(layer, name, init, dtype, trainable)
 
-    name0 = name
-    init0 = init
-    dtype0 = dtype
-
-    def flax_param_factory(shape, name=name, dtype=dtype, init=init, **kwargs):
-        if name0 is not None:
-            name = name0
-        if init0 is not None:
-            init = init0
-        if dtype0 is not None:
-            dtype = dtype0
-
-        if name is None:
-            raise ValueError(
-                "Must specify name for tensor factory flax.linen.Module.{param|variable}"
-            )
 
-        if init is None:
-            raise ValueError(
-                "Must specify init for tensor factory flax.linen.Module.{param|variable}"
-            )
-        elif isinstance(init, str):
-            if init == "get_at" or init == "rearrange":
-                init = nn.initializers.normal(stddev=0.02)
-            elif init == "add":
-                init = nn.initializers.zeros_init()
-            elif init == "multiply":
-                init = nn.initializers.ones_init()
-            elif init == "dot":
-                init = nn.initializers.lecun_normal(
-                    kwargs["in_axis"], kwargs["out_axis"], kwargs["batch_axis"]
-                )
-            else:
-                raise ValueError(f"Don't know which initializer to use for operation '{init}'")
-        elif isinstance(init, (int, float)):
-            init = nn.initializers.constant(init, dtype=dtype)
-
-        if dtype is None:
-            module = bound_method.__self__
-            if hasattr(module, "dtype"):
-                dtype = module.dtype
-            else:
-                dtype = "float32"
-
-        if bound_method.__func__ == nn.Module.param:
-            if col is not None:
-                raise ValueError("col is not accepted for flax.linen.Module.param")
-            return bound_method(name, init, shape, dtype)
-        elif bound_method.__func__ == nn.Module.variable:
-            if col is None:
-                raise ValueError("col must be specified for flax.linen.Module.variable")
-            # Assume that variable initialization does not need an rng key by passing None:
-            return bound_method(col, name, init, None, shape, dtype).value
-        else:
-            raise ValueError(
-                f"Unknown tensor factory flax.linen.Module.{bound_method.__func__.__name__}"
-            )
+def is_leaf(x):
+    return isinstance(x, tuple) and all(isinstance(y, int) for y in x)
 
-    return flax_param_factory
 
+class Layer(keras.layers.Layer):
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
 
-def to_tensor_factory(x):
-    if isinstance(x, nn.Module) or (hasattr(x, "__func__") and x.__func__ == nn.Module.param):
-        return param(x)
-    else:
-        return None
-
-
-# Using _ prefix on classes and a separater constructor, since dataclass/nn.Module does
-# not support **kwargs parameter.
-
-
-class _Norm(nn.Module):
-    stats: str
-    params: str = "b... [c]"
-    mean: bool = True
-    var: bool = True
-    scale: bool = True
-    bias: bool = True
-    decay_rate: float = None
-    epsilon: float = 1e-5
-    fastvar: bool = True
-    dtype: nn.dtypes.Dtype = "float32"
-    kwargs: dict = None
-
-    @nn.compact
-    def __call__(self, x, training=None):
-        if self.decay_rate is not None and training is None:
-            raise ValueError("training must be specified when decay_rate is used")
-
-        use_ema = self.decay_rate is not None and (not training or self.is_initializing())
-        x, mean, var = einx.nn.norm(
-            x,
-            self.stats,
-            self.params,
-            mean=param(self.variable, col="stats", name="mean", dtype=self.dtype)
-            if use_ema and self.mean
-            else self.mean,
-            var=param(self.variable, col="stats", name="var", dtype=self.dtype)
-            if use_ema and self.var
-            else self.var,
-            scale=param(self.param, name="scale", dtype=self.dtype) if self.scale else None,
-            bias=param(self.param, name="bias", dtype=self.dtype) if self.bias else None,
-            epsilon=self.epsilon,
-            fastvar=self.fastvar,
-            **(self.kwargs if self.kwargs is not None else {}),
+    def build(self, inputs_shape):
+        tracers = einx.tree_util.tree_map(
+            lambda shape: keras.ops.zeros(shape, dtype="float32"), inputs_shape, is_leaf=is_leaf
         )
 
-        update_ema = self.decay_rate is not None and training and not self.is_initializing()
-        if update_ema:
-            if self.mean:
-                mean_ema = self.variable("stats", "mean", None)
-                mean_ema.value = self.decay_rate * mean_ema.value + (1 - self.decay_rate) * mean
-            if self.var:
-                var_ema = self.variable("stats", "var", None)
-                var_ema.value = self.decay_rate * var_ema.value + (1 - self.decay_rate) * var
-
-        return x
+        if "is_initializing" in inspect.signature(self.call).parameters:
+            self.call(tracers, is_initializing=True)
+        else:
+            self.call(tracers)
 
 
-def Norm(
-    stats: str,
-    params: str = "b... [c]",
-    mean: bool = True,
-    var: bool = True,
-    scale: bool = True,
-    bias: bool = True,
-    decay_rate: Optional[float] = None,
-    epsilon: float = 1e-5,
-    fastvar: bool = True,
-    dtype: nn.dtypes.Dtype = "float32",
-    name: Optional[str] = None,
-    **kwargs: Any,
-):
+class Norm(Layer):
     """Normalization layer.
 
     Args:
         stats: Einstein string determining the axes along which mean and variance are computed.
             Will be passed to ``einx.reduce``.
         params: Einstein string determining the axes along which learnable parameters are applied.
             Will be passed to ``einx.elementwise``. Defaults to ``"b... [c]"``.
@@ -180,105 +168,130 @@
         bias: Whether to apply a learnable bias according to ``params``. Defaults to ``True``.
         epsilon: A small float added to the variance to avoid division by zero. Defaults
             to ``1e-5``.
         fastvar: Whether to use a fast variance computation. Defaults to ``True``.
         dtype: Data type of the weights. Defaults to ``"float32"``.
         decay_rate: Decay rate for exponential moving average of mean and variance. If ``None``,
             no moving average is applied. Defaults to ``None``.
-        name: Name of the module. Defaults to ``None``.
         **kwargs: Additional parameters that specify values for single axes, e.g. ``a=4``.
     """
 
-    return _Norm(
-        stats,
-        params=params,
-        mean=mean,
-        var=var,
-        scale=scale,
-        bias=bias,
-        decay_rate=decay_rate,
-        epsilon=epsilon,
-        fastvar=fastvar,
-        dtype=dtype,
-        name=name,
-        kwargs=kwargs,
-    )
-
-
-class _Linear(nn.Module):
-    expr: str
-    bias: bool = True
-    dtype: nn.dtypes.Dtype = "float32"
-    kwargs: dict = None
+    def __init__(
+        self,
+        stats: str,
+        params: str = "b... [c]",
+        mean: bool = True,
+        var: bool = True,
+        scale: bool = True,
+        bias: bool = True,
+        epsilon: float = 1e-5,
+        fastvar: bool = True,
+        dtype: Any = "float32",
+        decay_rate: Optional[float] = None,
+        **kwargs: Any,
+    ):
+        super().__init__(dtype=dtype)
+        self.stats = stats
+        self.params = params
+        self.use_mean = mean
+        self.use_var = var
+        self.use_scale = scale
+        self.use_bias = bias
+        self.epsilon = epsilon
+        self.fastvar = fastvar
+        self.decay_rate = decay_rate
+        self.kwargs = kwargs
 
-    @nn.compact
-    def __call__(self, x):
-        return einx.nn.linear(
+    def call(self, x, training=None, is_initializing=False):
+        use_ema = self.decay_rate is not None and (not training or is_initializing)
+        x, mean, var = einx.nn.norm(
             x,
-            self.expr,
-            bias=param(self.param, name="bias", dtype=self.dtype) if self.bias else None,
-            weight=param(self.param, name="weight", dtype=self.dtype),
+            self.stats,
+            self.params,
+            mean=param(self, name="mean", trainable=False)
+            if use_ema and self.use_mean
+            else self.use_mean,
+            var=param(self, name="var", trainable=False)
+            if use_ema and self.use_var
+            else self.use_var,
+            scale=param(self, name="scale", trainable=True) if self.use_scale else None,
+            bias=param(self, name="bias", trainable=True) if self.use_bias else None,
+            epsilon=self.epsilon,
+            fastvar=self.fastvar,
             **(self.kwargs if self.kwargs is not None else {}),
         )
 
+        update_ema = self.decay_rate is not None and training and not is_initializing
+        if update_ema:
+            if self.use_mean:
+                self.mean.assign(
+                    keras.ops.cast(
+                        self.decay_rate * self.mean.value + (1 - self.decay_rate) * mean,
+                        self.mean.dtype,
+                    )
+                )
+            if self.use_var:
+                self.var.assign(
+                    keras.ops.cast(
+                        self.decay_rate * self.var.value + (1 - self.decay_rate) * var,
+                        self.var.dtype,
+                    )
+                )
 
-def Linear(
-    expr: str,
-    bias: bool = True,
-    dtype: nn.dtypes.Dtype = "float32",
-    name: Optional[str] = None,
-    **kwargs: Any,
-):
+        return x
+
+
+class Linear(Layer):
     """Linear layer.
 
     Args:
-        expr: Einstein string determining the axes along which the weight matrix is
-            multiplied. Will be passed to ``einx.dot``.
+        expr: Einstein string determining the axes along which the weight matrix is multiplied.
+            Will be passed to ``einx.dot``.
         bias: Whether to apply a learnable bias. Defaults to ``True``.
         dtype: Data type of the weights. Defaults to ``"float32"``.
-        name: Name of the module. Defaults to ``None``.
         **kwargs: Additional parameters that specify values for single axes, e.g. ``a=4``.
     """
 
-    return _Linear(expr, bias=bias, dtype=dtype, name=name, kwargs=kwargs)
-
+    def __init__(self, expr: str, bias: bool = True, dtype: Any = "float32", **kwargs: Any):
+        super().__init__(dtype=dtype)
 
-class _Dropout(nn.Module):
-    expr: str
-    drop_rate: float
-    rng_collection: str = "dropout"
-    kwargs: dict = None
+        self.expr = expr
+        self.use_bias = bias
+        self.kwargs = kwargs
 
-    @nn.compact
-    def __call__(self, x, training):
-        if training:
-            return einx.nn.dropout(
-                x,
-                self.expr,
-                drop_rate=self.drop_rate,
-                rng=self.make_rng(self.rng_collection),
-                **(self.kwargs if self.kwargs is not None else {}),
-            )
-        else:
-            return x
+    def call(self, x):
+        return einx.nn.linear(
+            x,
+            self.expr,
+            bias=param(self, name="bias") if self.use_bias else None,
+            weight=param(self, name="weight"),
+            **self.kwargs,
+        )
 
 
-def Dropout(
-    expr: str,
-    drop_rate: float,
-    rng_collection: str = "dropout",
-    name: Optional[str] = None,
-    **kwargs: Any,
-):
+class Dropout(Layer):
     """Dropout layer.
 
     Args:
-        expr: Einstein string determining the axes along which dropout is applied. Will be passed
-            to ``einx.elementwise``.
+        expr: Einstein string determining the axes along which dropout is applied. Will be
+            passed to ``einx.elementwise``.
         drop_rate: Drop rate.
-        rng_collection: the rng collection name to use when requesting an rng key. Defaults
-            to ``"dropout"``.
-        name: Name of the module. Defaults to ``None``.
         **kwargs: Additional parameters that specify values for single axes, e.g. ``a=4``.
     """
 
-    return _Dropout(expr, drop_rate, rng_collection=rng_collection, name=name, kwargs=kwargs)
+    def __init__(self, expr: str, drop_rate: float, **kwargs: Any):
+        super().__init__()
+
+        self.expr = expr
+        self.drop_rate = drop_rate
+        self.kwargs = kwargs
+
+    def call(self, x, training=None):
+        if training:
+            return einx.nn.dropout(
+                x,
+                self.expr,
+                drop_rate=self.drop_rate,
+                **self.kwargs,
+            )
+        else:
+            return x
```

### Comparing `einx-0.2.0/einx/nn/haiku.py` & `einx-0.2.1/einx/nn/haiku.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,13 +1,108 @@
 import haiku as hk
 import einx
 from functools import partial
 from haiku._src.base import current_module
 from typing import Any, Callable, Literal, Optional
 
+thk = einx.tracer.import_("haiku", "hk")
+
+
+class ParamFactory:
+    class Concrete(einx.tracer.input.Input):
+        def __init__(self, name, init, dtype, param_type):
+            self.name = name
+            self.init = init
+
+            if dtype is None:
+                module = current_module()
+                if hasattr(module, "dtype"):
+                    dtype = module.dtype
+                else:
+                    dtype = "float32"
+            self.dtype = dtype
+
+            self.param_type = param_type
+
+        def to_value_and_key(self):
+            return None, ParamFactory.CacheKey(self.name, self.init, self.dtype, self.param_type)
+
+    class CacheKey(einx.tracer.input.CacheKey):
+        def __init__(self, name, init, dtype, param_type):
+            self.name = name
+            self.init = init
+            self.dtype = dtype
+            self.param_type = param_type
+
+        def __hash__(self):
+            return hash((self.name, self.init, self.dtype, self.param_type))
+
+        def __eq__(self, other):
+            return (
+                isinstance(other, ParamFactory.CacheKey)
+                and self.name == other.name
+                and self.init == other.init
+                and self.dtype == other.dtype
+                and self.param_type == other.param_type
+            )
+
+        def to_tracer(self, backend, virtual_arg):
+            return (
+                None,
+                ParamFactory.Tracer(self.name, self.init, self.dtype, self.param_type, virtual_arg),
+            )
+
+    class Tracer(einx.tracer.TensorFactory):
+        def __init__(self, name, init, dtype, param_type, depend_on):
+            self.name = name
+            self.init = init
+            self.dtype = dtype
+            self.param_type = param_type
+            self.depend_on = depend_on
+
+        def __call__(self, shape, kwargs):
+            name = self.name if not self.name is None else kwargs.get("name", None)
+            init = self.init if not self.init is None else kwargs.get("init", None)
+            dtype = self.dtype if not self.dtype is None else kwargs.get("dtype", None)
+
+            if name is None:
+                raise ValueError("Must specify name for tensor factory hk.get_{parameter|state}")
+
+            if init is None:
+                raise ValueError("Must specify init for tensor factory hk.get_{parameter|state}")
+            elif isinstance(init, str):
+                if init in "get_at" or init == "rearrange":
+                    init = thk.initializers.RandomNormal(stddev=0.02)
+                elif init == "add":
+                    init = thk.initializers.Constant(0.0)
+                elif init == "multiply":
+                    init = thk.initializers.Constant(1.0)
+                elif init == "dot":
+                    init = thk.initializers.VarianceScaling(
+                        1.0, "fan_in", "truncated_normal", fan_in_axes=kwargs["in_axis"]
+                    )
+                else:
+                    raise ValueError(f"Don't know which initializer to use for operation '{init}'")
+            elif isinstance(init, (int, float)):
+                init = thk.initializers.Constant(init)
+
+            if self.param_type == "parameter":
+                func = thk.get_parameter
+            elif self.param_type == "state":
+                func = thk.get_state
+            else:
+                assert False
+
+            return einx.tracer.apply(
+                func,
+                kwargs={"shape": shape, "name": name, "dtype": dtype, "init": init},
+                output=einx.tracer.Tensor(shape),
+                depend_on=[self.depend_on],
+            )
+
 
 def param(
     func: Literal[hk.get_parameter, hk.get_state] = hk.get_parameter,
     name: Optional[str] = None,
     init: Optional[Any] = None,
     dtype: Optional[Any] = None,
 ):
@@ -21,63 +116,28 @@
             from the calling operation. Defaults to ``None``.
         dtype: Data type of the parameter. If ``None``, uses the ``dtype`` member of the calling
             module or ``float32`` if it does not exist. Defaults to ``None``.
 
     Returns:
         A tensor factory with the given default parameters.
     """
-
-    name0 = name
-    init0 = init
-    dtype0 = dtype
-
-    def haiku_param_factory(shape, name=name, dtype=dtype, init=init, **kwargs):
-        if name0 is not None:
-            name = name0
-        if init0 is not None:
-            init = init0
-        if dtype0 is not None:
-            dtype = dtype0
-
-        if name is None:
-            raise ValueError("Must specify name for tensor factory hk.get_{parameter|state}")
-
-        if init is None:
-            raise ValueError("Must specify init for tensor factory hk.get_{parameter|state}")
-        elif isinstance(init, str):
-            if init in "get_at" or init == "rearrange":
-                init = hk.initializers.RandomNormal(stddev=0.02)
-            elif init == "add":
-                init = hk.initializers.Constant(0.0)
-            elif init == "multiply":
-                init = hk.initializers.Constant(1.0)
-            elif init == "dot":
-                init = hk.initializers.VarianceScaling(
-                    1.0, "fan_in", "truncated_normal", fan_in_axes=kwargs["in_axis"]
-                )
-            else:
-                raise ValueError(f"Don't know which initializer to use for operation '{init}'")
-        elif isinstance(init, (int, float)):
-            init = hk.initializers.Constant(init)
-
-        if dtype is None:
-            module = current_module()
-            if hasattr(module, "dtype"):
-                dtype = module.dtype
-            else:
-                dtype = "float32"
-
-        return func(shape=shape, name=name, dtype=dtype, init=init)
-
-    return haiku_param_factory
+    if func == hk.get_parameter:
+        param_type = "parameter"
+    elif func == hk.get_state:
+        param_type = "state"
+    else:
+        raise ValueError(f"Unknown parameter function '{func}'")
+    return ParamFactory.Concrete(name, init, dtype, param_type)
 
 
-def to_tensor_factory(x):
+# Allow passing hk.get_parameter and hk.get_state as tensor factory:
+@einx.tracer.input.register_tensor_factory
+def tensor_factory(x):
     if id(x) == id(hk.get_parameter) or id(x) == id(hk.get_state):
-        return param(x)
+        return param(x).to_value_and_key()
     else:
         return None
 
 
 class Norm(hk.Module):
     """Normalization layer.
```

### Comparing `einx-0.2.0/einx/nn/keras.py` & `einx-0.2.1/einx/nn/flax.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,124 +1,246 @@
-import keras
+import flax.linen as nn
 import einx
-import inspect
-import numpy as np
-from typing import Any, Callable, Optional
-
-_version = tuple(int(i) for i in keras.__version__.split(".")[:2])
-if _version < (3, 0):
-    raise ImportError(f"einx.nn.keras requires Keras version >= 3, but found {keras.__version__}")
+import flax
+from functools import partial
+import jax.numpy as jnp
+from typing import Callable, Union, Optional, Any
+
+tnn = einx.tracer.import_("flax.linen", "nn")
+
+
+class ParamFactory:
+    class Concrete(einx.tracer.input.Input):
+        def __init__(self, module, name, init, dtype, col, param_type):
+            self.module = module
+            self.name = name
+            self.init = init
+
+            if dtype is None:
+                if hasattr(module, "dtype"):
+                    dtype = module.dtype
+                else:
+                    dtype = "float32"
+            self.dtype = dtype
+
+            self.col = col
+
+            if param_type == "param":
+                if col is not None:
+                    raise ValueError("col is not accepted for flax.linen.Module.param")
+            elif param_type == "variable":
+                if col is None:
+                    raise ValueError("col must be specified for flax.linen.Module.variable")
+            else:
+                raise ValueError(f"Unknown tensor factory flax.linen.Module.{param_type}")
+            self.param_type = param_type
+
+        def to_value_and_key(self):
+            return self.module, ParamFactory.CacheKey(
+                self.name, self.init, self.dtype, self.col, self.param_type
+            )
+
+    class CacheKey(einx.tracer.input.CacheKey):
+        def __init__(self, name, init, dtype, col, param_type):
+            self.name = name
+            self.init = init
+            self.dtype = dtype
+            self.col = col
+            self.param_type = param_type
+
+        def __hash__(self):
+            return hash((self.name, self.init, self.dtype, self.col, self.param_type))
+
+        def __eq__(self, other):
+            return (
+                isinstance(other, ParamFactory.CacheKey)
+                and self.name == other.name
+                and self.init == other.init
+                and self.dtype == other.dtype
+                and self.col == other.col
+                and self.param_type == other.param_type
+            )
+
+        def to_tracer(self, backend, virtual_arg):
+            x = ParamFactory.Tracer(self.name, self.init, self.dtype, self.col, self.param_type)
+            return x, x
+
+    class Tracer(einx.tracer.TensorFactory):
+        def __init__(self, name, init, dtype, col, param_type):
+            self.name = name
+            self.init = init
+            self.dtype = dtype
+            self.col = col
+            self.param_type = param_type
+
+        def __call__(self, shape, kwargs):
+            name = self.name if not self.name is None else kwargs.get("name", None)
+            init = self.init if not self.init is None else kwargs.get("init", None)
+            dtype = self.dtype if not self.dtype is None else kwargs.get("dtype", None)
+            col = self.col
+
+            if name is None:
+                raise ValueError(
+                    "Must specify name for tensor factory flax.linen.Module.{param|variable}"
+                )
+
+            if init is None:
+                raise ValueError(
+                    "Must specify init for tensor factory flax.linen.Module.{param|variable}"
+                )
+            elif isinstance(init, str):
+                if init == "get_at" or init == "rearrange":
+                    init = tnn.initializers.normal(stddev=0.02)
+                elif init == "add":
+                    init = tnn.initializers.zeros_init()
+                elif init == "multiply":
+                    init = tnn.initializers.ones_init()
+                elif init == "dot":
+                    init = tnn.initializers.lecun_normal(
+                        kwargs["in_axis"], kwargs["out_axis"], kwargs["batch_axis"]
+                    )
+                else:
+                    raise ValueError(f"Don't know which initializer to use for operation '{init}'")
+            elif isinstance(init, (int, float)):
+                init = tnn.initializers.constant(init, dtype=dtype)
+
+            if self.param_type == "param":
+                x = einx.tracer.apply(
+                    self.param, args=[name, init, shape, dtype], output=einx.tracer.Tensor(shape)
+                )
+            else:
+                assert self.param_type == "variable"
+                # Assume that variable initialization does not need an rng key by passing None
+                x = einx.tracer.apply(
+                    self.variable,
+                    args=[col, name, init, None, shape, dtype],
+                )
+                x = einx.tracer.apply(
+                    einx.tracer.MemberAccess(), args=[x, "value"], output=einx.tracer.Tensor(shape)
+                )
+            return x
 
 
 def param(
-    layer: keras.layers.Layer,
+    x: Union[Callable, nn.Module],
     name: Optional[str] = None,
     init: Optional[Any] = None,
-    dtype: Optional[Any] = None,
-    trainable: bool = True,
+    dtype: Optional[nn.dtypes.Dtype] = None,
+    col: Optional[str] = None,
 ):
-    """Create a tensor factory for Keras parameters.
+    """Create a tensor factory for Flax parameters.
 
     Args:
-        layer: The layer to create the parameter in. Must be an instance of ``keras.layers.Layer``.
-        name: Name of the parameter. If ``None``, uses a default name determined from the
-            calling operation. Defaults to ``None``.
+        x: The bound method of a Flax module, i.e. ``nn.Module.param`` or
+            ``nn.Module.variable``, or a module instance in which case its ``param`` method
+            is used.
+        name: Name of the parameter. If ``None``, uses a default name determined from the calling
+            operation. Defaults to ``None``.
         init: Initializer for the parameter. If ``None``, uses a default init method determined
             from the calling operation. Defaults to ``None``.
         dtype: Data type of the parameter. If ``None``, uses the ``dtype`` member of the calling
             module or ``float32`` if it does not exist. Defaults to ``None``.
-        trainable: Whether the parameter is trainable. Defaults to ``True``.
+        col: The collection name to use when ``bound_method`` is ``nn.Module.variable``.
 
     Returns:
         A tensor factory with the given default parameters.
     """
+    if hasattr(x, "__func__") and x.__func__ == nn.Module.param:
+        module = x.__self__
+        param_type = "param"
+    elif hasattr(x, "__func__") and x.__func__ == nn.Module.variable:
+        module = x.__self__
+        param_type = "variable"
+    elif isinstance(x, nn.Module):
+        module = x
+        param_type = "param"
+    else:
+        raise ValueError("x must be a bound method of a Flax module or a Flax module instance")
+
+    return ParamFactory.Concrete(module, name, init, dtype, col, param_type)
+
+
+# Allow passing nn.Module, nn.Module.param, nn.Module.variable as tensor factory:
+@einx.tracer.input.register_tensor_factory
+def tensor_factory(x):
+    if isinstance(x, nn.Module) or (
+        hasattr(x, "__func__")
+        and (x.__func__ == nn.Module.param or x.__func__ == nn.Module.variable)
+    ):
+        return param(x).to_value_and_key()
+    else:
+        return None
+
+
+# Using _ prefix on classes and a separater constructor, since dataclass/nn.Module does
+# not support **kwargs parameter.
+
+
+class _Norm(nn.Module):
+    stats: str
+    params: str = "b... [c]"
+    mean: bool = True
+    var: bool = True
+    scale: bool = True
+    bias: bool = True
+    decay_rate: float = None
+    epsilon: float = 1e-5
+    fastvar: bool = True
+    dtype: nn.dtypes.Dtype = "float32"
+    kwargs: dict = None
+
+    @nn.compact
+    def __call__(self, x, training=None):
+        if self.decay_rate is not None and training is None:
+            raise ValueError("training must be specified when decay_rate is used")
 
-    name0 = name
-    init0 = init
-    dtype0 = dtype
-
-    def keras_param_factory(shape, name=name, dtype=dtype, init=init, **kwargs):
-        if name0 is not None:
-            name = name0
-        if init0 is not None:
-            init = init0
-        if dtype0 is not None:
-            dtype = dtype0
-
-        if name is None:
-            raise ValueError("Must specify name for tensor factory keras.layers.Layer")
-
-        if dtype is None:
-            if hasattr(layer, "dtype"):
-                dtype = layer.dtype
-            else:
-                dtype = "float32"
-
-        if init is None:
-            raise ValueError("Must specify init for tensor factory keras.layers.Layer")
-        elif isinstance(init, str):
-            if init == "get_at" or init == "rearrange":
-                init = keras.initializers.TruncatedNormal(stddev=0.02)
-            elif init == "add":
-                init = keras.initializers.Constant(0.0)
-            elif init == "multiply":
-                init = keras.initializers.Constant(1.0)
-            elif init == "dot":
-                fan_in = np.prod([shape[i] for i in kwargs["in_axis"]])
-                std = np.sqrt(1.0 / fan_in) / 0.87962566103423978
-                init = keras.initializers.TruncatedNormal(mean=0.0, stddev=std)
-            else:
-                raise ValueError(f"Don't know which initializer to use for operation '{init}'")
-        elif isinstance(init, (int, float)):
-            init = keras.initializers.Constant(init)
-
-        if name in vars(layer):
-            tensor = vars(layer)[name]
-        else:
-            tensor = vars(layer)[name] = layer.add_weight(
-                shape=shape,
-                dtype=dtype,
-                initializer=init,
-                name=name,
-                trainable=trainable,
-            )
-        return tensor
-
-    return keras_param_factory
-
-
-def to_tensor_factory(x):
-    return None
-
-
-def einx_backend_for_keras():
-    return einx.backend.get(keras.config.backend())
-
-
-def is_leaf(x):
-    return isinstance(x, tuple) and all(isinstance(y, int) for y in x)
-
-
-class Layer(keras.layers.Layer):
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
-
-    def build(self, inputs_shape):
-        backend = einx_backend_for_keras()
-        tracers = einx.tree_util.tree_map(
-            lambda shape: backend.zeros(shape=shape, dtype="float32"), inputs_shape, is_leaf=is_leaf
+        use_ema = self.decay_rate is not None and (not training or self.is_initializing())
+        x, mean, var = einx.nn.norm(
+            x,
+            self.stats,
+            self.params,
+            mean=param(self.variable, col="stats", name="mean", dtype=self.dtype)
+            if use_ema and self.mean
+            else self.mean,
+            var=param(self.variable, col="stats", name="var", dtype=self.dtype)
+            if use_ema and self.var
+            else self.var,
+            scale=param(self.param, name="scale", dtype=self.dtype) if self.scale else None,
+            bias=param(self.param, name="bias", dtype=self.dtype) if self.bias else None,
+            epsilon=self.epsilon,
+            fastvar=self.fastvar,
+            **(self.kwargs if self.kwargs is not None else {}),
         )
 
-        if "is_initializing" in inspect.signature(self.call).parameters:
-            self.call(tracers, is_initializing=True)
-        else:
-            self.call(tracers)
+        update_ema = self.decay_rate is not None and training and not self.is_initializing()
+        if update_ema:
+            if self.mean:
+                mean_ema = self.variable("stats", "mean", None)
+                mean_ema.value = self.decay_rate * mean_ema.value + (1 - self.decay_rate) * mean
+            if self.var:
+                var_ema = self.variable("stats", "var", None)
+                var_ema.value = self.decay_rate * var_ema.value + (1 - self.decay_rate) * var
 
+        return x
 
-class Norm(Layer):
+
+def Norm(
+    stats: str,
+    params: str = "b... [c]",
+    mean: bool = True,
+    var: bool = True,
+    scale: bool = True,
+    bias: bool = True,
+    decay_rate: Optional[float] = None,
+    epsilon: float = 1e-5,
+    fastvar: bool = True,
+    dtype: nn.dtypes.Dtype = "float32",
+    name: Optional[str] = None,
+    **kwargs: Any,
+):
     """Normalization layer.
 
     Args:
         stats: Einstein string determining the axes along which mean and variance are computed.
             Will be passed to ``einx.reduce``.
         params: Einstein string determining the axes along which learnable parameters are applied.
             Will be passed to ``einx.elementwise``. Defaults to ``"b... [c]"``.
@@ -128,130 +250,105 @@
         bias: Whether to apply a learnable bias according to ``params``. Defaults to ``True``.
         epsilon: A small float added to the variance to avoid division by zero. Defaults
             to ``1e-5``.
         fastvar: Whether to use a fast variance computation. Defaults to ``True``.
         dtype: Data type of the weights. Defaults to ``"float32"``.
         decay_rate: Decay rate for exponential moving average of mean and variance. If ``None``,
             no moving average is applied. Defaults to ``None``.
+        name: Name of the module. Defaults to ``None``.
         **kwargs: Additional parameters that specify values for single axes, e.g. ``a=4``.
     """
 
-    def __init__(
-        self,
-        stats: str,
-        params: str = "b... [c]",
-        mean: bool = True,
-        var: bool = True,
-        scale: bool = True,
-        bias: bool = True,
-        epsilon: float = 1e-5,
-        fastvar: bool = True,
-        dtype: Any = "float32",
-        decay_rate: Optional[float] = None,
-        **kwargs: Any,
-    ):
-        super().__init__(dtype=dtype)
-        self.stats = stats
-        self.params = params
-        self.use_mean = mean
-        self.use_var = var
-        self.use_scale = scale
-        self.use_bias = bias
-        self.epsilon = epsilon
-        self.fastvar = fastvar
-        self.decay_rate = decay_rate
-        self.kwargs = kwargs
+    return _Norm(
+        stats,
+        params=params,
+        mean=mean,
+        var=var,
+        scale=scale,
+        bias=bias,
+        decay_rate=decay_rate,
+        epsilon=epsilon,
+        fastvar=fastvar,
+        dtype=dtype,
+        name=name,
+        kwargs=kwargs,
+    )
+
+
+class _Linear(nn.Module):
+    expr: str
+    bias: bool = True
+    dtype: nn.dtypes.Dtype = "float32"
+    kwargs: dict = None
 
-    def call(self, x, training=None, is_initializing=False):
-        use_ema = self.decay_rate is not None and (not training or is_initializing)
-        x, mean, var = einx.nn.norm(
+    @nn.compact
+    def __call__(self, x):
+        return einx.nn.linear(
             x,
-            self.stats,
-            self.params,
-            mean=param(self, name="mean", trainable=False)
-            if use_ema and self.use_mean
-            else self.use_mean,
-            var=param(self, name="var", trainable=False)
-            if use_ema and self.use_var
-            else self.use_var,
-            scale=param(self, name="scale", trainable=True) if self.use_scale else None,
-            bias=param(self, name="bias", trainable=True) if self.use_bias else None,
-            epsilon=self.epsilon,
-            fastvar=self.fastvar,
+            self.expr,
+            bias=param(self.param, name="bias", dtype=self.dtype) if self.bias else None,
+            weight=param(self.param, name="weight", dtype=self.dtype),
             **(self.kwargs if self.kwargs is not None else {}),
         )
 
-        update_ema = self.decay_rate is not None and training and not is_initializing
-        if update_ema:
-            if self.use_mean:
-                self.mean.assign(
-                    keras.ops.cast(
-                        self.decay_rate * self.mean.value + (1 - self.decay_rate) * mean,
-                        self.mean.dtype,
-                    )
-                )
-            if self.use_var:
-                self.var.assign(
-                    keras.ops.cast(
-                        self.decay_rate * self.var.value + (1 - self.decay_rate) * var,
-                        self.var.dtype,
-                    )
-                )
-
-        return x
-
 
-class Linear(Layer):
+def Linear(
+    expr: str,
+    bias: bool = True,
+    dtype: nn.dtypes.Dtype = "float32",
+    name: Optional[str] = None,
+    **kwargs: Any,
+):
     """Linear layer.
 
     Args:
-        expr: Einstein string determining the axes along which the weight matrix is multiplied.
-            Will be passed to ``einx.dot``.
+        expr: Einstein string determining the axes along which the weight matrix is
+            multiplied. Will be passed to ``einx.dot``.
         bias: Whether to apply a learnable bias. Defaults to ``True``.
         dtype: Data type of the weights. Defaults to ``"float32"``.
+        name: Name of the module. Defaults to ``None``.
         **kwargs: Additional parameters that specify values for single axes, e.g. ``a=4``.
     """
 
-    def __init__(self, expr: str, bias: bool = True, dtype: Any = "float32", **kwargs: Any):
-        super().__init__(dtype=dtype)
-
-        self.expr = expr
-        self.use_bias = bias
-        self.kwargs = kwargs
-
-    def call(self, x):
-        return einx.nn.linear(
-            x,
-            self.expr,
-            bias=param(self, name="bias") if self.use_bias else None,
-            weight=param(self, name="weight"),
-            **self.kwargs,
-        )
-
-
-class Dropout(Layer):
-    """Dropout layer.
-
-    Args:
-        expr: Einstein string determining the axes along which dropout is applied. Will be
-            passed to ``einx.elementwise``.
-        drop_rate: Drop rate.
-        **kwargs: Additional parameters that specify values for single axes, e.g. ``a=4``.
-    """
+    return _Linear(expr, bias=bias, dtype=dtype, name=name, kwargs=kwargs)
 
-    def __init__(self, expr: str, drop_rate: float, **kwargs: Any):
-        super().__init__()
 
-        self.expr = expr
-        self.drop_rate = drop_rate
-        self.kwargs = kwargs
+class _Dropout(nn.Module):
+    expr: str
+    drop_rate: float
+    rng_collection: str = "dropout"
+    kwargs: dict = None
 
-    def call(self, x, training=None):
+    @nn.compact
+    def __call__(self, x, training):
         if training:
             return einx.nn.dropout(
                 x,
                 self.expr,
                 drop_rate=self.drop_rate,
-                **self.kwargs,
+                rng=self.make_rng(self.rng_collection),
+                **(self.kwargs if self.kwargs is not None else {}),
             )
         else:
             return x
+
+
+def Dropout(
+    expr: str,
+    drop_rate: float,
+    rng_collection: str = "dropout",
+    name: Optional[str] = None,
+    **kwargs: Any,
+):
+    """Dropout layer.
+
+    Args:
+        expr: Einstein string determining the axes along which dropout is applied. Will be passed
+            to ``einx.elementwise``.
+        drop_rate: Drop rate.
+        rng_collection: the rng collection name to use when requesting an rng key. Defaults
+            to ``"dropout"``.
+        name: Name of the module. Defaults to ``None``.
+        **kwargs: Additional parameters that specify values for single axes, e.g. ``a=4``.
+    """
+
+    return _Dropout(expr, drop_rate, rng_collection=rng_collection, name=name, kwargs=kwargs)
```

### Comparing `einx-0.2.0/einx/nn/nn.py` & `einx-0.2.1/einx/nn/nn.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import einx
 from typing import Union, Optional, Any
 
 
-@einx.lru_cache(
+@einx.jit(
     trace=lambda t, c: lambda x,
     stats,
     params="b... [c]",
     mean=True,
     var=True,
     scale=None,
     bias=None,
@@ -37,113 +37,122 @@
     epsilon: float = 0,
     fastvar: bool = True,
     backend: Union[einx.Backend, str, None] = None,
     **kwargs: Any,
 ):
     if mean is None or var is None:
         raise ValueError("mean and var cannot be None")
-    if backend is None:
-        backend = einx.backend.get([
-            x,
-            mean if not isinstance(mean, bool) else None,
-            var if not isinstance(var, bool) else None,
-            scale,
-            bias,
-        ])
-    elif isinstance(backend, str):
-        backend = einx.backend.get(backend)
 
-    expr_in, expr_stats = einx.reduce.parse(stats, einx.param.get_shape(x), **kwargs)
+    expr_in, expr_stats = einx.reduce.parse(stats, einx.tracer.get_shape(x), **kwargs)
     expr_in = einx.expr.stage3.demark(expr_in)
     expr_stats = einx.expr.stage3.demark(expr_stats)
 
     # Instantiate moving averages
     if not isinstance(mean, bool) and mean is not None:
-        mean = einx.param.instantiate(mean, shape=expr_stats.shape, backend=backend, init="add")
+        mean = einx.tracer.call_factory(mean, shape=expr_stats.shape, backend=backend, init="add")
     if not isinstance(var, bool) and var is not None:
-        var = einx.param.instantiate(var, shape=expr_stats.shape, backend=backend, init="multiply")
+        var = einx.tracer.call_factory(
+            var, shape=expr_stats.shape, backend=backend, init="multiply"
+        )
 
     # Compute mean and variance
     if isinstance(mean, bool):
         if mean:
-            mean = einx.mean(stats, x, **kwargs)
+            mean = einx.mean(stats, x, backend=backend, **kwargs)
         else:
             mean = None
     if isinstance(var, bool):
         if var:
             if mean is None:
                 # RMS norm
-                var = einx.mean(stats, backend.square(x), **kwargs)
+                var = einx.mean(stats, backend.square(x), backend=backend, **kwargs)
             else:
                 if fastvar:
-                    mean_of_squares = einx.mean(stats, backend.square(x), **kwargs)
+                    mean_of_squares = einx.mean(stats, backend.square(x), backend=backend, **kwargs)
                     var = mean_of_squares - backend.square(mean)
                     var = backend.maximum(var, 0)
                 else:
-                    var = einx.var(stats, x, **kwargs)
+                    var = einx.var(stats, x, backend=backend, **kwargs)
         else:
             var = None
 
     # Normalize mean and variance
     if mean is not None:
-        x, _ = einx.subtract_stage3([expr_in, expr_stats], [x, mean], expr_in)
+        x, _ = einx.subtract_stage3([expr_in, expr_stats], [x, mean], expr_in, backend=backend)
     if var is not None:
         inv_std = backend.rsqrt(var + epsilon)
-        x, _ = einx.multiply_stage3([expr_in, expr_stats], [x, inv_std], expr_in)
+        x, _ = einx.multiply_stage3([expr_in, expr_stats], [x, inv_std], expr_in, backend=backend)
 
     # Apply scale and bias
     if scale is not None:
-        x = einx.multiply(params, x, scale, **kwargs)
+        x = einx.multiply(params, x, scale, backend=backend, **kwargs)
     if bias is not None:
-        x = einx.add(params, x, bias, **kwargs)
+        x = einx.add(params, x, bias, backend=backend, **kwargs)
 
     return x, mean, var
 
 
-@einx.lru_cache(
+@einx.jit(
     trace=lambda t, c: lambda x, expr, weight, bias=None, **kwargs: c(
         t(x), expr, t(weight), t(bias) if bias is not None else None, **kwargs
     )
 )
 def linear(
-    x: einx.Tensor, expr: str, weight: einx.Tensor, bias: Optional[einx.Tensor], **kwargs: Any
+    x: einx.Tensor,
+    expr: str,
+    weight: einx.Tensor,
+    bias: Optional[einx.Tensor],
+    backend: Union[einx.Backend, str, None] = None,
+    **kwargs: Any,
 ):
     (_expr_in1, expr_in2), expr_afterdot = einx.dot.parse(
-        expr, einx.param.get_shape(x), einx.param.get_shape(weight), **kwargs
+        expr, einx.tracer.get_shape(x), einx.tracer.get_shape(weight), **kwargs
     )
 
     # Weight matrix multiplication
-    x = einx.dot(expr, x, weight, **kwargs)
+    x = einx.dot(expr, x, weight, backend=backend, **kwargs)
 
     if bias is not None:
         # Bias expression includes all axes in output that are also in weight matrix
         weight_axes_names = {a.name for a in expr_in2.all() if isinstance(a, einx.expr.stage3.Axis)}
         expr_bias = []
         for a in expr_afterdot.all():
             if isinstance(a, einx.expr.stage3.Axis) and a.name in weight_axes_names:
                 expr_bias.append(a.__deepcopy__())
         expr_bias = einx.expr.stage3.List(expr_bias)
 
-        x, _ = einx.add_stage3([expr_afterdot, expr_bias], [x, bias], expr_afterdot)
+        x, _ = einx.add_stage3(
+            [expr_afterdot, expr_bias], [x, bias], expr_afterdot, backend=backend
+        )
 
     return x
 
 
-@einx.lru_cache(
+@einx.jit(
     trace=lambda t, c: lambda x, expr, drop_rate, rng=None, **kwargs: c(
         t(x), expr, drop_rate, t(rng) if rng is not None else None, **kwargs
     )
 )
-def dropout(x: einx.Tensor, expr: str, drop_rate: float, rng: Any = None, **kwargs: Any):
-    backend = einx.backend.get([x])
+def dropout(
+    x: einx.Tensor,
+    expr: str,
+    drop_rate: float,
+    rng: Any = None,
+    backend: Union[einx.Backend, str, None] = None,
+    **kwargs: Any,
+):
     keep_rate = 1 - drop_rate
 
     (expr_in, expr_mask), expr_out = einx.elementwise.parse(
-        expr, einx.param.get_shape(x), None, **kwargs
+        expr, einx.tracer.get_shape(x), None, **kwargs
     )
 
-    drop_mask = backend.random.bernoulli(rng=rng, p=keep_rate, shape=expr_mask.shape)
-    x, _ = einx.where_stage3(
-        [expr_mask, expr_in, einx.expr.stage3.List([])], [drop_mask, x, 0], expr_out
-    )
+    with einx.tracer.depend_on(x):
+        drop_mask = backend.random.bernoulli(rng=rng, p=keep_rate, shape=expr_mask.shape)
+        x, _ = einx.where_stage3(
+            [expr_mask, expr_in, einx.expr.stage3.List([])],
+            [drop_mask, x, 0],
+            expr_out,
+            backend=backend,
+        )
 
-    return x / keep_rate
+    return x * (1 / keep_rate)
```

### Comparing `einx-0.2.0/einx/nn/torch.py` & `einx-0.2.1/einx/nn/torch.py`

 * *Files 17% similar despite different names*

```diff
@@ -15,75 +15,129 @@
         return torch.compiler.allow_in_graph(func)
     else:
         import torch._dynamo as _dynamo
 
         return _dynamo.allow_in_graph(func)
 
 
+ttorch = einx.tracer.import_("torch")
+
+
+class ParamFactory:
+    class Concrete(einx.tracer.input.Input):
+        def __init__(self, param, init):
+            self.param = param
+            self.init = init
+
+        def to_value_and_key(self):
+            return self.param, ParamFactory.CacheKey(self.init)
+
+    class CacheKey(einx.tracer.input.CacheKey):
+        def __init__(self, init):
+            self.init = init
+
+        def __hash__(self):
+            return hash(self.init)
+
+        def __eq__(self, other):
+            return isinstance(other, ParamFactory.CacheKey) and self.init == other.init
+
+        def to_tracer(self, backend, virtual_arg):
+            x = ParamFactory.Tracer(self.init)
+            return x, x
+
+    class Tracer(einx.tracer.TensorFactory):
+        def __init__(self, init):
+            self.init = init
+
+        def __call__(self, shape, kwargs):
+            init = self.init if not self.init is None else kwargs.get("init", None)
+
+            x = self
+
+            output = einx.tracer.Tensor(shape)
+            x = einx.tracer.apply(
+                x.materialize,
+                args=[shape],
+                output=output,
+                inplace_updates=[(x, output)],
+            )
+
+            if init is None:
+                raise ValueError(
+                    "Must specify init for tensor factory torch.nn.parameter.Uninitialized*"
+                )
+            elif isinstance(init, str):
+                if init == "get_at" or init == "rearrange":
+                    init = partial(ttorch.nn.init.normal_, std=0.02)
+                elif init == "add":
+                    init = ttorch.nn.init.zeros_
+                elif init == "multiply":
+                    init = ttorch.nn.init.ones_
+                elif init == "dot":
+                    fan_in = np.prod([shape[i] for i in kwargs["in_axis"]])
+                    std = np.sqrt(1.0 / fan_in) / 0.87962566103423978
+                    init = partial(ttorch.nn.init.trunc_normal_, mean=0.0, std=std, a=-2.0, b=2.0)
+                else:
+                    raise ValueError(f"Don't know which initializer to use for operation '{init}'")
+            elif isinstance(init, (int, float)):
+                init = partial(ttorch.nn.init.constant_, val=init)
+
+            output = einx.tracer.Tensor(shape)
+            x = einx.tracer.apply(
+                init,
+                args=[x],
+                output=output,
+                inplace_updates=[(x, output)],
+            )
+
+            return x
+
+
 def param(
-    uninitialized: Union[
-        torch.nn.parameter.UninitializedParameter, torch.nn.parameter.UninitializedBuffer
+    x: Union[
+        torch.nn.parameter.UninitializedParameter,
+        torch.nn.parameter.UninitializedBuffer,
+        torch.nn.parameter.Parameter,
     ],
     init: Optional[Any] = None,
 ):
     """Create a tensor factory for an uninitialized PyTorch parameter or buffer.
 
-    When the tensor factory is invoked, it calls the ``materialize`` method of ``uninitialized``
-        with the given shape and returns ``uninitialized``.
+    If the given parameter is not initialized, this returns a tensor factory that calls
+    the ``materialize`` method of ``uninitialized`` with the given shape and returns
+    ``uninitialized``. Otherwise, the parameter is returned as is.
 
     Args:
-        uninitialized: An instance of either ``torch.nn.parameter.UninitializedParameter`` or
-            ``torch.nn.parameter.UninitializedBuffer``.
+        x: An instance of ``torch.nn.parameter.UninitializedParameter``,
+            ``torch.nn.parameter.UninitializedBuffer`` or ``torch.nn.parameter.Parameter``.
         init: Initializer for the parameter. If ``None``, uses a default init method determined
             from the calling operation. Defaults to ``None``.
 
     Returns:
-        A tensor factory with the given default parameters.
+        A tensor factory with the given default parameters, or the parameter itself if it is
+        already materialized.
     """
-
-    init0 = init
-
-    def torch_param_factory(shape, init=init, **kwargs):
-        if init0 is not None:
-            init = init0
-
-        if init is None:
-            raise ValueError(
-                "Must specify init for tensor factory torch.nn.parameter.Uninitialized*"
-            )
-        elif isinstance(init, str):
-            if init == "get_at" or init == "rearrange":
-                init = partial(torch.nn.init.normal_, std=0.02)
-            elif init == "add":
-                init = torch.nn.init.zeros_
-            elif init == "multiply":
-                init = torch.nn.init.ones_
-            elif init == "dot":
-                fan_in = np.prod([shape[i] for i in kwargs["in_axis"]])
-                std = np.sqrt(1.0 / fan_in) / 0.87962566103423978
-                init = partial(torch.nn.init.trunc_normal_, mean=0.0, std=std, a=-2.0, b=2.0)
-            else:
-                raise ValueError(f"Don't know which initializer to use for operation '{init}'")
-        elif isinstance(init, (int, float)):
-            init = partial(torch.nn.init.constant_, val=init)
-
-        with torch.no_grad():
-            uninitialized.materialize(shape)
-            init(uninitialized)
-
-        return uninitialized
-
-    return torch_param_factory
+    if isinstance(
+        x, (torch.nn.parameter.UninitializedParameter, torch.nn.parameter.UninitializedBuffer)
+    ) and not isinstance(x, torch._subclasses.FakeTensor):
+        # Return
+        return ParamFactory.Concrete(x, init)
+    else:
+        # If parameter is already materialized, return it as is
+        return x
 
 
-def to_tensor_factory(x):
+# Allow passing UninitializedParameter and UninitializedBuffer as tensor factory:
+@einx.tracer.input.register_tensor_factory
+def tensor_factory(x):
     if isinstance(
         x, (torch.nn.parameter.UninitializedParameter, torch.nn.parameter.UninitializedBuffer)
     ) and not isinstance(x, torch._subclasses.FakeTensor):
-        return param(x)
+        return param(x).to_value_and_key()
     else:
         return None
 
 
 class Norm(torch.nn.Module):
     """Normalization layer.
```

### Comparing `einx-0.2.0/einx/op/arange.py` & `einx-0.2.1/einx/op/arange.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from functools import partial
 from . import util
 import numpy as np
 from typing import Union
 import numpy.typing as npt
 
 
-@einx.lru_cache(
+@einx.jit(
     trace=lambda t, c: lambda exprs_in, expr_out, backend=None, dtype="int32": c(
         exprs_in, expr_out, dtype=dtype
     )
 )
 def arange_stage3(expr_in, expr_out, backend, dtype="int32"):
     if isinstance(backend, str):
         backend = einx.backend.get(backend)
@@ -45,14 +45,15 @@
     expr_out_flat_withconcat = einx.expr.stage3.replace(expr_out_flat, replace)
     expr_out_flat_withconcat = einx.expr.stage3.demark(expr_out_flat_withconcat)
 
     (tensor,), _ = einx.rearrange_stage3(
         [axis.__deepcopy__() for axis in expr_in],
         [backend.arange(axis.value, dtype=dtype) for axis in expr_in],
         [expr_out_flat_withconcat],
+        backend=backend,
     )
 
     # Unflatten output expressions
     (tensor,) = util.unflatten(
         [expr_out_flat],
         [
             tensor,
@@ -112,17 +113,15 @@
         after_stage2=after_stage2,
     )[:2]
 
     return expr_in, expr_out
 
 
 @einx.traceback_util.filter
-@einx.lru_cache(
-    trace=lambda t, c: lambda description, backend=None, **kwargs: c(description, **kwargs)
-)
+@einx.jit(trace=lambda t, c: lambda description, backend=None, **kwargs: c(description, **kwargs))
 def arange(
     description: str,
     *,
     backend: Union[einx.Backend, str],
     dtype: str = "int32",
     cse: bool = True,
     **parameters: npt.ArrayLike,
```

### Comparing `einx-0.2.0/einx/op/dot.py` & `einx-0.2.1/einx/op/dot.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,20 @@
 import einx
 from . import util
 import numpy as np
 from typing import Union
 import numpy.typing as npt
 
 
-@einx.lru_cache(
+@einx.jit(
     trace=lambda t, c: lambda exprs_in, tensors_in, expr_out, backend=None: c(
         exprs_in, [t(x) for x in tensors_in], expr_out
     )
 )
 def dot_stage3(exprs_in, tensors_in, expr_out, backend=None):
-    if backend is None:
-        backend = einx.backend.get(tensors_in)
-    elif isinstance(backend, str):
-        backend = einx.backend.get(backend)
     if any(isinstance(expr, einx.expr.stage3.Concatenation) for expr in expr_out.all()):
         raise ValueError("Output expression cannot contain concatenations")
     for root in list(exprs_in) + [expr_out]:
         for expr in root.all():
             if isinstance(expr, einx.expr.stage3.Marker):
                 raise ValueError("Marker is not allowed")
             if isinstance(expr, einx.expr.stage3.Concatenation):
@@ -55,19 +51,20 @@
         return {
             "in_axis": tuple(in_axis),
             "out_axis": tuple(out_axis),
             "batch_axis": tuple(batch_axis),
         }
 
     tensors_in = [
-        einx.param.instantiate(
+        einx.tracer.call_factory(
             tensor, expr.shape, backend, **get_fans(i), name="weight", init="dot"
         )
         for i, (tensor, expr) in enumerate(zip(tensors_in, exprs_in))
     ]
+    tensors_in = backend.all_to_tensor(tensors_in)
 
     # Flatten expressions
     exprs_in, tensors_in = util.flatten(exprs_in, tensors_in, backend=backend)
     expr_out_flat = util.flatten([expr_out])[0]
     assert all(einx.expr.stage3.is_flat(expr) for expr in exprs_in)
     assert einx.expr.stage3.is_flat(expr_out_flat)
 
@@ -104,17 +101,15 @@
         if a.name in input_axis_names
     ])
 
     # Transpose and broadcast missing output dimensions
     tensor = util.transpose_broadcast(expr, tensor, expr_out_flat, backend=backend)[0]
 
     # Unflatten output expression
-    assert tensor.shape is not None
-    if tensor.shape != expr_out.shape:
-        tensor = backend.reshape(tensor, expr_out.shape)
+    tensor = backend.reshape(tensor, expr_out.shape)
 
     return tensor, expr_out
 
 
 @einx.lru_cache
 def parse(description, *tensor_shapes, cse=True, **parameters):
     description, parameters = einx.op.util._clean_description_and_parameters(
@@ -190,15 +185,15 @@
     )[: len(op[0]) + 1]
     exprs_in, expr_out = exprs[:-1], exprs[-1]
 
     return exprs_in, expr_out
 
 
 @einx.traceback_util.filter
-@einx.lru_cache(
+@einx.jit(
     trace=lambda t, c: lambda description, *tensors, backend=None, **kwargs: c(
         description, *[t(x) for x in tensors], **kwargs
     )
 )
 def dot(
     description: str,
     *tensors: einx.Tensor,
@@ -285,14 +280,14 @@
         ...         )
         ...     ),
         ... )
         >>> einx.dot("b... [c1->c2]", x, w).shape
         (4, 16, 16, 32)
     """
     exprs_in, expr_out = parse(
-        description, *[einx.param.get_shape(tensor) for tensor in tensors], cse=cse, **parameters
+        description, *[einx.tracer.get_shape(tensor) for tensor in tensors], cse=cse, **parameters
     )
     tensor, _expr = dot_stage3(exprs_in, tensors, expr_out, backend=backend)
     return tensor
 
 
 dot.parse = parse
```

### Comparing `einx-0.2.0/einx/op/elementwise.py` & `einx-0.2.1/einx/op/elementwise.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,24 +2,20 @@
 from . import util
 from functools import partial
 import numpy as np
 from typing import Callable, Union
 import numpy.typing as npt
 
 
-@einx.lru_cache(
+@einx.jit(
     trace=lambda t, c: lambda exprs_in, tensors_in, expr_out, op, backend=None: c(
         exprs_in, [t(x) for x in tensors_in], expr_out, op
     )
 )
 def elementwise_stage3(exprs_in, tensors_in, expr_out, op, backend=None):
-    if backend is None:
-        backend = einx.backend.get(tensors_in)
-    elif isinstance(backend, str):
-        backend = einx.backend.get(backend)
     for root in list(exprs_in) + [expr_out]:
         for expr in root.all():
             if isinstance(expr, einx.expr.stage3.Concatenation):
                 raise ValueError("Concatenation not allowed")
 
     assert not any(einx.expr.stage3.is_marked(expr) for root in exprs_in for expr in root.all())
     assert not any(einx.expr.stage3.is_marked(expr) for expr in expr_out.all())
@@ -30,23 +26,24 @@
             return "bias"
         elif s == "multiply":
             return "scale"
         else:
             return s
 
     tensors_in = [
-        einx.param.instantiate(
+        einx.tracer.call_factory(
             tensor,
             expr.shape,
             backend,
             name=get_name(util._op_to_str(op)),
             init=util._op_to_str(op),
         )
         for tensor, expr in zip(tensors_in, exprs_in)
     ]
+    tensors_in = backend.all_to_tensor(tensors_in)
 
     tensors_out, exprs_out = einx.vmap_with_axis_stage3(
         exprs_in, tensors_in, [expr_out], op, backend=backend
     )
     assert len(tensors_out) == 1 and len(exprs_out) == 1
     return tensors_out[0], exprs_out[0]
 
@@ -119,15 +116,15 @@
     )[: len(op[0]) + 1]
     exprs_in, expr_out = exprs[:-1], exprs[-1]
 
     return exprs_in, expr_out
 
 
 @einx.traceback_util.filter
-@einx.lru_cache(
+@einx.jit(
     trace=lambda t, c: lambda description, *tensors, backend=None, **kwargs: c(
         description, *[t(x) for x in tensors], **kwargs
     )
 )
 def elementwise(
     description: str,
     *tensors: einx.Tensor,
@@ -214,15 +211,15 @@
         ...     np.random.uniform(size=(4, 16, 16, 64)),
         ...     np.random.uniform(size=(64,)),
         ... )
         >>> einx.add("b... [c]", x, w).shape
         (4, 16, 16, 64)
     """
     exprs_in, expr_out = parse(
-        description, *[einx.param.get_shape(tensor) for tensor in tensors], cse=cse, **parameters
+        description, *[einx.tracer.get_shape(tensor) for tensor in tensors], cse=cse, **parameters
     )
     tensor, expr_out = elementwise_stage3(exprs_in, tensors, expr_out, op=op, backend=backend)
     return tensor
 
 
 elementwise.parse = parse
```

### Comparing `einx-0.2.0/einx/op/index.py` & `einx-0.2.1/einx/op/index.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,25 +60,20 @@
     return (
         op(tensor_in, tensor_coordinates)
         if not update
         else op(tensor_in, tensor_coordinates, tensor_update)
     )
 
 
-@einx.lru_cache(
+@einx.jit(
     trace=lambda t, c: lambda exprs_in, tensors_in, expr_out, **kwargs: c(
         exprs_in, [t(x) for x in tensors_in], expr_out, **kwargs
     )
 )
 def index_stage3(exprs_in, tensors_in, expr_out, *, update, op=None, backend=None):
-    if backend is None:
-        backend = einx.backend.get(tensors_in)
-    elif isinstance(backend, str):
-        backend = einx.backend.get(backend)
-    op = backend.op(op, tracable=False)
     if len(exprs_in) != len(tensors_in):
         raise ValueError(f"Expected {len(exprs_in)} input tensors, got {len(tensors_in)}")
     for expr in exprs_in[0]:
         if isinstance(expr, einx.expr.stage3.Axis) and expr.is_unnamed and expr.value == 1:
             raise ValueError("First expression cannot contain unnamed axes with value 1")
     for root in list(exprs_in) + [expr_out]:
         for expr in root.all():
@@ -107,23 +102,24 @@
     def get_name(s):
         if s == "get_at":
             return "embedding"
         else:
             return s
 
     tensors_in = [
-        einx.param.instantiate(
+        einx.tracer.call_factory(
             tensor,
             expr.shape,
             backend,
             name=get_name(util._op_to_str(op)),
             init=util._op_to_str(op),
         )
         for tensor, expr in zip(tensors_in, exprs_in)
     ]
+    tensors_in = backend.all_to_tensor(tensors_in)
 
     expr_tensor = exprs_in[0]
     exprs_coordinates = exprs_in[1:-1] if update else exprs_in[1:]
     if update:
         expr_update = exprs_in[-1]
 
     layout = []
@@ -244,24 +240,26 @@
                     axes_names.add(axis.name)
                     all_axes.append(axis)
         expr_common = einx.expr.stage3.List.maybe(all_axes)
     else:
         expr_common = einx.expr.stage3.get_marked(util.flatten([expr_out])[0])
 
     # Construct vmapped indexing function
+    if isinstance(op, str):
+        op = getattr(backend, op)
     op = partial(
         _index,
         op=op,
         update=update,
         layout=layout,
         expr_common=expr_common,
         expr_update_inner=expr_update_inner,
         backend=backend,
     )
-    op = backend.op(op, tracable=True)
+    op = einx.trace(op)
 
     exprs_in = [expr_tensor] + exprs_coordinates + ([expr_update] if update else [])
     tensors_out, exprs_out = einx.vmap_stage3(
         exprs_in, tensors_in, [expr_out], op=op, flat=True, backend=backend
     )
     assert len(tensors_out) == 1 and len(exprs_out) == 1
     return tensors_out[0], exprs_out[0]
@@ -366,20 +364,20 @@
                 f"{axes_in - axes_out}"
             )
 
     return exprs_in, expr_out
 
 
 def _has_zero_shape(tensor):
-    shape = einx.param.get_shape(tensor)
+    shape = einx.tracer.get_shape(tensor)
     return shape is not None and any(s == 0 for s in shape)
 
 
 @einx.traceback_util.filter
-@einx.lru_cache(
+@einx.jit(
     trace=lambda t, c: lambda description, *tensors, backend=None, **kwargs: c(
         description, *[t(x) for x in tensors], **kwargs
     )
 )
 def index(
     description: str,
     *tensors: einx.Tensor,
@@ -467,15 +465,15 @@
         (4, 128, 128, 3)
     """
     if update and any(_has_zero_shape(tensor) for tensor in tensors[1:]):
         # Skip update if no coordinates are given
         return tensors[0]
     exprs_in, expr_out = parse(
         description,
-        *[einx.param.get_shape(tensor) for tensor in tensors],
+        *[einx.tracer.get_shape(tensor) for tensor in tensors],
         update=update,
         cse=cse,
         **parameters,
     )
     tensor, expr_out = index_stage3(
         exprs_in, tensors, expr_out, op=op, update=update, backend=backend
     )
```

### Comparing `einx-0.2.0/einx/op/rearrange.py` & `einx-0.2.1/einx/op/rearrange.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,38 +1,35 @@
 import einx
 from . import util
 import numpy as np
 from typing import Union, Tuple
 import numpy.typing as npt
 
 
-@einx.lru_cache(
+@einx.jit(
     trace=lambda t, c: lambda exprs_in, tensors_in, exprs_out, backend=None: c(
         exprs_in, [t(x) for x in tensors_in], exprs_out
     )
 )
 def rearrange_stage3(exprs_in, tensors_in, exprs_out, backend=None):
-    if backend is None:
-        backend = einx.backend.get(tensors_in)
-    elif isinstance(backend, str):
-        backend = einx.backend.get(backend)
     if len(exprs_in) != len(tensors_in):
         raise ValueError(f"Expected {len(exprs_in)} input tensor(s), got {len(tensors_in)}")
     if any(
         isinstance(expr, einx.expr.stage3.Marker)
         for root in list(exprs_in) + list(exprs_out)
         for expr in root.all()
     ):
         raise ValueError(f"Marker '{expr}' is not allowed")
 
     # Call tensor factories
     tensors_in = [
-        einx.param.instantiate(tensor, expr.shape, backend, name="embedding", init="rearrange")
+        einx.tracer.call_factory(tensor, expr.shape, backend, name="embedding", init="rearrange")
         for tensor, expr in zip(tensors_in, exprs_in)
     ]
+    tensors_in = backend.all_to_tensor(tensors_in, convert_scalars=True)
 
     # Flatten expressions
     exprs_in, tensors_in = util.flatten(exprs_in, tensors_in, backend=backend)
     exprs_out_flat = util.flatten(exprs_out)
     assert all(einx.expr.stage3.is_flat(expr) for expr in exprs_in)
     assert all(einx.expr.stage3.is_flat(expr) for expr in exprs_out_flat)
     if len(exprs_in) != len(exprs_out_flat):
@@ -83,15 +80,15 @@
     )[: len(op[0]) + len(op[1])]
     exprs_in, exprs_out = exprs[: len(op[0])], exprs[len(op[0]) :]
 
     return exprs_in, exprs_out
 
 
 @einx.traceback_util.filter
-@einx.lru_cache(
+@einx.jit(
     trace=lambda t, c: lambda description, *tensors, backend=None, **kwargs: c(
         description, *[t(x) for x in tensors], **kwargs
     )
 )
 def rearrange(
     description: str,
     *tensors: einx.Tensor,
@@ -154,14 +151,14 @@
         Swap the first and last third of a tensor along a given axis:
 
         >>> x = np.arange(6)
         >>> einx.rearrange("(b + c + d) -> (d + c + b)", x, b=2, c=2)
         array([4, 5, 2, 3, 0, 1])
     """
     exprs_in, exprs_out = parse(
-        description, *[einx.param.get_shape(tensor) for tensor in tensors], cse=cse, **parameters
+        description, *[einx.tracer.get_shape(tensor) for tensor in tensors], cse=cse, **parameters
     )
     tensors, exprs_out = rearrange_stage3(exprs_in, tensors, exprs_out, backend=backend)
     return tensors[0] if len(exprs_out) == 1 else tensors
 
 
 rearrange.parse = parse
```

### Comparing `einx-0.2.0/einx/op/reduce.py` & `einx-0.2.1/einx/op/reduce.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from functools import partial
 from typing import Callable, Union
 import numpy.typing as npt
 
 _any = any  # Is overwritten below
 
 
-@einx.lru_cache(
+@einx.jit(
     trace=lambda t, c: lambda expr_in, tensor_in, expr_out, op, backend=None: c(
         expr_in, t(tensor_in), expr_out, op=op
     )
 )
 def reduce_stage3(expr_in, tensor_in, expr_out, op, backend=None):
     for root in [expr_in, expr_out]:
         for expr in root.all():
@@ -88,15 +88,15 @@
                 and expr.name not in axes_names_out,
             )
 
     return expr_in, expr_out
 
 
 @einx.traceback_util.filter
-@einx.lru_cache(
+@einx.jit(
     trace=lambda t, c: lambda description, tensor, backend=None, **kwargs: c(
         description, t(tensor), **kwargs
     )
 )
 def reduce(
     description: str,
     tensor: einx.Tensor,
@@ -172,15 +172,15 @@
         Compute variance per channel over an image:
 
         >>> x = np.random.uniform(size=(256, 256, 3))
         >>> einx.var("[...] c", x).shape
         (3,)
     """
     expr_in, expr_out = parse(
-        description, einx.param.get_shape(tensor), keepdims=keepdims, cse=cse, **parameters
+        description, einx.tracer.get_shape(tensor), keepdims=keepdims, cse=cse, **parameters
     )
     tensor, expr_out = reduce_stage3(expr_in, tensor, expr_out, op=op, backend=backend)
     return tensor
 
 
 reduce.parse = parse
```

### Comparing `einx-0.2.0/einx/op/solve.py` & `einx-0.2.1/einx/op/solve.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,15 +74,15 @@
 
     Examples:
         >>> x = np.zeros((10, 5))
         >>> einx.solve("a b", x)
         {'a': 10, 'b': 5}
     """
     return _solve(
-        description, *[einx.param.get_shape(tensor) for tensor in tensors], cse=cse, **parameters
+        description, *[einx.tracer.get_shape(tensor) for tensor in tensors], cse=cse, **parameters
     )
 
 
 def matches(
     description: str, *tensors: einx.Tensor, cse: bool = True, **parameters: npt.ArrayLike
 ) -> bool:
     """Check whether the given expressions and tensors match.
@@ -124,15 +124,15 @@
         description, parameters
     )
 
     exprs = einx.expr.stage1.parse_args(description)
     if len(exprs) != len(tensors):
         raise ValueError(f"Expected {len(exprs)} tensors, got {len(tensors)}")
 
-    tensor_shapes = [einx.param.get_shape(tensor) for tensor in tensors]
+    tensor_shapes = [einx.tracer.get_shape(tensor) for tensor in tensors]
     einx.expr.solve(
         [einx.expr.Equation(expr, tensor_shape) for expr, tensor_shape in zip(exprs, tensor_shapes)]
         + [
             einx.expr.Equation(k, np.asarray(v)[..., np.newaxis], depth1=None, depth2=None)
             for k, v in parameters.items()
         ],
         cse=cse,
```

### Comparing `einx-0.2.0/einx/op/util.py` & `einx-0.2.1/einx/op/util.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,16 +9,15 @@
     Flattening removes all compositions and concatenations and returns a list of new expressions
     (and optinally a list of flattened tensors).
 
     Parameters:
         exprs: Expressions to flatten.
         tensors: Tensors corresponding to ``exprs``. If None, flattens and returns only
             ``exprs``. Defaults to None.
-        backend: Backend to use for tensor operations. If None, determines backend from
-            ``tensors``. Defaults to None.
+        backend: Backend to use for tensor operations.
 
     Returns:
         exprs: The flattened expressions.
         tensors, optional: The flattened tensors. Only returned if ``tensors`` is not None.
     """
     if tensors is None:
         exprs_out = []
@@ -51,17 +50,15 @@
         if len(exprs) != len(tensors):
             raise ValueError("Got different number of expressions and tensors")
         exprs_out = []
         tensors_out = []
         for expr, tensor in zip(exprs, tensors):
             expr = einx.expr.stage3.decompose(expr)
             expr = einx.expr.stage3.remove_unnamed_trivial_axes(expr)
-            assert tensor.shape is not None
-            if tensor.shape != expr.shape:
-                tensor = backend.reshape(tensor, expr.shape)
+            tensor = backend.reshape(tensor, expr.shape)
 
             if any(isinstance(e, einx.expr.stage3.Concatenation) for e in expr):
                 concat_index, concat_expr = [
                     (i, e)
                     for i, e in enumerate(expr)
                     if isinstance(e, einx.expr.stage3.Concatenation)
                 ][0]
@@ -153,27 +150,24 @@
     out_axes = [a.name for a in einx.expr.stage3.get_axes(expr_out)]
     out_axes_intersect = [a for a in out_axes if a in in_axes]
     out_axes_broadcast = [a for a in out_axes if a not in in_axes]
     if set(out_axes_intersect) != set(in_axes):
         raise RuntimeError("Found input axes that are not in output expression")  # TODO:
 
     perm = [in_axes.index(out_axis) for out_axis in out_axes_intersect]
-    if perm != list(range(len(perm))):
-        tensor = backend.transpose(tensor, tuple(perm))
+    tensor = backend.transpose(tensor, tuple(perm))
 
     # Expand and broadcast missing output dimensions if necessary
     if len(out_axes_broadcast) > 0:
         pre_broadcast_shape = tuple(
             1 if a.name in out_axes_broadcast else a.value
             for a in einx.expr.stage3.get_axes(expr_out)
         )
-        assert tensor.shape is not None
-        if tensor.shape != pre_broadcast_shape:
-            tensor = backend.reshape(tensor, pre_broadcast_shape)
-        if broadcast and tensor.shape != expr_out.shape:
+        tensor = backend.reshape(tensor, pre_broadcast_shape)
+        if broadcast:
             tensor = backend.broadcast_to(tensor, expr_out.shape)
 
     if not broadcast:
         expr_out = einx.expr.stage3.List([
             (axis if axis.name in in_axes else einx.expr.stage3.Axis(None, 1)) for axis in expr_out
         ])
     return tensor, expr_out
@@ -209,33 +203,30 @@
     else:
         next_expr_in = next(exprs_in)
         assert einx.expr.stage3.remove_unnamed_trivial_axes(
             einx.expr.stage3.decompose(expr_out)
         ) == einx.expr.stage3.remove_unnamed_trivial_axes(einx.expr.stage3.decompose(next_expr_in))
         tensor_out = next(tensors_in)
 
-    assert tensor_out.shape is not None
-    if tensor_out.shape != expr_out.shape:
-        tensor_out = backend.reshape(tensor_out, expr_out.shape)
+    tensor_out = backend.reshape(tensor_out, expr_out.shape)
 
     return tensor_out
 
 
 def unflatten(exprs_in, tensors_in, exprs_out, *, backend):
     if len(exprs_in) != len(tensors_in):
         raise ValueError("Got different number of input expressions and tensors")
-    if backend is None:
-        backend = einx.backend.get(tensors_in)
+    assert not backend is None
 
     iter_exprs_in = iter(exprs_in)
     iter_tensors_in = iter(tensors_in)
     tensors_out = []
     for expr_out in exprs_out:
         t = _unflatten(iter_exprs_in, iter_tensors_in, expr_out, backend)
-        assert t.shape == expr_out.shape
+        assert einx.tracer.get_shape(t) == expr_out.shape
         tensors_out.append(t)
 
     return tensors_out
 
 
 def _clean_parameter(k, v):
     try:
```

### Comparing `einx-0.2.0/einx/op/vmap.py` & `einx-0.2.1/einx/op/vmap.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 import einx
-import inspect
 import functools
 from . import util
 import numpy as np
 from typing import Callable, Union, Mapping
 import numpy.typing as npt
 
 
-@einx.lru_cache(
+@einx.jit(
     trace=lambda t, c: lambda exprs_in, tensors_in, exprs_out, **kwargs: c(
         exprs_in, [t(x) for x in tensors_in], exprs_out, **kwargs
     )
 )
 def vmap_stage3(
     exprs_in,
     tensors_in,
@@ -21,31 +20,27 @@
     backend=None,
     op=None,
     kwargs=None,
     verbose=False,
 ):
     if kwargs is None:
         kwargs = {}
-    if backend is None:
-        backend = einx.backend.get(tensors_in)
-    elif isinstance(backend, str):
-        backend = einx.backend.get(backend)
-    op = backend.op(op, tracable=False)
     if len(exprs_in) != len(tensors_in):
         raise ValueError(f"Expected {len(exprs_in)} input tensor(s), got {len(tensors_in)}")
     for root in list(exprs_in) + list(exprs_out):
         for expr in root.all():
             if isinstance(expr, einx.expr.stage3.Concatenation):
                 raise ValueError("Concatenation not allowed")
 
     # Call tensor factories
     tensors_in = [
-        einx.param.instantiate(tensor, expr.shape, backend=backend)
+        einx.tracer.call_factory(tensor, expr.shape, backend=backend)
         for tensor, expr in zip(tensors_in, exprs_in)
     ]
+    tensors_in = backend.all_to_tensor(tensors_in)
 
     if verbose:
         print("Expressions:")
         print("    IN:", [str(e) for e in exprs_in])
         print("    OUT:", [str(e) for e in exprs_out])
 
     # Flatten expressions
@@ -69,73 +64,97 @@
         print("Expressions used in op:")
         if not flat:
             print("    IN:", [str(e) for e in exprs_in_funcargs])
             print("    OUT:", [str(e) for e in exprs_out_funcargs])
         print("    IN_FLAT:", [str(e) for e in exprs_in_funcargs_flat])
         print("    OUT_FLAT:", [str(e) for e in exprs_out_funcargs_flat])
 
+    @einx.trace(args=[einx.tracer.Tensor(expr.shape) for expr in exprs_in_funcargs_flat])
     def op(*tensors_in_flat, op=op):
         if verbose:
-            print("Flat input tensors that arrived in op:", [str(a.shape) for a in tensors_in_flat])
+            print(
+                "Flat input tensors that arrived in op:",
+                [str(einx.tracer.get_shape(a)) for a in tensors_in_flat],
+            )
             print("Input types to vmapped function:", [type(t) for t in tensors_in_flat])
         assert len(tensors_in_flat) == len(exprs_in_funcargs_flat)
 
         if not flat:
             tensors_in = util.unflatten(
                 exprs_in_funcargs_flat, tensors_in_flat, exprs_in_funcargs, backend=backend
             )
             if verbose:
-                print("Unflattened input tensors in op:", [str(a.shape) for a in tensors_in])
+                print(
+                    "Unflattened input tensors in op:",
+                    [str(einx.tracer.get_shape(a)) for a in tensors_in],
+                )
             assert len(tensors_in) == len(exprs_in)
         else:
             tensors_in = tensors_in_flat
         exprs_out_expected = exprs_out_funcargs if not flat else exprs_out_funcargs_flat
 
-        output_shapes = [expr.shape for expr in exprs_out_expected]
-        if len(output_shapes) == 1:
-            output_shapes = output_shapes[0]
-        tensors_out = backend.apply(op, args=tensors_in, kwargs=kwargs, output_shapes=output_shapes)
+        if isinstance(op, str):
+            op = getattr(backend, op)
+        elif not isinstance(op, einx.tracer.Tracer):
+            concrete_op = op
+            op = lambda *args, **kwargs: einx.tracer.apply(
+                concrete_op,
+                args=args,
+                kwargs=kwargs,
+                output=[einx.tracer.Tensor(expr.shape) for expr in exprs_out_expected]
+                if len(exprs_out_expected) > 1
+                else einx.tracer.Tensor(exprs_out_expected[0].shape),
+            )
+
+        tensors_out = op(*tensors_in, **kwargs)
+
         if not isinstance(tensors_out, (tuple, list)):
             tensors_out = (tensors_out,)
         if len(tensors_out) != len(exprs_out_expected):
             raise ValueError(
                 f"Expected {len(exprs_out_expected)} output tensor(s) from vmapped "
                 f"function, but got {len(tensors_out)}"
             )
+        if any(not isinstance(t, einx.tracer.Tensor) for t in tensors_out):
+            # TODO: might also be int, float, etc?
+            raise ValueError(
+                f"Expected tensors from vmapped function, but got {[type(t) for t in tensors_out]}"
+            )
 
         if verbose:
             print("Unflattened output tensors in op:")
             for expr_out, tensor_out in zip(exprs_out_expected, tensors_out):
                 print("    ", expr_out, tensor_out.shape)
 
         for i, (expr_out, tensor_out) in enumerate(zip(exprs_out_expected, tensors_out)):
-            if tensor_out.shape != expr_out.shape:
+            if einx.tracer.get_shape(tensor_out) != expr_out.shape:
                 raise ValueError(
                     f"Expected output shape {expr_out.shape} from {i}-th (zero-based) "
-                    f"output of vmapped function, but got {tensor_out.shape}"
+                    f"output of vmapped function, but got {einx.tracer.get_shape(tensor_out)}"
                 )
 
         if not flat:
             exprs_out_funcargs_flat2, tensors_out = util.flatten(
                 exprs_out_funcargs, tensors_out, backend=backend
             )
 
             if verbose:
-                print("Flattened output tensors in op:", [str(a.shape) for a in tensors_out])
+                print(
+                    "Flattened output tensors in op:",
+                    [str(einx.tracer.get_shape(a)) for a in tensors_out],
+                )
             assert (
                 exprs_out_funcargs_flat2 == exprs_out_funcargs_flat
             ), f"{[str(s) for s in exprs_out_funcargs_flat2]} != "
             f"{[str(s) for s in exprs_out_funcargs_flat]}"
 
         if verbose:
             print("Returning types from vmapped function:", [type(t) for t in tensors_out])
         return tuple(tensors_out)
 
-    op = backend.op(op, tracable=True)
-
     axes_names_in = [[a.name for a in root] for root in exprs_in_flat]
     axes_names_in_set = {a.name for root in exprs_in_flat for a in root}
 
     def is_broadcast_axis(expr):
         return (
             isinstance(expr, einx.expr.stage3.Axis)
             and expr.name not in axes_names_in_set
@@ -232,19 +251,18 @@
             input_shapes=input_shapes,
             output_shapes=output_shapes,
         )
 
     # Apply op to tensors
     if verbose:
         print("\nSending shapes to backend.vmap:", [str(a.shape) for a in tensors_in])
-    tensors = backend.apply(
+    tensors = einx.tracer.apply(  # TODO: replace with tensors = op(*tensors_in)
         op,
         args=tensors_in,
-        kwargs={},
-        output_shapes=tuple(expr.shape for expr in exprs_out_flat_without_broadcast),
+        output=tuple(einx.tracer.Tensor(expr.shape) for expr in exprs_out_flat_without_broadcast),
     )
     if verbose:
         for tensor, expr in zip(tensors, exprs_out_flat_without_broadcast):
             print("Got overall flat tensor_out:", tensor.shape, expr)
 
     # Transpose and broadcast missing output dimensions
     tensors = [
@@ -252,20 +270,22 @@
         for expr_out_wb, tensor, expr_out in zip(
             exprs_out_flat_without_broadcast, tensors, exprs_out_flat
         )
     ]
     if verbose:
         print("Got overall transposed+broadcasted tensors_out:")
         for tensor, expr in zip(tensors, exprs_out_flat):
-            print("    ", tensor.shape, expr)
+            print("    ", einx.tracer.get_shape(tensor), expr)
 
     # Unflatten output expressions
     tensors = util.unflatten(exprs_out_flat, tensors, exprs_out, backend=backend)
     if verbose:
-        print("Got overall unflattened tensors_out:", [str(a.shape) for a in tensors])
+        print(
+            "Got overall unflattened tensors_out:", [str(einx.tracer.get_shape(a)) for a in tensors]
+        )
 
     return tensors, exprs_out
 
 
 @einx.lru_cache
 def parse(description, *tensor_shapes, cse=True, **parameters):
     description, parameters = einx.op.util._clean_description_and_parameters(
@@ -299,15 +319,15 @@
     )[: len(op[0]) + len(op[1])]
     exprs_in, exprs_out = exprs[: len(op[0])], exprs[len(op[0]) :]
 
     return exprs_in, exprs_out
 
 
 @einx.traceback_util.filter
-@einx.lru_cache(
+@einx.jit(
     trace=lambda t, c: lambda description, *tensors, **kwargs: c(
         description, *[t(x) for x in tensors], **kwargs
     )
 )
 def vmap(
     description: str,
     *tensors: einx.Tensor,
@@ -381,13 +401,13 @@
         ...     np.random.uniform(size=(5, 10)),
         ...     np.random.uniform(size=(10, 3)),
         ... )
         >>> einx.vmap("a [b], [b] c -> a c", x, y, op=np.dot).shape
         (5, 3)
     """
     exprs_in, exprs_out = parse(
-        description, *[einx.param.get_shape(tensor) for tensor in tensors], cse=cse, **parameters
+        description, *[einx.tracer.get_shape(tensor) for tensor in tensors], cse=cse, **parameters
     )
     tensors, exprs_out = vmap_stage3(
         exprs_in, tensors, exprs_out, flat=flat, backend=backend, op=op, kwargs=kwargs
     )
     return tensors[0] if len(exprs_out) == 1 else tensors
```

### Comparing `einx-0.2.0/einx/op/vmap_with_axis.py` & `einx-0.2.1/einx/op/vmap_with_axis.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,44 +4,42 @@
 from functools import partial
 from typing import Callable, Mapping, Union, Tuple
 import numpy.typing as npt
 
 _op_names = ["roll", "flip"]
 
 
-@einx.lru_cache(
+@einx.jit(
     trace=lambda t, c: lambda exprs_in, tensors_in, exprs_out, op, kwargs={}, backend=None: c(
         exprs_in, [t(x) for x in tensors_in], exprs_out, op, kwargs
     )
 )
 def vmap_with_axis_stage3(exprs_in, tensors_in, exprs_out, op, kwargs=None, backend=None):
     if kwargs is None:
         kwargs = {}
-    if backend is None:
-        backend = einx.backend.get(tensors_in)
-    elif isinstance(backend, str):
-        backend = einx.backend.get(backend)
-    op = backend.op(op, tracable=False)
     if len(exprs_in) != len(tensors_in):
         raise ValueError(f"Expected {len(exprs_in)} input tensor(s), got {len(tensors_in)}")
     if len(set(exprs_out)) != 1:
         raise ValueError("All output expressions must be the same")
     for root in list(exprs_in) + list(exprs_out):
         for expr in root.all():
             if isinstance(expr, einx.expr.stage3.Concatenation):
                 raise ValueError("Concatenation not allowed")
     if len(exprs_out) > 1:
         raise ValueError("Only one output tensor allowed")
+    if all(einx.tracer.is_scalar(tensor) for tensor in tensors_in):
+        raise ValueError("At least one input tensor must be a non-scalar")  # TODO: support this
     kwargs = {**kwargs}
 
     # Call tensor factories
     tensors_in = [
-        einx.param.instantiate(tensor, expr.shape, backend=backend)
+        einx.tracer.call_factory(tensor, expr.shape, backend=backend)
         for tensor, expr in zip(tensors_in, exprs_in)
     ]
+    tensors_in = backend.all_to_tensor(tensors_in)
 
     # Flatten expressions
     exprs_in, tensors_in = util.flatten(exprs_in, tensors_in, backend=backend)
     in_axis_names = {axis.name for expr in exprs_in for axis in expr}
 
     def is_broadcast_axis(expr):
         return isinstance(expr, einx.expr.stage3.Axis) and expr.name not in in_axis_names
@@ -86,26 +84,28 @@
     if transpose_first:
         # Transpose and insert trivial axes
         if marked_input_axes != marked_output_axes:
             raise ValueError(
                 "When using multiple input tensors the same axes must be marked in all tensors"
             )
         x = [
-            util.transpose_broadcast(
+            (tensor_in, expr_in)
+            if einx.tracer.is_scalar(tensor_in)
+            else util.transpose_broadcast(
                 expr_in,
                 tensor_in,
                 exprs_out_flat_without_broadcast[0],
                 broadcast=False,
                 backend=backend,
             )
             for expr_in, tensor_in in zip(exprs_in, tensors_in)
         ]
         tensors_in = [x[0] for x in x]
         exprs_in = [x[1] for x in x]
-        assert len({len(expr) for expr in exprs_in}) == 1
+        assert len({len(expr) for expr in exprs_in if len(expr) > 0}) == 1
         marked_input_axes = {
             axis.name
             for expr_in in exprs_in
             for axis in expr_in.all()
             if isinstance(axis, einx.expr.stage3.Axis) and einx.expr.stage3.is_marked(axis)
         }
         exprs_op_output = exprs_out_flat_without_broadcast
@@ -145,22 +145,29 @@
             for i in range(len(axes_in[0]))
             if any(axes_in[i].name in marked_input_axes for axes_in in axes_in)
         )
     if len(axis_indices) > 0:
         kwargs["axis"] = axis_indices if len(axis_indices) > 1 else axis_indices[0]
 
     # Apply operation
-    tensors_out = backend.apply(
-        op,
-        args=tensors_in,
-        kwargs=kwargs,
-        output_shapes=[expr.shape for expr in exprs_op_output]
-        if len(exprs_op_output) > 1
-        else exprs_op_output[0].shape,
-    )
+    if isinstance(op, str):
+        op = getattr(backend, op)
+    elif not isinstance(op, einx.tracer.Tracer):
+        concrete_op = op
+        op = lambda *args, **kwargs: einx.tracer.apply(
+            concrete_op,
+            args=args,
+            kwargs=kwargs,
+            output=[einx.tracer.Tensor(expr.shape) for expr in exprs_op_output]
+            if len(exprs_op_output) > 1
+            else einx.tracer.Tensor(exprs_op_output[0].shape),
+        )
+
+    tensors_out = op(*tensors_in, **kwargs)
+
     if not isinstance(tensors_out, (tuple, list)):
         tensors_out = (tensors_out,)
     if len(tensors_out) != len(exprs_out_flat_without_broadcast):
         raise ValueError(
             f"Expected {len(exprs_out_flat_without_broadcast)} output tensor(s), "
             f"got {len(tensors_out)}"
         )
@@ -210,15 +217,15 @@
     )[: len(op[0]) + len(op[1])]
     exprs_in, exprs_out = exprs[: len(op[0])], exprs[len(op[0]) :]
 
     return exprs_in, exprs_out
 
 
 @einx.traceback_util.filter
-@einx.lru_cache(
+@einx.jit(
     trace=lambda t, c: lambda description, *tensors, backend=None, **kwargs: c(
         description, *[t(x) for x in tensors], **kwargs
     )
 )
 def vmap_with_axis(
     description: str,
     *tensors: einx.Tensor,
@@ -280,15 +287,15 @@
         Compute sum along axis:
 
         >>> x = np.random.uniform(size=(16, 20))
         >>> einx.vmap_with_axis("a ([b] c) -> c a", x, op=np.sum, b=2).shape
         (16, 20)
     """
     exprs_in, exprs_out = parse(
-        description, *[einx.param.get_shape(tensor) for tensor in tensors], cse=cse, **parameters
+        description, *[einx.tracer.get_shape(tensor) for tensor in tensors], cse=cse, **parameters
     )
     tensors, exprs_out = vmap_with_axis_stage3(
         exprs_in, tensors, exprs_out, op=op, kwargs=kwargs, backend=backend
     )
     return tensors[0] if len(exprs_out) == 1 else tensors
```

### Comparing `einx-0.2.0/einx/traceback_util.py` & `einx-0.2.1/einx/traceback_util.py`

 * *Files identical despite different names*

### Comparing `einx-0.2.0/einx/tree_util.py` & `einx-0.2.1/einx/tree_util.py`

 * *Files identical despite different names*

### Comparing `einx-0.2.0/einx.egg-info/PKG-INFO` & `einx-0.2.1/einx.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,29 @@
 Metadata-Version: 2.1
 Name: einx
-Version: 0.2.0
+Version: 0.2.1
 Summary: Tensor Operations Expressed in Einstein-Inspired Notation
 Home-page: https://github.com/fferflo/einx
 Author: Florian Fervers
 Author-email: florian.fervers@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: numpy
+Requires-Dist: sympy
+Requires-Dist: frozendict
 Provides-Extra: torch
+Requires-Dist: torch>=2; extra == "torch"
 Provides-Extra: keras
-License-File: LICENSE
+Requires-Dist: keras>=3; extra == "keras"
 
 # *einx* - Tensor Operations in Einstein-Inspired Notation
 
 [![pytest](https://github.com/fferflo/einx/actions/workflows/run_pytest.yml/badge.svg)](https://github.com/fferflo/einx/actions/workflows/run_pytest.yml)
 [![Documentation](https://img.shields.io/badge/documentation-link-blue.svg)](https://einx.readthedocs.io)
 [![PyPI version](https://badge.fury.io/py/einx.svg)](https://badge.fury.io/py/einx)
 [![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue.svg)](https://www.python.org/downloads/release/python-380/)
@@ -129,15 +134,15 @@
 
 einx traces the required backend operations for a given call into graph representation and just-in-time compiles them into a regular Python function using Python's [`exec()`](https://docs.python.org/3/library/functions.html#exec). This reduces overhead to a single cache lookup and allows inspecting the generated function. For example:
 
 ```python
 >>> x = np.zeros((3, 10, 10))
 >>> graph = einx.sum("... (g [c])", x, g=2, graph=True)
 >>> print(graph)
-# backend: einx.backend.numpy
+import numpy as np
 def op0(i0):
-    x1 = backend.reshape(i0, (3, 10, 2, 5))
-    x0 = backend.sum(x1, axis=3)
-    return x0
+    x0 = np.reshape(i0, (3, 10, 2, 5))
+    x1 = np.sum(x0, axis=3)
+    return x1
 ```
 
 See [Just-in-time compilation](https://einx.readthedocs.io/en/latest/gettingstarted/jit.html) for more details.
```

### Comparing `einx-0.2.0/einx.egg-info/SOURCES.txt` & `einx-0.2.1/einx.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 LICENSE
 README.md
 setup.cfg
 setup.py
 einx/__init__.py
-einx/lru_cache.py
-einx/param.py
 einx/traceback_util.py
 einx/tree_util.py
 einx/types.py
 einx.egg-info/PKG-INFO
 einx.egg-info/SOURCES.txt
 einx.egg-info/dependency_links.txt
 einx.egg-info/requires.txt
@@ -17,25 +15,24 @@
 einx/backend/_dask.py
 einx/backend/_jax.py
 einx/backend/_mlx.py
 einx/backend/_numpy.py
 einx/backend/_tensorflow.py
 einx/backend/_torch.py
 einx/backend/base.py
-einx/backend/tracer.py
+einx/backend/register.py
 einx/expr/__init__.py
 einx/expr/solver.py
 einx/expr/stage1.py
 einx/expr/stage2.py
 einx/expr/stage3.py
 einx/expr/util.py
 einx/nn/__init__.py
 einx/nn/equinox.py
 einx/nn/flax.py
-einx/nn/framework.py
 einx/nn/haiku.py
 einx/nn/keras.py
 einx/nn/nn.py
 einx/nn/torch.py
 einx/op/__init__.py
 einx/op/arange.py
 einx/op/dot.py
@@ -43,11 +40,18 @@
 einx/op/index.py
 einx/op/rearrange.py
 einx/op/reduce.py
 einx/op/solve.py
 einx/op/util.py
 einx/op/vmap.py
 einx/op/vmap_with_axis.py
+einx/tracer/__init__.py
+einx/tracer/compile.py
+einx/tracer/decorator.py
+einx/tracer/input.py
+einx/tracer/optimize.py
+einx/tracer/tensor.py
+einx/tracer/tracer.py
 test/test_compare_einops.py
 test/test_nn.py
 test/test_shapes.py
 test/test_values.py
```

### Comparing `einx-0.2.0/setup.py` & `einx-0.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md") as f:
     long_description = f.read()
 
 setup(
     name="einx",
-    version="0.2.0",
+    version="0.2.1",
     python_requires=">=3.8",
     description="Tensor Operations Expressed in Einstein-Inspired Notation",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Florian Fervers",
     author_email="florian.fervers@gmail.com",
     url="https://github.com/fferflo/einx",
```

### Comparing `einx-0.2.0/test/test_compare_einops.py` & `einx-0.2.1/test/test_compare_einops.py`

 * *Files identical despite different names*

### Comparing `einx-0.2.0/test/test_nn.py` & `einx-0.2.1/test/test_nn.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,36 +12,34 @@
     ("b [s...] ([g] c)", {"g": 2}),
 ]
 
 if importlib.util.find_spec("torch"):
     import torch
     import einx.nn.torch
 
-    # Tests are run with many different sets of parameters which cause torch.compile
-    # to recompile the used function and hit the cache limit.
-    # We increase the cache limit to avoid this issue.
-    try:
-        torch._dynamo.config.accumulated_cache_size_limit = 99999
-    except:
-        pass
-    torch._dynamo.config.cache_size_limit = 99999
+    if "compiler" in dir(torch):
+        compiler = torch.compiler
+    else:
+        import torch._dynamo as compiler
 
     def test_torch_linear():
+        compiler.reset()
         x = torch.zeros((4, 128, 128, 3))
 
         layer = einx.nn.torch.Linear("b... [c1->c2]", c2=32)
         assert layer.forward(x).shape == (4, 128, 128, 32)
         layer = torch.compile(layer)
         assert layer.forward(x).shape == (4, 128, 128, 32)
 
     @pytest.mark.parametrize("expr_kwargs", norms)
     @pytest.mark.parametrize("mean", [True, False])
     @pytest.mark.parametrize("scale", [True, False])
     @pytest.mark.parametrize("decay_rate", [None, 0.9])
     def test_torch_norm(expr_kwargs, mean, scale, decay_rate):
+        compiler.reset()
         expr, kwargs = expr_kwargs
         x = torch.zeros((4, 128, 128, 32))
 
         layer = einx.nn.torch.Norm(expr, mean=mean, scale=scale, decay_rate=decay_rate, **kwargs)
         layer.train()
         assert layer.forward(x).shape == (4, 128, 128, 32)
         layer.eval()
@@ -50,14 +48,15 @@
         layer = torch.compile(layer, fullgraph=True)
         layer.train()
         assert layer.forward(x).shape == (4, 128, 128, 32)
         layer.eval()
         assert layer.forward(x).shape == (4, 128, 128, 32)
 
     def test_torch_dropout():
+        compiler.reset()
         x = torch.zeros((4, 128, 128, 3))
 
         layer = einx.nn.torch.Dropout("[b] ... [c]", drop_rate=0.2)
         layer.train()
         assert layer.forward(x).shape == (4, 128, 128, 3)
         layer = torch.compile(layer)
         assert layer.forward(x).shape == (4, 128, 128, 3)
@@ -243,15 +242,15 @@
         assert layer(x, rng=rng).shape == (4, 128, 128, 3)
 
 
 if importlib.util.find_spec("keras"):
     import keras
 
     version = tuple(int(i) for i in keras.__version__.split(".")[:2])
-    if version > (3, 0):
+    if version >= (3, 0):
         import tensorflow as tf
         import einx.nn.keras
 
         def test_keras_linear():
             x = tf.zeros((4, 128, 128, 3))
 
             layer = einx.nn.keras.Linear("b... [c1->c2]", c2=32)
```

### Comparing `einx-0.2.0/test/test_shapes.py` & `einx-0.2.1/test/test_shapes.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,358 +1,414 @@
-import importlib
-
-if importlib.util.find_spec("jax"):
-    import jax
-if importlib.util.find_spec("torch"):
-    import torch
-if importlib.util.find_spec("tensorflow"):
-    import os
-
-    os.environ["TF_FORCE_GPU_ALLOW_GROWTH"] = "true"
-    import tensorflow
-    import tensorflow.experimental.numpy as tnp
-
-    tnp.experimental_enable_numpy_behavior()
-if importlib.util.find_spec("mlx"):
-    import mlx
-if importlib.util.find_spec("dask"):
-    import dask.array
-
 import einx
 import pytest
-from functools import partial
 import numpy as np
+import conftest
+
 
-backends = [b for b in einx.backend.backends if b != einx.backend.tracer]
+@pytest.mark.parametrize("test", conftest.tests)
+def test_shape_rearrange(test):
+    einx, backend, setup = test
 
+    x = setup.full((10, 20, 1))
 
-@pytest.mark.parametrize("backend", backends)
-def test_shape_rearrange(backend):
-    x = backend.zeros((10, 20, 1), "float32")
     assert einx.rearrange("a b c -> (a b) c 1", x).shape == (200, 1, 1)
     assert einx.rearrange("a b c -> (a b) c 1", x).shape == (200, 1, 1)
     assert einx.rearrange("a b c -> (a b) c 1 1 1", x).shape == (200, 1, 1, 1, 1)
     with pytest.raises(Exception):
         einx.rearrange("a a b c -> (a b) c 1", x)
         einx.rearrange("a (a + b) c -> (a b) c 1", x)
 
-    x = backend.zeros((10, 20, 20, 2), "float32")
+    x = setup.full((10, 20, 20, 2))
     assert einx.rearrange("b s... c -> b (s...) c", x).shape == (10, 400, 2)
     assert einx.rearrange("b ... c -> b (...) c", x).shape == (10, 400, 2)
     assert einx.rearrange("b (s...) (r...) c -> b (s...) r... c", x, r=(10, 2)).shape == (
         10,
         20,
         10,
         2,
         2,
     )
 
-    assert einx.rearrange("1 -> (x)", backend.to_tensor([1]), x=10).shape == (10,)
-    assert einx.rearrange("1 -> (x y)", backend.to_tensor([1]), x=10, y=20).shape == (200,)
+    if backend.name != "torch":
+        assert einx.rearrange("1 -> (x)", [1], x=10, backend=backend).shape == (10,)
+        assert einx.rearrange("1 -> (x y)", [1], x=10, y=20, backend=backend).shape == (200,)
+
+    assert einx.rearrange("1 -> (x)", setup.to_tensor([1]), x=10).shape == (10,)
+    assert einx.rearrange("1 -> (x y)", setup.to_tensor([1]), x=10, y=20).shape == (200,)
+
+    x = setup.full((1,))
+    assert einx.rearrange("1 -> (x)", x, x=10).shape == (10,)
+    assert einx.rearrange("1 -> (x y)", x, x=10, y=20).shape == (200,)
 
-    x = backend.zeros((10, 20, 1), "float32")
+    x = setup.full((10, 20, 1))
     assert einx.rearrange("a b c d... -> a b c (d...)", x).shape == (10, 20, 1, 1)
 
-    x = backend.zeros((10, 20, 1, 2), "float32")
+    x = setup.full((10, 20, 1, 2))
     assert einx.rearrange("a (b...) c d -> a (b... c) d", x).shape == (10, 20, 2)
 
-    x = backend.zeros((10, 20, 1, 2, 3), "float32")
+    x = setup.full((10, 20, 1, 2, 3))
     assert einx.rearrange("a (b... c) d... e -> a (b...) (c d...) e", x, b=[2, 5]).shape == (
         10,
         10,
         4,
         3,
     )
 
-    x = backend.zeros((10, 20, 6, 24), "float32")
+    x = setup.full((10, 20, 6, 24))
     assert einx.rearrange("a b (c...) (d...) -> a c... b d...", x, c=[2, 3], d=[4, 6]).shape == (
         10,
         2,
         3,
         20,
         4,
         6,
     )
 
-    x = backend.zeros((10, 10), "float32")
+    x = setup.full((10, 10))
     assert einx.rearrange("a... -> 1 (a...)", x).shape == (1, 100)
 
-    x = backend.zeros((10, 20, 5), "float32")
+    x = setup.full((10, 20, 5))
     assert einx.rearrange("(s1...) (s2...) h -> 1 h (s1...) (s2...)", x).shape == (1, 5, 10, 20)
 
-    x = backend.zeros((10, 20), "float32")
+    x = setup.full((10, 20))
     with pytest.raises(Exception):
         assert einx.rearrange("(s1...) (s2...) h -> 1 h (s1...) (s2...)", x).shape == (1, 5, 10, 20)
 
-    x = backend.zeros((10, 20, 1), "float32")
+    x = setup.full((10, 20, 1))
     with pytest.raises(Exception):
         einx.rearrange("a b c -> (a b) c d", x)
 
-    x = backend.zeros((10, 20, 1), "float32")
+    x = setup.full((10, 20, 1))
     with pytest.raises(Exception):
         einx.rearrange("a b... c... -> a (b...) c...", x)
     with pytest.raises(Exception):
         einx.rearrange("a b... -> a b", x)
 
-    x = backend.zeros((1, 10, 20, 6), "float32")
+    x = setup.full((1, 10, 20, 6))
     assert einx.rearrange("a (b...) (e f...) (d c) -> a d (b...) (e f...) c", x, d=2).shape == (
         1,
         2,
         10,
         20,
         3,
     )
 
-    x = backend.zeros((1, 10, 20, 6, 7, 12), "float32")
+    x = setup.full((1, 10, 20, 6, 7, 12))
     assert einx.rearrange(
         "a b c d... (e f...) -> a b c d... ((e 2 2) f...)", x, f=[2, 2]
     ).shape == (
         1,
         10,
         20,
         6,
         7,
         12 * 2 * 2,
     )
 
-    x = backend.zeros((10, 20, 3), "float32")
+    x = setup.full((10, 20, 3))
     assert einx.rearrange("(s s2)... c -> s... s2... c", x, s2=(2, 2)).shape == (5, 10, 2, 2, 3)
     assert einx.rearrange("(s s2)... c -> s... s2... c", x, s2=2).shape == (5, 10, 2, 2, 3)
 
-    x = backend.zeros((10, 10, 10), "float32")
+    x = setup.full((10, 10, 10))
     assert einx.rearrange("(a b) (c d) (e f) -> a (b c d e) f", x, a=2, f=2).shape == (2, 250, 2)
 
-    x = backend.zeros((10,), "float32")
-    y = backend.zeros((20,), "float32")
+    x = setup.full((10,))
+    y = setup.full((20,))
     assert einx.rearrange("a, b -> a + b", x, y).shape == (30,)
     assert einx.rearrange("a, b -> b + a", x, y).shape == (30,)
     assert einx.rearrange("a, b -> a b (1 + 1)", x, y).shape == (10, 20, 2)
     assert [x.shape for x in einx.rearrange("(a + b) -> a, b 1", x, a=4)] == [(4,), (6, 1)]
     with pytest.raises(Exception):
         einx.rearrange("a, b -> a b (1 + 1)", x)
         einx.rearrange("(a + b) -> a b (1 + 1)", x)
     assert einx.rearrange("a, (b c) -> c (b + a)", x, y, c=2).shape == (2, 20)
     with pytest.raises(Exception):
         assert einx.rearrange("a, -> (a +)", x, 1).shape == (11,)
 
-    x = backend.zeros((10, 10), "float32")
+    x = setup.full((10, 10))
     assert einx.rearrange("b c, 1 -> b (c + 1)", x, [42]).shape == (10, 11)
+    assert einx.rearrange("b c, -> b (c + 1)", x, 42).shape == (10, 11)
+    s = setup.full(())
+    assert einx.rearrange("b c, -> b (c + 1)", x, s).shape == (10, 11)
 
     assert einx.arange("c", c=2, backend=backend).shape == (2,)
     assert einx.arange("c... [2]", c=(4, 3), backend=backend).shape == (4, 3, 2)
     assert einx.arange("c... [l]", c=(4, 3), backend=backend).shape == (4, 3, 2)
     with pytest.raises(Exception):
         einx.arange("c... [3]", c=(4, 3), backend=backend)
     assert einx.arange("c1 c2 -> [l] c2 c1", c1=4, c2=3, backend=backend).shape == (2, 3, 4)
     assert einx.arange("(c...) [2]", c=(4, 3), backend=backend).shape == (4 * 3, 2)
     assert einx.arange("(c... [l])", c=(4, 3), backend=backend).shape == (4 * 3 * 2,)
     assert einx.arange("c1 c2 -> ([l] c2) c1", c1=4, c2=3, backend=backend).shape == (2 * 3, 4)
 
-    x = backend.zeros((10, 20), "bool")
-    y = backend.zeros((4, 10, 20, 3), "float32")
+    x = setup.full((10, 20), dtype="bool")
+    y = setup.full((4, 10, 20, 3))
     x, y = einx.rearrange("h w, b h w c -> 1 h w 1, b h w c", x, y)
-    assert backend.where(x, y, 0.0).shape == (4, 10, 20, 3)
 
     x = np.zeros((5, 4))
     x = einx.rearrange("(a + b + c) d -> b d, (a + c) d", x, a=1, b=2)
     assert x[0].shape == (2, 4)
     assert x[1].shape == (3, 4)
     x = np.zeros((5, 4))
     x = einx.rearrange("(a + b + c) d -> (a + c) d, b d", x, a=1, b=2)
     assert x[0].shape == (3, 4)
     assert x[1].shape == (2, 4)
 
 
-@pytest.mark.parametrize("backend", backends)
-def test_shape_dot(backend):
+@pytest.mark.parametrize("test", conftest.tests)
+def test_shape_dot(test):
+    einx, backend, setup = test
+
     if backend.name == "mlx":
-        pytest.xfail(reason="mlx does not support einsum yet")
-    x = backend.zeros((10, 10), "float32")
+        pytest.xfail(reason="Backend does not support einsum")
+    x = setup.full((10, 10))
     assert einx.dot("a..., a... -> 1", x, x).shape == (1,)
     with pytest.raises(Exception):
         einx.dot("a..., [a]... -> 1", x, x)
 
-    x = backend.zeros((10, 20, 1), "float32")
-    y = backend.zeros((10, 24), "float32")
+    x = setup.full((10, 20, 1))
+    y = setup.full((10, 24))
     assert einx.dot("a b c, a d -> 1 b c d", x, y).shape == (1, 20, 1, 24)
-    assert einx.dot("a b c, a d -> 1 b c d", x, backend.zeros, d=24).shape == (1, 20, 1, 24)
+    assert einx.dot("a b c, a d -> 1 b c d", x, setup.full, d=24).shape == (1, 20, 1, 24)
 
-    x = backend.zeros((10, 20, 1), "float32")
+    x = setup.full((10, 20, 1))
     with pytest.raises(Exception):
         einx.dot("a b c -> a b c", x, x)
     with pytest.raises(Exception):
         einx.dot("a b c, a -> a b c", x)
 
-    x = backend.zeros((10, 20), "float32")
-    y = backend.zeros((20, 30), "float32")
+    x = setup.full((10, 20))
+    y = setup.full((20, 30))
     assert einx.dot("a [b] -> a [c]", x, y).shape == (10, 30)
     assert einx.dot("a b, b c -> a c", x, y).shape == (10, 30)
     assert einx.dot("a [b->c]", x, y).shape == (10, 30)
     assert einx.dot("a [b...->c]", x, y).shape == (10, 30)
 
-    x = backend.zeros((10, 20), "float32")
-    y = backend.zeros((10, 20, 30), "float32")
+    x = setup.full((10, 20))
+    y = setup.full((10, 20, 30))
     assert einx.dot("a b, a b c -> a c", x, y).shape == (10, 30)
     assert einx.dot("[a b] -> [a c]", x, y).shape == (10, 30)
     assert einx.dot("[a b->a c]", x, y).shape == (10, 30)
 
-    x = backend.zeros((10,), "float32")
-    y = backend.zeros((30,), "float32")
+    x = setup.full((10,))
+    y = setup.full((30,))
     assert einx.dot("a, a ->", x, x).shape == ()
     assert einx.dot("[a->]", x, x).shape == ()
     assert einx.dot("a, c -> a c", x, y).shape == (10, 30)
     assert einx.dot("a [->c]", x, y).shape == (10, 30)
     assert einx.dot("a [b...->c]", x, y).shape == (10, 30)
 
-    x = backend.zeros((4, 128, 128, 16), "float32")
-    assert einx.dot("b s... [c1->c2]", x, backend.zeros, c2=32).shape == (4, 128, 128, 32)
-    assert einx.dot("b [s...->s2] c", x, backend.zeros, s2=32).shape == (4, 32, 16)
+    x = setup.full((4, 128, 128, 16))
+    assert einx.dot("b s... [c1->c2]", x, setup.full, c2=32).shape == (4, 128, 128, 32)
+    assert einx.dot("b [s...->s2] c", x, setup.full, s2=32).shape == (4, 32, 16)
 
-    w = backend.zeros((2, 2, 16, 32), "float32")
+    w = setup.full((2, 2, 16, 32))
     assert einx.dot("b (s [s2->])... [c1->c2]", x, w, s2=2, c2=32).shape == (4, 64, 64, 32)
 
-    x = backend.zeros((4, 16, 16, 16), "float32")
+    x = setup.full((4, 16, 16, 16))
 
     def w(shape):
-        return backend.zeros(shape, "float32")
+        return setup.full(shape)
 
     assert einx.dot("b [(s s2)->s]... [c1->c2]", x, w, s2=4, c2=4).shape == (4, 4, 4, 4)
     assert einx.dot("b (s [s2->])... [c1->c2]", x, w, s2=4, c2=4).shape == (4, 4, 4, 4)
 
-    x = backend.ones((10, 10), "float32")
-    y = backend.ones((10,), "float32")
-    assert einx.dot("[->]", 1, 1).shape == ()
+    s = setup.full(())
+    x = setup.full((10, 10))
+    y = setup.full((10,))
+    assert einx.dot("[->]", s, s, backend=backend).shape == ()
+    assert einx.dot("a [->]", y, s).shape == (10,)
+    if backend.name not in {"torch"}:
+        einx.dot("[->]", 1, 1, backend=backend).shape == ()
     assert einx.dot("a [->]", y, 1).shape == (10,)
     assert einx.dot("a [b->]", x, y).shape == (10,)
     assert einx.dot("a [->b]", y, y).shape == (10, 10)
 
-    x = backend.ones((11, 10), "float32")
-    y = backend.ones((11,), "float32")
+    x = setup.full((11, 10))
+    y = setup.full((11,))
     assert einx.dot("... b, ... -> b", x, y).shape == (10,)
     assert einx.dot("[...] b -> b", x, y).shape == (10,)
 
-    x = backend.ones((10,), "float32")
-    y = backend.ones((), "float32")
+    x = setup.full((10,))
+    y = setup.full(())
     assert einx.dot("... b, ... -> b", x, y).shape == (10,)
     assert einx.dot("[...] b -> b", x, y).shape == (10,)
 
 
-@pytest.mark.parametrize("backend", backends)
-def test_shape_reduce(backend):
-    x = backend.zeros((10, 10), "float32")
+@pytest.mark.parametrize("test", conftest.tests)
+def test_shape_reduce(test):
+    einx, backend, setup = test
+
+    x = setup.full((10, 10))
     assert einx.reduce("a b -> 1 a", x, op=backend.mean).shape == (1, 10)
+    op = lambda tensor, axis: einx.jit(lambda tensor, backend: backend.mean(tensor, axis))(tensor)
+    assert einx.reduce("a b -> 1 a", x, op=op).shape == (
+        1,
+        10,
+    )
     assert einx.mean("a b -> 1 a", x).shape == (1, 10)
     assert einx.mean("[a] b", x).shape == (10,)
     assert einx.mean("[a] b -> 1 b", x).shape == (1, 10)
 
-    x = backend.zeros((10, 10, 10), "float32")
+    x = setup.full((10, 10, 10))
     with pytest.raises(Exception):
         einx.sum("a [b] c -> a b", x)
 
-    x = backend.zeros((10, 3, 1), "float32")
+    x = setup.full((10, 3, 1))
     assert einx.mean("(a [b]) c 1", x, b=2).shape == (5, 3, 1)
     assert einx.mean("([a b]) c 1", x).shape == (1, 3, 1)
     assert einx.mean("[(a b)] c 1", x).shape == (3, 1)
     assert einx.mean("[(a...)] c 1", x).shape == (3, 1)
     assert einx.mean("(b... [a...]) c 1", x, b=(1, 1)).shape == (1, 3, 1)
 
-    x = backend.zeros((1, 10, 3, 2), "float32")
+    x = setup.full((1, 10, 3, 2))
     assert einx.mean("1 [a...] b", x).shape == (1, 2)
     assert einx.mean("1 [a]... b", x).shape == (1, 2)
     assert einx.mean("1 ([a])... b", x).shape == (1, 1, 1, 2)
     assert einx.mean("1 [a]... b", x, keepdims=True).shape == (1, 1, 1, 2)
     assert einx.mean("1 [a...] b", x, keepdims=True).shape == (1, 1, 2)
 
-    x = backend.zeros((16, 1, 20, 30, 64), "float32")
+    x = setup.full((16, 1, 20, 30, 64))
     assert einx.mean("(b rg) pv [s...] c", x).shape == (16, 1, 64)
 
-    x = backend.ones((16, 16, 32))
-    bias = backend.ones((4,))
+    x = setup.full((16, 16, 32))
+    bias = setup.full((4,))
     assert einx.add("b... (g [c])", x, bias).shape == (16, 16, 32)
 
     assert einx.logsumexp("a [...]", x).shape == (16,)
 
-    assert einx.logsumexp("[a]", [0.0, 1.0], backend=backend).shape == ()
-    assert (
-        einx.sum("[a]", [backend.to_tensor(0.0), backend.to_tensor(1.0)], backend=backend).shape
-        == ()
-    )
-    assert einx.logsumexp("[a] 1", [[0.0], [1.0]], backend=backend).shape == (1,)
-    assert einx.logsumexp("[a]", [0.0] * 10, backend=backend).shape == ()
-    with pytest.raises(ValueError):
-        einx.logsumexp("a", [0.0, [1.0]], backend=backend)
+    if backend.name != "torch":
+        assert einx.logsumexp("[a]", [0.0, 1.0], backend=backend).shape == ()
+        assert einx.logsumexp("[a] 1", [[0.0], [1.0]], backend=backend).shape == (1,)
+        assert einx.logsumexp("[a]", [0.0] * 10, backend=backend).shape == ()
+        with pytest.raises(Exception):
+            einx.logsumexp("a", [0.0, [1.0]], backend=backend)
 
-    x = backend.ones((16, 15))
+    x = setup.full((16, 15))
     assert einx.sum("[b] a []", x).shape == (15,)
     assert einx.sum("[b] a [...]", x).shape == (15,)
 
     assert einx.sum("b [p] -> b p2", x, p2=7).shape == (16, 7)
 
 
-@pytest.mark.parametrize("backend", backends)
-def test_shape_elementwise(backend):
-    x = backend.zeros((10, 5, 1), "float32")
-    y = backend.zeros((13,), "float32")
+@pytest.mark.parametrize("test", conftest.tests)
+def test_shape_elementwise(test):
+    einx, backend, setup = test
+
+    x = setup.full((10, 5, 1))
+    y = setup.full((13,))
     assert einx.elementwise("a b 1, l -> b l a 1", x, y, op=backend.add).shape == (5, 13, 10, 1)
+    assert einx.elementwise("a b 1, l -> b l a 1", x, y, op=lambda x, y: x + y).shape == (
+        5,
+        13,
+        10,
+        1,
+    )
     assert einx.add("a b 1, l -> b l a 1", x, y).shape == (5, 13, 10, 1)
     assert einx.add("a b 1, l -> a b l", x, y).shape == (10, 5, 13)
 
-    x = backend.zeros((10, 10), "float32")
-    y = backend.zeros((10,), "float32")
+    x = setup.full((10, 10))
+    y = setup.full((10,))
     assert einx.add("a, a b", y, x).shape == (10, 10)
     assert einx.add("a b, a", x, y).shape == (10, 10)
     assert einx.add("a b, b", x, y).shape == (10, 10)
     assert einx.add("a [b]", x, y).shape == (10, 10)
     assert einx.add("a b, a b", x, x).shape == (10, 10)
     assert einx.add("a b, ", x, 1).shape == (10, 10)
     assert einx.add(", a b", 1, x).shape == (10, 10)
     assert einx.add("a b, 1", x, [1]).shape == (10, 10)
     assert einx.add("1, a b", [1], x).shape == (10, 10)
     with pytest.raises(Exception):
         einx.add("a a, a -> a a", x, y)
-    assert einx.add("a b, a b", x, backend.zeros).shape == (10, 10)
+    assert einx.add("a b, a b", x, setup.full).shape == (10, 10)
     assert einx.add("a, a", y, y).shape == (10,)
     assert einx.add("[a]", y, y).shape == (10,)
     assert einx.add("b, -> b 3", y, 1).shape == (10, 3)
 
-    x = backend.zeros((2, 3), "float32")
-    y = backend.ones((10,), "float32")
+    x = setup.full((2, 3))
+    y = setup.full((10,))
     with pytest.raises(Exception):
         einx.add("a b, c", x, y)
 
-    x = backend.zeros((3, 128, 196, 64), "float32")
-    y = backend.zeros((3, 4, 16), "float32")
+    x = setup.full((3, 128, 196, 64))
+    y = setup.full((3, 4, 16))
     assert einx.add("b h w (g c), b (g) c -> b h w (g c)", x, y).shape == (3, 128, 196, 64)
 
-    x = backend.zeros((10, 20), "float32")
-    y = backend.zeros((10, 20, 30), "float32")
+    x = setup.full((10, 20))
+    y = setup.full((10, 20, 30))
     assert einx.add("a b, a b c -> a b c", x, y).shape == (10, 20, 30)
-    assert einx.add("(a [1])...", x, backend.ones).shape == (10, 20)
+    assert einx.add("(a [1])...", x, setup.full).shape == (10, 20)
 
-    x = backend.zeros((10, 20), "float32")
-    y = backend.zeros((30, 20), "float32")
+    x = setup.full((10, 20))
+    y = setup.full((30, 20))
     with pytest.raises(Exception):
         einx.subtract("ba c, i c -> i ba", x, y)
 
+    ops = [
+        ("add", ("float32", "float32")),
+        ("subtract", ("float32", "float32")),
+        ("multiply", ("float32", "float32")),
+        ("true_divide", ("float32", "float32")),
+        ("floor_divide", ("float32", "float32")),
+        ("divide", ("float32", "float32")),
+        ("logical_and", ("bool", "bool")),
+        ("logical_or", ("bool", "bool")),
+        ("where", ("bool", "float32", "float32")),
+        ("less", ("float32", "float32")),
+        ("less_equal", ("float32", "float32")),
+        ("greater", ("float32", "float32")),
+        ("greater_equal", ("float32", "float32")),
+        ("equal", ("float32", "float32")),
+        ("not_equal", ("float32", "float32")),
+        ("maximum", ("float32", "float32")),
+        ("minimum", ("float32", "float32")),
+    ]
+
+    def create_scalar(dtype):
+        if dtype == "float32":
+            return 1.0
+        elif dtype == "bool":
+            return True
+        else:
+            assert False
+
+    for op, dtypes in ops:
+        tensor_args = [setup.full((10,), dtype=dtype, value=1) for dtype in dtypes]
+        scalar_args = [create_scalar(dtype) for dtype in dtypes]
+
+        for scalar_index in range(len(dtypes)):
+            args = [
+                scalar_args[scalar_index] if i == scalar_index else tensor_args[i]
+                for i in range(len(dtypes))
+            ]
+            expr = (
+                ", ".join(["" if i == scalar_index else "a" for i in range(len(dtypes))]) + " -> a"
+            )
+            assert getattr(einx, op)(expr, *args).shape == (10,)
+
+
+@pytest.mark.parametrize("test", conftest.tests)
+def test_shape_vmap(test):
+    einx, backend, setup = test
 
-@pytest.mark.parametrize("backend", backends)
-def test_shape_vmap(backend):
     if backend.name in {"mlx", "dask"}:
-        pytest.xfail(reason="mlx does not fully support vmap with all primites yet")
+        pytest.xfail(reason="Backend does not fully support vmap")
 
-    x = backend.zeros((13,), "float32")
-    assert einx.vmap("b -> b [3]", x, op=lambda x: x + backend.zeros((3,))).shape == (13, 3)
+    x = setup.full((13,))
+    assert einx.vmap("b -> b [3]", x, op=lambda x: x + setup.full((3,))).shape == (13, 3)
 
-    with pytest.raises(ValueError):
-        einx.vmap("b -> [b] 3", x, op=lambda x: x + backend.zeros((3,)))
     with pytest.raises(Exception):
-        einx.vmap("b -> b 3", x, op=lambda x: x + backend.ones((3,)))
+        einx.vmap("b -> [b] 3", x, op=lambda x: x + setup.full((3,)))
+    with pytest.raises(Exception):
+        einx.vmap("b -> b 3", x, op=einx.trace(lambda x: x + setup.full((3,))))
+    with pytest.raises(Exception):
+        einx.vmap("b -> b 3", x, op=lambda x: x + setup.full((3,)))
 
-    x = backend.zeros((4, 13, 2), "float32")
-    y = backend.zeros((13, 4, 5, 5), "float32")
+    x = setup.full((4, 13, 2))
+    y = setup.full((13, 4, 5, 5))
 
     def f(x, y):
         assert x.shape == (4, 2)
         assert y.shape == (4, 5)
         x = x[:, 0] + y[:, 0]
         return einx.rearrange("a -> a 15", x)
 
@@ -376,95 +432,107 @@
             assert x.shape == (4, 2)
             assert y.shape == (4, 5)
             x = x[:, 0] + y[:, 0]
             return einx.rearrange("a -> a 16", x)
 
         einx.vmap("[a] b [e], b [a] c [d] -> [a] b [g] c", x, y, op=f, g=15)
 
-    x = backend.zeros((4, 16), "float32")
-    y = backend.zeros((16, 32), "float32")
-    assert einx.vmap("b [c1], [c1] c2 -> b c2", x, y, op=lambda x, y: backend.sum(x * y)).shape == (
+    x = setup.full((4, 16))
+    y = setup.full((16, 32))
+    op = lambda x, y: einx.jit(lambda x, y, backend: backend.sum(x * y))(x, y)
+    assert einx.vmap("b [c1], [c1] c2 -> b c2", x, y, op=op).shape == (
         4,
         32,
     )
 
-    x = backend.zeros((4,), "float32")
-    y = backend.zeros((16, 32), "float32")
+    x = setup.full((4,))
+    y = setup.full((16, 32))
     assert einx.vmap("a, b c -> a b c", x, y, op=backend.add).shape == (4, 16, 32)
 
-    def func(x):  # c -> 2
-        return backend.stack([backend.mean(x), backend.max(x)])
+    func = lambda x: einx.jit(lambda x, backend: backend.stack([backend.mean(x), backend.max(x)]))(
+        x
+    )  # c -> 2
 
-    x = backend.zeros(
+    x = setup.full(
         (
             16,
             64,
             3,
         ),
-        "float32",
     )
     assert einx.vmap("b [c] a -> a b [2]", x, op=func).shape == (3, 16, 2)
 
-    def func(x, y):  # c, d -> 2
-        return backend.stack([backend.mean(x), backend.max(y)])
+    func = lambda x, y: einx.jit(
+        lambda x, y, backend: backend.stack([backend.mean(x), backend.max(y)])
+    )(x, y)  # c, d -> 2
 
-    x = backend.zeros((16, 64), "float32")  # b c
-    y = backend.zeros((16, 72), "float32")  # b d
+    x = setup.full((16, 64))  # b c
+    y = setup.full((16, 72))  # b d
     assert einx.vmap("b [c], b [d] -> b [2]", x, y, op=func).shape == (16, 2)
 
-    x = backend.zeros((16, 64, 3), "float32")  # b1 c b2
-    y = backend.zeros((3, 72), "float32")  # b2 d
+    x = setup.full((16, 64, 3))  # b1 c b2
+    y = setup.full((3, 72))  # b2 d
     assert einx.vmap("b1 [c] b2, b2 [d] -> b2 [2] b1", x, y, op=func).shape == (3, 2, 16)
 
+    @einx.trace
     def func(x):  # (c d) -> 2
         x = einx.vmap("([c] d) -> d", x, op=backend.mean, c=16)
         x = backend.max(x)
         return backend.stack([x, x])
 
-    x = backend.zeros((16, 64), "float32")  # b c
+    x = setup.full((16, 64))  # b c
     assert einx.vmap("b ([c d]) -> b [2]", x, op=func, c=16).shape == (16, 2)
     assert einx.vmap("b ([c d]) -> b [2] 1", x, op=func, c=16).shape == (16, 2, 1)
     assert einx.vmap("b [(c d)->2]", x, op=func, c=16).shape == (16, 2)
     assert einx.vmap("b ([c d->2])", x, op=func, c=16).shape == (16, 2)
     with pytest.raises(Exception):
         einx.vmap("b ([c d]) -> [2]", x, op=func, c=16)
 
+    @einx.trace
     def func(x):  # c d -> 2
         x = einx.vmap("[c] d -> d", x, op=backend.mean, c=16)
         x = backend.max(x)
         return backend.stack([x, x])
 
-    x = backend.zeros((16, 64), "float32")  # b c
+    x = setup.full((16, 64))  # b c
     assert einx.vmap("b ([c d]) -> b [2]", x, op=func, c=16, flat=True).shape == (16, 2)
     assert einx.vmap("b ([c d]) -> b [2] 1", x, op=func, c=16, flat=True).shape == (16, 2, 1)
     assert einx.vmap("b [(c d)->2]", x, op=func, c=16, flat=True).shape == (16, 2)
     assert einx.vmap("b ([c d->2])", x, op=func, c=16, flat=True).shape == (16, 2)
     with pytest.raises(Exception):
         einx.vmap("b ([c d]) -> [2]", x, op=func, c=16, flat=True)
 
+    op = lambda tensor, axis: einx.jit(
+        lambda tensor, backend: backend.roll(tensor, axis=axis, shift=(2, 2))
+    )(tensor)
     with pytest.raises(Exception):
-        einx.vmap_with_axis("a ([b c]) -> a ([b c])", x, op=partial(backend.roll, shift=(2, 2)))
+        einx.vmap_with_axis("a ([b c]) -> a ([b c])", x, op=op)
     assert einx.vmap_with_axis(
-        "a ([b c]) -> a ([b c])", x, op=partial(backend.roll, shift=(2, 2)), b=2
+        "a ([b c]) -> a ([b c])",
+        x,
+        op=op,
+        b=2,
     ).shape == (
         16,
         64,
     )
 
 
-@pytest.mark.parametrize("backend", backends)
-def test_shape_index(backend):
+@pytest.mark.parametrize("test", conftest.tests)
+def test_shape_index(test):
+    einx, backend, setup = test
+
     if backend.name in {"mlx", "dask"}:
-        pytest.xfail(reason="mlx does not fully support vmap with all primites yet")
+        pytest.xfail(reason="Backend does not fully support vmap")
 
     coord_dtype = "int32" if backend.name != "torch" else "long"
-    x = backend.ones((4, 16, 16, 3))
-    y = backend.cast(backend.ones((4, 128, 2)), coord_dtype)
-    y2 = backend.cast(backend.ones((128, 4, 2)), coord_dtype)
-    z = backend.ones((4, 128, 3))
+    x = setup.full((4, 16, 16, 3))
+    y = setup.full((4, 128, 2), dtype=coord_dtype)
+    y2 = setup.full((128, 4, 2), dtype=coord_dtype)
+    z = setup.full((4, 128, 3))
     assert einx.get_at("b [h w] c, b p [2] -> b p c", x, y).shape == (4, 128, 3)
     assert einx.get_at("b [h w] c, p b [2] -> b p c", x, y2).shape == (4, 128, 3)
     assert einx.get_at("b [h w] c, b p, b p -> b p c", x, y[..., 0], y[..., 1]).shape == (4, 128, 3)
     assert einx.get_at("b [h w] c, b (p [1]), b p -> b p c", x, y[..., 0], y[..., 1]).shape == (
         4,
         128,
         3,
@@ -481,18 +549,24 @@
     )
     assert einx.get_at("b [h w] c, b (p [1]), p b -> b p c", x, y[..., 0], y2[..., 1]).shape == (
         4,
         128,
         3,
     )
     assert einx.get_at(
-        "b [h w] c, b p [2] -> b p c", x, lambda shape: backend.ones(shape, coord_dtype), p=128
+        "b [h w] c, b p [2] -> b p c",
+        x,
+        lambda shape: setup.full(shape, dtype=coord_dtype, value=0),
+        p=128,
     ).shape == (4, 128, 3)
     assert einx.get_at(
-        "b [h w] c, b p [l] -> b p c", x, lambda shape: backend.ones(shape, coord_dtype), p=128
+        "b [h w] c, b p [l] -> b p c",
+        x,
+        lambda shape: setup.full(shape, dtype=coord_dtype, value=0),
+        p=128,
     ).shape == (4, 128, 3)
     assert einx.get_at("b [16 w] c, b p [2] -> b p c", x, y).shape == (4, 128, 3)
     assert einx.get_at("b [16 16] c, b p [2] -> b p c", x, y).shape == (4, 128, 3)
     assert einx.get_at("b [h w] c, p [2] -> b p c", x, y[0]).shape == (4, 128, 3)
     for op in [einx.set_at, einx.add_at, einx.subtract_at]:
         assert op("b [h w] c, b p [2], b p c -> b [h w] c", x, y, z).shape == (4, 16, 16, 3)
         assert op("b [h w] c, b p [2], b p c", x, y, z).shape == (4, 16, 16, 3)
@@ -516,168 +590,179 @@
         ).shape == (4, 16, 16, 3)
         assert op("b [h w] c, p [2], p c -> b [h w] c", x, y[0], z[0]).shape == (4, 16, 16, 3)
         assert op("b [h w] c, b p [2], b p c -> b h w c", x, y, z).shape == (4, 16, 16, 3)
         assert op("b [h w] c, b p [2], p c -> b h w c", x, y, z[0]).shape == (4, 16, 16, 3)
         assert op("b [h w] c, p [2], b p c -> b h w c", x, y[0], z).shape == (4, 16, 16, 3)
         assert op("b [h w] c, p [2], p c -> b h w c", x, y[0], z[0]).shape == (4, 16, 16, 3)
 
-    x = backend.ones((16, 4, 3, 16))
-    y = backend.cast(backend.ones((2, 4, 128)), coord_dtype)
-    z = backend.ones((3, 4, 128))
+    x = setup.full((16, 4, 3, 16))
+    y = setup.full((2, 4, 128), dtype=coord_dtype, value=0)
+    z = setup.full((3, 4, 128))
     assert einx.get_at("[w] b c [h], [2] b p -> b p c", x, y).shape == (4, 128, 3)
     assert einx.get_at("[w] b c [h], [2] p -> b p c", x, y[:, 0]).shape == (4, 128, 3)
     for op in [einx.set_at, einx.add_at, einx.subtract_at]:
         assert op("[w] b c [h], [2] b p, c b p -> b [w h] c", x, y, z).shape == (4, 16, 16, 3)
         assert op("[w] b c [h], [2] p, c p -> b [w h] c", x, y[:, 0], z[:, 0]).shape == (
             4,
             16,
             16,
             3,
         )
 
-    x = backend.ones((16, 4, 3 * 16))
-    y = backend.cast(backend.ones((2, 4, 128)), coord_dtype)
-    z = backend.ones((3, 4, 128))
+    x = setup.full((16, 4, 3 * 16))
+    y = setup.full((2, 4, 128), dtype=coord_dtype)
+    z = setup.full((3, 4, 128))
     assert einx.get_at("[w] b (c [h]), [2] b p -> b p c", x, y, c=3).shape == (4, 128, 3)
     assert einx.get_at("[w] b (c [h]), [2] p -> b p c", x, y[:, 0], c=3).shape == (4, 128, 3)
     for op in [einx.set_at, einx.add_at, einx.subtract_at]:
         assert op("[w] b (c [h]), [2] b p, c b p -> b ([w h]) c", x, y, z).shape == (4, 256, 3)
         assert op("[w] b (c [h]), [2] p, c p -> b ([w h]) c", x, y[:, 0], z[:, 0]).shape == (
             4,
             256,
             3,
         )
 
-    x = backend.ones((4, 16, 16, 3))
-    y = backend.cast(backend.ones((4, 3, 4, 5, 2)), coord_dtype)
-    z = backend.ones((4, 3, 4, 5, 3))
+    x = setup.full((4, 16, 16, 3))
+    y = setup.full((4, 3, 4, 5, 2), dtype=coord_dtype)
+    z = setup.full((4, 3, 4, 5, 3))
     assert einx.get_at("b [h w] c, b p q r [2] -> b p q r c", x, y).shape == (4, 3, 4, 5, 3)
     assert einx.get_at("b [h w] c, p q r [2] -> b p q r c", x, y[0]).shape == (4, 3, 4, 5, 3)
     for op in [einx.set_at, einx.add_at, einx.subtract_at]:
         assert op("b [h w] c, b p q r [2], b p q r c -> b [h w] c", x, y, z).shape == (4, 16, 16, 3)
         assert op("b [h w] c, p q r [2], p q r c -> b [h w] c", x, y[0], z[0]).shape == (
             4,
             16,
             16,
             3,
         )
 
-    x = backend.ones((4, 1, 1, 3))
-    y = backend.cast(backend.zeros((4, 128, 2)), coord_dtype)
-    z = backend.ones((4, 128, 3))
+    x = setup.full((4, 1, 1, 3))
+    y = setup.full((4, 128, 2), dtype=coord_dtype)
+    z = setup.full((4, 128, 3))
     with pytest.raises(Exception):
         einx.get_at("b ([1 1]) c, b p [2] -> b p c", x, y)
 
-    x = backend.zeros((4, 5, 6))
-    y = backend.cast(backend.zeros((4, 5)), coord_dtype)
+    x = setup.full((4, 5, 6))
+    y = setup.full((4, 5), dtype=coord_dtype)
     assert einx.get_at("b t [d], b t -> b t", x, y).shape == (4, 5)
     assert einx.get_at("... [d], ... -> ...", x, y).shape == (4, 5)
     assert einx.get_at("b t [d], b (t [1]) -> b (t 1)", x, y).shape == (4, 5)
-    with pytest.raises(ValueError):
+    with pytest.raises(Exception):
         einx.get_at("b t [d], b (t [1]) -> b (t [1])", x, y)
 
-    x = backend.ones((4, 128, 128, 3))
-    y = backend.cast(backend.zeros((4, 0, 2)), coord_dtype)
-    y2 = backend.cast(backend.zeros((4, 2)), coord_dtype)
-    z = backend.ones((4, 0, 3))
-    z2 = backend.ones((4, 3))
+    x = setup.full((4, 128, 128, 3))
+    y = setup.full((4, 0, 2), dtype=coord_dtype)
+    y2 = setup.full((4, 2), dtype=coord_dtype)
+    z = setup.full((4, 0, 3))
+    z2 = setup.full((4, 3))
     assert einx.set_at("b [h w] c, b p [2], b p c -> b [h w] c", x, y, z).shape == (4, 128, 128, 3)
     assert einx.set_at("b [h w] c, b p [2], b c -> b [h w] c", x, y, z2).shape == (4, 128, 128, 3)
     assert einx.set_at("b [h w] c, b [2], b p c -> b [h w] c", x, y, z2).shape == (4, 128, 128, 3)
 
-    x = backend.ones((4, 128, 16))
-    y = backend.cast(backend.zeros((4, 128)), coord_dtype)
-    z = backend.ones((4, 128))
+    x = setup.full((4, 128, 16))
+    y = setup.full((4, 128), dtype=coord_dtype)
+    z = setup.full((4, 128))
     assert einx.get_at("b p [i,->]", x, y).shape == (4, 128)
     assert einx.set_at("b p [i,,->i]", x, y, z).shape == (4, 128, 16)
 
     consts = {"b": 4, "h": 16, "w": 16, "c": 3, "p": 128}
 
     def make_coords(shape):
-        return backend.cast(backend.zeros(shape), coord_dtype)
+        return setup.full(shape, dtype=coord_dtype)
 
     xs = ["([h] b) [w] c", "[h] c [w]", "[h w]"]
     ys = ["b (p [2])", "[2] p", "[2]"]
     ys2 = ["p b", "p", "[1]"]
     zs = ["b p c", "c (p b)"]
     for x in xs:
         for z in zs:
-            shape = einx.add(f"{z}, ", backend.zeros, 0, **consts, backend=backend).shape
-            for y in ys:
-                assert (
-                    einx.get_at(
-                        f"{x}, {y} -> {z}", backend.zeros, make_coords, **consts, backend=backend
-                    ).shape
-                    == shape
-                )
-            for y1 in ys2:
-                for y2 in ys2:
+            if not (z == "c (p b)" and getattr(einx, "name", "") == "torch.compile"):
+                shape = einx.add(f"{z}, ", setup.full, 0, **consts, backend=backend).shape
+                for y in ys:
                     assert (
                         einx.get_at(
-                            f"{x}, {y1}, {y2} -> {z}",
-                            backend.zeros,
-                            make_coords,
+                            f"{x}, {y} -> {z}",
+                            setup.full,
                             make_coords,
                             **consts,
                             backend=backend,
                         ).shape
                         == shape
                     )
+                for y1 in ys2:
+                    for y2 in ys2:
+                        assert (
+                            einx.get_at(
+                                f"{x}, {y1}, {y2} -> {z}",
+                                setup.full,
+                                make_coords,
+                                make_coords,
+                                **consts,
+                                backend=backend,
+                            ).shape
+                            == shape
+                        )
 
     for x in xs:
         shape = einx.add(
-            f"{x.replace('[', '').replace(']', '')}, ", backend.zeros, 0, **consts, backend=backend
+            f"{x.replace('[', '').replace(']', '')}, ",
+            setup.full,
+            0,
+            **consts,
+            backend=backend,
         ).shape
         for z in zs:
             z_axes = {a for a in z if a.isalpha()}
             for y in ys:
                 if all(a in (x + y) for a in z_axes):
                     assert (
                         einx.set_at(
                             f"{x}, {y}, {z} -> {x}",
-                            backend.ones,
+                            setup.full,
                             make_coords,
-                            backend.zeros,
+                            setup.full,
                             **consts,
                             backend=backend,
                         ).shape
                         == shape
                     )
             for y1 in ys2:
                 for y2 in ys2:
                     if all(a in (x + y1 + y2) for a in z_axes):
                         assert (
                             einx.set_at(
                                 f"{x}, {y1}, {y2}, {z} -> {x}",
-                                backend.ones,
+                                setup.full,
                                 make_coords,
                                 make_coords,
-                                backend.zeros,
+                                setup.full,
                                 **consts,
                                 backend=backend,
                             ).shape
                             == shape
                         )
                         assert (
                             einx.set_at(
                                 f"{x}, {y1}, {y2}, {z}",
-                                backend.ones,
+                                setup.full,
                                 make_coords,
                                 make_coords,
-                                backend.zeros,
+                                setup.full,
                                 **consts,
                                 backend=backend,
                             ).shape
                             == shape
                         )
 
 
-@pytest.mark.parametrize("backend", backends)
-def test_shape_vmap_with_axis(backend):
-    x = backend.ones((10, 10), "float32")
+@pytest.mark.parametrize("test", conftest.tests)
+def test_shape_vmap_with_axis(test):
+    einx, backend, setup = test
+
+    x = setup.full((10, 10))
     assert einx.flip("a [b] -> a [b]", x).shape == (10, 10)
     assert einx.flip("a [b]", x).shape == (10, 10)
     assert einx.roll("a [b]", x, shift=5).shape == (10, 10)
     assert einx.roll("a [b]", x, shift=(5,)).shape == (10, 10)
     assert einx.softmax("a [b] -> a [b]", x).shape == (10, 10)
     assert einx.softmax("a [b]", x).shape == (10, 10)
     assert einx.softmax("a [b] -> (a [b]) c", x, c=3).shape == (100, 3)
@@ -692,29 +777,31 @@
             5,
             5,
         ),
         b=2,
     ).shape == (10, 10)
 
 
-@pytest.mark.parametrize("backend", backends)
-def test_shape_solve(backend):
-    x = backend.ones((2, 3, 4))
+@pytest.mark.parametrize("test", conftest.tests)
+def test_shape_solve(test):
+    einx, backend, setup = test
+
+    x = setup.full((2, 3, 4))
     assert einx.matches("a b c", x)
     assert not einx.matches("a b", x)
     with pytest.raises(Exception):
         einx.check("a b c d", x)
     einx.check("a b c", x)
 
-    x = backend.ones((6, 4))
+    x = setup.full((6, 4))
     assert einx.matches("(a b) c", x)
 
-    x = backend.ones((2, 3, 4))
+    x = setup.full((2, 3, 4))
     assert einx.matches("a b...", x)
 
-    x = backend.ones((5, 4))
+    x = setup.full((5, 4))
     assert einx.matches("(a + b) c", x)
     assert einx.matches("(a + b) c", x, a=2)
     assert not einx.matches("(a + b) c", x, a=10)
 
     params = einx.solve("a b, c b", x, x)
     assert params["a"] == 5 and params["b"] == 4 and params["c"] == 5
```

