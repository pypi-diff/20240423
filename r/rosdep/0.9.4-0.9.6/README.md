# Comparing `tmp/rosdep-0.9.4.tar.gz` & `tmp/rosdep-0.9.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rosdep-0.9.4.tar", last modified: Mon Jun  4 22:50:02 2012, max compression, from Unix
+gzip compressed data, was "rosdep-0.9.6.tar", last modified: Thu Aug  9 20:31:38 2012, max compression, from Unix
```

## Comparing `rosdep-0.9.4.tar` & `rosdep-0.9.6.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxr-xr-x   0 tfoote    (1020) wgusers   (9000)        0 2012-06-04 22:50:02.000000 rosdep-0.9.4/
--rw-r--r--   0 tfoote    (1020) wgusers   (9000)     1030 2012-04-27 21:48:00.000000 rosdep-0.9.4/setup.py
-drwxr-xr-x   0 tfoote    (1020) wgusers   (9000)        0 2012-06-04 22:50:02.000000 rosdep-0.9.4/src/
-drwxr-xr-x   0 tfoote    (1020) wgusers   (9000)        0 2012-06-04 22:50:02.000000 rosdep-0.9.4/src/rosdep2/
--rw-r--r--   0 tfoote    (1020) wgusers   (9000)    22572 2012-04-27 22:10:34.000000 rosdep-0.9.4/src/rosdep2/installers.py
--rw-r--r--   0 tfoote    (1020) wgusers   (9000)     6284 2012-04-27 22:20:25.000000 rosdep-0.9.4/src/rosdep2/dependency_graph.py
--rw-r--r--   0 tfoote    (1020) wgusers   (9000)     5996 2012-04-27 21:48:00.000000 rosdep-0.9.4/src/rosdep2/rospkg_loader.py
--rw-r--r--   0 tfoote    (1020) wgusers   (9000)     4977 2012-04-27 21:48:00.000000 rosdep-0.9.4/src/rosdep2/model.py
--rw-r--r--   0 tfoote    (1020) wgusers   (9000)     3334 2012-04-27 21:48:00.000000 rosdep-0.9.4/src/rosdep2/core.py
--rw-r--r--   0 tfoote    (1020) wgusers   (9000)     3113 2012-04-27 21:48:00.000000 rosdep-0.9.4/src/rosdep2/shell_utils.py
--rw-r--r--   0 tfoote    (1020) wgusers   (9000)     2863 2012-04-27 21:48:00.000000 rosdep-0.9.4/src/rosdep2/rep3.py
--rw-r--r--   0 tfoote    (1020) wgusers   (9000)    23029 2012-04-27 22:08:48.000000 rosdep-0.9.4/src/rosdep2/main.py
--rw-r--r--   0 tfoote    (1020) wgusers   (9000)    25236 2012-04-27 22:19:52.000000 rosdep-0.9.4/src/rosdep2/lookup.py
-drwxr-xr-x   0 tfoote    (1020) wgusers   (9000)        0 2012-06-04 22:50:02.000000 rosdep-0.9.4/src/rosdep2/platforms/
--rw-r--r--   0 tfoote    (1020) wgusers   (9000)     5491 2012-05-11 07:12:46.000000 rosdep-0.9.4/src/rosdep2/platforms/osx.py
--rw-r--r--   0 tfoote    (1020) wgusers   (9000)     4787 2012-06-03 20:55:15.000000 rosdep-0.9.4/src/rosdep2/platforms/gentoo.py
--rw-r--r--   0 tfoote    (1020) wgusers   (9000)     2847 2012-04-27 21:48:00.000000 rosdep-0.9.4/src/rosdep2/platforms/arch.py
--rw-r--r--   0 tfoote    (1020) wgusers   (9000)     3102 2012-04-27 21:48:00.000000 rosdep-0.9.4/src/rosdep2/platforms/cygwin.py
--rw-r--r--   0 tfoote    (1020) wgusers   (9000)     3797 2012-04-27 21:48:00.000000 rosdep-0.9.4/src/rosdep2/platforms/redhat.py
--rw-r--r--   0 tfoote    (1020) wgusers   (9000)     1793 2012-04-27 21:48:00.000000 rosdep-0.9.4/src/rosdep2/platforms/brewmaker.py
--rw-r--r--   0 tfoote    (1020) wgusers   (9000)     4441 2012-04-27 21:48:00.000000 rosdep-0.9.4/src/rosdep2/platforms/debian.py
--rw-r--r--   0 tfoote    (1020) wgusers   (9000)     2889 2012-04-27 21:48:00.000000 rosdep-0.9.4/src/rosdep2/platforms/opensuse.py
--rw-r--r--   0 tfoote    (1020) wgusers   (9000)     3259 2012-04-27 21:50:32.000000 rosdep-0.9.4/src/rosdep2/platforms/pip.py
--rw-r--r--   0 tfoote    (1020) wgusers   (9000)     3583 2012-04-27 21:48:00.000000 rosdep-0.9.4/src/rosdep2/platforms/freebsd.py
--rw-r--r--   0 tfoote    (1020) wgusers   (9000)    10919 2012-04-27 21:48:00.000000 rosdep-0.9.4/src/rosdep2/platforms/source.py
--rw-r--r--   0 tfoote    (1020) wgusers   (9000)        0 2012-04-27 21:48:00.000000 rosdep-0.9.4/src/rosdep2/platforms/__init__.py
--rw-r--r--   0 tfoote    (1020) wgusers   (9000)     3861 2012-04-27 21:48:00.000000 rosdep-0.9.4/src/rosdep2/gbpdistro_support.py
--rw-r--r--   0 tfoote    (1020) wgusers   (9000)     4109 2012-04-27 21:48:00.000000 rosdep-0.9.4/src/rosdep2/catkin_support.py
--rw-r--r--   0 tfoote    (1020) wgusers   (9000)     4119 2012-04-27 21:48:00.000000 rosdep-0.9.4/src/rosdep2/loader.py
--rw-r--r--   0 tfoote    (1020) wgusers   (9000)     5140 2012-06-04 22:47:46.000000 rosdep-0.9.4/src/rosdep2/__init__.py
--rw-r--r--   0 tfoote    (1020) wgusers   (9000)    20693 2012-04-27 21:48:00.000000 rosdep-0.9.4/src/rosdep2/sources_list.py
-drwxr-xr-x   0 tfoote    (1020) wgusers   (9000)        0 2012-06-04 22:50:02.000000 rosdep-0.9.4/src/rosdep.egg-info/
--rw-r--r--   0 tfoote    (1020) wgusers   (9000)     1628 2012-06-04 22:50:02.000000 rosdep-0.9.4/src/rosdep.egg-info/SOURCES.txt
--rw-r--r--   0 tfoote    (1020) wgusers   (9000)      535 2012-06-04 22:50:02.000000 rosdep-0.9.4/src/rosdep.egg-info/PKG-INFO
--rw-r--r--   0 tfoote    (1020) wgusers   (9000)        6 2012-06-04 22:50:02.000000 rosdep-0.9.4/src/rosdep.egg-info/requires.txt
--rw-r--r--   0 tfoote    (1020) wgusers   (9000)        1 2012-06-04 22:50:02.000000 rosdep-0.9.4/src/rosdep.egg-info/dependency_links.txt
--rw-r--r--   0 tfoote    (1020) wgusers   (9000)        8 2012-06-04 22:50:02.000000 rosdep-0.9.4/src/rosdep.egg-info/top_level.txt
-drwxr-xr-x   0 tfoote    (1020) wgusers   (9000)        0 2012-06-04 22:50:02.000000 rosdep-0.9.4/test/
--rw-r--r--   0 tfoote    (1020) wgusers   (9000)     2725 2012-04-27 21:48:00.000000 rosdep-0.9.4/test/test_rosdep_cygwin.py
--rw-r--r--   0 tfoote    (1020) wgusers   (9000)     8895 2012-04-27 21:48:00.000000 rosdep-0.9.4/test/test_rosdep_main.py
--rw-r--r--   0 tfoote    (1020) wgusers   (9000)     2593 2012-04-27 21:48:00.000000 rosdep-0.9.4/test/test_rosdep_rep3.py
--rw-r--r--   0 tfoote    (1020) wgusers   (9000)     4111 2012-04-27 21:48:00.000000 rosdep-0.9.4/test/test_rosdep_pip.py
--rw-r--r--   0 tfoote    (1020) wgusers   (9000)     7470 2012-06-04 22:42:58.000000 rosdep-0.9.4/test/test_rosdep_gentoo.py
--rw-r--r--   0 tfoote    (1020) wgusers   (9000)     6467 2012-04-27 21:48:00.000000 rosdep-0.9.4/test/test_rosdep_gbpdistro_support.py
--rw-r--r--   0 tfoote    (1020) wgusers   (9000)     2651 2012-04-27 21:48:00.000000 rosdep-0.9.4/test/test_rosdep_opensuse.py
--rw-r--r--   0 tfoote    (1020) wgusers   (9000)     2375 2012-04-27 21:48:00.000000 rosdep-0.9.4/test/test_rosdep.py
--rw-r--r--   0 tfoote    (1020) wgusers   (9000)     4201 2012-04-27 21:48:00.000000 rosdep-0.9.4/test/test_rosdep_osx.py
--rw-r--r--   0 tfoote    (1020) wgusers   (9000)     2149 2012-04-27 21:48:00.000000 rosdep-0.9.4/test/test_rosdep_core.py
--rw-r--r--   0 tfoote    (1020) wgusers   (9000)     6598 2012-04-27 21:48:00.000000 rosdep-0.9.4/test/test_rosdep_rospkg_loader.py
--rw-r--r--   0 tfoote    (1020) wgusers   (9000)    10918 2012-04-27 21:48:00.000000 rosdep-0.9.4/test/test_rosdep_source.py
--rw-r--r--   0 tfoote    (1020) wgusers   (9000)      592 2012-04-27 21:48:00.000000 rosdep-0.9.4/test/test_rosdep_catkin_support.py
--rw-r--r--   0 tfoote    (1020) wgusers   (9000)     2783 2012-04-27 21:48:00.000000 rosdep-0.9.4/test/test_rosdep_arch.py
--rw-r--r--   0 tfoote    (1020) wgusers   (9000)     3679 2012-04-27 21:48:00.000000 rosdep-0.9.4/test/test_rosdep_model.py
--rw-r--r--   0 tfoote    (1020) wgusers   (9000)    19136 2012-04-27 21:50:32.000000 rosdep-0.9.4/test/test_rosdep_lookup.py
--rw-r--r--   0 tfoote    (1020) wgusers   (9000)    18229 2012-04-27 21:48:00.000000 rosdep-0.9.4/test/test_rosdep_sources_list.py
--rw-r--r--   0 tfoote    (1020) wgusers   (9000)     2986 2012-04-27 21:48:00.000000 rosdep-0.9.4/test/test_rosdep_redhat.py
--rw-r--r--   0 tfoote    (1020) wgusers   (9000)     7778 2012-04-27 21:50:32.000000 rosdep-0.9.4/test/test_rosdep_dependency_graph.py
--rw-r--r--   0 tfoote    (1020) wgusers   (9000)     2463 2012-04-27 21:48:00.000000 rosdep-0.9.4/test/test_rosdep_loader.py
--rw-r--r--   0 tfoote    (1020) wgusers   (9000)     3480 2012-04-27 21:48:00.000000 rosdep-0.9.4/test/test_rosdep_debian.py
--rw-r--r--   0 tfoote    (1020) wgusers   (9000)    22386 2012-04-27 21:50:32.000000 rosdep-0.9.4/test/test_rosdep_installers.py
--rw-r--r--   0 tfoote    (1020) wgusers   (9000)     2088 2012-04-27 21:48:00.000000 rosdep-0.9.4/test/test_rosdep_shell_utils.py
--rw-r--r--   0 tfoote    (1020) wgusers   (9000)      535 2012-06-04 22:50:02.000000 rosdep-0.9.4/PKG-INFO
--rw-r--r--   0 tfoote    (1020) wgusers   (9000)       59 2012-06-04 22:50:02.000000 rosdep-0.9.4/setup.cfg
-drwxr-xr-x   0 tfoote    (1020) wgusers   (9000)        0 2012-06-04 22:50:02.000000 rosdep-0.9.4/scripts/
--rwxr-xr-x   0 tfoote    (1020) wgusers   (9000)       74 2012-04-27 21:48:00.000000 rosdep-0.9.4/scripts/rosdep
--rwxr-xr-x   0 tfoote    (1020) wgusers   (9000)     2563 2012-04-27 21:48:00.000000 rosdep-0.9.4/scripts/rosdep-source
--rwxr-xr-x   0 tfoote    (1020) wgusers   (9000)      946 2012-04-27 21:48:00.000000 rosdep-0.9.4/scripts/rosdep-gbp-brew
+drwxr-xr-x   0 tfoote    (1020) wgusers   (9000)        0 2012-08-09 20:31:38.000000 rosdep-0.9.6/
+-rw-r--r--   0 tfoote    (1020) wgusers   (9000)     1030 2012-04-27 21:48:00.000000 rosdep-0.9.6/setup.py
+drwxr-xr-x   0 tfoote    (1020) wgusers   (9000)        0 2012-08-09 20:31:38.000000 rosdep-0.9.6/src/
+drwxr-xr-x   0 tfoote    (1020) wgusers   (9000)        0 2012-08-09 20:31:38.000000 rosdep-0.9.6/src/rosdep2/
+-rw-r--r--   0 tfoote    (1020) wgusers   (9000)    22572 2012-04-27 22:10:34.000000 rosdep-0.9.6/src/rosdep2/installers.py
+-rw-r--r--   0 tfoote    (1020) wgusers   (9000)     6284 2012-04-27 22:20:25.000000 rosdep-0.9.6/src/rosdep2/dependency_graph.py
+-rw-r--r--   0 tfoote    (1020) wgusers   (9000)     5996 2012-04-27 21:48:00.000000 rosdep-0.9.6/src/rosdep2/rospkg_loader.py
+-rw-r--r--   0 tfoote    (1020) wgusers   (9000)     4977 2012-04-27 21:48:00.000000 rosdep-0.9.6/src/rosdep2/model.py
+-rw-r--r--   0 tfoote    (1020) wgusers   (9000)     3334 2012-04-27 21:48:00.000000 rosdep-0.9.6/src/rosdep2/core.py
+-rw-r--r--   0 tfoote    (1020) wgusers   (9000)     3113 2012-04-27 21:48:00.000000 rosdep-0.9.6/src/rosdep2/shell_utils.py
+-rw-r--r--   0 tfoote    (1020) wgusers   (9000)     2863 2012-04-27 21:48:00.000000 rosdep-0.9.6/src/rosdep2/rep3.py
+-rw-r--r--   0 tfoote    (1020) wgusers   (9000)    23100 2012-06-14 20:47:22.000000 rosdep-0.9.6/src/rosdep2/main.py
+-rw-r--r--   0 tfoote    (1020) wgusers   (9000)    25236 2012-04-27 22:19:52.000000 rosdep-0.9.6/src/rosdep2/lookup.py
+drwxr-xr-x   0 tfoote    (1020) wgusers   (9000)        0 2012-08-09 20:31:38.000000 rosdep-0.9.6/src/rosdep2/platforms/
+-rw-r--r--   0 tfoote    (1020) wgusers   (9000)     5491 2012-05-11 07:12:46.000000 rosdep-0.9.6/src/rosdep2/platforms/osx.py
+-rw-r--r--   0 tfoote    (1020) wgusers   (9000)     4787 2012-06-03 20:55:15.000000 rosdep-0.9.6/src/rosdep2/platforms/gentoo.py
+-rw-r--r--   0 tfoote    (1020) wgusers   (9000)     2847 2012-04-27 21:48:00.000000 rosdep-0.9.6/src/rosdep2/platforms/arch.py
+-rw-r--r--   0 tfoote    (1020) wgusers   (9000)     3102 2012-04-27 21:48:00.000000 rosdep-0.9.6/src/rosdep2/platforms/cygwin.py
+-rw-r--r--   0 tfoote    (1020) wgusers   (9000)     3797 2012-04-27 21:48:00.000000 rosdep-0.9.6/src/rosdep2/platforms/redhat.py
+-rw-r--r--   0 tfoote    (1020) wgusers   (9000)     1793 2012-04-27 21:48:00.000000 rosdep-0.9.6/src/rosdep2/platforms/brewmaker.py
+-rw-r--r--   0 tfoote    (1020) wgusers   (9000)     4441 2012-04-27 21:48:00.000000 rosdep-0.9.6/src/rosdep2/platforms/debian.py
+-rw-r--r--   0 tfoote    (1020) wgusers   (9000)     2889 2012-04-27 21:48:00.000000 rosdep-0.9.6/src/rosdep2/platforms/opensuse.py
+-rw-r--r--   0 tfoote    (1020) wgusers   (9000)     3259 2012-04-27 21:50:32.000000 rosdep-0.9.6/src/rosdep2/platforms/pip.py
+-rw-r--r--   0 tfoote    (1020) wgusers   (9000)     3583 2012-04-27 21:48:00.000000 rosdep-0.9.6/src/rosdep2/platforms/freebsd.py
+-rw-r--r--   0 tfoote    (1020) wgusers   (9000)    10919 2012-04-27 21:48:00.000000 rosdep-0.9.6/src/rosdep2/platforms/source.py
+-rw-r--r--   0 tfoote    (1020) wgusers   (9000)        0 2012-04-27 21:48:00.000000 rosdep-0.9.6/src/rosdep2/platforms/__init__.py
+-rw-r--r--   0 tfoote    (1020) wgusers   (9000)     3861 2012-04-27 21:48:00.000000 rosdep-0.9.6/src/rosdep2/gbpdistro_support.py
+-rw-r--r--   0 tfoote    (1020) wgusers   (9000)     3694 2012-08-09 20:08:35.000000 rosdep-0.9.6/src/rosdep2/catkin_support.py
+-rw-r--r--   0 tfoote    (1020) wgusers   (9000)     4119 2012-04-27 21:48:00.000000 rosdep-0.9.6/src/rosdep2/loader.py
+-rw-r--r--   0 tfoote    (1020) wgusers   (9000)     5140 2012-08-09 20:21:46.000000 rosdep-0.9.6/src/rosdep2/__init__.py
+-rw-r--r--   0 tfoote    (1020) wgusers   (9000)    20693 2012-04-27 21:48:00.000000 rosdep-0.9.6/src/rosdep2/sources_list.py
+drwxr-xr-x   0 tfoote    (1020) wgusers   (9000)        0 2012-08-09 20:31:38.000000 rosdep-0.9.6/src/rosdep.egg-info/
+-rw-r--r--   0 tfoote    (1020) wgusers   (9000)     1628 2012-08-09 20:31:38.000000 rosdep-0.9.6/src/rosdep.egg-info/SOURCES.txt
+-rw-r--r--   0 tfoote    (1020) wgusers   (9000)      535 2012-08-09 20:31:38.000000 rosdep-0.9.6/src/rosdep.egg-info/PKG-INFO
+-rw-r--r--   0 tfoote    (1020) wgusers   (9000)        6 2012-08-09 20:31:38.000000 rosdep-0.9.6/src/rosdep.egg-info/requires.txt
+-rw-r--r--   0 tfoote    (1020) wgusers   (9000)        1 2012-08-09 20:31:38.000000 rosdep-0.9.6/src/rosdep.egg-info/dependency_links.txt
+-rw-r--r--   0 tfoote    (1020) wgusers   (9000)        8 2012-08-09 20:31:38.000000 rosdep-0.9.6/src/rosdep.egg-info/top_level.txt
+drwxr-xr-x   0 tfoote    (1020) wgusers   (9000)        0 2012-08-09 20:31:38.000000 rosdep-0.9.6/test/
+-rw-r--r--   0 tfoote    (1020) wgusers   (9000)     2725 2012-04-27 21:48:00.000000 rosdep-0.9.6/test/test_rosdep_cygwin.py
+-rw-r--r--   0 tfoote    (1020) wgusers   (9000)     8895 2012-04-27 21:48:00.000000 rosdep-0.9.6/test/test_rosdep_main.py
+-rw-r--r--   0 tfoote    (1020) wgusers   (9000)     2593 2012-04-27 21:48:00.000000 rosdep-0.9.6/test/test_rosdep_rep3.py
+-rw-r--r--   0 tfoote    (1020) wgusers   (9000)     4111 2012-04-27 21:48:00.000000 rosdep-0.9.6/test/test_rosdep_pip.py
+-rw-r--r--   0 tfoote    (1020) wgusers   (9000)     7470 2012-06-04 22:42:58.000000 rosdep-0.9.6/test/test_rosdep_gentoo.py
+-rw-r--r--   0 tfoote    (1020) wgusers   (9000)     6467 2012-04-27 21:48:00.000000 rosdep-0.9.6/test/test_rosdep_gbpdistro_support.py
+-rw-r--r--   0 tfoote    (1020) wgusers   (9000)     2651 2012-04-27 21:48:00.000000 rosdep-0.9.6/test/test_rosdep_opensuse.py
+-rw-r--r--   0 tfoote    (1020) wgusers   (9000)     2375 2012-04-27 21:48:00.000000 rosdep-0.9.6/test/test_rosdep.py
+-rw-r--r--   0 tfoote    (1020) wgusers   (9000)     4201 2012-04-27 21:48:00.000000 rosdep-0.9.6/test/test_rosdep_osx.py
+-rw-r--r--   0 tfoote    (1020) wgusers   (9000)     2149 2012-04-27 21:48:00.000000 rosdep-0.9.6/test/test_rosdep_core.py
+-rw-r--r--   0 tfoote    (1020) wgusers   (9000)     6598 2012-04-27 21:48:00.000000 rosdep-0.9.6/test/test_rosdep_rospkg_loader.py
+-rw-r--r--   0 tfoote    (1020) wgusers   (9000)    10918 2012-04-27 21:48:00.000000 rosdep-0.9.6/test/test_rosdep_source.py
+-rw-r--r--   0 tfoote    (1020) wgusers   (9000)      647 2012-08-09 20:14:36.000000 rosdep-0.9.6/test/test_rosdep_catkin_support.py
+-rw-r--r--   0 tfoote    (1020) wgusers   (9000)     2783 2012-04-27 21:48:00.000000 rosdep-0.9.6/test/test_rosdep_arch.py
+-rw-r--r--   0 tfoote    (1020) wgusers   (9000)     3679 2012-04-27 21:48:00.000000 rosdep-0.9.6/test/test_rosdep_model.py
+-rw-r--r--   0 tfoote    (1020) wgusers   (9000)    19136 2012-04-27 21:50:32.000000 rosdep-0.9.6/test/test_rosdep_lookup.py
+-rw-r--r--   0 tfoote    (1020) wgusers   (9000)    18229 2012-04-27 21:48:00.000000 rosdep-0.9.6/test/test_rosdep_sources_list.py
+-rw-r--r--   0 tfoote    (1020) wgusers   (9000)     2986 2012-04-27 21:48:00.000000 rosdep-0.9.6/test/test_rosdep_redhat.py
+-rw-r--r--   0 tfoote    (1020) wgusers   (9000)     7778 2012-04-27 21:50:32.000000 rosdep-0.9.6/test/test_rosdep_dependency_graph.py
+-rw-r--r--   0 tfoote    (1020) wgusers   (9000)     2463 2012-04-27 21:48:00.000000 rosdep-0.9.6/test/test_rosdep_loader.py
+-rw-r--r--   0 tfoote    (1020) wgusers   (9000)     3480 2012-04-27 21:48:00.000000 rosdep-0.9.6/test/test_rosdep_debian.py
+-rw-r--r--   0 tfoote    (1020) wgusers   (9000)    22386 2012-04-27 21:50:32.000000 rosdep-0.9.6/test/test_rosdep_installers.py
+-rw-r--r--   0 tfoote    (1020) wgusers   (9000)     2088 2012-04-27 21:48:00.000000 rosdep-0.9.6/test/test_rosdep_shell_utils.py
+-rw-r--r--   0 tfoote    (1020) wgusers   (9000)      535 2012-08-09 20:31:38.000000 rosdep-0.9.6/PKG-INFO
+-rw-r--r--   0 tfoote    (1020) wgusers   (9000)       59 2012-08-09 20:31:38.000000 rosdep-0.9.6/setup.cfg
+drwxr-xr-x   0 tfoote    (1020) wgusers   (9000)        0 2012-08-09 20:31:38.000000 rosdep-0.9.6/scripts/
+-rwxr-xr-x   0 tfoote    (1020) wgusers   (9000)       74 2012-04-27 21:48:00.000000 rosdep-0.9.6/scripts/rosdep
+-rwxr-xr-x   0 tfoote    (1020) wgusers   (9000)     2563 2012-04-27 21:48:00.000000 rosdep-0.9.6/scripts/rosdep-source
+-rwxr-xr-x   0 tfoote    (1020) wgusers   (9000)      946 2012-04-27 21:48:00.000000 rosdep-0.9.6/scripts/rosdep-gbp-brew
```

### Comparing `rosdep-0.9.4/setup.py` & `rosdep-0.9.6/setup.py`

 * *Files identical despite different names*

### Comparing `rosdep-0.9.4/src/rosdep2/installers.py` & `rosdep-0.9.6/src/rosdep2/installers.py`

 * *Files identical despite different names*

### Comparing `rosdep-0.9.4/src/rosdep2/dependency_graph.py` & `rosdep-0.9.6/src/rosdep2/dependency_graph.py`

 * *Files identical despite different names*

### Comparing `rosdep-0.9.4/src/rosdep2/rospkg_loader.py` & `rosdep-0.9.6/src/rosdep2/rospkg_loader.py`

 * *Files identical despite different names*

### Comparing `rosdep-0.9.4/src/rosdep2/model.py` & `rosdep-0.9.6/src/rosdep2/model.py`

 * *Files identical despite different names*

### Comparing `rosdep-0.9.4/src/rosdep2/core.py` & `rosdep-0.9.6/src/rosdep2/core.py`

 * *Files identical despite different names*

### Comparing `rosdep-0.9.4/src/rosdep2/shell_utils.py` & `rosdep-0.9.6/src/rosdep2/shell_utils.py`

 * *Files identical despite different names*

### Comparing `rosdep-0.9.4/src/rosdep2/rep3.py` & `rosdep-0.9.6/src/rosdep2/rep3.py`

 * *Files identical despite different names*

### Comparing `rosdep-0.9.4/src/rosdep2/main.py` & `rosdep-0.9.6/src/rosdep2/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -203,16 +203,16 @@
                       action="store_true", help="Tell the package manager to default to y or fail when installing")
     parser.add_option("--simulate", "-s", dest="simulate", default=False, 
                       action="store_true", help="Simulate install")
     parser.add_option("-r", dest="robust", default=False, 
                       action="store_true", help="Continue installing despite errors.")
     parser.add_option("-a", "--all", dest="rosdep_all", default=False, 
                       action="store_true", help="select all packages")
