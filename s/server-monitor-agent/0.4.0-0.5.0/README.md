# Comparing `tmp/server-monitor-agent-0.4.0.tar.gz` & `tmp/server_monitor_agent-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "server-monitor-agent-0.4.0.tar", last modified: Thu Nov 30 04:35:25 2023, max compression
+gzip compressed data, was "server_monitor_agent-0.5.0.tar", last modified: Tue Apr 23 00:43:13 2024, max compression
```

## Comparing `server-monitor-agent-0.4.0.tar` & `server_monitor_agent-0.5.0.tar`

### file list

```diff
@@ -1,94 +1,94 @@
-drwxrwxrwx   0        0        0        0 2023-11-30 04:35:25.040444 server-monitor-agent-0.4.0/
--rw-rw-rw-   0        0        0    11558 2023-11-20 03:29:37.000000 server-monitor-agent-0.4.0/LICENSE
--rw-rw-rw-   0        0        0       73 2023-11-20 03:29:37.000000 server-monitor-agent-0.4.0/MANIFEST.in
--rw-rw-rw-   0        0        0     2526 2023-11-30 04:35:25.039364 server-monitor-agent-0.4.0/PKG-INFO
--rw-rw-rw-   0        0        0      145 2023-11-20 03:36:36.000000 server-monitor-agent-0.4.0/README.md
--rw-rw-rw-   0        0        0        7 2023-11-30 04:35:11.000000 server-monitor-agent-0.4.0/VERSION
--rw-rw-rw-   0        0        0     2234 2023-11-30 04:07:01.000000 server-monitor-agent-0.4.0/pyproject.toml
--rw-rw-rw-   0        0        0      432 2023-11-30 03:42:54.000000 server-monitor-agent-0.4.0/requirements-dev.txt
--rw-rw-rw-   0        0        0      254 2023-11-30 04:28:32.000000 server-monitor-agent-0.4.0/requirements.txt
--rw-rw-rw-   0        0        0      592 2023-11-30 04:35:25.043445 server-monitor-agent-0.4.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-11-30 04:35:24.760593 server-monitor-agent-0.4.0/src/
-drwxrwxrwx   0        0        0        0 2023-11-30 04:35:24.803691 server-monitor-agent-0.4.0/src/server_monitor_agent/
--rw-rw-rw-   0        0        0        3 2023-11-30 02:42:34.000000 server-monitor-agent-0.4.0/src/server_monitor_agent/__init__.py
-drwxrwxrwx   0        0        0        0 2023-11-30 04:35:24.871693 server-monitor-agent-0.4.0/src/server_monitor_agent/agent/
--rw-rw-rw-   0        0        0        0 2023-11-20 03:29:37.000000 server-monitor-agent-0.4.0/src/server_monitor_agent/agent/__init__.py
--rw-rw-rw-   0        0        0     7601 2023-11-30 04:08:28.000000 server-monitor-agent-0.4.0/src/server_monitor_agent/agent/cli.py
--rw-rw-rw-   0        0        0     1862 2023-11-30 04:08:28.000000 server-monitor-agent-0.4.0/src/server_monitor_agent/agent/command.py
--rw-rw-rw-   0        0        0     4531 2023-11-30 04:29:47.000000 server-monitor-agent-0.4.0/src/server_monitor_agent/agent/common.py
--rw-rw-rw-   0        0        0     4189 2023-11-20 03:33:24.000000 server-monitor-agent-0.4.0/src/server_monitor_agent/agent/consul.py
--rw-rw-rw-   0        0        0     2520 2023-11-30 02:42:34.000000 server-monitor-agent-0.4.0/src/server_monitor_agent/agent/convert.py
--rw-rw-rw-   0        0        0     4364 2023-11-20 03:33:24.000000 server-monitor-agent-0.4.0/src/server_monitor_agent/agent/instance.py
--rw-rw-rw-   0        0        0     1323 2023-11-30 02:42:34.000000 server-monitor-agent-0.4.0/src/server_monitor_agent/agent/io.py
--rw-rw-rw-   0        0        0     9047 2023-11-30 02:42:34.000000 server-monitor-agent-0.4.0/src/server_monitor_agent/agent/model.py
--rw-rw-rw-   0        0        0     4818 2023-11-30 03:55:34.000000 server-monitor-agent-0.4.0/src/server_monitor_agent/agent/monitor.py
--rw-rw-rw-   0        0        0     3870 2023-11-30 04:29:47.000000 server-monitor-agent-0.4.0/src/server_monitor_agent/agent/operation.py
--rw-rw-rw-   0        0        0     5973 2023-11-30 04:29:47.000000 server-monitor-agent-0.4.0/src/server_monitor_agent/agent/registry.py
--rw-rw-rw-   0        0        0    15442 2023-11-30 04:15:04.000000 server-monitor-agent-0.4.0/src/server_monitor_agent/agent/service.py
--rw-rw-rw-   0        0        0      246 2023-11-20 03:33:24.000000 server-monitor-agent-0.4.0/src/server_monitor_agent/agent/slack.py
--rw-rw-rw-   0        0        0     1641 2023-11-20 03:35:09.000000 server-monitor-agent-0.4.0/src/server_monitor_agent/entry.py
-drwxrwxrwx   0        0        0        0 2023-11-30 04:35:24.873692 server-monitor-agent-0.4.0/src/server_monitor_agent/service/
--rw-rw-rw-   0        0        0       39 2023-11-30 02:42:34.000000 server-monitor-agent-0.4.0/src/server_monitor_agent/service/__init__.py
-drwxrwxrwx   0        0        0        0 2023-11-30 04:35:24.889240 server-monitor-agent-0.4.0/src/server_monitor_agent/service/alert_manager/
--rw-rw-rw-   0        0        0        0 2023-11-30 02:42:34.000000 server-monitor-agent-0.4.0/src/server_monitor_agent/service/alert_manager/__init__.py
--rw-rw-rw-   0        0        0      490 2023-11-30 03:07:57.000000 server-monitor-agent-0.4.0/src/server_monitor_agent/service/alert_manager/io.py
--rw-rw-rw-   0        0        0     2850 2023-11-30 02:42:34.000000 server-monitor-agent-0.4.0/src/server_monitor_agent/service/alert_manager/model.py
--rw-rw-rw-   0        0        0      454 2023-11-30 02:42:34.000000 server-monitor-agent-0.4.0/src/server_monitor_agent/service/alert_manager/operation.py
--rw-rw-rw-   0        0        0      805 2023-11-30 02:42:34.000000 server-monitor-agent-0.4.0/src/server_monitor_agent/service/alert_manager/send.py
-drwxrwxrwx   0        0        0        0 2023-11-30 04:35:24.904761 server-monitor-agent-0.4.0/src/server_monitor_agent/service/consul/
--rw-rw-rw-   0        0        0        0 2023-11-30 02:42:34.000000 server-monitor-agent-0.4.0/src/server_monitor_agent/service/consul/__init__.py
--rw-rw-rw-   0        0        0     2519 2023-11-30 02:42:34.000000 server-monitor-agent-0.4.0/src/server_monitor_agent/service/consul/collect.py
--rw-rw-rw-   0        0        0     1165 2023-11-30 02:42:34.000000 server-monitor-agent-0.4.0/src/server_monitor_agent/service/consul/io.py
--rw-rw-rw-   0        0        0    12695 2023-11-30 02:42:34.000000 server-monitor-agent-0.4.0/src/server_monitor_agent/service/consul/model.py
--rw-rw-rw-   0        0        0     1019 2023-11-30 02:42:34.000000 server-monitor-agent-0.4.0/src/server_monitor_agent/service/consul/operation.py
-drwxrwxrwx   0        0        0        0 2023-11-30 04:35:24.924344 server-monitor-agent-0.4.0/src/server_monitor_agent/service/disk/
--rw-rw-rw-   0        0        0        0 2023-11-30 02:42:34.000000 server-monitor-agent-0.4.0/src/server_monitor_agent/service/disk/__init__.py
--rw-rw-rw-   0        0        0     3594 2023-11-30 02:42:34.000000 server-monitor-agent-0.4.0/src/server_monitor_agent/service/disk/collect.py
--rw-rw-rw-   0        0        0     7328 2023-11-30 02:42:34.000000 server-monitor-agent-0.4.0/src/server_monitor_agent/service/disk/io.py
--rw-rw-rw-   0        0        0     2761 2023-11-30 02:42:34.000000 server-monitor-agent-0.4.0/src/server_monitor_agent/service/disk/model.py
--rw-rw-rw-   0        0        0     7030 2023-11-30 02:42:34.000000 server-monitor-agent-0.4.0/src/server_monitor_agent/service/disk/operation.py
--rw-rw-rw-   0        0        0     1139 2023-11-30 02:42:34.000000 server-monitor-agent-0.4.0/src/server_monitor_agent/service/disk/send.py
-drwxrwxrwx   0        0        0        0 2023-11-30 04:35:24.939360 server-monitor-agent-0.4.0/src/server_monitor_agent/service/docker/
--rw-rw-rw-   0        0        0        0 2023-11-30 02:42:34.000000 server-monitor-agent-0.4.0/src/server_monitor_agent/service/docker/__init__.py
--rw-rw-rw-   0        0        0     1274 2023-11-30 02:42:34.000000 server-monitor-agent-0.4.0/src/server_monitor_agent/service/docker/collect.py
--rw-rw-rw-   0        0        0     3678 2023-11-30 02:42:34.000000 server-monitor-agent-0.4.0/src/server_monitor_agent/service/docker/io.py
--rw-rw-rw-   0        0        0      522 2023-11-30 02:42:34.000000 server-monitor-agent-0.4.0/src/server_monitor_agent/service/docker/model.py
--rw-rw-rw-   0        0        0     1073 2023-11-30 02:42:34.000000 server-monitor-agent-0.4.0/src/server_monitor_agent/service/docker/operation.py
-drwxrwxrwx   0        0        0        0 2023-11-30 04:35:24.962446 server-monitor-agent-0.4.0/src/server_monitor_agent/service/server/
--rw-rw-rw-   0        0        0        0 2023-11-30 02:42:34.000000 server-monitor-agent-0.4.0/src/server_monitor_agent/service/server/__init__.py
--rw-rw-rw-   0        0        0     3002 2023-11-30 02:42:34.000000 server-monitor-agent-0.4.0/src/server_monitor_agent/service/server/collect.py
--rw-rw-rw-   0        0        0     4324 2023-11-30 02:42:34.000000 server-monitor-agent-0.4.0/src/server_monitor_agent/service/server/io.py
--rw-rw-rw-   0        0        0     2415 2023-11-30 02:42:34.000000 server-monitor-agent-0.4.0/src/server_monitor_agent/service/server/model.py
--rw-rw-rw-   0        0        0     7708 2023-11-30 02:42:34.000000 server-monitor-agent-0.4.0/src/server_monitor_agent/service/server/operation.py
--rw-rw-rw-   0        0        0     1777 2023-11-30 02:42:34.000000 server-monitor-agent-0.4.0/src/server_monitor_agent/service/server/send.py
-drwxrwxrwx   0        0        0        0 2023-11-30 04:35:24.982498 server-monitor-agent-0.4.0/src/server_monitor_agent/service/statuscake/
--rw-rw-rw-   0        0        0        0 2023-11-30 02:42:34.000000 server-monitor-agent-0.4.0/src/server_monitor_agent/service/statuscake/__init__.py
--rw-rw-rw-   0        0        0      928 2023-11-30 02:42:34.000000 server-monitor-agent-0.4.0/src/server_monitor_agent/service/statuscake/collect.py
--rw-rw-rw-   0        0        0     2113 2023-11-30 02:42:34.000000 server-monitor-agent-0.4.0/src/server_monitor_agent/service/statuscake/io.py
--rw-rw-rw-   0        0        0      341 2023-11-30 02:42:34.000000 server-monitor-agent-0.4.0/src/server_monitor_agent/service/statuscake/model.py
--rw-rw-rw-   0        0        0     2707 2023-11-30 02:42:34.000000 server-monitor-agent-0.4.0/src/server_monitor_agent/service/statuscake/operation.py
--rw-rw-rw-   0        0        0      674 2023-11-30 02:42:34.000000 server-monitor-agent-0.4.0/src/server_monitor_agent/service/statuscake/send.py
-drwxrwxrwx   0        0        0        0 2023-11-30 04:35:24.997538 server-monitor-agent-0.4.0/src/server_monitor_agent/service/systemd/
--rw-rw-rw-   0        0        0        0 2023-11-30 02:42:34.000000 server-monitor-agent-0.4.0/src/server_monitor_agent/service/systemd/__init__.py
--rw-rw-rw-   0        0        0     1848 2023-11-30 02:42:34.000000 server-monitor-agent-0.4.0/src/server_monitor_agent/service/systemd/collect.py
--rw-rw-rw-   0        0        0     3614 2023-11-30 02:42:34.000000 server-monitor-agent-0.4.0/src/server_monitor_agent/service/systemd/io.py
--rw-rw-rw-   0        0        0     2315 2023-11-30 02:42:34.000000 server-monitor-agent-0.4.0/src/server_monitor_agent/service/systemd/model.py
--rw-rw-rw-   0        0        0     2969 2023-11-30 02:42:34.000000 server-monitor-agent-0.4.0/src/server_monitor_agent/service/systemd/operation.py
-drwxrwxrwx   0        0        0        0 2023-11-30 04:35:25.018350 server-monitor-agent-0.4.0/src/server_monitor_agent/service/web/
--rw-rw-rw-   0        0        0        0 2023-11-30 02:42:34.000000 server-monitor-agent-0.4.0/src/server_monitor_agent/service/web/__init__.py
--rw-rw-rw-   0        0        0     2356 2023-11-30 02:42:34.000000 server-monitor-agent-0.4.0/src/server_monitor_agent/service/web/collect.py
--rw-rw-rw-   0        0        0     6280 2023-11-30 03:55:34.000000 server-monitor-agent-0.4.0/src/server_monitor_agent/service/web/io.py
--rw-rw-rw-   0        0        0     1434 2023-11-30 02:42:34.000000 server-monitor-agent-0.4.0/src/server_monitor_agent/service/web/model.py
--rw-rw-rw-   0        0        0     2603 2023-11-30 02:42:34.000000 server-monitor-agent-0.4.0/src/server_monitor_agent/service/web/operation.py
--rw-rw-rw-   0        0        0     2185 2023-11-30 02:42:34.000000 server-monitor-agent-0.4.0/src/server_monitor_agent/service/web/send.py
-drwxrwxrwx   0        0        0        0 2023-11-30 04:35:25.031359 server-monitor-agent-0.4.0/src/server_monitor_agent.egg-info/
--rw-rw-rw-   0        0        0     2526 2023-11-30 04:35:24.000000 server-monitor-agent-0.4.0/src/server_monitor_agent.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3372 2023-11-30 04:35:24.000000 server-monitor-agent-0.4.0/src/server_monitor_agent.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-11-30 04:35:24.000000 server-monitor-agent-0.4.0/src/server_monitor_agent.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       73 2023-11-30 04:35:24.000000 server-monitor-agent-0.4.0/src/server_monitor_agent.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      584 2023-11-30 04:35:24.000000 server-monitor-agent-0.4.0/src/server_monitor_agent.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2023-11-30 04:35:24.000000 server-monitor-agent-0.4.0/src/server_monitor_agent.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-11-30 04:35:25.026844 server-monitor-agent-0.4.0/tests/
--rw-rw-rw-   0        0        0     5670 2023-11-30 03:07:57.000000 server-monitor-agent-0.4.0/tests/test_agent.py
--rw-rw-rw-   0        0        0     8476 2023-11-30 04:35:11.000000 server-monitor-agent-0.4.0/tests/test_cli.py
--rw-rw-rw-   0        0        0    45321 2023-11-30 04:27:46.000000 server-monitor-agent-0.4.0/tests/test_todo.py
+drwxrwxrwx   0        0        0        0 2024-04-23 00:43:13.341616 server_monitor_agent-0.5.0/
+-rw-rw-rw-   0        0        0    11558 2023-11-20 03:29:37.000000 server_monitor_agent-0.5.0/LICENSE
+-rw-rw-rw-   0        0        0       73 2023-11-20 03:29:37.000000 server_monitor_agent-0.5.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     2526 2024-04-23 00:43:13.340613 server_monitor_agent-0.5.0/PKG-INFO
+-rw-rw-rw-   0        0        0      145 2023-11-20 03:36:36.000000 server_monitor_agent-0.5.0/README.md
+-rw-rw-rw-   0        0        0        7 2024-04-23 00:39:00.000000 server_monitor_agent-0.5.0/VERSION
+-rw-rw-rw-   0        0        0     2234 2023-11-30 04:39:39.000000 server_monitor_agent-0.5.0/pyproject.toml
+-rw-rw-rw-   0        0        0      432 2023-11-30 04:39:39.000000 server_monitor_agent-0.5.0/requirements-dev.txt
+-rw-rw-rw-   0        0        0      242 2024-04-23 00:34:40.000000 server_monitor_agent-0.5.0/requirements.txt
+-rw-rw-rw-   0        0        0      592 2024-04-23 00:43:13.343617 server_monitor_agent-0.5.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-23 00:43:13.081877 server_monitor_agent-0.5.0/src/
+drwxrwxrwx   0        0        0        0 2024-04-23 00:43:13.114631 server_monitor_agent-0.5.0/src/server_monitor_agent/
+-rw-rw-rw-   0        0        0        3 2023-11-30 02:42:34.000000 server_monitor_agent-0.5.0/src/server_monitor_agent/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-23 00:43:13.178011 server_monitor_agent-0.5.0/src/server_monitor_agent/agent/
+-rw-rw-rw-   0        0        0        0 2023-11-20 03:29:37.000000 server_monitor_agent-0.5.0/src/server_monitor_agent/agent/__init__.py
+-rw-rw-rw-   0        0        0     7601 2023-11-30 04:39:39.000000 server_monitor_agent-0.5.0/src/server_monitor_agent/agent/cli.py
+-rw-rw-rw-   0        0        0     1862 2023-11-30 04:39:39.000000 server_monitor_agent-0.5.0/src/server_monitor_agent/agent/command.py
+-rw-rw-rw-   0        0        0     4531 2023-11-30 04:39:39.000000 server_monitor_agent-0.5.0/src/server_monitor_agent/agent/common.py
+-rw-rw-rw-   0        0        0     4776 2024-04-23 00:38:26.000000 server_monitor_agent-0.5.0/src/server_monitor_agent/agent/consul.py
+-rw-rw-rw-   0        0        0     2520 2023-11-30 02:42:34.000000 server_monitor_agent-0.5.0/src/server_monitor_agent/agent/convert.py
+-rw-rw-rw-   0        0        0     4364 2023-11-20 03:33:24.000000 server_monitor_agent-0.5.0/src/server_monitor_agent/agent/instance.py
+-rw-rw-rw-   0        0        0     1323 2023-11-30 02:42:34.000000 server_monitor_agent-0.5.0/src/server_monitor_agent/agent/io.py
+-rw-rw-rw-   0        0        0     9047 2023-11-30 02:42:34.000000 server_monitor_agent-0.5.0/src/server_monitor_agent/agent/model.py
+-rw-rw-rw-   0        0        0     4818 2023-11-30 04:39:39.000000 server_monitor_agent-0.5.0/src/server_monitor_agent/agent/monitor.py
+-rw-rw-rw-   0        0        0     3870 2023-11-30 04:39:39.000000 server_monitor_agent-0.5.0/src/server_monitor_agent/agent/operation.py
+-rw-rw-rw-   0        0        0     5973 2023-11-30 04:39:39.000000 server_monitor_agent-0.5.0/src/server_monitor_agent/agent/registry.py
+-rw-rw-rw-   0        0        0    15442 2023-11-30 04:39:39.000000 server_monitor_agent-0.5.0/src/server_monitor_agent/agent/service.py
+-rw-rw-rw-   0        0        0      246 2023-11-20 03:33:24.000000 server_monitor_agent-0.5.0/src/server_monitor_agent/agent/slack.py
+-rw-rw-rw-   0        0        0     1641 2023-11-20 03:35:09.000000 server_monitor_agent-0.5.0/src/server_monitor_agent/entry.py
+drwxrwxrwx   0        0        0        0 2024-04-23 00:43:13.181022 server_monitor_agent-0.5.0/src/server_monitor_agent/service/
+-rw-rw-rw-   0        0        0       39 2023-11-30 02:42:34.000000 server_monitor_agent-0.5.0/src/server_monitor_agent/service/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-23 00:43:13.197068 server_monitor_agent-0.5.0/src/server_monitor_agent/service/alert_manager/
+-rw-rw-rw-   0        0        0        0 2023-11-30 02:42:34.000000 server_monitor_agent-0.5.0/src/server_monitor_agent/service/alert_manager/__init__.py
+-rw-rw-rw-   0        0        0      490 2023-11-30 03:07:57.000000 server_monitor_agent-0.5.0/src/server_monitor_agent/service/alert_manager/io.py
+-rw-rw-rw-   0        0        0     2850 2023-11-30 02:42:34.000000 server_monitor_agent-0.5.0/src/server_monitor_agent/service/alert_manager/model.py
+-rw-rw-rw-   0        0        0      454 2023-11-30 02:42:34.000000 server_monitor_agent-0.5.0/src/server_monitor_agent/service/alert_manager/operation.py
+-rw-rw-rw-   0        0        0      805 2023-11-30 02:42:34.000000 server_monitor_agent-0.5.0/src/server_monitor_agent/service/alert_manager/send.py
+drwxrwxrwx   0        0        0        0 2024-04-23 00:43:13.218255 server_monitor_agent-0.5.0/src/server_monitor_agent/service/consul/
+-rw-rw-rw-   0        0        0        0 2023-11-30 02:42:34.000000 server_monitor_agent-0.5.0/src/server_monitor_agent/service/consul/__init__.py
+-rw-rw-rw-   0        0        0     2519 2023-11-30 02:42:34.000000 server_monitor_agent-0.5.0/src/server_monitor_agent/service/consul/collect.py
+-rw-rw-rw-   0        0        0     1165 2023-11-30 02:42:34.000000 server_monitor_agent-0.5.0/src/server_monitor_agent/service/consul/io.py
+-rw-rw-rw-   0        0        0    12695 2023-11-30 02:42:34.000000 server_monitor_agent-0.5.0/src/server_monitor_agent/service/consul/model.py
+-rw-rw-rw-   0        0        0     1019 2023-11-30 02:42:34.000000 server_monitor_agent-0.5.0/src/server_monitor_agent/service/consul/operation.py
+drwxrwxrwx   0        0        0        0 2024-04-23 00:43:13.240823 server_monitor_agent-0.5.0/src/server_monitor_agent/service/disk/
+-rw-rw-rw-   0        0        0        0 2023-11-30 02:42:34.000000 server_monitor_agent-0.5.0/src/server_monitor_agent/service/disk/__init__.py
+-rw-rw-rw-   0        0        0     3594 2023-11-30 02:42:34.000000 server_monitor_agent-0.5.0/src/server_monitor_agent/service/disk/collect.py
+-rw-rw-rw-   0        0        0     7328 2023-11-30 02:42:34.000000 server_monitor_agent-0.5.0/src/server_monitor_agent/service/disk/io.py
+-rw-rw-rw-   0        0        0     2761 2023-11-30 02:42:34.000000 server_monitor_agent-0.5.0/src/server_monitor_agent/service/disk/model.py
+-rw-rw-rw-   0        0        0     7030 2023-11-30 02:42:34.000000 server_monitor_agent-0.5.0/src/server_monitor_agent/service/disk/operation.py
+-rw-rw-rw-   0        0        0     1139 2023-11-30 02:42:34.000000 server_monitor_agent-0.5.0/src/server_monitor_agent/service/disk/send.py
+drwxrwxrwx   0        0        0        0 2024-04-23 00:43:13.255937 server_monitor_agent-0.5.0/src/server_monitor_agent/service/docker/
+-rw-rw-rw-   0        0        0        0 2023-11-30 02:42:34.000000 server_monitor_agent-0.5.0/src/server_monitor_agent/service/docker/__init__.py
+-rw-rw-rw-   0        0        0     1274 2023-11-30 02:42:34.000000 server_monitor_agent-0.5.0/src/server_monitor_agent/service/docker/collect.py
+-rw-rw-rw-   0        0        0     3678 2023-11-30 02:42:34.000000 server_monitor_agent-0.5.0/src/server_monitor_agent/service/docker/io.py
+-rw-rw-rw-   0        0        0      522 2023-11-30 02:42:34.000000 server_monitor_agent-0.5.0/src/server_monitor_agent/service/docker/model.py
+-rw-rw-rw-   0        0        0     1073 2023-11-30 02:42:34.000000 server_monitor_agent-0.5.0/src/server_monitor_agent/service/docker/operation.py
+drwxrwxrwx   0        0        0        0 2024-04-23 00:43:13.272948 server_monitor_agent-0.5.0/src/server_monitor_agent/service/server/
+-rw-rw-rw-   0        0        0        0 2023-11-30 02:42:34.000000 server_monitor_agent-0.5.0/src/server_monitor_agent/service/server/__init__.py
+-rw-rw-rw-   0        0        0     3002 2023-11-30 02:42:34.000000 server_monitor_agent-0.5.0/src/server_monitor_agent/service/server/collect.py
+-rw-rw-rw-   0        0        0     4324 2023-11-30 02:42:34.000000 server_monitor_agent-0.5.0/src/server_monitor_agent/service/server/io.py
+-rw-rw-rw-   0        0        0     3340 2024-04-23 00:38:26.000000 server_monitor_agent-0.5.0/src/server_monitor_agent/service/server/model.py
+-rw-rw-rw-   0        0        0     8689 2024-04-23 00:38:26.000000 server_monitor_agent-0.5.0/src/server_monitor_agent/service/server/operation.py
+-rw-rw-rw-   0        0        0     1777 2023-11-30 02:42:34.000000 server_monitor_agent-0.5.0/src/server_monitor_agent/service/server/send.py
+drwxrwxrwx   0        0        0        0 2024-04-23 00:43:13.290993 server_monitor_agent-0.5.0/src/server_monitor_agent/service/statuscake/
+-rw-rw-rw-   0        0        0        0 2023-11-30 02:42:34.000000 server_monitor_agent-0.5.0/src/server_monitor_agent/service/statuscake/__init__.py
+-rw-rw-rw-   0        0        0      928 2023-11-30 02:42:34.000000 server_monitor_agent-0.5.0/src/server_monitor_agent/service/statuscake/collect.py
+-rw-rw-rw-   0        0        0     2113 2023-11-30 02:42:34.000000 server_monitor_agent-0.5.0/src/server_monitor_agent/service/statuscake/io.py
+-rw-rw-rw-   0        0        0      341 2023-11-30 02:42:34.000000 server_monitor_agent-0.5.0/src/server_monitor_agent/service/statuscake/model.py
+-rw-rw-rw-   0        0        0     2707 2023-11-30 02:42:34.000000 server_monitor_agent-0.5.0/src/server_monitor_agent/service/statuscake/operation.py
+-rw-rw-rw-   0        0        0      674 2023-11-30 02:42:34.000000 server_monitor_agent-0.5.0/src/server_monitor_agent/service/statuscake/send.py
+drwxrwxrwx   0        0        0        0 2024-04-23 00:43:13.304514 server_monitor_agent-0.5.0/src/server_monitor_agent/service/systemd/
+-rw-rw-rw-   0        0        0        0 2023-11-30 02:42:34.000000 server_monitor_agent-0.5.0/src/server_monitor_agent/service/systemd/__init__.py
+-rw-rw-rw-   0        0        0     1848 2023-11-30 02:42:34.000000 server_monitor_agent-0.5.0/src/server_monitor_agent/service/systemd/collect.py
+-rw-rw-rw-   0        0        0     3614 2023-11-30 02:42:34.000000 server_monitor_agent-0.5.0/src/server_monitor_agent/service/systemd/io.py
+-rw-rw-rw-   0        0        0     2315 2023-11-30 02:42:34.000000 server_monitor_agent-0.5.0/src/server_monitor_agent/service/systemd/model.py
+-rw-rw-rw-   0        0        0     2969 2023-11-30 02:42:34.000000 server_monitor_agent-0.5.0/src/server_monitor_agent/service/systemd/operation.py
+drwxrwxrwx   0        0        0        0 2024-04-23 00:43:13.322575 server_monitor_agent-0.5.0/src/server_monitor_agent/service/web/
+-rw-rw-rw-   0        0        0        0 2023-11-30 02:42:34.000000 server_monitor_agent-0.5.0/src/server_monitor_agent/service/web/__init__.py
+-rw-rw-rw-   0        0        0     2356 2023-11-30 02:42:34.000000 server_monitor_agent-0.5.0/src/server_monitor_agent/service/web/collect.py
+-rw-rw-rw-   0        0        0     6280 2023-11-30 04:39:39.000000 server_monitor_agent-0.5.0/src/server_monitor_agent/service/web/io.py
+-rw-rw-rw-   0        0        0     1434 2023-11-30 02:42:34.000000 server_monitor_agent-0.5.0/src/server_monitor_agent/service/web/model.py
+-rw-rw-rw-   0        0        0     2603 2023-11-30 02:42:34.000000 server_monitor_agent-0.5.0/src/server_monitor_agent/service/web/operation.py
+-rw-rw-rw-   0        0        0     2185 2023-11-30 02:42:34.000000 server_monitor_agent-0.5.0/src/server_monitor_agent/service/web/send.py
+drwxrwxrwx   0        0        0        0 2024-04-23 00:43:13.335102 server_monitor_agent-0.5.0/src/server_monitor_agent.egg-info/
+-rw-rw-rw-   0        0        0     2526 2024-04-23 00:43:13.000000 server_monitor_agent-0.5.0/src/server_monitor_agent.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3372 2024-04-23 00:43:13.000000 server_monitor_agent-0.5.0/src/server_monitor_agent.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-23 00:43:13.000000 server_monitor_agent-0.5.0/src/server_monitor_agent.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       73 2024-04-23 00:43:13.000000 server_monitor_agent-0.5.0/src/server_monitor_agent.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      584 2024-04-23 00:43:13.000000 server_monitor_agent-0.5.0/src/server_monitor_agent.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2024-04-23 00:43:13.000000 server_monitor_agent-0.5.0/src/server_monitor_agent.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-23 00:43:13.330100 server_monitor_agent-0.5.0/tests/
+-rw-rw-rw-   0        0        0     5670 2023-11-30 03:07:57.000000 server_monitor_agent-0.5.0/tests/test_agent.py
+-rw-rw-rw-   0        0        0     8741 2024-04-23 00:39:00.000000 server_monitor_agent-0.5.0/tests/test_cli.py
+-rw-rw-rw-   0        0        0    45321 2023-11-30 04:39:39.000000 server_monitor_agent-0.5.0/tests/test_todo.py
```

### Comparing `server-monitor-agent-0.4.0/LICENSE` & `server_monitor_agent-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `server-monitor-agent-0.4.0/PKG-INFO` & `server_monitor_agent-0.5.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 Metadata-Version: 2.1
 Name: server-monitor-agent
-Version: 0.4.0
+Version: 0.5.0
 Summary: Utility to run checks on a server and send notifications.
 Project-URL: Homepage, https://github.com/qcif/server-monitor-agent
 Project-URL: Bug Tracker, https://github.com/qcif/server-monitor-agent/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: System Administrators
 Classifier: Topic :: System :: Monitoring
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests==2.31.0
-Requires-Dist: psutil==5.9.6
+Requires-Dist: psutil==5.9.8
 Requires-Dist: dateparser==1.2.0
 Requires-Dist: humanize==4.9.0
-Requires-Dist: tzdata==2023.3
+Requires-Dist: tzdata==2024.1
 Requires-Dist: colorama==0.4.6
 Requires-Dist: PyYAML==6.0.1
-Requires-Dist: boltons==23.1.1
+Requires-Dist: boltons==24.0.0
 Requires-Dist: click==8.1.7
-Requires-Dist: beartype==0.16.4
+Requires-Dist: beartype==0.18.5
 Requires-Dist: importlib-resources
 Requires-Dist: importlib-metadata
 Requires-Dist: backports.zoneinfo[tzdata]; python_version < "3.9"
 Provides-Extra: dev
 Requires-Dist: pip; extra == "dev"
 Requires-Dist: setuptools; extra == "dev"
 Requires-Dist: wheel; extra == "dev"
```

