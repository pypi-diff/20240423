# Comparing `tmp/cdktf-cdktf-provider-dns-8.0.0.tar.gz` & `tmp/cdktf-cdktf-provider-dns-8.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdktf-cdktf-provider-dns-8.0.0.tar", last modified: Wed Jan 10 11:24:22 2024, max compression
+gzip compressed data, was "cdktf-cdktf-provider-dns-8.0.1.tar", last modified: Tue Apr 23 03:12:00 2024, max compression
```

## Comparing `cdktf-cdktf-provider-dns-8.0.0.tar` & `cdktf-cdktf-provider-dns-8.0.1.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 11:24:22.811778 cdktf-cdktf-provider-dns-8.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)    16012 2024-01-10 11:24:08.000000 cdktf-cdktf-provider-dns-8.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-01-10 11:24:08.000000 cdktf-cdktf-provider-dns-8.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4121 2024-01-10 11:24:22.811778 cdktf-cdktf-provider-dns-8.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3231 2024-01-10 11:24:08.000000 cdktf-cdktf-provider-dns-8.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-01-10 11:24:08.000000 cdktf-cdktf-provider-dns-8.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-10 11:24:22.811778 cdktf-cdktf-provider-dns-8.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2690 2024-01-10 11:24:08.000000 cdktf-cdktf-provider-dns-8.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 11:24:22.803778 cdktf-cdktf-provider-dns-8.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 11:24:22.807778 cdktf-cdktf-provider-dns-8.0.0/src/cdktf_cdktf_provider_dns/
--rw-r--r--   0 runner    (1001) docker     (127)     4524 2024-01-10 11:24:08.000000 cdktf-cdktf-provider-dns-8.0.0/src/cdktf_cdktf_provider_dns/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 11:24:22.807778 cdktf-cdktf-provider-dns-8.0.0/src/cdktf_cdktf_provider_dns/_jsii/
--rw-r--r--   0 runner    (1001) docker     (127)      396 2024-01-10 11:24:08.000000 cdktf-cdktf-provider-dns-8.0.0/src/cdktf_cdktf_provider_dns/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    91743 2024-01-10 11:24:08.000000 cdktf-cdktf-provider-dns-8.0.0/src/cdktf_cdktf_provider_dns/_jsii/provider-dns@8.0.0.jsii.tgz
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 11:24:22.807778 cdktf-cdktf-provider-dns-8.0.0/src/cdktf_cdktf_provider_dns/a_record_set/
--rw-r--r--   0 runner    (1001) docker     (127)    27229 2024-01-10 11:24:08.000000 cdktf-cdktf-provider-dns-8.0.0/src/cdktf_cdktf_provider_dns/a_record_set/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 11:24:22.807778 cdktf-cdktf-provider-dns-8.0.0/src/cdktf_cdktf_provider_dns/aaaa_record_set/
--rw-r--r--   0 runner    (1001) docker     (127)    27385 2024-01-10 11:24:08.000000 cdktf-cdktf-provider-dns-8.0.0/src/cdktf_cdktf_provider_dns/aaaa_record_set/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 11:24:22.811778 cdktf-cdktf-provider-dns-8.0.0/src/cdktf_cdktf_provider_dns/cname_record/
--rw-r--r--   0 runner    (1001) docker     (127)    23843 2024-01-10 11:24:08.000000 cdktf-cdktf-provider-dns-8.0.0/src/cdktf_cdktf_provider_dns/cname_record/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 11:24:22.811778 cdktf-cdktf-provider-dns-8.0.0/src/cdktf_cdktf_provider_dns/data_dns_a_record_set/
--rw-r--r--   0 runner    (1001) docker     (127)    17416 2024-01-10 11:24:08.000000 cdktf-cdktf-provider-dns-8.0.0/src/cdktf_cdktf_provider_dns/data_dns_a_record_set/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 11:24:22.811778 cdktf-cdktf-provider-dns-8.0.0/src/cdktf_cdktf_provider_dns/data_dns_aaaa_record_set/
--rw-r--r--   0 runner    (1001) docker     (127)    17500 2024-01-10 11:24:08.000000 cdktf-cdktf-provider-dns-8.0.0/src/cdktf_cdktf_provider_dns/data_dns_aaaa_record_set/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 11:24:22.811778 cdktf-cdktf-provider-dns-8.0.0/src/cdktf_cdktf_provider_dns/data_dns_cname_record_set/
--rw-r--r--   0 runner    (1001) docker     (127)    17502 2024-01-10 11:24:08.000000 cdktf-cdktf-provider-dns-8.0.0/src/cdktf_cdktf_provider_dns/data_dns_cname_record_set/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 11:24:22.811778 cdktf-cdktf-provider-dns-8.0.0/src/cdktf_cdktf_provider_dns/data_dns_mx_record_set/
--rw-r--r--   0 runner    (1001) docker     (127)    26356 2024-01-10 11:24:08.000000 cdktf-cdktf-provider-dns-8.0.0/src/cdktf_cdktf_provider_dns/data_dns_mx_record_set/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 11:24:22.811778 cdktf-cdktf-provider-dns-8.0.0/src/cdktf_cdktf_provider_dns/data_dns_ns_record_set/
--rw-r--r--   0 runner    (1001) docker     (127)    17462 2024-01-10 11:24:08.000000 cdktf-cdktf-provider-dns-8.0.0/src/cdktf_cdktf_provider_dns/data_dns_ns_record_set/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 11:24:22.811778 cdktf-cdktf-provider-dns-8.0.0/src/cdktf_cdktf_provider_dns/data_dns_ptr_record_set/
--rw-r--r--   0 runner    (1001) docker     (127)    17650 2024-01-10 11:24:08.000000 cdktf-cdktf-provider-dns-8.0.0/src/cdktf_cdktf_provider_dns/data_dns_ptr_record_set/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 11:24:22.811778 cdktf-cdktf-provider-dns-8.0.0/src/cdktf_cdktf_provider_dns/data_dns_srv_record_set/
--rw-r--r--   0 runner    (1001) docker     (127)    26772 2024-01-10 11:24:08.000000 cdktf-cdktf-provider-dns-8.0.0/src/cdktf_cdktf_provider_dns/data_dns_srv_record_set/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 11:24:22.811778 cdktf-cdktf-provider-dns-8.0.0/src/cdktf_cdktf_provider_dns/data_dns_txt_record_set/
--rw-r--r--   0 runner    (1001) docker     (127)    17644 2024-01-10 11:24:08.000000 cdktf-cdktf-provider-dns-8.0.0/src/cdktf_cdktf_provider_dns/data_dns_txt_record_set/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 11:24:22.811778 cdktf-cdktf-provider-dns-8.0.0/src/cdktf_cdktf_provider_dns/mx_record_set/
--rw-r--r--   0 runner    (1001) docker     (127)    38955 2024-01-10 11:24:08.000000 cdktf-cdktf-provider-dns-8.0.0/src/cdktf_cdktf_provider_dns/mx_record_set/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 11:24:22.811778 cdktf-cdktf-provider-dns-8.0.0/src/cdktf_cdktf_provider_dns/ns_record_set/
--rw-r--r--   0 runner    (1001) docker     (127)    24260 2024-01-10 11:24:08.000000 cdktf-cdktf-provider-dns-8.0.0/src/cdktf_cdktf_provider_dns/ns_record_set/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 11:24:22.811778 cdktf-cdktf-provider-dns-8.0.0/src/cdktf_cdktf_provider_dns/provider/
--rw-r--r--   0 runner    (1001) docker     (127)    28895 2024-01-10 11:24:08.000000 cdktf-cdktf-provider-dns-8.0.0/src/cdktf_cdktf_provider_dns/provider/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 11:24:22.811778 cdktf-cdktf-provider-dns-8.0.0/src/cdktf_cdktf_provider_dns/ptr_record/
--rw-r--r--   0 runner    (1001) docker     (127)    23929 2024-01-10 11:24:08.000000 cdktf-cdktf-provider-dns-8.0.0/src/cdktf_cdktf_provider_dns/ptr_record/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-10 11:24:08.000000 cdktf-cdktf-provider-dns-8.0.0/src/cdktf_cdktf_provider_dns/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 11:24:22.811778 cdktf-cdktf-provider-dns-8.0.0/src/cdktf_cdktf_provider_dns/srv_record_set/
--rw-r--r--   0 runner    (1001) docker     (127)    42301 2024-01-10 11:24:08.000000 cdktf-cdktf-provider-dns-8.0.0/src/cdktf_cdktf_provider_dns/srv_record_set/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 11:24:22.811778 cdktf-cdktf-provider-dns-8.0.0/src/cdktf_cdktf_provider_dns/txt_record_set/
--rw-r--r--   0 runner    (1001) docker     (127)    24292 2024-01-10 11:24:08.000000 cdktf-cdktf-provider-dns-8.0.0/src/cdktf_cdktf_provider_dns/txt_record_set/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 11:24:22.807778 cdktf-cdktf-provider-dns-8.0.0/src/cdktf_cdktf_provider_dns.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4121 2024-01-10 11:24:22.000000 cdktf-cdktf-provider-dns-8.0.0/src/cdktf_cdktf_provider_dns.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-01-10 11:24:22.000000 cdktf-cdktf-provider-dns-8.0.0/src/cdktf_cdktf_provider_dns.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-10 11:24:22.000000 cdktf-cdktf-provider-dns-8.0.0/src/cdktf_cdktf_provider_dns.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-01-10 11:24:22.000000 cdktf-cdktf-provider-dns-8.0.0/src/cdktf_cdktf_provider_dns.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-01-10 11:24:22.000000 cdktf-cdktf-provider-dns-8.0.0/src/cdktf_cdktf_provider_dns.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 03:12:00.400456 cdktf-cdktf-provider-dns-8.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    16012 2024-04-23 03:11:48.000000 cdktf-cdktf-provider-dns-8.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-23 03:11:48.000000 cdktf-cdktf-provider-dns-8.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4356 2024-04-23 03:12:00.400456 cdktf-cdktf-provider-dns-8.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3466 2024-04-23 03:11:48.000000 cdktf-cdktf-provider-dns-8.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-23 03:11:48.000000 cdktf-cdktf-provider-dns-8.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 03:12:00.400456 cdktf-cdktf-provider-dns-8.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2690 2024-04-23 03:11:48.000000 cdktf-cdktf-provider-dns-8.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 03:12:00.392456 cdktf-cdktf-provider-dns-8.0.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 03:12:00.396456 cdktf-cdktf-provider-dns-8.0.1/src/cdktf_cdktf_provider_dns/
+-rw-r--r--   0 runner    (1001) docker     (127)     4835 2024-04-23 03:11:48.000000 cdktf-cdktf-provider-dns-8.0.1/src/cdktf_cdktf_provider_dns/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 03:12:00.396456 cdktf-cdktf-provider-dns-8.0.1/src/cdktf_cdktf_provider_dns/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (127)      472 2024-04-23 03:11:48.000000 cdktf-cdktf-provider-dns-8.0.1/src/cdktf_cdktf_provider_dns/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    92118 2024-04-23 03:11:48.000000 cdktf-cdktf-provider-dns-8.0.1/src/cdktf_cdktf_provider_dns/_jsii/provider-dns@8.0.1.jsii.tgz
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 03:12:00.396456 cdktf-cdktf-provider-dns-8.0.1/src/cdktf_cdktf_provider_dns/a_record_set/
+-rw-r--r--   0 runner    (1001) docker     (127)    27305 2024-04-23 03:11:48.000000 cdktf-cdktf-provider-dns-8.0.1/src/cdktf_cdktf_provider_dns/a_record_set/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 03:12:00.396456 cdktf-cdktf-provider-dns-8.0.1/src/cdktf_cdktf_provider_dns/aaaa_record_set/
+-rw-r--r--   0 runner    (1001) docker     (127)    27461 2024-04-23 03:11:48.000000 cdktf-cdktf-provider-dns-8.0.1/src/cdktf_cdktf_provider_dns/aaaa_record_set/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 03:12:00.400456 cdktf-cdktf-provider-dns-8.0.1/src/cdktf_cdktf_provider_dns/cname_record/
+-rw-r--r--   0 runner    (1001) docker     (127)    23919 2024-04-23 03:11:48.000000 cdktf-cdktf-provider-dns-8.0.1/src/cdktf_cdktf_provider_dns/cname_record/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 03:12:00.400456 cdktf-cdktf-provider-dns-8.0.1/src/cdktf_cdktf_provider_dns/data_dns_a_record_set/
+-rw-r--r--   0 runner    (1001) docker     (127)    17492 2024-04-23 03:11:48.000000 cdktf-cdktf-provider-dns-8.0.1/src/cdktf_cdktf_provider_dns/data_dns_a_record_set/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 03:12:00.400456 cdktf-cdktf-provider-dns-8.0.1/src/cdktf_cdktf_provider_dns/data_dns_aaaa_record_set/
+-rw-r--r--   0 runner    (1001) docker     (127)    17576 2024-04-23 03:11:48.000000 cdktf-cdktf-provider-dns-8.0.1/src/cdktf_cdktf_provider_dns/data_dns_aaaa_record_set/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 03:12:00.400456 cdktf-cdktf-provider-dns-8.0.1/src/cdktf_cdktf_provider_dns/data_dns_cname_record_set/
+-rw-r--r--   0 runner    (1001) docker     (127)    17578 2024-04-23 03:11:48.000000 cdktf-cdktf-provider-dns-8.0.1/src/cdktf_cdktf_provider_dns/data_dns_cname_record_set/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 03:12:00.400456 cdktf-cdktf-provider-dns-8.0.1/src/cdktf_cdktf_provider_dns/data_dns_mx_record_set/
+-rw-r--r--   0 runner    (1001) docker     (127)    26432 2024-04-23 03:11:48.000000 cdktf-cdktf-provider-dns-8.0.1/src/cdktf_cdktf_provider_dns/data_dns_mx_record_set/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 03:12:00.400456 cdktf-cdktf-provider-dns-8.0.1/src/cdktf_cdktf_provider_dns/data_dns_ns_record_set/
+-rw-r--r--   0 runner    (1001) docker     (127)    17538 2024-04-23 03:11:48.000000 cdktf-cdktf-provider-dns-8.0.1/src/cdktf_cdktf_provider_dns/data_dns_ns_record_set/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 03:12:00.400456 cdktf-cdktf-provider-dns-8.0.1/src/cdktf_cdktf_provider_dns/data_dns_ptr_record_set/
+-rw-r--r--   0 runner    (1001) docker     (127)    17726 2024-04-23 03:11:48.000000 cdktf-cdktf-provider-dns-8.0.1/src/cdktf_cdktf_provider_dns/data_dns_ptr_record_set/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 03:12:00.400456 cdktf-cdktf-provider-dns-8.0.1/src/cdktf_cdktf_provider_dns/data_dns_srv_record_set/
+-rw-r--r--   0 runner    (1001) docker     (127)    26848 2024-04-23 03:11:48.000000 cdktf-cdktf-provider-dns-8.0.1/src/cdktf_cdktf_provider_dns/data_dns_srv_record_set/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 03:12:00.400456 cdktf-cdktf-provider-dns-8.0.1/src/cdktf_cdktf_provider_dns/data_dns_txt_record_set/
+-rw-r--r--   0 runner    (1001) docker     (127)    17720 2024-04-23 03:11:48.000000 cdktf-cdktf-provider-dns-8.0.1/src/cdktf_cdktf_provider_dns/data_dns_txt_record_set/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 03:12:00.400456 cdktf-cdktf-provider-dns-8.0.1/src/cdktf_cdktf_provider_dns/mx_record_set/
+-rw-r--r--   0 runner    (1001) docker     (127)    39031 2024-04-23 03:11:48.000000 cdktf-cdktf-provider-dns-8.0.1/src/cdktf_cdktf_provider_dns/mx_record_set/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 03:12:00.400456 cdktf-cdktf-provider-dns-8.0.1/src/cdktf_cdktf_provider_dns/ns_record_set/
+-rw-r--r--   0 runner    (1001) docker     (127)    24336 2024-04-23 03:11:48.000000 cdktf-cdktf-provider-dns-8.0.1/src/cdktf_cdktf_provider_dns/ns_record_set/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 03:12:00.400456 cdktf-cdktf-provider-dns-8.0.1/src/cdktf_cdktf_provider_dns/provider/
+-rw-r--r--   0 runner    (1001) docker     (127)    28971 2024-04-23 03:11:48.000000 cdktf-cdktf-provider-dns-8.0.1/src/cdktf_cdktf_provider_dns/provider/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 03:12:00.400456 cdktf-cdktf-provider-dns-8.0.1/src/cdktf_cdktf_provider_dns/ptr_record/
+-rw-r--r--   0 runner    (1001) docker     (127)    24005 2024-04-23 03:11:48.000000 cdktf-cdktf-provider-dns-8.0.1/src/cdktf_cdktf_provider_dns/ptr_record/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 03:11:48.000000 cdktf-cdktf-provider-dns-8.0.1/src/cdktf_cdktf_provider_dns/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 03:12:00.400456 cdktf-cdktf-provider-dns-8.0.1/src/cdktf_cdktf_provider_dns/srv_record_set/
+-rw-r--r--   0 runner    (1001) docker     (127)    42377 2024-04-23 03:11:48.000000 cdktf-cdktf-provider-dns-8.0.1/src/cdktf_cdktf_provider_dns/srv_record_set/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 03:12:00.400456 cdktf-cdktf-provider-dns-8.0.1/src/cdktf_cdktf_provider_dns/txt_record_set/
+-rw-r--r--   0 runner    (1001) docker     (127)    24368 2024-04-23 03:11:48.000000 cdktf-cdktf-provider-dns-8.0.1/src/cdktf_cdktf_provider_dns/txt_record_set/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 03:12:00.396456 cdktf-cdktf-provider-dns-8.0.1/src/cdktf_cdktf_provider_dns.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4356 2024-04-23 03:12:00.000000 cdktf-cdktf-provider-dns-8.0.1/src/cdktf_cdktf_provider_dns.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-04-23 03:12:00.000000 cdktf-cdktf-provider-dns-8.0.1/src/cdktf_cdktf_provider_dns.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 03:12:00.000000 cdktf-cdktf-provider-dns-8.0.1/src/cdktf_cdktf_provider_dns.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-23 03:12:00.000000 cdktf-cdktf-provider-dns-8.0.1/src/cdktf_cdktf_provider_dns.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-23 03:12:00.000000 cdktf-cdktf-provider-dns-8.0.1/src/cdktf_cdktf_provider_dns.egg-info/top_level.txt
```

### Comparing `cdktf-cdktf-provider-dns-8.0.0/LICENSE` & `cdktf-cdktf-provider-dns-8.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-dns-8.0.0/PKG-INFO` & `cdktf-cdktf-provider-dns-8.0.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdktf-cdktf-provider-dns
-Version: 8.0.0
+Version: 8.0.1
 Summary: Prebuilt dns Provider for Terraform CDK (cdktf)
 Home-page: https://github.com/cdktf/cdktf-provider-dns.git
 Author: HashiCorp
 License: MPL-2.0
 Project-URL: Source, https://github.com/cdktf/cdktf-provider-dns.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
