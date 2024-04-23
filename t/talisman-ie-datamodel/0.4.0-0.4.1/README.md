# Comparing `tmp/talisman-ie-datamodel-0.4.0.tar.gz` & `tmp/talisman-ie-datamodel-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "talisman-ie-datamodel-0.4.0.tar", last modified: Wed Mar 20 12:53:00 2024, max compression
+gzip compressed data, was "talisman-ie-datamodel-0.4.1.tar", last modified: Tue Apr 23 13:12:51 2024, max compression
```

## Comparing `talisman-ie-datamodel-0.4.0.tar` & `talisman-ie-datamodel-0.4.1.tar`

### file list

```diff
@@ -1,75 +1,75 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-20 12:53:00.618098 talisman-ie-datamodel-0.4.0/
--rw-r--r--   0 root         (0) root         (0)      646 2024-03-20 12:53:00.618098 talisman-ie-datamodel-0.4.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-20 12:52:39.000000 talisman-ie-datamodel-0.4.0/README.md
--rw-rw-rw-   0 root         (0) root         (0)        5 2024-03-19 10:09:27.000000 talisman-ie-datamodel-0.4.0/VERSION
--rw-r--r--   0 root         (0) root         (0)       38 2024-03-20 12:53:00.618098 talisman-ie-datamodel-0.4.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1395 2024-03-20 12:40:08.000000 talisman-ie-datamodel-0.4.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-20 12:53:00.614098 talisman-ie-datamodel-0.4.0/talisman_ie_datamodel.egg-info/
--rw-r--r--   0 root         (0) root         (0)      646 2024-03-20 12:53:00.000000 talisman-ie-datamodel-0.4.0/talisman_ie_datamodel.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2309 2024-03-20 12:53:00.000000 talisman-ie-datamodel-0.4.0/talisman_ie_datamodel.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-20 12:53:00.000000 talisman-ie-datamodel-0.4.0/talisman_ie_datamodel.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       39 2024-03-20 12:53:00.000000 talisman-ie-datamodel-0.4.0/talisman_ie_datamodel.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      156 2024-03-20 12:53:00.000000 talisman-ie-datamodel-0.4.0/talisman_ie_datamodel.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2024-03-20 12:53:00.000000 talisman-ie-datamodel-0.4.0/talisman_ie_datamodel.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-20 12:53:00.614098 talisman-ie-datamodel-0.4.0/tie_datamodel/
--rw-rw-rw-   0 root         (0) root         (0)      265 2024-03-04 15:46:06.000000 talisman-ie-datamodel-0.4.0/tie_datamodel/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-20 12:53:00.614098 talisman-ie-datamodel-0.4.0/tie_datamodel/datamodel/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-20 12:52:39.000000 talisman-ie-datamodel-0.4.0/tie_datamodel/datamodel/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5085 2024-03-04 15:46:06.000000 talisman-ie-datamodel-0.4.0/tie_datamodel/datamodel/container.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-20 12:53:00.614098 talisman-ie-datamodel-0.4.0/tie_datamodel/datamodel/node/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-20 12:52:39.000000 talisman-ie-datamodel-0.4.0/tie_datamodel/datamodel/node/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5272 2024-03-04 15:46:06.000000 talisman-ie-datamodel-0.4.0/tie_datamodel/datamodel/node/node_converter.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-20 12:53:00.614098 talisman-ie-datamodel-0.4.0/tie_datamodel/datamodel/node/table/
--rw-rw-rw-   0 root         (0) root         (0)      201 2024-03-04 15:46:06.000000 talisman-ie-datamodel-0.4.0/tie_datamodel/datamodel/node/table/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4018 2024-03-04 15:46:06.000000 talisman-ie-datamodel-0.4.0/tie_datamodel/datamodel/node/table/abstract.py
--rw-rw-rw-   0 root         (0) root         (0)     2159 2024-03-04 15:46:06.000000 talisman-ie-datamodel-0.4.0/tie_datamodel/datamodel/node/table/markup.py
--rw-rw-rw-   0 root         (0) root         (0)      580 2024-03-04 15:46:06.000000 talisman-ie-datamodel-0.4.0/tie_datamodel/datamodel/node/table/node.py
--rw-rw-rw-   0 root         (0) root         (0)     5241 2024-03-04 15:46:06.000000 talisman-ie-datamodel-0.4.0/tie_datamodel/datamodel/node/table/table_view.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-20 12:53:00.614098 talisman-ie-datamodel-0.4.0/tie_datamodel/datamodel/node/text/
--rw-rw-rw-   0 root         (0) root         (0)      293 2024-03-04 15:46:06.000000 talisman-ie-datamodel-0.4.0/tie_datamodel/datamodel/node/text/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1918 2024-03-04 15:46:06.000000 talisman-ie-datamodel-0.4.0/tie_datamodel/datamodel/node/text/abstract.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-20 12:53:00.618098 talisman-ie-datamodel-0.4.0/tie_datamodel/datamodel/node/text/chain/
--rw-rw-rw-   0 root         (0) root         (0)      113 2024-03-04 15:46:06.000000 talisman-ie-datamodel-0.4.0/tie_datamodel/datamodel/node/text/chain/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1496 2024-03-04 15:46:06.000000 talisman-ie-datamodel-0.4.0/tie_datamodel/datamodel/node/text/chain/impl.py
--rw-rw-rw-   0 root         (0) root         (0)     2272 2024-03-04 15:46:06.000000 talisman-ie-datamodel-0.4.0/tie_datamodel/datamodel/node/text/chain/mention.py
--rw-rw-rw-   0 root         (0) root         (0)      806 2024-03-04 15:46:06.000000 talisman-ie-datamodel-0.4.0/tie_datamodel/datamodel/node/text/chain/model.py
--rw-rw-rw-   0 root         (0) root         (0)     3472 2024-03-04 15:46:06.000000 talisman-ie-datamodel-0.4.0/tie_datamodel/datamodel/node/text/markup.py
--rw-rw-rw-   0 root         (0) root         (0)     1361 2024-03-04 15:46:06.000000 talisman-ie-datamodel-0.4.0/tie_datamodel/datamodel/node/text/model.py
--rw-rw-rw-   0 root         (0) root         (0)     2059 2024-03-04 15:46:06.000000 talisman-ie-datamodel-0.4.0/tie_datamodel/datamodel/node/text/node.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-20 12:53:00.618098 talisman-ie-datamodel-0.4.0/tie_datamodel/datamodel/node/text/sentence/
--rw-rw-rw-   0 root         (0) root         (0)       99 2024-03-04 15:46:06.000000 talisman-ie-datamodel-0.4.0/tie_datamodel/datamodel/node/text/sentence/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6481 2024-03-04 15:46:06.000000 talisman-ie-datamodel-0.4.0/tie_datamodel/datamodel/node/text/sentence/impl.py
--rw-rw-rw-   0 root         (0) root         (0)     1198 2024-03-04 15:46:06.000000 talisman-ie-datamodel-0.4.0/tie_datamodel/datamodel/node/text/sentence/model.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-20 12:53:00.618098 talisman-ie-datamodel-0.4.0/tie_datamodel/datamodel/span/
--rw-rw-rw-   0 root         (0) root         (0)      233 2024-03-04 15:46:06.000000 talisman-ie-datamodel-0.4.0/tie_datamodel/datamodel/span/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1609 2024-03-04 15:46:06.000000 talisman-ie-datamodel-0.4.0/tie_datamodel/datamodel/span/abstract.py
--rw-rw-rw-   0 root         (0) root         (0)      723 2024-03-04 15:46:06.000000 talisman-ie-datamodel-0.4.0/tie_datamodel/datamodel/span/default.py
--rw-rw-rw-   0 root         (0) root         (0)      896 2024-03-04 15:46:06.000000 talisman-ie-datamodel-0.4.0/tie_datamodel/datamodel/span/nullable.py
--rw-rw-rw-   0 root         (0) root         (0)      914 2024-03-04 15:46:06.000000 talisman-ie-datamodel-0.4.0/tie_datamodel/datamodel/span/span.py
--rw-rw-rw-   0 root         (0) root         (0)     1029 2024-03-04 15:46:06.000000 talisman-ie-datamodel-0.4.0/tie_datamodel/datamodel/span/token.py
--rw-rw-rw-   0 root         (0) root         (0)      223 2024-03-20 12:40:08.000000 talisman-ie-datamodel-0.4.0/tie_datamodel/env.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-20 12:53:00.618098 talisman-ie-datamodel-0.4.0/tie_datamodel/readers/
--rw-rw-rw-   0 root         (0) root         (0)      723 2024-03-04 15:46:06.000000 talisman-ie-datamodel-0.4.0/tie_datamodel/readers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4271 2024-03-04 15:46:06.000000 talisman-ie-datamodel-0.4.0/tie_datamodel/readers/brat.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-20 12:53:00.618098 talisman-ie-datamodel-0.4.0/tie_datamodel/readers/conll/
--rw-rw-rw-   0 root         (0) root         (0)      196 2024-03-04 15:46:06.000000 talisman-ie-datamodel-0.4.0/tie_datamodel/readers/conll/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3825 2024-03-04 15:46:06.000000 talisman-ie-datamodel-0.4.0/tie_datamodel/readers/conll/abstract.py
--rw-rw-rw-   0 root         (0) root         (0)      816 2024-03-04 15:46:06.000000 talisman-ie-datamodel-0.4.0/tie_datamodel/readers/conll/common.py
--rw-rw-rw-   0 root         (0) root         (0)      636 2024-03-04 15:46:06.000000 talisman-ie-datamodel-0.4.0/tie_datamodel/readers/conll/ontonotes.py
--rw-rw-rw-   0 root         (0) root         (0)      433 2024-03-04 15:46:06.000000 talisman-ie-datamodel-0.4.0/tie_datamodel/readers/directory.py
--rw-rw-rw-   0 root         (0) root         (0)     8440 2024-03-04 15:46:06.000000 talisman-ie-datamodel-0.4.0/tie_datamodel/readers/docred.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-20 12:53:00.618098 talisman-ie-datamodel-0.4.0/tie_datamodel/readers/jsonl/
--rw-rw-rw-   0 root         (0) root         (0)      191 2024-03-04 15:46:06.000000 talisman-ie-datamodel-0.4.0/tie_datamodel/readers/jsonl/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2597 2024-03-20 12:40:08.000000 talisman-ie-datamodel-0.4.0/tie_datamodel/readers/jsonl/abstract.py
--rw-rw-rw-   0 root         (0) root         (0)     1084 2024-03-04 15:46:06.000000 talisman-ie-datamodel-0.4.0/tie_datamodel/readers/jsonl/doccano.py
--rw-rw-rw-   0 root         (0) root         (0)      287 2024-03-04 15:46:06.000000 talisman-ie-datamodel-0.4.0/tie_datamodel/readers/jsonl/tdm.py
--rw-rw-rw-   0 root         (0) root         (0)     2493 2024-03-04 15:46:06.000000 talisman-ie-datamodel-0.4.0/tie_datamodel/readers/jsonl/wlcoref.py
--rw-rw-rw-   0 root         (0) root         (0)     1495 2024-03-04 15:46:06.000000 talisman-ie-datamodel-0.4.0/tie_datamodel/readers/raw.py
--rw-rw-rw-   0 root         (0) root         (0)     1164 2024-03-04 15:46:06.000000 talisman-ie-datamodel-0.4.0/tie_datamodel/readers/readers.py
--rw-rw-rw-   0 root         (0) root         (0)     1245 2024-03-04 15:46:06.000000 talisman-ie-datamodel-0.4.0/tie_datamodel/readers/rucoco.py
--rw-rw-rw-   0 root         (0) root         (0)     2029 2024-03-04 15:46:06.000000 talisman-ie-datamodel-0.4.0/tie_datamodel/readers/rueval.py
--rw-rw-rw-   0 root         (0) root         (0)     4654 2024-03-04 15:46:06.000000 talisman-ie-datamodel-0.4.0/tie_datamodel/readers/tacred.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-20 12:53:00.618098 talisman-ie-datamodel-0.4.0/tie_datamodel/serializers/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-20 12:52:39.000000 talisman-ie-datamodel-0.4.0/tie_datamodel/serializers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1388 2024-03-04 15:46:06.000000 talisman-ie-datamodel-0.4.0/tie_datamodel/serializers/jsonl.py
--rw-rw-rw-   0 root         (0) root         (0)      141 2024-03-04 15:46:06.000000 talisman-ie-datamodel-0.4.0/tie_datamodel/serializers/serializers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 13:12:51.952477 talisman-ie-datamodel-0.4.1/
+-rw-r--r--   0 root         (0) root         (0)      646 2024-04-23 13:12:51.952477 talisman-ie-datamodel-0.4.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-23 13:12:43.000000 talisman-ie-datamodel-0.4.1/README.md
+-rw-rw-rw-   0 root         (0) root         (0)        5 2024-04-23 13:05:07.000000 talisman-ie-datamodel-0.4.1/VERSION
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-23 13:12:51.952477 talisman-ie-datamodel-0.4.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1395 2024-04-23 13:05:07.000000 talisman-ie-datamodel-0.4.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 13:12:51.952477 talisman-ie-datamodel-0.4.1/talisman_ie_datamodel.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      646 2024-04-23 13:12:51.000000 talisman-ie-datamodel-0.4.1/talisman_ie_datamodel.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2309 2024-04-23 13:12:51.000000 talisman-ie-datamodel-0.4.1/talisman_ie_datamodel.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-23 13:12:51.000000 talisman-ie-datamodel-0.4.1/talisman_ie_datamodel.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       39 2024-04-23 13:12:51.000000 talisman-ie-datamodel-0.4.1/talisman_ie_datamodel.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      156 2024-04-23 13:12:51.000000 talisman-ie-datamodel-0.4.1/talisman_ie_datamodel.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2024-04-23 13:12:51.000000 talisman-ie-datamodel-0.4.1/talisman_ie_datamodel.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 13:12:51.952477 talisman-ie-datamodel-0.4.1/tie_datamodel/
+-rw-rw-rw-   0 root         (0) root         (0)      265 2024-04-23 13:05:07.000000 talisman-ie-datamodel-0.4.1/tie_datamodel/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 13:12:51.952477 talisman-ie-datamodel-0.4.1/tie_datamodel/datamodel/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-23 13:12:43.000000 talisman-ie-datamodel-0.4.1/tie_datamodel/datamodel/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5085 2024-04-23 13:05:07.000000 talisman-ie-datamodel-0.4.1/tie_datamodel/datamodel/container.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 13:12:51.952477 talisman-ie-datamodel-0.4.1/tie_datamodel/datamodel/node/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-23 13:12:43.000000 talisman-ie-datamodel-0.4.1/tie_datamodel/datamodel/node/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5272 2024-04-23 13:05:07.000000 talisman-ie-datamodel-0.4.1/tie_datamodel/datamodel/node/node_converter.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 13:12:51.952477 talisman-ie-datamodel-0.4.1/tie_datamodel/datamodel/node/table/
+-rw-rw-rw-   0 root         (0) root         (0)      201 2024-04-23 13:05:07.000000 talisman-ie-datamodel-0.4.1/tie_datamodel/datamodel/node/table/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4018 2024-04-23 13:05:07.000000 talisman-ie-datamodel-0.4.1/tie_datamodel/datamodel/node/table/abstract.py
+-rw-rw-rw-   0 root         (0) root         (0)     2159 2024-04-23 13:05:07.000000 talisman-ie-datamodel-0.4.1/tie_datamodel/datamodel/node/table/markup.py
+-rw-rw-rw-   0 root         (0) root         (0)      580 2024-04-23 13:05:07.000000 talisman-ie-datamodel-0.4.1/tie_datamodel/datamodel/node/table/node.py
+-rw-rw-rw-   0 root         (0) root         (0)     5241 2024-04-23 13:05:07.000000 talisman-ie-datamodel-0.4.1/tie_datamodel/datamodel/node/table/table_view.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 13:12:51.952477 talisman-ie-datamodel-0.4.1/tie_datamodel/datamodel/node/text/
+-rw-rw-rw-   0 root         (0) root         (0)      293 2024-04-23 13:05:07.000000 talisman-ie-datamodel-0.4.1/tie_datamodel/datamodel/node/text/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1918 2024-04-23 13:05:07.000000 talisman-ie-datamodel-0.4.1/tie_datamodel/datamodel/node/text/abstract.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 13:12:51.952477 talisman-ie-datamodel-0.4.1/tie_datamodel/datamodel/node/text/chain/
+-rw-rw-rw-   0 root         (0) root         (0)      113 2024-04-23 13:05:07.000000 talisman-ie-datamodel-0.4.1/tie_datamodel/datamodel/node/text/chain/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1496 2024-04-23 13:05:07.000000 talisman-ie-datamodel-0.4.1/tie_datamodel/datamodel/node/text/chain/impl.py
+-rw-rw-rw-   0 root         (0) root         (0)     2272 2024-04-23 13:05:07.000000 talisman-ie-datamodel-0.4.1/tie_datamodel/datamodel/node/text/chain/mention.py
+-rw-rw-rw-   0 root         (0) root         (0)      806 2024-04-23 13:05:07.000000 talisman-ie-datamodel-0.4.1/tie_datamodel/datamodel/node/text/chain/model.py
+-rw-rw-rw-   0 root         (0) root         (0)     3472 2024-04-23 13:05:07.000000 talisman-ie-datamodel-0.4.1/tie_datamodel/datamodel/node/text/markup.py
+-rw-rw-rw-   0 root         (0) root         (0)     1361 2024-04-23 13:05:07.000000 talisman-ie-datamodel-0.4.1/tie_datamodel/datamodel/node/text/model.py
+-rw-rw-rw-   0 root         (0) root         (0)     2059 2024-04-23 13:05:07.000000 talisman-ie-datamodel-0.4.1/tie_datamodel/datamodel/node/text/node.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 13:12:51.952477 talisman-ie-datamodel-0.4.1/tie_datamodel/datamodel/node/text/sentence/
+-rw-rw-rw-   0 root         (0) root         (0)       99 2024-04-23 13:05:07.000000 talisman-ie-datamodel-0.4.1/tie_datamodel/datamodel/node/text/sentence/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6481 2024-04-23 13:05:07.000000 talisman-ie-datamodel-0.4.1/tie_datamodel/datamodel/node/text/sentence/impl.py
+-rw-rw-rw-   0 root         (0) root         (0)     1198 2024-04-23 13:05:07.000000 talisman-ie-datamodel-0.4.1/tie_datamodel/datamodel/node/text/sentence/model.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 13:12:51.952477 talisman-ie-datamodel-0.4.1/tie_datamodel/datamodel/span/
+-rw-rw-rw-   0 root         (0) root         (0)      233 2024-04-23 13:05:07.000000 talisman-ie-datamodel-0.4.1/tie_datamodel/datamodel/span/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1609 2024-04-23 13:05:07.000000 talisman-ie-datamodel-0.4.1/tie_datamodel/datamodel/span/abstract.py
+-rw-rw-rw-   0 root         (0) root         (0)      723 2024-04-23 13:05:07.000000 talisman-ie-datamodel-0.4.1/tie_datamodel/datamodel/span/default.py
+-rw-rw-rw-   0 root         (0) root         (0)      896 2024-04-23 13:05:07.000000 talisman-ie-datamodel-0.4.1/tie_datamodel/datamodel/span/nullable.py
+-rw-rw-rw-   0 root         (0) root         (0)      914 2024-04-23 13:05:07.000000 talisman-ie-datamodel-0.4.1/tie_datamodel/datamodel/span/span.py
+-rw-rw-rw-   0 root         (0) root         (0)     1029 2024-04-23 13:05:07.000000 talisman-ie-datamodel-0.4.1/tie_datamodel/datamodel/span/token.py
+-rw-rw-rw-   0 root         (0) root         (0)      223 2024-04-23 13:05:07.000000 talisman-ie-datamodel-0.4.1/tie_datamodel/env.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 13:12:51.952477 talisman-ie-datamodel-0.4.1/tie_datamodel/readers/
+-rw-rw-rw-   0 root         (0) root         (0)      723 2024-04-23 13:05:07.000000 talisman-ie-datamodel-0.4.1/tie_datamodel/readers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4271 2024-04-23 13:05:07.000000 talisman-ie-datamodel-0.4.1/tie_datamodel/readers/brat.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 13:12:51.952477 talisman-ie-datamodel-0.4.1/tie_datamodel/readers/conll/
+-rw-rw-rw-   0 root         (0) root         (0)      196 2024-04-23 13:05:07.000000 talisman-ie-datamodel-0.4.1/tie_datamodel/readers/conll/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3825 2024-04-23 13:05:07.000000 talisman-ie-datamodel-0.4.1/tie_datamodel/readers/conll/abstract.py
+-rw-rw-rw-   0 root         (0) root         (0)      816 2024-04-23 13:05:07.000000 talisman-ie-datamodel-0.4.1/tie_datamodel/readers/conll/common.py
+-rw-rw-rw-   0 root         (0) root         (0)      636 2024-04-23 13:05:07.000000 talisman-ie-datamodel-0.4.1/tie_datamodel/readers/conll/ontonotes.py
+-rw-rw-rw-   0 root         (0) root         (0)      433 2024-04-23 13:05:07.000000 talisman-ie-datamodel-0.4.1/tie_datamodel/readers/directory.py
+-rw-rw-rw-   0 root         (0) root         (0)     8440 2024-04-23 13:05:07.000000 talisman-ie-datamodel-0.4.1/tie_datamodel/readers/docred.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 13:12:51.952477 talisman-ie-datamodel-0.4.1/tie_datamodel/readers/jsonl/
+-rw-rw-rw-   0 root         (0) root         (0)      191 2024-04-23 13:05:07.000000 talisman-ie-datamodel-0.4.1/tie_datamodel/readers/jsonl/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2906 2024-04-23 13:05:07.000000 talisman-ie-datamodel-0.4.1/tie_datamodel/readers/jsonl/abstract.py
+-rw-rw-rw-   0 root         (0) root         (0)     1084 2024-04-23 13:05:07.000000 talisman-ie-datamodel-0.4.1/tie_datamodel/readers/jsonl/doccano.py
+-rw-rw-rw-   0 root         (0) root         (0)      287 2024-04-23 13:05:07.000000 talisman-ie-datamodel-0.4.1/tie_datamodel/readers/jsonl/tdm.py
+-rw-rw-rw-   0 root         (0) root         (0)     2493 2024-04-23 13:05:07.000000 talisman-ie-datamodel-0.4.1/tie_datamodel/readers/jsonl/wlcoref.py
+-rw-rw-rw-   0 root         (0) root         (0)     1495 2024-04-23 13:05:07.000000 talisman-ie-datamodel-0.4.1/tie_datamodel/readers/raw.py
+-rw-rw-rw-   0 root         (0) root         (0)     1164 2024-04-23 13:05:07.000000 talisman-ie-datamodel-0.4.1/tie_datamodel/readers/readers.py
+-rw-rw-rw-   0 root         (0) root         (0)     1245 2024-04-23 13:05:07.000000 talisman-ie-datamodel-0.4.1/tie_datamodel/readers/rucoco.py
+-rw-rw-rw-   0 root         (0) root         (0)     2029 2024-04-23 13:05:07.000000 talisman-ie-datamodel-0.4.1/tie_datamodel/readers/rueval.py
+-rw-rw-rw-   0 root         (0) root         (0)     4654 2024-04-23 13:05:07.000000 talisman-ie-datamodel-0.4.1/tie_datamodel/readers/tacred.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 13:12:51.952477 talisman-ie-datamodel-0.4.1/tie_datamodel/serializers/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-23 13:12:43.000000 talisman-ie-datamodel-0.4.1/tie_datamodel/serializers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1388 2024-04-23 13:05:07.000000 talisman-ie-datamodel-0.4.1/tie_datamodel/serializers/jsonl.py
+-rw-rw-rw-   0 root         (0) root         (0)      141 2024-04-23 13:05:07.000000 talisman-ie-datamodel-0.4.1/tie_datamodel/serializers/serializers.py
```

### Comparing `talisman-ie-datamodel-0.4.0/PKG-INFO` & `talisman-ie-datamodel-0.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: talisman-ie-datamodel
-Version: 0.4.0
+Version: 0.4.1
 Summary: Talisman-IE Document Model
 Author: ISPRAS Talisman NLP team
 Author-email: modis@ispras.ru
 Maintainer: Vladimir Mayorov
 Maintainer-email: vmayorov@ispras.ru
 License: Apache Software License
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `talisman-ie-datamodel-0.4.0/setup.py` & `talisman-ie-datamodel-0.4.1/setup.py`

 * *Files identical despite different names*

