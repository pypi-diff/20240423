# Comparing `tmp/pulumi_civo-2.4.0a1713560943.tar.gz` & `tmp/pulumi_civo-2.4.0a1713897269.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_civo-2.4.0a1713560943.tar", last modified: Fri Apr 19 21:11:42 2024, max compression
+gzip compressed data, was "pulumi_civo-2.4.0a1713897269.tar", last modified: Tue Apr 23 18:56:45 2024, max compression
```

## Comparing `pulumi_civo-2.4.0a1713560943.tar` & `pulumi_civo-2.4.0a1713897269.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:11:42.157178 pulumi_civo-2.4.0a1713560943/
--rw-r--r--   0 runner    (1001) docker     (127)     2509 2024-04-19 21:11:42.157178 pulumi_civo-2.4.0a1713560943/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2065 2024-04-19 21:11:35.000000 pulumi_civo-2.4.0a1713560943/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:11:42.153178 pulumi_civo-2.4.0a1713560943/pulumi_civo/
--rw-r--r--   0 runner    (1001) docker     (127)     4334 2024-04-19 21:11:35.000000 pulumi_civo-2.4.0a1713560943/pulumi_civo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    41211 2024-04-19 21:11:35.000000 pulumi_civo-2.4.0a1713560943/pulumi_civo/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-04-19 21:11:35.000000 pulumi_civo-2.4.0a1713560943/pulumi_civo/_utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:11:42.157178 pulumi_civo-2.4.0a1713560943/pulumi_civo/config/
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-19 21:11:35.000000 pulumi_civo-2.4.0a1713560943/pulumi_civo/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      743 2024-04-19 21:11:35.000000 pulumi_civo-2.4.0a1713560943/pulumi_civo/config/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-04-19 21:11:35.000000 pulumi_civo-2.4.0a1713560943/pulumi_civo/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (127)    23846 2024-04-19 21:11:35.000000 pulumi_civo-2.4.0a1713560943/pulumi_civo/database.py
--rw-r--r--   0 runner    (1001) docker     (127)     7205 2024-04-19 21:11:35.000000 pulumi_civo-2.4.0a1713560943/pulumi_civo/dns_domain_name.py
--rw-r--r--   0 runner    (1001) docker     (127)    19775 2024-04-19 21:11:35.000000 pulumi_civo-2.4.0a1713560943/pulumi_civo/dns_domain_record.py
--rw-r--r--   0 runner    (1001) docker     (127)    18933 2024-04-19 21:11:35.000000 pulumi_civo-2.4.0a1713560943/pulumi_civo/firewall.py
--rw-r--r--   0 runner    (1001) docker     (127)    24234 2024-04-19 21:11:35.000000 pulumi_civo-2.4.0a1713560943/pulumi_civo/firewall_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     9765 2024-04-19 21:11:35.000000 pulumi_civo-2.4.0a1713560943/pulumi_civo/get_database.py
--rw-r--r--   0 runner    (1001) docker     (127)     4725 2024-04-19 21:11:35.000000 pulumi_civo-2.4.0a1713560943/pulumi_civo/get_database_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     5485 2024-04-19 21:11:35.000000 pulumi_civo-2.4.0a1713560943/pulumi_civo/get_disk_image.py
--rw-r--r--   0 runner    (1001) docker     (127)     3708 2024-04-19 21:11:35.000000 pulumi_civo-2.4.0a1713560943/pulumi_civo/get_dns_domain_name.py
--rw-r--r--   0 runner    (1001) docker     (127)     7767 2024-04-19 21:11:35.000000 pulumi_civo-2.4.0a1713560943/pulumi_civo/get_dns_domain_record.py
--rw-r--r--   0 runner    (1001) docker     (127)     4953 2024-04-19 21:11:35.000000 pulumi_civo-2.4.0a1713560943/pulumi_civo/get_firewall.py
--rw-r--r--   0 runner    (1001) docker     (127)    13548 2024-04-19 21:11:35.000000 pulumi_civo-2.4.0a1713560943/pulumi_civo/get_instance.py
--rw-r--r--   0 runner    (1001) docker     (127)     6248 2024-04-19 21:11:35.000000 pulumi_civo-2.4.0a1713560943/pulumi_civo/get_instances.py
--rw-r--r--   0 runner    (1001) docker     (127)    12769 2024-04-19 21:11:35.000000 pulumi_civo-2.4.0a1713560943/pulumi_civo/get_kubernetes_cluster.py
--rw-r--r--   0 runner    (1001) docker     (127)     5651 2024-04-19 21:11:35.000000 pulumi_civo-2.4.0a1713560943/pulumi_civo/get_kubernetes_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    11535 2024-04-19 21:11:35.000000 pulumi_civo-2.4.0a1713560943/pulumi_civo/get_load_balancer.py
--rw-r--r--   0 runner    (1001) docker     (127)     5304 2024-04-19 21:11:35.000000 pulumi_civo-2.4.0a1713560943/pulumi_civo/get_network.py
--rw-r--r--   0 runner    (1001) docker     (127)     6592 2024-04-19 21:11:35.000000 pulumi_civo-2.4.0a1713560943/pulumi_civo/get_object_store.py
--rw-r--r--   0 runner    (1001) docker     (127)     7100 2024-04-19 21:11:35.000000 pulumi_civo-2.4.0a1713560943/pulumi_civo/get_object_store_credential.py
--rw-r--r--   0 runner    (1001) docker     (127)     4384 2024-04-19 21:11:35.000000 pulumi_civo-2.4.0a1713560943/pulumi_civo/get_region.py
--rw-r--r--   0 runner    (1001) docker     (127)     4680 2024-04-19 21:11:35.000000 pulumi_civo-2.4.0a1713560943/pulumi_civo/get_reserved_ip.py
--rw-r--r--   0 runner    (1001) docker     (127)     4290 2024-04-19 21:11:35.000000 pulumi_civo-2.4.0a1713560943/pulumi_civo/get_size.py
--rw-r--r--   0 runner    (1001) docker     (127)     3523 2024-04-19 21:11:35.000000 pulumi_civo-2.4.0a1713560943/pulumi_civo/get_ssh_key.py
--rw-r--r--   0 runner    (1001) docker     (127)     5764 2024-04-19 21:11:35.000000 pulumi_civo-2.4.0a1713560943/pulumi_civo/get_volume.py
--rw-r--r--   0 runner    (1001) docker     (127)    47548 2024-04-19 21:11:35.000000 pulumi_civo-2.4.0a1713560943/pulumi_civo/instance.py
--rw-r--r--   0 runner    (1001) docker     (127)    10425 2024-04-19 21:11:35.000000 pulumi_civo-2.4.0a1713560943/pulumi_civo/instance_reserved_ip_assignment.py
--rw-r--r--   0 runner    (1001) docker     (127)    44029 2024-04-19 21:11:35.000000 pulumi_civo-2.4.0a1713560943/pulumi_civo/kubernetes_cluster.py
--rw-r--r--   0 runner    (1001) docker     (127)    20650 2024-04-19 21:11:35.000000 pulumi_civo-2.4.0a1713560943/pulumi_civo/kubernetes_node_pool.py
--rw-r--r--   0 runner    (1001) docker     (127)     9672 2024-04-19 21:11:35.000000 pulumi_civo-2.4.0a1713560943/pulumi_civo/network.py
--rw-r--r--   0 runner    (1001) docker     (127)    15788 2024-04-19 21:11:35.000000 pulumi_civo-2.4.0a1713560943/pulumi_civo/object_store.py
--rw-r--r--   0 runner    (1001) docker     (127)    15615 2024-04-19 21:11:35.000000 pulumi_civo-2.4.0a1713560943/pulumi_civo/object_store_credential.py
--rw-r--r--   0 runner    (1001) docker     (127)    55857 2024-04-19 21:11:35.000000 pulumi_civo-2.4.0a1713560943/pulumi_civo/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     7299 2024-04-19 21:11:35.000000 pulumi_civo-2.4.0a1713560943/pulumi_civo/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-19 21:11:35.000000 pulumi_civo-2.4.0a1713560943/pulumi_civo/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 21:11:35.000000 pulumi_civo-2.4.0a1713560943/pulumi_civo/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     8587 2024-04-19 21:11:35.000000 pulumi_civo-2.4.0a1713560943/pulumi_civo/reserved_ip.py
--rw-r--r--   0 runner    (1001) docker     (127)     9661 2024-04-19 21:11:35.000000 pulumi_civo-2.4.0a1713560943/pulumi_civo/ssh_key.py
--rw-r--r--   0 runner    (1001) docker     (127)    14331 2024-04-19 21:11:35.000000 pulumi_civo-2.4.0a1713560943/pulumi_civo/volume.py
--rw-r--r--   0 runner    (1001) docker     (127)     9414 2024-04-19 21:11:35.000000 pulumi_civo-2.4.0a1713560943/pulumi_civo/volume_attachment.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:11:42.157178 pulumi_civo-2.4.0a1713560943/pulumi_civo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2509 2024-04-19 21:11:42.000000 pulumi_civo-2.4.0a1713560943/pulumi_civo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-04-19 21:11:42.000000 pulumi_civo-2.4.0a1713560943/pulumi_civo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 21:11:42.000000 pulumi_civo-2.4.0a1713560943/pulumi_civo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-19 21:11:42.000000 pulumi_civo-2.4.0a1713560943/pulumi_civo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-19 21:11:42.000000 pulumi_civo-2.4.0a1713560943/pulumi_civo.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      669 2024-04-19 21:11:35.000000 pulumi_civo-2.4.0a1713560943/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 21:11:42.157178 pulumi_civo-2.4.0a1713560943/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:56:45.203404 pulumi_civo-2.4.0a1713897269/
+-rw-r--r--   0 runner    (1001) docker     (127)     2509 2024-04-23 18:56:45.203404 pulumi_civo-2.4.0a1713897269/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2065 2024-04-23 18:56:38.000000 pulumi_civo-2.4.0a1713897269/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:56:45.199403 pulumi_civo-2.4.0a1713897269/pulumi_civo/
+-rw-r--r--   0 runner    (1001) docker     (127)     4334 2024-04-23 18:56:38.000000 pulumi_civo-2.4.0a1713897269/pulumi_civo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41211 2024-04-23 18:56:38.000000 pulumi_civo-2.4.0a1713897269/pulumi_civo/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-04-23 18:56:38.000000 pulumi_civo-2.4.0a1713897269/pulumi_civo/_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:56:45.203404 pulumi_civo-2.4.0a1713897269/pulumi_civo/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-23 18:56:38.000000 pulumi_civo-2.4.0a1713897269/pulumi_civo/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      743 2024-04-23 18:56:38.000000 pulumi_civo-2.4.0a1713897269/pulumi_civo/config/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-04-23 18:56:38.000000 pulumi_civo-2.4.0a1713897269/pulumi_civo/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23846 2024-04-23 18:56:38.000000 pulumi_civo-2.4.0a1713897269/pulumi_civo/database.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7049 2024-04-23 18:56:38.000000 pulumi_civo-2.4.0a1713897269/pulumi_civo/dns_domain_name.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19775 2024-04-23 18:56:38.000000 pulumi_civo-2.4.0a1713897269/pulumi_civo/dns_domain_record.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18933 2024-04-23 18:56:38.000000 pulumi_civo-2.4.0a1713897269/pulumi_civo/firewall.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24234 2024-04-23 18:56:38.000000 pulumi_civo-2.4.0a1713897269/pulumi_civo/firewall_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9625 2024-04-23 18:56:38.000000 pulumi_civo-2.4.0a1713897269/pulumi_civo/get_database.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4725 2024-04-23 18:56:38.000000 pulumi_civo-2.4.0a1713897269/pulumi_civo/get_database_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5485 2024-04-23 18:56:38.000000 pulumi_civo-2.4.0a1713897269/pulumi_civo/get_disk_image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3568 2024-04-23 18:56:38.000000 pulumi_civo-2.4.0a1713897269/pulumi_civo/get_dns_domain_name.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7627 2024-04-23 18:56:38.000000 pulumi_civo-2.4.0a1713897269/pulumi_civo/get_dns_domain_record.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4813 2024-04-23 18:56:38.000000 pulumi_civo-2.4.0a1713897269/pulumi_civo/get_firewall.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13408 2024-04-23 18:56:38.000000 pulumi_civo-2.4.0a1713897269/pulumi_civo/get_instance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6266 2024-04-23 18:56:38.000000 pulumi_civo-2.4.0a1713897269/pulumi_civo/get_instances.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12629 2024-04-23 18:56:38.000000 pulumi_civo-2.4.0a1713897269/pulumi_civo/get_kubernetes_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5511 2024-04-23 18:56:38.000000 pulumi_civo-2.4.0a1713897269/pulumi_civo/get_kubernetes_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11395 2024-04-23 18:56:38.000000 pulumi_civo-2.4.0a1713897269/pulumi_civo/get_load_balancer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5164 2024-04-23 18:56:38.000000 pulumi_civo-2.4.0a1713897269/pulumi_civo/get_network.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6452 2024-04-23 18:56:38.000000 pulumi_civo-2.4.0a1713897269/pulumi_civo/get_object_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6960 2024-04-23 18:56:38.000000 pulumi_civo-2.4.0a1713897269/pulumi_civo/get_object_store_credential.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4384 2024-04-23 18:56:38.000000 pulumi_civo-2.4.0a1713897269/pulumi_civo/get_region.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4680 2024-04-23 18:56:38.000000 pulumi_civo-2.4.0a1713897269/pulumi_civo/get_reserved_ip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4290 2024-04-23 18:56:38.000000 pulumi_civo-2.4.0a1713897269/pulumi_civo/get_size.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3523 2024-04-23 18:56:38.000000 pulumi_civo-2.4.0a1713897269/pulumi_civo/get_ssh_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5624 2024-04-23 18:56:38.000000 pulumi_civo-2.4.0a1713897269/pulumi_civo/get_volume.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47548 2024-04-23 18:56:38.000000 pulumi_civo-2.4.0a1713897269/pulumi_civo/instance.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10269 2024-04-23 18:56:38.000000 pulumi_civo-2.4.0a1713897269/pulumi_civo/instance_reserved_ip_assignment.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44029 2024-04-23 18:56:38.000000 pulumi_civo-2.4.0a1713897269/pulumi_civo/kubernetes_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20650 2024-04-23 18:56:38.000000 pulumi_civo-2.4.0a1713897269/pulumi_civo/kubernetes_node_pool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9516 2024-04-23 18:56:38.000000 pulumi_civo-2.4.0a1713897269/pulumi_civo/network.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15632 2024-04-23 18:56:38.000000 pulumi_civo-2.4.0a1713897269/pulumi_civo/object_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15459 2024-04-23 18:56:38.000000 pulumi_civo-2.4.0a1713897269/pulumi_civo/object_store_credential.py
+-rw-r--r--   0 runner    (1001) docker     (127)    55857 2024-04-23 18:56:38.000000 pulumi_civo-2.4.0a1713897269/pulumi_civo/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7299 2024-04-23 18:56:38.000000 pulumi_civo-2.4.0a1713897269/pulumi_civo/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-23 18:56:38.000000 pulumi_civo-2.4.0a1713897269/pulumi_civo/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 18:56:38.000000 pulumi_civo-2.4.0a1713897269/pulumi_civo/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     8431 2024-04-23 18:56:38.000000 pulumi_civo-2.4.0a1713897269/pulumi_civo/reserved_ip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9505 2024-04-23 18:56:38.000000 pulumi_civo-2.4.0a1713897269/pulumi_civo/ssh_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14175 2024-04-23 18:56:38.000000 pulumi_civo-2.4.0a1713897269/pulumi_civo/volume.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9414 2024-04-23 18:56:38.000000 pulumi_civo-2.4.0a1713897269/pulumi_civo/volume_attachment.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:56:45.203404 pulumi_civo-2.4.0a1713897269/pulumi_civo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2509 2024-04-23 18:56:45.000000 pulumi_civo-2.4.0a1713897269/pulumi_civo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-04-23 18:56:45.000000 pulumi_civo-2.4.0a1713897269/pulumi_civo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 18:56:45.000000 pulumi_civo-2.4.0a1713897269/pulumi_civo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-23 18:56:45.000000 pulumi_civo-2.4.0a1713897269/pulumi_civo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-23 18:56:45.000000 pulumi_civo-2.4.0a1713897269/pulumi_civo.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      669 2024-04-23 18:56:38.000000 pulumi_civo-2.4.0a1713897269/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 18:56:45.203404 pulumi_civo-2.4.0a1713897269/setup.cfg
```

### Comparing `pulumi_civo-2.4.0a1713560943/PKG-INFO` & `pulumi_civo-2.4.0a1713897269/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_civo
-Version: 2.4.0a1713560943
+Version: 2.4.0a1713897269
 Summary: A Pulumi package for creating and managing Civo cloud resources.
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.io
 Project-URL: Repository, https://github.com/pulumi/pulumi-civo
 Keywords: pulumi,civo
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_civo-2.4.0a1713560943/README.md` & `pulumi_civo-2.4.0a1713897269/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1713560943/pulumi_civo/__init__.py` & `pulumi_civo-2.4.0a1713897269/pulumi_civo/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1713560943/pulumi_civo/_inputs.py` & `pulumi_civo-2.4.0a1713897269/pulumi_civo/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1713560943/pulumi_civo/_utilities.py` & `pulumi_civo-2.4.0a1713897269/pulumi_civo/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1713560943/pulumi_civo/config/__init__.pyi` & `pulumi_civo-2.4.0a1713897269/pulumi_civo/config/__init__.pyi`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1713560943/pulumi_civo/config/vars.py` & `pulumi_civo-2.4.0a1713897269/pulumi_civo/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1713560943/pulumi_civo/database.py` & `pulumi_civo-2.4.0a1713897269/pulumi_civo/database.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1713560943/pulumi_civo/dns_domain_name.py` & `pulumi_civo-2.4.0a1713897269/pulumi_civo/dns_domain_name.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,23 +83,21 @@
                  name: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         Provides a Civo DNS domain name resource.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_civo as civo
 
         # Create a new domain name
         main = civo.DnsDomainName("main", name="mydomain.com")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         using domain name
 
         ```sh
         $ pulumi import civo:index/dnsDomainName:DnsDomainName main mydomain.com