@@ -17,17 +17,17 @@
 Classifier: Typing :: Typed
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved
 Requires-Python: ~=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# CDKTF prebuilt bindings for hashicorp/dns provider version 3.4.0
+# CDKTF prebuilt bindings for hashicorp/dns provider version 3.4.1
 
-This repo builds and publishes the [Terraform dns provider](https://registry.terraform.io/providers/hashicorp/dns/3.4.0/docs) bindings for [CDK for Terraform](https://cdk.tf).
+This repo builds and publishes the [Terraform dns provider](https://registry.terraform.io/providers/hashicorp/dns/3.4.1/docs) bindings for [CDK for Terraform](https://cdk.tf).
 
 ## Available Packages
 
 ### NPM
 
 The npm package is available at [https://www.npmjs.com/package/@cdktf/provider-dns](https://www.npmjs.com/package/@cdktf/provider-dns).
 
@@ -57,15 +57,18 @@
 </dependency>
 ```
 
 ### Go
 
 The go package is generated into the [`github.com/cdktf/cdktf-provider-dns-go`](https://github.com/cdktf/cdktf-provider-dns-go) package.
 
-`go get github.com/cdktf/cdktf-provider-dns-go/dns`
+`go get github.com/cdktf/cdktf-provider-dns-go/dns/<version>`
+
+Where `<version>` is the version of the prebuilt provider you would like to use e.g. `v11`. The full module name can be found
+within the [go.mod](https://github.com/cdktf/cdktf-provider-dns-go/blob/main/dns/go.mod#L1) file.
 
 ## Docs
 
 Find auto-generated docs for this provider here:
 
 * [Typescript](./docs/API.typescript.md)
 * [Python](./docs/API.python.md)
@@ -78,15 +81,15 @@
 ## Versioning
 
 This project is explicitly not tracking the Terraform dns provider version 1:1. In fact, it always tracks `latest` of `~> 3.2` with every release. If there are scenarios where you explicitly have to pin your provider version, you can do so by [generating the provider constructs manually](https://cdk.tf/imports).
 
 These are the upstream dependencies:
 
 * [CDK for Terraform](https://cdk.tf)
-* [Terraform dns provider](https://registry.terraform.io/providers/hashicorp/dns/3.4.0)
+* [Terraform dns provider](https://registry.terraform.io/providers/hashicorp/dns/3.4.1)
 * [Terraform Engine](https://terraform.io)
 
 If there are breaking changes (backward incompatible) in any of the above, the major version of this project will be bumped.
 
 ## Features / Issues / Bugs
 
 Please report bugs and issues to the [CDK for Terraform](https://cdk.tf) project:
```

### Comparing `cdktf-cdktf-provider-dns-8.0.0/README.md` & `cdktf-cdktf-provider-dns-8.0.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-# CDKTF prebuilt bindings for hashicorp/dns provider version 3.4.0
+# CDKTF prebuilt bindings for hashicorp/dns provider version 3.4.1
 
-This repo builds and publishes the [Terraform dns provider](https://registry.terraform.io/providers/hashicorp/dns/3.4.0/docs) bindings for [CDK for Terraform](https://cdk.tf).
+This repo builds and publishes the [Terraform dns provider](https://registry.terraform.io/providers/hashicorp/dns/3.4.1/docs) bindings for [CDK for Terraform](https://cdk.tf).
 
 ## Available Packages
 
 ### NPM
 
 The npm package is available at [https://www.npmjs.com/package/@cdktf/provider-dns](https://www.npmjs.com/package/@cdktf/provider-dns).
 
@@ -34,15 +34,18 @@
 </dependency>
 ```
 
 ### Go
 
 The go package is generated into the [`github.com/cdktf/cdktf-provider-dns-go`](https://github.com/cdktf/cdktf-provider-dns-go) package.
 
-`go get github.com/cdktf/cdktf-provider-dns-go/dns`
+`go get github.com/cdktf/cdktf-provider-dns-go/dns/<version>`
+
+Where `<version>` is the version of the prebuilt provider you would like to use e.g. `v11`. The full module name can be found
+within the [go.mod](https://github.com/cdktf/cdktf-provider-dns-go/blob/main/dns/go.mod#L1) file.
 
 ## Docs
 
 Find auto-generated docs for this provider here:
 
 * [Typescript](./docs/API.typescript.md)
 * [Python](./docs/API.python.md)
@@ -55,15 +58,15 @@
 ## Versioning
 
 This project is explicitly not tracking the Terraform dns provider version 1:1. In fact, it always tracks `latest` of `~> 3.2` with every release. If there are scenarios where you explicitly have to pin your provider version, you can do so by [generating the provider constructs manually](https://cdk.tf/imports).
 
 These are the upstream dependencies:
 
 * [CDK for Terraform](https://cdk.tf)
-* [Terraform dns provider](https://registry.terraform.io/providers/hashicorp/dns/3.4.0)
+* [Terraform dns provider](https://registry.terraform.io/providers/hashicorp/dns/3.4.1)
 * [Terraform Engine](https://terraform.io)
 
 If there are breaking changes (backward incompatible) in any of the above, the major version of this project will be bumped.
 
 ## Features / Issues / Bugs
 
 Please report bugs and issues to the [CDK for Terraform](https://cdk.tf) project:
```

### Comparing `cdktf-cdktf-provider-dns-8.0.0/setup.py` & `cdktf-cdktf-provider-dns-8.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdktf-cdktf-provider-dns",
-    "version": "8.0.0",
+    "version": "8.0.1",
     "description": "Prebuilt dns Provider for Terraform CDK (cdktf)",
     "license": "MPL-2.0",
     "url": "https://github.com/cdktf/cdktf-provider-dns.git",
     "long_description_content_type": "text/markdown",
     "author": "HashiCorp",
     "bdist_wheel": {
         "universal": true
@@ -39,25 +39,25 @@
         "cdktf_cdktf_provider_dns.provider",
         "cdktf_cdktf_provider_dns.ptr_record",
         "cdktf_cdktf_provider_dns.srv_record_set",
         "cdktf_cdktf_provider_dns.txt_record_set"
     ],
     "package_data": {
         "cdktf_cdktf_provider_dns._jsii": [
-            "provider-dns@8.0.0.jsii.tgz"
+            "provider-dns@8.0.1.jsii.tgz"
         ],
         "cdktf_cdktf_provider_dns": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.8",
     "install_requires": [
         "cdktf>=0.20.0, <0.21.0",
         "constructs>=10.3.0, <11.0.0",
-        "jsii>=1.93.0, <2.0.0",
+        "jsii>=1.97.0, <2.0.0",
         "publication>=0.0.3",
         "typeguard~=2.13.3"
     ],
     "classifiers": [
         "Intended Audience :: Developers",
         "Operating System :: OS Independent",
         "Programming Language :: JavaScript",
```

### Comparing `cdktf-cdktf-provider-dns-8.0.0/src/cdktf_cdktf_provider_dns/__init__.py` & `cdktf-cdktf-provider-dns-8.0.1/src/cdktf_cdktf_provider_dns/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
-# CDKTF prebuilt bindings for hashicorp/dns provider version 3.4.0
+# CDKTF prebuilt bindings for hashicorp/dns provider version 3.4.1
 
-This repo builds and publishes the [Terraform dns provider](https://registry.terraform.io/providers/hashicorp/dns/3.4.0/docs) bindings for [CDK for Terraform](https://cdk.tf).
+This repo builds and publishes the [Terraform dns provider](https://registry.terraform.io/providers/hashicorp/dns/3.4.1/docs) bindings for [CDK for Terraform](https://cdk.tf).
 
 ## Available Packages
 
 ### NPM
 
 The npm package is available at [https://www.npmjs.com/package/@cdktf/provider-dns](https://www.npmjs.com/package/@cdktf/provider-dns).
 
@@ -35,15 +35,18 @@
 </dependency>
 ```
 
 ### Go
 
 The go package is generated into the [`github.com/cdktf/cdktf-provider-dns-go`](https://github.com/cdktf/cdktf-provider-dns-go) package.
 
-`go get github.com/cdktf/cdktf-provider-dns-go/dns`
+`go get github.com/cdktf/cdktf-provider-dns-go/dns/<version>`
+
+Where `<version>` is the version of the prebuilt provider you would like to use e.g. `v11`. The full module name can be found
+within the [go.mod](https://github.com/cdktf/cdktf-provider-dns-go/blob/main/dns/go.mod#L1) file.
 
 ## Docs
 
 Find auto-generated docs for this provider here:
 
 * [Typescript](./docs/API.typescript.md)
 * [Python](./docs/API.python.md)
@@ -56,15 +59,15 @@
 ## Versioning
 
 This project is explicitly not tracking the Terraform dns provider version 1:1. In fact, it always tracks `latest` of `~> 3.2` with every release. If there are scenarios where you explicitly have to pin your provider version, you can do so by [generating the provider constructs manually](https://cdk.tf/imports).
 
 These are the upstream dependencies:
 
 * [CDK for Terraform](https://cdk.tf)
-* [Terraform dns provider](https://registry.terraform.io/providers/hashicorp/dns/3.4.0)
+* [Terraform dns provider](https://registry.terraform.io/providers/hashicorp/dns/3.4.1)
 * [Terraform Engine](https://terraform.io)
 
 If there are breaking changes (backward incompatible) in any of the above, the major version of this project will be bumped.
 
 ## Features / Issues / Bugs
 
 Please report bugs and issues to the [CDK for Terraform](https://cdk.tf) project:
@@ -86,14 +89,17 @@
 
 The provider version can be adjusted in [./.projenrc.js](./.projenrc.js).
 
 ### Repository Management
 
 The repository is managed by [CDKTF Repository Manager](https://github.com/cdktf/cdktf-repository-manager/).
 '''
+from pkgutil import extend_path
+__path__ = extend_path(__path__, __name__)
+
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
 import jsii
```

### Comparing `cdktf-cdktf-provider-dns-8.0.0/src/cdktf_cdktf_provider_dns/a_record_set/__init__.py` & `cdktf-cdktf-provider-dns-8.0.1/src/cdktf_cdktf_provider_dns/a_record_set/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 '''
 # `dns_a_record_set`
 
-Refer to the Terraform Registry for docs: [`dns_a_record_set`](https://registry.terraform.io/providers/hashicorp/dns/3.4.0/docs/resources/a_record_set).
+Refer to the Terraform Registry for docs: [`dns_a_record_set`](https://registry.terraform.io/providers/hashicorp/dns/3.4.1/docs/resources/a_record_set).
 '''
+from pkgutil import extend_path
+__path__ = extend_path(__path__, __name__)
+
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
 import jsii
@@ -22,15 +25,15 @@
 
 
 class ARecordSet(
     _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-dns.aRecordSet.ARecordSet",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.0/docs/resources/a_record_set dns_a_record_set}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.1/docs/resources/a_record_set dns_a_record_set}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id_: builtins.str,
         *,
         addresses: typing.Sequence[builtins.str],
@@ -42,23 +45,23 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.0/docs/resources/a_record_set dns_a_record_set} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.1/docs/resources/a_record_set dns_a_record_set} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param addresses: The IPv4 addresses this record set will point to. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.0/docs/resources/a_record_set#addresses ARecordSet#addresses}
-        :param zone: DNS zone the record set belongs to. It must be an FQDN, that is, include the trailing dot. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.0/docs/resources/a_record_set#zone ARecordSet#zone}
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.0/docs/resources/a_record_set#id ARecordSet#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param name: The name of the record set. The ``zone`` argument will be appended to this value to create the full record path. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.0/docs/resources/a_record_set#name ARecordSet#name}
-        :param ttl: The TTL of the record set. Defaults to ``3600``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.0/docs/resources/a_record_set#ttl ARecordSet#ttl}
+        :param addresses: The IPv4 addresses this record set will point to. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.1/docs/resources/a_record_set#addresses ARecordSet#addresses}
+        :param zone: DNS zone the record set belongs to. It must be an FQDN, that is, include the trailing dot. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.1/docs/resources/a_record_set#zone ARecordSet#zone}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.1/docs/resources/a_record_set#id ARecordSet#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param name: The name of the record set. The ``zone`` argument will be appended to this value to create the full record path. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.1/docs/resources/a_record_set#name ARecordSet#name}
+        :param ttl: The TTL of the record set. Defaults to ``3600``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.1/docs/resources/a_record_set#ttl ARecordSet#ttl}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -93,15 +96,15 @@
         import_from_id: builtins.str,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     ) -> _cdktf_9a9027ec.ImportableResource:
         '''Generates CDKTF code for importing a ARecordSet resource upon running "cdktf plan ".
 
         :param scope: The scope in which to define this construct.
         :param import_to_id: The construct id used in the generated config for the ARecordSet to import.
-        :param import_from_id: The id of the existing ARecordSet that should be imported. Refer to the {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.0/docs/resources/a_record_set#import import section} in the documentation of this resource for the id to use
+        :param import_from_id: The id of the existing ARecordSet that should be imported. Refer to the {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.1/docs/resources/a_record_set#import import section} in the documentation of this resource for the id to use
         :param provider: ? Optional instance of the provider where the ARecordSet to import is found.
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__203c7a17484ff808d45d8ea26c09f4dfb1339b63829aacb63c8b13011c77ae42)
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
             check_type(argname="argument import_to_id", value=import_to_id, expected_type=type_hints["import_to_id"])
             check_type(argname="argument import_from_id", value=import_from_id, expected_type=type_hints["import_from_id"])
@@ -258,19 +261,19 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param addresses: The IPv4 addresses this record set will point to. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.0/docs/resources/a_record_set#addresses ARecordSet#addresses}
-        :param zone: DNS zone the record set belongs to. It must be an FQDN, that is, include the trailing dot. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.0/docs/resources/a_record_set#zone ARecordSet#zone}
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.0/docs/resources/a_record_set#id ARecordSet#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param name: The name of the record set. The ``zone`` argument will be appended to this value to create the full record path. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.0/docs/resources/a_record_set#name ARecordSet#name}
-        :param ttl: The TTL of the record set. Defaults to ``3600``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.0/docs/resources/a_record_set#ttl ARecordSet#ttl}
+        :param addresses: The IPv4 addresses this record set will point to. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.1/docs/resources/a_record_set#addresses ARecordSet#addresses}
+        :param zone: DNS zone the record set belongs to. It must be an FQDN, that is, include the trailing dot. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.1/docs/resources/a_record_set#zone ARecordSet#zone}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.1/docs/resources/a_record_set#id ARecordSet#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param name: The name of the record set. The ``zone`` argument will be appended to this value to create the full record path. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.1/docs/resources/a_record_set#name ARecordSet#name}
+        :param ttl: The TTL of the record set. Defaults to ``3600``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.1/docs/resources/a_record_set#ttl ARecordSet#ttl}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__15cff60de25b8724a41dea37bad793e750c7efcacadb8bc6470dbb98cec4342f)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -373,56 +376,56 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def addresses(self) -> typing.List[builtins.str]:
         '''The IPv4 addresses this record set will point to.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.0/docs/resources/a_record_set#addresses ARecordSet#addresses}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.1/docs/resources/a_record_set#addresses ARecordSet#addresses}
         '''
         result = self._values.get("addresses")
         assert result is not None, "Required property 'addresses' is missing"
         return typing.cast(typing.List[builtins.str], result)
 
     @builtins.property
     def zone(self) -> builtins.str:
         '''DNS zone the record set belongs to. It must be an FQDN, that is, include the trailing dot.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.0/docs/resources/a_record_set#zone ARecordSet#zone}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.1/docs/resources/a_record_set#zone ARecordSet#zone}
         '''
         result = self._values.get("zone")
         assert result is not None, "Required property 'zone' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.0/docs/resources/a_record_set#id ARecordSet#id}.
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.1/docs/resources/a_record_set#id ARecordSet#id}.
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def name(self) -> typing.Optional[builtins.str]:
         '''The name of the record set.
 
         The ``zone`` argument will be appended to this value to create the full record path.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.0/docs/resources/a_record_set#name ARecordSet#name}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.1/docs/resources/a_record_set#name ARecordSet#name}
         '''
         result = self._values.get("name")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def ttl(self) -> typing.Optional[jsii.Number]:
         '''The TTL of the record set. Defaults to ``3600``.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.0/docs/resources/a_record_set#ttl ARecordSet#ttl}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.1/docs/resources/a_record_set#ttl ARecordSet#ttl}
         '''
         result = self._values.get("ttl")
         return typing.cast(typing.Optional[jsii.Number], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
```

### Comparing `cdktf-cdktf-provider-dns-8.0.0/src/cdktf_cdktf_provider_dns/aaaa_record_set/__init__.py` & `cdktf-cdktf-provider-dns-8.0.1/src/cdktf_cdktf_provider_dns/aaaa_record_set/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 '''
 # `dns_aaaa_record_set`
 
-Refer to the Terraform Registry for docs: [`dns_aaaa_record_set`](https://registry.terraform.io/providers/hashicorp/dns/3.4.0/docs/resources/aaaa_record_set).
+Refer to the Terraform Registry for docs: [`dns_aaaa_record_set`](https://registry.terraform.io/providers/hashicorp/dns/3.4.1/docs/resources/aaaa_record_set).
 '''
+from pkgutil import extend_path
+__path__ = extend_path(__path__, __name__)
+
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
 import jsii
@@ -22,15 +25,15 @@
 
 
 class AaaaRecordSet(
     _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-dns.aaaaRecordSet.AaaaRecordSet",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.0/docs/resources/aaaa_record_set dns_aaaa_record_set}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.1/docs/resources/aaaa_record_set dns_aaaa_record_set}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id_: builtins.str,
         *,
         addresses: typing.Sequence[builtins.str],
@@ -42,23 +45,23 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.0/docs/resources/aaaa_record_set dns_aaaa_record_set} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.1/docs/resources/aaaa_record_set dns_aaaa_record_set} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param addresses: The IPv6 addresses this record set will point to. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.0/docs/resources/aaaa_record_set#addresses AaaaRecordSet#addresses}
-        :param zone: DNS zone the record set belongs to. It must be an FQDN, that is, include the trailing dot. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.0/docs/resources/aaaa_record_set#zone AaaaRecordSet#zone}
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.0/docs/resources/aaaa_record_set#id AaaaRecordSet#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param name: The name of the record set. The ``zone`` argument will be appended to this value to create the full record path. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.0/docs/resources/aaaa_record_set#name AaaaRecordSet#name}
-        :param ttl: The TTL of the record set. Defaults to ``3600``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.0/docs/resources/aaaa_record_set#ttl AaaaRecordSet#ttl}
+        :param addresses: The IPv6 addresses this record set will point to. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.1/docs/resources/aaaa_record_set#addresses AaaaRecordSet#addresses}
+        :param zone: DNS zone the record set belongs to. It must be an FQDN, that is, include the trailing dot. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.1/docs/resources/aaaa_record_set#zone AaaaRecordSet#zone}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.1/docs/resources/aaaa_record_set#id AaaaRecordSet#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param name: The name of the record set. The ``zone`` argument will be appended to this value to create the full record path. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.1/docs/resources/aaaa_record_set#name AaaaRecordSet#name}
+        :param ttl: The TTL of the record set. Defaults to ``3600``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.1/docs/resources/aaaa_record_set#ttl AaaaRecordSet#ttl}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -93,15 +96,15 @@
         import_from_id: builtins.str,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     ) -> _cdktf_9a9027ec.ImportableResource:
         '''Generates CDKTF code for importing a AaaaRecordSet resource upon running "cdktf plan ".
 
         :param scope: The scope in which to define this construct.
         :param import_to_id: The construct id used in the generated config for the AaaaRecordSet to import.
-        :param import_from_id: The id of the existing AaaaRecordSet that should be imported. Refer to the {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.0/docs/resources/aaaa_record_set#import import section} in the documentation of this resource for the id to use
+        :param import_from_id: The id of the existing AaaaRecordSet that should be imported. Refer to the {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.1/docs/resources/aaaa_record_set#import import section} in the documentation of this resource for the id to use
         :param provider: ? Optional instance of the provider where the AaaaRecordSet to import is found.
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__c0a1ca531ebffb297561eb5ef12080ee48065e591dbe0ea6b9424ec3c5e96eb4)
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
             check_type(argname="argument import_to_id", value=import_to_id, expected_type=type_hints["import_to_id"])
             check_type(argname="argument import_from_id", value=import_from_id, expected_type=type_hints["import_from_id"])
@@ -258,19 +261,19 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param addresses: The IPv6 addresses this record set will point to. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.0/docs/resources/aaaa_record_set#addresses AaaaRecordSet#addresses}
-        :param zone: DNS zone the record set belongs to. It must be an FQDN, that is, include the trailing dot. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.0/docs/resources/aaaa_record_set#zone AaaaRecordSet#zone}
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.0/docs/resources/aaaa_record_set#id AaaaRecordSet#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param name: The name of the record set. The ``zone`` argument will be appended to this value to create the full record path. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.0/docs/resources/aaaa_record_set#name AaaaRecordSet#name}
-        :param ttl: The TTL of the record set. Defaults to ``3600``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.0/docs/resources/aaaa_record_set#ttl AaaaRecordSet#ttl}
+        :param addresses: The IPv6 addresses this record set will point to. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.1/docs/resources/aaaa_record_set#addresses AaaaRecordSet#addresses}
+        :param zone: DNS zone the record set belongs to. It must be an FQDN, that is, include the trailing dot. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.1/docs/resources/aaaa_record_set#zone AaaaRecordSet#zone}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.1/docs/resources/aaaa_record_set#id AaaaRecordSet#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param name: The name of the record set. The ``zone`` argument will be appended to this value to create the full record path. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.1/docs/resources/aaaa_record_set#name AaaaRecordSet#name}
+        :param ttl: The TTL of the record set. Defaults to ``3600``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.1/docs/resources/aaaa_record_set#ttl AaaaRecordSet#ttl}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__7b02504a909c79d4df8654eda870cd6b0da805b48d848ba6bc32daaa4249e3a3)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -373,56 +376,56 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def addresses(self) -> typing.List[builtins.str]:
         '''The IPv6 addresses this record set will point to.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.0/docs/resources/aaaa_record_set#addresses AaaaRecordSet#addresses}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.1/docs/resources/aaaa_record_set#addresses AaaaRecordSet#addresses}
         '''
         result = self._values.get("addresses")
         assert result is not None, "Required property 'addresses' is missing"
         return typing.cast(typing.List[builtins.str], result)
 
     @builtins.property
     def zone(self) -> builtins.str:
         '''DNS zone the record set belongs to. It must be an FQDN, that is, include the trailing dot.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.0/docs/resources/aaaa_record_set#zone AaaaRecordSet#zone}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.1/docs/resources/aaaa_record_set#zone AaaaRecordSet#zone}
         '''
         result = self._values.get("zone")
         assert result is not None, "Required property 'zone' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.0/docs/resources/aaaa_record_set#id AaaaRecordSet#id}.
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.1/docs/resources/aaaa_record_set#id AaaaRecordSet#id}.
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def name(self) -> typing.Optional[builtins.str]:
         '''The name of the record set.
 
         The ``zone`` argument will be appended to this value to create the full record path.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.0/docs/resources/aaaa_record_set#name AaaaRecordSet#name}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.1/docs/resources/aaaa_record_set#name AaaaRecordSet#name}
         '''
         result = self._values.get("name")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def ttl(self) -> typing.Optional[jsii.Number]:
         '''The TTL of the record set. Defaults to ``3600``.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.0/docs/resources/aaaa_record_set#ttl AaaaRecordSet#ttl}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.1/docs/resources/aaaa_record_set#ttl AaaaRecordSet#ttl}
         '''
         result = self._values.get("ttl")
         return typing.cast(typing.Optional[jsii.Number], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
```

### Comparing `cdktf-cdktf-provider-dns-8.0.0/src/cdktf_cdktf_provider_dns/cname_record/__init__.py` & `cdktf-cdktf-provider-dns-8.0.1/src/cdktf_cdktf_provider_dns/cname_record/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 '''
 # `dns_cname_record`
 
-Refer to the Terraform Registry for docs: [`dns_cname_record`](https://registry.terraform.io/providers/hashicorp/dns/3.4.0/docs/resources/cname_record).
+Refer to the Terraform Registry for docs: [`dns_cname_record`](https://registry.terraform.io/providers/hashicorp/dns/3.4.1/docs/resources/cname_record).
 '''
+from pkgutil import extend_path
+__path__ = extend_path(__path__, __name__)
+
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
 import jsii
@@ -22,15 +25,15 @@
 
 
 class CnameRecord(
     _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-dns.cnameRecord.CnameRecord",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.0/docs/resources/cname_record dns_cname_record}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.1/docs/resources/cname_record dns_cname_record}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id: builtins.str,
         *,
         cname: builtins.str,
@@ -41,22 +44,22 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.0/docs/resources/cname_record dns_cname_record} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.1/docs/resources/cname_record dns_cname_record} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param cname: The canonical name this record will point to. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.0/docs/resources/cname_record#cname CnameRecord#cname}
-        :param name: The name of the record. The ``zone`` argument will be appended to this value to create the full record path. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.0/docs/resources/cname_record#name CnameRecord#name}
-        :param zone: DNS zone the record belongs to. It must be an FQDN, that is, include the trailing dot. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.0/docs/resources/cname_record#zone CnameRecord#zone}
-        :param ttl: The TTL of the record set. Defaults to ``3600``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.0/docs/resources/cname_record#ttl CnameRecord#ttl}
+        :param cname: The canonical name this record will point to. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.1/docs/resources/cname_record#cname CnameRecord#cname}
+        :param name: The name of the record. The ``zone`` argument will be appended to this value to create the full record path. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.1/docs/resources/cname_record#name CnameRecord#name}
+        :param zone: DNS zone the record belongs to. It must be an FQDN, that is, include the trailing dot. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.1/docs/resources/cname_record#zone CnameRecord#zone}
+        :param ttl: The TTL of the record set. Defaults to ``3600``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.1/docs/resources/cname_record#ttl CnameRecord#ttl}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -90,15 +93,15 @@
         import_from_id: builtins.str,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     ) -> _cdktf_9a9027ec.ImportableResource:
         '''Generates CDKTF code for importing a CnameRecord resource upon running "cdktf plan ".
 
         :param scope: The scope in which to define this construct.
         :param import_to_id: The construct id used in the generated config for the CnameRecord to import.
-        :param import_from_id: The id of the existing CnameRecord that should be imported. Refer to the {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.0/docs/resources/cname_record#import import section} in the documentation of this resource for the id to use
+        :param import_from_id: The id of the existing CnameRecord that should be imported. Refer to the {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.1/docs/resources/cname_record#import import section} in the documentation of this resource for the id to use
         :param provider: ? Optional instance of the provider where the CnameRecord to import is found.
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__911d2fcea22e61391d05f0e32b8b00fe941cc0392fe71e269cf4bc68e94a73bb)
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
             check_type(argname="argument import_to_id", value=import_to_id, expected_type=type_hints["import_to_id"])
             check_type(argname="argument import_from_id", value=import_from_id, expected_type=type_hints["import_from_id"])
@@ -233,18 +236,18 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param cname: The canonical name this record will point to. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.0/docs/resources/cname_record#cname CnameRecord#cname}
-        :param name: The name of the record. The ``zone`` argument will be appended to this value to create the full record path. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.0/docs/resources/cname_record#name CnameRecord#name}
-        :param zone: DNS zone the record belongs to. It must be an FQDN, that is, include the trailing dot. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.0/docs/resources/cname_record#zone CnameRecord#zone}
-        :param ttl: The TTL of the record set. Defaults to ``3600``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.0/docs/resources/cname_record#ttl CnameRecord#ttl}
+        :param cname: The canonical name this record will point to. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.1/docs/resources/cname_record#cname CnameRecord#cname}
+        :param name: The name of the record. The ``zone`` argument will be appended to this value to create the full record path. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.1/docs/resources/cname_record#name CnameRecord#name}
+        :param zone: DNS zone the record belongs to. It must be an FQDN, that is, include the trailing dot. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.1/docs/resources/cname_record#zone CnameRecord#zone}
+        :param ttl: The TTL of the record set. Defaults to ``3600``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.1/docs/resources/cname_record#ttl CnameRecord#ttl}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__85ab3d3a662907f40b18ce9ac321aedec0c7f81fc9368400c9f94ee960050a8a)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -343,47 +346,47 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def cname(self) -> builtins.str:
         '''The canonical name this record will point to.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.0/docs/resources/cname_record#cname CnameRecord#cname}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.1/docs/resources/cname_record#cname CnameRecord#cname}
         '''
         result = self._values.get("cname")
         assert result is not None, "Required property 'cname' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def name(self) -> builtins.str:
         '''The name of the record.
 
         The ``zone`` argument will be appended to this value to create the full record path.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.0/docs/resources/cname_record#name CnameRecord#name}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.1/docs/resources/cname_record#name CnameRecord#name}
         '''
         result = self._values.get("name")
         assert result is not None, "Required property 'name' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def zone(self) -> builtins.str:
         '''DNS zone the record belongs to. It must be an FQDN, that is, include the trailing dot.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.0/docs/resources/cname_record#zone CnameRecord#zone}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.1/docs/resources/cname_record#zone CnameRecord#zone}
         '''
         result = self._values.get("zone")
         assert result is not None, "Required property 'zone' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def ttl(self) -> typing.Optional[jsii.Number]:
         '''The TTL of the record set. Defaults to ``3600``.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.0/docs/resources/cname_record#ttl CnameRecord#ttl}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.1/docs/resources/cname_record#ttl CnameRecord#ttl}
         '''
         result = self._values.get("ttl")
         return typing.cast(typing.Optional[jsii.Number], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
```

### Comparing `cdktf-cdktf-provider-dns-8.0.0/src/cdktf_cdktf_provider_dns/data_dns_a_record_set/__init__.py` & `cdktf-cdktf-provider-dns-8.0.1/src/cdktf_cdktf_provider_dns/data_dns_a_record_set/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 '''
 # `data_dns_a_record_set`
 
-Refer to the Terraform Registry for docs: [`data_dns_a_record_set`](https://registry.terraform.io/providers/hashicorp/dns/3.4.0/docs/data-sources/a_record_set).
+Refer to the Terraform Registry for docs: [`data_dns_a_record_set`](https://registry.terraform.io/providers/hashicorp/dns/3.4.1/docs/data-sources/a_record_set).
 '''
+from pkgutil import extend_path
+__path__ = extend_path(__path__, __name__)
+
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
 import jsii
@@ -22,15 +25,15 @@
 
 
 class DataDnsARecordSet(
     _cdktf_9a9027ec.TerraformDataSource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-dns.dataDnsARecordSet.DataDnsARecordSet",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.0/docs/data-sources/a_record_set dns_a_record_set}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.1/docs/data-sources/a_record_set dns_a_record_set}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id: builtins.str,
         *,
         host: builtins.str,
@@ -38,19 +41,19 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.0/docs/data-sources/a_record_set dns_a_record_set} Data Source.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.1/docs/data-sources/a_record_set dns_a_record_set} Data Source.
 
         :param scope: The scope in which to define this construct.
         :param id: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param host: Host to look up. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.0/docs/data-sources/a_record_set#host DataDnsARecordSet#host}
+        :param host: Host to look up. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.1/docs/data-sources/a_record_set#host DataDnsARecordSet#host}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -81,15 +84,15 @@
         import_from_id: builtins.str,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     ) -> _cdktf_9a9027ec.ImportableResource:
         '''Generates CDKTF code for importing a DataDnsARecordSet resource upon running "cdktf plan ".
 
         :param scope: The scope in which to define this construct.
         :param import_to_id: The construct id used in the generated config for the DataDnsARecordSet to import.
-        :param import_from_id: The id of the existing DataDnsARecordSet that should be imported. Refer to the {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.0/docs/data-sources/a_record_set#import import section} in the documentation of this resource for the id to use
+        :param import_from_id: The id of the existing DataDnsARecordSet that should be imported. Refer to the {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.1/docs/data-sources/a_record_set#import import section} in the documentation of this resource for the id to use
         :param provider: ? Optional instance of the provider where the DataDnsARecordSet to import is found.
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__5eaa1135d06ddd6f60d7ba281eb8c9a66ea557f00b985db4b7f40dfeaf09848d)
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
             check_type(argname="argument import_to_id", value=import_to_id, expected_type=type_hints["import_to_id"])
             check_type(argname="argument import_from_id", value=import_from_id, expected_type=type_hints["import_from_id"])
@@ -168,15 +171,15 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param host: Host to look up. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.0/docs/data-sources/a_record_set#host DataDnsARecordSet#host}
+        :param host: Host to look up. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.1/docs/data-sources/a_record_set#host DataDnsARecordSet#host}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__4392563f6d6ca59db53a3f1e6c445df6f633bba1c3bced497176d8a70eb282ed)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -268,15 +271,15 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def host(self) -> builtins.str:
         '''Host to look up.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.0/docs/data-sources/a_record_set#host DataDnsARecordSet#host}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.1/docs/data-sources/a_record_set#host DataDnsARecordSet#host}
         '''
         result = self._values.get("host")
         assert result is not None, "Required property 'host' is missing"
         return typing.cast(builtins.str, result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
```

### Comparing `cdktf-cdktf-provider-dns-8.0.0/src/cdktf_cdktf_provider_dns/data_dns_aaaa_record_set/__init__.py` & `cdktf-cdktf-provider-dns-8.0.1/src/cdktf_cdktf_provider_dns/data_dns_aaaa_record_set/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 '''
 # `data_dns_aaaa_record_set`
 
-Refer to the Terraform Registry for docs: [`data_dns_aaaa_record_set`](https://registry.terraform.io/providers/hashicorp/dns/3.4.0/docs/data-sources/aaaa_record_set).
+Refer to the Terraform Registry for docs: [`data_dns_aaaa_record_set`](https://registry.terraform.io/providers/hashicorp/dns/3.4.1/docs/data-sources/aaaa_record_set).
 '''
+from pkgutil import extend_path
+__path__ = extend_path(__path__, __name__)
+
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
 import jsii
@@ -22,15 +25,15 @@
 
 
 class DataDnsAaaaRecordSet(
     _cdktf_9a9027ec.TerraformDataSource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-dns.dataDnsAaaaRecordSet.DataDnsAaaaRecordSet",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.0/docs/data-sources/aaaa_record_set dns_aaaa_record_set}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.1/docs/data-sources/aaaa_record_set dns_aaaa_record_set}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id: builtins.str,
         *,
         host: builtins.str,
@@ -38,19 +41,19 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.0/docs/data-sources/aaaa_record_set dns_aaaa_record_set} Data Source.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.1/docs/data-sources/aaaa_record_set dns_aaaa_record_set} Data Source.
 
         :param scope: The scope in which to define this construct.
         :param id: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param host: Host to look up. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.0/docs/data-sources/aaaa_record_set#host DataDnsAaaaRecordSet#host}
+        :param host: Host to look up. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.1/docs/data-sources/aaaa_record_set#host DataDnsAaaaRecordSet#host}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -81,15 +84,15 @@
         import_from_id: builtins.str,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     ) -> _cdktf_9a9027ec.ImportableResource:
         '''Generates CDKTF code for importing a DataDnsAaaaRecordSet resource upon running "cdktf plan ".
 
         :param scope: The scope in which to define this construct.
         :param import_to_id: The construct id used in the generated config for the DataDnsAaaaRecordSet to import.
-        :param import_from_id: The id of the existing DataDnsAaaaRecordSet that should be imported. Refer to the {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.0/docs/data-sources/aaaa_record_set#import import section} in the documentation of this resource for the id to use
+        :param import_from_id: The id of the existing DataDnsAaaaRecordSet that should be imported. Refer to the {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.1/docs/data-sources/aaaa_record_set#import import section} in the documentation of this resource for the id to use
         :param provider: ? Optional instance of the provider where the DataDnsAaaaRecordSet to import is found.
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__2ceb882622ad4233db3440d6cf79aa64a9f39e57e3ff7f750192b7cbd16dbf48)
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
             check_type(argname="argument import_to_id", value=import_to_id, expected_type=type_hints["import_to_id"])
             check_type(argname="argument import_from_id", value=import_from_id, expected_type=type_hints["import_from_id"])
@@ -168,15 +171,15 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param host: Host to look up. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.0/docs/data-sources/aaaa_record_set#host DataDnsAaaaRecordSet#host}
+        :param host: Host to look up. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.1/docs/data-sources/aaaa_record_set#host DataDnsAaaaRecordSet#host}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__908caa216afdc6eb58e4534363fab765aca58abf2556163688267bf57a2baf0a)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -268,15 +271,15 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def host(self) -> builtins.str:
         '''Host to look up.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.0/docs/data-sources/aaaa_record_set#host DataDnsAaaaRecordSet#host}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.1/docs/data-sources/aaaa_record_set#host DataDnsAaaaRecordSet#host}
         '''
         result = self._values.get("host")
         assert result is not None, "Required property 'host' is missing"
         return typing.cast(builtins.str, result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
```

### Comparing `cdktf-cdktf-provider-dns-8.0.0/src/cdktf_cdktf_provider_dns/data_dns_cname_record_set/__init__.py` & `cdktf-cdktf-provider-dns-8.0.1/src/cdktf_cdktf_provider_dns/data_dns_cname_record_set/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 '''
 # `data_dns_cname_record_set`
 
-Refer to the Terraform Registry for docs: [`data_dns_cname_record_set`](https://registry.terraform.io/providers/hashicorp/dns/3.4.0/docs/data-sources/cname_record_set).
+Refer to the Terraform Registry for docs: [`data_dns_cname_record_set`](https://registry.terraform.io/providers/hashicorp/dns/3.4.1/docs/data-sources/cname_record_set).
 '''
+from pkgutil import extend_path
+__path__ = extend_path(__path__, __name__)
+
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
 import jsii
@@ -22,15 +25,15 @@
 
 
 class DataDnsCnameRecordSet(
     _cdktf_9a9027ec.TerraformDataSource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-dns.dataDnsCnameRecordSet.DataDnsCnameRecordSet",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.0/docs/data-sources/cname_record_set dns_cname_record_set}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.1/docs/data-sources/cname_record_set dns_cname_record_set}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id: builtins.str,
         *,
         host: builtins.str,
@@ -38,19 +41,19 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.0/docs/data-sources/cname_record_set dns_cname_record_set} Data Source.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.1/docs/data-sources/cname_record_set dns_cname_record_set} Data Source.
 
         :param scope: The scope in which to define this construct.
         :param id: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param host: Host to look up. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.0/docs/data-sources/cname_record_set#host DataDnsCnameRecordSet#host}
+        :param host: Host to look up. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.1/docs/data-sources/cname_record_set#host DataDnsCnameRecordSet#host}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -81,15 +84,15 @@
         import_from_id: builtins.str,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     ) -> _cdktf_9a9027ec.ImportableResource:
         '''Generates CDKTF code for importing a DataDnsCnameRecordSet resource upon running "cdktf plan ".
 
         :param scope: The scope in which to define this construct.
         :param import_to_id: The construct id used in the generated config for the DataDnsCnameRecordSet to import.
-        :param import_from_id: The id of the existing DataDnsCnameRecordSet that should be imported. Refer to the {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.0/docs/data-sources/cname_record_set#import import section} in the documentation of this resource for the id to use
+        :param import_from_id: The id of the existing DataDnsCnameRecordSet that should be imported. Refer to the {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.1/docs/data-sources/cname_record_set#import import section} in the documentation of this resource for the id to use
         :param provider: ? Optional instance of the provider where the DataDnsCnameRecordSet to import is found.
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__c7f16e0f186c6456e604465a4cbb0ce0cd37fb42acbd4e379646d1cc18434288)
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
             check_type(argname="argument import_to_id", value=import_to_id, expected_type=type_hints["import_to_id"])
             check_type(argname="argument import_from_id", value=import_from_id, expected_type=type_hints["import_from_id"])
@@ -168,15 +171,15 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param host: Host to look up. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.0/docs/data-sources/cname_record_set#host DataDnsCnameRecordSet#host}
+        :param host: Host to look up. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.1/docs/data-sources/cname_record_set#host DataDnsCnameRecordSet#host}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__3d1a77e5261d74d2f0b88c8a59df0d2ff76c2bdc029e41e1cfdd2cabeb567e46)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -268,15 +271,15 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def host(self) -> builtins.str:
         '''Host to look up.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.0/docs/data-sources/cname_record_set#host DataDnsCnameRecordSet#host}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.1/docs/data-sources/cname_record_set#host DataDnsCnameRecordSet#host}
         '''
         result = self._values.get("host")
         assert result is not None, "Required property 'host' is missing"
         return typing.cast(builtins.str, result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
```

### Comparing `cdktf-cdktf-provider-dns-8.0.0/src/cdktf_cdktf_provider_dns/data_dns_mx_record_set/__init__.py` & `cdktf-cdktf-provider-dns-8.0.1/src/cdktf_cdktf_provider_dns/data_dns_mx_record_set/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 '''
 # `data_dns_mx_record_set`
 
-Refer to the Terraform Registry for docs: [`data_dns_mx_record_set`](https://registry.terraform.io/providers/hashicorp/dns/3.4.0/docs/data-sources/mx_record_set).
+Refer to the Terraform Registry for docs: [`data_dns_mx_record_set`](https://registry.terraform.io/providers/hashicorp/dns/3.4.1/docs/data-sources/mx_record_set).
 '''
+from pkgutil import extend_path
+__path__ = extend_path(__path__, __name__)
+
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
 import jsii
@@ -22,15 +25,15 @@
 
 
 class DataDnsMxRecordSet(
     _cdktf_9a9027ec.TerraformDataSource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-dns.dataDnsMxRecordSet.DataDnsMxRecordSet",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.0/docs/data-sources/mx_record_set dns_mx_record_set}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.1/docs/data-sources/mx_record_set dns_mx_record_set}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id: builtins.str,
         *,
         domain: builtins.str,
@@ -38,19 +41,19 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.0/docs/data-sources/mx_record_set dns_mx_record_set} Data Source.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.1/docs/data-sources/mx_record_set dns_mx_record_set} Data Source.
 
         :param scope: The scope in which to define this construct.
         :param id: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param domain: Domain to look up. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.0/docs/data-sources/mx_record_set#domain DataDnsMxRecordSet#domain}
+        :param domain: Domain to look up. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.1/docs/data-sources/mx_record_set#domain DataDnsMxRecordSet#domain}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -81,15 +84,15 @@
         import_from_id: builtins.str,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     ) -> _cdktf_9a9027ec.ImportableResource:
         '''Generates CDKTF code for importing a DataDnsMxRecordSet resource upon running "cdktf plan ".
 
         :param scope: The scope in which to define this construct.
         :param import_to_id: The construct id used in the generated config for the DataDnsMxRecordSet to import.
-        :param import_from_id: The id of the existing DataDnsMxRecordSet that should be imported. Refer to the {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.0/docs/data-sources/mx_record_set#import import section} in the documentation of this resource for the id to use
+        :param import_from_id: The id of the existing DataDnsMxRecordSet that should be imported. Refer to the {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.1/docs/data-sources/mx_record_set#import import section} in the documentation of this resource for the id to use
         :param provider: ? Optional instance of the provider where the DataDnsMxRecordSet to import is found.
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__3fea9240ae2f40fe635ab42163144707a12629a0b82d958746a692cf26ef3fcc)
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
             check_type(argname="argument import_to_id", value=import_to_id, expected_type=type_hints["import_to_id"])
             check_type(argname="argument import_from_id", value=import_from_id, expected_type=type_hints["import_from_id"])
@@ -168,15 +171,15 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param domain: Domain to look up. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.0/docs/data-sources/mx_record_set#domain DataDnsMxRecordSet#domain}
+        :param domain: Domain to look up. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.1/docs/data-sources/mx_record_set#domain DataDnsMxRecordSet#domain}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__112b631474f3656d4096e3a10b250e7363827fdc3f044c40f9d5c97caf0f0ec4)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -268,15 +271,15 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def domain(self) -> builtins.str:
         '''Domain to look up.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.0/docs/data-sources/mx_record_set#domain DataDnsMxRecordSet#domain}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.1/docs/data-sources/mx_record_set#domain DataDnsMxRecordSet#domain}
         '''
         result = self._values.get("domain")
         assert result is not None, "Required property 'domain' is missing"
         return typing.cast(builtins.str, result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
```

### Comparing `cdktf-cdktf-provider-dns-8.0.0/src/cdktf_cdktf_provider_dns/data_dns_ns_record_set/__init__.py` & `cdktf-cdktf-provider-dns-8.0.1/src/cdktf_cdktf_provider_dns/data_dns_ns_record_set/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 '''
 # `data_dns_ns_record_set`
 
-Refer to the Terraform Registry for docs: [`data_dns_ns_record_set`](https://registry.terraform.io/providers/hashicorp/dns/3.4.0/docs/data-sources/ns_record_set).
+Refer to the Terraform Registry for docs: [`data_dns_ns_record_set`](https://registry.terraform.io/providers/hashicorp/dns/3.4.1/docs/data-sources/ns_record_set).
 '''
+from pkgutil import extend_path
+__path__ = extend_path(__path__, __name__)
+
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
 import jsii
@@ -22,15 +25,15 @@
 
 
 class DataDnsNsRecordSet(
     _cdktf_9a9027ec.TerraformDataSource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-dns.dataDnsNsRecordSet.DataDnsNsRecordSet",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.0/docs/data-sources/ns_record_set dns_ns_record_set}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.1/docs/data-sources/ns_record_set dns_ns_record_set}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id: builtins.str,
         *,
         host: builtins.str,
@@ -38,19 +41,19 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.0/docs/data-sources/ns_record_set dns_ns_record_set} Data Source.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.1/docs/data-sources/ns_record_set dns_ns_record_set} Data Source.
 
         :param scope: The scope in which to define this construct.
         :param id: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param host: Host to look up. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.0/docs/data-sources/ns_record_set#host DataDnsNsRecordSet#host}
+        :param host: Host to look up. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.1/docs/data-sources/ns_record_set#host DataDnsNsRecordSet#host}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -81,15 +84,15 @@
         import_from_id: builtins.str,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     ) -> _cdktf_9a9027ec.ImportableResource:
         '''Generates CDKTF code for importing a DataDnsNsRecordSet resource upon running "cdktf plan ".
 
         :param scope: The scope in which to define this construct.
         :param import_to_id: The construct id used in the generated config for the DataDnsNsRecordSet to import.
-        :param import_from_id: The id of the existing DataDnsNsRecordSet that should be imported. Refer to the {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.0/docs/data-sources/ns_record_set#import import section} in the documentation of this resource for the id to use
+        :param import_from_id: The id of the existing DataDnsNsRecordSet that should be imported. Refer to the {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.1/docs/data-sources/ns_record_set#import import section} in the documentation of this resource for the id to use
         :param provider: ? Optional instance of the provider where the DataDnsNsRecordSet to import is found.
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__822f634e668813647f22746c2e0cc800c785303ce95bdc9e4073ff94611eabac)
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
             check_type(argname="argument import_to_id", value=import_to_id, expected_type=type_hints["import_to_id"])
             check_type(argname="argument import_from_id", value=import_from_id, expected_type=type_hints["import_from_id"])
@@ -168,15 +171,15 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param host: Host to look up. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.0/docs/data-sources/ns_record_set#host DataDnsNsRecordSet#host}
+        :param host: Host to look up. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.1/docs/data-sources/ns_record_set#host DataDnsNsRecordSet#host}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__83f15275c0d7535be3797ec071f20244f1d9cf271ac24f43dc5fe373457644e3)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -268,15 +271,15 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def host(self) -> builtins.str:
         '''Host to look up.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.0/docs/data-sources/ns_record_set#host DataDnsNsRecordSet#host}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.1/docs/data-sources/ns_record_set#host DataDnsNsRecordSet#host}
         '''
         result = self._values.get("host")
         assert result is not None, "Required property 'host' is missing"
         return typing.cast(builtins.str, result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
```

### Comparing `cdktf-cdktf-provider-dns-8.0.0/src/cdktf_cdktf_provider_dns/data_dns_ptr_record_set/__init__.py` & `cdktf-cdktf-provider-dns-8.0.1/src/cdktf_cdktf_provider_dns/data_dns_ptr_record_set/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 '''
 # `data_dns_ptr_record_set`
 
-Refer to the Terraform Registry for docs: [`data_dns_ptr_record_set`](https://registry.terraform.io/providers/hashicorp/dns/3.4.0/docs/data-sources/ptr_record_set).
+Refer to the Terraform Registry for docs: [`data_dns_ptr_record_set`](https://registry.terraform.io/providers/hashicorp/dns/3.4.1/docs/data-sources/ptr_record_set).
 '''
+from pkgutil import extend_path
+__path__ = extend_path(__path__, __name__)
+
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
 import jsii
@@ -22,15 +25,15 @@
 
 
 class DataDnsPtrRecordSet(
     _cdktf_9a9027ec.TerraformDataSource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-dns.dataDnsPtrRecordSet.DataDnsPtrRecordSet",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.0/docs/data-sources/ptr_record_set dns_ptr_record_set}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.1/docs/data-sources/ptr_record_set dns_ptr_record_set}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id: builtins.str,
         *,
         ip_address: builtins.str,
@@ -38,19 +41,19 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.0/docs/data-sources/ptr_record_set dns_ptr_record_set} Data Source.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.1/docs/data-sources/ptr_record_set dns_ptr_record_set} Data Source.
 
         :param scope: The scope in which to define this construct.
         :param id: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param ip_address: IP address to look up. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.0/docs/data-sources/ptr_record_set#ip_address DataDnsPtrRecordSet#ip_address}
+        :param ip_address: IP address to look up. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.1/docs/data-sources/ptr_record_set#ip_address DataDnsPtrRecordSet#ip_address}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -81,15 +84,15 @@
         import_from_id: builtins.str,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     ) -> _cdktf_9a9027ec.ImportableResource:
         '''Generates CDKTF code for importing a DataDnsPtrRecordSet resource upon running "cdktf plan ".
 
         :param scope: The scope in which to define this construct.
         :param import_to_id: The construct id used in the generated config for the DataDnsPtrRecordSet to import.
-        :param import_from_id: The id of the existing DataDnsPtrRecordSet that should be imported. Refer to the {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.0/docs/data-sources/ptr_record_set#import import section} in the documentation of this resource for the id to use
+        :param import_from_id: The id of the existing DataDnsPtrRecordSet that should be imported. Refer to the {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.1/docs/data-sources/ptr_record_set#import import section} in the documentation of this resource for the id to use
         :param provider: ? Optional instance of the provider where the DataDnsPtrRecordSet to import is found.
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__ca1aceba21467182773034c81224e170fcde693510fd2030ff76031d73c629cb)
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
             check_type(argname="argument import_to_id", value=import_to_id, expected_type=type_hints["import_to_id"])
             check_type(argname="argument import_from_id", value=import_from_id, expected_type=type_hints["import_from_id"])
@@ -168,15 +171,15 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param ip_address: IP address to look up. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.0/docs/data-sources/ptr_record_set#ip_address DataDnsPtrRecordSet#ip_address}
+        :param ip_address: IP address to look up. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.1/docs/data-sources/ptr_record_set#ip_address DataDnsPtrRecordSet#ip_address}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__fcf1fd55b23b7e629d56697ab8a11be420526958500797f4bdec98583deded00)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -268,15 +271,15 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def ip_address(self) -> builtins.str:
         '''IP address to look up.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.0/docs/data-sources/ptr_record_set#ip_address DataDnsPtrRecordSet#ip_address}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.1/docs/data-sources/ptr_record_set#ip_address DataDnsPtrRecordSet#ip_address}
         '''
         result = self._values.get("ip_address")
         assert result is not None, "Required property 'ip_address' is missing"
         return typing.cast(builtins.str, result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
```

### Comparing `cdktf-cdktf-provider-dns-8.0.0/src/cdktf_cdktf_provider_dns/data_dns_srv_record_set/__init__.py` & `cdktf-cdktf-provider-dns-8.0.1/src/cdktf_cdktf_provider_dns/data_dns_srv_record_set/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 '''
 # `data_dns_srv_record_set`
 
-Refer to the Terraform Registry for docs: [`data_dns_srv_record_set`](https://registry.terraform.io/providers/hashicorp/dns/3.4.0/docs/data-sources/srv_record_set).
+Refer to the Terraform Registry for docs: [`data_dns_srv_record_set`](https://registry.terraform.io/providers/hashicorp/dns/3.4.1/docs/data-sources/srv_record_set).
 '''
+from pkgutil import extend_path
+__path__ = extend_path(__path__, __name__)
+
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
 import jsii
@@ -22,15 +25,15 @@
 
 
 class DataDnsSrvRecordSet(
     _cdktf_9a9027ec.TerraformDataSource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-dns.dataDnsSrvRecordSet.DataDnsSrvRecordSet",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.0/docs/data-sources/srv_record_set dns_srv_record_set}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.1/docs/data-sources/srv_record_set dns_srv_record_set}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id: builtins.str,
         *,
         service: builtins.str,
@@ -38,19 +41,19 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.0/docs/data-sources/srv_record_set dns_srv_record_set} Data Source.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.1/docs/data-sources/srv_record_set dns_srv_record_set} Data Source.
 
         :param scope: The scope in which to define this construct.
         :param id: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param service: Service to look up. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.0/docs/data-sources/srv_record_set#service DataDnsSrvRecordSet#service}
+        :param service: Service to look up. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.1/docs/data-sources/srv_record_set#service DataDnsSrvRecordSet#service}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -81,15 +84,15 @@
         import_from_id: builtins.str,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     ) -> _cdktf_9a9027ec.ImportableResource:
         '''Generates CDKTF code for importing a DataDnsSrvRecordSet resource upon running "cdktf plan ".
 
         :param scope: The scope in which to define this construct.
         :param import_to_id: The construct id used in the generated config for the DataDnsSrvRecordSet to import.
-        :param import_from_id: The id of the existing DataDnsSrvRecordSet that should be imported. Refer to the {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.0/docs/data-sources/srv_record_set#import import section} in the documentation of this resource for the id to use
+        :param import_from_id: The id of the existing DataDnsSrvRecordSet that should be imported. Refer to the {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.1/docs/data-sources/srv_record_set#import import section} in the documentation of this resource for the id to use
         :param provider: ? Optional instance of the provider where the DataDnsSrvRecordSet to import is found.
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__f6531bd9106de7fe94aaba37d67db0ca5dc86fb6822f5c192e84f66fb15961a4)
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
             check_type(argname="argument import_to_id", value=import_to_id, expected_type=type_hints["import_to_id"])
             check_type(argname="argument import_from_id", value=import_from_id, expected_type=type_hints["import_from_id"])
@@ -168,15 +171,15 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param service: Service to look up. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.0/docs/data-sources/srv_record_set#service DataDnsSrvRecordSet#service}
+        :param service: Service to look up. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.1/docs/data-sources/srv_record_set#service DataDnsSrvRecordSet#service}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__e8e5d88426be0b98ea34a69b2a05888d2eb35258075775c0b01206258ff94272)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -268,15 +271,15 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def service(self) -> builtins.str:
         '''Service to look up.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.0/docs/data-sources/srv_record_set#service DataDnsSrvRecordSet#service}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.1/docs/data-sources/srv_record_set#service DataDnsSrvRecordSet#service}
         '''
         result = self._values.get("service")
         assert result is not None, "Required property 'service' is missing"
         return typing.cast(builtins.str, result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
```

### Comparing `cdktf-cdktf-provider-dns-8.0.0/src/cdktf_cdktf_provider_dns/data_dns_txt_record_set/__init__.py` & `cdktf-cdktf-provider-dns-8.0.1/src/cdktf_cdktf_provider_dns/data_dns_txt_record_set/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 '''
 # `data_dns_txt_record_set`
 
-Refer to the Terraform Registry for docs: [`data_dns_txt_record_set`](https://registry.terraform.io/providers/hashicorp/dns/3.4.0/docs/data-sources/txt_record_set).
+Refer to the Terraform Registry for docs: [`data_dns_txt_record_set`](https://registry.terraform.io/providers/hashicorp/dns/3.4.1/docs/data-sources/txt_record_set).
 '''
+from pkgutil import extend_path
+__path__ = extend_path(__path__, __name__)
+
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
 import jsii
@@ -22,15 +25,15 @@
 
 
 class DataDnsTxtRecordSet(
     _cdktf_9a9027ec.TerraformDataSource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-dns.dataDnsTxtRecordSet.DataDnsTxtRecordSet",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.0/docs/data-sources/txt_record_set dns_txt_record_set}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.1/docs/data-sources/txt_record_set dns_txt_record_set}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id: builtins.str,
         *,
         host: builtins.str,
@@ -38,19 +41,19 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.0/docs/data-sources/txt_record_set dns_txt_record_set} Data Source.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.1/docs/data-sources/txt_record_set dns_txt_record_set} Data Source.
 
         :param scope: The scope in which to define this construct.
         :param id: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param host: Host to look up. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.0/docs/data-sources/txt_record_set#host DataDnsTxtRecordSet#host}
+        :param host: Host to look up. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.1/docs/data-sources/txt_record_set#host DataDnsTxtRecordSet#host}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -81,15 +84,15 @@
         import_from_id: builtins.str,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     ) -> _cdktf_9a9027ec.ImportableResource:
         '''Generates CDKTF code for importing a DataDnsTxtRecordSet resource upon running "cdktf plan ".
 
         :param scope: The scope in which to define this construct.
         :param import_to_id: The construct id used in the generated config for the DataDnsTxtRecordSet to import.
-        :param import_from_id: The id of the existing DataDnsTxtRecordSet that should be imported. Refer to the {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.0/docs/data-sources/txt_record_set#import import section} in the documentation of this resource for the id to use
+        :param import_from_id: The id of the existing DataDnsTxtRecordSet that should be imported. Refer to the {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.1/docs/data-sources/txt_record_set#import import section} in the documentation of this resource for the id to use
         :param provider: ? Optional instance of the provider where the DataDnsTxtRecordSet to import is found.
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__9999db56950aec01892ac92fc94fbab533568fe7436c5be652763fd498176221)
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
             check_type(argname="argument import_to_id", value=import_to_id, expected_type=type_hints["import_to_id"])
             check_type(argname="argument import_from_id", value=import_from_id, expected_type=type_hints["import_from_id"])
@@ -173,15 +176,15 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param host: Host to look up. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.0/docs/data-sources/txt_record_set#host DataDnsTxtRecordSet#host}
+        :param host: Host to look up. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.1/docs/data-sources/txt_record_set#host DataDnsTxtRecordSet#host}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__f61abd6fb273d5267b36dde3dc223e24b8418c0ecba25b1d1c82dafbe200648f)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -273,15 +276,15 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def host(self) -> builtins.str:
         '''Host to look up.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.0/docs/data-sources/txt_record_set#host DataDnsTxtRecordSet#host}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.1/docs/data-sources/txt_record_set#host DataDnsTxtRecordSet#host}
         '''
         result = self._values.get("host")
         assert result is not None, "Required property 'host' is missing"
         return typing.cast(builtins.str, result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
```

### Comparing `cdktf-cdktf-provider-dns-8.0.0/src/cdktf_cdktf_provider_dns/mx_record_set/__init__.py` & `cdktf-cdktf-provider-dns-8.0.1/src/cdktf_cdktf_provider_dns/mx_record_set/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 '''
 # `dns_mx_record_set`
 
-Refer to the Terraform Registry for docs: [`dns_mx_record_set`](https://registry.terraform.io/providers/hashicorp/dns/3.4.0/docs/resources/mx_record_set).
+Refer to the Terraform Registry for docs: [`dns_mx_record_set`](https://registry.terraform.io/providers/hashicorp/dns/3.4.1/docs/resources/mx_record_set).
 '''
+from pkgutil import extend_path
+__path__ = extend_path(__path__, __name__)
+
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
 import jsii
@@ -22,15 +25,15 @@
 
 
 class MxRecordSet(
     _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-dns.mxRecordSet.MxRecordSet",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.0/docs/resources/mx_record_set dns_mx_record_set}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.1/docs/resources/mx_record_set dns_mx_record_set}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id: builtins.str,
         *,
         zone: builtins.str,
@@ -41,22 +44,22 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.0/docs/resources/mx_record_set dns_mx_record_set} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.1/docs/resources/mx_record_set dns_mx_record_set} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param zone: DNS zone the record set belongs to. It must be an FQDN, that is, include the trailing dot. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.0/docs/resources/mx_record_set#zone MxRecordSet#zone}
-        :param mx: mx block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.0/docs/resources/mx_record_set#mx MxRecordSet#mx}
-        :param name: The name of the record set. The ``zone`` argument will be appended to this value to create the full record path. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.0/docs/resources/mx_record_set#name MxRecordSet#name}
-        :param ttl: The TTL of the record set. Defaults to ``3600``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.0/docs/resources/mx_record_set#ttl MxRecordSet#ttl}
+        :param zone: DNS zone the record set belongs to. It must be an FQDN, that is, include the trailing dot. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.1/docs/resources/mx_record_set#zone MxRecordSet#zone}
+        :param mx: mx block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.1/docs/resources/mx_record_set#mx MxRecordSet#mx}
+        :param name: The name of the record set. The ``zone`` argument will be appended to this value to create the full record path. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.1/docs/resources/mx_record_set#name MxRecordSet#name}
+        :param ttl: The TTL of the record set. Defaults to ``3600``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.1/docs/resources/mx_record_set#ttl MxRecordSet#ttl}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -90,15 +93,15 @@
         import_from_id: builtins.str,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     ) -> _cdktf_9a9027ec.ImportableResource:
         '''Generates CDKTF code for importing a MxRecordSet resource upon running "cdktf plan ".
 
         :param scope: The scope in which to define this construct.
         :param import_to_id: The construct id used in the generated config for the MxRecordSet to import.
-        :param import_from_id: The id of the existing MxRecordSet that should be imported. Refer to the {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.0/docs/resources/mx_record_set#import import section} in the documentation of this resource for the id to use
+        :param import_from_id: The id of the existing MxRecordSet that should be imported. Refer to the {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.1/docs/resources/mx_record_set#import import section} in the documentation of this resource for the id to use
         :param provider: ? Optional instance of the provider where the MxRecordSet to import is found.
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__111ea77ef87e919ac87cbd6738177eb178a30c97fa84245b2fff4dfa1eb93bc6)
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
             check_type(argname="argument import_to_id", value=import_to_id, expected_type=type_hints["import_to_id"])
             check_type(argname="argument import_from_id", value=import_from_id, expected_type=type_hints["import_from_id"])
@@ -249,18 +252,18 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param zone: DNS zone the record set belongs to. It must be an FQDN, that is, include the trailing dot. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.0/docs/resources/mx_record_set#zone MxRecordSet#zone}
-        :param mx: mx block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.0/docs/resources/mx_record_set#mx MxRecordSet#mx}
-        :param name: The name of the record set. The ``zone`` argument will be appended to this value to create the full record path. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.0/docs/resources/mx_record_set#name MxRecordSet#name}
-        :param ttl: The TTL of the record set. Defaults to ``3600``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.0/docs/resources/mx_record_set#ttl MxRecordSet#ttl}
+        :param zone: DNS zone the record set belongs to. It must be an FQDN, that is, include the trailing dot. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.1/docs/resources/mx_record_set#zone MxRecordSet#zone}
+        :param mx: mx block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.1/docs/resources/mx_record_set#mx MxRecordSet#mx}
+        :param name: The name of the record set. The ``zone`` argument will be appended to this value to create the full record path. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.1/docs/resources/mx_record_set#name MxRecordSet#name}
+        :param ttl: The TTL of the record set. Defaults to ``3600``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.1/docs/resources/mx_record_set#ttl MxRecordSet#ttl}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__ec52a97ad6f232299e279d08e298f4d1d15ec84a55f739a2354b185a4ac6f39c)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -361,47 +364,47 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def zone(self) -> builtins.str:
         '''DNS zone the record set belongs to. It must be an FQDN, that is, include the trailing dot.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.0/docs/resources/mx_record_set#zone MxRecordSet#zone}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.1/docs/resources/mx_record_set#zone MxRecordSet#zone}
         '''
         result = self._values.get("zone")
         assert result is not None, "Required property 'zone' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def mx(
         self,
     ) -> typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List["MxRecordSetMx"]]]:
         '''mx block.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.0/docs/resources/mx_record_set#mx MxRecordSet#mx}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.1/docs/resources/mx_record_set#mx MxRecordSet#mx}
         '''
         result = self._values.get("mx")
         return typing.cast(typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List["MxRecordSetMx"]]], result)
 
     @builtins.property
     def name(self) -> typing.Optional[builtins.str]:
         '''The name of the record set.
 
         The ``zone`` argument will be appended to this value to create the full record path.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.0/docs/resources/mx_record_set#name MxRecordSet#name}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.1/docs/resources/mx_record_set#name MxRecordSet#name}
         '''
         result = self._values.get("name")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def ttl(self) -> typing.Optional[jsii.Number]:
         '''The TTL of the record set. Defaults to ``3600``.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.0/docs/resources/mx_record_set#ttl MxRecordSet#ttl}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.1/docs/resources/mx_record_set#ttl MxRecordSet#ttl}
         '''
         result = self._values.get("ttl")
         return typing.cast(typing.Optional[jsii.Number], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
@@ -418,41 +421,41 @@
     jsii_type="@cdktf/provider-dns.mxRecordSet.MxRecordSetMx",
     jsii_struct_bases=[],
     name_mapping={"exchange": "exchange", "preference": "preference"},
 )
 class MxRecordSetMx:
     def __init__(self, *, exchange: builtins.str, preference: jsii.Number) -> None:
         '''
-        :param exchange: The FQDN of the mail exchange, include the trailing dot. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.0/docs/resources/mx_record_set#exchange MxRecordSet#exchange}
-        :param preference: The preference for the record. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.0/docs/resources/mx_record_set#preference MxRecordSet#preference}
+        :param exchange: The FQDN of the mail exchange, include the trailing dot. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.1/docs/resources/mx_record_set#exchange MxRecordSet#exchange}
+        :param preference: The preference for the record. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.1/docs/resources/mx_record_set#preference MxRecordSet#preference}
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__62db89f8cd7dfd80d666fc650cddbbb0d8c9a8866c7654e8b7a20dc912ebb67a)
             check_type(argname="argument exchange", value=exchange, expected_type=type_hints["exchange"])
             check_type(argname="argument preference", value=preference, expected_type=type_hints["preference"])
         self._values: typing.Dict[builtins.str, typing.Any] = {
             "exchange": exchange,
             "preference": preference,
         }
 
     @builtins.property
     def exchange(self) -> builtins.str:
         '''The FQDN of the mail exchange, include the trailing dot.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.0/docs/resources/mx_record_set#exchange MxRecordSet#exchange}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.1/docs/resources/mx_record_set#exchange MxRecordSet#exchange}
         '''
         result = self._values.get("exchange")
         assert result is not None, "Required property 'exchange' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def preference(self) -> jsii.Number:
         '''The preference for the record.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.0/docs/resources/mx_record_set#preference MxRecordSet#preference}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.1/docs/resources/mx_record_set#preference MxRecordSet#preference}
         '''
         result = self._values.get("preference")
         assert result is not None, "Required property 'preference' is missing"
         return typing.cast(jsii.Number, result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
```

### Comparing `cdktf-cdktf-provider-dns-8.0.0/src/cdktf_cdktf_provider_dns/ns_record_set/__init__.py` & `cdktf-cdktf-provider-dns-8.0.1/src/cdktf_cdktf_provider_dns/ns_record_set/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 '''
 # `dns_ns_record_set`
 
-Refer to the Terraform Registry for docs: [`dns_ns_record_set`](https://registry.terraform.io/providers/hashicorp/dns/3.4.0/docs/resources/ns_record_set).
+Refer to the Terraform Registry for docs: [`dns_ns_record_set`](https://registry.terraform.io/providers/hashicorp/dns/3.4.1/docs/resources/ns_record_set).
 '''
+from pkgutil import extend_path
+__path__ = extend_path(__path__, __name__)
+
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
 import jsii
@@ -22,15 +25,15 @@
 
 
 class NsRecordSet(
     _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-dns.nsRecordSet.NsRecordSet",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.0/docs/resources/ns_record_set dns_ns_record_set}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.1/docs/resources/ns_record_set dns_ns_record_set}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id: builtins.str,
         *,
         name: builtins.str,
@@ -41,22 +44,22 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.0/docs/resources/ns_record_set dns_ns_record_set} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.1/docs/resources/ns_record_set dns_ns_record_set} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param name: The name of the record set. The ``zone`` argument will be appended to this value to create the full record path. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.0/docs/resources/ns_record_set#name NsRecordSet#name}
-        :param nameservers: The nameservers this record set will point to. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.0/docs/resources/ns_record_set#nameservers NsRecordSet#nameservers}
-        :param zone: DNS zone the record set belongs to. It must be an FQDN, that is, include the trailing dot. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.0/docs/resources/ns_record_set#zone NsRecordSet#zone}
-        :param ttl: The TTL of the record set. Defaults to ``3600``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.0/docs/resources/ns_record_set#ttl NsRecordSet#ttl}
+        :param name: The name of the record set. The ``zone`` argument will be appended to this value to create the full record path. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.1/docs/resources/ns_record_set#name NsRecordSet#name}
+        :param nameservers: The nameservers this record set will point to. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.1/docs/resources/ns_record_set#nameservers NsRecordSet#nameservers}
+        :param zone: DNS zone the record set belongs to. It must be an FQDN, that is, include the trailing dot. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.1/docs/resources/ns_record_set#zone NsRecordSet#zone}
+        :param ttl: The TTL of the record set. Defaults to ``3600``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.1/docs/resources/ns_record_set#ttl NsRecordSet#ttl}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -90,15 +93,15 @@
         import_from_id: builtins.str,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     ) -> _cdktf_9a9027ec.ImportableResource:
         '''Generates CDKTF code for importing a NsRecordSet resource upon running "cdktf plan ".
 
         :param scope: The scope in which to define this construct.
         :param import_to_id: The construct id used in the generated config for the NsRecordSet to import.
-        :param import_from_id: The id of the existing NsRecordSet that should be imported. Refer to the {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.0/docs/resources/ns_record_set#import import section} in the documentation of this resource for the id to use
+        :param import_from_id: The id of the existing NsRecordSet that should be imported. Refer to the {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.1/docs/resources/ns_record_set#import import section} in the documentation of this resource for the id to use
         :param provider: ? Optional instance of the provider where the NsRecordSet to import is found.
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__aaa18bc3bc88ad65e100bdec5c2a167c8d5e84260517f627b792bb37b84797d7)
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
             check_type(argname="argument import_to_id", value=import_to_id, expected_type=type_hints["import_to_id"])
             check_type(argname="argument import_from_id", value=import_from_id, expected_type=type_hints["import_from_id"])
@@ -233,18 +236,18 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param name: The name of the record set. The ``zone`` argument will be appended to this value to create the full record path. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.0/docs/resources/ns_record_set#name NsRecordSet#name}
-        :param nameservers: The nameservers this record set will point to. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.0/docs/resources/ns_record_set#nameservers NsRecordSet#nameservers}
-        :param zone: DNS zone the record set belongs to. It must be an FQDN, that is, include the trailing dot. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.0/docs/resources/ns_record_set#zone NsRecordSet#zone}
-        :param ttl: The TTL of the record set. Defaults to ``3600``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.0/docs/resources/ns_record_set#ttl NsRecordSet#ttl}
+        :param name: The name of the record set. The ``zone`` argument will be appended to this value to create the full record path. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.1/docs/resources/ns_record_set#name NsRecordSet#name}
+        :param nameservers: The nameservers this record set will point to. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.1/docs/resources/ns_record_set#nameservers NsRecordSet#nameservers}
+        :param zone: DNS zone the record set belongs to. It must be an FQDN, that is, include the trailing dot. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.1/docs/resources/ns_record_set#zone NsRecordSet#zone}
+        :param ttl: The TTL of the record set. Defaults to ``3600``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.1/docs/resources/ns_record_set#ttl NsRecordSet#ttl}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__f6a1231a3a6a7ab541c206eb7f9e24e0c86f26ee0a5c23e6f66eb0bb66fe6cd3)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -345,45 +348,45 @@
 
     @builtins.property
     def name(self) -> builtins.str:
         '''The name of the record set.
 
         The ``zone`` argument will be appended to this value to create the full record path.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.0/docs/resources/ns_record_set#name NsRecordSet#name}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.1/docs/resources/ns_record_set#name NsRecordSet#name}
         '''
         result = self._values.get("name")
         assert result is not None, "Required property 'name' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def nameservers(self) -> typing.List[builtins.str]:
         '''The nameservers this record set will point to.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.0/docs/resources/ns_record_set#nameservers NsRecordSet#nameservers}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.1/docs/resources/ns_record_set#nameservers NsRecordSet#nameservers}
         '''
         result = self._values.get("nameservers")
         assert result is not None, "Required property 'nameservers' is missing"
         return typing.cast(typing.List[builtins.str], result)
 
     @builtins.property
     def zone(self) -> builtins.str:
         '''DNS zone the record set belongs to. It must be an FQDN, that is, include the trailing dot.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.0/docs/resources/ns_record_set#zone NsRecordSet#zone}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.1/docs/resources/ns_record_set#zone NsRecordSet#zone}
         '''
         result = self._values.get("zone")
         assert result is not None, "Required property 'zone' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def ttl(self) -> typing.Optional[jsii.Number]:
         '''The TTL of the record set. Defaults to ``3600``.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.0/docs/resources/ns_record_set#ttl NsRecordSet#ttl}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.1/docs/resources/ns_record_set#ttl NsRecordSet#ttl}
         '''
         result = self._values.get("ttl")
         return typing.cast(typing.Optional[jsii.Number], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
```

### Comparing `cdktf-cdktf-provider-dns-8.0.0/src/cdktf_cdktf_provider_dns/provider/__init__.py` & `cdktf-cdktf-provider-dns-8.0.1/src/cdktf_cdktf_provider_dns/provider/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 '''
 # `provider`
 
-Refer to the Terraform Registry for docs: [`dns`](https://registry.terraform.io/providers/hashicorp/dns/3.4.0/docs).
+Refer to the Terraform Registry for docs: [`dns`](https://registry.terraform.io/providers/hashicorp/dns/3.4.1/docs).
 '''
+from pkgutil import extend_path
+__path__ = extend_path(__path__, __name__)
+
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
 import jsii
@@ -22,30 +25,30 @@
 
 
 class DnsProvider(
     _cdktf_9a9027ec.TerraformProvider,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-dns.provider.DnsProvider",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.0/docs dns}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.1/docs dns}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id: builtins.str,
         *,
         alias: typing.Optional[builtins.str] = None,
         update: typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.Sequence[typing.Union["DnsProviderUpdate", typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.0/docs dns} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.1/docs dns} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param alias: Alias name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.0/docs#alias DnsProvider#alias}
-        :param update: update block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.0/docs#update DnsProvider#update}
+        :param alias: Alias name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.1/docs#alias DnsProvider#alias}
+        :param update: update block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.1/docs#update DnsProvider#update}
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__83bf38d9ae03bfa89c25f343b9ea5329f0d370be06091b19566d6b3f6633bd21)
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
             check_type(argname="argument id", value=id, expected_type=type_hints["id"])
         config = DnsProviderConfig(alias=alias, update=update)
 
@@ -60,15 +63,15 @@
         import_from_id: builtins.str,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     ) -> _cdktf_9a9027ec.ImportableResource:
         '''Generates CDKTF code for importing a DnsProvider resource upon running "cdktf plan ".
 
         :param scope: The scope in which to define this construct.
         :param import_to_id: The construct id used in the generated config for the DnsProvider to import.
-        :param import_from_id: The id of the existing DnsProvider that should be imported. Refer to the {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.0/docs#import import section} in the documentation of this resource for the id to use
+        :param import_from_id: The id of the existing DnsProvider that should be imported. Refer to the {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.1/docs#import import section} in the documentation of this resource for the id to use
         :param provider: ? Optional instance of the provider where the DnsProvider to import is found.
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__a4a133372db4c3fef5ecf48d9669cce3c99acc83a29af21011a8768118126b0d)
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
             check_type(argname="argument import_to_id", value=import_to_id, expected_type=type_hints["import_to_id"])
             check_type(argname="argument import_from_id", value=import_from_id, expected_type=type_hints["import_from_id"])
@@ -147,16 +150,16 @@
     def __init__(
         self,
         *,
         alias: typing.Optional[builtins.str] = None,
         update: typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.Sequence[typing.Union["DnsProviderUpdate", typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
         '''
-        :param alias: Alias name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.0/docs#alias DnsProvider#alias}
-        :param update: update block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.0/docs#update DnsProvider#update}
+        :param alias: Alias name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.1/docs#alias DnsProvider#alias}
+        :param update: update block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.1/docs#update DnsProvider#update}
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__ff89cf22e9a26fed2a506744d38e6232134b31b6cade93c7995e77925523359f)
             check_type(argname="argument alias", value=alias, expected_type=type_hints["alias"])
             check_type(argname="argument update", value=update, expected_type=type_hints["update"])
         self._values: typing.Dict[builtins.str, typing.Any] = {}
         if alias is not None:
@@ -164,26 +167,26 @@
         if update is not None:
             self._values["update"] = update
 
     @builtins.property
     def alias(self) -> typing.Optional[builtins.str]:
         '''Alias name.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.0/docs#alias DnsProvider#alias}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.1/docs#alias DnsProvider#alias}
         '''
         result = self._values.get("alias")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def update(
         self,
     ) -> typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List["DnsProviderUpdate"]]]:
         '''update block.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.0/docs#update DnsProvider#update}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.1/docs#update DnsProvider#update}
         '''
         result = self._values.get("update")
         return typing.cast(typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List["DnsProviderUpdate"]]], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
@@ -222,23 +225,23 @@
         port: typing.Optional[jsii.Number] = None,
         retries: typing.Optional[jsii.Number] = None,
         server: typing.Optional[builtins.str] = None,
         timeout: typing.Optional[builtins.str] = None,
         transport: typing.Optional[builtins.str] = None,
     ) -> None:
         '''
-        :param gssapi: gssapi block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.0/docs#gssapi DnsProvider#gssapi}
-        :param key_algorithm: Required if ``key_name`` is set. When using TSIG authentication, the algorithm to use for HMAC. Valid values are ``hmac-md5``, ``hmac-sha1``, ``hmac-sha256`` or ``hmac-sha512``. Value can also be sourced from the DNS_UPDATE_KEYALGORITHM environment variable. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.0/docs#key_algorithm DnsProvider#key_algorithm}
-        :param key_name: The name of the TSIG key used to sign the DNS update messages. Value can also be sourced from the DNS_UPDATE_KEYNAME environment variable. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.0/docs#key_name DnsProvider#key_name}
-        :param key_secret: Required if ``key_name`` is set A Base64-encoded string containing the shared secret to be used for TSIG. Value can also be sourced from the DNS_UPDATE_KEYSECRET environment variable. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.0/docs#key_secret DnsProvider#key_secret}
-        :param port: The target UDP port on the server where updates are sent to. Defaults to ``53``. Value can also be sourced from the DNS_UPDATE_PORT environment variable. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.0/docs#port DnsProvider#port}
-        :param retries: How many times to retry on connection timeout. Defaults to ``3``. Value can also be sourced from the DNS_UPDATE_RETRIES environment variable. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.0/docs#retries DnsProvider#retries}
-        :param server: The hostname or IP address of the DNS server to send updates to. Value can also be sourced from the DNS_UPDATE_SERVER environment variable. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.0/docs#server DnsProvider#server}
-        :param timeout: Timeout for DNS queries. Valid values are durations expressed as ``500ms``, etc. or a plain number which is treated as whole seconds. Value can also be sourced from the DNS_UPDATE_TIMEOUT environment variable. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.0/docs#timeout DnsProvider#timeout}
-        :param transport: Transport to use for DNS queries. Valid values are ``udp``, ``udp4``, ``udp6``, ``tcp``, ``tcp4``, or ``tcp6``. Any UDP transport will retry automatically with the equivalent TCP transport in the event of a truncated response. Defaults to ``udp``. Value can also be sourced from the DNS_UPDATE_TRANSPORT environment variable. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.0/docs#transport DnsProvider#transport}
+        :param gssapi: gssapi block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.1/docs#gssapi DnsProvider#gssapi}
+        :param key_algorithm: Required if ``key_name`` is set. When using TSIG authentication, the algorithm to use for HMAC. Valid values are ``hmac-md5``, ``hmac-sha1``, ``hmac-sha256`` or ``hmac-sha512``. Value can also be sourced from the DNS_UPDATE_KEYALGORITHM environment variable. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.1/docs#key_algorithm DnsProvider#key_algorithm}
+        :param key_name: The name of the TSIG key used to sign the DNS update messages. Value can also be sourced from the DNS_UPDATE_KEYNAME environment variable. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.1/docs#key_name DnsProvider#key_name}
+        :param key_secret: Required if ``key_name`` is set A Base64-encoded string containing the shared secret to be used for TSIG. Value can also be sourced from the DNS_UPDATE_KEYSECRET environment variable. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.1/docs#key_secret DnsProvider#key_secret}
+        :param port: The target UDP port on the server where updates are sent to. Defaults to ``53``. Value can also be sourced from the DNS_UPDATE_PORT environment variable. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.1/docs#port DnsProvider#port}
+        :param retries: How many times to retry on connection timeout. Defaults to ``3``. Value can also be sourced from the DNS_UPDATE_RETRIES environment variable. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.1/docs#retries DnsProvider#retries}
+        :param server: The hostname or IP address of the DNS server to send updates to. Value can also be sourced from the DNS_UPDATE_SERVER environment variable. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.1/docs#server DnsProvider#server}
+        :param timeout: Timeout for DNS queries. Valid values are durations expressed as ``500ms``, etc. or a plain number which is treated as whole seconds. Value can also be sourced from the DNS_UPDATE_TIMEOUT environment variable. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.1/docs#timeout DnsProvider#timeout}
+        :param transport: Transport to use for DNS queries. Valid values are ``udp``, ``udp4``, ``udp6``, ``tcp``, ``tcp4``, or ``tcp6``. Any UDP transport will retry automatically with the equivalent TCP transport in the event of a truncated response. Defaults to ``udp``. Value can also be sourced from the DNS_UPDATE_TRANSPORT environment variable. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.1/docs#transport DnsProvider#transport}
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__d13f30fc44e99d87fcc72348a45e82b442b9705c51be72b7c208949a900678ea)
             check_type(argname="argument gssapi", value=gssapi, expected_type=type_hints["gssapi"])
             check_type(argname="argument key_algorithm", value=key_algorithm, expected_type=type_hints["key_algorithm"])
             check_type(argname="argument key_name", value=key_name, expected_type=type_hints["key_name"])
             check_type(argname="argument key_secret", value=key_secret, expected_type=type_hints["key_secret"])
@@ -269,103 +272,103 @@
 
     @builtins.property
     def gssapi(
         self,
     ) -> typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List["DnsProviderUpdateGssapi"]]]:
         '''gssapi block.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.0/docs#gssapi DnsProvider#gssapi}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.1/docs#gssapi DnsProvider#gssapi}
         '''
         result = self._values.get("gssapi")
         return typing.cast(typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List["DnsProviderUpdateGssapi"]]], result)
 
     @builtins.property
     def key_algorithm(self) -> typing.Optional[builtins.str]:
         '''Required if ``key_name`` is set.
 
         When using TSIG authentication, the algorithm to use for HMAC. Valid values are ``hmac-md5``, ``hmac-sha1``, ``hmac-sha256`` or ``hmac-sha512``. Value can also be sourced from the DNS_UPDATE_KEYALGORITHM environment variable.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.0/docs#key_algorithm DnsProvider#key_algorithm}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.1/docs#key_algorithm DnsProvider#key_algorithm}
         '''
         result = self._values.get("key_algorithm")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def key_name(self) -> typing.Optional[builtins.str]:
         '''The name of the TSIG key used to sign the DNS update messages.
 
         Value can also be sourced from the DNS_UPDATE_KEYNAME environment variable.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.0/docs#key_name DnsProvider#key_name}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.1/docs#key_name DnsProvider#key_name}
         '''
         result = self._values.get("key_name")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def key_secret(self) -> typing.Optional[builtins.str]:
         '''Required if ``key_name`` is set A Base64-encoded string containing the shared secret to be used for TSIG.
 
         Value can also be sourced from the DNS_UPDATE_KEYSECRET environment variable.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.0/docs#key_secret DnsProvider#key_secret}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.1/docs#key_secret DnsProvider#key_secret}
         '''
         result = self._values.get("key_secret")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def port(self) -> typing.Optional[jsii.Number]:
         '''The target UDP port on the server where updates are sent to.
 
         Defaults to ``53``. Value can also be sourced from the DNS_UPDATE_PORT environment variable.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.0/docs#port DnsProvider#port}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.1/docs#port DnsProvider#port}
         '''
         result = self._values.get("port")
         return typing.cast(typing.Optional[jsii.Number], result)
 
     @builtins.property
     def retries(self) -> typing.Optional[jsii.Number]:
         '''How many times to retry on connection timeout.
 
         Defaults to ``3``. Value can also be sourced from the DNS_UPDATE_RETRIES environment variable.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.0/docs#retries DnsProvider#retries}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.1/docs#retries DnsProvider#retries}
         '''
         result = self._values.get("retries")
         return typing.cast(typing.Optional[jsii.Number], result)
 
     @builtins.property
     def server(self) -> typing.Optional[builtins.str]:
         '''The hostname or IP address of the DNS server to send updates to.
 
         Value can also be sourced from the DNS_UPDATE_SERVER environment variable.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.0/docs#server DnsProvider#server}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.1/docs#server DnsProvider#server}
         '''
         result = self._values.get("server")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def timeout(self) -> typing.Optional[builtins.str]:
         '''Timeout for DNS queries.
 
         Valid values are durations expressed as ``500ms``, etc. or a plain number which is treated as whole seconds. Value can also be sourced from the DNS_UPDATE_TIMEOUT environment variable.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.0/docs#timeout DnsProvider#timeout}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.1/docs#timeout DnsProvider#timeout}
         '''
         result = self._values.get("timeout")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def transport(self) -> typing.Optional[builtins.str]:
         '''Transport to use for DNS queries.
 
         Valid values are ``udp``, ``udp4``, ``udp6``, ``tcp``, ``tcp4``, or ``tcp6``. Any UDP transport will retry automatically with the equivalent TCP transport in the event of a truncated response. Defaults to ``udp``. Value can also be sourced from the DNS_UPDATE_TRANSPORT environment variable.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.0/docs#transport DnsProvider#transport}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.1/docs#transport DnsProvider#transport}
         '''
         result = self._values.get("transport")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
@@ -394,18 +397,18 @@
         *,
         keytab: typing.Optional[builtins.str] = None,
         password: typing.Optional[builtins.str] = None,
         realm: typing.Optional[builtins.str] = None,
         username: typing.Optional[builtins.str] = None,
     ) -> None:
         '''
-        :param keytab: This or ``password`` is required if ``username`` is set, not supported on Windows. The path to a keytab file containing a key for ``username``. Value can also be sourced from the DNS_UPDATE_KEYTAB environment variable. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.0/docs#keytab DnsProvider#keytab}
-        :param password: This or ``keytab`` is required if ``username`` is set. The matching password for ``username``. Value can also be sourced from the DNS_UPDATE_PASSWORD environment variable. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.0/docs#password DnsProvider#password}
-        :param realm: The Kerberos realm or Active Directory domain. Value can also be sourced from the DNS_UPDATE_REALM environment variable. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.0/docs#realm DnsProvider#realm}
-        :param username: The name of the user to authenticate as. If not set the current user session will be used. Value can also be sourced from the DNS_UPDATE_USERNAME environment variable. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.0/docs#username DnsProvider#username}
+        :param keytab: This or ``password`` is required if ``username`` is set, not supported on Windows. The path to a keytab file containing a key for ``username``. Value can also be sourced from the DNS_UPDATE_KEYTAB environment variable. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.1/docs#keytab DnsProvider#keytab}
+        :param password: This or ``keytab`` is required if ``username`` is set. The matching password for ``username``. Value can also be sourced from the DNS_UPDATE_PASSWORD environment variable. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.1/docs#password DnsProvider#password}
+        :param realm: The Kerberos realm or Active Directory domain. Value can also be sourced from the DNS_UPDATE_REALM environment variable. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.1/docs#realm DnsProvider#realm}
+        :param username: The name of the user to authenticate as. If not set the current user session will be used. Value can also be sourced from the DNS_UPDATE_USERNAME environment variable. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.1/docs#username DnsProvider#username}
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__e7014d1d1021660ba17144ae563b347a69e967d0adff111c7c0a48ab98549cef)
             check_type(argname="argument keytab", value=keytab, expected_type=type_hints["keytab"])
             check_type(argname="argument password", value=password, expected_type=type_hints["password"])
             check_type(argname="argument realm", value=realm, expected_type=type_hints["realm"])
             check_type(argname="argument username", value=username, expected_type=type_hints["username"])
@@ -421,46 +424,46 @@
 
     @builtins.property
     def keytab(self) -> typing.Optional[builtins.str]:
         '''This or ``password`` is required if ``username`` is set, not supported on Windows.
 
         The path to a keytab file containing a key for ``username``. Value can also be sourced from the DNS_UPDATE_KEYTAB environment variable.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.0/docs#keytab DnsProvider#keytab}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.1/docs#keytab DnsProvider#keytab}
         '''
         result = self._values.get("keytab")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def password(self) -> typing.Optional[builtins.str]:
         '''This or ``keytab`` is required if ``username`` is set.
 
         The matching password for ``username``. Value can also be sourced from the DNS_UPDATE_PASSWORD environment variable.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.0/docs#password DnsProvider#password}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.1/docs#password DnsProvider#password}
         '''
         result = self._values.get("password")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def realm(self) -> typing.Optional[builtins.str]:
         '''The Kerberos realm or Active Directory domain. Value can also be sourced from the DNS_UPDATE_REALM environment variable.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.0/docs#realm DnsProvider#realm}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.1/docs#realm DnsProvider#realm}
         '''
         result = self._values.get("realm")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def username(self) -> typing.Optional[builtins.str]:
         '''The name of the user to authenticate as.
 
         If not set the current user session will be used. Value can also be sourced from the DNS_UPDATE_USERNAME environment variable.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.0/docs#username DnsProvider#username}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.1/docs#username DnsProvider#username}
         '''
         result = self._values.get("username")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
```

### Comparing `cdktf-cdktf-provider-dns-8.0.0/src/cdktf_cdktf_provider_dns/ptr_record/__init__.py` & `cdktf-cdktf-provider-dns-8.0.1/src/cdktf_cdktf_provider_dns/ptr_record/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 '''
 # `dns_ptr_record`
 
-Refer to the Terraform Registry for docs: [`dns_ptr_record`](https://registry.terraform.io/providers/hashicorp/dns/3.4.0/docs/resources/ptr_record).
+Refer to the Terraform Registry for docs: [`dns_ptr_record`](https://registry.terraform.io/providers/hashicorp/dns/3.4.1/docs/resources/ptr_record).
 '''
+from pkgutil import extend_path
+__path__ = extend_path(__path__, __name__)
+
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
 import jsii
@@ -22,15 +25,15 @@
 
 
 class PtrRecord(
     _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-dns.ptrRecord.PtrRecord",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.0/docs/resources/ptr_record dns_ptr_record}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.1/docs/resources/ptr_record dns_ptr_record}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id: builtins.str,
         *,
         ptr: builtins.str,
@@ -41,22 +44,22 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.0/docs/resources/ptr_record dns_ptr_record} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.1/docs/resources/ptr_record dns_ptr_record} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param ptr: The canonical name this record will point to. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.0/docs/resources/ptr_record#ptr PtrRecord#ptr}
-        :param zone: DNS zone the record set belongs to. It must be an FQDN, that is, include the trailing dot. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.0/docs/resources/ptr_record#zone PtrRecord#zone}
-        :param name: The name of the record. The ``zone`` argument will be appended to this value to create the full record path. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.0/docs/resources/ptr_record#name PtrRecord#name}
-        :param ttl: The TTL of the record. Defaults to ``3600``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.0/docs/resources/ptr_record#ttl PtrRecord#ttl}
+        :param ptr: The canonical name this record will point to. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.1/docs/resources/ptr_record#ptr PtrRecord#ptr}
+        :param zone: DNS zone the record set belongs to. It must be an FQDN, that is, include the trailing dot. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.1/docs/resources/ptr_record#zone PtrRecord#zone}
+        :param name: The name of the record. The ``zone`` argument will be appended to this value to create the full record path. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.1/docs/resources/ptr_record#name PtrRecord#name}
+        :param ttl: The TTL of the record. Defaults to ``3600``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.1/docs/resources/ptr_record#ttl PtrRecord#ttl}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -90,15 +93,15 @@
         import_from_id: builtins.str,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     ) -> _cdktf_9a9027ec.ImportableResource:
         '''Generates CDKTF code for importing a PtrRecord resource upon running "cdktf plan ".
 
         :param scope: The scope in which to define this construct.
         :param import_to_id: The construct id used in the generated config for the PtrRecord to import.
-        :param import_from_id: The id of the existing PtrRecord that should be imported. Refer to the {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.0/docs/resources/ptr_record#import import section} in the documentation of this resource for the id to use
+        :param import_from_id: The id of the existing PtrRecord that should be imported. Refer to the {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.1/docs/resources/ptr_record#import import section} in the documentation of this resource for the id to use
         :param provider: ? Optional instance of the provider where the PtrRecord to import is found.
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__cd7ed48e8f2329a4a3c7e4108ccd5f8127e2ac997b684e7f96e84c3acb3acf65)
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
             check_type(argname="argument import_to_id", value=import_to_id, expected_type=type_hints["import_to_id"])
             check_type(argname="argument import_from_id", value=import_from_id, expected_type=type_hints["import_from_id"])
@@ -237,18 +240,18 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param ptr: The canonical name this record will point to. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.0/docs/resources/ptr_record#ptr PtrRecord#ptr}
-        :param zone: DNS zone the record set belongs to. It must be an FQDN, that is, include the trailing dot. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.0/docs/resources/ptr_record#zone PtrRecord#zone}
-        :param name: The name of the record. The ``zone`` argument will be appended to this value to create the full record path. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.0/docs/resources/ptr_record#name PtrRecord#name}
-        :param ttl: The TTL of the record. Defaults to ``3600``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.0/docs/resources/ptr_record#ttl PtrRecord#ttl}
+        :param ptr: The canonical name this record will point to. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.1/docs/resources/ptr_record#ptr PtrRecord#ptr}
+        :param zone: DNS zone the record set belongs to. It must be an FQDN, that is, include the trailing dot. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.1/docs/resources/ptr_record#zone PtrRecord#zone}
+        :param name: The name of the record. The ``zone`` argument will be appended to this value to create the full record path. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.1/docs/resources/ptr_record#name PtrRecord#name}
+        :param ttl: The TTL of the record. Defaults to ``3600``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.1/docs/resources/ptr_record#ttl PtrRecord#ttl}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__b49158521f7275c89a62a7ef19fe09213221f904f5b6b549c8cbf760fa926d3b)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -348,46 +351,46 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def ptr(self) -> builtins.str:
         '''The canonical name this record will point to.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.0/docs/resources/ptr_record#ptr PtrRecord#ptr}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.1/docs/resources/ptr_record#ptr PtrRecord#ptr}
         '''
         result = self._values.get("ptr")
         assert result is not None, "Required property 'ptr' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def zone(self) -> builtins.str:
         '''DNS zone the record set belongs to. It must be an FQDN, that is, include the trailing dot.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.0/docs/resources/ptr_record#zone PtrRecord#zone}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.1/docs/resources/ptr_record#zone PtrRecord#zone}
         '''
         result = self._values.get("zone")
         assert result is not None, "Required property 'zone' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def name(self) -> typing.Optional[builtins.str]:
         '''The name of the record.
 
         The ``zone`` argument will be appended to this value to create the full record path.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.0/docs/resources/ptr_record#name PtrRecord#name}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.1/docs/resources/ptr_record#name PtrRecord#name}
         '''
         result = self._values.get("name")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def ttl(self) -> typing.Optional[jsii.Number]:
         '''The TTL of the record. Defaults to ``3600``.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.0/docs/resources/ptr_record#ttl PtrRecord#ttl}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.1/docs/resources/ptr_record#ttl PtrRecord#ttl}
         '''
         result = self._values.get("ttl")
         return typing.cast(typing.Optional[jsii.Number], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
```

### Comparing `cdktf-cdktf-provider-dns-8.0.0/src/cdktf_cdktf_provider_dns/srv_record_set/__init__.py` & `cdktf-cdktf-provider-dns-8.0.1/src/cdktf_cdktf_provider_dns/srv_record_set/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 '''
 # `dns_srv_record_set`
 
-Refer to the Terraform Registry for docs: [`dns_srv_record_set`](https://registry.terraform.io/providers/hashicorp/dns/3.4.0/docs/resources/srv_record_set).
+Refer to the Terraform Registry for docs: [`dns_srv_record_set`](https://registry.terraform.io/providers/hashicorp/dns/3.4.1/docs/resources/srv_record_set).
 '''
+from pkgutil import extend_path
+__path__ = extend_path(__path__, __name__)
+
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
 import jsii
@@ -22,15 +25,15 @@
 
 
 class SrvRecordSet(
     _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-dns.srvRecordSet.SrvRecordSet",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.0/docs/resources/srv_record_set dns_srv_record_set}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.1/docs/resources/srv_record_set dns_srv_record_set}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id: builtins.str,
         *,
         name: builtins.str,
@@ -41,22 +44,22 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.0/docs/resources/srv_record_set dns_srv_record_set} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.1/docs/resources/srv_record_set dns_srv_record_set} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param name: The name of the record set. The ``zone`` argument will be appended to this value to create the full record path. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.0/docs/resources/srv_record_set#name SrvRecordSet#name}
-        :param zone: DNS zone the record set belongs to. It must be an FQDN, that is, include the trailing dot. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.0/docs/resources/srv_record_set#zone SrvRecordSet#zone}
-        :param srv: srv block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.0/docs/resources/srv_record_set#srv SrvRecordSet#srv}
-        :param ttl: The TTL of the record set. Defaults to ``3600``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.0/docs/resources/srv_record_set#ttl SrvRecordSet#ttl}
+        :param name: The name of the record set. The ``zone`` argument will be appended to this value to create the full record path. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.1/docs/resources/srv_record_set#name SrvRecordSet#name}
+        :param zone: DNS zone the record set belongs to. It must be an FQDN, that is, include the trailing dot. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.1/docs/resources/srv_record_set#zone SrvRecordSet#zone}
+        :param srv: srv block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.1/docs/resources/srv_record_set#srv SrvRecordSet#srv}
+        :param ttl: The TTL of the record set. Defaults to ``3600``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.1/docs/resources/srv_record_set#ttl SrvRecordSet#ttl}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -90,15 +93,15 @@
         import_from_id: builtins.str,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     ) -> _cdktf_9a9027ec.ImportableResource:
         '''Generates CDKTF code for importing a SrvRecordSet resource upon running "cdktf plan ".
 
         :param scope: The scope in which to define this construct.
         :param import_to_id: The construct id used in the generated config for the SrvRecordSet to import.
-        :param import_from_id: The id of the existing SrvRecordSet that should be imported. Refer to the {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.0/docs/resources/srv_record_set#import import section} in the documentation of this resource for the id to use
+        :param import_from_id: The id of the existing SrvRecordSet that should be imported. Refer to the {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.1/docs/resources/srv_record_set#import import section} in the documentation of this resource for the id to use
         :param provider: ? Optional instance of the provider where the SrvRecordSet to import is found.
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__1ab6abb7b953934e2f9daa42ff132f2441359b64f25272423c03514a9c548957)
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
             check_type(argname="argument import_to_id", value=import_to_id, expected_type=type_hints["import_to_id"])
             check_type(argname="argument import_from_id", value=import_from_id, expected_type=type_hints["import_from_id"])
@@ -245,18 +248,18 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param name: The name of the record set. The ``zone`` argument will be appended to this value to create the full record path. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.0/docs/resources/srv_record_set#name SrvRecordSet#name}
-        :param zone: DNS zone the record set belongs to. It must be an FQDN, that is, include the trailing dot. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.0/docs/resources/srv_record_set#zone SrvRecordSet#zone}
-        :param srv: srv block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.0/docs/resources/srv_record_set#srv SrvRecordSet#srv}
-        :param ttl: The TTL of the record set. Defaults to ``3600``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.0/docs/resources/srv_record_set#ttl SrvRecordSet#ttl}
+        :param name: The name of the record set. The ``zone`` argument will be appended to this value to create the full record path. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.1/docs/resources/srv_record_set#name SrvRecordSet#name}
+        :param zone: DNS zone the record set belongs to. It must be an FQDN, that is, include the trailing dot. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.1/docs/resources/srv_record_set#zone SrvRecordSet#zone}
+        :param srv: srv block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.1/docs/resources/srv_record_set#srv SrvRecordSet#srv}
+        :param ttl: The TTL of the record set. Defaults to ``3600``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.1/docs/resources/srv_record_set#ttl SrvRecordSet#ttl}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__a6cead32c63515d033c83d20cbbfcf8c7bcd53fa2262ec6c1d0833d054ff2ada)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -358,46 +361,46 @@
 
     @builtins.property
     def name(self) -> builtins.str:
         '''The name of the record set.
 
         The ``zone`` argument will be appended to this value to create the full record path.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.0/docs/resources/srv_record_set#name SrvRecordSet#name}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.1/docs/resources/srv_record_set#name SrvRecordSet#name}
         '''
         result = self._values.get("name")
         assert result is not None, "Required property 'name' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def zone(self) -> builtins.str:
         '''DNS zone the record set belongs to. It must be an FQDN, that is, include the trailing dot.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.0/docs/resources/srv_record_set#zone SrvRecordSet#zone}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.1/docs/resources/srv_record_set#zone SrvRecordSet#zone}
         '''
         result = self._values.get("zone")
         assert result is not None, "Required property 'zone' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def srv(
         self,
     ) -> typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List["SrvRecordSetSrv"]]]:
         '''srv block.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.0/docs/resources/srv_record_set#srv SrvRecordSet#srv}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.1/docs/resources/srv_record_set#srv SrvRecordSet#srv}
         '''
         result = self._values.get("srv")
         return typing.cast(typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List["SrvRecordSetSrv"]]], result)
 
     @builtins.property
     def ttl(self) -> typing.Optional[jsii.Number]:
         '''The TTL of the record set. Defaults to ``3600``.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.0/docs/resources/srv_record_set#ttl SrvRecordSet#ttl}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.1/docs/resources/srv_record_set#ttl SrvRecordSet#ttl}
         '''
         result = self._values.get("ttl")
         return typing.cast(typing.Optional[jsii.Number], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
@@ -426,18 +429,18 @@
         *,
         port: jsii.Number,
         priority: jsii.Number,
         target: builtins.str,
         weight: jsii.Number,
     ) -> None:
         '''
-        :param port: The port for the service on the target. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.0/docs/resources/srv_record_set#port SrvRecordSet#port}
-        :param priority: The priority for the record. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.0/docs/resources/srv_record_set#priority SrvRecordSet#priority}
-        :param target: The FQDN of the target, include the trailing dot. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.0/docs/resources/srv_record_set#target SrvRecordSet#target}
-        :param weight: The weight for the record. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.0/docs/resources/srv_record_set#weight SrvRecordSet#weight}
+        :param port: The port for the service on the target. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.1/docs/resources/srv_record_set#port SrvRecordSet#port}
+        :param priority: The priority for the record. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.1/docs/resources/srv_record_set#priority SrvRecordSet#priority}
+        :param target: The FQDN of the target, include the trailing dot. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.1/docs/resources/srv_record_set#target SrvRecordSet#target}
+        :param weight: The weight for the record. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.1/docs/resources/srv_record_set#weight SrvRecordSet#weight}
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__8e3b61e2f863fa4a109ee13e90a0ecff126e73fce1309591ec6e079b4f7ad5f6)
             check_type(argname="argument port", value=port, expected_type=type_hints["port"])
             check_type(argname="argument priority", value=priority, expected_type=type_hints["priority"])
             check_type(argname="argument target", value=target, expected_type=type_hints["target"])
             check_type(argname="argument weight", value=weight, expected_type=type_hints["weight"])
@@ -448,45 +451,45 @@
             "weight": weight,
         }
 
     @builtins.property
     def port(self) -> jsii.Number:
         '''The port for the service on the target.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.0/docs/resources/srv_record_set#port SrvRecordSet#port}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.1/docs/resources/srv_record_set#port SrvRecordSet#port}
         '''
         result = self._values.get("port")
         assert result is not None, "Required property 'port' is missing"
         return typing.cast(jsii.Number, result)
 
     @builtins.property
     def priority(self) -> jsii.Number:
         '''The priority for the record.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.0/docs/resources/srv_record_set#priority SrvRecordSet#priority}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.1/docs/resources/srv_record_set#priority SrvRecordSet#priority}
         '''
         result = self._values.get("priority")
         assert result is not None, "Required property 'priority' is missing"
         return typing.cast(jsii.Number, result)
 
     @builtins.property
     def target(self) -> builtins.str:
         '''The FQDN of the target, include the trailing dot.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.0/docs/resources/srv_record_set#target SrvRecordSet#target}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.1/docs/resources/srv_record_set#target SrvRecordSet#target}
         '''
         result = self._values.get("target")
         assert result is not None, "Required property 'target' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def weight(self) -> jsii.Number:
         '''The weight for the record.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.0/docs/resources/srv_record_set#weight SrvRecordSet#weight}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.1/docs/resources/srv_record_set#weight SrvRecordSet#weight}
         '''
         result = self._values.get("weight")
         assert result is not None, "Required property 'weight' is missing"
         return typing.cast(jsii.Number, result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
```

### Comparing `cdktf-cdktf-provider-dns-8.0.0/src/cdktf_cdktf_provider_dns/txt_record_set/__init__.py` & `cdktf-cdktf-provider-dns-8.0.1/src/cdktf_cdktf_provider_dns/txt_record_set/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 '''
 # `dns_txt_record_set`
 
-Refer to the Terraform Registry for docs: [`dns_txt_record_set`](https://registry.terraform.io/providers/hashicorp/dns/3.4.0/docs/resources/txt_record_set).
+Refer to the Terraform Registry for docs: [`dns_txt_record_set`](https://registry.terraform.io/providers/hashicorp/dns/3.4.1/docs/resources/txt_record_set).
 '''
+from pkgutil import extend_path
+__path__ = extend_path(__path__, __name__)
+
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
 import jsii
@@ -22,15 +25,15 @@
 
 
 class TxtRecordSet(
     _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-dns.txtRecordSet.TxtRecordSet",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.0/docs/resources/txt_record_set dns_txt_record_set}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.1/docs/resources/txt_record_set dns_txt_record_set}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id: builtins.str,
         *,
         txt: typing.Sequence[builtins.str],
@@ -41,22 +44,22 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.0/docs/resources/txt_record_set dns_txt_record_set} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.1/docs/resources/txt_record_set dns_txt_record_set} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param txt: The text records this record set will be set to. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.0/docs/resources/txt_record_set#txt TxtRecordSet#txt}
-        :param zone: DNS zone the record set belongs to. It must be an FQDN, that is, include the trailing dot. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.0/docs/resources/txt_record_set#zone TxtRecordSet#zone}
-        :param name: The name of the record set. The ``zone`` argument will be appended to this value to create the full record path. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.0/docs/resources/txt_record_set#name TxtRecordSet#name}
-        :param ttl: The TTL of the record set. Defaults to ``3600``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.0/docs/resources/txt_record_set#ttl TxtRecordSet#ttl}
+        :param txt: The text records this record set will be set to. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.1/docs/resources/txt_record_set#txt TxtRecordSet#txt}
+        :param zone: DNS zone the record set belongs to. It must be an FQDN, that is, include the trailing dot. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.1/docs/resources/txt_record_set#zone TxtRecordSet#zone}
+        :param name: The name of the record set. The ``zone`` argument will be appended to this value to create the full record path. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.1/docs/resources/txt_record_set#name TxtRecordSet#name}
+        :param ttl: The TTL of the record set. Defaults to ``3600``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.1/docs/resources/txt_record_set#ttl TxtRecordSet#ttl}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -90,15 +93,15 @@
         import_from_id: builtins.str,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     ) -> _cdktf_9a9027ec.ImportableResource:
         '''Generates CDKTF code for importing a TxtRecordSet resource upon running "cdktf plan ".
 
         :param scope: The scope in which to define this construct.
         :param import_to_id: The construct id used in the generated config for the TxtRecordSet to import.
-        :param import_from_id: The id of the existing TxtRecordSet that should be imported. Refer to the {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.0/docs/resources/txt_record_set#import import section} in the documentation of this resource for the id to use
+        :param import_from_id: The id of the existing TxtRecordSet that should be imported. Refer to the {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.1/docs/resources/txt_record_set#import import section} in the documentation of this resource for the id to use
         :param provider: ? Optional instance of the provider where the TxtRecordSet to import is found.
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__269109e13fe050245f8ecb808aa302de2486f371e809b5c589358dc923efc9bb)
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
             check_type(argname="argument import_to_id", value=import_to_id, expected_type=type_hints["import_to_id"])
             check_type(argname="argument import_from_id", value=import_from_id, expected_type=type_hints["import_from_id"])
@@ -237,18 +240,18 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param txt: The text records this record set will be set to. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.0/docs/resources/txt_record_set#txt TxtRecordSet#txt}
-        :param zone: DNS zone the record set belongs to. It must be an FQDN, that is, include the trailing dot. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.0/docs/resources/txt_record_set#zone TxtRecordSet#zone}
-        :param name: The name of the record set. The ``zone`` argument will be appended to this value to create the full record path. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.0/docs/resources/txt_record_set#name TxtRecordSet#name}
-        :param ttl: The TTL of the record set. Defaults to ``3600``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.0/docs/resources/txt_record_set#ttl TxtRecordSet#ttl}
+        :param txt: The text records this record set will be set to. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.1/docs/resources/txt_record_set#txt TxtRecordSet#txt}
+        :param zone: DNS zone the record set belongs to. It must be an FQDN, that is, include the trailing dot. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.1/docs/resources/txt_record_set#zone TxtRecordSet#zone}
+        :param name: The name of the record set. The ``zone`` argument will be appended to this value to create the full record path. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.1/docs/resources/txt_record_set#name TxtRecordSet#name}
+        :param ttl: The TTL of the record set. Defaults to ``3600``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.1/docs/resources/txt_record_set#ttl TxtRecordSet#ttl}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__d17e9bfe665b6b04383b6279df11401d9213158e0dd640fa26830d2ae7466fbd)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -348,46 +351,46 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def txt(self) -> typing.List[builtins.str]:
         '''The text records this record set will be set to.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.0/docs/resources/txt_record_set#txt TxtRecordSet#txt}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.1/docs/resources/txt_record_set#txt TxtRecordSet#txt}
         '''
         result = self._values.get("txt")
         assert result is not None, "Required property 'txt' is missing"
         return typing.cast(typing.List[builtins.str], result)
 
     @builtins.property
     def zone(self) -> builtins.str:
         '''DNS zone the record set belongs to. It must be an FQDN, that is, include the trailing dot.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.0/docs/resources/txt_record_set#zone TxtRecordSet#zone}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.1/docs/resources/txt_record_set#zone TxtRecordSet#zone}
         '''
         result = self._values.get("zone")
         assert result is not None, "Required property 'zone' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def name(self) -> typing.Optional[builtins.str]:
         '''The name of the record set.
 
         The ``zone`` argument will be appended to this value to create the full record path.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.0/docs/resources/txt_record_set#name TxtRecordSet#name}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.1/docs/resources/txt_record_set#name TxtRecordSet#name}
         '''
         result = self._values.get("name")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def ttl(self) -> typing.Optional[jsii.Number]:
         '''The TTL of the record set. Defaults to ``3600``.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.0/docs/resources/txt_record_set#ttl TxtRecordSet#ttl}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/dns/3.4.1/docs/resources/txt_record_set#ttl TxtRecordSet#ttl}
         '''
         result = self._values.get("ttl")
         return typing.cast(typing.Optional[jsii.Number], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
```

### Comparing `cdktf-cdktf-provider-dns-8.0.0/src/cdktf_cdktf_provider_dns.egg-info/PKG-INFO` & `cdktf-cdktf-provider-dns-8.0.1/src/cdktf_cdktf_provider_dns.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdktf-cdktf-provider-dns
-Version: 8.0.0
+Version: 8.0.1
 Summary: Prebuilt dns Provider for Terraform CDK (cdktf)
 Home-page: https://github.com/cdktf/cdktf-provider-dns.git
 Author: HashiCorp
 License: MPL-2.0
 Project-URL: Source, https://github.com/cdktf/cdktf-provider-dns.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
@@ -17,17 +17,17 @@
 Classifier: Typing :: Typed
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved
 Requires-Python: ~=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# CDKTF prebuilt bindings for hashicorp/dns provider version 3.4.0
+# CDKTF prebuilt bindings for hashicorp/dns provider version 3.4.1
 
-This repo builds and publishes the [Terraform dns provider](https://registry.terraform.io/providers/hashicorp/dns/3.4.0/docs) bindings for [CDK for Terraform](https://cdk.tf).
+This repo builds and publishes the [Terraform dns provider](https://registry.terraform.io/providers/hashicorp/dns/3.4.1/docs) bindings for [CDK for Terraform](https://cdk.tf).
 
 ## Available Packages
 
 ### NPM
 
 The npm package is available at [https://www.npmjs.com/package/@cdktf/provider-dns](https://www.npmjs.com/package/@cdktf/provider-dns).
 
@@ -57,15 +57,18 @@
 </dependency>
 ```
 
 ### Go
 
 The go package is generated into the [`github.com/cdktf/cdktf-provider-dns-go`](https://github.com/cdktf/cdktf-provider-dns-go) package.
 
-`go get github.com/cdktf/cdktf-provider-dns-go/dns`
+`go get github.com/cdktf/cdktf-provider-dns-go/dns/<version>`
+
+Where `<version>` is the version of the prebuilt provider you would like to use e.g. `v11`. The full module name can be found
+within the [go.mod](https://github.com/cdktf/cdktf-provider-dns-go/blob/main/dns/go.mod#L1) file.
 
 ## Docs
 
 Find auto-generated docs for this provider here:
 
 * [Typescript](./docs/API.typescript.md)
 * [Python](./docs/API.python.md)
@@ -78,15 +81,15 @@
 ## Versioning
 
 This project is explicitly not tracking the Terraform dns provider version 1:1. In fact, it always tracks `latest` of `~> 3.2` with every release. If there are scenarios where you explicitly have to pin your provider version, you can do so by [generating the provider constructs manually](https://cdk.tf/imports).
 
 These are the upstream dependencies:
 
 * [CDK for Terraform](https://cdk.tf)
-* [Terraform dns provider](https://registry.terraform.io/providers/hashicorp/dns/3.4.0)
+* [Terraform dns provider](https://registry.terraform.io/providers/hashicorp/dns/3.4.1)
 * [Terraform Engine](https://terraform.io)
 
 If there are breaking changes (backward incompatible) in any of the above, the major version of this project will be bumped.
 
 ## Features / Issues / Bugs
 
 Please report bugs and issues to the [CDK for Terraform](https://cdk.tf) project:
```

### Comparing `cdktf-cdktf-provider-dns-8.0.0/src/cdktf_cdktf_provider_dns.egg-info/SOURCES.txt` & `cdktf-cdktf-provider-dns-8.0.1/src/cdktf_cdktf_provider_dns.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 src/cdktf_cdktf_provider_dns/py.typed
 src/cdktf_cdktf_provider_dns.egg-info/PKG-INFO
 src/cdktf_cdktf_provider_dns.egg-info/SOURCES.txt
 src/cdktf_cdktf_provider_dns.egg-info/dependency_links.txt
 src/cdktf_cdktf_provider_dns.egg-info/requires.txt
 src/cdktf_cdktf_provider_dns.egg-info/top_level.txt
 src/cdktf_cdktf_provider_dns/_jsii/__init__.py
-src/cdktf_cdktf_provider_dns/_jsii/provider-dns@8.0.0.jsii.tgz
+src/cdktf_cdktf_provider_dns/_jsii/provider-dns@8.0.1.jsii.tgz
 src/cdktf_cdktf_provider_dns/a_record_set/__init__.py
 src/cdktf_cdktf_provider_dns/aaaa_record_set/__init__.py
 src/cdktf_cdktf_provider_dns/cname_record/__init__.py
 src/cdktf_cdktf_provider_dns/data_dns_a_record_set/__init__.py
 src/cdktf_cdktf_provider_dns/data_dns_aaaa_record_set/__init__.py
 src/cdktf_cdktf_provider_dns/data_dns_cname_record_set/__init__.py
 src/cdktf_cdktf_provider_dns/data_dns_mx_record_set/__init__.py
```