-    parser.add_option("-R", dest="recursive", default=False, 
-                      action="store_true", help="Install implicit/recursive dependencies.  Only valid with 'install' command.")
+    parser.add_option("-n", dest="recursive", default=True, 
+                      action="store_false", help="Do not consider implicit/recursive dependencies.  Only valid with 'keys', 'check', and 'install' commands.")
 
     options, args = parser.parse_args(args)
     if options.print_version:
         print(__version__)
         sys.exit(0)
 
     if len(args) == 0:
@@ -352,27 +352,27 @@
     except IOError as e:
         print("ERROR: error loading sources list:\n\t%s"%(e), file=sys.stderr)
     
 def command_keys(lookup, packages, options):
     lookup = _get_default_RosdepLookup(options)
     rosdep_keys = []
     for package_name in packages:
-        rosdep_keys.extend(lookup.get_rosdeps(package_name, implicit=True))
+        rosdep_keys.extend(lookup.get_rosdeps(package_name, implicit=options.recursive))
 
     _print_lookup_errors(lookup)
     print('\n'.join(set(rosdep_keys)))
 
 def command_check(lookup, packages, options):
     verbose = options.verbose
     
     installer_context = create_default_installer_context(verbose=verbose)
     configure_installer_context_os(installer_context, options)
     installer = RosdepInstaller(installer_context, lookup)
 