@@ -116,23 +114,21 @@
                  args: Optional[DnsDomainNameArgs] = None,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         Provides a Civo DNS domain name resource.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_civo as civo
 
         # Create a new domain name
         main = civo.DnsDomainName("main", name="mydomain.com")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         using domain name
 
         ```sh
         $ pulumi import civo:index/dnsDomainName:DnsDomainName main mydomain.com
```

### Comparing `pulumi_civo-2.4.0a1713560943/pulumi_civo/dns_domain_record.py` & `pulumi_civo-2.4.0a1713897269/pulumi_civo/dns_domain_record.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1713560943/pulumi_civo/firewall.py` & `pulumi_civo-2.4.0a1713897269/pulumi_civo/firewall.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1713560943/pulumi_civo/firewall_rule.py` & `pulumi_civo-2.4.0a1713897269/pulumi_civo/firewall_rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1713560943/pulumi_civo/get_database.py` & `pulumi_civo-2.4.0a1713897269/pulumi_civo/get_database.py`

 * *Files 1% similar despite different names*

```diff
@@ -219,23 +219,21 @@
     """
     Get information of an Database for use in other resources. This data source provides all of the Database's properties as configured on your Civo account.
 
     Note: This data source returns a single Database. When specifying a name, an error will be raised if more than one Databases with the same name found.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_civo as civo
 
     test = civo.get_database(name="test-database",
         region="LON1")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str id: The ID of the Database
     :param str name: The name of the Database
     :param str region: The region of an existing Database
     """
     __args__ = dict()
@@ -271,23 +269,21 @@
     """
     Get information of an Database for use in other resources. This data source provides all of the Database's properties as configured on your Civo account.
 
     Note: This data source returns a single Database. When specifying a name, an error will be raised if more than one Databases with the same name found.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_civo as civo
 
     test = civo.get_database(name="test-database",
         region="LON1")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str id: The ID of the Database
     :param str name: The name of the Database
     :param str region: The region of an existing Database
     """
     ...
```

