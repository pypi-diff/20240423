# Comparing `tmp/l3c-0.1.0.2.tar.gz` & `tmp/l3c-0.1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "l3c-0.1.0.2.tar", last modified: Tue Apr 16 02:22:58 2024, max compression
+gzip compressed data, was "l3c-0.1.0.3.tar", last modified: Tue Apr 23 09:01:36 2024, max compression
```

## Comparing `l3c-0.1.0.2.tar` & `l3c-0.1.0.3.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 wangfan04   (502) staff       (20)        0 2024-04-16 02:22:58.426622 l3c-0.1.0.2/
--rw-r--r--   0 wangfan04   (502) staff       (20)    11357 2023-02-23 10:00:57.000000 l3c-0.1.0.2/LICENSE
--rw-r--r--   0 wangfan04   (502) staff       (20)      953 2024-04-16 02:22:58.426443 l3c-0.1.0.2/PKG-INFO
--rw-r--r--   0 wangfan04   (502) staff       (20)      620 2023-02-27 11:35:59.000000 l3c-0.1.0.2/README.md
-drwxr-xr-x   0 wangfan04   (502) staff       (20)        0 2024-04-16 02:22:58.411497 l3c-0.1.0.2/l3c/
--rw-r--r--   0 wangfan04   (502) staff       (20)      762 2023-02-23 10:11:06.000000 l3c-0.1.0.2/l3c/__init__.py
-drwxr-xr-x   0 wangfan04   (502) staff       (20)        0 2024-04-16 02:22:58.416394 l3c-0.1.0.2/l3c/bandits/
--rw-r--r--   0 wangfan04   (502) staff       (20)      838 2023-02-23 10:11:06.000000 l3c-0.1.0.2/l3c/bandits/__init__.py
--rw-r--r--   0 wangfan04   (502) staff       (20)     2717 2023-02-23 10:11:06.000000 l3c-0.1.0.2/l3c/bandits/bandits_env.py
--rw-r--r--   0 wangfan04   (502) staff       (20)     1022 2023-02-23 10:32:50.000000 l3c-0.1.0.2/l3c/bandits/demo_thompson_sampling.py
-drwxr-xr-x   0 wangfan04   (502) staff       (20)        0 2024-04-16 02:22:58.416892 l3c-0.1.0.2/l3c/mazeworld/
--rw-r--r--   0 wangfan04   (502) staff       (20)     1714 2024-02-20 08:03:46.000000 l3c-0.1.0.2/l3c/mazeworld/__init__.py
-drwxr-xr-x   0 wangfan04   (502) staff       (20)        0 2024-04-16 02:22:58.418393 l3c-0.1.0.2/l3c/mazeworld/agents/
--rw-r--r--   0 wangfan04   (502) staff       (20)       45 2024-02-22 03:03:45.000000 l3c-0.1.0.2/l3c/mazeworld/agents/__init__.py
--rw-r--r--   0 wangfan04   (502) staff       (20)     2857 2024-02-22 12:10:38.000000 l3c-0.1.0.2/l3c/mazeworld/agents/agent_base.py
--rw-r--r--   0 wangfan04   (502) staff       (20)    11413 2024-04-16 01:44:52.000000 l3c-0.1.0.2/l3c/mazeworld/agents/smart_slam_agent.py
-drwxr-xr-x   0 wangfan04   (502) staff       (20)        0 2024-04-16 02:22:58.420357 l3c-0.1.0.2/l3c/mazeworld/demo/
--rw-r--r--   0 wangfan04   (502) staff       (20)        0 2024-02-22 12:15:15.000000 l3c-0.1.0.2/l3c/mazeworld/demo/__init__.py
--rw-r--r--   0 wangfan04   (502) staff       (20)     3609 2024-04-15 03:45:14.000000 l3c-0.1.0.2/l3c/mazeworld/demo/agent_play_demo.py
--rw-r--r--   0 wangfan04   (502) staff       (20)     3844 2024-02-26 06:25:37.000000 l3c-0.1.0.2/l3c/mazeworld/demo/dump_maze.py
--rw-r--r--   0 wangfan04   (502) staff       (20)     3366 2024-02-22 14:53:11.000000 l3c-0.1.0.2/l3c/mazeworld/demo/keyboard_play_demo.py
-drwxr-xr-x   0 wangfan04   (502) staff       (20)        0 2024-04-16 02:22:58.423812 l3c-0.1.0.2/l3c/mazeworld/envs/
--rw-r--r--   0 wangfan04   (502) staff       (20)      258 2024-02-04 12:16:02.000000 l3c-0.1.0.2/l3c/mazeworld/envs/__init__.py
--rw-r--r--   0 wangfan04   (502) staff       (20)     3644 2023-02-23 10:11:06.000000 l3c-0.1.0.2/l3c/mazeworld/envs/dynamics.py
--rw-r--r--   0 wangfan04   (502) staff       (20)    14649 2024-04-16 01:39:53.000000 l3c-0.1.0.2/l3c/mazeworld/envs/maze_base.py
--rw-r--r--   0 wangfan04   (502) staff       (20)     6324 2024-04-16 02:20:31.000000 l3c-0.1.0.2/l3c/mazeworld/envs/maze_continuous_3d.py
--rw-r--r--   0 wangfan04   (502) staff       (20)     3345 2024-02-22 06:12:11.000000 l3c-0.1.0.2/l3c/mazeworld/envs/maze_discrete_2d.py
--rw-r--r--   0 wangfan04   (502) staff       (20)     6849 2024-04-16 02:13:20.000000 l3c-0.1.0.2/l3c/mazeworld/envs/maze_discrete_3d.py
--rw-r--r--   0 wangfan04   (502) staff       (20)     7295 2024-04-16 02:07:18.000000 l3c-0.1.0.2/l3c/mazeworld/envs/maze_env.py
--rw-r--r--   0 wangfan04   (502) staff       (20)     9184 2024-02-20 01:19:41.000000 l3c-0.1.0.2/l3c/mazeworld/envs/maze_task.py
--rw-r--r--   0 wangfan04   (502) staff       (20)    12366 2024-04-16 02:19:02.000000 l3c-0.1.0.2/l3c/mazeworld/envs/ray_caster_utils.py
-drwxr-xr-x   0 wangfan04   (502) staff       (20)        0 2024-04-16 02:22:58.424862 l3c-0.1.0.2/l3c/mazeworld/tests/
--rw-r--r--   0 wangfan04   (502) staff       (20)        0 2024-02-22 12:15:23.000000 l3c-0.1.0.2/l3c/mazeworld/tests/__init__.py
--rw-r--r--   0 wangfan04   (502) staff       (20)     2068 2024-02-04 15:06:43.000000 l3c-0.1.0.2/l3c/mazeworld/tests/test.py
--rw-r--r--   0 wangfan04   (502) staff       (20)     2390 2024-02-22 11:56:16.000000 l3c-0.1.0.2/l3c/mazeworld/tests/test_agent.py
-drwxr-xr-x   0 wangfan04   (502) staff       (20)        0 2024-04-16 02:22:58.426204 l3c-0.1.0.2/l3c/metalm/
--rw-r--r--   0 wangfan04   (502) staff       (20)     1080 2023-05-09 04:51:28.000000 l3c-0.1.0.2/l3c/metalm/__init__.py
--rw-r--r--   0 wangfan04   (502) staff       (20)     2294 2024-02-01 05:22:53.000000 l3c-0.1.0.2/l3c/metalm/data_generator.py
--rw-r--r--   0 wangfan04   (502) staff       (20)     4267 2024-02-01 05:22:53.000000 l3c-0.1.0.2/l3c/metalm/metalmv1.py
--rw-r--r--   0 wangfan04   (502) staff       (20)     5530 2024-02-01 05:22:53.000000 l3c-0.1.0.2/l3c/metalm/metalmv2.py
-drwxr-xr-x   0 wangfan04   (502) staff       (20)        0 2024-04-16 02:22:58.414862 l3c-0.1.0.2/l3c.egg-info/
--rw-r--r--   0 wangfan04   (502) staff       (20)      953 2024-04-16 02:22:58.000000 l3c-0.1.0.2/l3c.egg-info/PKG-INFO
--rw-r--r--   0 wangfan04   (502) staff       (20)     1075 2024-04-16 02:22:58.000000 l3c-0.1.0.2/l3c.egg-info/SOURCES.txt
--rw-r--r--   0 wangfan04   (502) staff       (20)        1 2024-04-16 02:22:58.000000 l3c-0.1.0.2/l3c.egg-info/dependency_links.txt
--rw-r--r--   0 wangfan04   (502) staff       (20)        1 2023-04-19 12:54:38.000000 l3c-0.1.0.2/l3c.egg-info/not-zip-safe
--rw-r--r--   0 wangfan04   (502) staff       (20)       84 2024-04-16 02:22:58.000000 l3c-0.1.0.2/l3c.egg-info/requires.txt
--rw-r--r--   0 wangfan04   (502) staff       (20)        4 2024-04-16 02:22:58.000000 l3c-0.1.0.2/l3c.egg-info/top_level.txt
--rw-r--r--   0 wangfan04   (502) staff       (20)       38 2024-04-16 02:22:58.426673 l3c-0.1.0.2/setup.cfg
--rwxr-xr-x   0 wangfan04   (502) staff       (20)     1814 2024-04-16 02:22:26.000000 l3c-0.1.0.2/setup.py
+drwxr-xr-x   0 wangfan04   (502) staff       (20)        0 2024-04-23 09:01:36.083829 l3c-0.1.0.3/
+-rw-r--r--   0 wangfan04   (502) staff       (20)    11357 2023-02-23 10:00:57.000000 l3c-0.1.0.3/LICENSE
+-rw-r--r--   0 wangfan04   (502) staff       (20)     1015 2024-04-23 09:01:36.083597 l3c-0.1.0.3/PKG-INFO
+-rw-r--r--   0 wangfan04   (502) staff       (20)      682 2024-04-23 08:58:47.000000 l3c-0.1.0.3/README.md
+drwxr-xr-x   0 wangfan04   (502) staff       (20)        0 2024-04-23 09:01:36.030724 l3c-0.1.0.3/l3c/
+-rw-r--r--   0 wangfan04   (502) staff       (20)      762 2023-02-23 10:11:06.000000 l3c-0.1.0.3/l3c/__init__.py
+drwxr-xr-x   0 wangfan04   (502) staff       (20)        0 2024-04-23 09:01:36.041768 l3c-0.1.0.3/l3c/bandits/
+-rw-r--r--   0 wangfan04   (502) staff       (20)      838 2023-02-23 10:11:06.000000 l3c-0.1.0.3/l3c/bandits/__init__.py
+-rw-r--r--   0 wangfan04   (502) staff       (20)     2717 2023-02-23 10:11:06.000000 l3c-0.1.0.3/l3c/bandits/bandits_env.py
+-rw-r--r--   0 wangfan04   (502) staff       (20)     1022 2023-02-23 10:32:50.000000 l3c-0.1.0.3/l3c/bandits/demo_thompson_sampling.py
+drwxr-xr-x   0 wangfan04   (502) staff       (20)        0 2024-04-23 09:01:36.042782 l3c-0.1.0.3/l3c/mazeworld/
+-rw-r--r--   0 wangfan04   (502) staff       (20)     1714 2024-02-20 08:03:46.000000 l3c-0.1.0.3/l3c/mazeworld/__init__.py
+drwxr-xr-x   0 wangfan04   (502) staff       (20)        0 2024-04-23 09:01:36.045919 l3c-0.1.0.3/l3c/mazeworld/agents/
+-rw-r--r--   0 wangfan04   (502) staff       (20)       45 2024-02-22 03:03:45.000000 l3c-0.1.0.3/l3c/mazeworld/agents/__init__.py
+-rw-r--r--   0 wangfan04   (502) staff       (20)     2857 2024-02-22 12:10:38.000000 l3c-0.1.0.3/l3c/mazeworld/agents/agent_base.py
+-rw-r--r--   0 wangfan04   (502) staff       (20)    11413 2024-04-16 01:44:52.000000 l3c-0.1.0.3/l3c/mazeworld/agents/smart_slam_agent.py
+drwxr-xr-x   0 wangfan04   (502) staff       (20)        0 2024-04-23 09:01:36.049859 l3c-0.1.0.3/l3c/mazeworld/demo/
+-rw-r--r--   0 wangfan04   (502) staff       (20)        0 2024-02-22 12:15:15.000000 l3c-0.1.0.3/l3c/mazeworld/demo/__init__.py
+-rw-r--r--   0 wangfan04   (502) staff       (20)     3609 2024-04-15 03:45:14.000000 l3c-0.1.0.3/l3c/mazeworld/demo/agent_play_demo.py
+-rw-r--r--   0 wangfan04   (502) staff       (20)     3844 2024-02-26 06:25:37.000000 l3c-0.1.0.3/l3c/mazeworld/demo/dump_maze.py
+-rw-r--r--   0 wangfan04   (502) staff       (20)     3366 2024-02-22 14:53:11.000000 l3c-0.1.0.3/l3c/mazeworld/demo/keyboard_play_demo.py
+drwxr-xr-x   0 wangfan04   (502) staff       (20)        0 2024-04-23 09:01:36.075228 l3c-0.1.0.3/l3c/mazeworld/envs/
+-rw-r--r--   0 wangfan04   (502) staff       (20)      258 2024-02-04 12:16:02.000000 l3c-0.1.0.3/l3c/mazeworld/envs/__init__.py
+-rw-r--r--   0 wangfan04   (502) staff       (20)     3644 2023-02-23 10:11:06.000000 l3c-0.1.0.3/l3c/mazeworld/envs/dynamics.py
+-rw-r--r--   0 wangfan04   (502) staff       (20)    14954 2024-04-23 08:19:34.000000 l3c-0.1.0.3/l3c/mazeworld/envs/maze_base.py
+-rw-r--r--   0 wangfan04   (502) staff       (20)     6324 2024-04-16 02:20:31.000000 l3c-0.1.0.3/l3c/mazeworld/envs/maze_continuous_3d.py
+-rw-r--r--   0 wangfan04   (502) staff       (20)     3345 2024-02-22 06:12:11.000000 l3c-0.1.0.3/l3c/mazeworld/envs/maze_discrete_2d.py
+-rw-r--r--   0 wangfan04   (502) staff       (20)     6849 2024-04-16 02:13:20.000000 l3c-0.1.0.3/l3c/mazeworld/envs/maze_discrete_3d.py
+-rw-r--r--   0 wangfan04   (502) staff       (20)     7295 2024-04-16 02:07:18.000000 l3c-0.1.0.3/l3c/mazeworld/envs/maze_env.py
+-rw-r--r--   0 wangfan04   (502) staff       (20)     9184 2024-02-20 01:19:41.000000 l3c-0.1.0.3/l3c/mazeworld/envs/maze_task.py
+-rw-r--r--   0 wangfan04   (502) staff       (20)    12366 2024-04-16 02:19:02.000000 l3c-0.1.0.3/l3c/mazeworld/envs/ray_caster_utils.py
+drwxr-xr-x   0 wangfan04   (502) staff       (20)        0 2024-04-23 09:01:36.078763 l3c-0.1.0.3/l3c/mazeworld/tests/
+-rw-r--r--   0 wangfan04   (502) staff       (20)        0 2024-02-22 12:15:23.000000 l3c-0.1.0.3/l3c/mazeworld/tests/__init__.py
+-rw-r--r--   0 wangfan04   (502) staff       (20)     2068 2024-02-04 15:06:43.000000 l3c-0.1.0.3/l3c/mazeworld/tests/test.py
+-rw-r--r--   0 wangfan04   (502) staff       (20)     2390 2024-02-22 11:56:16.000000 l3c-0.1.0.3/l3c/mazeworld/tests/test_agent.py
+drwxr-xr-x   0 wangfan04   (502) staff       (20)        0 2024-04-23 09:01:36.083042 l3c-0.1.0.3/l3c/rpl/
+-rw-r--r--   0 wangfan04   (502) staff       (20)     1088 2024-04-23 08:45:19.000000 l3c-0.1.0.3/l3c/rpl/__init__.py
+-rw-r--r--   0 wangfan04   (502) staff       (20)     2636 2024-04-23 08:54:57.000000 l3c-0.1.0.3/l3c/rpl/data_generator.py
+-rw-r--r--   0 wangfan04   (502) staff       (20)     4415 2024-04-23 08:46:14.000000 l3c-0.1.0.3/l3c/rpl/rplv1.py
+-rw-r--r--   0 wangfan04   (502) staff       (20)     5485 2024-04-23 08:46:24.000000 l3c-0.1.0.3/l3c/rpl/rplv2.py
+drwxr-xr-x   0 wangfan04   (502) staff       (20)        0 2024-04-23 09:01:36.038832 l3c-0.1.0.3/l3c.egg-info/
+-rw-r--r--   0 wangfan04   (502) staff       (20)     1015 2024-04-23 09:01:35.000000 l3c-0.1.0.3/l3c.egg-info/PKG-INFO
+-rw-r--r--   0 wangfan04   (502) staff       (20)     1057 2024-04-23 09:01:35.000000 l3c-0.1.0.3/l3c.egg-info/SOURCES.txt
+-rw-r--r--   0 wangfan04   (502) staff       (20)        1 2024-04-23 09:01:35.000000 l3c-0.1.0.3/l3c.egg-info/dependency_links.txt
+-rw-r--r--   0 wangfan04   (502) staff       (20)        1 2023-04-19 12:54:38.000000 l3c-0.1.0.3/l3c.egg-info/not-zip-safe
+-rw-r--r--   0 wangfan04   (502) staff       (20)       84 2024-04-23 09:01:35.000000 l3c-0.1.0.3/l3c.egg-info/requires.txt
+-rw-r--r--   0 wangfan04   (502) staff       (20)        4 2024-04-23 09:01:35.000000 l3c-0.1.0.3/l3c.egg-info/top_level.txt
+-rw-r--r--   0 wangfan04   (502) staff       (20)       38 2024-04-23 09:01:36.083882 l3c-0.1.0.3/setup.cfg
+-rwxr-xr-x   0 wangfan04   (502) staff       (20)     1814 2024-04-23 09:00:38.000000 l3c-0.1.0.3/setup.py
```

### Comparing `l3c-0.1.0.2/LICENSE` & `l3c-0.1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `l3c-0.1.0.2/PKG-INFO` & `l3c-0.1.0.3/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 2.1
 Name: l3c
-Version: 0.1.0.2
+Version: 0.1.0.3
 Summary: L3C provide abundant environments for Lifelong Learning (L3) in Context.
 Home-page: https://github.com/FutureAGI/L3C
 Author: WorldEditors
 Author-email: 
 License: Apache
 Platform: UNKNOWN
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # L3C - Life Long Learning In Context
 
-L3C provide abundant environments for Lifelong Learning (L3) in Context.
+L3C provide abundant environments for Lifelong Learning (L3) in Context, with long-term dependencies on the Contexts for task generalization.
 
 In-Context Learning entails a different learning process than that of gradient descent, as it involves feeding data through prompts instead. Our objective is to enhance lifelong learning research by utilizing prompts, which involve agents that learn through interaction in a forward-only manner.
 
 # Environments Updating
 
 - [MazeWorlds](l3c/mazeworld): 2D/3D maze generators for task generalization
 
-- [MetaLM](l3c/metalm): Meta language model dataset
+- [RPL](l3c/rpl): Randomized Pseudo-Language
 
 - [Bandits](l3c/bandits): Bandits task generalization
```