### Comparing `server-monitor-agent-0.4.0/pyproject.toml` & `server_monitor_agent-0.5.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `server-monitor-agent-0.4.0/setup.cfg` & `server_monitor_agent-0.5.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `server-monitor-agent-0.4.0/src/server_monitor_agent/agent/cli.py` & `server_monitor_agent-0.5.0/src/server_monitor_agent/agent/cli.py`

 * *Files identical despite different names*

### Comparing `server-monitor-agent-0.4.0/src/server_monitor_agent/agent/command.py` & `server_monitor_agent-0.5.0/src/server_monitor_agent/agent/command.py`

 * *Files identical despite different names*

### Comparing `server-monitor-agent-0.4.0/src/server_monitor_agent/agent/common.py` & `server_monitor_agent-0.5.0/src/server_monitor_agent/agent/common.py`

 * *Files identical despite different names*

### Comparing `server-monitor-agent-0.4.0/src/server_monitor_agent/agent/convert.py` & `server_monitor_agent-0.5.0/src/server_monitor_agent/agent/convert.py`

 * *Files identical despite different names*

### Comparing `server-monitor-agent-0.4.0/src/server_monitor_agent/agent/instance.py` & `server_monitor_agent-0.5.0/src/server_monitor_agent/agent/instance.py`

 * *Files identical despite different names*