-    uninstalled, errors = installer.get_uninstalled(packages, verbose=verbose)
+    uninstalled, errors = installer.get_uninstalled(packages, implicit=options.recursive, verbose=verbose)
 
     # pretty print the result
     if [v for k, v in uninstalled if v]:
         print("System dependencies have not been satisified:")
         for installer_key, resolved in uninstalled:
             if resolved:
                 for r in resolved:
```

### Comparing `rosdep-0.9.4/src/rosdep2/lookup.py` & `rosdep-0.9.6/src/rosdep2/lookup.py`

 * *Files identical despite different names*

### Comparing `rosdep-0.9.4/src/rosdep2/platforms/osx.py` & `rosdep-0.9.6/src/rosdep2/platforms/osx.py`

 * *Files identical despite different names*

### Comparing `rosdep-0.9.4/src/rosdep2/platforms/gentoo.py` & `rosdep-0.9.6/src/rosdep2/platforms/gentoo.py`

 * *Files identical despite different names*

### Comparing `rosdep-0.9.4/src/rosdep2/platforms/arch.py` & `rosdep-0.9.6/src/rosdep2/platforms/arch.py`

 * *Files identical despite different names*

### Comparing `rosdep-0.9.4/src/rosdep2/platforms/cygwin.py` & `rosdep-0.9.6/src/rosdep2/platforms/cygwin.py`

 * *Files identical despite different names*

### Comparing `rosdep-0.9.4/src/rosdep2/platforms/redhat.py` & `rosdep-0.9.6/src/rosdep2/platforms/redhat.py`

 * *Files identical despite different names*

### Comparing `rosdep-0.9.4/src/rosdep2/platforms/brewmaker.py` & `rosdep-0.9.6/src/rosdep2/platforms/brewmaker.py`

 * *Files identical despite different names*

### Comparing `rosdep-0.9.4/src/rosdep2/platforms/debian.py` & `rosdep-0.9.6/src/rosdep2/platforms/debian.py`

 * *Files identical despite different names*

### Comparing `rosdep-0.9.4/src/rosdep2/platforms/opensuse.py` & `rosdep-0.9.6/src/rosdep2/platforms/opensuse.py`

 * *Files identical despite different names*

### Comparing `rosdep-0.9.4/src/rosdep2/platforms/pip.py` & `rosdep-0.9.6/src/rosdep2/platforms/pip.py`

 * *Files identical despite different names*

### Comparing `rosdep-0.9.4/src/rosdep2/platforms/freebsd.py` & `rosdep-0.9.6/src/rosdep2/platforms/freebsd.py`

 * *Files identical despite different names*

### Comparing `rosdep-0.9.4/src/rosdep2/platforms/source.py` & `rosdep-0.9.6/src/rosdep2/platforms/source.py`

 * *Files identical despite different names*

### Comparing `rosdep-0.9.4/src/rosdep2/gbpdistro_support.py` & `rosdep-0.9.6/src/rosdep2/gbpdistro_support.py`

 * *Files identical despite different names*

### Comparing `rosdep-0.9.4/src/rosdep2/catkin_support.py` & `rosdep-0.9.6/src/rosdep2/catkin_support.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,30 +5,31 @@
 and thus return end-user oriented error messages.
 
 Errors are returned as arguments to raised :exc:`ValidationFailed`
 exceptions.
 
 Workflow::
 