### Comparing `l3c-0.1.0.2/l3c/__init__.py` & `l3c-0.1.0.3/l3c/__init__.py`

 * *Files identical despite different names*

### Comparing `l3c-0.1.0.2/l3c/bandits/__init__.py` & `l3c-0.1.0.3/l3c/bandits/__init__.py`

 * *Files identical despite different names*

### Comparing `l3c-0.1.0.2/l3c/bandits/bandits_env.py` & `l3c-0.1.0.3/l3c/bandits/bandits_env.py`

 * *Files identical despite different names*

### Comparing `l3c-0.1.0.2/l3c/bandits/demo_thompson_sampling.py` & `l3c-0.1.0.3/l3c/bandits/demo_thompson_sampling.py`

 * *Files identical despite different names*

### Comparing `l3c-0.1.0.2/l3c/mazeworld/__init__.py` & `l3c-0.1.0.3/l3c/mazeworld/__init__.py`

 * *Files identical despite different names*

### Comparing `l3c-0.1.0.2/l3c/mazeworld/agents/agent_base.py` & `l3c-0.1.0.3/l3c/mazeworld/agents/agent_base.py`

 * *Files identical despite different names*

### Comparing `l3c-0.1.0.2/l3c/mazeworld/agents/smart_slam_agent.py` & `l3c-0.1.0.3/l3c/mazeworld/agents/smart_slam_agent.py`

 * *Files identical despite different names*