### Comparing `server-monitor-agent-0.4.0/src/server_monitor_agent/agent/io.py` & `server_monitor_agent-0.5.0/src/server_monitor_agent/agent/io.py`

 * *Files identical despite different names*

### Comparing `server-monitor-agent-0.4.0/src/server_monitor_agent/agent/model.py` & `server_monitor_agent-0.5.0/src/server_monitor_agent/agent/model.py`

 * *Files identical despite different names*

### Comparing `server-monitor-agent-0.4.0/src/server_monitor_agent/agent/monitor.py` & `server_monitor_agent-0.5.0/src/server_monitor_agent/agent/monitor.py`

 * *Files identical despite different names*

### Comparing `server-monitor-agent-0.4.0/src/server_monitor_agent/agent/operation.py` & `server_monitor_agent-0.5.0/src/server_monitor_agent/agent/operation.py`

 * *Files identical despite different names*

### Comparing `server-monitor-agent-0.4.0/src/server_monitor_agent/agent/registry.py` & `server_monitor_agent-0.5.0/src/server_monitor_agent/agent/registry.py`

 * *Files identical despite different names*

### Comparing `server-monitor-agent-0.4.0/src/server_monitor_agent/agent/service.py` & `server_monitor_agent-0.5.0/src/server_monitor_agent/agent/service.py`

 * *Files identical despite different names*