### Comparing `pulumi_civo-2.4.0a1713560943/pulumi_civo/get_database_version.py` & `pulumi_civo-2.4.0a1713897269/pulumi_civo/get_database_version.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1713560943/pulumi_civo/get_disk_image.py` & `pulumi_civo-2.4.0a1713897269/pulumi_civo/get_disk_image.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1713560943/pulumi_civo/get_dns_domain_name.py` & `pulumi_civo-2.4.0a1713897269/pulumi_civo/get_dns_domain_name.py`

 * *Files 6% similar despite different names*

```diff
@@ -62,24 +62,22 @@
     """
     Get information on a domain. This data source provides the name and the id.
 
     An error will be raised if the provided domain name is not in your Civo account.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_civo as civo
 
     domain = civo.get_dns_domain_name(name="domain.com")
     pulumi.export("domainOutput", domain.name)
     pulumi.export("domainIdOutput", domain.id)
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str id: The ID of this resource.
     :param str name: The name of the domain
     """
     __args__ = dict()
     __args__['id'] = id
@@ -99,23 +97,21 @@
     """
     Get information on a domain. This data source provides the name and the id.
 
     An error will be raised if the provided domain name is not in your Civo account.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_civo as civo
 
     domain = civo.get_dns_domain_name(name="domain.com")
     pulumi.export("domainOutput", domain.name)
     pulumi.export("domainIdOutput", domain.id)
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str id: The ID of this resource.
     :param str name: The name of the domain
     """
     ...
```