### Comparing `l3c-0.1.0.2/l3c/mazeworld/demo/agent_play_demo.py` & `l3c-0.1.0.3/l3c/mazeworld/demo/agent_play_demo.py`

 * *Files identical despite different names*

### Comparing `l3c-0.1.0.2/l3c/mazeworld/demo/dump_maze.py` & `l3c-0.1.0.3/l3c/mazeworld/demo/dump_maze.py`

 * *Files identical despite different names*

### Comparing `l3c-0.1.0.2/l3c/mazeworld/demo/keyboard_play_demo.py` & `l3c-0.1.0.3/l3c/mazeworld/demo/keyboard_play_demo.py`

 * *Files identical despite different names*

### Comparing `l3c-0.1.0.2/l3c/mazeworld/envs/dynamics.py` & `l3c-0.1.0.3/l3c/mazeworld/envs/dynamics.py`

 * *Files identical despite different names*

### Comparing `l3c-0.1.0.2/l3c/mazeworld/envs/maze_base.py` & `l3c-0.1.0.3/l3c/mazeworld/envs/maze_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -251,14 +251,19 @@
             noise = (factor - 0.5) * 0.10
             p = self._agent_trajectory[i]
             n = self._agent_trajectory[i+1]
             p = [(p[0] + 0.5 + noise) * self._render_cell_size, (p[1] + 0.5 + noise) *  self._render_cell_size]
             n = [(n[0] + 0.5 + noise) * self._render_cell_size, (n[1] + 0.5 + noise) *  self._render_cell_size]
             pygame.draw.line(traj_screen, pygame.Color(int(255 * factor), int(255 * (1 - factor)), 0, 255), p, n, width=2)
 