### Comparing `talisman-ie-datamodel-0.4.0/talisman_ie_datamodel.egg-info/PKG-INFO` & `talisman-ie-datamodel-0.4.1/talisman_ie_datamodel.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: talisman-ie-datamodel
-Version: 0.4.0
+Version: 0.4.1
 Summary: Talisman-IE Document Model
 Author: ISPRAS Talisman NLP team
 Author-email: modis@ispras.ru
 Maintainer: Vladimir Mayorov
 Maintainer-email: vmayorov@ispras.ru
 License: Apache Software License
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `talisman-ie-datamodel-0.4.0/talisman_ie_datamodel.egg-info/SOURCES.txt` & `talisman-ie-datamodel-0.4.1/talisman_ie_datamodel.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `talisman-ie-datamodel-0.4.0/tie_datamodel/datamodel/container.py` & `talisman-ie-datamodel-0.4.1/tie_datamodel/datamodel/container.py`

 * *Files identical despite different names*

### Comparing `talisman-ie-datamodel-0.4.0/tie_datamodel/datamodel/node/node_converter.py` & `talisman-ie-datamodel-0.4.1/tie_datamodel/datamodel/node/node_converter.py`

 * *Files identical despite different names*

### Comparing `talisman-ie-datamodel-0.4.0/tie_datamodel/datamodel/node/table/abstract.py` & `talisman-ie-datamodel-0.4.1/tie_datamodel/datamodel/node/table/abstract.py`

 * *Files identical despite different names*

### Comparing `talisman-ie-datamodel-0.4.0/tie_datamodel/datamodel/node/table/markup.py` & `talisman-ie-datamodel-0.4.1/tie_datamodel/datamodel/node/table/markup.py`

 * *Files identical despite different names*

### Comparing `talisman-ie-datamodel-0.4.0/tie_datamodel/datamodel/node/table/node.py` & `talisman-ie-datamodel-0.4.1/tie_datamodel/datamodel/node/table/node.py`

 * *Files identical despite different names*

### Comparing `talisman-ie-datamodel-0.4.0/tie_datamodel/datamodel/node/table/table_view.py` & `talisman-ie-datamodel-0.4.1/tie_datamodel/datamodel/node/table/table_view.py`

 * *Files identical despite different names*

### Comparing `talisman-ie-datamodel-0.4.0/tie_datamodel/datamodel/node/text/abstract.py` & `talisman-ie-datamodel-0.4.1/tie_datamodel/datamodel/node/text/abstract.py`

 * *Files identical despite different names*

### Comparing `talisman-ie-datamodel-0.4.0/tie_datamodel/datamodel/node/text/chain/impl.py` & `talisman-ie-datamodel-0.4.1/tie_datamodel/datamodel/node/text/chain/impl.py`

 * *Files identical despite different names*

### Comparing `talisman-ie-datamodel-0.4.0/tie_datamodel/datamodel/node/text/chain/mention.py` & `talisman-ie-datamodel-0.4.1/tie_datamodel/datamodel/node/text/chain/mention.py`

 * *Files identical despite different names*

### Comparing `talisman-ie-datamodel-0.4.0/tie_datamodel/datamodel/node/text/chain/model.py` & `talisman-ie-datamodel-0.4.1/tie_datamodel/datamodel/node/text/chain/model.py`

 * *Files identical despite different names*

### Comparing `talisman-ie-datamodel-0.4.0/tie_datamodel/datamodel/node/text/markup.py` & `talisman-ie-datamodel-0.4.1/tie_datamodel/datamodel/node/text/markup.py`

 * *Files identical despite different names*

### Comparing `talisman-ie-datamodel-0.4.0/tie_datamodel/datamodel/node/text/model.py` & `talisman-ie-datamodel-0.4.1/tie_datamodel/datamodel/node/text/model.py`

 * *Files identical despite different names*

### Comparing `talisman-ie-datamodel-0.4.0/tie_datamodel/datamodel/node/text/node.py` & `talisman-ie-datamodel-0.4.1/tie_datamodel/datamodel/node/text/node.py`

 * *Files identical despite different names*

### Comparing `talisman-ie-datamodel-0.4.0/tie_datamodel/datamodel/node/text/sentence/impl.py` & `talisman-ie-datamodel-0.4.1/tie_datamodel/datamodel/node/text/sentence/impl.py`

 * *Files identical despite different names*

### Comparing `talisman-ie-datamodel-0.4.0/tie_datamodel/datamodel/node/text/sentence/model.py` & `talisman-ie-datamodel-0.4.1/tie_datamodel/datamodel/node/text/sentence/model.py`

 * *Files identical despite different names*

### Comparing `talisman-ie-datamodel-0.4.0/tie_datamodel/datamodel/span/abstract.py` & `talisman-ie-datamodel-0.4.1/tie_datamodel/datamodel/span/abstract.py`

 * *Files identical despite different names*

### Comparing `talisman-ie-datamodel-0.4.0/tie_datamodel/datamodel/span/default.py` & `talisman-ie-datamodel-0.4.1/tie_datamodel/datamodel/span/default.py`

 * *Files identical despite different names*

### Comparing `talisman-ie-datamodel-0.4.0/tie_datamodel/datamodel/span/nullable.py` & `talisman-ie-datamodel-0.4.1/tie_datamodel/datamodel/span/nullable.py`

 * *Files identical despite different names*

### Comparing `talisman-ie-datamodel-0.4.0/tie_datamodel/datamodel/span/span.py` & `talisman-ie-datamodel-0.4.1/tie_datamodel/datamodel/span/span.py`

 * *Files identical despite different names*

### Comparing `talisman-ie-datamodel-0.4.0/tie_datamodel/datamodel/span/token.py` & `talisman-ie-datamodel-0.4.1/tie_datamodel/datamodel/span/token.py`

 * *Files identical despite different names*

### Comparing `talisman-ie-datamodel-0.4.0/tie_datamodel/readers/__init__.py` & `talisman-ie-datamodel-0.4.1/tie_datamodel/readers/__init__.py`

 * *Files identical despite different names*

### Comparing `talisman-ie-datamodel-0.4.0/tie_datamodel/readers/brat.py` & `talisman-ie-datamodel-0.4.1/tie_datamodel/readers/brat.py`

 * *Files identical despite different names*

### Comparing `talisman-ie-datamodel-0.4.0/tie_datamodel/readers/conll/abstract.py` & `talisman-ie-datamodel-0.4.1/tie_datamodel/readers/conll/abstract.py`

 * *Files identical despite different names*

### Comparing `talisman-ie-datamodel-0.4.0/tie_datamodel/readers/conll/common.py` & `talisman-ie-datamodel-0.4.1/tie_datamodel/readers/conll/common.py`

 * *Files identical despite different names*

### Comparing `talisman-ie-datamodel-0.4.0/tie_datamodel/readers/conll/ontonotes.py` & `talisman-ie-datamodel-0.4.1/tie_datamodel/readers/conll/ontonotes.py`

 * *Files identical despite different names*

### Comparing `talisman-ie-datamodel-0.4.0/tie_datamodel/readers/docred.py` & `talisman-ie-datamodel-0.4.1/tie_datamodel/readers/docred.py`

 * *Files identical despite different names*

### Comparing `talisman-ie-datamodel-0.4.0/tie_datamodel/readers/jsonl/abstract.py` & `talisman-ie-datamodel-0.4.1/tie_datamodel/readers/jsonl/abstract.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 from multiprocessing.pool import ApplyResult, Pool
 from os import PathLike
 from pathlib import Path
 from random import Random
 from typing import Dict, Iterable, Iterator
 
 from tdm import TalismanDocument