### Comparing `pulumi_civo-2.4.0a1713560943/pulumi_civo/get_dns_domain_record.py` & `pulumi_civo-2.4.0a1713897269/pulumi_civo/get_dns_domain_record.py`

 * *Files 2% similar despite different names*

```diff
@@ -158,26 +158,24 @@
     """
     Get information on a DNS record. This data source provides the name, TTL, and zone file as configured on your Civo account.
 
     An error will be raised if the provided domain name or record are not in your Civo account.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_civo as civo
 
     domain = civo.get_dns_domain_name(name="domain.com")
     www = civo.get_dns_domain_record(domain_id=domain.id,
         name="www")
     pulumi.export("recordType", www.type)
     pulumi.export("recordTtl", www.ttl)
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str domain_id: The ID of the domain
     :param str name: The name of the record
     """
     __args__ = dict()
     __args__['domainId'] = domain_id
@@ -205,25 +203,23 @@
     """
     Get information on a DNS record. This data source provides the name, TTL, and zone file as configured on your Civo account.
 
     An error will be raised if the provided domain name or record are not in your Civo account.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_civo as civo
 
     domain = civo.get_dns_domain_name(name="domain.com")
     www = civo.get_dns_domain_record(domain_id=domain.id,
         name="www")
     pulumi.export("recordType", www.type)
     pulumi.export("recordTtl", www.ttl)
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str domain_id: The ID of the domain
     :param str name: The name of the record
     """
     ...
```

### Comparing `pulumi_civo-2.4.0a1713560943/pulumi_civo/get_firewall.py` & `pulumi_civo-2.4.0a1713897269/pulumi_civo/get_firewall.py`

 * *Files 6% similar despite different names*

```diff
@@ -89,23 +89,21 @@
 
     This data source provides all of the firewall's properties as configured on your Civo account.
 
     Firewalls may be looked up by id or name, and you can optionally pass region if you want to make a lookup for a specific firewall inside that region.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_civo as civo
 
     test = civo.get_firewall(name="test-firewall",
         region="LON1")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str id: The ID of this resource.
     :param str name: The name of the firewall
     :param str region: The region where the firewall is
     """
     __args__ = dict()
@@ -132,23 +130,21 @@
 
     This data source provides all of the firewall's properties as configured on your Civo account.
 
     Firewalls may be looked up by id or name, and you can optionally pass region if you want to make a lookup for a specific firewall inside that region.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_civo as civo
 
     test = civo.get_firewall(name="test-firewall",
         region="LON1")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str id: The ID of this resource.
     :param str name: The name of the firewall
     :param str region: The region where the firewall is
     """
     ...
```

### Comparing `pulumi_civo-2.4.0a1713560943/pulumi_civo/get_instance.py` & `pulumi_civo-2.4.0a1713897269/pulumi_civo/get_instance.py`

 * *Files 2% similar despite different names*

```diff
@@ -303,23 +303,21 @@
     """
     Get information on an instance for use in other resources. This data source provides all of the instance's properties as configured on your Civo account.
 
     Note: This data source returns a single instance. When specifying a hostname, an error will be raised if more than one instances found.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_civo as civo
 
     myhostaname = civo.get_instance(hostname="myhostname.com")
     pulumi.export("instanceOutput", myhostaname.public_ip)
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str hostname: The hostname of the Instance
     :param str id: The ID of this resource.
     :param str region: The region of an existing Instance
     """
     __args__ = dict()
@@ -362,23 +360,21 @@
     """
     Get information on an instance for use in other resources. This data source provides all of the instance's properties as configured on your Civo account.
 
     Note: This data source returns a single instance. When specifying a hostname, an error will be raised if more than one instances found.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_civo as civo
 
     myhostaname = civo.get_instance(hostname="myhostname.com")
     pulumi.export("instanceOutput", myhostaname.public_ip)
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str hostname: The hostname of the Instance
     :param str id: The ID of this resource.
     :param str region: The region of an existing Instance
     """
     ...
```