+        for landmarks_id, (x,y) in enumerate(self._landmarks_coordinates):
+            pygame.draw.rect(traj_screen, landmarks_color(landmarks_id), 
+                    (x * self._render_cell_size, y * self._render_cell_size,
+                    self._render_cell_size, self._render_cell_size), width=0)
+
         # paint some additional surfaces where necessary
         if(additional != None):
             for i in range(len(additional["surfaces"])):
                 traj_screen.blit(additional["surfaces"][i], (self._view_size, 0))
                 pygame.image.save(traj_screen, file_name.split(".")[0] + additional["file_names"][i] + ".png")
         else:
             pygame.image.save(traj_screen, file_name)
```

### Comparing `l3c-0.1.0.2/l3c/mazeworld/envs/maze_continuous_3d.py` & `l3c-0.1.0.3/l3c/mazeworld/envs/maze_continuous_3d.py`

 * *Files identical despite different names*

### Comparing `l3c-0.1.0.2/l3c/mazeworld/envs/maze_discrete_2d.py` & `l3c-0.1.0.3/l3c/mazeworld/envs/maze_discrete_2d.py`

 * *Files identical despite different names*

### Comparing `l3c-0.1.0.2/l3c/mazeworld/envs/maze_discrete_3d.py` & `l3c-0.1.0.3/l3c/mazeworld/envs/maze_discrete_3d.py`

 * *Files identical despite different names*

### Comparing `l3c-0.1.0.2/l3c/mazeworld/envs/maze_env.py` & `l3c-0.1.0.3/l3c/mazeworld/envs/maze_env.py`

 * *Files identical despite different names*

### Comparing `l3c-0.1.0.2/l3c/mazeworld/envs/maze_task.py` & `l3c-0.1.0.3/l3c/mazeworld/envs/maze_task.py`

 * *Files identical despite different names*

### Comparing `l3c-0.1.0.2/l3c/mazeworld/envs/ray_caster_utils.py` & `l3c-0.1.0.3/l3c/mazeworld/envs/ray_caster_utils.py`

 * *Files identical despite different names*

### Comparing `l3c-0.1.0.2/l3c/mazeworld/tests/test.py` & `l3c-0.1.0.3/l3c/mazeworld/tests/test.py`

 * *Files identical despite different names*

### Comparing `l3c-0.1.0.2/l3c/mazeworld/tests/test_agent.py` & `l3c-0.1.0.3/l3c/mazeworld/tests/test_agent.py`

 * *Files identical despite different names*

### Comparing `l3c-0.1.0.2/l3c/metalm/__init__.py` & `l3c-0.1.0.3/l3c/rpl/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,31 +9,31 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from gym.envs.registration import register
-from l3c.metalm.metalmv1 import MetaLMv1
-from l3c.metalm.metalmv2 import MetaLMv2
+from l3c.rpl.rplv1 import RPLv1
+from l3c.rpl.rplv2 import RPLv2
 
 register(
-    id='meta-lm-v1',
-    entry_point='l3c.metalm:MetaLMv1',
+    id='randomized-pseudo-language-v1',
+    entry_point='l3c.rpl:RPLv1',
     kwargs={"V": 64,
         "n": 10,
         "l": 64,
         "e": 0.10,
         "L": 2048
     }
 )
 
 register(
-    id='meta-lm-v2',
-    entry_point='l3c.metalm:MetaLMv2',
+    id='randomized-pseudo-language-v2',
+    entry_point='l3c.rpl:RPLv2',
     kwargs={"V": 64,
         "n": 16,
         "N": 16,
         "e": 0.10,
         "L": 2048
     }
 )
