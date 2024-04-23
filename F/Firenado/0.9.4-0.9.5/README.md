# Comparing `tmp/Firenado-0.9.4.tar.gz` & `tmp/firenado-0.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Firenado-0.9.4.tar", last modified: Sat Feb 24 01:32:12 2024, max compression
+gzip compressed data, was "firenado-0.9.5.tar", last modified: Tue Apr 23 19:09:00 2024, max compression
```

## Comparing `Firenado-0.9.4.tar` & `firenado-0.9.5.tar`

### file list

```diff
@@ -1,108 +1,108 @@
-drwxr-xr-x   0 fpiraz    (1000) fpiraz    (1000)        0 2024-02-24 01:32:12.548275 Firenado-0.9.4/
-drwxr-xr-x   0 fpiraz    (1000) fpiraz    (1000)        0 2024-02-24 01:32:12.545275 Firenado-0.9.4/Firenado.egg-info/
--rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)     5799 2024-02-24 01:32:12.000000 Firenado-0.9.4/Firenado.egg-info/PKG-INFO
--rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)     2549 2024-02-24 01:32:12.000000 Firenado-0.9.4/Firenado.egg-info/SOURCES.txt
--rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)        1 2024-02-24 01:32:12.000000 Firenado-0.9.4/Firenado.egg-info/dependency_links.txt
--rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)       71 2024-02-24 01:32:12.000000 Firenado-0.9.4/Firenado.egg-info/entry_points.txt
--rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)      250 2024-02-24 01:32:12.000000 Firenado-0.9.4/Firenado.egg-info/requires.txt
--rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)       15 2024-02-24 01:32:12.000000 Firenado-0.9.4/Firenado.egg-info/top_level.txt
--rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)    11361 2022-01-22 03:40:14.000000 Firenado-0.9.4/LICENSE
--rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)      593 2021-03-14 16:46:20.000000 Firenado-0.9.4/MANIFEST.in
--rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)     5799 2024-02-24 01:32:12.548275 Firenado-0.9.4/PKG-INFO
--rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)     3789 2022-04-15 16:36:51.000000 Firenado-0.9.4/README.md
--rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)     3118 2019-01-26 05:48:04.000000 Firenado-0.9.4/README.rst
-drwxr-xr-x   0 fpiraz    (1000) fpiraz    (1000)        0 2024-02-24 01:32:12.530275 Firenado-0.9.4/firenado/
--rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)     1049 2024-02-24 01:27:11.000000 Firenado-0.9.4/firenado/__init__.py
-drwxr-xr-x   0 fpiraz    (1000) fpiraz    (1000)        0 2024-02-24 01:32:12.531275 Firenado-0.9.4/firenado/bin/
--rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)        0 2023-06-10 05:12:04.000000 Firenado-0.9.4/firenado/bin/__init__.py
--rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)      716 2023-06-10 05:14:23.000000 Firenado-0.9.4/firenado/bin/firenado-cli.py
--rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)      727 2023-06-16 03:06:08.000000 Firenado-0.9.4/firenado/bin/firenado-cli1.py
-drwxr-xr-x   0 fpiraz    (1000) fpiraz    (1000)        0 2024-02-24 01:32:12.531275 Firenado-0.9.4/firenado/cli/
--rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)       31 2023-06-16 03:06:08.000000 Firenado-0.9.4/firenado/cli/__init__.py
--rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)      915 2023-08-04 15:30:18.000000 Firenado-0.9.4/firenado/cli/commands.py
--rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)      206 2023-08-04 15:43:18.000000 Firenado-0.9.4/firenado/cli/root.py
-drwxr-xr-x   0 fpiraz    (1000) fpiraz    (1000)        0 2024-02-24 01:32:12.532275 Firenado-0.9.4/firenado/components/
--rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)      759 2019-01-19 15:51:14.000000 Firenado-0.9.4/firenado/components/__init__.py
-drwxr-xr-x   0 fpiraz    (1000) fpiraz    (1000)        0 2024-02-24 01:32:12.532275 Firenado-0.9.4/firenado/components/firenado/
--rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)        0 2016-09-08 01:38:40.000000 Firenado-0.9.4/firenado/components/firenado/__init__.py
--rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)      872 2016-09-08 01:38:40.000000 Firenado-0.9.4/firenado/components/firenado/component.py
--rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)     1063 2016-09-08 01:38:40.000000 Firenado-0.9.4/firenado/components/firenado/handlers.py
-drwxr-xr-x   0 fpiraz    (1000) fpiraz    (1000)        0 2024-02-24 01:32:12.532275 Firenado-0.9.4/firenado/components/firenado/templates/
--rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)     4008 2016-08-29 15:57:57.000000 Firenado-0.9.4/firenado/components/firenado/templates/info.html
-drwxr-xr-x   0 fpiraz    (1000) fpiraz    (1000)        0 2024-02-24 01:32:12.533275 Firenado-0.9.4/firenado/components/static_maps/
--rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)        0 2016-09-08 01:38:40.000000 Firenado-0.9.4/firenado/components/static_maps/__init__.py
--rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)     4137 2018-08-25 00:58:30.000000 Firenado-0.9.4/firenado/components/static_maps/component.py
-drwxr-xr-x   0 fpiraz    (1000) fpiraz    (1000)        0 2024-02-24 01:32:12.534275 Firenado-0.9.4/firenado/components/toolbox/
--rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)        0 2016-11-26 15:05:30.000000 Firenado-0.9.4/firenado/components/toolbox/__init__.py
--rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)      831 2016-11-26 15:05:30.000000 Firenado-0.9.4/firenado/components/toolbox/component.py
--rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)     1937 2023-06-10 05:29:53.000000 Firenado-0.9.4/firenado/components/toolbox/uimodules.py
-drwxr-xr-x   0 fpiraz    (1000) fpiraz    (1000)        0 2024-02-24 01:32:12.534275 Firenado-0.9.4/firenado/conf/
--rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)     4719 2023-08-04 15:13:51.000000 Firenado-0.9.4/firenado/conf/__init__.py
--rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)     1140 2023-08-04 15:24:44.000000 Firenado-0.9.4/firenado/conf/firenado.yml
--rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)    18308 2023-08-04 15:34:05.000000 Firenado-0.9.4/firenado/config.py
--rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)    15446 2023-11-25 18:14:13.000000 Firenado-0.9.4/firenado/data.py
--rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)    12677 2024-02-19 05:23:58.000000 Firenado-0.9.4/firenado/launcher.py
-drwxr-xr-x   0 fpiraz    (1000) fpiraz    (1000)        0 2024-02-24 01:32:12.535275 Firenado-0.9.4/firenado/management/
--rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)      738 2019-05-18 04:12:04.000000 Firenado-0.9.4/firenado/management/__init__.py
--rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)     1993 2020-02-29 17:12:35.000000 Firenado-0.9.4/firenado/management/commands.py
--rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)     8615 2023-06-10 05:24:28.000000 Firenado-0.9.4/firenado/management/management.py
--rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)     6784 2023-06-10 05:27:13.000000 Firenado-0.9.4/firenado/management/tasks.py
-drwxr-xr-x   0 fpiraz    (1000) fpiraz    (1000)        0 2024-02-24 01:32:12.523275 Firenado-0.9.4/firenado/management/templates/
-drwxr-xr-x   0 fpiraz    (1000) fpiraz    (1000)        0 2024-02-24 01:32:12.537275 Firenado-0.9.4/firenado/management/templates/help/
--rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)      160 2016-09-08 01:38:40.000000 Firenado-0.9.4/firenado/management/templates/help/app_command_help.txt
--rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)      119 2018-11-03 23:08:57.000000 Firenado-0.9.4/firenado/management/templates/help/header.txt
--rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)       46 2016-09-08 01:38:40.000000 Firenado-0.9.4/firenado/management/templates/help/init_command_help.txt
--rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)      252 2018-11-03 23:09:50.000000 Firenado-0.9.4/firenado/management/templates/help/main_command_help.txt
--rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)      117 2017-06-19 04:13:32.000000 Firenado-0.9.4/firenado/management/templates/help/project_command_help.txt
--rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)      241 2020-02-29 17:12:35.000000 Firenado-0.9.4/firenado/management/templates/help/random_command_help.txt
-drwxr-xr-x   0 fpiraz    (1000) fpiraz    (1000)        0 2024-02-24 01:32:12.539275 Firenado-0.9.4/firenado/management/templates/project/
--rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)      224 2018-11-21 07:38:12.000000 Firenado-0.9.4/firenado/management/templates/project/app.py.txt
--rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)      691 2016-09-10 17:22:04.000000 Firenado-0.9.4/firenado/management/templates/project/firenado.yml.txt
--rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)      212 2018-11-21 07:38:12.000000 Firenado-0.9.4/firenado/management/templates/project/handlers.py.txt
--rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)       54 2016-09-08 01:38:40.000000 Firenado-0.9.4/firenado/management/templates/project/init_command_help.txt
--rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)    15329 2024-02-16 22:26:37.000000 Firenado-0.9.4/firenado/schedule.py
--rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)    10092 2024-02-19 07:20:27.000000 Firenado-0.9.4/firenado/security.py
--rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)     4894 2023-06-10 05:21:44.000000 Firenado-0.9.4/firenado/service.py
--rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)    22705 2023-11-25 18:14:44.000000 Firenado-0.9.4/firenado/session.py
--rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)     6148 2023-11-25 18:15:01.000000 Firenado-0.9.4/firenado/sqlalchemy.py
--rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)     2566 2024-02-21 23:21:12.000000 Firenado-0.9.4/firenado/testing.py
--rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)    21703 2023-06-10 05:22:53.000000 Firenado-0.9.4/firenado/tornadoweb.py
--rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)      847 2023-06-10 05:23:10.000000 Firenado-0.9.4/firenado/uimodules.py
-drwxr-xr-x   0 fpiraz    (1000) fpiraz    (1000)        0 2024-02-24 01:32:12.540275 Firenado-0.9.4/firenado/util/
--rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)        1 2023-11-25 18:15:35.000000 Firenado-0.9.4/firenado/util/__init__.py
--rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)     1084 2023-06-10 05:28:19.000000 Firenado-0.9.4/firenado/util/argparse_util.py
--rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)      901 2023-06-10 05:28:55.000000 Firenado-0.9.4/firenado/util/sqlalchemy_util.py
--rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)      896 2023-06-10 05:28:37.000000 Firenado-0.9.4/firenado/util/url_util.py
-drwxr-xr-x   0 fpiraz    (1000) fpiraz    (1000)        0 2024-02-24 01:32:12.541275 Firenado-0.9.4/requirements/
--rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)       62 2020-07-28 14:20:19.000000 Firenado-0.9.4/requirements/all.txt
--rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)       41 2024-02-06 18:49:19.000000 Firenado-0.9.4/requirements/basic.txt
--rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)       15 2024-02-06 18:52:02.000000 Firenado-0.9.4/requirements/pexpect.txt
--rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)       28 2024-02-06 18:52:07.000000 Firenado-0.9.4/requirements/redis.txt
--rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)       16 2023-11-22 03:01:02.000000 Firenado-0.9.4/requirements/schedule.txt
--rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)       19 2023-11-22 03:02:15.000000 Firenado-0.9.4/requirements/sqlalchemy.txt
--rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)      103 2024-02-24 01:32:12.548275 Firenado-0.9.4/setup.cfg
--rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)     3754 2023-11-08 00:28:58.000000 Firenado-0.9.4/setup.py
-drwxr-xr-x   0 fpiraz    (1000) fpiraz    (1000)        0 2024-02-24 01:32:12.543275 Firenado-0.9.4/tests/
--rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)     2180 2024-02-06 21:27:09.000000 Firenado-0.9.4/tests/__init__.py
--rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)     2010 2022-12-18 22:09:16.000000 Firenado-0.9.4/tests/components_test.py
--rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)     9962 2023-06-10 05:31:08.000000 Firenado-0.9.4/tests/conf_test.py
--rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)     1903 2023-06-10 05:31:25.000000 Firenado-0.9.4/tests/config_test.py
--rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)     5212 2023-06-10 05:31:35.000000 Firenado-0.9.4/tests/data_test.py
-drwxr-xr-x   0 fpiraz    (1000) fpiraz    (1000)        0 2024-02-24 01:32:12.544275 Firenado-0.9.4/tests/features/
--rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)        0 2019-05-18 04:12:19.000000 Firenado-0.9.4/tests/features/__init__.py
--rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)     1021 2024-02-21 23:51:47.000000 Firenado-0.9.4/tests/features/environment.py
-drwxr-xr-x   0 fpiraz    (1000) fpiraz    (1000)        0 2024-02-24 01:32:12.544275 Firenado-0.9.4/tests/features/steps/
--rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)        0 2020-03-17 14:16:49.000000 Firenado-0.9.4/tests/features/steps/__init__.py
--rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)     1037 2023-06-16 03:06:08.000000 Firenado-0.9.4/tests/features/steps/cli.py
--rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)     2212 2024-02-23 16:19:30.000000 Firenado-0.9.4/tests/features/steps/launcher.py
--rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)     2202 2024-02-23 16:32:18.000000 Firenado-0.9.4/tests/loader_test.py
--rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)     1964 2024-02-23 16:22:57.000000 Firenado-0.9.4/tests/runtests.py
--rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)     3025 2024-02-21 22:32:52.000000 Firenado-0.9.4/tests/security_test.py
--rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)     8024 2023-06-10 05:32:16.000000 Firenado-0.9.4/tests/service_test.py
--rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)     5170 2023-06-10 05:32:35.000000 Firenado-0.9.4/tests/session_test.py
--rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)     8862 2023-06-10 05:32:47.000000 Firenado-0.9.4/tests/sqlalchemy_test.py
--rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)     2308 2024-02-21 23:19:06.000000 Firenado-0.9.4/tests/testing_test.py
--rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)     6025 2023-06-10 05:32:56.000000 Firenado-0.9.4/tests/tornadoweb_test.py
-drwxr-xr-x   0 fpiraz    (1000) fpiraz    (1000)        0 2024-02-24 01:32:12.545275 Firenado-0.9.4/tests/util/
--rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)        0 2018-07-08 04:28:25.000000 Firenado-0.9.4/tests/util/__init__.py
--rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)     1895 2021-03-23 17:10:31.000000 Firenado-0.9.4/tests/util/url_util_test.py
+drwxr-xr-x   0 fpiraz    (1000) fpiraz    (1000)        0 2024-04-23 19:09:00.006140 firenado-0.9.5/
+drwxr-xr-x   0 fpiraz    (1000) fpiraz    (1000)        0 2024-04-23 19:09:00.004140 firenado-0.9.5/Firenado.egg-info/
+-rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)     5799 2024-04-23 19:08:59.000000 firenado-0.9.5/Firenado.egg-info/PKG-INFO
+-rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)     2549 2024-04-23 19:08:59.000000 firenado-0.9.5/Firenado.egg-info/SOURCES.txt
+-rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)        1 2024-04-23 19:08:59.000000 firenado-0.9.5/Firenado.egg-info/dependency_links.txt
+-rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)       71 2024-04-23 19:08:59.000000 firenado-0.9.5/Firenado.egg-info/entry_points.txt
+-rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)      250 2024-04-23 19:08:59.000000 firenado-0.9.5/Firenado.egg-info/requires.txt
+-rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)       15 2024-04-23 19:08:59.000000 firenado-0.9.5/Firenado.egg-info/top_level.txt
+-rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)    11349 2024-04-23 18:51:59.000000 firenado-0.9.5/LICENSE
+-rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)      593 2021-03-14 16:46:20.000000 firenado-0.9.5/MANIFEST.in
+-rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)     5799 2024-04-23 19:09:00.006140 firenado-0.9.5/PKG-INFO
+-rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)     3789 2022-04-15 16:36:51.000000 firenado-0.9.5/README.md
+-rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)     3118 2019-01-26 05:48:04.000000 firenado-0.9.5/README.rst
+drwxr-xr-x   0 fpiraz    (1000) fpiraz    (1000)        0 2024-04-23 19:08:59.992140 firenado-0.9.5/firenado/
+-rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)     1049 2024-04-23 18:52:34.000000 firenado-0.9.5/firenado/__init__.py
+drwxr-xr-x   0 fpiraz    (1000) fpiraz    (1000)        0 2024-04-23 19:08:59.993140 firenado-0.9.5/firenado/bin/
+-rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)        0 2023-06-10 05:12:04.000000 firenado-0.9.5/firenado/bin/__init__.py
+-rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)      716 2023-06-10 05:14:23.000000 firenado-0.9.5/firenado/bin/firenado-cli.py
+-rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)      727 2023-06-16 03:06:08.000000 firenado-0.9.5/firenado/bin/firenado-cli1.py
+drwxr-xr-x   0 fpiraz    (1000) fpiraz    (1000)        0 2024-04-23 19:08:59.994140 firenado-0.9.5/firenado/cli/
+-rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)       31 2023-06-16 03:06:08.000000 firenado-0.9.5/firenado/cli/__init__.py
+-rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)      915 2024-03-16 20:41:52.000000 firenado-0.9.5/firenado/cli/commands.py
+-rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)      298 2024-02-29 19:12:13.000000 firenado-0.9.5/firenado/cli/root.py
+drwxr-xr-x   0 fpiraz    (1000) fpiraz    (1000)        0 2024-04-23 19:08:59.994140 firenado-0.9.5/firenado/components/
+-rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)      759 2019-01-19 15:51:14.000000 firenado-0.9.5/firenado/components/__init__.py
+drwxr-xr-x   0 fpiraz    (1000) fpiraz    (1000)        0 2024-04-23 19:08:59.994140 firenado-0.9.5/firenado/components/firenado/
+-rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)        0 2016-09-08 01:38:40.000000 firenado-0.9.5/firenado/components/firenado/__init__.py
+-rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)      872 2016-09-08 01:38:40.000000 firenado-0.9.5/firenado/components/firenado/component.py
+-rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)     1063 2016-09-08 01:38:40.000000 firenado-0.9.5/firenado/components/firenado/handlers.py
+drwxr-xr-x   0 fpiraz    (1000) fpiraz    (1000)        0 2024-04-23 19:08:59.995140 firenado-0.9.5/firenado/components/firenado/templates/
+-rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)     4008 2016-08-29 15:57:57.000000 firenado-0.9.5/firenado/components/firenado/templates/info.html
+drwxr-xr-x   0 fpiraz    (1000) fpiraz    (1000)        0 2024-04-23 19:08:59.995140 firenado-0.9.5/firenado/components/static_maps/
+-rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)        0 2016-09-08 01:38:40.000000 firenado-0.9.5/firenado/components/static_maps/__init__.py
+-rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)     4137 2018-08-25 00:58:30.000000 firenado-0.9.5/firenado/components/static_maps/component.py
+drwxr-xr-x   0 fpiraz    (1000) fpiraz    (1000)        0 2024-04-23 19:08:59.995140 firenado-0.9.5/firenado/components/toolbox/
+-rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)        0 2016-11-26 15:05:30.000000 firenado-0.9.5/firenado/components/toolbox/__init__.py
+-rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)      831 2016-11-26 15:05:30.000000 firenado-0.9.5/firenado/components/toolbox/component.py
+-rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)     1937 2023-06-10 05:29:53.000000 firenado-0.9.5/firenado/components/toolbox/uimodules.py
+drwxr-xr-x   0 fpiraz    (1000) fpiraz    (1000)        0 2024-04-23 19:08:59.996140 firenado-0.9.5/firenado/conf/
+-rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)     4719 2023-08-04 15:13:51.000000 firenado-0.9.5/firenado/conf/__init__.py
+-rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)     1140 2023-08-04 15:24:44.000000 firenado-0.9.5/firenado/conf/firenado.yml
+-rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)    17137 2024-04-22 22:21:07.000000 firenado-0.9.5/firenado/config.py
+-rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)    16157 2024-04-22 23:21:56.000000 firenado-0.9.5/firenado/data.py
+-rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)    12677 2024-02-19 05:23:58.000000 firenado-0.9.5/firenado/launcher.py
+drwxr-xr-x   0 fpiraz    (1000) fpiraz    (1000)        0 2024-04-23 19:08:59.997140 firenado-0.9.5/firenado/management/
+-rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)      738 2019-05-18 04:12:04.000000 firenado-0.9.5/firenado/management/__init__.py
+-rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)     1993 2020-02-29 17:12:35.000000 firenado-0.9.5/firenado/management/commands.py
+-rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)     8615 2023-06-10 05:24:28.000000 firenado-0.9.5/firenado/management/management.py
+-rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)     6784 2023-06-10 05:27:13.000000 firenado-0.9.5/firenado/management/tasks.py
+drwxr-xr-x   0 fpiraz    (1000) fpiraz    (1000)        0 2024-04-23 19:08:59.987140 firenado-0.9.5/firenado/management/templates/
+drwxr-xr-x   0 fpiraz    (1000) fpiraz    (1000)        0 2024-04-23 19:08:59.998140 firenado-0.9.5/firenado/management/templates/help/
+-rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)      160 2016-09-08 01:38:40.000000 firenado-0.9.5/firenado/management/templates/help/app_command_help.txt
+-rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)      119 2018-11-03 23:08:57.000000 firenado-0.9.5/firenado/management/templates/help/header.txt
+-rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)       46 2016-09-08 01:38:40.000000 firenado-0.9.5/firenado/management/templates/help/init_command_help.txt
+-rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)      252 2018-11-03 23:09:50.000000 firenado-0.9.5/firenado/management/templates/help/main_command_help.txt
+-rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)      117 2017-06-19 04:13:32.000000 firenado-0.9.5/firenado/management/templates/help/project_command_help.txt
+-rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)      241 2020-02-29 17:12:35.000000 firenado-0.9.5/firenado/management/templates/help/random_command_help.txt
+drwxr-xr-x   0 fpiraz    (1000) fpiraz    (1000)        0 2024-04-23 19:08:59.998140 firenado-0.9.5/firenado/management/templates/project/
+-rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)      224 2018-11-21 07:38:12.000000 firenado-0.9.5/firenado/management/templates/project/app.py.txt
+-rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)      691 2016-09-10 17:22:04.000000 firenado-0.9.5/firenado/management/templates/project/firenado.yml.txt
+-rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)      212 2018-11-21 07:38:12.000000 firenado-0.9.5/firenado/management/templates/project/handlers.py.txt
+-rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)       54 2016-09-08 01:38:40.000000 firenado-0.9.5/firenado/management/templates/project/init_command_help.txt
+-rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)    15329 2024-02-16 22:26:37.000000 firenado-0.9.5/firenado/schedule.py
+-rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)    10092 2024-02-19 07:20:27.000000 firenado-0.9.5/firenado/security.py
+-rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)     4894 2023-06-10 05:21:44.000000 firenado-0.9.5/firenado/service.py
+-rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)    22703 2024-04-22 22:21:01.000000 firenado-0.9.5/firenado/session.py
+-rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)     6260 2024-04-22 03:21:29.000000 firenado-0.9.5/firenado/sqlalchemy.py
+-rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)     3366 2024-04-22 21:48:07.000000 firenado-0.9.5/firenado/testing.py
+-rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)    21703 2024-04-22 22:21:40.000000 firenado-0.9.5/firenado/tornadoweb.py
+-rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)      847 2023-06-10 05:23:10.000000 firenado-0.9.5/firenado/uimodules.py
+drwxr-xr-x   0 fpiraz    (1000) fpiraz    (1000)        0 2024-04-23 19:08:59.999140 firenado-0.9.5/firenado/util/
+-rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)        1 2023-11-25 18:15:35.000000 firenado-0.9.5/firenado/util/__init__.py
+-rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)     1084 2023-06-10 05:28:19.000000 firenado-0.9.5/firenado/util/argparse_util.py
+-rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)      901 2023-06-10 05:28:55.000000 firenado-0.9.5/firenado/util/sqlalchemy_util.py
+-rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)      896 2023-06-10 05:28:37.000000 firenado-0.9.5/firenado/util/url_util.py
+drwxr-xr-x   0 fpiraz    (1000) fpiraz    (1000)        0 2024-04-23 19:09:00.000140 firenado-0.9.5/requirements/
+-rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)       62 2020-07-28 14:20:19.000000 firenado-0.9.5/requirements/all.txt
+-rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)       41 2024-04-21 04:14:11.000000 firenado-0.9.5/requirements/basic.txt
+-rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)       15 2024-02-06 18:52:02.000000 firenado-0.9.5/requirements/pexpect.txt
+-rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)       28 2024-02-06 18:52:07.000000 firenado-0.9.5/requirements/redis.txt
+-rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)       16 2023-11-22 03:01:02.000000 firenado-0.9.5/requirements/schedule.txt
+-rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)       19 2024-04-21 23:24:26.000000 firenado-0.9.5/requirements/sqlalchemy.txt
+-rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)      103 2024-04-23 19:09:00.006140 firenado-0.9.5/setup.cfg
+-rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)     3669 2024-04-22 21:27:02.000000 firenado-0.9.5/setup.py
+drwxr-xr-x   0 fpiraz    (1000) fpiraz    (1000)        0 2024-04-23 19:09:00.003140 firenado-0.9.5/tests/
+-rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)     2180 2024-02-06 21:27:09.000000 firenado-0.9.5/tests/__init__.py
+-rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)     2010 2022-12-18 22:09:16.000000 firenado-0.9.5/tests/components_test.py
+-rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)     9962 2023-06-10 05:31:08.000000 firenado-0.9.5/tests/conf_test.py
+-rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)     1854 2024-04-23 18:08:20.000000 firenado-0.9.5/tests/config_test.py
+-rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)     5212 2023-06-10 05:31:35.000000 firenado-0.9.5/tests/data_test.py
+drwxr-xr-x   0 fpiraz    (1000) fpiraz    (1000)        0 2024-04-23 19:09:00.003140 firenado-0.9.5/tests/features/
+-rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)        0 2019-05-18 04:12:19.000000 firenado-0.9.5/tests/features/__init__.py
+-rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)     1021 2024-02-21 23:51:47.000000 firenado-0.9.5/tests/features/environment.py
+drwxr-xr-x   0 fpiraz    (1000) fpiraz    (1000)        0 2024-04-23 19:09:00.003140 firenado-0.9.5/tests/features/steps/
+-rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)        0 2020-03-17 14:16:49.000000 firenado-0.9.5/tests/features/steps/__init__.py
+-rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)     1037 2023-06-16 03:06:08.000000 firenado-0.9.5/tests/features/steps/cli.py
+-rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)     2212 2024-02-23 16:19:30.000000 firenado-0.9.5/tests/features/steps/launcher.py
+-rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)     2202 2024-02-23 16:32:18.000000 firenado-0.9.5/tests/loader_test.py
+-rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)     1964 2024-02-23 16:22:57.000000 firenado-0.9.5/tests/runtests.py
+-rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)     3025 2024-02-21 22:32:52.000000 firenado-0.9.5/tests/security_test.py
+-rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)     7392 2024-04-22 21:48:23.000000 firenado-0.9.5/tests/service_test.py
+-rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)     5170 2023-06-10 05:32:35.000000 firenado-0.9.5/tests/session_test.py
+-rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)     8920 2024-04-22 21:49:35.000000 firenado-0.9.5/tests/sqlalchemy_test.py
+-rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)     2308 2024-04-22 21:19:48.000000 firenado-0.9.5/tests/testing_test.py
+-rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)     6025 2023-06-10 05:32:56.000000 firenado-0.9.5/tests/tornadoweb_test.py
+drwxr-xr-x   0 fpiraz    (1000) fpiraz    (1000)        0 2024-04-23 19:09:00.004140 firenado-0.9.5/tests/util/
+-rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)        0 2018-07-08 04:28:25.000000 firenado-0.9.5/tests/util/__init__.py
+-rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)     1895 2021-03-23 17:10:31.000000 firenado-0.9.5/tests/util/url_util_test.py
```

### Comparing `Firenado-0.9.4/Firenado.egg-info/PKG-INFO` & `firenado-0.9.5/Firenado.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Firenado
-Version: 0.9.4
+Version: 0.9.5
 Summary: Firenado is a python web framework based on Tornado web framework/server.
 Home-page: https://github.com/candango/firenado
 Author: Flavio Garcia
 Author-email: piraz@candango.org
 Maintainer: Flavio Garcia
 Maintainer-email: piraz@candango.org
 License: Apache License V2.0