-    installer = get_apt_installer()
+    installer = get_installer(APT_INSTALLER)
     view = get_catkin_view(rosdistro_name, 'ubuntu', 'lucid')
-    resolve_for_apt(rosdep_key, view, installer, 'ubuntu', 'lucid')
+    resolve_for_os(rosdep_key, view, installer, 'ubuntu', 'lucid')
 
 """
 
 from __future__ import print_function
 
 import os
 
 from subprocess import Popen, PIPE, CalledProcessError
 
 from . import create_default_installer_context
 from .platforms.debian import APT_INSTALLER
 from .platforms.osx import BREW_INSTALLER
 from .platforms.pip import PIP_INSTALLER
+from .platforms.redhat import YUM_INSTALLER
 from .rep3 import download_targets_data
 from .sources_list import get_sources_list_dir, DataSourceMatcher, SourcesListLoader
 from .lookup import RosdepLookup
 from .rospkg_loader import DEFAULT_VIEW_KEY
 
 class ValidationFailed(Exception):
     pass
@@ -53,50 +54,41 @@
     distribution.  This method blocks on an HTTP download.
 
     :raises: :exc:`ValidationFailed`
     """
     targets_data = download_targets_data()
     return targets_data[rosdistro]
 
-def get_apt_installer():
-    installer_context = create_default_installer_context()
-    return installer_context.get_installer(APT_INSTALLER)
+def get_installer(installer_name):
+    """ Expected installers APT_INSTALLER, YUM_INSTALLER, ..."""
 