### Comparing `pulumi_civo-2.4.0a1713560943/pulumi_civo/get_instances.py` & `pulumi_civo-2.4.0a1713897269/pulumi_civo/get_instances.py`

 * *Files 6% similar despite different names*

```diff
@@ -98,29 +98,28 @@
     """
     Get information on instances for use in other resources, with the ability to filter and sort the results. If no filters are specified, all instances will be returned.
 
     Note: You can use the `Instance` data source to obtain metadata about a single instance if you already know the id, unique hostname, or unique tag to retrieve.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_civo as civo
 
     small_size = civo.get_instances(region="LON1",
         filters=[civo.GetInstancesFilterArgs(
             key="size",
             values=[small],
         )])
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param Sequence[pulumi.InputType['GetInstancesFilterArgs']] filters: One or more key/value pairs on which to filter results
+    :param str region: If used, all instances will be from the provided region
     :param Sequence[pulumi.InputType['GetInstancesSortArgs']] sorts: One or more key/direction pairs on which to sort results
     """
     __args__ = dict()
     __args__['filters'] = filters
     __args__['region'] = region
     __args__['sorts'] = sorts
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
@@ -142,25 +141,24 @@
     """
     Get information on instances for use in other resources, with the ability to filter and sort the results. If no filters are specified, all instances will be returned.
 
     Note: You can use the `Instance` data source to obtain metadata about a single instance if you already know the id, unique hostname, or unique tag to retrieve.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_civo as civo
 
     small_size = civo.get_instances(region="LON1",
         filters=[civo.GetInstancesFilterArgs(
             key="size",
             values=[small],
         )])
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param Sequence[pulumi.InputType['GetInstancesFilterArgs']] filters: One or more key/value pairs on which to filter results
+    :param str region: If used, all instances will be from the provided region
     :param Sequence[pulumi.InputType['GetInstancesSortArgs']] sorts: One or more key/direction pairs on which to sort results
     """
     ...
```

### Comparing `pulumi_civo-2.4.0a1713560943/pulumi_civo/get_kubernetes_cluster.py` & `pulumi_civo-2.4.0a1713897269/pulumi_civo/get_kubernetes_cluster.py`

 * *Files 1% similar despite different names*

```diff
@@ -256,23 +256,21 @@
     """
     Provides a Civo Kubernetes cluster data source.
 
     Note: This data source returns a single Kubernetes cluster. When specifying a name, an error will be raised if more than one Kubernetes cluster found.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_civo as civo
 
     my_cluster = civo.get_kubernetes_cluster(name="my-super-cluster")
     pulumi.export("kubernetesClusterOutput", my_cluster.master_ip)
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str id: The ID of this resource.
     :param str name: The name of the Kubernetes Cluster
     :param str region: The region where cluster is running
     """
     __args__ = dict()
@@ -311,23 +309,21 @@
     """
     Provides a Civo Kubernetes cluster data source.
 
     Note: This data source returns a single Kubernetes cluster. When specifying a name, an error will be raised if more than one Kubernetes cluster found.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_civo as civo
 
     my_cluster = civo.get_kubernetes_cluster(name="my-super-cluster")
     pulumi.export("kubernetesClusterOutput", my_cluster.master_ip)
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str id: The ID of this resource.
     :param str name: The name of the Kubernetes Cluster
     :param str region: The region where cluster is running
     """
     ...
```

### Comparing `pulumi_civo-2.4.0a1713560943/pulumi_civo/get_kubernetes_version.py` & `pulumi_civo-2.4.0a1713897269/pulumi_civo/get_kubernetes_version.py`

 * *Files 4% similar despite different names*

```diff
@@ -83,29 +83,27 @@
                            sorts: Optional[Sequence[pulumi.InputType['GetKubernetesVersionSortArgs']]] = None,
                            opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetKubernetesVersionResult:
     """
     Provides access to the available Civo Kubernetes versions, with the ability to filter the results.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_civo as civo
 
     talos = civo.get_kubernetes_version(filters=[civo.GetKubernetesVersionFilterArgs(
         key="type",
         values=["talos"],
     )])
     k3s = civo.get_kubernetes_version(filters=[civo.GetKubernetesVersionFilterArgs(
         key="type",
         values=["k3s"],
     )])
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param Sequence[pulumi.InputType['GetKubernetesVersionFilterArgs']] filters: One or more key/value pairs on which to filter results
     :param Sequence[pulumi.InputType['GetKubernetesVersionSortArgs']] sorts: One or more key/direction pairs on which to sort results
     """
     __args__ = dict()
     __args__['filters'] = filters
@@ -125,28 +123,26 @@
                                   sorts: Optional[pulumi.Input[Optional[Sequence[pulumi.InputType['GetKubernetesVersionSortArgs']]]]] = None,
                                   opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetKubernetesVersionResult]:
     """
     Provides access to the available Civo Kubernetes versions, with the ability to filter the results.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_civo as civo
 
     talos = civo.get_kubernetes_version(filters=[civo.GetKubernetesVersionFilterArgs(
         key="type",
         values=["talos"],
     )])
     k3s = civo.get_kubernetes_version(filters=[civo.GetKubernetesVersionFilterArgs(
         key="type",
         values=["k3s"],
     )])
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param Sequence[pulumi.InputType['GetKubernetesVersionFilterArgs']] filters: One or more key/value pairs on which to filter results
     :param Sequence[pulumi.InputType['GetKubernetesVersionSortArgs']] sorts: One or more key/direction pairs on which to sort results
     """
     ...
```

### Comparing `pulumi_civo-2.4.0a1713560943/pulumi_civo/get_load_balancer.py` & `pulumi_civo-2.4.0a1713897269/pulumi_civo/get_load_balancer.py`

 * *Files 2% similar despite different names*

