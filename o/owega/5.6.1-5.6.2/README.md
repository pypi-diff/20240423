# Comparing `tmp/owega-5.6.1.tar.gz` & `tmp/owega-5.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "owega-5.6.1.tar", last modified: Thu Apr 18 20:51:53 2024, max compression
+gzip compressed data, was "owega-5.6.2.tar", last modified: Tue Apr 23 20:55:18 2024, max compression
```

## Comparing `owega-5.6.1.tar` & `owega-5.6.2.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxr-xr-x   0 darkgeem  (1000) darkgeem  (1000)        0 2024-04-18 20:51:53.018164 owega-5.6.1/
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      496 2024-04-17 02:21:38.000000 owega-5.6.1/LICENSE
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)    15726 2024-04-18 20:51:53.018164 owega-5.6.1/PKG-INFO
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     5023 2024-04-17 02:21:38.000000 owega-5.6.1/README.md
-drwxr-xr-x   0 darkgeem  (1000) darkgeem  (1000)        0 2024-04-18 20:51:53.012164 owega-5.6.1/owega/
-drwxr-xr-x   0 darkgeem  (1000) darkgeem  (1000)        0 2024-04-18 20:51:53.015164 owega-5.6.1/owega/OweHandlers/
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      156 2024-04-17 02:21:38.000000 owega-5.6.1/owega/OweHandlers/__init__.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      874 2024-04-17 02:21:38.000000 owega-5.6.1/owega/OweHandlers/handle_add_sysmem.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1430 2024-04-17 02:21:38.000000 owega-5.6.1/owega/OweHandlers/handle_commands.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1076 2024-04-17 02:21:38.000000 owega-5.6.1/owega/OweHandlers/handle_context.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1515 2024-04-18 20:42:21.000000 owega-5.6.1/owega/OweHandlers/handle_del_sysmem.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1695 2024-04-17 02:21:38.000000 owega-5.6.1/owega/OweHandlers/handle_dinput.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     3372 2024-04-17 02:21:38.000000 owega-5.6.1/owega/OweHandlers/handle_edit.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1175 2024-04-17 02:21:38.000000 owega-5.6.1/owega/OweHandlers/handle_estimation.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     4778 2024-04-17 02:21:38.000000 owega-5.6.1/owega/OweHandlers/handle_finput.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1692 2024-04-17 02:21:38.000000 owega-5.6.1/owega/OweHandlers/handle_frequency.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      418 2024-04-17 02:21:38.000000 owega-5.6.1/owega/OweHandlers/handle_genconf.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      422 2024-04-17 02:21:38.000000 owega-5.6.1/owega/OweHandlers/handle_history.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     3056 2024-04-17 02:21:38.000000 owega-5.6.1/owega/OweHandlers/handle_image.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      993 2024-04-17 02:21:38.000000 owega-5.6.1/owega/OweHandlers/handle_load.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1568 2024-04-17 02:21:38.000000 owega-5.6.1/owega/OweHandlers/handle_model.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1670 2024-04-17 02:21:38.000000 owega-5.6.1/owega/OweHandlers/handle_presence.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      552 2024-04-17 02:21:38.000000 owega-5.6.1/owega/OweHandlers/handle_quit.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      967 2024-04-17 02:21:38.000000 owega-5.6.1/owega/OweHandlers/handle_save.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      846 2024-04-17 02:21:38.000000 owega-5.6.1/owega/OweHandlers/handle_system.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1617 2024-04-17 02:21:38.000000 owega-5.6.1/owega/OweHandlers/handle_temperature.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1277 2024-04-17 02:21:38.000000 owega-5.6.1/owega/OweHandlers/handle_tokens.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1446 2024-04-17 02:21:38.000000 owega-5.6.1/owega/OweHandlers/handle_top_p.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1105 2024-04-17 02:21:38.000000 owega-5.6.1/owega/OweHandlers/handle_tts.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     2407 2024-04-17 02:21:38.000000 owega-5.6.1/owega/OweHandlers/handlers.py
-drwxr-xr-x   0 darkgeem  (1000) darkgeem  (1000)        0 2024-04-18 20:51:53.015164 owega-5.6.1/owega/OwegaFun/
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      873 2024-04-17 02:21:38.000000 owega-5.6.1/owega/OwegaFun/__init__.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     3867 2024-04-17 02:21:38.000000 owega-5.6.1/owega/OwegaFun/functions.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     4341 2024-04-18 20:40:40.000000 owega-5.6.1/owega/OwegaFun/longTermSouvenirs.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     5813 2024-04-18 20:41:08.000000 owega-5.6.1/owega/OwegaFun/utility.py
-drwxr-xr-x   0 darkgeem  (1000) darkgeem  (1000)        0 2024-04-18 20:51:53.016164 owega-5.6.1/owega/OwegaSession/
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      100 2024-04-17 02:21:38.000000 owega-5.6.1/owega/OwegaSession/__init__.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     2762 2024-04-17 02:21:38.000000 owega-5.6.1/owega/OwegaSession/main_bottom_toolbar.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     5590 2024-04-17 02:21:38.000000 owega-5.6.1/owega/OwegaSession/promptsession.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)       62 2024-04-17 02:21:38.000000 owega-5.6.1/owega/__init__.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)       94 2024-04-17 02:21:38.000000 owega-5.6.1/owega/__main__.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     9249 2024-04-18 20:30:35.000000 owega-5.6.1/owega/ask.py
-drwxr-xr-x   0 darkgeem  (1000) darkgeem  (1000)        0 2024-04-18 20:51:53.017164 owega-5.6.1/owega/changelog/
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)       80 2024-04-17 02:21:38.000000 owega-5.6.1/owega/changelog/__init__.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)    23524 2024-04-18 20:51:22.000000 owega-5.6.1/owega/changelog/changelog.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1533 2024-04-17 02:21:38.000000 owega-5.6.1/owega/changelog/changelogEntry.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     3315 2024-04-17 02:21:38.000000 owega-5.6.1/owega/changelog/version.py
-drwxr-xr-x   0 darkgeem  (1000) darkgeem  (1000)        0 2024-04-18 20:51:53.017164 owega-5.6.1/owega/config/
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)       86 2024-04-17 02:21:38.000000 owega-5.6.1/owega/config/__init__.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1808 2024-04-17 02:21:38.000000 owega-5.6.1/owega/config/baseConf.py
-drwxr-xr-x   0 darkgeem  (1000) darkgeem  (1000)        0 2024-04-18 20:51:53.017164 owega-5.6.1/owega/conversation/
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)       83 2024-04-17 02:21:38.000000 owega-5.6.1/owega/conversation/__init__.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)    10102 2024-04-18 20:35:07.000000 owega-5.6.1/owega/conversation/conversation.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1417 2024-04-18 20:49:15.000000 owega-5.6.1/owega/getLogger.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)       64 2024-04-17 02:21:38.000000 owega-5.6.1/owega/handlerBase.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      549 2024-04-17 02:21:38.000000 owega-5.6.1/owega/license.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)    11666 2024-04-17 02:21:38.000000 owega-5.6.1/owega/owega.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     6026 2024-04-18 20:46:49.000000 owega-5.6.1/owega/utils.py
-drwxr-xr-x   0 darkgeem  (1000) darkgeem  (1000)        0 2024-04-18 20:51:53.017164 owega-5.6.1/owega.egg-info/
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)    15726 2024-04-18 20:51:52.000000 owega-5.6.1/owega.egg-info/PKG-INFO
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1656 2024-04-18 20:51:52.000000 owega-5.6.1/owega.egg-info/SOURCES.txt
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)        1 2024-04-18 20:51:52.000000 owega-5.6.1/owega.egg-info/dependency_links.txt
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)       43 2024-04-18 20:51:52.000000 owega-5.6.1/owega.egg-info/entry_points.txt
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      156 2024-04-18 20:51:52.000000 owega-5.6.1/owega.egg-info/requires.txt
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)        6 2024-04-18 20:51:52.000000 owega-5.6.1/owega.egg-info/top_level.txt
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)       90 2024-04-17 02:21:38.000000 owega-5.6.1/pyproject.toml
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)       38 2024-04-18 20:51:53.018164 owega-5.6.1/setup.cfg
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     2082 2024-04-17 02:21:38.000000 owega-5.6.1/setup.py
+drwxr-xr-x   0 darkgeem  (1000) darkgeem  (1000)        0 2024-04-23 20:55:18.699515 owega-5.6.2/
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      496 2024-04-17 02:21:38.000000 owega-5.6.2/LICENSE
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)    15764 2024-04-23 20:55:18.699515 owega-5.6.2/PKG-INFO
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     5023 2024-04-17 02:21:38.000000 owega-5.6.2/README.md
+drwxr-xr-x   0 darkgeem  (1000) darkgeem  (1000)        0 2024-04-23 20:55:18.697515 owega-5.6.2/owega/
+drwxr-xr-x   0 darkgeem  (1000) darkgeem  (1000)        0 2024-04-23 20:55:18.698515 owega-5.6.2/owega/OweHandlers/
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      156 2024-04-17 02:21:38.000000 owega-5.6.2/owega/OweHandlers/__init__.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      874 2024-04-17 02:21:38.000000 owega-5.6.2/owega/OweHandlers/handle_add_sysmem.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1430 2024-04-17 02:21:38.000000 owega-5.6.2/owega/OweHandlers/handle_commands.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1076 2024-04-17 02:21:38.000000 owega-5.6.2/owega/OweHandlers/handle_context.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1515 2024-04-18 20:54:01.000000 owega-5.6.2/owega/OweHandlers/handle_del_sysmem.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1695 2024-04-17 02:21:38.000000 owega-5.6.2/owega/OweHandlers/handle_dinput.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     3372 2024-04-17 02:21:38.000000 owega-5.6.2/owega/OweHandlers/handle_edit.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1175 2024-04-17 02:21:38.000000 owega-5.6.2/owega/OweHandlers/handle_estimation.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     4778 2024-04-17 02:21:38.000000 owega-5.6.2/owega/OweHandlers/handle_finput.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1692 2024-04-17 02:21:38.000000 owega-5.6.2/owega/OweHandlers/handle_frequency.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      418 2024-04-17 02:21:38.000000 owega-5.6.2/owega/OweHandlers/handle_genconf.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      422 2024-04-17 02:21:38.000000 owega-5.6.2/owega/OweHandlers/handle_history.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     3056 2024-04-17 02:21:38.000000 owega-5.6.2/owega/OweHandlers/handle_image.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      993 2024-04-17 02:21:38.000000 owega-5.6.2/owega/OweHandlers/handle_load.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1568 2024-04-17 02:21:38.000000 owega-5.6.2/owega/OweHandlers/handle_model.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1670 2024-04-17 02:21:38.000000 owega-5.6.2/owega/OweHandlers/handle_presence.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      552 2024-04-17 02:21:38.000000 owega-5.6.2/owega/OweHandlers/handle_quit.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      967 2024-04-17 02:21:38.000000 owega-5.6.2/owega/OweHandlers/handle_save.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      846 2024-04-17 02:21:38.000000 owega-5.6.2/owega/OweHandlers/handle_system.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1617 2024-04-17 02:21:38.000000 owega-5.6.2/owega/OweHandlers/handle_temperature.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1277 2024-04-17 02:21:38.000000 owega-5.6.2/owega/OweHandlers/handle_tokens.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1446 2024-04-17 02:21:38.000000 owega-5.6.2/owega/OweHandlers/handle_top_p.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1105 2024-04-17 02:21:38.000000 owega-5.6.2/owega/OweHandlers/handle_tts.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     2407 2024-04-17 02:21:38.000000 owega-5.6.2/owega/OweHandlers/handlers.py
+drwxr-xr-x   0 darkgeem  (1000) darkgeem  (1000)        0 2024-04-23 20:55:18.698515 owega-5.6.2/owega/OwegaFun/
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      873 2024-04-17 02:21:38.000000 owega-5.6.2/owega/OwegaFun/__init__.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     3867 2024-04-17 02:21:38.000000 owega-5.6.2/owega/OwegaFun/functions.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     4341 2024-04-18 20:54:01.000000 owega-5.6.2/owega/OwegaFun/longTermSouvenirs.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     5813 2024-04-18 20:54:01.000000 owega-5.6.2/owega/OwegaFun/utility.py
+drwxr-xr-x   0 darkgeem  (1000) darkgeem  (1000)        0 2024-04-23 20:55:18.699515 owega-5.6.2/owega/OwegaSession/
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      100 2024-04-17 02:21:38.000000 owega-5.6.2/owega/OwegaSession/__init__.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     2762 2024-04-17 02:21:38.000000 owega-5.6.2/owega/OwegaSession/main_bottom_toolbar.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     5590 2024-04-17 02:21:38.000000 owega-5.6.2/owega/OwegaSession/promptsession.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)       62 2024-04-17 02:21:38.000000 owega-5.6.2/owega/__init__.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)       94 2024-04-17 02:21:38.000000 owega-5.6.2/owega/__main__.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     9249 2024-04-18 20:54:01.000000 owega-5.6.2/owega/ask.py
+drwxr-xr-x   0 darkgeem  (1000) darkgeem  (1000)        0 2024-04-23 20:55:18.699515 owega-5.6.2/owega/changelog/
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)       80 2024-04-17 02:21:38.000000 owega-5.6.2/owega/changelog/__init__.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)    23651 2024-04-23 20:40:46.000000 owega-5.6.2/owega/changelog/changelog.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1533 2024-04-17 02:21:38.000000 owega-5.6.2/owega/changelog/changelogEntry.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     3315 2024-04-17 02:21:38.000000 owega-5.6.2/owega/changelog/version.py
+drwxr-xr-x   0 darkgeem  (1000) darkgeem  (1000)        0 2024-04-23 20:55:18.699515 owega-5.6.2/owega/config/
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)       86 2024-04-17 02:21:38.000000 owega-5.6.2/owega/config/__init__.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1808 2024-04-17 02:21:38.000000 owega-5.6.2/owega/config/baseConf.py
+drwxr-xr-x   0 darkgeem  (1000) darkgeem  (1000)        0 2024-04-23 20:55:18.699515 owega-5.6.2/owega/conversation/
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)       83 2024-04-17 02:21:38.000000 owega-5.6.2/owega/conversation/__init__.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)    10102 2024-04-18 20:54:01.000000 owega-5.6.2/owega/conversation/conversation.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1417 2024-04-18 20:54:01.000000 owega-5.6.2/owega/getLogger.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)       64 2024-04-17 02:21:38.000000 owega-5.6.2/owega/handlerBase.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      549 2024-04-17 02:21:38.000000 owega-5.6.2/owega/license.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)    12104 2024-04-23 20:51:39.000000 owega-5.6.2/owega/owega.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     6107 2024-04-23 20:31:42.000000 owega-5.6.2/owega/utils.py
+drwxr-xr-x   0 darkgeem  (1000) darkgeem  (1000)        0 2024-04-23 20:55:18.699515 owega-5.6.2/owega.egg-info/
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)    15764 2024-04-23 20:55:18.000000 owega-5.6.2/owega.egg-info/PKG-INFO
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1656 2024-04-23 20:55:18.000000 owega-5.6.2/owega.egg-info/SOURCES.txt
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)        1 2024-04-23 20:55:18.000000 owega-5.6.2/owega.egg-info/dependency_links.txt
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)       43 2024-04-23 20:55:18.000000 owega-5.6.2/owega.egg-info/entry_points.txt
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      156 2024-04-23 20:55:18.000000 owega-5.6.2/owega.egg-info/requires.txt
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)        6 2024-04-23 20:55:18.000000 owega-5.6.2/owega.egg-info/top_level.txt
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)       90 2024-04-17 02:21:38.000000 owega-5.6.2/pyproject.toml
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)       38 2024-04-23 20:55:18.699515 owega-5.6.2/setup.cfg
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     2082 2024-04-17 02:21:38.000000 owega-5.6.2/setup.py
```

### Comparing `owega-5.6.1/PKG-INFO` & `owega-5.6.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: owega
-Version: 5.6.1
+Version: 5.6.2
 Summary: A command-line interface for conversing with GPT models (from OpenAI)
 Home-page: https://git.pyrokinesis.fr/darkgeem/owega
 Author: darkgeem
 Author-email: darkgeem@pyrokinesis.fr
 License: WTFPL
 Project-URL: Source, https://git.pyrokinesis.fr/darkgeem/owega
 Project-URL: Support, https://discord.gg/KdRmyRrA48