### Comparing `server-monitor-agent-0.4.0/src/server_monitor_agent/entry.py` & `server_monitor_agent-0.5.0/src/server_monitor_agent/entry.py`

 * *Files identical despite different names*

### Comparing `server-monitor-agent-0.4.0/src/server_monitor_agent/service/alert_manager/model.py` & `server_monitor_agent-0.5.0/src/server_monitor_agent/service/alert_manager/model.py`

 * *Files identical despite different names*

### Comparing `server-monitor-agent-0.4.0/src/server_monitor_agent/service/alert_manager/send.py` & `server_monitor_agent-0.5.0/src/server_monitor_agent/service/alert_manager/send.py`

 * *Files identical despite different names*

### Comparing `server-monitor-agent-0.4.0/src/server_monitor_agent/service/consul/collect.py` & `server_monitor_agent-0.5.0/src/server_monitor_agent/service/consul/collect.py`

 * *Files identical despite different names*

### Comparing `server-monitor-agent-0.4.0/src/server_monitor_agent/service/consul/io.py` & `server_monitor_agent-0.5.0/src/server_monitor_agent/service/consul/io.py`

 * *Files identical despite different names*

### Comparing `server-monitor-agent-0.4.0/src/server_monitor_agent/service/consul/model.py` & `server_monitor_agent-0.5.0/src/server_monitor_agent/service/consul/model.py`

 * *Files identical despite different names*