```diff
@@ -205,25 +205,23 @@
     """
     Get information on a load balancer for use in other resources. This data source provides all of the load balancers properties as configured on your Civo account.
 
     An error will be raised if the provided load balancer name does not exist in your Civo account.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_civo as civo
 
     # TODO
     my_lb = civo.get_load_balancer(name="lb-name",
         region="LON1")
     pulumi.export("civoLoadbalancerOutput", my_lb.public_ip)
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str id: The id of the load balancer to retrieve (You can find this id from service annotations 'kubernetes.civo.com/loadbalancer-id')
     :param str name: The name of the load balancer (You can find this name from service annotations 'kubernetes.civo.com/loadbalancer-name')
     :param str region: The region of the load balancer, if you declare this field, the datasource will use this value instead of the one defined in the provider
     """
     __args__ = dict()
@@ -258,25 +256,23 @@
     """
     Get information on a load balancer for use in other resources. This data source provides all of the load balancers properties as configured on your Civo account.
 
     An error will be raised if the provided load balancer name does not exist in your Civo account.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_civo as civo
 
     # TODO
     my_lb = civo.get_load_balancer(name="lb-name",
         region="LON1")
     pulumi.export("civoLoadbalancerOutput", my_lb.public_ip)
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str id: The id of the load balancer to retrieve (You can find this id from service annotations 'kubernetes.civo.com/loadbalancer-id')
     :param str name: The name of the load balancer (You can find this name from service annotations 'kubernetes.civo.com/loadbalancer-name')
     :param str region: The region of the load balancer, if you declare this field, the datasource will use this value instead of the one defined in the provider
     """
     ...
```

### Comparing `pulumi_civo-2.4.0a1713560943/pulumi_civo/get_network.py` & `pulumi_civo-2.4.0a1713897269/pulumi_civo/get_network.py`

 * *Files 6% similar despite different names*

```diff
@@ -101,23 +101,21 @@
 
     This data source provides all of the network's properties as configured on your Civo account.
 
     Networks may be looked up by id or label, and you can optionally pass region if you want to make a lookup for a specific network inside that region.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_civo as civo
 
     test = civo.get_network(label="test-network",
         region="LON1")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str id: The ID of this resource.
     :param str label: The label of an existing network
     :param str region: The region of an existing network
     """
     __args__ = dict()
@@ -145,23 +143,21 @@
 
     This data source provides all of the network's properties as configured on your Civo account.
 
     Networks may be looked up by id or label, and you can optionally pass region if you want to make a lookup for a specific network inside that region.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_civo as civo
 
     test = civo.get_network(label="test-network",
         region="LON1")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str id: The ID of this resource.
     :param str label: The label of an existing network
     :param str region: The region of an existing network
     """
     ...
```

### Comparing `pulumi_civo-2.4.0a1713560943/pulumi_civo/get_object_store.py` & `pulumi_civo-2.4.0a1713897269/pulumi_civo/get_object_store.py`

 * *Files 3% similar despite different names*

```diff
@@ -123,22 +123,20 @@
     """
     Get information of an Object Store for use in other resources. This data source provides all of the Object Store's properties as configured on your Civo account.
 
     Note: This data source returns a single Object Store. When specifying a name, an error will be raised if more than one Object Stores with the same name found.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_civo as civo
 
     backup = civo.get_object_store(name="backup-server")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str id: The ID of the Object Store
     :param str name: The name of the Object Store
     :param str region: The region of an existing Object Store
     """
     __args__ = dict()
@@ -166,22 +164,20 @@
     """
     Get information of an Object Store for use in other resources. This data source provides all of the Object Store's properties as configured on your Civo account.
 
     Note: This data source returns a single Object Store. When specifying a name, an error will be raised if more than one Object Stores with the same name found.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_civo as civo
 
     backup = civo.get_object_store(name="backup-server")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str id: The ID of the Object Store
     :param str name: The name of the Object Store
     :param str region: The region of an existing Object Store
     """
     ...
```

### Comparing `pulumi_civo-2.4.0a1713560943/pulumi_civo/get_object_store_credential.py` & `pulumi_civo-2.4.0a1713897269/pulumi_civo/get_object_store_credential.py`

 * *Files 5% similar despite different names*

```diff
@@ -111,29 +111,27 @@
     """
     Get information of an Object Store Credential for use in other resources. This data source provides all of the Object Store Credential's properties as configured on your Civo account.
 
     Note: This data source returns a single Object Store Credential. When specifying a name, an error will be raised if more than one Object Store Credentials with the same name found.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_civo as civo
 
     # Read a credential for the object store
     backup = civo.get_object_store_credential(name="backup-server")
     # Use the credential to create a bucket
     backup_object_store = civo.ObjectStore("backup",
         name="backup-server",
         max_size_gb=500,
         region="LON1",
         access_key_id=backup.access_key_id)
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str id: The ID of the Object Store Credential
     :param str name: The name of the Object Store Credential
     :param str region: The region of an existing Object Store
     """
     __args__ = dict()
@@ -160,29 +158,27 @@
     """
     Get information of an Object Store Credential for use in other resources. This data source provides all of the Object Store Credential's properties as configured on your Civo account.
 
     Note: This data source returns a single Object Store Credential. When specifying a name, an error will be raised if more than one Object Store Credentials with the same name found.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_civo as civo
 
     # Read a credential for the object store
     backup = civo.get_object_store_credential(name="backup-server")
     # Use the credential to create a bucket
     backup_object_store = civo.ObjectStore("backup",
         name="backup-server",
         max_size_gb=500,
         region="LON1",
         access_key_id=backup.access_key_id)
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str id: The ID of the Object Store Credential
     :param str name: The name of the Object Store Credential
     :param str region: The region of an existing Object Store
     """
     ...
```

### Comparing `pulumi_civo-2.4.0a1713560943/pulumi_civo/get_region.py` & `pulumi_civo-2.4.0a1713897269/pulumi_civo/get_region.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1713560943/pulumi_civo/get_reserved_ip.py` & `pulumi_civo-2.4.0a1713897269/pulumi_civo/get_reserved_ip.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1713560943/pulumi_civo/get_size.py` & `pulumi_civo-2.4.0a1713897269/pulumi_civo/get_size.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1713560943/pulumi_civo/get_ssh_key.py` & `pulumi_civo-2.4.0a1713897269/pulumi_civo/get_ssh_key.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1713560943/pulumi_civo/get_volume.py` & `pulumi_civo-2.4.0a1713897269/pulumi_civo/get_volume.py`

 * *Files 6% similar despite different names*