@@ -135,15 +135,15 @@
 See ΦωΦ in action!
 
 [![asciicast](https://asciinema.org/a/613143.png)](https://asciinema.org/a/613143)
 
 
 ## CHANGELOG: 
 ```
-OWEGA v5.6.1 CHANGELOG:
+OWEGA v5.6.2 CHANGELOG:
 
 
 2.0.0: WTFPL license
 2.0.1: added genconf command
 
 2.1.0: added file_input command
 2.1.1: added file_input in help command
@@ -356,8 +356,9 @@
 5.5.5: Now using openai module to ask mistral API.
        (the code is waaaay cleaner)
 
 5.6.0: Added basic support for Chub's API 
        (chub mars, mercury, mixtral)
        Also, Mi(s/x)tral support is no more in beta :D
 5.6.1: Added extensive logging for errors.
+5.6.2: Added terminal title status :3
 ```
```

### Comparing `owega-5.6.1/README.md` & `owega-5.6.2/README.md`

 * *Files identical despite different names*

### Comparing `owega-5.6.1/owega/OweHandlers/handle_add_sysmem.py` & `owega-5.6.2/owega/OweHandlers/handle_add_sysmem.py`

 * *Files identical despite different names*

### Comparing `owega-5.6.1/owega/OweHandlers/handle_commands.py` & `owega-5.6.2/owega/OweHandlers/handle_commands.py`

 * *Files identical despite different names*

### Comparing `owega-5.6.1/owega/OweHandlers/handle_context.py` & `owega-5.6.2/owega/OweHandlers/handle_context.py`

 * *Files identical despite different names*

### Comparing `owega-5.6.1/owega/OweHandlers/handle_del_sysmem.py` & `owega-5.6.2/owega/OweHandlers/handle_del_sysmem.py`

 * *Files identical despite different names*

### Comparing `owega-5.6.1/owega/OweHandlers/handle_dinput.py` & `owega-5.6.2/owega/OweHandlers/handle_dinput.py`

 * *Files identical despite different names*

### Comparing `owega-5.6.1/owega/OweHandlers/handle_edit.py` & `owega-5.6.2/owega/OweHandlers/handle_edit.py`

 * *Files identical despite different names*

### Comparing `owega-5.6.1/owega/OweHandlers/handle_estimation.py` & `owega-5.6.2/owega/OweHandlers/handle_estimation.py`

 * *Files identical despite different names*

### Comparing `owega-5.6.1/owega/OweHandlers/handle_finput.py` & `owega-5.6.2/owega/OweHandlers/handle_finput.py`

 * *Files identical despite different names*

### Comparing `owega-5.6.1/owega/OweHandlers/handle_frequency.py` & `owega-5.6.2/owega/OweHandlers/handle_frequency.py`

 * *Files identical despite different names*

### Comparing `owega-5.6.1/owega/OweHandlers/handle_image.py` & `owega-5.6.2/owega/OweHandlers/handle_image.py`

 * *Files identical despite different names*

### Comparing `owega-5.6.1/owega/OweHandlers/handle_load.py` & `owega-5.6.2/owega/OweHandlers/handle_load.py`

 * *Files identical despite different names*

### Comparing `owega-5.6.1/owega/OweHandlers/handle_model.py` & `owega-5.6.2/owega/OweHandlers/handle_model.py`

 * *Files identical despite different names*

### Comparing `owega-5.6.1/owega/OweHandlers/handle_presence.py` & `owega-5.6.2/owega/OweHandlers/handle_presence.py`

 * *Files identical despite different names*

### Comparing `owega-5.6.1/owega/OweHandlers/handle_quit.py` & `owega-5.6.2/owega/OweHandlers/handle_quit.py`

 * *Files identical despite different names*

### Comparing `owega-5.6.1/owega/OweHandlers/handle_save.py` & `owega-5.6.2/owega/OweHandlers/handle_save.py`

 * *Files identical despite different names*

### Comparing `owega-5.6.1/owega/OweHandlers/handle_system.py` & `owega-5.6.2/owega/OweHandlers/handle_system.py`

 * *Files identical despite different names*

### Comparing `owega-5.6.1/owega/OweHandlers/handle_temperature.py` & `owega-5.6.2/owega/OweHandlers/handle_temperature.py`

 * *Files identical despite different names*

### Comparing `owega-5.6.1/owega/OweHandlers/handle_tokens.py` & `owega-5.6.2/owega/OweHandlers/handle_tokens.py`

 * *Files identical despite different names*

### Comparing `owega-5.6.1/owega/OweHandlers/handle_top_p.py` & `owega-5.6.2/owega/OweHandlers/handle_top_p.py`

 * *Files identical despite different names*

### Comparing `owega-5.6.1/owega/OweHandlers/handle_tts.py` & `owega-5.6.2/owega/OweHandlers/handle_tts.py`

 * *Files identical despite different names*

### Comparing `owega-5.6.1/owega/OweHandlers/handlers.py` & `owega-5.6.2/owega/OweHandlers/handlers.py`

 * *Files identical despite different names*

### Comparing `owega-5.6.1/owega/OwegaFun/__init__.py` & `owega-5.6.2/owega/OwegaFun/__init__.py`

 * *Files identical despite different names*

### Comparing `owega-5.6.1/owega/OwegaFun/functions.py` & `owega-5.6.2/owega/OwegaFun/functions.py`

 * *Files identical despite different names*

### Comparing `owega-5.6.1/owega/OwegaFun/longTermSouvenirs.py` & `owega-5.6.2/owega/OwegaFun/longTermSouvenirs.py`

 * *Files identical despite different names*

### Comparing `owega-5.6.1/owega/OwegaFun/utility.py` & `owega-5.6.2/owega/OwegaFun/utility.py`

 * *Files identical despite different names*

### Comparing `owega-5.6.1/owega/OwegaSession/main_bottom_toolbar.py` & `owega-5.6.2/owega/OwegaSession/main_bottom_toolbar.py`

 * *Files identical despite different names*

### Comparing `owega-5.6.1/owega/OwegaSession/promptsession.py` & `owega-5.6.2/owega/OwegaSession/promptsession.py`

 * *Files identical despite different names*

### Comparing `owega-5.6.1/owega/ask.py` & `owega-5.6.2/owega/ask.py`

 * *Files identical despite different names*

### Comparing `owega-5.6.1/owega/changelog/changelog.py` & `owega-5.6.2/owega/changelog/changelog.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,14 +13,18 @@
         self.version = Version(0, 0, 0)
         self.initLogs()
         self.genLog()
 
     def initLogs(self):
         """Fill the changelog."""
         self.logs.append(
+            ChangelogEntry(5, 6, 2)
+            .addLine("Added terminal title status :3")
+        )
+        self.logs.append(
             ChangelogEntry(5, 6, 1)
             .addLine("Added extensive logging for errors.")
         )
         self.logs.append(
             ChangelogEntry(5, 6, 0)
             .addLine("Added basic support for Chub's API ")
             .addLine("(chub mars, mercury, mixtral)")
```

### Comparing `owega-5.6.1/owega/changelog/changelogEntry.py` & `owega-5.6.2/owega/changelog/changelogEntry.py`

 * *Files identical despite different names*

### Comparing `owega-5.6.1/owega/changelog/version.py` & `owega-5.6.2/owega/changelog/version.py`

 * *Files identical despite different names*

### Comparing `owega-5.6.1/owega/config/baseConf.py` & `owega-5.6.2/owega/config/baseConf.py`

 * *Files identical despite different names*

### Comparing `owega-5.6.1/owega/conversation/conversation.py` & `owega-5.6.2/owega/conversation/conversation.py`

 * *Files identical despite different names*

### Comparing `owega-5.6.1/owega/getLogger.py` & `owega-5.6.2/owega/getLogger.py`

 * *Files identical despite different names*

### Comparing `owega-5.6.1/owega/license.py` & `owega-5.6.2/owega/license.py`

 * *Files identical despite different names*

### Comparing `owega-5.6.1/owega/owega.py` & `owega-5.6.2/owega/owega.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,14 +22,15 @@
     info_print,
     do_quit,
     success_msg,
     clrtxt,
     print_help,
     estimated_tokens,
     play_tts,
+    set_term_title,
 )
 from .conversation import Conversation, Conversation_from
 from .ask import ask
 from .OwegaSession import OwegaSession as ps
 
 
 def get_oc_conf():
@@ -82,14 +83,23 @@
         openai.organization = baseConf.get("organization", "")
 
     # main interaction loop:
     while True:
         # save temp file
         messages.save(temp_file)
 
+        new_title = "Owega"
+        new_title += f" v{OwegaChangelog.version}"
+        new_title += f" - {baseConf.get('model', '?')}"
+        new_title += f" - {baseConf.get('temperature', '?')}"
+        new_title += f"/{baseConf.get('top_p', '?')}"
+        new_title += f"/{baseConf.get('frequency_penalty', '?')}"
+        new_title += f"/{baseConf.get('presence_penalty', '?')}"
+        set_term_title(new_title)
+
         # get user input, and strip it (no excess spaces / tabs / newlines
         user_input = ps['main'].prompt(pt.ANSI(input_prompt)).strip()
 
         command_found = False
         if user_input.startswith('/'):
             uinp_spl = user_input.split(' ')
             given = ' '.join(uinp_spl[1:])
@@ -279,14 +289,15 @@
     temp_file = get_temp_file()
     temp_is_temp = True
     if (args.output):
         temp_is_temp = False
         temp_file = args.output
 
     get_conf(args.config_file)
+
     if baseConf.get("commands", False):
         existingFunctions.enableGroup("utility.system")
     else:
         existingFunctions.disableGroup("utility.system")
 
     if (args.debug):  # bypass after loading conf
         baseConf["debug"] = True
```

### Comparing `owega-5.6.1/owega/utils.py` & `owega-5.6.2/owega/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,18 @@
 from .config import baseConf
 os.environ['PYGAME_HIDE_SUPPORT_PROMPT'] = '1'
 warnings.filterwarnings("ignore", category=RuntimeWarning, message=".*pygame.*")
 import pygame  # noqa
 from . import getLogger
 
 
+def set_term_title(new_title: str):
+    print(f"\033]0;{new_title}\a", end='')
+
+
 def genconfig(conf_path=""):
     """Generate the config file if it doesn't exist already."""
     if not conf_path:
         conf_path = get_home_dir() + "/.owega.json"
     is_blank = True
     if (os.path.exists(conf_path)):
         is_blank = False
```

### Comparing `owega-5.6.1/owega.egg-info/PKG-INFO` & `owega-5.6.2/owega.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: owega
-Version: 5.6.1
+Version: 5.6.2
 Summary: A command-line interface for conversing with GPT models (from OpenAI)
 Home-page: https://git.pyrokinesis.fr/darkgeem/owega
 Author: darkgeem
 Author-email: darkgeem@pyrokinesis.fr
 License: WTFPL
 Project-URL: Source, https://git.pyrokinesis.fr/darkgeem/owega
 Project-URL: Support, https://discord.gg/KdRmyRrA48
@@ -135,15 +135,15 @@
 See ΦωΦ in action!
 
 [![asciicast](https://asciinema.org/a/613143.png)](https://asciinema.org/a/613143)
 
 
 ## CHANGELOG: 
 ```
-OWEGA v5.6.1 CHANGELOG:
+OWEGA v5.6.2 CHANGELOG:
 
 
 2.0.0: WTFPL license
 2.0.1: added genconf command
 
 2.1.0: added file_input command
 2.1.1: added file_input in help command
@@ -356,8 +356,9 @@
 5.5.5: Now using openai module to ask mistral API.
        (the code is waaaay cleaner)
 
 5.6.0: Added basic support for Chub's API 
        (chub mars, mercury, mixtral)
        Also, Mi(s/x)tral support is no more in beta :D
 5.6.1: Added extensive logging for errors.
+5.6.2: Added terminal title status :3
 ```
```

### Comparing `owega-5.6.1/owega.egg-info/SOURCES.txt` & `owega-5.6.2/owega.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `owega-5.6.1/setup.py` & `owega-5.6.2/setup.py`

 * *Files identical despite different names*