```

### Comparing `l3c-0.1.0.2/l3c/metalm/data_generator.py` & `l3c-0.1.0.3/l3c/rpl/data_generator.py`

 * *Files 22% similar despite different names*

```diff
@@ -12,46 +12,52 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 # This file is used to generate data for meta language models
 
 import sys
 import argparse
-from l3c.metalm import MetaLMv1
-from l3c.metalm import MetaLMv2
+from l3c.rpl import RPLv1
+from l3c.rpl import RPLv2
 
 if __name__=='__main__':
     parser = argparse.ArgumentParser(description='Generating Pseudo-Training Data')
-    parser.add_argument('--version', type=str, default='v1')
+    parser.add_argument('--version', type=str, choices=['v1', 'v2'], default='v2')
     parser.add_argument('--vocab_size', type=int, default=64)
     parser.add_argument('--embedding_size', type=int, default=16)
     parser.add_argument('--hidden_size', type=int, default=16)
     parser.add_argument('--elements_length', type=int, default=64)
     parser.add_argument('--elements_number', type=int, default=10)
     parser.add_argument('--error_rate', type=float, default=0.20)
     parser.add_argument('--n_gram', type=float, default=3)
     parser.add_argument('--sequence_length', type=int, default=4096)
     parser.add_argument('--samples', type=int, default=100)