### Comparing `server-monitor-agent-0.4.0/src/server_monitor_agent/service/consul/operation.py` & `server_monitor_agent-0.5.0/src/server_monitor_agent/service/consul/operation.py`

 * *Files identical despite different names*

### Comparing `server-monitor-agent-0.4.0/src/server_monitor_agent/service/disk/collect.py` & `server_monitor_agent-0.5.0/src/server_monitor_agent/service/disk/collect.py`

 * *Files identical despite different names*

### Comparing `server-monitor-agent-0.4.0/src/server_monitor_agent/service/disk/io.py` & `server_monitor_agent-0.5.0/src/server_monitor_agent/service/disk/io.py`

 * *Files identical despite different names*

### Comparing `server-monitor-agent-0.4.0/src/server_monitor_agent/service/disk/model.py` & `server_monitor_agent-0.5.0/src/server_monitor_agent/service/disk/model.py`

 * *Files identical despite different names*

### Comparing `server-monitor-agent-0.4.0/src/server_monitor_agent/service/disk/operation.py` & `server_monitor_agent-0.5.0/src/server_monitor_agent/service/disk/operation.py`

 * *Files identical despite different names*

### Comparing `server-monitor-agent-0.4.0/src/server_monitor_agent/service/disk/send.py` & `server_monitor_agent-0.5.0/src/server_monitor_agent/service/disk/send.py`

 * *Files identical despite different names*

### Comparing `server-monitor-agent-0.4.0/src/server_monitor_agent/service/docker/collect.py` & `server_monitor_agent-0.5.0/src/server_monitor_agent/service/docker/collect.py`

 * *Files identical despite different names*

### Comparing `server-monitor-agent-0.4.0/src/server_monitor_agent/service/docker/io.py` & `server_monitor_agent-0.5.0/src/server_monitor_agent/service/docker/io.py`

 * *Files identical despite different names*

### Comparing `server-monitor-agent-0.4.0/src/server_monitor_agent/service/docker/model.py` & `server_monitor_agent-0.5.0/src/server_monitor_agent/service/docker/model.py`

 * *Files identical despite different names*

### Comparing `server-monitor-agent-0.4.0/src/server_monitor_agent/service/docker/operation.py` & `server_monitor_agent-0.5.0/src/server_monitor_agent/service/docker/operation.py`

 * *Files identical despite different names*