+from tdm.datamodel.common._view import generate_dataclass_view
+from tdm.datamodel.mentions import NodeMention, TextNodeMention
 
 from tie_datamodel.env import get_max_spawned_processes
 from tp_interfaces.readers.abstract import AbstractConfigurableReader
 
 try:
     from talisman_tools.helper.multiprocessing import setup_multiprocessing
     from talisman_tools.helper.concurrency import check_on_jobs
@@ -47,14 +49,18 @@
         yield from self._parse_contents(lines, n_jobs=get_max_spawned_processes())
 
     def _parse_contents(self, lines: Iterable[str], *, n_jobs: int = 1) -> Iterable[TalismanDocument]:
         if n_jobs <= 1:
             yield from map(self._process_line, lines)
             return
 
+        # for fixing deserialization of document instance when process from pool exits
+        generate_dataclass_view(TextNodeMention)
+        generate_dataclass_view(NodeMention)
+
         decoding_jobs: Dict[int, ApplyResult[TalismanDocument]] = {}
         decoded_docs: Dict[int, TalismanDocument] = {}
         with Pool(n_jobs) as pool:
             for doc_id, line in enumerate(lines):
                 decoding_jobs[doc_id] = pool.apply_async(self._process_line, args=(line,))
 
             last_processed_doc_id = 0