```diff
@@ -111,23 +111,21 @@
     """
     Get information on a volume for use in other resources. This data source provides all of the volumes properties as configured on your Civo account.
 
     An error will be raised if the provided volume name does not exist in your Civo account.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_civo as civo
 
     myvolume = civo.get_volume(name="test-volume-name")
     pulumi.export("volumeOutput", myvolume)
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str id: The ID of this resource.
     :param str name: The name of the volume
     :param str region: The region where volume is running
     """
     __args__ = dict()
@@ -154,23 +152,21 @@
     """
     Get information on a volume for use in other resources. This data source provides all of the volumes properties as configured on your Civo account.
 
     An error will be raised if the provided volume name does not exist in your Civo account.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_civo as civo
 
     myvolume = civo.get_volume(name="test-volume-name")
     pulumi.export("volumeOutput", myvolume)
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str id: The ID of this resource.
     :param str name: The name of the volume
     :param str region: The region where volume is running
     """
     ...
```

### Comparing `pulumi_civo-2.4.0a1713560943/pulumi_civo/instance.py` & `pulumi_civo-2.4.0a1713897269/pulumi_civo/instance.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1713560943/pulumi_civo/instance_reserved_ip_assignment.py` & `pulumi_civo-2.4.0a1713897269/pulumi_civo/instance_reserved_ip_assignment.py`

 * *Files 1% similar despite different names*

```diff
@@ -131,27 +131,25 @@
                  reserved_ip_id: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         The instance reserved ip assignment resource schema definition
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_civo as civo
 
         # Send to create a reserved IP
         www = civo.ReservedIp("www", name="nginx-www")
         # We assign the reserved IP to the instance
         webserver_www = civo.InstanceReservedIpAssignment("webserver-www",
             instance_id=www_civo_instance["id"],
             reserved_ip_id=web_server["id"])
         ```