+    parser.add_argument('--output_type', type=str, choices=['txt', 'npy'], default='txt')
     parser.add_argument('--output', type=str, default=None)
 
     args = parser.parse_args()
 
     if(args.version == 'v1'):
-        dataset = MetaLMv1(
+        dataset = RPLv1(
                 V=args.vocab_size,
                 n=args.elements_number,
                 l=args.elements_length,
                 e=args.error_rate,
                 L=args.sequence_length)
     elif(args.version == 'v2'):
-        dataset = MetaLMv2(
+        dataset = RPLv2(
                 V=args.vocab_size,
                 n=args.n_gram,
                 d=args.embedding_size,
                 N=args.hidden_size,
                 e=args.error_rate,
                 L=args.sequence_length)
 
-    if(args.output is None):
-        dataset.generate_to_file(args.samples, sys.stdout)
-    else:
-        dataset.generate_to_file(args.samples, args.output)
+    if(args.output_type == 'npy'):
+        if(args.output is None):
+            raise Exception("Must specify --output when output_type is npy")
+        dataset.generate_npy(args.samples, args.output)
+    elif(args.output_type == 'txt'):
+        if(args.output is None):
+            dataset.generate_text(args.samples, sys.stdout)
+        else:
+            dataset.generate_text(args.samples, args.output)
```

### Comparing `l3c-0.1.0.2/l3c/metalm/metalmv1.py` & `l3c-0.1.0.3/l3c/rpl/rplv1.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 import sys
 import _io
 import numpy
 import gym
 from numpy import random
 
-class MetaLMv1(gym.Env):
+class RPLv1(gym.Env):
     """
     Meta Language Model
     MetaLM(V, n, l, e, L) generates n Exponential(1/l)-length sequences, which appears repeatedly until reaching length L
     Each time it repeats, we add a noise by replacing the number with e probablity 
     V: Vocabulary Size
     l: mean repeating length
     e: noise ratio
@@ -92,27 +92,31 @@
             fea, lab = self.data_generator(seed=seed)
             features.append(fea.tolist())
             labels.append(lab.tolist())
         features = numpy.asarray(features)
         labels = numpy.asarray(labels)
         return features, labels
 
-    def generate_to_file(self, size, output_stream):
+    def generate_text(self, size, output_stream):
         features, labels = self.batch_generator(size)
         if(isinstance(output_stream, _io.TextIOWrapper)):
             need_close = False
         elif(isinstance(output_stream, str)):
             output_stream = open(output_stream, "w")
             need_close = True
         for i in range(features.shape[0]):
             output_stream.write("\t".join(map(lambda x: "%d,%d"%(x[0],x[1]), zip(features[i].tolist(), labels[i].tolist()))))
             output_stream.write("\n")
         if(need_close):
             output_stream.close()
 
+    def generate_npy(self, size, file_name):
+        feas, labs = self.batch_generator(size)
+        numpy.save(file, numpy.stack([feas, labs], axis=0))
+
     @property
     def VocabSize(self):
         return self.V
 
     @property
     def SepID(self):
         return 0
```

### Comparing `l3c-0.1.0.2/l3c/metalm/metalmv2.py` & `l3c-0.1.0.3/l3c/rpl/rplv2.py`

 * *Files 5% similar despite different names*

```diff
@@ -83,15 +83,15 @@
             tok_cnt += cur_prob.shape[0]
 
             seqs.append(cur_tok)
         print("GT Perplexity: %f" % (ppl / tok_cnt))
 
         return numpy.transpose(numpy.asarray(seqs, dtype="int32"))
 
-class MetaLMv2(gym.Env):
+class RPLv2(gym.Env):
     """
     Pseudo Langauge Generated from RNN models
     V: vocabulary size
     d: embedding size (input size)
     n: n-gram
     N: hidden size
     e: inverse of softmax - temporature
@@ -111,46 +111,46 @@
         self.N = N
         self.hardness = 1.0/e
         assert n > 1 and V > 1 and N > 1 and L > 1 
 
     def data_generator(self, seed=None):
         nn = RandomRNN(n_emb = self.d, n_gram=self.n, n_hidden = self.N, n_vocab = self.V, hardness=self.hardness, seed=seed)
         tokens = nn.forward(self.L)[0]
-        feas = tokens[:-1]
-        labs = tokens[1:]
-        return feas, labs
+        return tokens
 
     def batch_generator(self, batch_size, seed=None):
         nn = RandomRNN(batch = batch_size, n_emb = self.d, n_gram=self.n, n_hidden = self.N, n_vocab = self.V, hardness=self.hardness, seed=seed)
         tokens = nn.forward(self.L)
-        feas = tokens[:,:-1]
-        labs = tokens[:,1:]
-        return feas, labs
+        return tokens
 
-    def generate_to_file(self, size, output_stream):
-        feas,labs = self.batch_generator(size)
+    def generate_text(self, size, output_stream):
+        tokens = self.batch_generator(size)
         if(isinstance(output_stream, _io.TextIOWrapper)):
             need_close = False
         elif(isinstance(output_stream, str)):
             output_stream = open(output_stream, "w")
             need_close = True
-        for i in range(feas.shape[0]):
-            output_stream.write("\t".join(map(lambda x:"%s,%s"%(x[0],x[1]), zip(feas[i].tolist(), labs[i].tolist()))))
+        for i in range(tokens.shape[0]):
+            output_stream.write("\t".join(map(str, tokens[i].tolist())))
             output_stream.write("\n")
         if(need_close):
             output_stream.close()
 
+    def generate_npy(self, size, file_name):
+        tokens = self.batch_generator(size)
+        numpy.save(file_name, tokens)
+
     @property
     def VocabSize(self):
-        return self.V + 1
+        return self.V
 
     @property
     def SepID(self):
         raise Exception("Not Defined")
 
     @property
     def MaskID(self):
-        return 0
+        return -1
 
     @property
     def PaddingID(self):
-        return 0
+        return -1
```

### Comparing `l3c-0.1.0.2/l3c.egg-info/PKG-INFO` & `l3c-0.1.0.3/l3c.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 2.1
 Name: l3c
-Version: 0.1.0.2
+Version: 0.1.0.3
 Summary: L3C provide abundant environments for Lifelong Learning (L3) in Context.
 Home-page: https://github.com/FutureAGI/L3C
 Author: WorldEditors
 Author-email: 
 License: Apache
 Platform: UNKNOWN
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # L3C - Life Long Learning In Context
 
-L3C provide abundant environments for Lifelong Learning (L3) in Context.
+L3C provide abundant environments for Lifelong Learning (L3) in Context, with long-term dependencies on the Contexts for task generalization.
 
 In-Context Learning entails a different learning process than that of gradient descent, as it involves feeding data through prompts instead. Our objective is to enhance lifelong learning research by utilizing prompts, which involve agents that learn through interaction in a forward-only manner.
 
 # Environments Updating
 
 - [MazeWorlds](l3c/mazeworld): 2D/3D maze generators for task generalization
 
-- [MetaLM](l3c/metalm): Meta language model dataset
+- [RPL](l3c/rpl): Randomized Pseudo-Language
 
 - [Bandits](l3c/bandits): Bandits task generalization
```

### Comparing `l3c-0.1.0.2/l3c.egg-info/SOURCES.txt` & `l3c-0.1.0.3/l3c.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -27,11 +27,11 @@
 l3c/mazeworld/envs/maze_discrete_3d.py
 l3c/mazeworld/envs/maze_env.py
 l3c/mazeworld/envs/maze_task.py
 l3c/mazeworld/envs/ray_caster_utils.py
 l3c/mazeworld/tests/__init__.py
 l3c/mazeworld/tests/test.py
 l3c/mazeworld/tests/test_agent.py
-l3c/metalm/__init__.py
-l3c/metalm/data_generator.py
-l3c/metalm/metalmv1.py
-l3c/metalm/metalmv2.py
+l3c/rpl/__init__.py
+l3c/rpl/data_generator.py
+l3c/rpl/rplv1.py
+l3c/rpl/rplv2.py
```

### Comparing `l3c-0.1.0.2/setup.py` & `l3c-0.1.0.3/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import io
 from setuptools import setup, find_packages
 
-__version__ = '0.1.0.2'
+__version__ = '0.1.0.3'
 
 with io.open('README.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
 
 setup(
     name='l3c',
     version=__version__,
```