@@ -25,31 +25,31 @@
 Classifier: Topic :: Internet :: WWW/HTTP :: WSGI
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >= 3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: cartola>=0.18
-Requires-Dist: taskio==0.0.6
+Requires-Dist: taskio==0.0.7
 Requires-Dist: tornado==6.4
 Provides-Extra: all
 Requires-Dist: pexpect>=4.9.0; extra == "all"
 Requires-Dist: redis>=5.0.1; extra == "all"
 Requires-Dist: hiredis>=2.3.2; extra == "all"
 Requires-Dist: croniter==2.0.1; extra == "all"
-Requires-Dist: sqlalchemy>=2.0.23; extra == "all"
+Requires-Dist: sqlalchemy>=2.0.29; extra == "all"
 Provides-Extra: redis
 Requires-Dist: redis>=5.0.1; extra == "redis"
 Requires-Dist: hiredis>=2.3.2; extra == "redis"
 Provides-Extra: pexpect
 Requires-Dist: pexpect>=4.9.0; extra == "pexpect"
 Provides-Extra: schedule
 Requires-Dist: croniter==2.0.1; extra == "schedule"
 Provides-Extra: sqlalchemy
-Requires-Dist: sqlalchemy>=2.0.23; extra == "sqlalchemy"
+Requires-Dist: sqlalchemy>=2.0.29; extra == "sqlalchemy"
 
 # Firenado Framework 
 
 [![Latest PyPI version](https://img.shields.io/pypi/v/firenado.svg)](https://pypi.org/project/firenado/)
 [![Number of PyPI downloads](https://img.shields.io/pypi/dm/firenado.svg)](https://pypi.org/project/firenado/#files)
 [![Build Status](https://img.shields.io/endpoint.svg?url=https%3A%2F%2Factions-badge.atrox.dev%2Fcandango%2Ffirenado%2Fbadge&style=flat)](https://actions-badge.atrox.dev/candango/firenado/goto)
 [![GitHub license](https://img.shields.io/github/license/candango/firenado)](https://github.com/candango/firenado/blob/develop/LICENSE)
```

### Comparing `Firenado-0.9.4/Firenado.egg-info/SOURCES.txt` & `firenado-0.9.5/Firenado.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Firenado-0.9.4/LICENSE` & `firenado-0.9.5/LICENSE`

 * *Files 2% similar despite different names*

```diff
@@ -182,15 +182,15 @@
       replaced with your own identifying information. (Don't include
       the brackets!)  The text should be enclosed in the appropriate
       comment syntax for the file format. We also recommend that a
       file or class name and description of purpose be included on the
       same "printed page" as the copyright notice for easier
       identification within third-party archives.
 
-   Copyright 2015-2022 Flávio Gonçalves Garcia
+   Copyright 2015-2024 Flavio Garcia
 
    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at
 
        http://www.apache.org/licenses/LICENSE-2.0
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `Firenado-0.9.4/MANIFEST.in` & `firenado-0.9.5/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `Firenado-0.9.4/PKG-INFO` & `firenado-0.9.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Firenado
-Version: 0.9.4
+Version: 0.9.5
 Summary: Firenado is a python web framework based on Tornado web framework/server.
 Home-page: https://github.com/candango/firenado
 Author: Flavio Garcia
 Author-email: piraz@candango.org
 Maintainer: Flavio Garcia
 Maintainer-email: piraz@candango.org
 License: Apache License V2.0
@@ -25,31 +25,31 @@
 Classifier: Topic :: Internet :: WWW/HTTP :: WSGI
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >= 3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: cartola>=0.18
-Requires-Dist: taskio==0.0.6
+Requires-Dist: taskio==0.0.7
 Requires-Dist: tornado==6.4
 Provides-Extra: all
 Requires-Dist: pexpect>=4.9.0; extra == "all"
 Requires-Dist: redis>=5.0.1; extra == "all"
 Requires-Dist: hiredis>=2.3.2; extra == "all"
 Requires-Dist: croniter==2.0.1; extra == "all"
-Requires-Dist: sqlalchemy>=2.0.23; extra == "all"
+Requires-Dist: sqlalchemy>=2.0.29; extra == "all"
 Provides-Extra: redis
 Requires-Dist: redis>=5.0.1; extra == "redis"
 Requires-Dist: hiredis>=2.3.2; extra == "redis"
 Provides-Extra: pexpect
 Requires-Dist: pexpect>=4.9.0; extra == "pexpect"
 Provides-Extra: schedule
 Requires-Dist: croniter==2.0.1; extra == "schedule"
 Provides-Extra: sqlalchemy
-Requires-Dist: sqlalchemy>=2.0.23; extra == "sqlalchemy"
+Requires-Dist: sqlalchemy>=2.0.29; extra == "sqlalchemy"
 
 # Firenado Framework 
 
 [![Latest PyPI version](https://img.shields.io/pypi/v/firenado.svg)](https://pypi.org/project/firenado/)
 [![Number of PyPI downloads](https://img.shields.io/pypi/dm/firenado.svg)](https://pypi.org/project/firenado/#files)
 [![Build Status](https://img.shields.io/endpoint.svg?url=https%3A%2F%2Factions-badge.atrox.dev%2Fcandango%2Ffirenado%2Fbadge&style=flat)](https://actions-badge.atrox.dev/candango/firenado/goto)
 [![GitHub license](https://img.shields.io/github/license/candango/firenado)](https://github.com/candango/firenado/blob/develop/LICENSE)
```

### Comparing `Firenado-0.9.4/README.md` & `firenado-0.9.5/README.md`

 * *Files identical despite different names*

### Comparing `Firenado-0.9.4/README.rst` & `firenado-0.9.5/README.rst`

 * *Files identical despite different names*

### Comparing `Firenado-0.9.4/firenado/__init__.py` & `firenado-0.9.5/firenado/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
 """The Firenado Framework"""
 
 __author__ = "Flavio Garcia <piraz@candango.org>"
-__version__ = (0, 9, 4)
+__version__ = (0, 9, 5)
 __licence__ = "Apache License V2.0"
 
 
 def get_version():
     if isinstance(__version__[-1], str):
         return '.'.join(map(str, __version__[:-1])) + __version__[-1]
     return ".".join(map(str, __version__))
```

### Comparing `Firenado-0.9.4/firenado/bin/firenado-cli.py` & `firenado-0.9.5/firenado/bin/firenado-cli.py`

 * *Files identical despite different names*

### Comparing `Firenado-0.9.4/firenado/bin/firenado-cli1.py` & `firenado-0.9.5/firenado/bin/firenado-cli1.py`

 * *Files identical despite different names*

### Comparing `Firenado-0.9.4/firenado/cli/commands.py` & `firenado-0.9.5/firenado/cli/commands.py`

 * *Files identical despite different names*

### Comparing `Firenado-0.9.4/firenado/components/__init__.py` & `firenado-0.9.5/firenado/components/__init__.py`

 * *Files identical despite different names*

### Comparing `Firenado-0.9.4/firenado/components/firenado/component.py` & `firenado-0.9.5/firenado/components/firenado/component.py`

 * *Files identical despite different names*

### Comparing `Firenado-0.9.4/firenado/components/firenado/handlers.py` & `firenado-0.9.5/firenado/components/firenado/handlers.py`

 * *Files identical despite different names*

### Comparing `Firenado-0.9.4/firenado/components/firenado/templates/info.html` & `firenado-0.9.5/firenado/components/firenado/templates/info.html`

 * *Files identical despite different names*

### Comparing `Firenado-0.9.4/firenado/components/static_maps/component.py` & `firenado-0.9.5/firenado/components/static_maps/component.py`

 * *Files identical despite different names*

### Comparing `Firenado-0.9.4/firenado/components/toolbox/component.py` & `firenado-0.9.5/firenado/components/toolbox/component.py`

 * *Files identical despite different names*

### Comparing `Firenado-0.9.4/firenado/components/toolbox/uimodules.py` & `firenado-0.9.5/firenado/components/toolbox/uimodules.py`

 * *Files identical despite different names*

### Comparing `Firenado-0.9.4/firenado/conf/__init__.py` & `firenado-0.9.5/firenado/conf/__init__.py`

 * *Files identical despite different names*

### Comparing `Firenado-0.9.4/firenado/conf/firenado.yml` & `firenado-0.9.5/firenado/conf/firenado.yml`

 * *Files identical despite different names*

### Comparing `Firenado-0.9.4/firenado/config.py` & `firenado-0.9.5/firenado/config.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,23 @@
-# -*- coding: UTF-8 -*-
-#
-# Copyright 2015-2023 Flavio Garcia
+# Copyright 2015-2024 Flavio Garcia
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from cartola import sysexits
-from cartola.config import load_yaml_file, log_level_from_string
+from cartola.config import get_from_dict, load_yaml_file, log_level_from_string
 import logging
 import os
 
 
 def get_app_defaults():
     """ Return the application configuration defaults
     :return:
@@ -66,54 +64,21 @@
 
 def get_config_from_package(package):
     """ Breaks a package string in module and class.
 
     :param package: A package string.
     :return: A config dict with class and module.
     """
-    package_x = package.split('.')
+    package_x = package.split(".")
     package_conf = {}
     package_conf['class'] = package_x[-1]
-    package_conf['module'] = '.'.join(package_x[:-1][:])
+    package_conf['module'] = ".".join(package_x[:-1][:])
     return package_conf
 
 
-def get_class_from_name(name):
-    """ Return a class reference from the class name provided as a parameter.
-    Class name must be the full class reference, in another words, the module
-    with the class absolute reference.
-
-    Example:
-    >>> get_class_from_name("my.module.Myclass")
-
-    :param basestring name: Class absolute reference.
-    :return: The class resolved from the absolute reference name provided.
-    """
-    return get_class_from_module(
-        ".".join(name.split(".")[:-1]),
-        name.split(".")[-1]
-    )
-
-
-def get_class_from_module(module, class_name):
-    """ Returns a class from a module and a class name parameters.
-    This function is used by get_class_from_config and get_class_from_name.
-
-    Example:
-    >>> get_class_from_module("my.module", "MyClass")
-
-    :param basestring module: The module name.
-    :param basestring class_name: The class name.
-    :return: The class resolved by the module and class name provided.
-    """
-    import importlib
-    module = importlib.import_module(module)
-    return getattr(module, class_name)
-
-
 def get_class_from_config(config, index="class"):
     """ Return a class from a config dict bit containing the indexes module and
     class.
 
     Examples:
 
     When class name index into the config is class:
@@ -124,15 +89,15 @@
     >>> config = {'module': "my.module", 'my_class': "MyClass"}
     >>> get_class_from_config(config, index="my_class")
 
     :param dict config: Config containing index and module information.
     :param basestring index: Index to be used to get the class name
     :return: The class resolved at the module referred into the config.
     """
-    return get_class_from_module(config['module'], config[index])
+    return get_from_dict(config, module_index="module", attr_index=index)
 
 
 def process_config(config, config_data):
     """ Populates config with data from the configuration data dict. It handles
     components, data, log, management and session sections from the
     configuration data.
 
@@ -233,106 +198,102 @@
 def process_app_config_section(config, app_config):
     """ Processes the app section from a configuration data dict.
 
     :param config: The config reference of the object that will hold the
     configuration data from the config_data.
     :param app_config: App section from a config data dict.
     """
-    if 'addresses' in app_config:
+    if "addresses" in app_config:
         config.app['addresses'] = app_config['addresses']
-    if 'component' in app_config:
+    if "component" in app_config:
         config.app['component'] = app_config['component']
-    if 'data' in app_config:
-        if 'sources' in app_config['data']:
-            config.app['data']['sources'] = app_config['data']['sources']
-    if 'id' in app_config:
+    if "data" in app_config and "sources" in app_config['data']:
+        config.app['data']['sources'] = app_config['data']['sources']
+    if "id" in app_config:
         config.app['id'] = app_config['id']
-    if 'login' in app_config:
-        if 'urls' in app_config['login']:
-            if app_config['login']['urls']:
-                for url in app_config['login']['urls']:
-                    config.app['login']['urls'][url['name']] = url['value']
-    if 'pythonpath' in app_config:
+    if "login" in app_config and "urls" in app_config['login']:
+        if len(app_config['login']['urls']) > 0:
+            for url in app_config['login']['urls']:
+                config.app['login']['urls'][url['name']] = url['value']
+    if "pythonpath" in app_config:
         config.app['pythonpath'] = app_config['pythonpath']
-    if 'port' in app_config:
+    if "port" in app_config:
         config.app['port'] = app_config['port']
-    if 'process' in app_config:
-        if 'num_processes' in app_config['process']:
-            config.app['process']['num_processes'] = app_config[
+    if "process" in app_config and "num_processes" in app_config['process']:
+        config.app['process']['num_processes'] = app_config[
                 'process']['num_processes']
-    if 'url_root_path' in app_config:
+    if "url_root_path" in app_config:
         root_url = app_config['url_root_path'].strip()
         if root_url[0] == "/":
             root_url = root_url[1:]
         if root_url == "":
             root_url = None
         config.app['url_root_path'] = root_url
-    if 'settings' in app_config:
+    if "settings" in app_config:
         config.app['settings'] = app_config['settings']
-    if 'socket' in app_config:
+    if "socket" in app_config:
         config.app['socket'] = app_config['socket']
-    if 'static_path' in app_config:
+    if "static_path" in app_config:
         config.app['static_path'] = app_config['static_path']
-    if 'static_url_prefix' in app_config:
+    if "static_url_prefix" in app_config:
         config.app['static_url_prefix'] = app_config['static_url_prefix']
-    if 'type' in app_config:
+    if "type" in app_config:
         config.app['type'] = app_config['type']
-    if 'types' in app_config:
+    if "types" in app_config:
         for app_type in app_config['types']:
             app_type['launcher'] = get_config_from_package(
                 app_type['launcher'])
             config.app['types'][app_type['name']] = app_type
-    if 'xheaders' in app_config:
+    if "xheaders" in app_config:
         config.app['xheaders'] = app_config['xheaders']
-    if 'wait_before_shutdown' in app_config:
+    if "wait_before_shutdown" in app_config:
         config.app['wait_before_shutdown'] = app_config['wait_before_shutdown']
 
 
 def process_components_config_section(config, components_config):
     """ Processes the components section from a configuration data dict.
 
     :param config: The config reference of the object that will hold the
     configuration data from the config_data.
     :param components_config: Data section from a config data dict.
     """
     for component_config in components_config:
-        if 'id' not in component_config:
+        if "id" not in component_config:
             raise Exception('The component %s was defined without an id.' %
                             component_config)
         component_id = component_config['id']
         if component_id not in config.components:
             config.components[component_id] = {}
             config.components[component_id]['enabled'] = False
             config.components[component_id]['config'] = {}
-        if 'class' in component_config:
-            class_config_x = component_config['class'].split('.')
+        if "class" in component_config:
+            class_config_x = component_config['class'].split(".")
             config.components[component_id]['class'] = class_config_x[-1]
-            config.components[component_id]['module'] = '.'.join(
+            config.components[component_id]['module'] = ".".join(
                 class_config_x[:-1])
-        if 'enabled' in component_config:
+        if "enabled" in component_config:
             config.components[component_id]['enabled'] = bool(
                 component_config['enabled'])
 
 
 def process_data_config_section(config, data_config):
     """ Processes the data configuration section from the configuration
     data dict.
 
     :param config: The config reference of the object that will hold the
     configuration data from the config_data.
     :param data_config: Data configuration section from a config data dict.
     """
-    if 'connectors' in data_config:
+    if "connectors" in data_config:
         for connector in data_config['connectors']:
             config.data['connectors'][
                 connector['name']] = get_config_from_package(
                 connector['class'])
-    if 'sources' in data_config:
-        if data_config['sources']:
-            process_data_sources_config(config, data_config['sources'])
+    if "sources" in data_config and data_config['sources']:
+        process_data_sources_config(config, data_config['sources'])
 
 
 def process_data_sources_config_file(config, file):
     if not os.path.isabs(file):
         file = os.path.join(config.APP_CONFIG_PATH, file)
         sources_config = load_yaml_file(file)
         process_data_sources_config(config, sources_config)
@@ -350,89 +311,87 @@
 def process_log_config_section(config, log_config):
     """ Processes the log section from a configuration  data dict.
 
     :param config: The config reference of the object that will hold the
     configuration data from the config_data.
     :param log_config: Log section from a config data dict.
     """
-    if 'format' in log_config:
+    if "format" in log_config:
         config.log['format'] = log_config['format']
-    if 'level' in log_config:
+    if "level" in log_config:
         config.log['level'] = log_level_from_string(log_config['level'])
 
 
 def process_management_config_section(config, management_config):
     """ Processes the management section from a configuration data dict.
 
     :param config: The config reference of the object that will hold the
     configuration data from the config_data.
     :param management_config: Management section from a config data dict.
     """
-    if 'commands' in management_config:
+    if "commands" in management_config:
         for command in management_config['commands']:
             config.management['commands'].append(command)
 
 
 def process_session_config_section(config, session_config):
     """ Processes the session section from the configuration data dict.
 
     :param config: The config reference of the object that will hold the
     configuration data from the config_data.
     :param session_config: Session configuration section from a config data
     dict.
     """
     # Setting session type as file by default
-    config.session['type'] = 'file'
-    if 'enabled' in session_config:
+    config.session['type'] = "file"
+    if "enabled" in session_config:
         config.session['enabled'] = session_config['enabled']
-    if 'type' in session_config:
+    if "type" in session_config:
         config.session['type'] = session_config['type']
-        if config.session['type'] == 'file':
-            if 'path' in session_config:
-                config.session['file']['path'] = session_config['path']
-        if config.session['type'] == 'redis':
-            if 'data' in session_config:
-                if 'source' in session_config['data']:
-                    config.session['redis']['data']['source'] = session_config[
-                        'data']['source']
-    if 'handlers' in session_config:
+        if config.session['type'] == 'file' and "path" in session_config:
+            config.session['file']['path'] = session_config['path']
+        if (config.session['type'] == 'redis' and "data" in session_config and
+                "source" in session_config['data']):
+            config.session['redis']['data']['source'] = session_config[
+                'data']['source']
+    if "handlers" in session_config:
         for handler in session_config['handlers']:
-            handler_class_x = handler['class'].split('.')
+            handler_class_x = handler['class'].split(".")
             handler['class'] = handler_class_x[-1]
-            handler['module'] = '.'.join(handler_class_x[:-1][:])
+            handler['module'] = ".".join(handler_class_x[:-1][:])
             config.session['handlers'][handler['name']] = handler
             del config.session['handlers'][handler['name']]['name']
-    if 'encoders' in session_config:
+    if "encoders" in session_config:
         for encoder in session_config['encoders']:
             encoder_class_x = encoder['class'].split('.')
             encoder['encoder'] = encoder_class_x[-1]
             encoder['class'] = encoder_class_x[-1]
             encoder['module'] = '.'.join(encoder_class_x[:-1][:])
             config.session['encoders'][encoder['name']] = encoder
             del config.session['encoders'][encoder['name']]['name']
-    if 'id_generators' in session_config:
+    if "id_generators" in session_config:
         for generator in session_config['id_generators']:
-            generator_ref_x = generator['function'].split('.')
+            generator_ref_x = generator['function'].split(".")
             generator['function'] = generator_ref_x[-1]
-            generator['module'] = '.'.join(generator_ref_x[:-1][:])
+            generator['module'] = ".".join(generator_ref_x[:-1][:])
             config.session['id_generators'][generator['name']] = generator
             del config.session['id_generators'][generator['name']]['name']
-    if 'name' in session_config:
+    if "name" in session_config:
         config.session['name'] = session_config['name']
-    if 'life_time' in session_config:
+    if "life_time" in session_config:
         config.session['life_time'] = session_config['life_time']
-    if 'callback_hiccup' in session_config:
+    if "callback_hiccup" in session_config:
         config.session['callback_hiccup'] = session_config['callback_hiccup']
-    if 'callback_time' in session_config:
+    if "callback_time" in session_config:
         config.session['callback_time'] = session_config['callback_time']
-    if 'prefix' in session_config:
+    if "prefix" in session_config:
         config.session['prefix'] = session_config['prefix']
-    if 'purge_limit' in session_config:
+    if "purge_limit" in session_config:
         config.session['purge_limit'] = session_config['purge_limit']
-    if 'encoder' in session_config:
+    if "encoder" in session_config:
         if session_config['encoder'] in config.session['encoders']:
             config.session['encoder'] = session_config['encoder']
         else:
             logger = logging.getLogger(__name__)
             logger.critical("The session encoder \"%s\" is not defined.",
                             session_config['encoder'])
             sysexits.exit_fatal(sysexits.EX_CONFIG)
```

### Comparing `Firenado-0.9.4/firenado/data.py` & `firenado-0.9.5/firenado/data.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2015-2023 Flavio Garcia
+# Copyright 2015-2024 Flavio Garcia
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -130,73 +130,81 @@
                 if key in ['db', 'port']:
                     db_conf[key] = int(conf[key])
                 db_conf[key] = conf[key]
         return db_conf
 
 
 class SqlalchemyConnector(Connector):
+    from sqlalchemy import Engine
     from sqlalchemy.orm import Session
     """ Connects a sqlalchemy engine to a data connected instance.
     Sqlalchemy support a big variety of relational database backends. The
     connection returned by this handler contains an engine and session created
     by sqlalchemy and the database backend name.
     """
+    __name: str
+    __engine: Engine
+    __connection: dict
 
-    def __init__(self, data_connected):
-        super(SqlalchemyConnector, self).__init__(data_connected)
-        self.__name = None
+    def configure(self, name, conf):
+        from sqlalchemy import Connection, create_engine
+        from sqlalchemy import exc, event, select
+        self.__name = name
         self.__connection = {
             'backend': None,
+            'ping': False,
             'session': {
+                'autobegin': True,
                 'autoflush': True,
                 'expire_on_commit': True,
                 'info': None
             }
         }
-        self.__engine = None
-
-    def configure(self, name, conf):
-        self.__name = name
-        from sqlalchemy import create_engine
-        from sqlalchemy import exc, event, select
         # We will set the isolation level to READ UNCOMMITTED by default
         # to avoid the "cache" effect sqlalchemy has without this option.
         # Solution from: http://bit.ly/2bDq0Nv
-        # TODO: Get the isolation level from data source conf
         engine_params = {
             'isolation_level': "READ UNCOMMITTED"
         }
 
         if "backend" in conf:
             if conf['backend'] == 'mysql':
                 # Setting connection default connection timeout for mysql
                 # backends as suggested on http://bit.ly/2bvOLxs
                 engine_params['pool_recycle'] = 3600
 
         if "future" in conf:
             if conf['future']:
                 engine_params['future'] = True
 
+        if "isolation_level" in conf:
+            if conf['isolation_level']:
+                engine_params['isolation_level'] = conf['isolation_level']
+
+        if "ping" in conf:
+            if conf['ping']:
+                engine_params['ping'] = conf['ping']
+
         if "pool" in conf:
             if "class" in conf['pool']:
                 engine_params['pool_class'] = conf['pool']['class']
                 if isinstance(engine_params['pool_class'], str):
                     engine_params['pool_class'] = config.get_from_string(
                         engine_params['pool_class'])
-            if "isolation_level" in conf['pool']:
-                engine_params['isolation_level'] = conf['pool'][
-                    'isolation_level']
             if "max_overflow" in conf['pool']:
                 engine_params['max_overflow'] = conf['pool']['max_overflow']
             if "pool_recycle" in conf['pool']:
                 engine_params['pool_recycle'] = conf['pool']['pool_recycle']
             if "size" in conf['pool']:
                 engine_params['pool_size'] = conf['pool']['size']
 
         if "session" in conf:
+            if "autobegin" in conf['session']:
+                self.__connection['session']['autobegin'] = conf['session'][
+                    'autobegin']
             if "autoflush" in conf['session']:
                 self.__connection['session']['autoflush'] = conf['session'][
                     'autoflush']
             if "expire_on_commit" in conf['session']:
                 self.__connection['session']['expire_on_commit'] = conf[
                     'session']['expire_on_commit']
             if "info" in conf['session']:
@@ -205,34 +213,38 @@
         if "url" not in conf:
             logger.error("It is not possible to create sqlalchemy engine"
                          "for %s datasource. Configuration: %s.", self.__name,
                          conf)
         self.__engine = create_engine(conf['url'], **engine_params)
 
         @event.listens_for(self.__engine, "engine_connect")
-        def ping_connection(connection, branch):
+        def ping_connection(conn: Connection, branch):
+            if not self.__connection['ping']:
+                return
             # Adding ping connection event handler as described at the
             # pessimistic disconnect section of: http://bit.ly/2c8Sm2t
             logger.debug("Pinging sqlalchemy connection.")
             if branch:
                 # "branch" refers to a sub-connection of a connection,
                 # we don't want to bother pinging on these.
                 logger.debug("The connection is a branch. There is no need to "
                              "ping those.")
                 return
             # turn off "close with result".  This flag is only used with
             # "connectionless" execution, otherwise will be False in any case
-            save_should_close_with_result = connection.should_close_with_result
-            connection.should_close_with_result = False
+            save_should_close_with_result = conn.should_close_with_result
+            conn.should_close_with_result = False
             try:
                 # run a SELECT 1.   use a core select() so that
                 # the SELECT of a scalar value without a table is
                 # appropriately formatted for the backend
                 logger.debug("Testing sqlalchemy connection.")
-                connection.scalar(select(1))
+                conn.begin()
+                conn.scalar(select(1))
+                conn.commit()
             except exc.DBAPIError as err:
                 logger.warning(err)
                 logger.warning("Firenado will try to reestablish the data "
                                "source connection.")
                 # catch SQLAlchemy's DBAPIError, which is a wrapper
                 # for the DBAPI's exception.  It includes a
                 # .connection_invalidated attribute which specifies if this
@@ -240,21 +252,23 @@
                 # inspection of the original exception by the dialect in use.
                 if err.connection_invalidated:
                     # run the same SELECT again - the connection will
                     # re-validate itself and establish a new connection.
                     # The disconnect detection here also causes the whole
                     # connection pool to be invalidated so that all stale
                     # connections are discarded.
-                    connection.scalar(select([1]))
+                    conn.begin()
+                    conn.scalar(select(1))
+                    conn.commit()
                     logger.warning("Data source connection reestablished.")
                 else:
                     raise
             finally:
                 # restore "close with result"
-                connection.should_close_with_result = (
+                conn.should_close_with_result = (
                     save_should_close_with_result)
         logger.info("Connecting to the database using the engine: %s.",
                     self.__engine)
         self.__connection['backend'] = conf['backend']
         # will just happen during the handler execution
 
     def get_connection(self):
@@ -269,27 +283,32 @@
             sys.exit(errno.ECONNREFUSED)
 
     def get_a_session(self, **kwargs) -> Session:
         """ Return a session bind to the datasource engine.
 
         Default parameters based on: https://bit.ly/3MjWDzF
         :param dict kwargs:
-        :key bool autoflush: Default to True
-        :key bool expire_on_commit: Default to False
+        :key bool autobegin: Default to False
+        :key bool autoflush: Default to False
+        :key bool expire_on_commit: Default to True
         :key dict info: Default to None
         :return Session:
         """
-        autoflush = kwargs.get("autoflush", True)
-        expire_on_commit = kwargs.get("expire_on_commit", True)
-        info = kwargs.get("info")
+        session_config = self.__connection['session']
+        autobegin = kwargs.get("autobegin", session_config['autobegin'])
+        autoflush = kwargs.get("autoflush", session_config['autoflush'])
+        expire_on_commit = kwargs.get("expire_on_commit",
+                                      session_config['expire_on_commit'])
+        info = kwargs.get("info", session_config['info'])
 
         from sqlalchemy.orm import sessionmaker
-        Session = sessionmaker(bind=self.__engine, autoflush=autoflush,
-                               expire_on_commit=expire_on_commit, info=info)
-        return Session()
+        maker = sessionmaker(bind=self.__engine, autoflush=autoflush,
+                             expire_on_commit=expire_on_commit, info=info,
+                             autobegin=autobegin)
+        return maker()
 
     @property
     def backend(self):
         return self.__connection['backend']
 
     @property
     def engine(self):
```

### Comparing `Firenado-0.9.4/firenado/launcher.py` & `firenado-0.9.5/firenado/launcher.py`

 * *Files identical despite different names*

### Comparing `Firenado-0.9.4/firenado/management/__init__.py` & `firenado-0.9.5/firenado/management/__init__.py`

 * *Files identical despite different names*

### Comparing `Firenado-0.9.4/firenado/management/commands.py` & `firenado-0.9.5/firenado/management/commands.py`

 * *Files identical despite different names*

### Comparing `Firenado-0.9.4/firenado/management/management.py` & `firenado-0.9.5/firenado/management/management.py`

 * *Files identical despite different names*

### Comparing `Firenado-0.9.4/firenado/management/tasks.py` & `firenado-0.9.5/firenado/management/tasks.py`

 * *Files identical despite different names*

### Comparing `Firenado-0.9.4/firenado/management/templates/project/firenado.yml.txt` & `firenado-0.9.5/firenado/management/templates/project/firenado.yml.txt`

 * *Files identical despite different names*

### Comparing `Firenado-0.9.4/firenado/schedule.py` & `firenado-0.9.5/firenado/schedule.py`

 * *Files identical despite different names*

### Comparing `Firenado-0.9.4/firenado/security.py` & `firenado-0.9.5/firenado/security.py`

 * *Files identical despite different names*

### Comparing `Firenado-0.9.4/firenado/service.py` & `firenado-0.9.5/firenado/service.py`

 * *Files identical despite different names*

### Comparing `Firenado-0.9.4/firenado/session.py` & `firenado-0.9.5/firenado/session.py`

 * *Files 0% similar despite different names*

```diff
@@ -186,23 +186,23 @@
         self.id = sess_id
         self.__data = {} if data is None else data
         self.__params = {}
         self.__destroyed = False
         self.__changed = False
 
     def clear(self):
-        """ Clear all data stored into the session. This is not 
-        renewing/creating a new session id. If you want that use 
+        """ Clear all data stored into the session. This is not
+        renewing/creating a new session id. If you want that use
         session.destroy() """
         self.__data.clear()
         self.__changed = True
 
     def destroy(self, request_handler):
-        """ Clearing session data and marking the session to be
-        renewed at the end of the request. """
+        """ Clearing session data and marking the session to be renewed at the
+        end of the request. """
         self.clear()
         self.__destroyed = True
         self.__engine.store_session(request_handler)
 
     def get(self, key):
         """ Returns the value from the session data by a given key """
         self.__lock_if_destroyed()
```

### Comparing `Firenado-0.9.4/firenado/sqlalchemy.py` & `firenado-0.9.5/firenado/sqlalchemy.py`

 * *Files 2% similar despite different names*

```diff
@@ -129,14 +129,16 @@
                                      "index \"%s\" related to the service.",
                                      data_source)
             result = method(self, *method_args, **method_kwargs)
             if close:
                 if not session:
                     logger.warning("No session was resolved.")
                 logger.debug("Closing session %s.", session)
+                if hasattr(session, "autoflush") and not session.autoflush:
+                    session.flush()
                 session.close()
             return result
         return wrapper
     # If the decorator has no parameter, I mean no parentesis, we need to wrap
     # the service variable again , instead of the service instance, we need to
     # deal with the method being decorated but as a <function> instace.
     if isfunction(service):
```

### Comparing `Firenado-0.9.4/firenado/testing.py` & `firenado-0.9.5/firenado/testing.py`

 * *Files 18% similar despite different names*

```diff
@@ -9,29 +9,60 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import asyncio
+from firenado.service import FirenadoService
 from firenado.launcher import ProcessLauncher, TornadoLauncher
 from tornado.testing import (bind_unused_port, AsyncTestCase,
                              AsyncHTTPTestCase)
+from unittest import TestCase
 
 
 def get_event_loop():
     """ Return a new event asyncio evenvent loop with trigerring a
     depreciation warning from Python 10.
 
     :return: A event loop
     """
     loop = asyncio.get_event_loop_policy().get_event_loop()
     return loop if loop else asyncio.new_event_loop()
 
 
+class ServiceTestCase(TestCase):
+
+    def setUp(self):
+        """ Call the configure data connection method
+        """
+        self.configure_data_connected()
+
+    def configure_data_connected(self):
+        """Should be overridden with the configutation of the data connected
+        instance
+        """
+        raise NotImplementedError()
+
+    @property
+    def data_connected(self):
+        """Should be overridden by subclasses to return a data connected
+        instance
+        """
+        raise NotImplementedError()
+
+
+class TestableService(FirenadoService):
+    """ Serves a data connected method directly.
+    When decorating a data connected directly the service must return the
+    consumer.
+    """
+    pass
+
+
 class TornadoAsyncTestCase(AsyncTestCase):
 
     @property
     def launcher(self) -> ProcessLauncher:
         return self.__launcher
 
     def get_launcher(self) -> ProcessLauncher:
```

### Comparing `Firenado-0.9.4/firenado/tornadoweb.py` & `firenado-0.9.5/firenado/tornadoweb.py`

 * *Files identical despite different names*

### Comparing `Firenado-0.9.4/firenado/uimodules.py` & `firenado-0.9.5/firenado/uimodules.py`

 * *Files identical despite different names*

### Comparing `Firenado-0.9.4/firenado/util/argparse_util.py` & `firenado-0.9.5/firenado/util/argparse_util.py`

 * *Files identical despite different names*

### Comparing `Firenado-0.9.4/firenado/util/sqlalchemy_util.py` & `firenado-0.9.5/firenado/util/sqlalchemy_util.py`

 * *Files identical despite different names*

### Comparing `Firenado-0.9.4/firenado/util/url_util.py` & `firenado-0.9.5/firenado/util/url_util.py`

 * *Files identical despite different names*

### Comparing `Firenado-0.9.4/setup.py` & `firenado-0.9.5/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python
 #
-# Copyright 2015-2023 Flavio Garcia
+# Copyright 2015-2024 Flavio Garcia
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -12,43 +12,38 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import firenado
 from setuptools import setup, find_packages
-import sys
+import os
 
-try:
-    # for pip >= 10
-    from pip._internal.req import parse_requirements
-except ImportError:
-    # for pip <= 9.0.3
-    print("error: Upgrade to a pip version newer than 10. Run \"pip install "
-          "--upgrade pip\".")
-    sys.exit(1)
+with open("README.md", "r") as fh:
+    long_description = fh.read()
 
 
 # Solution from http://bit.ly/29Yl8VN
 def resolve_requires(requirements_file):
-    try:
-        requirements = parse_requirements("./%s" % requirements_file,
-                                          session=False)
-        return [str(ir.req) for ir in requirements]
-    except AttributeError:
-        # for pip >= 20.1.x
-        # Need to run again as the first run was ruined by the exception
-        requirements = parse_requirements("./%s" % requirements_file,
-                                          session=False)
-        # pr stands for parsed_requirement
-        return [str(pr.requirement) for pr in requirements]
-
+    requires = []
+    if os.path.isfile(f"./{requirements_file}"):
+        file_dir = os.path.dirname(f"./{requirements_file}")
+        with open(f"./{requirements_file}") as f:
+            for raw_line in f.readlines():
+                line = raw_line.strip().replace("\n", "")
+                if len(line) > 0:
+                    if line.startswith("-r "):
+                        partial_file = os.path.join(file_dir, line.replace(
+                            "-r ", ""))
+                        partial_requires = resolve_requires(partial_file)
+                        requires = requires + partial_requires
+                        continue
+                    requires.append(line)
+    return requires
 
-with open("README.md", "r") as fh:
-    long_description = fh.read()
 
 setup(
     name="Firenado",
     version=firenado.get_version(),
     description="Firenado is a python web framework based on Tornado web "
                 "framework/server.",
     long_description=long_description,
```

### Comparing `Firenado-0.9.4/tests/__init__.py` & `firenado-0.9.5/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `Firenado-0.9.4/tests/components_test.py` & `firenado-0.9.5/tests/components_test.py`

 * *Files identical despite different names*

### Comparing `Firenado-0.9.4/tests/conf_test.py` & `firenado-0.9.5/tests/conf_test.py`

 * *Files identical despite different names*

### Comparing `Firenado-0.9.4/tests/config_test.py` & `firenado-0.9.5/tests/config_test.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,26 +1,24 @@
-#!/usr/bin/env python
-#
-# Copyright 2015-2023 Flavio Garcia
+# Copyright 2015-2024 Flavio Garcia
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+from cartola.config import get_from_module, get_from_string
 import unittest
-from firenado.config import (get_class_from_config, get_class_from_module,
-                             get_class_from_name)
+from firenado.config import get_class_from_config
 from firenado.session import SessionEngine
 
 
 class GetClassTestCase(unittest.TestCase):
     """ Case that test all get class functions.
     """
 
@@ -36,14 +34,14 @@
         result_custom = get_class_from_config(custom_config, index="my_class")
 
         self.assertTrue(result == SessionEngine)
         self.assertTrue(result_custom == SessionEngine)
 
     def test_get_class_from_name(self):
         """ Getting a class from the full class name."""
-        result = get_class_from_name("firenado.session.SessionEngine")
+        result = get_from_string("firenado.session.SessionEngine")
         self.assertTrue(result == SessionEngine)
 
     def test_get_class_from_module(self):
         """ Getting a class from a given module and class name parameters. """
-        result = get_class_from_module("firenado.session", "SessionEngine")
+        result = get_from_module("firenado.session", "SessionEngine")
         self.assertTrue(result == SessionEngine)
```

### Comparing `Firenado-0.9.4/tests/data_test.py` & `firenado-0.9.5/tests/data_test.py`

 * *Files identical despite different names*

### Comparing `Firenado-0.9.4/tests/features/environment.py` & `firenado-0.9.5/tests/features/environment.py`

 * *Files identical despite different names*

### Comparing `Firenado-0.9.4/tests/features/steps/cli.py` & `firenado-0.9.5/tests/features/steps/cli.py`

 * *Files identical despite different names*

### Comparing `Firenado-0.9.4/tests/features/steps/launcher.py` & `firenado-0.9.5/tests/features/steps/launcher.py`

 * *Files identical despite different names*

### Comparing `Firenado-0.9.4/tests/loader_test.py` & `firenado-0.9.5/tests/loader_test.py`

 * *Files identical despite different names*

### Comparing `Firenado-0.9.4/tests/runtests.py` & `firenado-0.9.5/tests/runtests.py`

 * *Files identical despite different names*

### Comparing `Firenado-0.9.4/tests/security_test.py` & `firenado-0.9.5/tests/security_test.py`

 * *Files identical despite different names*

### Comparing `Firenado-0.9.4/tests/service_test.py` & `firenado-0.9.5/tests/service_test.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,23 +10,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from firenado.data import DataConnectedMixin
 from firenado.service import with_service, FirenadoService
-import unittest
-
-
-class TestableServiceDataConnected(FirenadoService):
-    """ Serves a data connected method directly.
-    When decorating a data connected directly the service must return the
-    consumer.
-    """
-    pass
+from firenado.testing import ServiceTestCase, TestableService
 
 
 class TestableSession(object):
 
     def __init__(self, data_source):
         self._data_source = data_source
         self._oppened = True
@@ -65,74 +57,63 @@
         return "Session resolved from data source"
 
     def resolve_session(self):
         return "%s: %s" % (self.session_resolved_string, self.name)
 
 
 class TestableDataConnected(DataConnectedMixin):
-    """ Data connected mock object. This object holds the data sources to be
+    """ Data connected dummy object. This object holds the data sources to be
     used in the test cases.
     """
 
-    testable_service_data_connected: TestableServiceDataConnected
+    testable_service: TestableService
 
     def __init__(self):
         self.data_sources['datasource1'] = TestableDataSource("DataSource1")
         self.data_sources['datasource2'] = TestableDataSource("DataSource2")
 
-    @with_service(TestableServiceDataConnected)
+    @with_service(TestableService)
     def get_service_data_sources_directly(self):
-        return self.testable_service_data_connected.get_data_sources()
-
-
-class TestableService(FirenadoService):
-    """ Service that decorates the instance to be served directly and
-    indirectly thought MockTestServiceRecursion.
-    When decorating directly data connected and data sources will be returned
-    in one interaction.
-    When decorating indirectly MockTestServiceRecursion will be used to return
-    the data connected instance and data sources.
-    """
-    pass
+        return self.testable_service.get_data_sources()
 
 
 class RecursiveService(FirenadoService):
     """ This service will be used to return the data connected reference
-    and data source, during the recursive test, delegating to MockTestService.
+    and data source, during the recursive test, delegating to TestableService.
     """
 
     testable_service: TestableService
 
     @with_service(TestableService)
     def get_service_data_sources_recursively(self):
         return self.testable_service.get_data_sources()
 
     @with_service(TestableService)
     def get_data_connected_recursively(self):
         return self.testable_service.data_connected
 
 
-class ServedByInstance(object):
+class ServedInstance(object):
     """ Class with methods to be decorated with the served_by decorator.
     """
 
     testable_service: TestableService
     recursive_service: RecursiveService
 
     def __init__(self, data_connected):
         self.data_connected = data_connected
 
     @with_service(TestableService)
-    def do_served_by_class(self):
+    def do_with_service_by_class(self):
         """ Method to be decorated with served_by with a class reference
         """
         pass
 
     @with_service("tests.service_test.TestableService")
-    def do_served_by_string(self):
+    def do_with_service_by_string(self):
         """ Method to be decorated with served_by with a string as class
         reference
         """
         pass
 
     @with_service(TestableService)
     def get_service_data_connected(self):
@@ -158,68 +139,67 @@
         """
         return (self.recursive_service.get_service_data_sources_recursively())
 
     def get_data_connected(self):
         return self.data_connected
 
 
-class ServiceTestCase(unittest.TestCase):
+class WithServiceTestCase(ServiceTestCase):
 
-    def setUp(self):
+    def configure_data_connected(self):
         """ Setting up an object that has firenado.core.service.served_by
         decorators on some methods.
         """
         self.data_connected_instance = TestableDataConnected()
-        self.served_by_instance = ServedByInstance(
-            self.data_connected_instance)
+        self.served_instance = ServedInstance(self.data_connected_instance)
 
-    def test_served_by_class_reference(self):
-        self.assertFalse(hasattr(self.served_by_instance, 'testable_service'))
-        self.served_by_instance.do_served_by_class()
-        self.assertTrue(hasattr(self.served_by_instance, 'testable_service'))
+    def test_with_service_class_reference(self):
+        self.assertFalse(hasattr(self.served_instance, "testable_service"))
+        self.served_instance.do_with_service_by_class()
+        self.assertTrue(hasattr(self.served_instance, "testable_service"))
         self.assertTrue(isinstance(
-            self.served_by_instance.testable_service, TestableService))
+            self.served_instance.testable_service, TestableService))
 
-    def test_served_by_class_name_string(self):
-        self.assertFalse(hasattr(self.served_by_instance, 'testable_service'))
-        self.served_by_instance.do_served_by_string()
-        self.assertTrue(hasattr(self.served_by_instance, 'testable_service'))
+    def test_with_service_class_name_string(self):
+        self.assertFalse(hasattr(self.served_instance, 'testable_service'))
+        self.served_instance.do_with_service_by_string()
+        self.assertTrue(hasattr(self.served_instance, 'testable_service'))
         self.assertEqual(
-            self.served_by_instance.testable_service.__class__.__name__,
+            self.served_instance.testable_service.__class__.__name__,
             TestableService.__name__)
 
     def test_data_connected_from_service(self):
-        data_connected = self.served_by_instance.get_data_connected()
+        data_connected = self.served_instance.get_data_connected()
         self.assertEqual(data_connected, self.data_connected_instance)
 
     def test_data_connected_from_service_recursively(self):
-        data_connected = (self.served_by_instance.
+        data_connected = (self.served_instance.
                           get_service_data_connected_recursively())
         self.assertEqual(data_connected, self.data_connected_instance)
 
     def test_data_connected_from_service_none(self):
         service = TestableService(None)
         data_connected = service.data_connected
         self.assertIsNone(data_connected)
 
     def test_get_data_source_from_service(self):
-        data_sources = self.served_by_instance.get_service_data_sources()
+        data_sources = self.served_instance.get_service_data_sources()
         self.assertTrue(len(data_sources) == 2)
         self.assertEqual(data_sources['datasource1'].name, "DataSource1")
         self.assertEqual(data_sources['datasource2'].name, "DataSource2")
 
     def test_get_data_source_from_data_connected(self):
         data_sources = (self.data_connected_instance.
                         get_service_data_sources_directly())
         self.assertTrue(len(data_sources) == 2)
         self.assertEqual(data_sources['datasource1'].name, "DataSource1")
         self.assertEqual(data_sources['datasource2'].name, "DataSource2")
 
     def test_get_data_source_from_service_recursively(self):
-        data_sources = (self.served_by_instance.
+        data_sources = (self.served_instance.
                         get_service_data_sources_recursively())
         self.assertTrue(len(data_sources) == 2)
         self.assertEqual(data_sources['datasource1'].name, "DataSource1")
         self.assertEqual(data_sources['datasource2'].name, "DataSource2")
 
     def test_get_data_source_from_service_none(self):
         service = TestableService(None)
```

### Comparing `Firenado-0.9.4/tests/session_test.py` & `firenado-0.9.5/tests/session_test.py`

 * *Files identical despite different names*

### Comparing `Firenado-0.9.4/tests/sqlalchemy_test.py` & `firenado-0.9.5/tests/sqlalchemy_test.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,17 +9,18 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from datetime import datetime
-from tests.service_test import TestableDataConnected, ServedByInstance
+from tests.service_test import TestableDataConnected, ServedInstance
 from firenado.sqlalchemy import base_to_dict, with_session
 from firenado.service import FirenadoService, with_service
+from firenado.testing import ServiceTestCase
 from sqlalchemy import String
 from sqlalchemy.types import DateTime
 from sqlalchemy.orm import DeclarativeBase, Mapped, mapped_column
 from sqlalchemy.sql import text
 import unittest
 
 
@@ -39,15 +40,15 @@
     email: Mapped[str] = mapped_column(String(150), nullable=False)
     created: Mapped[datetime] = mapped_column(DateTime, nullable=False,
                                               server_default=text("now()"))
     modified: Mapped[datetime] = mapped_column(DateTime, nullable=False,
                                                server_default=text("now()"))
 
 
-class MockSessionedService(FirenadoService):
+class DummySessionedService(FirenadoService):
 
     @with_session
     def resolve_from_default_data_source(self, **kwargs):
         return kwargs
 
     @with_session(data_source="datasource1")
     def resolve_from_data_source(self, **kwargs):
@@ -92,114 +93,113 @@
         self.assertTrue("password" not in dict_from_base)
         self.assertTrue("last_name" not in dict_from_base)
         self.assertTrue("email" not in dict_from_base)
         self.assertTrue("created" not in dict_from_base)
         self.assertTrue("modified" not in dict_from_base)
 
 
-class SessionedTestCase(unittest.TestCase):
+class SessionedTestCase(ServiceTestCase):
 
-    mock_sessioned_service: MockSessionedService
+    dummy_sessioned_service: DummySessionedService
 
-    def setUp(self):
+    def configure_data_connected(self):
         """ Setting up an object that has firenado.core.service.served_by
         decorators on some methods.
         """
         self.data_connected_instance = TestableDataConnected()
-        self.served_by_instance = ServedByInstance(
-            self.data_connected_instance)
+        self.served_by_instance = ServedInstance(self.data_connected_instance)
 
     @property
     def data_connected(self):
         return self.served_by_instance.data_connected
 
-    @with_service(MockSessionedService)
+    @with_service(DummySessionedService)
     def test_sessioned_default_data_source(self):
         """ Method resolve_from_default_data_source is anoteded with sessioned
         and no parameter. The data source to be used is the one defined either
         in the property or method named default_data_source. In this case we're
         using a property.
 
         As no session was provided the session will be closed
         """
         resolved_kwargs = (
-            self.mock_sessioned_service.resolve_from_default_data_source()
+            self.dummy_sessioned_service.resolve_from_default_data_source()
         )
         self.assertEqual("datasource2", resolved_kwargs['data_source'])
         data_source = self.data_connected.get_data_source(
             resolved_kwargs['data_source']
         )
         self.assertEqual(data_source.resolve_session(),
                          resolved_kwargs['session'].name)
         self.assertFalse(resolved_kwargs['session'].is_oppened)
 
-    @with_service(MockSessionedService)
+    @with_service(DummySessionedService)
     def test_sessioned_default_data_source_my_session(self):
         """ Method resolve_from_default_data_source is anoteded with sessioned
         and no parameter. Instead of getting the session from the default data
         source, we're providing our own session.
         """
         data_source = self.data_connected.get_data_source("datasource1")
         resolved_kwargs = (
-            self.mock_sessioned_service.resolve_from_default_data_source(
+            self.dummy_sessioned_service.resolve_from_default_data_source(
                 session=data_source.session
             )
         )
         # No datasource will be added to the kwards
         self.assertIsNone(resolved_kwargs.get("data_source"))
         # Using session provided
         self.assertEqual(data_source.resolve_session(),
                          resolved_kwargs['session'].name)
         self.assertTrue(resolved_kwargs['session'].is_oppened)
 
-    @with_service(MockSessionedService)
+    @with_service(DummySessionedService)
     def test_sessioned_from_data_source(self):
         """ Method resolve_from_data_source is anoteded with sessioned and
         datasource1 as parameter. It will be injected to the method kwargs
         session from datasource1.
         """
         resolved_kwargs = (
-            self.mock_sessioned_service.resolve_from_data_source()
+            self.dummy_sessioned_service.resolve_from_data_source()
         )
         self.assertEqual("datasource1", resolved_kwargs['data_source'])
         data_source = self.data_connected.get_data_source(
             resolved_kwargs['data_source']
         )
         self.assertEqual(data_source.resolve_session(),
                          resolved_kwargs['session'].name)
         self.assertFalse(resolved_kwargs['session'].is_oppened)
 
-    @with_service(MockSessionedService)
+    @with_service(DummySessionedService)
     def test_sessioned_from_data_source_provide_session(self):
         """ Method resolve_from_default_data_source is anoteded with sessioned
         and no parameter. This time we provide the session and provided to
         close the datasource after executing resolve_from_data_source.
         """
         data_source = self.data_connected.get_data_source("datasource2")
         resolved_kwargs = (
-            self.mock_sessioned_service.resolve_from_data_source(
+            self.dummy_sessioned_service.resolve_from_data_source(
                 session=data_source.session, close=True
             )
         )
         # No datasource will be added to the kwards
         self.assertIsNone(resolved_kwargs.get("data_source"))
         # Using session provided
         self.assertEqual(data_source.resolve_session(),
                          resolved_kwargs['session'].name)
         self.assertFalse(resolved_kwargs['session'].is_oppened)
 
-    @with_service(MockSessionedService)
+    @with_service(DummySessionedService)
     def test_sessioned_with_my_data_source_closing_connection(self):
         """ Method resolve_from_data_source is anoteded with sessioned and
         datasource1 as parameter. We're overwriting the data_source parameter
         during the method call, changing to datasource2. It will be injected
         to the method kwargs a session from data_source1.
         """
         resolved_kwargs = (
-            self.mock_sessioned_service.resolve_from_data_source(
+            self.dummy_sessioned_service.resolve_from_data_source(
                 data_source="datasource2")
         )
         self.assertEqual("datasource2", resolved_kwargs['data_source'])
         data_source = self.data_connected.get_data_source(
             resolved_kwargs['data_source']
         )
         self.assertEqual(data_source.resolve_session(),
```

### Comparing `Firenado-0.9.4/tests/testing_test.py` & `firenado-0.9.5/tests/testing_test.py`

 * *Files identical despite different names*

### Comparing `Firenado-0.9.4/tests/tornadoweb_test.py` & `firenado-0.9.5/tests/tornadoweb_test.py`

 * *Files identical despite different names*

### Comparing `Firenado-0.9.4/tests/util/url_util_test.py` & `firenado-0.9.5/tests/util/url_util_test.py`

 * *Files identical despite different names*