### Comparing `server-monitor-agent-0.4.0/src/server_monitor_agent/service/server/collect.py` & `server_monitor_agent-0.5.0/src/server_monitor_agent/service/server/collect.py`

 * *Files identical despite different names*

### Comparing `server-monitor-agent-0.4.0/src/server_monitor_agent/service/server/io.py` & `server_monitor_agent-0.5.0/src/server_monitor_agent/service/server/io.py`

 * *Files identical despite different names*

### Comparing `server-monitor-agent-0.4.0/src/server_monitor_agent/service/server/operation.py` & `server_monitor_agent-0.5.0/src/server_monitor_agent/service/server/operation.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,269 +1,298 @@
-"""Operations on a server instance."""
-
-import datetime
-import logging
-import platform
-import socket
-import sys
-
-import beartype
-import psutil
-from beartype import typing
-
-from server_monitor_agent.agent import model as agent_model, operation as agent_op
-from server_monitor_agent.service.server import model as server_model
-
-logger = logging.getLogger(f"{agent_model.APP_NAME_UNDER}.device.instance")
-
-
-@beartype.beartype
-def network() -> typing.List[server_model.NetworkResult]:
-    """Get the network information."""
-
-    output = []
-    result = psutil.net_io_counters(pernic=True)
-
-    agent_op.log_msg(
-        logging.DEBUG, f"Result from psutil.net_io_counters with pernic: {result}"
-    )
-
-    for name, info in result.items():
-        output.append(
-            server_model.NetworkResult(
-                name=name,
-                exit_code=0,
-                bytes_recv=info.bytes_recv,
-                bytes_sent=info.bytes_sent,
-                dropin=info.dropin,
-                dropout=info.dropout,
-                errin=info.errin,
-                errout=info.errout,
-                packets_recv=info.packets_recv,
-                packets_sent=info.packets_sent,
-            )
-        )
-    return output
-
-
-@beartype.beartype
-def memory() -> server_model.MemoryResult:
-    """Get the memory information."""
-
-    result = psutil.virtual_memory()
-
-    agent_op.log_msg(logging.DEBUG, f"Result from psutil.virtual_memory: {result}")
-
-    return server_model.MemoryResult(
-        exit_code=0,
-        total=result.total,
-        available=result.available,
-        percent=result.percent,
-        used=result.used,
-        free=result.free,
-        active=getattr(result, "active", 0),
-        inactive=getattr(result, "inactive", 0),
-        buffers=getattr(result, "buffers", 0),
-        cached=getattr(result, "cached", 0),
-        wired=getattr(result, "wired", 0),
-        shared=getattr(result, "shared", 0),
-    )
-
-
-@beartype.beartype
-def hostname() -> str:
-    """Get the local hostname."""
-
-    output = None
-
-    if not output:
-        output = socket.getfqdn()
-
-        agent_op.log_msg(logging.DEBUG, f"Result from socket.getfqdn: {output}")
-
-    if not output:
-        output = platform.node()
-
-        agent_op.log_msg(logging.DEBUG, f"Result from platform.node: {output}")
-
-    if output:
-        return output
-
-    raise ValueError("Could not get hostname.")
-
-
-@beartype.beartype
-def timezone() -> server_model.TimeZoneResult:
-    """Get the configured local time zone."""
-
-    args = ["timedatectl", "show"]
-    result = agent_op.execute_process(args)
-
-    agent_op.log_msg(logging.DEBUG, f"Result from '{' '.join(args)}': {result}")
-
-    if result.returncode != 0:
-        return server_model.TimeZoneResult(exit_code=result.returncode, raw=None)
-
-    items = dict([i.split("=", maxsplit=1) for i in result.stdout.splitlines()])
-
-    output = items.get("Timezone")
-    return server_model.TimeZoneResult(exit_code=result.returncode, raw=output)
-
-
-@beartype.beartype
-def uptime() -> int:
-    """Get the time since the local machine booted."""
-
-    output_now = datetime.datetime.now().timestamp()
-    output_boot = psutil.boot_time()
-    output = int(output_now - output_boot)
-
-    agent_op.log_msg(
-        logging.DEBUG,
-        f"Result from datetime.now '{output_now}' "
-        f"psutil.boot_time '{output_boot}' "
-        f"uptime '{output}'",
-    )
-
-    return output
-
-
-@beartype.beartype
-def cpu_usage(interval: float = 2.0) -> float:
-    """Get the cpu usage."""
-
-    output = psutil.cpu_percent(interval=interval)
-
-    agent_op.log_msg(
-        logging.DEBUG,
-        f"Result from psutil.cpu_percent with interval {interval}: {output}",
-    )
-
-    return float(output)
-
-
-@beartype.beartype
-def processes() -> typing.List[server_model.ProcessResult]:
-    """Get a list of the local processes."""
-
-    result = []
-    attrs = {
-        "pid": "PID",
-        "memory_percent": "%MEM",
-        "name": "COMMAND",
-        "cmdline": "COMMAND",
-        "cpu_percent": "%CPU",
-        "memory_info": ["VSZ", "RSS"],
-        "username": "USER",
-    }
-    count = 0
-    for p in psutil.process_iter(attrs=list(attrs.keys()), ad_value=None):
-        count += 1
-        info = p.info if hasattr(p, "info") else p
-
-        user = info.get("username") or "(unknown)"
-        if user and psutil.WINDOWS and "\\" in user:
-            user = user.split("\\")[1]
-        user = user[:9]
-        pid = info.get("pid")
-        vms = info.get("memory_info").vms if info.get("memory_info") else 0
-        rss = info.get("memory_info").rss if info.get("memory_info") else 0
-
-        mem_raw = info.get("memory_percent")
-        mem_p = round(mem_raw, 1) if mem_raw is not None else None
-
-        cpu_raw = info.get("cpu_percent")
-        cpu_p = round(cpu_raw, 1) if cpu_raw is not None else None
-
-        if info.get("cmdline"):
-            cmdline = " ".join(info["cmdline"])
-        else:
-            cmdline = info.get("name")
-
-        result.append(
-            server_model.ProcessResult(
-                exit_code=0,
-                user=user,
-                pid=pid,
-                cpu_percent=cpu_p,
-                mem_percent=mem_p,
-                vms=vms,
-                rss=rss,
-                cmdline=cmdline,
-            )
-        )
-
-    agent_op.log_msg(
-        logging.DEBUG, f"Result from psutil.process_iter: {count} processes"
-    )
-
-    return result
-
-
-@beartype.beartype
-def user_message(
-    item: agent_model.AgentItem, user_group: typing.Optional[str] = None
-) -> None:
-    """Submit a message to display to all users logged in to the local machine."""
-    users = f"users in group {user_group}" if user_group else "all users"
-
-    summary = item.summary
-    description = item.description
-    host_name = item.host_name
-    source_name = item.source_name
-    check_name = item.check_name
-    date = item.date
-    status_name = item.status_name
-    service_name = item.service_name
-    extra_data = item.extra_data
-
-    date_format = "%a, %d %b %Y %H:%M:%S %Z"
-    message = "\n".join(
-        [
-            f"On {date.strftime(date_format)}, {service_name} (from {source_name}, host {host_name}):",
-            "",
-            summary,
-            description,
-            "",
-            f"Sent to {users}",
-            "",
-            f"Status: {status_name}",
-            f"Check: {check_name}",
-            f"Tags:",
-            *[f"{k}={v}" for k, v in extra_data.items()],
-        ]
-    )
-
-    if not message or not message.strip():
-        raise ValueError("Must provide a message to send.")
-
-    cmd = ["wall", "--timeout", "30"]
-
-    if user_group and user_group.strip():
-        cmd.extend(["--group", user_group.strip()])
-
-    cmd.append(message)
-
-    result = agent_op.execute_process(cmd)
-
-    if result.returncode != 0:
-        raise ValueError(f"Could not send local system message due to :{result}")
-
-
-@beartype.beartype
-def write_stream(out_target: str, content: str) -> None:
-    if out_target == agent_model.STREAM_STDOUT:
-        sys.stdout.write(content)
-
-    elif out_target == agent_model.STREAM_STDERR:
-        sys.stderr.write(content)
-
-    else:
-        agent_op.raise_options("stream target", out_target, agent_model.STREAM_TARGETS)
-
-
-@beartype.beartype
-def read_stream(in_source: str) -> str:
-    if in_source == agent_model.STREAM_STDIN:
-        return sys.stdin.read()
-
-    agent_op.raise_options("stream source", in_source, agent_model.STREAM_SOURCES)
+"""Operations on a server instance."""
+
+import datetime
+import logging
+import platform
+import socket
+import sys
+
+import beartype
+import psutil
+from beartype import typing
+
+from server_monitor_agent.agent import model as agent_model, operation as agent_op
+from server_monitor_agent.service.server import model as server_model
+
+logger = logging.getLogger(f"{agent_model.APP_NAME_UNDER}.device.instance")
+
+
+@beartype.beartype
+def network() -> typing.List[server_model.NetworkResult]:
+    """Get the network information."""
+
+    output = []
+    result = psutil.net_io_counters(pernic=True)
+
+    agent_op.log_msg(
+        logging.DEBUG, f"Result from psutil.net_io_counters with pernic: {result}"
+    )
+
+    for name, info in result.items():
+        output.append(
+            server_model.NetworkResult(
+                name=name,
+                exit_code=0,
+                bytes_recv=info.bytes_recv,
+                bytes_sent=info.bytes_sent,
+                dropin=info.dropin,
+                dropout=info.dropout,
+                errin=info.errin,
+                errout=info.errout,
+                packets_recv=info.packets_recv,
+                packets_sent=info.packets_sent,
+            )
+        )
+    return output
+
+
+@beartype.beartype
+def memory() -> server_model.MemoryResult:
+    """Get the memory information."""
+
+    result = psutil.virtual_memory()
+
+    agent_op.log_msg(logging.DEBUG, f"Result from psutil.virtual_memory: {result}")
+
+    return server_model.MemoryResult(
+        exit_code=0,
+        total=result.total,
+        available=result.available,
+        percent=result.percent,
+        used=result.used,
+        free=result.free,
+        active=getattr(result, "active", 0),
+        inactive=getattr(result, "inactive", 0),
+        buffers=getattr(result, "buffers", 0),
+        cached=getattr(result, "cached", 0),
+        wired=getattr(result, "wired", 0),
+        shared=getattr(result, "shared", 0),
+    )
+
+
+@beartype.beartype
+def hostname() -> str:
+    """Get the local hostname."""
+
+    output = None
+
+    if not output:
+        output = socket.getfqdn()
+
+        agent_op.log_msg(logging.DEBUG, f"Result from socket.getfqdn: {output}")
+
+    if not output:
+        output = platform.node()
+
+        agent_op.log_msg(logging.DEBUG, f"Result from platform.node: {output}")
+
+    if output:
+        return output
+
+    raise ValueError("Could not get hostname.")
+
+
+@beartype.beartype
+def timezone() -> server_model.TimeZoneResult:
+    """Get the configured local time zone."""
+
+    args = ["timedatectl", "show"]
+    result = agent_op.execute_process(args)
+
+    agent_op.log_msg(logging.DEBUG, f"Result from '{' '.join(args)}': {result}")
+
+    if result.returncode != 0:
+        return server_model.TimeZoneResult(exit_code=result.returncode, raw=None)
+
+    items = dict([i.split("=", maxsplit=1) for i in result.stdout.splitlines()])
+
+    output = items.get("Timezone")
+    return server_model.TimeZoneResult(exit_code=result.returncode, raw=output)
+
+
+@beartype.beartype
+def uptime() -> int:
+    """Get the time since the local machine booted."""
+
+    output_now = datetime.datetime.now().timestamp()
+    output_boot = psutil.boot_time()
+    output = int(output_now - output_boot)
+
+    agent_op.log_msg(
+        logging.DEBUG,
+        f"Result from datetime.now '{output_now}' "
+        f"psutil.boot_time '{output_boot}' "
+        f"uptime '{output}'",
+    )
+
+    return output
+
+
+@beartype.beartype
+def cpu_usage(interval: float = 2.0) -> float:
+    """Get the cpu usage."""
+
+    output = psutil.cpu_percent(interval=interval)
+
+    agent_op.log_msg(
+        logging.DEBUG,
+        f"Result from psutil.cpu_percent with interval {interval}: {output}",
+    )
+
+    return float(output)
+
+
+@beartype.beartype
+def processes() -> typing.List[server_model.ProcessResult]:
+    """Get a list of the local processes."""
+
+    # Note: Linux doesn't seem to expose easily usable per-process network stats.
+    #       Maybe `sudo lsof -niTCP` combined with `iftop`?
+    #       See https://github.com/giampaolo/psutil/issues/1900
+
+    result = []
+    attrs = {
+        "pid": "PID",
+        "memory_percent": "%MEM",
+        "name": "COMMAND",
+        "cmdline": "COMMAND",
+        "cpu_percent": "%CPU",
+        "memory_info": ["VSZ", "RSS"],
+        "username": "USER",
+        "io_counters": "",
+        "cpu_times": "",
+    }
+    count = 0
+    for p in psutil.process_iter(attrs=list(attrs.keys()), ad_value=None):
+        count += 1
+        info = p.info if hasattr(p, "info") else p
+
+        user = info.get("username") or "(unknown)"
+        if user and psutil.WINDOWS and "\\" in user:
+            user = user.split("\\")[1]
+        user = user[:9]
+        pid = info.get("pid")
+        vms = info.get("memory_info").vms if info.get("memory_info") else 0
+        rss = info.get("memory_info").rss if info.get("memory_info") else 0
+
+        # ignore a process that is using no memory
+        if (vms + rss) < 1:
+            continue
+
+        # note that memory percent can be 0 if there is no previous information
+        mem_raw = info.get("memory_percent")
+        mem_p = round(mem_raw, 1) if mem_raw is not None else None
+
+        # note that cpu percent can be 0 if there is no previous information
+        cpu_raw = info.get("cpu_percent")
+        cpu_p = round(cpu_raw, 1) if cpu_raw is not None else None
+
+        if info.get("cmdline"):
+            cmdline = " ".join(info["cmdline"])
+        else:
+            cmdline = info.get("name")
+
+        io_counters = info.get("io_counters")
+        io_read_ops_count = io_counters.read_count
+        io_write_ops_count = io_counters.write_count
+        io_read_bytes_count = io_counters.read_bytes
+        io_write_bytes_count = io_counters.write_bytes
+
+        cpu_times = info.get("cpu_times")
+        cpu_time_count = cpu_times.user + cpu_times.system
+
+        cpu_usable_count = len(p.cpu_affinity())
+
+        result.append(
+            server_model.ProcessResult(
+                exit_code=0,
+                user=user,
+                pid=pid,
+                cpu_percent=cpu_p,
+                mem_percent=mem_p,
+                vms=vms,
+                rss=rss,
+                cmdline=cmdline,
+                io_read_ops_count=io_read_ops_count,
+                io_write_ops_count=io_write_ops_count,
+                io_read_bytes_count=io_read_bytes_count,
+                io_write_bytes_count=io_write_bytes_count,
+                cpu_time_count=cpu_time_count,
+                cpu_usable_count=cpu_usable_count,
+            )
+        )
+
+    agent_op.log_msg(
+        logging.DEBUG, f"Result from psutil.process_iter: {count} processes"
+    )
+
+    return result
+
+
+@beartype.beartype
+def user_message(
+    item: agent_model.AgentItem, user_group: typing.Optional[str] = None
+) -> None:
+    """Submit a message to display to all users logged in to the local machine."""
+    users = f"users in group {user_group}" if user_group else "all users"
+
+    summary = item.summary
+    description = item.description
+    host_name = item.host_name
+    source_name = item.source_name
+    check_name = item.check_name
+    date = item.date
+    status_name = item.status_name
+    service_name = item.service_name
+    extra_data = item.extra_data
+
+    date_format = "%a, %d %b %Y %H:%M:%S %Z"
+    message = "\n".join(
+        [
+            f"On {date.strftime(date_format)}, {service_name} (from {source_name}, host {host_name}):",
+            "",
+            summary,
+            description,
+            "",
+            f"Sent to {users}",
+            "",
+            f"Status: {status_name}",
+            f"Check: {check_name}",
+            f"Tags:",
+            *[f"{k}={v}" for k, v in extra_data.items()],
+        ]
+    )
+
+    if not message or not message.strip():
+        raise ValueError("Must provide a message to send.")
+
+    cmd = ["wall", "--timeout", "30"]
+
+    if user_group and user_group.strip():
+        cmd.extend(["--group", user_group.strip()])
+
+    cmd.append(message)
+
+    result = agent_op.execute_process(cmd)
+
+    if result.returncode != 0:
+        raise ValueError(f"Could not send local system message due to :{result}")
+
+
+@beartype.beartype
+def write_stream(out_target: str, content: str) -> None:
+    if out_target == agent_model.STREAM_STDOUT:
+        sys.stdout.write(content)
+
+    elif out_target == agent_model.STREAM_STDERR:
+        sys.stderr.write(content)
+
+    else:
+        agent_op.raise_options("stream target", out_target, agent_model.STREAM_TARGETS)
+
+
+@beartype.beartype
+def read_stream(in_source: str) -> str:
+    if in_source == agent_model.STREAM_STDIN:
+        return sys.stdin.read()
+
+    agent_op.raise_options("stream source", in_source, agent_model.STREAM_SOURCES)
```

### Comparing `server-monitor-agent-0.4.0/src/server_monitor_agent/service/server/send.py` & `server_monitor_agent-0.5.0/src/server_monitor_agent/service/server/send.py`

 * *Files identical despite different names*

### Comparing `server-monitor-agent-0.4.0/src/server_monitor_agent/service/statuscake/collect.py` & `server_monitor_agent-0.5.0/src/server_monitor_agent/service/statuscake/collect.py`

 * *Files identical despite different names*

### Comparing `server-monitor-agent-0.4.0/src/server_monitor_agent/service/statuscake/io.py` & `server_monitor_agent-0.5.0/src/server_monitor_agent/service/statuscake/io.py`

 * *Files identical despite different names*

### Comparing `server-monitor-agent-0.4.0/src/server_monitor_agent/service/statuscake/operation.py` & `server_monitor_agent-0.5.0/src/server_monitor_agent/service/statuscake/operation.py`

 * *Files identical despite different names*

### Comparing `server-monitor-agent-0.4.0/src/server_monitor_agent/service/statuscake/send.py` & `server_monitor_agent-0.5.0/src/server_monitor_agent/service/statuscake/send.py`

 * *Files identical despite different names*

### Comparing `server-monitor-agent-0.4.0/src/server_monitor_agent/service/systemd/collect.py` & `server_monitor_agent-0.5.0/src/server_monitor_agent/service/systemd/collect.py`

 * *Files identical despite different names*

### Comparing `server-monitor-agent-0.4.0/src/server_monitor_agent/service/systemd/io.py` & `server_monitor_agent-0.5.0/src/server_monitor_agent/service/systemd/io.py`

 * *Files identical despite different names*

### Comparing `server-monitor-agent-0.4.0/src/server_monitor_agent/service/systemd/model.py` & `server_monitor_agent-0.5.0/src/server_monitor_agent/service/systemd/model.py`

 * *Files identical despite different names*

### Comparing `server-monitor-agent-0.4.0/src/server_monitor_agent/service/systemd/operation.py` & `server_monitor_agent-0.5.0/src/server_monitor_agent/service/systemd/operation.py`

 * *Files identical despite different names*

### Comparing `server-monitor-agent-0.4.0/src/server_monitor_agent/service/web/collect.py` & `server_monitor_agent-0.5.0/src/server_monitor_agent/service/web/collect.py`

 * *Files identical despite different names*

### Comparing `server-monitor-agent-0.4.0/src/server_monitor_agent/service/web/io.py` & `server_monitor_agent-0.5.0/src/server_monitor_agent/service/web/io.py`

 * *Files identical despite different names*

### Comparing `server-monitor-agent-0.4.0/src/server_monitor_agent/service/web/model.py` & `server_monitor_agent-0.5.0/src/server_monitor_agent/service/web/model.py`

 * *Files identical despite different names*

### Comparing `server-monitor-agent-0.4.0/src/server_monitor_agent/service/web/operation.py` & `server_monitor_agent-0.5.0/src/server_monitor_agent/service/web/operation.py`

 * *Files identical despite different names*

### Comparing `server-monitor-agent-0.4.0/src/server_monitor_agent/service/web/send.py` & `server_monitor_agent-0.5.0/src/server_monitor_agent/service/web/send.py`

 * *Files identical despite different names*

### Comparing `server-monitor-agent-0.4.0/src/server_monitor_agent.egg-info/PKG-INFO` & `server_monitor_agent-0.5.0/src/server_monitor_agent.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 Metadata-Version: 2.1
 Name: server-monitor-agent