-        <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] instance_id: The instance id
         :param pulumi.Input[str] region: The region of the ip
         :param pulumi.Input[str] reserved_ip_id: The reserved ip id
         """
@@ -162,27 +160,25 @@
                  args: InstanceReservedIpAssignmentArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         The instance reserved ip assignment resource schema definition
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_civo as civo
 
         # Send to create a reserved IP
         www = civo.ReservedIp("www", name="nginx-www")
         # We assign the reserved IP to the instance
         webserver_www = civo.InstanceReservedIpAssignment("webserver-www",
             instance_id=www_civo_instance["id"],
             reserved_ip_id=web_server["id"])
         ```
-        <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param InstanceReservedIpAssignmentArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
```

### Comparing `pulumi_civo-2.4.0a1713560943/pulumi_civo/kubernetes_cluster.py` & `pulumi_civo-2.4.0a1713897269/pulumi_civo/kubernetes_cluster.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1713560943/pulumi_civo/kubernetes_node_pool.py` & `pulumi_civo-2.4.0a1713897269/pulumi_civo/kubernetes_node_pool.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1713560943/pulumi_civo/network.py` & `pulumi_civo-2.4.0a1713897269/pulumi_civo/network.py`

 * *Files 2% similar despite different names*

```diff
@@ -131,22 +131,20 @@
                  region: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         Provides a Civo network resource. This can be used to create, modify, and delete networks.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_civo as civo
 
         custom_net = civo.Network("custom_net", label="test_network")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         using ID
 
         ```sh
         $ pulumi import civo:index/network:Network custom_net b8ecd2ab-2267-4a5e-8692-cbf1d32583e3
@@ -164,22 +162,20 @@
                  args: NetworkArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         Provides a Civo network resource. This can be used to create, modify, and delete networks.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_civo as civo
 
         custom_net = civo.Network("custom_net", label="test_network")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         using ID
 
         ```sh
         $ pulumi import civo:index/network:Network custom_net b8ecd2ab-2267-4a5e-8692-cbf1d32583e3
```

### Comparing `pulumi_civo-2.4.0a1713560943/pulumi_civo/object_store.py` & `pulumi_civo-2.4.0a1713897269/pulumi_civo/object_store.py`

 * *Files 3% similar despite different names*

```diff
@@ -198,27 +198,25 @@
                  region: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         Provides an Object Store resource. This can be used to create, modify, and delete object stores.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_civo as civo
 
         backup_object_store = civo.ObjectStore("backup",
             name="backup-server",
             max_size_gb=500,
             region="LON1")
         # If you create the bucket without credentials, you can read the credentials in this way
         backup = civo.get_object_store_credential_output(id=backup_object_store.access_key_id)
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         using ID
 
         ```sh
         $ pulumi import civo:index/objectStore:ObjectStore custom_object b8ecd2ab-2267-4a5e-8692-cbf1d32583e3
@@ -238,27 +236,25 @@
                  args: Optional[ObjectStoreArgs] = None,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         Provides an Object Store resource. This can be used to create, modify, and delete object stores.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_civo as civo
 
         backup_object_store = civo.ObjectStore("backup",
             name="backup-server",
             max_size_gb=500,
             region="LON1")
         # If you create the bucket without credentials, you can read the credentials in this way
         backup = civo.get_object_store_credential_output(id=backup_object_store.access_key_id)
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         using ID
 
         ```sh
         $ pulumi import civo:index/objectStore:ObjectStore custom_object b8ecd2ab-2267-4a5e-8692-cbf1d32583e3
```

### Comparing `pulumi_civo-2.4.0a1713560943/pulumi_civo/object_store_credential.py` & `pulumi_civo-2.4.0a1713897269/pulumi_civo/object_store_credential.py`

 * *Files 2% similar despite different names*

```diff
@@ -182,15 +182,14 @@
                  secret_access_key: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         Provides an Object Store Credential resource. This can be used to create, modify, and delete object stores credential.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_civo as civo
 
         # Create a simple credential for the object store
         backup = civo.get_object_store_credential(name="backup-server")
         # Create a credential for the object store with a specific access key and secret key
@@ -201,15 +200,14 @@
         # Use the credential to create a bucket
         backup_object_store = civo.ObjectStore("backup",
             name="backup-server",
             max_size_gb=500,
             region="LON1",
             access_key_id=backup_object_store_credential.access_key_id)
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         using ID
 
         ```sh
         $ pulumi import civo:index/objectStoreCredential:ObjectStoreCredential custom_object b8ecd2ab-2267-4a5e-8692-cbf1d32583e3
@@ -229,15 +227,14 @@
                  args: Optional[ObjectStoreCredentialArgs] = None,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         Provides an Object Store Credential resource. This can be used to create, modify, and delete object stores credential.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_civo as civo
 
         # Create a simple credential for the object store
         backup = civo.get_object_store_credential(name="backup-server")
         # Create a credential for the object store with a specific access key and secret key
@@ -248,15 +245,14 @@
         # Use the credential to create a bucket
         backup_object_store = civo.ObjectStore("backup",
             name="backup-server",
             max_size_gb=500,
             region="LON1",
             access_key_id=backup_object_store_credential.access_key_id)
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         using ID
 
         ```sh
         $ pulumi import civo:index/objectStoreCredential:ObjectStoreCredential custom_object b8ecd2ab-2267-4a5e-8692-cbf1d32583e3
```

### Comparing `pulumi_civo-2.4.0a1713560943/pulumi_civo/outputs.py` & `pulumi_civo-2.4.0a1713897269/pulumi_civo/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1713560943/pulumi_civo/provider.py` & `pulumi_civo-2.4.0a1713897269/pulumi_civo/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1713560943/pulumi_civo/reserved_ip.py` & `pulumi_civo-2.4.0a1713897269/pulumi_civo/reserved_ip.py`

 * *Files 2% similar despite different names*

```diff
@@ -116,22 +116,20 @@
                  region: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         Provides a Civo reserved IP to represent a publicly-accessible static IP addresses that can be mapped to one of your Instancesor Load Balancer.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_civo as civo
 
         www = civo.ReservedIp("www", name="nginx-www")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         terrafom import civo_reserved_ip.www 9f0e86fc-b2c6-46b4-82ed-2f28419f8ae3
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
@@ -145,22 +143,20 @@
                  args: Optional[ReservedIpArgs] = None,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         Provides a Civo reserved IP to represent a publicly-accessible static IP addresses that can be mapped to one of your Instancesor Load Balancer.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_civo as civo
 
         www = civo.ReservedIp("www", name="nginx-www")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         terrafom import civo_reserved_ip.www 9f0e86fc-b2c6-46b4-82ed-2f28419f8ae3
 
         :param str resource_name: The name of the resource.
         :param ReservedIpArgs args: The arguments to use to populate this resource's properties.
```

### Comparing `pulumi_civo-2.4.0a1713560943/pulumi_civo/ssh_key.py` & `pulumi_civo-2.4.0a1713897269/pulumi_civo/ssh_key.py`

 * *Files 2% similar despite different names*

```diff
@@ -115,25 +115,23 @@
                  public_key: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         Provides a Civo SSH key resource to allow you to manage SSH keys for instance access. Keys created with this resource can be referenced in your instance configuration via their ID.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_civo as civo
         import pulumi_std as std
 
         my_user = civo.SshKey("my-user",
             name="my-user",
             public_key=std.file(input="~/.ssh/id_rsa.pub").result)
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         using ID
 
         ```sh
         $ pulumi import civo:index/sshKey:SshKey mykey 87ca2ee4-57d3-4420-b9b6-411b0b4b2a0e
@@ -151,25 +149,23 @@
                  args: SshKeyArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         Provides a Civo SSH key resource to allow you to manage SSH keys for instance access. Keys created with this resource can be referenced in your instance configuration via their ID.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_civo as civo
         import pulumi_std as std
 
         my_user = civo.SshKey("my-user",
             name="my-user",
             public_key=std.file(input="~/.ssh/id_rsa.pub").result)
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         using ID
 
         ```sh
         $ pulumi import civo:index/sshKey:SshKey mykey 87ca2ee4-57d3-4420-b9b6-411b0b4b2a0e
```

### Comparing `pulumi_civo-2.4.0a1713560943/pulumi_civo/volume.py` & `pulumi_civo-2.4.0a1713897269/pulumi_civo/volume.py`

 * *Files 2% similar despite different names*

```diff
@@ -180,29 +180,27 @@
                  size_gb: Optional[pulumi.Input[int]] = None,
                  __props__=None):
         """
         Provides a Civo volume which can be attached to an instance in order to provide expanded storage.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_civo as civo
 
         # Get network
         default_network = civo.get_network(label="Default")
         # Create volume
         db = civo.Volume("db",
             name="backup-data",
             size_gb=5,
             network_id=default_network.id,
             opts=pulumi.ResourceOptions(depends_on=[default_network]))
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         using ID
 
         ```sh
         $ pulumi import civo:index/volume:Volume db 506f78a4-e098-11e5-ad9f-000f53306ae1
@@ -222,29 +220,27 @@
                  args: VolumeArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         Provides a Civo volume which can be attached to an instance in order to provide expanded storage.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_civo as civo
 
         # Get network
         default_network = civo.get_network(label="Default")
         # Create volume
         db = civo.Volume("db",
             name="backup-data",
             size_gb=5,
             network_id=default_network.id,
             opts=pulumi.ResourceOptions(depends_on=[default_network]))
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         using ID
 
         ```sh
         $ pulumi import civo:index/volume:Volume db 506f78a4-e098-11e5-ad9f-000f53306ae1
```

### Comparing `pulumi_civo-2.4.0a1713560943/pulumi_civo/volume_attachment.py` & `pulumi_civo-2.4.0a1713897269/pulumi_civo/volume_attachment.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1713560943/pulumi_civo.egg-info/PKG-INFO` & `pulumi_civo-2.4.0a1713897269/pulumi_civo.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_civo
-Version: 2.4.0a1713560943
+Version: 2.4.0a1713897269
 Summary: A Pulumi package for creating and managing Civo cloud resources.
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.io
 Project-URL: Repository, https://github.com/pulumi/pulumi-civo
 Keywords: pulumi,civo
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_civo-2.4.0a1713560943/pulumi_civo.egg-info/SOURCES.txt` & `pulumi_civo-2.4.0a1713897269/pulumi_civo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1713560943/pyproject.toml` & `pulumi_civo-2.4.0a1713897269/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [project]
   name = "pulumi_civo"
   description = "A Pulumi package for creating and managing Civo cloud resources."
   dependencies = ["parver>=0.2.1", "pulumi>=3.0.0,<4.0.0", "semver>=2.8.1"]
   keywords = ["pulumi", "civo"]
   readme = "README.md"
   requires-python = ">=3.8"
-  version = "2.4.0a1713560943"
+  version = "2.4.0a1713897269"
   [project.license]
     text = "Apache-2.0"
   [project.urls]
     Homepage = "https://pulumi.io"
     Repository = "https://github.com/pulumi/pulumi-civo"
 
 [build-system]
```