-def get_brew_installer():
     installer_context = create_default_installer_context()
-    return installer_context.get_installer(BREW_INSTALLER)
+    return installer_context.get_installer(installer_name)
+
+default_installers = {
+    'debian': [APT_INSTALLER],
+    'osx': [BREW_INSTALLER, PIP_INSTALLER],
+    'ubuntu': [APT_INSTALLER],
+    'fedora': [YUM_INSTALLER],
+    }
+
 
-def resolve_for_apt(rosdep_key, view, installer, os_name, os_version):
+def resolve_for_os(rosdep_key, view, installer, os_name, os_version):
     """
-    Resolve rosdep key to apt dependencies.
+    Resolve rosdep key to dependencies.
     
     :param os_name: OS name, e.g. 'ubuntu'
 
     :raises: :exc:`rosdep2.ResolutionError`
     """
     d = view.lookup(rosdep_key)
-    inst_key, rule = d.get_rule_for_platform(os_name, os_version, [APT_INSTALLER], APT_INSTALLER)    
+    inst_key, rule = d.get_rule_for_platform(os_name, os_version, default_installers[os_name], APT_INSTALLER)
     assert inst_key == APT_INSTALLER
     return installer.resolve(rule)
 
-def resolve_for_osx(rosdep_key, view, os_name, os_version):
-    """
-    Resolve rosdep key to brew and pip dependencies.
-    
-    :param rosdep_key: rosdep key that needs to be resolved
-    :param view: RosdepView that is used to lookup the rosdep_key
-    :param os_name: OS name, e.g. 'osx'
-    :param os_version: OS version, e.g. 'lion'
-
-    :raises: :exc:`rosdep2.ResolutionError`
-    """
-    d = view.lookup(rosdep_key)
-    inst_key, rule = d.get_rule_for_platform(os_name, os_version, [BREW_INSTALLER, PIP_INSTALLER], BREW_INSTALLER)    
-    return inst_key, rule
-
 def get_catkin_view(rosdistro_name, os_name, os_version):
     """
     :raises: :exc:`ValidationFailed`
     """
     sources_list_dir = get_sources_list_dir()
     if not os.path.exists(sources_list_dir):
         raise ValidationFailed("""rosdep database is not initialized, please run:
```

### Comparing `rosdep-0.9.4/src/rosdep2/loader.py` & `rosdep-0.9.6/src/rosdep2/loader.py`

 * *Files identical despite different names*

### Comparing `rosdep-0.9.4/src/rosdep2/__init__.py` & `rosdep-0.9.6/src/rosdep2/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 
 """
 rosdep library and command-line tool
 """
 
 from __future__ import print_function
 
-__version__ = '0.9.4'
+__version__ = '0.9.6'
 
 import sys
 
 try:
     from .installers import InstallerContext, Installer, \
             PackageManagerInstaller
     from .core import RosdepInternalError, InstallFailed, UnsupportedOs, \
```

### Comparing `rosdep-0.9.4/src/rosdep2/sources_list.py` & `rosdep-0.9.6/src/rosdep2/sources_list.py`

 * *Files identical despite different names*

### Comparing `rosdep-0.9.4/src/rosdep.egg-info/SOURCES.txt` & `rosdep-0.9.6/src/rosdep.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rosdep-0.9.4/src/rosdep.egg-info/PKG-INFO` & `rosdep-0.9.6/src/rosdep.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: rosdep
-Version: 0.9.4
+Version: 0.9.6
 Summary: rosdep system dependency installation tool
 Home-page: http://www.ros.org/wiki/rosdep
 Author: Tully Foote, Ken Conley
 Author-email: foote@willowgarage.com, kwc@willowgarage.com
 License: BSD
 Download-URL: http://pr.willowgarage.com/downloads/rosdep/
 Description: Command-line tool for installing system dependencies on a variety of platforms.
```

### Comparing `rosdep-0.9.4/test/test_rosdep_cygwin.py` & `rosdep-0.9.6/test/test_rosdep_cygwin.py`

 * *Files identical despite different names*

### Comparing `rosdep-0.9.4/test/test_rosdep_main.py` & `rosdep-0.9.6/test/test_rosdep_main.py`

 * *Files identical despite different names*

### Comparing `rosdep-0.9.4/test/test_rosdep_rep3.py` & `rosdep-0.9.6/test/test_rosdep_rep3.py`

 * *Files identical despite different names*

### Comparing `rosdep-0.9.4/test/test_rosdep_pip.py` & `rosdep-0.9.6/test/test_rosdep_pip.py`

 * *Files identical despite different names*

### Comparing `rosdep-0.9.4/test/test_rosdep_gentoo.py` & `rosdep-0.9.6/test/test_rosdep_gentoo.py`

 * *Files identical despite different names*

### Comparing `rosdep-0.9.4/test/test_rosdep_gbpdistro_support.py` & `rosdep-0.9.6/test/test_rosdep_gbpdistro_support.py`

 * *Files identical despite different names*

### Comparing `rosdep-0.9.4/test/test_rosdep_opensuse.py` & `rosdep-0.9.6/test/test_rosdep_opensuse.py`

 * *Files identical despite different names*

### Comparing `rosdep-0.9.4/test/test_rosdep.py` & `rosdep-0.9.6/test/test_rosdep.py`

 * *Files identical despite different names*

### Comparing `rosdep-0.9.4/test/test_rosdep_osx.py` & `rosdep-0.9.6/test/test_rosdep_osx.py`

 * *Files identical despite different names*

### Comparing `rosdep-0.9.4/test/test_rosdep_core.py` & `rosdep-0.9.6/test/test_rosdep_core.py`

 * *Files identical despite different names*

### Comparing `rosdep-0.9.4/test/test_rosdep_rospkg_loader.py` & `rosdep-0.9.6/test/test_rosdep_rospkg_loader.py`

 * *Files identical despite different names*

### Comparing `rosdep-0.9.4/test/test_rosdep_source.py` & `rosdep-0.9.6/test/test_rosdep_source.py`

 * *Files identical despite different names*

### Comparing `rosdep-0.9.4/test/test_rosdep_catkin_support.py` & `rosdep-0.9.6/test/test_rosdep_catkin_support.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,16 @@
-from rosdep2.catkin_support import get_apt_installer, get_catkin_view, resolve_for_apt, ValidationFailed
+from rosdep2.catkin_support import get_installer, get_catkin_view, ValidationFailed, resolve_for_os
+
+from rosdep2.platforms.debian import APT_INSTALLER
+
 
 def test_workflow():
     try:
-        installer = get_apt_installer()
+        installer = get_installer(APT_INSTALLER)
         view = get_catkin_view('fuerte', 'ubuntu', 'lucid')
-        resolved = resolve_for_apt('cmake', view, installer, 'ubuntu', 'lucid')
+        resolved = resolve_for_os('cmake', view, installer, 'ubuntu', 'lucid')
         assert ['cmake'] == resolved
-        resolved = resolve_for_apt('python', view, installer, 'ubuntu', 'lucid')
+        resolved = resolve_for_os('python', view, installer, 'ubuntu', 'lucid')
         assert resolved == ['python-dev']
     except ValidationFailed:
         # tests fail on the server because 'rosdep init' has not been run
         pass
```

### Comparing `rosdep-0.9.4/test/test_rosdep_arch.py` & `rosdep-0.9.6/test/test_rosdep_arch.py`

 * *Files identical despite different names*

### Comparing `rosdep-0.9.4/test/test_rosdep_model.py` & `rosdep-0.9.6/test/test_rosdep_model.py`

 * *Files identical despite different names*

### Comparing `rosdep-0.9.4/test/test_rosdep_lookup.py` & `rosdep-0.9.6/test/test_rosdep_lookup.py`

 * *Files identical despite different names*

### Comparing `rosdep-0.9.4/test/test_rosdep_sources_list.py` & `rosdep-0.9.6/test/test_rosdep_sources_list.py`

 * *Files identical despite different names*

### Comparing `rosdep-0.9.4/test/test_rosdep_redhat.py` & `rosdep-0.9.6/test/test_rosdep_redhat.py`

 * *Files identical despite different names*

### Comparing `rosdep-0.9.4/test/test_rosdep_dependency_graph.py` & `rosdep-0.9.6/test/test_rosdep_dependency_graph.py`

 * *Files identical despite different names*

### Comparing `rosdep-0.9.4/test/test_rosdep_loader.py` & `rosdep-0.9.6/test/test_rosdep_loader.py`

 * *Files identical despite different names*

### Comparing `rosdep-0.9.4/test/test_rosdep_debian.py` & `rosdep-0.9.6/test/test_rosdep_debian.py`

 * *Files identical despite different names*

### Comparing `rosdep-0.9.4/test/test_rosdep_installers.py` & `rosdep-0.9.6/test/test_rosdep_installers.py`

 * *Files identical despite different names*

### Comparing `rosdep-0.9.4/test/test_rosdep_shell_utils.py` & `rosdep-0.9.6/test/test_rosdep_shell_utils.py`

 * *Files identical despite different names*

### Comparing `rosdep-0.9.4/PKG-INFO` & `rosdep-0.9.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: rosdep
-Version: 0.9.4
+Version: 0.9.6
 Summary: rosdep system dependency installation tool
 Home-page: http://www.ros.org/wiki/rosdep
 Author: Tully Foote, Ken Conley
 Author-email: foote@willowgarage.com, kwc@willowgarage.com
 License: BSD
 Download-URL: http://pr.willowgarage.com/downloads/rosdep/
 Description: Command-line tool for installing system dependencies on a variety of platforms.
```

### Comparing `rosdep-0.9.4/scripts/rosdep-source` & `rosdep-0.9.6/scripts/rosdep-source`

 * *Files identical despite different names*

### Comparing `rosdep-0.9.4/scripts/rosdep-gbp-brew` & `rosdep-0.9.6/scripts/rosdep-gbp-brew`

 * *Files identical despite different names*