-Version: 0.4.0
+Version: 0.5.0
 Summary: Utility to run checks on a server and send notifications.
 Project-URL: Homepage, https://github.com/qcif/server-monitor-agent
 Project-URL: Bug Tracker, https://github.com/qcif/server-monitor-agent/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: System Administrators
 Classifier: Topic :: System :: Monitoring
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests==2.31.0
-Requires-Dist: psutil==5.9.6
+Requires-Dist: psutil==5.9.8
 Requires-Dist: dateparser==1.2.0
 Requires-Dist: humanize==4.9.0
-Requires-Dist: tzdata==2023.3
+Requires-Dist: tzdata==2024.1
 Requires-Dist: colorama==0.4.6
 Requires-Dist: PyYAML==6.0.1
-Requires-Dist: boltons==23.1.1
+Requires-Dist: boltons==24.0.0
 Requires-Dist: click==8.1.7
-Requires-Dist: beartype==0.16.4
+Requires-Dist: beartype==0.18.5
 Requires-Dist: importlib-resources
 Requires-Dist: importlib-metadata
 Requires-Dist: backports.zoneinfo[tzdata]; python_version < "3.9"
 Provides-Extra: dev
 Requires-Dist: pip; extra == "dev"
 Requires-Dist: setuptools; extra == "dev"
 Requires-Dist: wheel; extra == "dev"
```

### Comparing `server-monitor-agent-0.4.0/src/server_monitor_agent.egg-info/SOURCES.txt` & `server_monitor_agent-0.5.0/src/server_monitor_agent.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `server-monitor-agent-0.4.0/src/server_monitor_agent.egg-info/requires.txt` & `server_monitor_agent-0.5.0/src/server_monitor_agent.egg-info/requires.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 requests==2.31.0
-psutil==5.9.6
+psutil==5.9.8
 dateparser==1.2.0
 humanize==4.9.0
-tzdata==2023.3
+tzdata==2024.1
 colorama==0.4.6
 PyYAML==6.0.1
-boltons==23.1.1
+boltons==24.0.0
 click==8.1.7
-beartype==0.16.4
+beartype==0.18.5
 importlib-resources
 importlib-metadata
 
 [:python_version < "3.9"]
 backports.zoneinfo[tzdata]
 
 [dev]
```

### Comparing `server-monitor-agent-0.4.0/tests/test_agent.py` & `server_monitor_agent-0.5.0/tests/test_agent.py`

 * *Files identical despite different names*

### Comparing `server-monitor-agent-0.4.0/tests/test_todo.py` & `server_monitor_agent-0.5.0/tests/test_todo.py`

 * *Files identical despite different names*