```

### Comparing `talisman-ie-datamodel-0.4.0/tie_datamodel/readers/jsonl/doccano.py` & `talisman-ie-datamodel-0.4.1/tie_datamodel/readers/jsonl/doccano.py`

 * *Files identical despite different names*

### Comparing `talisman-ie-datamodel-0.4.0/tie_datamodel/readers/jsonl/wlcoref.py` & `talisman-ie-datamodel-0.4.1/tie_datamodel/readers/jsonl/wlcoref.py`

 * *Files identical despite different names*

### Comparing `talisman-ie-datamodel-0.4.0/tie_datamodel/readers/raw.py` & `talisman-ie-datamodel-0.4.1/tie_datamodel/readers/raw.py`

 * *Files identical despite different names*

### Comparing `talisman-ie-datamodel-0.4.0/tie_datamodel/readers/readers.py` & `talisman-ie-datamodel-0.4.1/tie_datamodel/readers/readers.py`

 * *Files identical despite different names*

### Comparing `talisman-ie-datamodel-0.4.0/tie_datamodel/readers/rucoco.py` & `talisman-ie-datamodel-0.4.1/tie_datamodel/readers/rucoco.py`

 * *Files identical despite different names*

### Comparing `talisman-ie-datamodel-0.4.0/tie_datamodel/readers/rueval.py` & `talisman-ie-datamodel-0.4.1/tie_datamodel/readers/rueval.py`

 * *Files identical despite different names*

### Comparing `talisman-ie-datamodel-0.4.0/tie_datamodel/readers/tacred.py` & `talisman-ie-datamodel-0.4.1/tie_datamodel/readers/tacred.py`

 * *Files identical despite different names*

### Comparing `talisman-ie-datamodel-0.4.0/tie_datamodel/serializers/jsonl.py` & `talisman-ie-datamodel-0.4.1/tie_datamodel/serializers/jsonl.py`

 * *Files identical despite different names*

