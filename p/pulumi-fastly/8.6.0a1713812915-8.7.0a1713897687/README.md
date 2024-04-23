# Comparing `tmp/pulumi_fastly-8.6.0a1713812915.tar.gz` & `tmp/pulumi_fastly-8.7.0a1713897687.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_fastly-8.6.0a1713812915.tar", last modified: Mon Apr 22 19:12:52 2024, max compression
+gzip compressed data, was "pulumi_fastly-8.7.0a1713897687.tar", last modified: Tue Apr 23 19:11:31 2024, max compression
```

## Comparing `pulumi_fastly-8.6.0a1713812915.tar` & `pulumi_fastly-8.7.0a1713897687.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 19:12:52.846125 pulumi_fastly-8.6.0a1713812915/
--rw-r--r--   0 runner    (1001) docker     (127)     2812 2024-04-22 19:12:52.846125 pulumi_fastly-8.6.0a1713812915/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2360 2024-04-22 19:12:46.000000 pulumi_fastly-8.6.0a1713812915/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 19:12:52.846125 pulumi_fastly-8.6.0a1713812915/pulumi_fastly/
--rw-r--r--   0 runner    (1001) docker     (127)     5734 2024-04-22 19:12:46.000000 pulumi_fastly-8.6.0a1713812915/pulumi_fastly/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   521999 2024-04-22 19:12:46.000000 pulumi_fastly-8.6.0a1713812915/pulumi_fastly/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-04-22 19:12:46.000000 pulumi_fastly-8.6.0a1713812915/pulumi_fastly/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)    24259 2024-04-22 19:12:46.000000 pulumi_fastly-8.6.0a1713812915/pulumi_fastly/alert.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 19:12:52.846125 pulumi_fastly-8.6.0a1713812915/pulumi_fastly/config/
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-22 19:12:46.000000 pulumi_fastly-8.6.0a1713812915/pulumi_fastly/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      936 2024-04-22 19:12:46.000000 pulumi_fastly-8.6.0a1713812915/pulumi_fastly/config/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1455 2024-04-22 19:12:46.000000 pulumi_fastly-8.6.0a1713812915/pulumi_fastly/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (127)    13129 2024-04-22 19:12:46.000000 pulumi_fastly-8.6.0a1713812915/pulumi_fastly/configstore.py
--rw-r--r--   0 runner    (1001) docker     (127)    11396 2024-04-22 19:12:46.000000 pulumi_fastly-8.6.0a1713812915/pulumi_fastly/configstore_entries.py
--rw-r--r--   0 runner    (1001) docker     (127)     2479 2024-04-22 19:12:46.000000 pulumi_fastly-8.6.0a1713812915/pulumi_fastly/get_configstores.py
--rw-r--r--   0 runner    (1001) docker     (127)     2536 2024-04-22 19:12:46.000000 pulumi_fastly-8.6.0a1713812915/pulumi_fastly/get_datacenters.py
--rw-r--r--   0 runner    (1001) docker     (127)     6367 2024-04-22 19:12:46.000000 pulumi_fastly-8.6.0a1713812915/pulumi_fastly/get_dictionaries.py
--rw-r--r--   0 runner    (1001) docker     (127)     4575 2024-04-22 19:12:46.000000 pulumi_fastly-8.6.0a1713812915/pulumi_fastly/get_fastly_ip_ranges.py
--rw-r--r--   0 runner    (1001) docker     (127)     2399 2024-04-22 19:12:46.000000 pulumi_fastly-8.6.0a1713812915/pulumi_fastly/get_kvstores.py
--rw-r--r--   0 runner    (1001) docker     (127)     5821 2024-04-22 19:12:46.000000 pulumi_fastly-8.6.0a1713812915/pulumi_fastly/get_package_hash.py
--rw-r--r--   0 runner    (1001) docker     (127)     2480 2024-04-22 19:12:46.000000 pulumi_fastly-8.6.0a1713812915/pulumi_fastly/get_secretstores.py
--rw-r--r--   0 runner    (1001) docker     (127)     3072 2024-04-22 19:12:46.000000 pulumi_fastly-8.6.0a1713812915/pulumi_fastly/get_services.py
--rw-r--r--   0 runner    (1001) docker     (127)     6799 2024-04-22 19:12:46.000000 pulumi_fastly-8.6.0a1713812915/pulumi_fastly/get_tls_activation.py
--rw-r--r--   0 runner    (1001) docker     (127)     4372 2024-04-22 19:12:46.000000 pulumi_fastly-8.6.0a1713812915/pulumi_fastly/get_tls_activation_ids.py
--rw-r--r--   0 runner    (1001) docker     (127)     9956 2024-04-22 19:12:46.000000 pulumi_fastly-8.6.0a1713812915/pulumi_fastly/get_tls_certificate.py
--rw-r--r--   0 runner    (1001) docker     (127)     3181 2024-04-22 19:12:46.000000 pulumi_fastly-8.6.0a1713812915/pulumi_fastly/get_tls_certificate_ids.py
--rw-r--r--   0 runner    (1001) docker     (127)    10747 2024-04-22 19:12:46.000000 pulumi_fastly-8.6.0a1713812915/pulumi_fastly/get_tls_configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     3234 2024-04-22 19:12:46.000000 pulumi_fastly-8.6.0a1713812915/pulumi_fastly/get_tls_configuration_ids.py
--rw-r--r--   0 runner    (1001) docker     (127)     5207 2024-04-22 19:12:46.000000 pulumi_fastly-8.6.0a1713812915/pulumi_fastly/get_tls_domain.py
--rw-r--r--   0 runner    (1001) docker     (127)     8137 2024-04-22 19:12:46.000000 pulumi_fastly-8.6.0a1713812915/pulumi_fastly/get_tls_platform_certificate.py
--rw-r--r--   0 runner    (1001) docker     (127)     3380 2024-04-22 19:12:46.000000 pulumi_fastly-8.6.0a1713812915/pulumi_fastly/get_tls_platform_certificate_ids.py
--rw-r--r--   0 runner    (1001) docker     (127)     8652 2024-04-22 19:12:46.000000 pulumi_fastly-8.6.0a1713812915/pulumi_fastly/get_tls_private_key.py
--rw-r--r--   0 runner    (1001) docker     (127)     3095 2024-04-22 19:12:46.000000 pulumi_fastly-8.6.0a1713812915/pulumi_fastly/get_tls_private_key_ids.py
--rw-r--r--   0 runner    (1001) docker     (127)     8453 2024-04-22 19:12:46.000000 pulumi_fastly-8.6.0a1713812915/pulumi_fastly/get_tls_subscription.py
--rw-r--r--   0 runner    (1001) docker     (127)     3407 2024-04-22 19:12:46.000000 pulumi_fastly-8.6.0a1713812915/pulumi_fastly/get_tls_subscription_ids.py
--rw-r--r--   0 runner    (1001) docker     (127)     3788 2024-04-22 19:12:46.000000 pulumi_fastly-8.6.0a1713812915/pulumi_fastly/get_vcl_snippets.py
--rw-r--r--   0 runner    (1001) docker     (127)     6294 2024-04-22 19:12:46.000000 pulumi_fastly-8.6.0a1713812915/pulumi_fastly/get_waf_rules.py
--rw-r--r--   0 runner    (1001) docker     (127)    14020 2024-04-22 19:12:46.000000 pulumi_fastly-8.6.0a1713812915/pulumi_fastly/kvstore.py
--rw-r--r--   0 runner    (1001) docker     (127)   472172 2024-04-22 19:12:46.000000 pulumi_fastly-8.6.0a1713812915/pulumi_fastly/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     8428 2024-04-22 19:12:46.000000 pulumi_fastly-8.6.0a1713812915/pulumi_fastly/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-22 19:12:46.000000 pulumi_fastly-8.6.0a1713812915/pulumi_fastly/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 19:12:46.000000 pulumi_fastly-8.6.0a1713812915/pulumi_fastly/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    10422 2024-04-22 19:12:46.000000 pulumi_fastly-8.6.0a1713812915/pulumi_fastly/secretstore.py
--rw-r--r--   0 runner    (1001) docker     (127)    13994 2024-04-22 19:12:46.000000 pulumi_fastly-8.6.0a1713812915/pulumi_fastly/service_acl_entries.py
--rw-r--r--   0 runner    (1001) docker     (127)    11875 2024-04-22 19:12:46.000000 pulumi_fastly-8.6.0a1713812915/pulumi_fastly/service_authorization.py
--rw-r--r--   0 runner    (1001) docker     (127)    97702 2024-04-22 19:12:46.000000 pulumi_fastly-8.6.0a1713812915/pulumi_fastly/service_compute.py
--rw-r--r--   0 runner    (1001) docker     (127)    14051 2024-04-22 19:12:46.000000 pulumi_fastly-8.6.0a1713812915/pulumi_fastly/service_dictionary_items.py
--rw-r--r--   0 runner    (1001) docker     (127)    14248 2024-04-22 19:12:46.000000 pulumi_fastly-8.6.0a1713812915/pulumi_fastly/service_dynamic_snippet_content.py
--rw-r--r--   0 runner    (1001) docker     (127)   131072 2024-04-22 19:12:46.000000 pulumi_fastly-8.6.0a1713812915/pulumi_fastly/service_vcl.py
--rw-r--r--   0 runner    (1001) docker     (127)    92456 2024-04-22 19:12:46.000000 pulumi_fastly-8.6.0a1713812915/pulumi_fastly/service_waf_configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)    18128 2024-04-22 19:12:46.000000 pulumi_fastly-8.6.0a1713812915/pulumi_fastly/tls_activation.py
--rw-r--r--   0 runner    (1001) docker     (127)    23105 2024-04-22 19:12:46.000000 pulumi_fastly-8.6.0a1713812915/pulumi_fastly/tls_certificate.py
--rw-r--r--   0 runner    (1001) docker     (127)    22173 2024-04-22 19:12:46.000000 pulumi_fastly-8.6.0a1713812915/pulumi_fastly/tls_mutual_authentication.py
--rw-r--r--   0 runner    (1001) docker     (127)    26020 2024-04-22 19:12:46.000000 pulumi_fastly-8.6.0a1713812915/pulumi_fastly/tls_platform_certificate.py
--rw-r--r--   0 runner    (1001) docker     (127)    14563 2024-04-22 19:12:46.000000 pulumi_fastly-8.6.0a1713812915/pulumi_fastly/tls_private_key.py
--rw-r--r--   0 runner    (1001) docker     (127)    35184 2024-04-22 19:12:46.000000 pulumi_fastly-8.6.0a1713812915/pulumi_fastly/tls_subscription.py
--rw-r--r--   0 runner    (1001) docker     (127)     7241 2024-04-22 19:12:46.000000 pulumi_fastly-8.6.0a1713812915/pulumi_fastly/tls_subscription_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)    11794 2024-04-22 19:12:46.000000 pulumi_fastly-8.6.0a1713812915/pulumi_fastly/user.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 19:12:52.846125 pulumi_fastly-8.6.0a1713812915/pulumi_fastly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2812 2024-04-22 19:12:52.000000 pulumi_fastly-8.6.0a1713812915/pulumi_fastly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2043 2024-04-22 19:12:52.000000 pulumi_fastly-8.6.0a1713812915/pulumi_fastly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 19:12:52.000000 pulumi_fastly-8.6.0a1713812915/pulumi_fastly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-22 19:12:52.000000 pulumi_fastly-8.6.0a1713812915/pulumi_fastly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-22 19:12:52.000000 pulumi_fastly-8.6.0a1713812915/pulumi_fastly.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      679 2024-04-22 19:12:46.000000 pulumi_fastly-8.6.0a1713812915/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 19:12:52.846125 pulumi_fastly-8.6.0a1713812915/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:11:31.756826 pulumi_fastly-8.7.0a1713897687/
+-rw-r--r--   0 runner    (1001) docker     (127)     2812 2024-04-23 19:11:31.756826 pulumi_fastly-8.7.0a1713897687/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2360 2024-04-23 19:11:23.000000 pulumi_fastly-8.7.0a1713897687/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:11:31.756826 pulumi_fastly-8.7.0a1713897687/pulumi_fastly/
+-rw-r--r--   0 runner    (1001) docker     (127)     5734 2024-04-23 19:11:23.000000 pulumi_fastly-8.7.0a1713897687/pulumi_fastly/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   521901 2024-04-23 19:11:23.000000 pulumi_fastly-8.7.0a1713897687/pulumi_fastly/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-04-23 19:11:23.000000 pulumi_fastly-8.7.0a1713897687/pulumi_fastly/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24103 2024-04-23 19:11:23.000000 pulumi_fastly-8.7.0a1713897687/pulumi_fastly/alert.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:11:31.756826 pulumi_fastly-8.7.0a1713897687/pulumi_fastly/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-23 19:11:23.000000 pulumi_fastly-8.7.0a1713897687/pulumi_fastly/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      936 2024-04-23 19:11:23.000000 pulumi_fastly-8.7.0a1713897687/pulumi_fastly/config/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1455 2024-04-23 19:11:23.000000 pulumi_fastly-8.7.0a1713897687/pulumi_fastly/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12973 2024-04-23 19:11:23.000000 pulumi_fastly-8.7.0a1713897687/pulumi_fastly/configstore.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11396 2024-04-23 19:11:23.000000 pulumi_fastly-8.7.0a1713897687/pulumi_fastly/configstore_entries.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2479 2024-04-23 19:11:23.000000 pulumi_fastly-8.7.0a1713897687/pulumi_fastly/get_configstores.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2536 2024-04-23 19:11:23.000000 pulumi_fastly-8.7.0a1713897687/pulumi_fastly/get_datacenters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6227 2024-04-23 19:11:23.000000 pulumi_fastly-8.7.0a1713897687/pulumi_fastly/get_dictionaries.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4435 2024-04-23 19:11:23.000000 pulumi_fastly-8.7.0a1713897687/pulumi_fastly/get_fastly_ip_ranges.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2399 2024-04-23 19:11:23.000000 pulumi_fastly-8.7.0a1713897687/pulumi_fastly/get_kvstores.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5681 2024-04-23 19:11:23.000000 pulumi_fastly-8.7.0a1713897687/pulumi_fastly/get_package_hash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2480 2024-04-23 19:11:23.000000 pulumi_fastly-8.7.0a1713897687/pulumi_fastly/get_secretstores.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3072 2024-04-23 19:11:23.000000 pulumi_fastly-8.7.0a1713897687/pulumi_fastly/get_services.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6659 2024-04-23 19:11:23.000000 pulumi_fastly-8.7.0a1713897687/pulumi_fastly/get_tls_activation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4232 2024-04-23 19:11:23.000000 pulumi_fastly-8.7.0a1713897687/pulumi_fastly/get_tls_activation_ids.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9816 2024-04-23 19:11:23.000000 pulumi_fastly-8.7.0a1713897687/pulumi_fastly/get_tls_certificate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3041 2024-04-23 19:11:23.000000 pulumi_fastly-8.7.0a1713897687/pulumi_fastly/get_tls_certificate_ids.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10607 2024-04-23 19:11:23.000000 pulumi_fastly-8.7.0a1713897687/pulumi_fastly/get_tls_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3094 2024-04-23 19:11:23.000000 pulumi_fastly-8.7.0a1713897687/pulumi_fastly/get_tls_configuration_ids.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5067 2024-04-23 19:11:23.000000 pulumi_fastly-8.7.0a1713897687/pulumi_fastly/get_tls_domain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7997 2024-04-23 19:11:23.000000 pulumi_fastly-8.7.0a1713897687/pulumi_fastly/get_tls_platform_certificate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3240 2024-04-23 19:11:23.000000 pulumi_fastly-8.7.0a1713897687/pulumi_fastly/get_tls_platform_certificate_ids.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8512 2024-04-23 19:11:23.000000 pulumi_fastly-8.7.0a1713897687/pulumi_fastly/get_tls_private_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2955 2024-04-23 19:11:23.000000 pulumi_fastly-8.7.0a1713897687/pulumi_fastly/get_tls_private_key_ids.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8313 2024-04-23 19:11:23.000000 pulumi_fastly-8.7.0a1713897687/pulumi_fastly/get_tls_subscription.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3267 2024-04-23 19:11:23.000000 pulumi_fastly-8.7.0a1713897687/pulumi_fastly/get_tls_subscription_ids.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3788 2024-04-23 19:11:23.000000 pulumi_fastly-8.7.0a1713897687/pulumi_fastly/get_vcl_snippets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6294 2024-04-23 19:11:23.000000 pulumi_fastly-8.7.0a1713897687/pulumi_fastly/get_waf_rules.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13864 2024-04-23 19:11:23.000000 pulumi_fastly-8.7.0a1713897687/pulumi_fastly/kvstore.py
+-rw-r--r--   0 runner    (1001) docker     (127)   472074 2024-04-23 19:11:23.000000 pulumi_fastly-8.7.0a1713897687/pulumi_fastly/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8428 2024-04-23 19:11:23.000000 pulumi_fastly-8.7.0a1713897687/pulumi_fastly/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-23 19:11:23.000000 pulumi_fastly-8.7.0a1713897687/pulumi_fastly/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 19:11:23.000000 pulumi_fastly-8.7.0a1713897687/pulumi_fastly/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    10266 2024-04-23 19:11:23.000000 pulumi_fastly-8.7.0a1713897687/pulumi_fastly/secretstore.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13994 2024-04-23 19:11:23.000000 pulumi_fastly-8.7.0a1713897687/pulumi_fastly/service_acl_entries.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11719 2024-04-23 19:11:23.000000 pulumi_fastly-8.7.0a1713897687/pulumi_fastly/service_authorization.py
+-rw-r--r--   0 runner    (1001) docker     (127)    97303 2024-04-23 19:11:23.000000 pulumi_fastly-8.7.0a1713897687/pulumi_fastly/service_compute.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14051 2024-04-23 19:11:23.000000 pulumi_fastly-8.7.0a1713897687/pulumi_fastly/service_dictionary_items.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14248 2024-04-23 19:11:23.000000 pulumi_fastly-8.7.0a1713897687/pulumi_fastly/service_dynamic_snippet_content.py
+-rw-r--r--   0 runner    (1001) docker     (127)   126107 2024-04-23 19:11:23.000000 pulumi_fastly-8.7.0a1713897687/pulumi_fastly/service_vcl.py
+-rw-r--r--   0 runner    (1001) docker     (127)    91888 2024-04-23 19:11:23.000000 pulumi_fastly-8.7.0a1713897687/pulumi_fastly/service_waf_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17972 2024-04-23 19:11:23.000000 pulumi_fastly-8.7.0a1713897687/pulumi_fastly/tls_activation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22949 2024-04-23 19:11:23.000000 pulumi_fastly-8.7.0a1713897687/pulumi_fastly/tls_certificate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22173 2024-04-23 19:11:23.000000 pulumi_fastly-8.7.0a1713897687/pulumi_fastly/tls_mutual_authentication.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25864 2024-04-23 19:11:23.000000 pulumi_fastly-8.7.0a1713897687/pulumi_fastly/tls_platform_certificate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14407 2024-04-23 19:11:23.000000 pulumi_fastly-8.7.0a1713897687/pulumi_fastly/tls_private_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35184 2024-04-23 19:11:23.000000 pulumi_fastly-8.7.0a1713897687/pulumi_fastly/tls_subscription.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7241 2024-04-23 19:11:23.000000 pulumi_fastly-8.7.0a1713897687/pulumi_fastly/tls_subscription_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11638 2024-04-23 19:11:23.000000 pulumi_fastly-8.7.0a1713897687/pulumi_fastly/user.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:11:31.756826 pulumi_fastly-8.7.0a1713897687/pulumi_fastly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2812 2024-04-23 19:11:31.000000 pulumi_fastly-8.7.0a1713897687/pulumi_fastly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2043 2024-04-23 19:11:31.000000 pulumi_fastly-8.7.0a1713897687/pulumi_fastly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 19:11:31.000000 pulumi_fastly-8.7.0a1713897687/pulumi_fastly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-23 19:11:31.000000 pulumi_fastly-8.7.0a1713897687/pulumi_fastly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-23 19:11:31.000000 pulumi_fastly-8.7.0a1713897687/pulumi_fastly.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      679 2024-04-23 19:11:23.000000 pulumi_fastly-8.7.0a1713897687/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 19:11:31.756826 pulumi_fastly-8.7.0a1713897687/setup.cfg
```

### Comparing `pulumi_fastly-8.6.0a1713812915/PKG-INFO` & `pulumi_fastly-8.7.0a1713897687/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_fastly
-Version: 8.6.0a1713812915
+Version: 8.7.0a1713897687
 Summary: A Pulumi package for creating and managing fastly cloud resources.
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.io
 Project-URL: Repository, https://github.com/pulumi/pulumi-fastly
 Keywords: pulumi,fastly
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_fastly-8.6.0a1713812915/README.md` & `pulumi_fastly-8.7.0a1713897687/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.6.0a1713812915/pulumi_fastly/__init__.py` & `pulumi_fastly-8.7.0a1713897687/pulumi_fastly/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.6.0a1713812915/pulumi_fastly/_inputs.py` & `pulumi_fastly-8.7.0a1713897687/pulumi_fastly/_inputs.py`

 * *Files 0% similar despite different names*

```diff
@@ -11471,39 +11471,39 @@
 @pulumi.input_type
 class ServiceVclRateLimiterResponseArgs:
     def __init__(__self__, *,
                  content: pulumi.Input[str],
                  content_type: pulumi.Input[str],
                  status: pulumi.Input[int]):
         """
-        :param pulumi.Input[str] content: The VCL code that specifies exactly what the snippet does
-        :param pulumi.Input[str] content_type: Value of the `Content-Type` header sent with the request
+        :param pulumi.Input[str] content: HTTP response body data
+        :param pulumi.Input[str] content_type: HTTP Content-Type (e.g. application/json)
         :param pulumi.Input[int] status: HTTP response status code (e.g. 429)
         """
         pulumi.set(__self__, "content", content)
         pulumi.set(__self__, "content_type", content_type)
         pulumi.set(__self__, "status", status)
 
     @property
     @pulumi.getter
     def content(self) -> pulumi.Input[str]:
         """
-        The VCL code that specifies exactly what the snippet does
+        HTTP response body data
         """
         return pulumi.get(self, "content")
 
     @content.setter
     def content(self, value: pulumi.Input[str]):
         pulumi.set(self, "content", value)
 
     @property
     @pulumi.getter(name="contentType")
     def content_type(self) -> pulumi.Input[str]:
         """
-        Value of the `Content-Type` header sent with the request
+        HTTP Content-Type (e.g. application/json)
         """
         return pulumi.get(self, "content_type")
 
     @content_type.setter
     def content_type(self, value: pulumi.Input[str]):
         pulumi.set(self, "content_type", value)
```

### Comparing `pulumi_fastly-8.6.0a1713812915/pulumi_fastly/_utilities.py` & `pulumi_fastly-8.7.0a1713897687/pulumi_fastly/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.6.0a1713812915/pulumi_fastly/alert.py` & `pulumi_fastly-8.7.0a1713897687/pulumi_fastly/alert.py`

 * *Files 1% similar despite different names*

```diff
@@ -296,15 +296,14 @@
                  source: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         Provides a Fastly Alert. Alerts send notifications to custom integrations (e.g., Slack channels, PagerDuty, Microsoft Teams and New Relic) when an observed metric either exceeds or falls below a threshold.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_fastly as fastly
 
         example = fastly.ServiceVcl("example", name="my_vcl_service")
         example_alert = fastly.Alert("example",
             name="my_vcl_service errors",
@@ -313,15 +312,14 @@
             metric="status_5xx",
             evaluation_strategy=fastly.AlertEvaluationStrategyArgs(
                 type="above_threshold",
                 period="5m",
                 threshold=10,
             ))
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Fastly Alerts can be imported using their ID, e.g.
 
         ```sh
         $ pulumi import fastly:index/alert:Alert example xxxxxxxxxxxxxxxxxxxx
@@ -345,15 +343,14 @@
                  args: AlertArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         Provides a Fastly Alert. Alerts send notifications to custom integrations (e.g., Slack channels, PagerDuty, Microsoft Teams and New Relic) when an observed metric either exceeds or falls below a threshold.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_fastly as fastly
 
         example = fastly.ServiceVcl("example", name="my_vcl_service")
         example_alert = fastly.Alert("example",
             name="my_vcl_service errors",
@@ -362,15 +359,14 @@
             metric="status_5xx",
             evaluation_strategy=fastly.AlertEvaluationStrategyArgs(
                 type="above_threshold",
                 period="5m",
                 threshold=10,
             ))
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Fastly Alerts can be imported using their ID, e.g.
 
         ```sh
         $ pulumi import fastly:index/alert:Alert example xxxxxxxxxxxxxxxxxxxx
```

### Comparing `pulumi_fastly-8.6.0a1713812915/pulumi_fastly/config/__init__.pyi` & `pulumi_fastly-8.7.0a1713897687/pulumi_fastly/config/__init__.pyi`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.6.0a1713812915/pulumi_fastly/config/vars.py` & `pulumi_fastly-8.7.0a1713897687/pulumi_fastly/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.6.0a1713812915/pulumi_fastly/configstore.py` & `pulumi_fastly-8.7.0a1713897687/pulumi_fastly/configstore.py`

 * *Files 2% similar despite different names*

```diff
@@ -104,15 +104,14 @@
 
         In order for a Config Store (`Configstore`) to be accessible to a [Compute](https://developer.fastly.com/learning/compute/) service you'll first need to define a Compute service (`ServiceCompute`) in your configuration, and then create a link to the Config Store from within the service using the `resource_link` block (shown in the below examples).
 
         ## Example Usage
 
         Basic usage:
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_fastly as fastly
 
         # IMPORTANT: Deleting a Config Store requires first deleting its resource_link.
         # This requires a two-step `pulumi up` as we can't guarantee deletion order.
         # e.g. resource_link deletion within fastly_service_compute might not finish first.
@@ -129,15 +128,14 @@
             ),
             resource_links=[fastly.ServiceComputeResourceLinkArgs(
                 name="my_resource_link",
                 resource_id=example_configstore.id,
             )],
             force_destroy=True)
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Fastly Config Stores can be imported using their Store ID, e.g.
 
         ```sh
         $ pulumi import fastly:index/configstore:Configstore example xxxxxxxxxxxxxxxxxxxx
@@ -159,15 +157,14 @@
 
         In order for a Config Store (`Configstore`) to be accessible to a [Compute](https://developer.fastly.com/learning/compute/) service you'll first need to define a Compute service (`ServiceCompute`) in your configuration, and then create a link to the Config Store from within the service using the `resource_link` block (shown in the below examples).
 
         ## Example Usage
 
         Basic usage:
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_fastly as fastly
 
         # IMPORTANT: Deleting a Config Store requires first deleting its resource_link.
         # This requires a two-step `pulumi up` as we can't guarantee deletion order.
         # e.g. resource_link deletion within fastly_service_compute might not finish first.
@@ -184,15 +181,14 @@
             ),
             resource_links=[fastly.ServiceComputeResourceLinkArgs(
                 name="my_resource_link",
                 resource_id=example_configstore.id,
             )],
             force_destroy=True)
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Fastly Config Stores can be imported using their Store ID, e.g.
 
         ```sh
         $ pulumi import fastly:index/configstore:Configstore example xxxxxxxxxxxxxxxxxxxx
```

### Comparing `pulumi_fastly-8.6.0a1713812915/pulumi_fastly/configstore_entries.py` & `pulumi_fastly-8.7.0a1713897687/pulumi_fastly/configstore_entries.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.6.0a1713812915/pulumi_fastly/get_configstores.py` & `pulumi_fastly-8.7.0a1713897687/pulumi_fastly/get_configstores.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.6.0a1713812915/pulumi_fastly/get_datacenters.py` & `pulumi_fastly-8.7.0a1713897687/pulumi_fastly/get_datacenters.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.6.0a1713812915/pulumi_fastly/get_dictionaries.py` & `pulumi_fastly-8.7.0a1713897687/pulumi_fastly/get_dictionaries.py`

 * *Files 2% similar despite different names*

```diff
@@ -85,15 +85,14 @@
                      service_version: Optional[int] = None,
                      opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetDictionariesResult:
     """
     Use this data source to get a list of [Fastly dictionaries](https://developer.fastly.com/reference/api/dictionaries/) for the specified service/version.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_fastly as fastly
 
     example_service_vcl = fastly.ServiceVcl("example",
         name="Example Service",
         domains=[fastly.ServiceVclDomainArgs(
@@ -111,15 +110,14 @@
             ),
         ],
         force_destroy=True)
     example = fastly.get_dictionaries_output(service_id=example_service_vcl.id,
         service_version=example_service_vcl.active_version)
     pulumi.export("serviceDictionaries", example)
     ```
-    <!--End PulumiCodeChooser -->
 
     [1]: https://developer.fastly.com/reference/api/dictionaries/
 
 
     :param str service_id: Alphanumeric string identifying the service.
     :param int service_version: Integer identifying a service version.
     """
@@ -141,15 +139,14 @@
                             service_version: Optional[pulumi.Input[int]] = None,
                             opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetDictionariesResult]:
     """
     Use this data source to get a list of [Fastly dictionaries](https://developer.fastly.com/reference/api/dictionaries/) for the specified service/version.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_fastly as fastly
 
     example_service_vcl = fastly.ServiceVcl("example",
         name="Example Service",
         domains=[fastly.ServiceVclDomainArgs(
@@ -167,15 +164,14 @@
             ),
         ],
         force_destroy=True)
     example = fastly.get_dictionaries_output(service_id=example_service_vcl.id,
         service_version=example_service_vcl.active_version)
     pulumi.export("serviceDictionaries", example)
     ```
-    <!--End PulumiCodeChooser -->
 
     [1]: https://developer.fastly.com/reference/api/dictionaries/
 
 
     :param str service_id: Alphanumeric string identifying the service.
     :param int service_version: Integer identifying a service version.
     """
```

### Comparing `pulumi_fastly-8.6.0a1713812915/pulumi_fastly/get_fastly_ip_ranges.py` & `pulumi_fastly-8.7.0a1713897687/pulumi_fastly/get_fastly_ip_ranges.py`

 * *Files 8% similar despite different names*

```diff
@@ -70,15 +70,14 @@
 
 def get_fastly_ip_ranges(opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetFastlyIpRangesResult:
     """
     Use this data source to get the [IP ranges](https://docs.fastly.com/guides/securing-communications/accessing-fastlys-ip-ranges) of Fastly edge nodes.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_aws as aws
     import pulumi_fastly as fastly
 
     fastly = fastly.get_fastly_ip_ranges()
     from_fastly = aws.index.SecurityGroup("from_fastly",
@@ -87,15 +86,14 @@
             fromPort: 443,
             toPort: 443,
             protocol: tcp,
             cidrBlocks: fastly.cidr_blocks,
             ipv6CidrBlocks: fastly.ipv6_cidr_blocks,
         }])
     ```
-    <!--End PulumiCodeChooser -->
 
     [1]: https://docs.fastly.com/guides/securing-communications/accessing-fastlys-ip-ranges
     """
     __args__ = dict()
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('fastly:index/getFastlyIpRanges:getFastlyIpRanges', __args__, opts=opts, typ=GetFastlyIpRangesResult).value
 
@@ -108,15 +106,14 @@
 @_utilities.lift_output_func(get_fastly_ip_ranges)
 def get_fastly_ip_ranges_output(opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetFastlyIpRangesResult]:
     """
     Use this data source to get the [IP ranges](https://docs.fastly.com/guides/securing-communications/accessing-fastlys-ip-ranges) of Fastly edge nodes.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_aws as aws
     import pulumi_fastly as fastly
 
     fastly = fastly.get_fastly_ip_ranges()
     from_fastly = aws.index.SecurityGroup("from_fastly",
@@ -125,12 +122,11 @@
             fromPort: 443,
             toPort: 443,
             protocol: tcp,
             cidrBlocks: fastly.cidr_blocks,
             ipv6CidrBlocks: fastly.ipv6_cidr_blocks,
         }])
     ```
-    <!--End PulumiCodeChooser -->
 
     [1]: https://docs.fastly.com/guides/securing-communications/accessing-fastlys-ip-ranges
     """
     ...
```

### Comparing `pulumi_fastly-8.6.0a1713812915/pulumi_fastly/get_kvstores.py` & `pulumi_fastly-8.7.0a1713897687/pulumi_fastly/get_kvstores.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.6.0a1713812915/pulumi_fastly/get_package_hash.py` & `pulumi_fastly-8.7.0a1713897687/pulumi_fastly/get_package_hash.py`

 * *Files 4% similar despite different names*

```diff
@@ -84,26 +84,24 @@
                      filename: Optional[str] = None,
                      opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetPackageHashResult:
     """
     Use this data source to generate a SHA512 hash of all files (in sorted order) within the package.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_fastly as fastly
 
     example = fastly.get_package_hash(filename="./path/to/package.tar.gz")
     example_service_compute = fastly.ServiceCompute("example", package=fastly.ServiceComputePackageArgs(
         filename="./path/to/package.tar.gz",
         source_code_hash=example.hash,
     ))
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str content: The contents of the Wasm deployment package as a base64 encoded string (e.g. could be provided using an input variable or via external data source output variable). Conflicts with `filename`. Exactly one of these two arguments must be specified
     :param str filename: The path to the Wasm deployment package within your local filesystem. Conflicts with `content`. Exactly one of these two arguments must be specified
     """
     __args__ = dict()
     __args__['content'] = content
@@ -123,25 +121,23 @@
                             filename: Optional[pulumi.Input[Optional[str]]] = None,
                             opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetPackageHashResult]:
     """
     Use this data source to generate a SHA512 hash of all files (in sorted order) within the package.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_fastly as fastly
 
     example = fastly.get_package_hash(filename="./path/to/package.tar.gz")
     example_service_compute = fastly.ServiceCompute("example", package=fastly.ServiceComputePackageArgs(
         filename="./path/to/package.tar.gz",
         source_code_hash=example.hash,
     ))
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str content: The contents of the Wasm deployment package as a base64 encoded string (e.g. could be provided using an input variable or via external data source output variable). Conflicts with `filename`. Exactly one of these two arguments must be specified
     :param str filename: The path to the Wasm deployment package within your local filesystem. Conflicts with `content`. Exactly one of these two arguments must be specified
     """
     ...
```

### Comparing `pulumi_fastly-8.6.0a1713812915/pulumi_fastly/get_secretstores.py` & `pulumi_fastly-8.7.0a1713897687/pulumi_fastly/get_secretstores.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.6.0a1713812915/pulumi_fastly/get_services.py` & `pulumi_fastly-8.7.0a1713897687/pulumi_fastly/get_services.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.6.0a1713812915/pulumi_fastly/get_tls_activation.py` & `pulumi_fastly-8.7.0a1713897687/pulumi_fastly/get_tls_activation.py`

 * *Files 4% similar despite different names*

```diff
@@ -104,22 +104,20 @@
     of filters, they may become mutually exclusive. The exception to this is `id` which must not be specified in combination
     with any of the others.
 
     > **Note:** If more or less than a single match is returned by the search, this provider will fail. Ensure that your search is specific enough to return a single key.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_fastly as fastly
 
     example = fastly.get_tls_activation(domain="example.com")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str certificate_id: ID of the TLS Certificate used.
     :param str configuration_id: ID of the TLS Configuration used.
     :param str domain: Domain that TLS was enabled on.
     :param str id: Fastly Activation ID. Conflicts with all other filters.
     """
@@ -152,22 +150,20 @@
     of filters, they may become mutually exclusive. The exception to this is `id` which must not be specified in combination
     with any of the others.
 
     > **Note:** If more or less than a single match is returned by the search, this provider will fail. Ensure that your search is specific enough to return a single key.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_fastly as fastly
 
     example = fastly.get_tls_activation(domain="example.com")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str certificate_id: ID of the TLS Certificate used.
     :param str configuration_id: ID of the TLS Configuration used.
     :param str domain: Domain that TLS was enabled on.
     :param str id: Fastly Activation ID. Conflicts with all other filters.
     """
```

### Comparing `pulumi_fastly-8.6.0a1713812915/pulumi_fastly/get_tls_activation_ids.py` & `pulumi_fastly-8.7.0a1713897687/pulumi_fastly/get_tls_activation_ids.py`

 * *Files 18% similar despite different names*

```diff
@@ -71,24 +71,22 @@
 def get_tls_activation_ids(certificate_id: Optional[str] = None,
                            opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetTlsActivationIdsResult:
     """
     Use this data source to get the list of TLS Activation identifiers in Fastly.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_fastly as fastly
 
     example = fastly.get_tls_activation_ids(certificate_id=example_fastly_tls_certificate["id"])
     example_get_tls_activation = {__key: fastly.get_tls_activation(id=__value) for __key, __value in example.ids}
     pulumi.export("activationDomains", [a.domain for a in example_get_tls_activation])
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str certificate_id: ID of TLS certificate used to filter activations
     """
     __args__ = dict()
     __args__['certificateId'] = certificate_id
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
@@ -104,22 +102,20 @@
 def get_tls_activation_ids_output(certificate_id: Optional[pulumi.Input[Optional[str]]] = None,
                                   opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetTlsActivationIdsResult]:
     """
     Use this data source to get the list of TLS Activation identifiers in Fastly.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_fastly as fastly
 
     example = fastly.get_tls_activation_ids(certificate_id=example_fastly_tls_certificate["id"])
     example_get_tls_activation = {__key: fastly.get_tls_activation(id=__value) for __key, __value in example.ids}
     pulumi.export("activationDomains", [a.domain for a in example_get_tls_activation])
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str certificate_id: ID of TLS certificate used to filter activations
     """
     ...
```

### Comparing `pulumi_fastly-8.6.0a1713812915/pulumi_fastly/get_tls_certificate.py` & `pulumi_fastly-8.7.0a1713897687/pulumi_fastly/get_tls_certificate.py`

 * *Files 2% similar despite different names*

```diff
@@ -165,22 +165,20 @@
     of filters, they may become mutually exclusive. The exception to this is `id` which must not be specified in combination
     with any of the others.
 
     > **Note:** If more or less than a single match is returned by the search, this provider will fail. Ensure that your search is specific enough to return a single key.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_fastly as fastly
 
     example = fastly.get_tls_certificate(name="example.com")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param Sequence[str] domains: Domains that are listed in any certificates' Subject Alternative Names (SAN) list.
     :param str id: Unique ID assigned to certificate by Fastly
     :param str issued_to: The hostname for which a certificate was issued.
     :param str issuer: The certificate authority that issued the certificate.
     :param str name: Human-readable name used to identify the certificate. Defaults to the certificate's Common Name or first Subject Alternative Name entry.
@@ -221,22 +219,20 @@
     of filters, they may become mutually exclusive. The exception to this is `id` which must not be specified in combination
     with any of the others.
 
     > **Note:** If more or less than a single match is returned by the search, this provider will fail. Ensure that your search is specific enough to return a single key.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_fastly as fastly
 
     example = fastly.get_tls_certificate(name="example.com")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param Sequence[str] domains: Domains that are listed in any certificates' Subject Alternative Names (SAN) list.
     :param str id: Unique ID assigned to certificate by Fastly
     :param str issued_to: The hostname for which a certificate was issued.
     :param str issuer: The certificate authority that issued the certificate.
     :param str name: Human-readable name used to identify the certificate. Defaults to the certificate's Common Name or first Subject Alternative Name entry.
```

### Comparing `pulumi_fastly-8.6.0a1713812915/pulumi_fastly/get_tls_certificate_ids.py` & `pulumi_fastly-8.7.0a1713897687/pulumi_fastly/get_tls_certificate_ids.py`

 * *Files 8% similar despite different names*

```diff
@@ -58,23 +58,21 @@
 
 def get_tls_certificate_ids(opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetTlsCertificateIdsResult:
     """
     Use this data source to get the IDs of available TLS certificates for use with other resources.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_fastly as fastly
 
     example = fastly.get_tls_certificate_ids()
     example_tls_activation = fastly.TlsActivation("example", certificate_id=example.ids[0])
     ```
-    <!--End PulumiCodeChooser -->
     """
     __args__ = dict()
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('fastly:index/getTlsCertificateIds:getTlsCertificateIds', __args__, opts=opts, typ=GetTlsCertificateIdsResult).value
 
     return AwaitableGetTlsCertificateIdsResult(
         id=pulumi.get(__ret__, 'id'),
@@ -84,18 +82,16 @@
 @_utilities.lift_output_func(get_tls_certificate_ids)
 def get_tls_certificate_ids_output(opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetTlsCertificateIdsResult]:
     """
     Use this data source to get the IDs of available TLS certificates for use with other resources.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_fastly as fastly
 
     example = fastly.get_tls_certificate_ids()
     example_tls_activation = fastly.TlsActivation("example", certificate_id=example.ids[0])
     ```
-    <!--End PulumiCodeChooser -->
     """
     ...
```

### Comparing `pulumi_fastly-8.6.0a1713812915/pulumi_fastly/get_tls_configuration.py` & `pulumi_fastly-8.7.0a1713897687/pulumi_fastly/get_tls_configuration.py`

 * *Files 8% similar despite different names*

```diff
@@ -155,23 +155,21 @@
     of filters, they may become mutually exclusive. The exception to this is `id` which must not be specified in combination
     with any of the others.
 
     > **Note:** If more or less than a single match is returned by the search, this provider will fail. Ensure that your search is specific enough to return a single key.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_fastly as fastly
 
     example = fastly.get_tls_configuration(default=True)
     example_tls_activation = fastly.TlsActivation("example", configuration_id=example.id)
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param bool default: Signifies whether Fastly will use this configuration as a default when creating a new TLS activation.
     :param Sequence[str] http_protocols: HTTP protocols available on the TLS configuration.
     :param str id: ID of the TLS configuration obtained from the Fastly API or another data source. Conflicts with all the other filters.
     :param str name: Custom name of the TLS configuration.
     :param Sequence[str] tls_protocols: TLS protocols available on the TLS configuration.
@@ -214,23 +212,21 @@
     of filters, they may become mutually exclusive. The exception to this is `id` which must not be specified in combination
     with any of the others.
 
     > **Note:** If more or less than a single match is returned by the search, this provider will fail. Ensure that your search is specific enough to return a single key.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_fastly as fastly
 
     example = fastly.get_tls_configuration(default=True)
     example_tls_activation = fastly.TlsActivation("example", configuration_id=example.id)
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param bool default: Signifies whether Fastly will use this configuration as a default when creating a new TLS activation.
     :param Sequence[str] http_protocols: HTTP protocols available on the TLS configuration.
     :param str id: ID of the TLS configuration obtained from the Fastly API or another data source. Conflicts with all the other filters.
     :param str name: Custom name of the TLS configuration.
     :param Sequence[str] tls_protocols: TLS protocols available on the TLS configuration.
```

### Comparing `pulumi_fastly-8.6.0a1713812915/pulumi_fastly/get_tls_configuration_ids.py` & `pulumi_fastly-8.7.0a1713897687/pulumi_fastly/get_tls_configuration_ids.py`

 * *Files 12% similar despite different names*

```diff
@@ -58,23 +58,21 @@
 
 def get_tls_configuration_ids(opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetTlsConfigurationIdsResult:
     """
     Use this data source to get the IDs of available TLS configurations for use with other resources.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_fastly as fastly
 
     example = fastly.get_tls_configuration_ids()
     example_tls_activation = fastly.TlsActivation("example", configuration_id=example.ids[0])
     ```
-    <!--End PulumiCodeChooser -->
     """
     __args__ = dict()
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('fastly:index/getTlsConfigurationIds:getTlsConfigurationIds', __args__, opts=opts, typ=GetTlsConfigurationIdsResult).value
 
     return AwaitableGetTlsConfigurationIdsResult(
         id=pulumi.get(__ret__, 'id'),
@@ -84,18 +82,16 @@
 @_utilities.lift_output_func(get_tls_configuration_ids)
 def get_tls_configuration_ids_output(opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetTlsConfigurationIdsResult]:
     """
     Use this data source to get the IDs of available TLS configurations for use with other resources.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_fastly as fastly
 
     example = fastly.get_tls_configuration_ids()
     example_tls_activation = fastly.TlsActivation("example", configuration_id=example.ids[0])
     ```
-    <!--End PulumiCodeChooser -->
     """
     ...
```

### Comparing `pulumi_fastly-8.6.0a1713812915/pulumi_fastly/get_tls_domain.py` & `pulumi_fastly-8.7.0a1713897687/pulumi_fastly/get_tls_domain.py`

 * *Files 9% similar despite different names*

```diff
@@ -95,22 +95,20 @@
 def get_tls_domain(domain: Optional[str] = None,
                    opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetTlsDomainResult:
     """
     Use this data source to get the IDs of activations, certificates and subscriptions associated with a domain.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_fastly as fastly
 
     domain = fastly.get_tls_domain(domain="example.com")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str domain: Domain name to look up activations, certificates and subscriptions for.
     """
     __args__ = dict()
     __args__['domain'] = domain
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
@@ -128,20 +126,18 @@
 def get_tls_domain_output(domain: Optional[pulumi.Input[str]] = None,
                           opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetTlsDomainResult]:
     """
     Use this data source to get the IDs of activations, certificates and subscriptions associated with a domain.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_fastly as fastly
 
     domain = fastly.get_tls_domain(domain="example.com")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str domain: Domain name to look up activations, certificates and subscriptions for.
     """
     ...
```

### Comparing `pulumi_fastly-8.6.0a1713812915/pulumi_fastly/get_tls_platform_certificate.py` & `pulumi_fastly-8.7.0a1713897687/pulumi_fastly/get_tls_platform_certificate.py`

 * *Files 2% similar despite different names*

```diff
@@ -138,22 +138,20 @@
     of filters, they may become mutually exclusive. The exception to this is `id` which must not be specified in combination
     with any of the others.
 
     > **Note:** If more or less than a single match is returned by the search, this provider will fail. Ensure that your search is specific enough to return a single key.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_fastly as fastly
 
     example = fastly.get_tls_platform_certificate(domains=["example.com"])
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param Sequence[str] domains: Domains that are listed in any certificate's Subject Alternative Names (SAN) list.
     :param str id: Unique ID assigned to certificate by Fastly. Conflicts with all the other filters.
     """
     __args__ = dict()
     __args__['domains'] = domains
@@ -183,21 +181,19 @@
     of filters, they may become mutually exclusive. The exception to this is `id` which must not be specified in combination
     with any of the others.
 
     > **Note:** If more or less than a single match is returned by the search, this provider will fail. Ensure that your search is specific enough to return a single key.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_fastly as fastly
 
     example = fastly.get_tls_platform_certificate(domains=["example.com"])
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param Sequence[str] domains: Domains that are listed in any certificate's Subject Alternative Names (SAN) list.
     :param str id: Unique ID assigned to certificate by Fastly. Conflicts with all the other filters.
     """
     ...
```

### Comparing `pulumi_fastly-8.6.0a1713812915/pulumi_fastly/get_tls_platform_certificate_ids.py` & `pulumi_fastly-8.7.0a1713897687/pulumi_fastly/get_tls_platform_certificate_ids.py`

 * *Files 17% similar despite different names*

```diff
@@ -58,23 +58,21 @@
 
 def get_tls_platform_certificate_ids(opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetTlsPlatformCertificateIdsResult:
     """
     Use this data source to get the IDs of available Platform TLS Certificates for use with other resources.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_fastly as fastly
 
     example = fastly.get_tls_platform_certificate_ids()
     example_get_tls_platform_certificate = fastly.get_tls_platform_certificate(id=example.ids[0])
     ```
-    <!--End PulumiCodeChooser -->
     """
     __args__ = dict()
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('fastly:index/getTlsPlatformCertificateIds:getTlsPlatformCertificateIds', __args__, opts=opts, typ=GetTlsPlatformCertificateIdsResult).value
 
     return AwaitableGetTlsPlatformCertificateIdsResult(
         id=pulumi.get(__ret__, 'id'),
@@ -84,18 +82,16 @@
 @_utilities.lift_output_func(get_tls_platform_certificate_ids)
 def get_tls_platform_certificate_ids_output(opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetTlsPlatformCertificateIdsResult]:
     """
     Use this data source to get the IDs of available Platform TLS Certificates for use with other resources.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_fastly as fastly
 
     example = fastly.get_tls_platform_certificate_ids()
     example_get_tls_platform_certificate = fastly.get_tls_platform_certificate(id=example.ids[0])
     ```
-    <!--End PulumiCodeChooser -->
     """
     ...
```

### Comparing `pulumi_fastly-8.6.0a1713812915/pulumi_fastly/get_tls_private_key.py` & `pulumi_fastly-8.7.0a1713897687/pulumi_fastly/get_tls_private_key.py`

 * *Files 2% similar despite different names*

```diff
@@ -131,23 +131,21 @@
      with any of the others.
 
     > **Note:** If more or less than a single match is returned by the search, this provider will fail. Ensure that your search
      is specific enough to return a single key.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_fastly as fastly
 
     demo = fastly.get_tls_private_key(name="demo-private-key")
     pulumi.export("privateKeyNeedsReplacing", demo.replace)
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str created_at: Timestamp (GMT) when the private key was created.
     :param str id: Fastly private key ID. Conflicts with all the other filters
     :param int key_length: The key length used to generate the private key.
     :param str key_type: The algorithm used to generate the private key. Must be RSA.
     :param str name: The human-readable name assigned to the private key when uploaded.
@@ -189,23 +187,21 @@
      with any of the others.
 
     > **Note:** If more or less than a single match is returned by the search, this provider will fail. Ensure that your search
      is specific enough to return a single key.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_fastly as fastly
 
     demo = fastly.get_tls_private_key(name="demo-private-key")
     pulumi.export("privateKeyNeedsReplacing", demo.replace)
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str created_at: Timestamp (GMT) when the private key was created.
     :param str id: Fastly private key ID. Conflicts with all the other filters
     :param int key_length: The key length used to generate the private key.
     :param str key_type: The algorithm used to generate the private key. Must be RSA.
     :param str name: The human-readable name assigned to the private key when uploaded.
```

### Comparing `pulumi_fastly-8.6.0a1713812915/pulumi_fastly/get_tls_private_key_ids.py` & `pulumi_fastly-8.7.0a1713897687/pulumi_fastly/get_tls_private_key_ids.py`

 * *Files 20% similar despite different names*

```diff
@@ -58,23 +58,21 @@
 
 def get_tls_private_key_ids(opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetTlsPrivateKeyIdsResult:
     """
     Use this data source to get the list of TLS private key identifiers in Fastly.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_fastly as fastly
 
     demo = fastly.get_tls_private_key_ids()
     example = fastly.get_tls_private_key(id=demo_fastly_tls_private_key_ids["ids"])
     ```
-    <!--End PulumiCodeChooser -->
     """
     __args__ = dict()
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('fastly:index/getTlsPrivateKeyIds:getTlsPrivateKeyIds', __args__, opts=opts, typ=GetTlsPrivateKeyIdsResult).value
 
     return AwaitableGetTlsPrivateKeyIdsResult(
         id=pulumi.get(__ret__, 'id'),
@@ -84,18 +82,16 @@
 @_utilities.lift_output_func(get_tls_private_key_ids)
 def get_tls_private_key_ids_output(opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetTlsPrivateKeyIdsResult]:
     """
     Use this data source to get the list of TLS private key identifiers in Fastly.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_fastly as fastly
 
     demo = fastly.get_tls_private_key_ids()
     example = fastly.get_tls_private_key(id=demo_fastly_tls_private_key_ids["ids"])
     ```
-    <!--End PulumiCodeChooser -->
     """
     ...
```

### Comparing `pulumi_fastly-8.6.0a1713812915/pulumi_fastly/get_tls_subscription.py` & `pulumi_fastly-8.7.0a1713897687/pulumi_fastly/get_tls_subscription.py`

 * *Files 3% similar despite different names*

```diff
@@ -146,22 +146,20 @@
                          id: Optional[str] = None,
                          opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetTlsSubscriptionResult:
     """
     Use this data source to get information about a TLS subscription.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_fastly as fastly
 
     example = fastly.get_tls_subscription(domains=["example.com"])
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str certificate_authority: The entity that issues and certifies the TLS certificates for the subscription.
     :param str configuration_id: ID of TLS configuration used to terminate TLS traffic.
     :param Sequence[str] domains: List of domains on which to enable TLS.
     :param str id: ID of TLS subscription. Conflicts with all the other filters.
     """
@@ -192,22 +190,20 @@
                                 id: Optional[pulumi.Input[Optional[str]]] = None,
                                 opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetTlsSubscriptionResult]:
     """
     Use this data source to get information about a TLS subscription.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_fastly as fastly
 
     example = fastly.get_tls_subscription(domains=["example.com"])
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str certificate_authority: The entity that issues and certifies the TLS certificates for the subscription.
     :param str configuration_id: ID of TLS configuration used to terminate TLS traffic.
     :param Sequence[str] domains: List of domains on which to enable TLS.
     :param str id: ID of TLS subscription. Conflicts with all the other filters.
     """
```

### Comparing `pulumi_fastly-8.6.0a1713812915/pulumi_fastly/get_tls_subscription_ids.py` & `pulumi_fastly-8.7.0a1713897687/pulumi_fastly/get_tls_subscription_ids.py`

 * *Files 15% similar despite different names*

```diff
@@ -58,24 +58,22 @@
 
 def get_tls_subscription_ids(opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetTlsSubscriptionIdsResult:
     """
     Use this data source to get the list of IDs of TLS Subscriptions in Fastly.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_fastly as fastly
 
     example = fastly.get_tls_subscription_ids()
     example_get_tls_subscription = {__key: fastly.get_tls_subscription(id=__value) for __key, __value in example.ids}
     pulumi.export("subscriptionDomains", [a.certificate_authority for a in example_get_tls_subscription])
     ```
-    <!--End PulumiCodeChooser -->
     """
     __args__ = dict()
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('fastly:index/getTlsSubscriptionIds:getTlsSubscriptionIds', __args__, opts=opts, typ=GetTlsSubscriptionIdsResult).value
 
     return AwaitableGetTlsSubscriptionIdsResult(
         id=pulumi.get(__ret__, 'id'),
@@ -85,19 +83,17 @@
 @_utilities.lift_output_func(get_tls_subscription_ids)
 def get_tls_subscription_ids_output(opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetTlsSubscriptionIdsResult]:
     """
     Use this data source to get the list of IDs of TLS Subscriptions in Fastly.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_fastly as fastly
 
     example = fastly.get_tls_subscription_ids()
     example_get_tls_subscription = {__key: fastly.get_tls_subscription(id=__value) for __key, __value in example.ids}
     pulumi.export("subscriptionDomains", [a.certificate_authority for a in example_get_tls_subscription])
     ```
-    <!--End PulumiCodeChooser -->
     """
     ...
```

### Comparing `pulumi_fastly-8.6.0a1713812915/pulumi_fastly/get_vcl_snippets.py` & `pulumi_fastly-8.7.0a1713897687/pulumi_fastly/get_vcl_snippets.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.6.0a1713812915/pulumi_fastly/get_waf_rules.py` & `pulumi_fastly-8.7.0a1713897687/pulumi_fastly/get_waf_rules.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.6.0a1713812915/pulumi_fastly/kvstore.py` & `pulumi_fastly-8.7.0a1713897687/pulumi_fastly/kvstore.py`

 * *Files 2% similar despite different names*

```diff
@@ -133,15 +133,14 @@
                  name: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         ## Example Usage
 
         Basic usage:
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_fastly as fastly
 
         # IMPORTANT: Deleting a KV Store requires first deleting its resource_link.
         # This requires a two-step `pulumi up` as we can't guarantee deletion order.
         # e.g. resource_link deletion within fastly_service_compute might not finish first.
@@ -158,15 +157,14 @@
             ),
             resource_links=[fastly.ServiceComputeResourceLinkArgs(
                 name="my_resource_link",
                 resource_id=example_kvstore.id,
             )],
             force_destroy=True)
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Fastly KV Stores can be imported using their Store ID, e.g.
 
         ```sh
         $ pulumi import fastly:index/kvstore:Kvstore example xxxxxxxxxxxxxxxxxxxx
@@ -185,15 +183,14 @@
                  args: Optional[KvstoreArgs] = None,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         ## Example Usage
 
         Basic usage:
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_fastly as fastly
 
         # IMPORTANT: Deleting a KV Store requires first deleting its resource_link.
         # This requires a two-step `pulumi up` as we can't guarantee deletion order.
         # e.g. resource_link deletion within fastly_service_compute might not finish first.
@@ -210,15 +207,14 @@
             ),
             resource_links=[fastly.ServiceComputeResourceLinkArgs(
                 name="my_resource_link",
                 resource_id=example_kvstore.id,
             )],
             force_destroy=True)
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Fastly KV Stores can be imported using their Store ID, e.g.
 
         ```sh
         $ pulumi import fastly:index/kvstore:Kvstore example xxxxxxxxxxxxxxxxxxxx
```

### Comparing `pulumi_fastly-8.6.0a1713812915/pulumi_fastly/outputs.py` & `pulumi_fastly-8.7.0a1713897687/pulumi_fastly/outputs.py`

 * *Files 0% similar despite different names*

```diff
@@ -10338,35 +10338,35 @@
         return super().get(key, default)
 
     def __init__(__self__, *,
                  content: str,
                  content_type: str,
                  status: int):
         """
-        :param str content: The VCL code that specifies exactly what the snippet does
-        :param str content_type: Value of the `Content-Type` header sent with the request
+        :param str content: HTTP response body data
+        :param str content_type: HTTP Content-Type (e.g. application/json)
         :param int status: HTTP response status code (e.g. 429)
         """
         pulumi.set(__self__, "content", content)
         pulumi.set(__self__, "content_type", content_type)
         pulumi.set(__self__, "status", status)
 
     @property
     @pulumi.getter
     def content(self) -> str:
         """
-        The VCL code that specifies exactly what the snippet does
+        HTTP response body data
         """
         return pulumi.get(self, "content")
 
     @property
     @pulumi.getter(name="contentType")
     def content_type(self) -> str:
         """
-        Value of the `Content-Type` header sent with the request
+        HTTP Content-Type (e.g. application/json)
         """
         return pulumi.get(self, "content_type")
 
     @property
     @pulumi.getter
     def status(self) -> int:
         """
```

### Comparing `pulumi_fastly-8.6.0a1713812915/pulumi_fastly/provider.py` & `pulumi_fastly-8.7.0a1713897687/pulumi_fastly/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.6.0a1713812915/pulumi_fastly/secretstore.py` & `pulumi_fastly-8.7.0a1713897687/pulumi_fastly/secretstore.py`

 * *Files 5% similar despite different names*

```diff
@@ -67,15 +67,14 @@
                  name: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         ## Example Usage
 
         Basic usage:
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_fastly as fastly
 
         # IMPORTANT: Deleting a Secret Store requires first deleting its resource_link.
         # This requires a two-step `pulumi up` as we can't guarantee deletion order.
         # e.g. resource_link deletion within fastly_service_compute might not finish first.
@@ -92,15 +91,14 @@
             ),
             resource_links=[fastly.ServiceComputeResourceLinkArgs(
                 name="my_resource_link",
                 resource_id=example_secretstore.id,
             )],
             force_destroy=True)
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Fastly Secret Stores can be imported using their Store ID, e.g.
 
         ```sh
         $ pulumi import fastly:index/secretstore:Secretstore example xxxxxxxxxxxxxxxxxxxx
@@ -117,15 +115,14 @@
                  args: Optional[SecretstoreArgs] = None,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         ## Example Usage
 
         Basic usage:
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_fastly as fastly
 
         # IMPORTANT: Deleting a Secret Store requires first deleting its resource_link.
         # This requires a two-step `pulumi up` as we can't guarantee deletion order.
         # e.g. resource_link deletion within fastly_service_compute might not finish first.
@@ -142,15 +139,14 @@
             ),
             resource_links=[fastly.ServiceComputeResourceLinkArgs(
                 name="my_resource_link",
                 resource_id=example_secretstore.id,
             )],
             force_destroy=True)
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Fastly Secret Stores can be imported using their Store ID, e.g.
 
         ```sh
         $ pulumi import fastly:index/secretstore:Secretstore example xxxxxxxxxxxxxxxxxxxx
```

### Comparing `pulumi_fastly-8.6.0a1713812915/pulumi_fastly/service_acl_entries.py` & `pulumi_fastly-8.7.0a1713897687/pulumi_fastly/service_acl_entries.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.6.0a1713812915/pulumi_fastly/service_authorization.py` & `pulumi_fastly-8.7.0a1713897687/pulumi_fastly/service_authorization.py`

 * *Files 2% similar despite different names*

```diff
@@ -134,27 +134,25 @@
 
         The Service Authorization resource requires a user id, service id and an optional permission.
 
         ## Example Usage
 
         Basic usage:
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_fastly as fastly
 
         demo = fastly.ServiceVcl("demo")
         user = fastly.User("user")
         auth = fastly.ServiceAuthorization("auth",
             service_id=demo.id,
             user_id=user.id,
             permission="purge_all")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         A Fastly Service Authorization can be imported using their user ID, e.g.
 
         ```sh
         $ pulumi import fastly:index/serviceAuthorization:ServiceAuthorization demo xxxxxxxxxxxxxxxxxxxx
@@ -177,27 +175,25 @@
 
         The Service Authorization resource requires a user id, service id and an optional permission.
 
         ## Example Usage
 
         Basic usage:
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_fastly as fastly
 
         demo = fastly.ServiceVcl("demo")
         user = fastly.User("user")
         auth = fastly.ServiceAuthorization("auth",
             service_id=demo.id,
             user_id=user.id,
             permission="purge_all")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         A Fastly Service Authorization can be imported using their user ID, e.g.
 
         ```sh
         $ pulumi import fastly:index/serviceAuthorization:ServiceAuthorization demo xxxxxxxxxxxxxxxxxxxx
```

### Comparing `pulumi_fastly-8.6.0a1713812915/pulumi_fastly/service_compute.py` & `pulumi_fastly-8.7.0a1713897687/pulumi_fastly/service_compute.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,19 +52,19 @@
                  package: Optional[pulumi.Input['ServiceComputePackageArgs']] = None,
                  product_enablement: Optional[pulumi.Input['ServiceComputeProductEnablementArgs']] = None,
                  resource_links: Optional[pulumi.Input[Sequence[pulumi.Input['ServiceComputeResourceLinkArgs']]]] = None,
                  reuse: Optional[pulumi.Input[bool]] = None,
                  version_comment: Optional[pulumi.Input[str]] = None):
         """
         The set of arguments for constructing a ServiceCompute resource.
-        :param pulumi.Input[Sequence[pulumi.Input['ServiceComputeDomainArgs']]] domains: The domain of the DigitalOcean Spaces endpoint (default `nyc3.digitaloceanspaces.com`)
+        :param pulumi.Input[Sequence[pulumi.Input['ServiceComputeDomainArgs']]] domains: A set of Domain names to serve as entry points for your Service
         :param pulumi.Input[bool] activate: Conditionally prevents the Service from being activated. The apply step will continue to create a new draft version but will not activate it if this is set to `false`. Default `true`
-        :param pulumi.Input[str] comment: An optional comment about the Domain.
-        :param pulumi.Input[bool] force_destroy: Allow the dictionary to be deleted, even if it contains entries. Defaults to false.
-        :param pulumi.Input[str] name: Name for this Backend. Must be unique to this Service. It is important to note that changing this attribute will delete and recreate the resource
+        :param pulumi.Input[str] comment: Description field for the service. Default `Managed by Terraform`
+        :param pulumi.Input[bool] force_destroy: Services that are active cannot be destroyed. In order to destroy the Service, set `force_destroy` to `true`. Default `false`
+        :param pulumi.Input[str] name: The unique name for the Service to create
         :param pulumi.Input['ServiceComputePackageArgs'] package: The `package` block supports uploading or modifying Wasm packages for use in a Fastly Compute service (if omitted, ensure `activate = false` is set on `ServiceCompute` to avoid service validation errors). See Fastly's documentation on [Compute](https://developer.fastly.com/learning/compute/)
         :param pulumi.Input[Sequence[pulumi.Input['ServiceComputeResourceLinkArgs']]] resource_links: A resource link represents a link between a shared resource (such as an KV Store or Config Store) and a service version.
         :param pulumi.Input[bool] reuse: Services that are active cannot be destroyed. If set to `true` a service Terraform intends to destroy will instead be
                deactivated (allowing it to be reused by importing it into another Terraform project). If `false`, attempting to destroy
                an active service will cause an error. Default `false`
         :param pulumi.Input[str] version_comment: Description field for the version
         """
@@ -144,15 +144,15 @@
         if version_comment is not None:
             pulumi.set(__self__, "version_comment", version_comment)
 
     @property
     @pulumi.getter
     def domains(self) -> pulumi.Input[Sequence[pulumi.Input['ServiceComputeDomainArgs']]]:
         """
-        The domain of the DigitalOcean Spaces endpoint (default `nyc3.digitaloceanspaces.com`)
+        A set of Domain names to serve as entry points for your Service
         """
         return pulumi.get(self, "domains")
 
     @domains.setter
     def domains(self, value: pulumi.Input[Sequence[pulumi.Input['ServiceComputeDomainArgs']]]):
         pulumi.set(self, "domains", value)
 
@@ -177,15 +177,15 @@
     def backends(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['ServiceComputeBackendArgs']]]]):
         pulumi.set(self, "backends", value)
 
     @property
     @pulumi.getter
     def comment(self) -> Optional[pulumi.Input[str]]:
         """
-        An optional comment about the Domain.
+        Description field for the service. Default `Managed by Terraform`
         """
         return pulumi.get(self, "comment")
 
     @comment.setter
     def comment(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "comment", value)
 
@@ -198,15 +198,15 @@
     def dictionaries(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['ServiceComputeDictionaryArgs']]]]):
         pulumi.set(self, "dictionaries", value)
 
     @property
     @pulumi.getter(name="forceDestroy")
     def force_destroy(self) -> Optional[pulumi.Input[bool]]:
         """
-        Allow the dictionary to be deleted, even if it contains entries. Defaults to false.
+        Services that are active cannot be destroyed. In order to destroy the Service, set `force_destroy` to `true`. Default `false`
         """
         return pulumi.get(self, "force_destroy")
 
     @force_destroy.setter
     def force_destroy(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "force_destroy", value)
 
@@ -444,15 +444,15 @@
     def logging_syslogs(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['ServiceComputeLoggingSyslogArgs']]]]):
         pulumi.set(self, "logging_syslogs", value)
 
     @property
     @pulumi.getter
     def name(self) -> Optional[pulumi.Input[str]]:
         """
-        Name for this Backend. Must be unique to this Service. It is important to note that changing this attribute will delete and recreate the resource
+        The unique name for the Service to create
         """
         return pulumi.get(self, "name")
 
     @name.setter
     def name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "name", value)
 
@@ -562,22 +562,22 @@
                  reuse: Optional[pulumi.Input[bool]] = None,
                  version_comment: Optional[pulumi.Input[str]] = None):
         """
         Input properties used for looking up and filtering ServiceCompute resources.
         :param pulumi.Input[bool] activate: Conditionally prevents the Service from being activated. The apply step will continue to create a new draft version but will not activate it if this is set to `false`. Default `true`
         :param pulumi.Input[int] active_version: The currently active version of your Fastly Service
         :param pulumi.Input[int] cloned_version: The latest cloned version by the provider
-        :param pulumi.Input[str] comment: An optional comment about the Domain.
-        :param pulumi.Input[Sequence[pulumi.Input['ServiceComputeDomainArgs']]] domains: The domain of the DigitalOcean Spaces endpoint (default `nyc3.digitaloceanspaces.com`)
-        :param pulumi.Input[bool] force_destroy: Allow the dictionary to be deleted, even if it contains entries. Defaults to false.
+        :param pulumi.Input[str] comment: Description field for the service. Default `Managed by Terraform`
+        :param pulumi.Input[Sequence[pulumi.Input['ServiceComputeDomainArgs']]] domains: A set of Domain names to serve as entry points for your Service
+        :param pulumi.Input[bool] force_destroy: Services that are active cannot be destroyed. In order to destroy the Service, set `force_destroy` to `true`. Default `false`
         :param pulumi.Input[bool] force_refresh: Used internally by the provider to temporarily indicate if all resources should call their associated API to update the
                local state. This is for scenarios where the service version has been reverted outside of Terraform (e.g. via the Fastly
                UI) and the provider needs to resync the state for a different active version (this is only if `activate` is `true`).
         :param pulumi.Input[bool] imported: Used internally by the provider to temporarily indicate if the service is being imported, and is reset to false once the import is finished
-        :param pulumi.Input[str] name: Name for this Backend. Must be unique to this Service. It is important to note that changing this attribute will delete and recreate the resource
+        :param pulumi.Input[str] name: The unique name for the Service to create
         :param pulumi.Input['ServiceComputePackageArgs'] package: The `package` block supports uploading or modifying Wasm packages for use in a Fastly Compute service (if omitted, ensure `activate = false` is set on `ServiceCompute` to avoid service validation errors). See Fastly's documentation on [Compute](https://developer.fastly.com/learning/compute/)
         :param pulumi.Input[Sequence[pulumi.Input['ServiceComputeResourceLinkArgs']]] resource_links: A resource link represents a link between a shared resource (such as an KV Store or Config Store) and a service version.
         :param pulumi.Input[bool] reuse: Services that are active cannot be destroyed. If set to `true` a service Terraform intends to destroy will instead be
                deactivated (allowing it to be reused by importing it into another Terraform project). If `false`, attempting to destroy
                an active service will cause an error. Default `false`
         :param pulumi.Input[str] version_comment: Description field for the version
         """
@@ -711,15 +711,15 @@
     def cloned_version(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "cloned_version", value)
 
     @property
     @pulumi.getter
     def comment(self) -> Optional[pulumi.Input[str]]:
         """
-        An optional comment about the Domain.
+        Description field for the service. Default `Managed by Terraform`
         """
         return pulumi.get(self, "comment")
 
     @comment.setter
     def comment(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "comment", value)
 
@@ -732,27 +732,27 @@
     def dictionaries(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['ServiceComputeDictionaryArgs']]]]):
         pulumi.set(self, "dictionaries", value)
 
     @property
     @pulumi.getter
     def domains(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['ServiceComputeDomainArgs']]]]:
         """
-        The domain of the DigitalOcean Spaces endpoint (default `nyc3.digitaloceanspaces.com`)
+        A set of Domain names to serve as entry points for your Service
         """
         return pulumi.get(self, "domains")
 
     @domains.setter
     def domains(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['ServiceComputeDomainArgs']]]]):
         pulumi.set(self, "domains", value)
 
     @property
     @pulumi.getter(name="forceDestroy")
     def force_destroy(self) -> Optional[pulumi.Input[bool]]:
         """
-        Allow the dictionary to be deleted, even if it contains entries. Defaults to false.
+        Services that are active cannot be destroyed. In order to destroy the Service, set `force_destroy` to `true`. Default `false`
         """
         return pulumi.get(self, "force_destroy")
 
     @force_destroy.setter
     def force_destroy(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "force_destroy", value)
 
@@ -1016,15 +1016,15 @@
     def logging_syslogs(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['ServiceComputeLoggingSyslogArgs']]]]):
         pulumi.set(self, "logging_syslogs", value)
 
     @property
     @pulumi.getter
     def name(self) -> Optional[pulumi.Input[str]]:
         """
-        Name for this Backend. Must be unique to this Service. It is important to note that changing this attribute will delete and recreate the resource
+        The unique name for the Service to create
         """
         return pulumi.get(self, "name")
 
     @name.setter
     def name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "name", value)
 
@@ -1148,18 +1148,18 @@
         ```sh
         $ pulumi import fastly:index/serviceCompute:ServiceCompute demo xxxxxxxxxxxxxxxxxxxx@2
         ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[bool] activate: Conditionally prevents the Service from being activated. The apply step will continue to create a new draft version but will not activate it if this is set to `false`. Default `true`
-        :param pulumi.Input[str] comment: An optional comment about the Domain.
-        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ServiceComputeDomainArgs']]]] domains: The domain of the DigitalOcean Spaces endpoint (default `nyc3.digitaloceanspaces.com`)
-        :param pulumi.Input[bool] force_destroy: Allow the dictionary to be deleted, even if it contains entries. Defaults to false.
-        :param pulumi.Input[str] name: Name for this Backend. Must be unique to this Service. It is important to note that changing this attribute will delete and recreate the resource
+        :param pulumi.Input[str] comment: Description field for the service. Default `Managed by Terraform`
+        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ServiceComputeDomainArgs']]]] domains: A set of Domain names to serve as entry points for your Service
+        :param pulumi.Input[bool] force_destroy: Services that are active cannot be destroyed. In order to destroy the Service, set `force_destroy` to `true`. Default `false`
+        :param pulumi.Input[str] name: The unique name for the Service to create
         :param pulumi.Input[pulumi.InputType['ServiceComputePackageArgs']] package: The `package` block supports uploading or modifying Wasm packages for use in a Fastly Compute service (if omitted, ensure `activate = false` is set on `ServiceCompute` to avoid service validation errors). See Fastly's documentation on [Compute](https://developer.fastly.com/learning/compute/)
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ServiceComputeResourceLinkArgs']]]] resource_links: A resource link represents a link between a shared resource (such as an KV Store or Config Store) and a service version.
         :param pulumi.Input[bool] reuse: Services that are active cannot be destroyed. If set to `true` a service Terraform intends to destroy will instead be
                deactivated (allowing it to be reused by importing it into another Terraform project). If `false`, attempting to destroy
                an active service will cause an error. Default `false`
         :param pulumi.Input[str] version_comment: Description field for the version
         """
@@ -1350,22 +1350,22 @@
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[bool] activate: Conditionally prevents the Service from being activated. The apply step will continue to create a new draft version but will not activate it if this is set to `false`. Default `true`
         :param pulumi.Input[int] active_version: The currently active version of your Fastly Service
         :param pulumi.Input[int] cloned_version: The latest cloned version by the provider
-        :param pulumi.Input[str] comment: An optional comment about the Domain.
-        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ServiceComputeDomainArgs']]]] domains: The domain of the DigitalOcean Spaces endpoint (default `nyc3.digitaloceanspaces.com`)
-        :param pulumi.Input[bool] force_destroy: Allow the dictionary to be deleted, even if it contains entries. Defaults to false.
+        :param pulumi.Input[str] comment: Description field for the service. Default `Managed by Terraform`
+        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ServiceComputeDomainArgs']]]] domains: A set of Domain names to serve as entry points for your Service
+        :param pulumi.Input[bool] force_destroy: Services that are active cannot be destroyed. In order to destroy the Service, set `force_destroy` to `true`. Default `false`
         :param pulumi.Input[bool] force_refresh: Used internally by the provider to temporarily indicate if all resources should call their associated API to update the
                local state. This is for scenarios where the service version has been reverted outside of Terraform (e.g. via the Fastly
                UI) and the provider needs to resync the state for a different active version (this is only if `activate` is `true`).
         :param pulumi.Input[bool] imported: Used internally by the provider to temporarily indicate if the service is being imported, and is reset to false once the import is finished
-        :param pulumi.Input[str] name: Name for this Backend. Must be unique to this Service. It is important to note that changing this attribute will delete and recreate the resource
+        :param pulumi.Input[str] name: The unique name for the Service to create
         :param pulumi.Input[pulumi.InputType['ServiceComputePackageArgs']] package: The `package` block supports uploading or modifying Wasm packages for use in a Fastly Compute service (if omitted, ensure `activate = false` is set on `ServiceCompute` to avoid service validation errors). See Fastly's documentation on [Compute](https://developer.fastly.com/learning/compute/)
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ServiceComputeResourceLinkArgs']]]] resource_links: A resource link represents a link between a shared resource (such as an KV Store or Config Store) and a service version.
         :param pulumi.Input[bool] reuse: Services that are active cannot be destroyed. If set to `true` a service Terraform intends to destroy will instead be
                deactivated (allowing it to be reused by importing it into another Terraform project). If `false`, attempting to destroy
                an active service will cause an error. Default `false`
         :param pulumi.Input[str] version_comment: Description field for the version
         """
@@ -1446,36 +1446,36 @@
         """
         return pulumi.get(self, "cloned_version")
 
     @property
     @pulumi.getter
     def comment(self) -> pulumi.Output[Optional[str]]:
         """
-        An optional comment about the Domain.
+        Description field for the service. Default `Managed by Terraform`
         """
         return pulumi.get(self, "comment")
 
     @property
     @pulumi.getter
     def dictionaries(self) -> pulumi.Output[Optional[Sequence['outputs.ServiceComputeDictionary']]]:
         return pulumi.get(self, "dictionaries")
 
     @property
     @pulumi.getter
     def domains(self) -> pulumi.Output[Sequence['outputs.ServiceComputeDomain']]:
         """
-        The domain of the DigitalOcean Spaces endpoint (default `nyc3.digitaloceanspaces.com`)
+        A set of Domain names to serve as entry points for your Service
         """
         return pulumi.get(self, "domains")
 
     @property
     @pulumi.getter(name="forceDestroy")
     def force_destroy(self) -> pulumi.Output[Optional[bool]]:
         """
-        Allow the dictionary to be deleted, even if it contains entries. Defaults to false.
+        Services that are active cannot be destroyed. In order to destroy the Service, set `force_destroy` to `true`. Default `false`
         """
         return pulumi.get(self, "force_destroy")
 
     @property
     @pulumi.getter(name="forceRefresh")
     def force_refresh(self) -> pulumi.Output[bool]:
         """
@@ -1623,15 +1623,15 @@
     def logging_syslogs(self) -> pulumi.Output[Optional[Sequence['outputs.ServiceComputeLoggingSyslog']]]:
         return pulumi.get(self, "logging_syslogs")
 
     @property
     @pulumi.getter
     def name(self) -> pulumi.Output[str]:
         """
-        Name for this Backend. Must be unique to this Service. It is important to note that changing this attribute will delete and recreate the resource
+        The unique name for the Service to create
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter
     def package(self) -> pulumi.Output[Optional['outputs.ServiceComputePackage']]:
         """
```

### Comparing `pulumi_fastly-8.6.0a1713812915/pulumi_fastly/service_dictionary_items.py` & `pulumi_fastly-8.7.0a1713897687/pulumi_fastly/service_dictionary_items.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.6.0a1713812915/pulumi_fastly/service_dynamic_snippet_content.py` & `pulumi_fastly-8.7.0a1713897687/pulumi_fastly/service_dynamic_snippet_content.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.6.0a1713812915/pulumi_fastly/service_vcl.py` & `pulumi_fastly-8.7.0a1713897687/pulumi_fastly/service_vcl.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,25 +70,22 @@
                  stale_if_error: Optional[pulumi.Input[bool]] = None,
                  stale_if_error_ttl: Optional[pulumi.Input[int]] = None,
                  vcls: Optional[pulumi.Input[Sequence[pulumi.Input['ServiceVclVclArgs']]]] = None,
                  version_comment: Optional[pulumi.Input[str]] = None,
                  waf: Optional[pulumi.Input['ServiceVclWafArgs']] = None):
         """
         The set of arguments for constructing a ServiceVcl resource.
-        :param pulumi.Input[Sequence[pulumi.Input['ServiceVclDomainArgs']]] domains: The domain of the DigitalOcean Spaces endpoint (default `nyc3.digitaloceanspaces.com`)
-        :param pulumi.Input[Sequence[pulumi.Input['ServiceVclAclArgs']]] acls: The AWS [Canned ACL](https://docs.aws.amazon.com/AmazonS3/latest/userguide/acl-overview.html#canned-acl) to use for objects uploaded to the S3 bucket. Options are: `private`, `public-read`, `public-read-write`, `aws-exec-read`, `authenticated-read`, `bucket-owner-read`, `bucket-owner-full-control`
+        :param pulumi.Input[Sequence[pulumi.Input['ServiceVclDomainArgs']]] domains: A set of Domain names to serve as entry points for your Service
         :param pulumi.Input[bool] activate: Conditionally prevents the Service from being activated. The apply step will continue to create a new draft version but will not activate it if this is set to `false`. Default `true`
-        :param pulumi.Input[str] comment: An optional comment about the Director
-        :param pulumi.Input[str] default_host: Sets the host header
+        :param pulumi.Input[str] comment: Description field for the service. Default `Managed by Terraform`
+        :param pulumi.Input[str] default_host: The default hostname
         :param pulumi.Input[int] default_ttl: The default Time-to-live (TTL) for requests
-        :param pulumi.Input[bool] force_destroy: Allow the ACL to be deleted, even if it contains entries. Defaults to false.
-        :param pulumi.Input[Sequence[pulumi.Input['ServiceVclHealthcheckArgs']]] healthchecks: Name of a defined `healthcheck` to assign to this backend
+        :param pulumi.Input[bool] force_destroy: Services that are active cannot be destroyed. In order to destroy the Service, set `force_destroy` to `true`. Default `false`
         :param pulumi.Input[bool] http3: Enables support for the HTTP/3 (QUIC) protocol
-        :param pulumi.Input[str] name: A unique name to identify this ACL. It is important to note that changing this attribute will delete and recreate the ACL, and discard the current items in the ACL
-        :param pulumi.Input[Sequence[pulumi.Input['ServiceVclResponseObjectArgs']]] response_objects: The name of the response object used by the Web Application Firewall
+        :param pulumi.Input[str] name: The unique name for the Service to create
         :param pulumi.Input[bool] reuse: Services that are active cannot be destroyed. If set to `true` a service Terraform intends to destroy will instead be
                deactivated (allowing it to be reused by importing it into another Terraform project). If `false`, attempting to destroy
                an active service will cause an error. Default `false`
         :param pulumi.Input[bool] stale_if_error: Enables serving a stale object if there is an error
         :param pulumi.Input[int] stale_if_error_ttl: The default time-to-live (TTL) for serving the stale object for the version
         :param pulumi.Input[str] version_comment: Description field for the version
         """
@@ -204,28 +201,25 @@
         if waf is not None:
             pulumi.set(__self__, "waf", waf)
 
     @property
     @pulumi.getter
     def domains(self) -> pulumi.Input[Sequence[pulumi.Input['ServiceVclDomainArgs']]]:
         """
-        The domain of the DigitalOcean Spaces endpoint (default `nyc3.digitaloceanspaces.com`)
+        A set of Domain names to serve as entry points for your Service
         """
         return pulumi.get(self, "domains")
 
     @domains.setter
     def domains(self, value: pulumi.Input[Sequence[pulumi.Input['ServiceVclDomainArgs']]]):
         pulumi.set(self, "domains", value)
 
     @property
     @pulumi.getter
     def acls(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['ServiceVclAclArgs']]]]:
-        """
-        The AWS [Canned ACL](https://docs.aws.amazon.com/AmazonS3/latest/userguide/acl-overview.html#canned-acl) to use for objects uploaded to the S3 bucket. Options are: `private`, `public-read`, `public-read-write`, `aws-exec-read`, `authenticated-read`, `bucket-owner-read`, `bucket-owner-full-control`
-        """
         return pulumi.get(self, "acls")
 
     @acls.setter
     def acls(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['ServiceVclAclArgs']]]]):
         pulumi.set(self, "acls", value)
 
     @property
@@ -258,15 +252,15 @@
     def cache_settings(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['ServiceVclCacheSettingArgs']]]]):
         pulumi.set(self, "cache_settings", value)
 
     @property
     @pulumi.getter
     def comment(self) -> Optional[pulumi.Input[str]]:
         """
-        An optional comment about the Director
+        Description field for the service. Default `Managed by Terraform`
         """
         return pulumi.get(self, "comment")
 
     @comment.setter
     def comment(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "comment", value)
 
@@ -279,15 +273,15 @@
     def conditions(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['ServiceVclConditionArgs']]]]):
         pulumi.set(self, "conditions", value)
 
     @property
     @pulumi.getter(name="defaultHost")
     def default_host(self) -> Optional[pulumi.Input[str]]:
         """
-        Sets the host header
+        The default hostname
         """
         return pulumi.get(self, "default_host")
 
     @default_host.setter
     def default_host(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "default_host", value)
 
@@ -330,15 +324,15 @@
     def dynamicsnippets(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['ServiceVclDynamicsnippetArgs']]]]):
         pulumi.set(self, "dynamicsnippets", value)
 
     @property
     @pulumi.getter(name="forceDestroy")
     def force_destroy(self) -> Optional[pulumi.Input[bool]]:
         """
-        Allow the ACL to be deleted, even if it contains entries. Defaults to false.
+        Services that are active cannot be destroyed. In order to destroy the Service, set `force_destroy` to `true`. Default `false`
         """
         return pulumi.get(self, "force_destroy")
 
     @force_destroy.setter
     def force_destroy(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "force_destroy", value)
 
@@ -359,17 +353,14 @@
     @headers.setter
     def headers(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['ServiceVclHeaderArgs']]]]):
         pulumi.set(self, "headers", value)
 
     @property
     @pulumi.getter
     def healthchecks(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['ServiceVclHealthcheckArgs']]]]:
-        """
-        Name of a defined `healthcheck` to assign to this backend
-        """
         return pulumi.get(self, "healthchecks")
 
     @healthchecks.setter
     def healthchecks(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['ServiceVclHealthcheckArgs']]]]):
         pulumi.set(self, "healthchecks", value)
 
     @property
@@ -627,15 +618,15 @@
     def logging_syslogs(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['ServiceVclLoggingSyslogArgs']]]]):
         pulumi.set(self, "logging_syslogs", value)
 
     @property
     @pulumi.getter
     def name(self) -> Optional[pulumi.Input[str]]:
         """
-        A unique name to identify this ACL. It is important to note that changing this attribute will delete and recreate the ACL, and discard the current items in the ACL
+        The unique name for the Service to create
         """
         return pulumi.get(self, "name")
 
     @name.setter
     def name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "name", value)
 
@@ -665,17 +656,14 @@
     @request_settings.setter
     def request_settings(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['ServiceVclRequestSettingArgs']]]]):
         pulumi.set(self, "request_settings", value)
 
     @property
     @pulumi.getter(name="responseObjects")
     def response_objects(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['ServiceVclResponseObjectArgs']]]]:
-        """
-        The name of the response object used by the Web Application Firewall
-        """
         return pulumi.get(self, "response_objects")
 
     @response_objects.setter
     def response_objects(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['ServiceVclResponseObjectArgs']]]]):
         pulumi.set(self, "response_objects", value)
 
     @property
@@ -817,31 +805,28 @@
                  stale_if_error: Optional[pulumi.Input[bool]] = None,
                  stale_if_error_ttl: Optional[pulumi.Input[int]] = None,
                  vcls: Optional[pulumi.Input[Sequence[pulumi.Input['ServiceVclVclArgs']]]] = None,
                  version_comment: Optional[pulumi.Input[str]] = None,
                  waf: Optional[pulumi.Input['ServiceVclWafArgs']] = None):
         """
         Input properties used for looking up and filtering ServiceVcl resources.
-        :param pulumi.Input[Sequence[pulumi.Input['ServiceVclAclArgs']]] acls: The AWS [Canned ACL](https://docs.aws.amazon.com/AmazonS3/latest/userguide/acl-overview.html#canned-acl) to use for objects uploaded to the S3 bucket. Options are: `private`, `public-read`, `public-read-write`, `aws-exec-read`, `authenticated-read`, `bucket-owner-read`, `bucket-owner-full-control`
         :param pulumi.Input[bool] activate: Conditionally prevents the Service from being activated. The apply step will continue to create a new draft version but will not activate it if this is set to `false`. Default `true`
         :param pulumi.Input[int] active_version: The currently active version of your Fastly Service
         :param pulumi.Input[int] cloned_version: The latest cloned version by the provider
-        :param pulumi.Input[str] comment: An optional comment about the Director
-        :param pulumi.Input[str] default_host: Sets the host header
+        :param pulumi.Input[str] comment: Description field for the service. Default `Managed by Terraform`
+        :param pulumi.Input[str] default_host: The default hostname
         :param pulumi.Input[int] default_ttl: The default Time-to-live (TTL) for requests
-        :param pulumi.Input[Sequence[pulumi.Input['ServiceVclDomainArgs']]] domains: The domain of the DigitalOcean Spaces endpoint (default `nyc3.digitaloceanspaces.com`)
-        :param pulumi.Input[bool] force_destroy: Allow the ACL to be deleted, even if it contains entries. Defaults to false.
+        :param pulumi.Input[Sequence[pulumi.Input['ServiceVclDomainArgs']]] domains: A set of Domain names to serve as entry points for your Service
+        :param pulumi.Input[bool] force_destroy: Services that are active cannot be destroyed. In order to destroy the Service, set `force_destroy` to `true`. Default `false`
         :param pulumi.Input[bool] force_refresh: Used internally by the provider to temporarily indicate if all resources should call their associated API to update the
                local state. This is for scenarios where the service version has been reverted outside of Terraform (e.g. via the Fastly
                UI) and the provider needs to resync the state for a different active version (this is only if `activate` is `true`).
-        :param pulumi.Input[Sequence[pulumi.Input['ServiceVclHealthcheckArgs']]] healthchecks: Name of a defined `healthcheck` to assign to this backend
         :param pulumi.Input[bool] http3: Enables support for the HTTP/3 (QUIC) protocol
         :param pulumi.Input[bool] imported: Used internally by the provider to temporarily indicate if the service is being imported, and is reset to false once the import is finished
-        :param pulumi.Input[str] name: A unique name to identify this ACL. It is important to note that changing this attribute will delete and recreate the ACL, and discard the current items in the ACL
-        :param pulumi.Input[Sequence[pulumi.Input['ServiceVclResponseObjectArgs']]] response_objects: The name of the response object used by the Web Application Firewall
+        :param pulumi.Input[str] name: The unique name for the Service to create
         :param pulumi.Input[bool] reuse: Services that are active cannot be destroyed. If set to `true` a service Terraform intends to destroy will instead be
                deactivated (allowing it to be reused by importing it into another Terraform project). If `false`, attempting to destroy
                an active service will cause an error. Default `false`
         :param pulumi.Input[bool] stale_if_error: Enables serving a stale object if there is an error
         :param pulumi.Input[int] stale_if_error_ttl: The default time-to-live (TTL) for serving the stale object for the version
         :param pulumi.Input[str] version_comment: Description field for the version
         """
@@ -965,17 +950,14 @@
             pulumi.set(__self__, "version_comment", version_comment)
         if waf is not None:
             pulumi.set(__self__, "waf", waf)
 
     @property
     @pulumi.getter
     def acls(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['ServiceVclAclArgs']]]]:
-        """
-        The AWS [Canned ACL](https://docs.aws.amazon.com/AmazonS3/latest/userguide/acl-overview.html#canned-acl) to use for objects uploaded to the S3 bucket. Options are: `private`, `public-read`, `public-read-write`, `aws-exec-read`, `authenticated-read`, `bucket-owner-read`, `bucket-owner-full-control`
-        """
         return pulumi.get(self, "acls")
 
     @acls.setter
     def acls(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['ServiceVclAclArgs']]]]):
         pulumi.set(self, "acls", value)
 
     @property
@@ -1032,15 +1014,15 @@
     def cloned_version(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "cloned_version", value)
 
     @property
     @pulumi.getter
     def comment(self) -> Optional[pulumi.Input[str]]:
         """
-        An optional comment about the Director
+        Description field for the service. Default `Managed by Terraform`
         """
         return pulumi.get(self, "comment")
 
     @comment.setter
     def comment(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "comment", value)
 
@@ -1053,15 +1035,15 @@
     def conditions(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['ServiceVclConditionArgs']]]]):
         pulumi.set(self, "conditions", value)
 
     @property
     @pulumi.getter(name="defaultHost")
     def default_host(self) -> Optional[pulumi.Input[str]]:
         """
-        Sets the host header
+        The default hostname
         """
         return pulumi.get(self, "default_host")
 
     @default_host.setter
     def default_host(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "default_host", value)
 
@@ -1095,15 +1077,15 @@
     def directors(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['ServiceVclDirectorArgs']]]]):
         pulumi.set(self, "directors", value)
 
     @property
     @pulumi.getter
     def domains(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['ServiceVclDomainArgs']]]]:
         """
-        The domain of the DigitalOcean Spaces endpoint (default `nyc3.digitaloceanspaces.com`)
+        A set of Domain names to serve as entry points for your Service
         """
         return pulumi.get(self, "domains")
 
     @domains.setter
     def domains(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['ServiceVclDomainArgs']]]]):
         pulumi.set(self, "domains", value)
 
@@ -1116,15 +1098,15 @@
     def dynamicsnippets(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['ServiceVclDynamicsnippetArgs']]]]):
         pulumi.set(self, "dynamicsnippets", value)
 
     @property
     @pulumi.getter(name="forceDestroy")
     def force_destroy(self) -> Optional[pulumi.Input[bool]]:
         """
-        Allow the ACL to be deleted, even if it contains entries. Defaults to false.
+        Services that are active cannot be destroyed. In order to destroy the Service, set `force_destroy` to `true`. Default `false`
         """
         return pulumi.get(self, "force_destroy")
 
     @force_destroy.setter
     def force_destroy(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "force_destroy", value)
 
@@ -1159,17 +1141,14 @@
     @headers.setter
     def headers(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['ServiceVclHeaderArgs']]]]):
         pulumi.set(self, "headers", value)
 
     @property
     @pulumi.getter
     def healthchecks(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['ServiceVclHealthcheckArgs']]]]:
-        """
-        Name of a defined `healthcheck` to assign to this backend
-        """
         return pulumi.get(self, "healthchecks")
 
     @healthchecks.setter
     def healthchecks(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['ServiceVclHealthcheckArgs']]]]):
         pulumi.set(self, "healthchecks", value)
 
     @property
@@ -1439,15 +1418,15 @@
     def logging_syslogs(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['ServiceVclLoggingSyslogArgs']]]]):
         pulumi.set(self, "logging_syslogs", value)
 
     @property
     @pulumi.getter
     def name(self) -> Optional[pulumi.Input[str]]:
         """
-        A unique name to identify this ACL. It is important to note that changing this attribute will delete and recreate the ACL, and discard the current items in the ACL
+        The unique name for the Service to create
         """
         return pulumi.get(self, "name")
 
     @name.setter
     def name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "name", value)
 
@@ -1477,17 +1456,14 @@
     @request_settings.setter
     def request_settings(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['ServiceVclRequestSettingArgs']]]]):
         pulumi.set(self, "request_settings", value)
 
     @property
     @pulumi.getter(name="responseObjects")
     def response_objects(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['ServiceVclResponseObjectArgs']]]]:
-        """
-        The name of the response object used by the Web Application Firewall
-        """
         return pulumi.get(self, "response_objects")
 
     @response_objects.setter
     def response_objects(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['ServiceVclResponseObjectArgs']]]]):
         pulumi.set(self, "response_objects", value)
 
     @property
@@ -1645,25 +1621,22 @@
 
         ```sh
         $ pulumi import fastly:index/serviceVcl:ServiceVcl demo xxxxxxxxxxxxxxxxxxxx@2
         ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ServiceVclAclArgs']]]] acls: The AWS [Canned ACL](https://docs.aws.amazon.com/AmazonS3/latest/userguide/acl-overview.html#canned-acl) to use for objects uploaded to the S3 bucket. Options are: `private`, `public-read`, `public-read-write`, `aws-exec-read`, `authenticated-read`, `bucket-owner-read`, `bucket-owner-full-control`
         :param pulumi.Input[bool] activate: Conditionally prevents the Service from being activated. The apply step will continue to create a new draft version but will not activate it if this is set to `false`. Default `true`
-        :param pulumi.Input[str] comment: An optional comment about the Director
-        :param pulumi.Input[str] default_host: Sets the host header
+        :param pulumi.Input[str] comment: Description field for the service. Default `Managed by Terraform`
+        :param pulumi.Input[str] default_host: The default hostname
         :param pulumi.Input[int] default_ttl: The default Time-to-live (TTL) for requests
-        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ServiceVclDomainArgs']]]] domains: The domain of the DigitalOcean Spaces endpoint (default `nyc3.digitaloceanspaces.com`)
-        :param pulumi.Input[bool] force_destroy: Allow the ACL to be deleted, even if it contains entries. Defaults to false.
-        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ServiceVclHealthcheckArgs']]]] healthchecks: Name of a defined `healthcheck` to assign to this backend
+        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ServiceVclDomainArgs']]]] domains: A set of Domain names to serve as entry points for your Service
+        :param pulumi.Input[bool] force_destroy: Services that are active cannot be destroyed. In order to destroy the Service, set `force_destroy` to `true`. Default `false`
         :param pulumi.Input[bool] http3: Enables support for the HTTP/3 (QUIC) protocol
-        :param pulumi.Input[str] name: A unique name to identify this ACL. It is important to note that changing this attribute will delete and recreate the ACL, and discard the current items in the ACL
-        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ServiceVclResponseObjectArgs']]]] response_objects: The name of the response object used by the Web Application Firewall
+        :param pulumi.Input[str] name: The unique name for the Service to create
         :param pulumi.Input[bool] reuse: Services that are active cannot be destroyed. If set to `true` a service Terraform intends to destroy will instead be
                deactivated (allowing it to be reused by importing it into another Terraform project). If `false`, attempting to destroy
                an active service will cause an error. Default `false`
         :param pulumi.Input[bool] stale_if_error: Enables serving a stale object if there is an error
         :param pulumi.Input[int] stale_if_error_ttl: The default time-to-live (TTL) for serving the stale object for the version
         :param pulumi.Input[str] version_comment: Description field for the version
         """
@@ -1905,31 +1878,28 @@
         """
         Get an existing ServiceVcl resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ServiceVclAclArgs']]]] acls: The AWS [Canned ACL](https://docs.aws.amazon.com/AmazonS3/latest/userguide/acl-overview.html#canned-acl) to use for objects uploaded to the S3 bucket. Options are: `private`, `public-read`, `public-read-write`, `aws-exec-read`, `authenticated-read`, `bucket-owner-read`, `bucket-owner-full-control`
         :param pulumi.Input[bool] activate: Conditionally prevents the Service from being activated. The apply step will continue to create a new draft version but will not activate it if this is set to `false`. Default `true`
         :param pulumi.Input[int] active_version: The currently active version of your Fastly Service
         :param pulumi.Input[int] cloned_version: The latest cloned version by the provider
-        :param pulumi.Input[str] comment: An optional comment about the Director
-        :param pulumi.Input[str] default_host: Sets the host header
+        :param pulumi.Input[str] comment: Description field for the service. Default `Managed by Terraform`
+        :param pulumi.Input[str] default_host: The default hostname
         :param pulumi.Input[int] default_ttl: The default Time-to-live (TTL) for requests
-        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ServiceVclDomainArgs']]]] domains: The domain of the DigitalOcean Spaces endpoint (default `nyc3.digitaloceanspaces.com`)
-        :param pulumi.Input[bool] force_destroy: Allow the ACL to be deleted, even if it contains entries. Defaults to false.
+        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ServiceVclDomainArgs']]]] domains: A set of Domain names to serve as entry points for your Service
+        :param pulumi.Input[bool] force_destroy: Services that are active cannot be destroyed. In order to destroy the Service, set `force_destroy` to `true`. Default `false`
         :param pulumi.Input[bool] force_refresh: Used internally by the provider to temporarily indicate if all resources should call their associated API to update the
                local state. This is for scenarios where the service version has been reverted outside of Terraform (e.g. via the Fastly
                UI) and the provider needs to resync the state for a different active version (this is only if `activate` is `true`).
-        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ServiceVclHealthcheckArgs']]]] healthchecks: Name of a defined `healthcheck` to assign to this backend
         :param pulumi.Input[bool] http3: Enables support for the HTTP/3 (QUIC) protocol
         :param pulumi.Input[bool] imported: Used internally by the provider to temporarily indicate if the service is being imported, and is reset to false once the import is finished
-        :param pulumi.Input[str] name: A unique name to identify this ACL. It is important to note that changing this attribute will delete and recreate the ACL, and discard the current items in the ACL
-        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ServiceVclResponseObjectArgs']]]] response_objects: The name of the response object used by the Web Application Firewall
+        :param pulumi.Input[str] name: The unique name for the Service to create
         :param pulumi.Input[bool] reuse: Services that are active cannot be destroyed. If set to `true` a service Terraform intends to destroy will instead be
                deactivated (allowing it to be reused by importing it into another Terraform project). If `false`, attempting to destroy
                an active service will cause an error. Default `false`
         :param pulumi.Input[bool] stale_if_error: Enables serving a stale object if there is an error
         :param pulumi.Input[int] stale_if_error_ttl: The default time-to-live (TTL) for serving the stale object for the version
         :param pulumi.Input[str] version_comment: Description field for the version
         """
@@ -1998,17 +1968,14 @@
         __props__.__dict__["version_comment"] = version_comment
         __props__.__dict__["waf"] = waf
         return ServiceVcl(resource_name, opts=opts, __props__=__props__)
 
     @property
     @pulumi.getter
     def acls(self) -> pulumi.Output[Optional[Sequence['outputs.ServiceVclAcl']]]:
-        """
-        The AWS [Canned ACL](https://docs.aws.amazon.com/AmazonS3/latest/userguide/acl-overview.html#canned-acl) to use for objects uploaded to the S3 bucket. Options are: `private`, `public-read`, `public-read-write`, `aws-exec-read`, `authenticated-read`, `bucket-owner-read`, `bucket-owner-full-control`
-        """
         return pulumi.get(self, "acls")
 
     @property
     @pulumi.getter
     def activate(self) -> pulumi.Output[Optional[bool]]:
         """
         Conditionally prevents the Service from being activated. The apply step will continue to create a new draft version but will not activate it if this is set to `false`. Default `true`
@@ -2041,28 +2008,28 @@
         """
         return pulumi.get(self, "cloned_version")
 
     @property
     @pulumi.getter
     def comment(self) -> pulumi.Output[Optional[str]]:
         """
-        An optional comment about the Director
+        Description field for the service. Default `Managed by Terraform`
         """
         return pulumi.get(self, "comment")
 
     @property
     @pulumi.getter
     def conditions(self) -> pulumi.Output[Optional[Sequence['outputs.ServiceVclCondition']]]:
         return pulumi.get(self, "conditions")
 
     @property
     @pulumi.getter(name="defaultHost")
     def default_host(self) -> pulumi.Output[Optional[str]]:
         """
-        Sets the host header
+        The default hostname
         """
         return pulumi.get(self, "default_host")
 
     @property
     @pulumi.getter(name="defaultTtl")
     def default_ttl(self) -> pulumi.Output[Optional[int]]:
         """
@@ -2080,28 +2047,28 @@
     def directors(self) -> pulumi.Output[Optional[Sequence['outputs.ServiceVclDirector']]]:
         return pulumi.get(self, "directors")
 
     @property
     @pulumi.getter
     def domains(self) -> pulumi.Output[Sequence['outputs.ServiceVclDomain']]:
         """
-        The domain of the DigitalOcean Spaces endpoint (default `nyc3.digitaloceanspaces.com`)
+        A set of Domain names to serve as entry points for your Service
         """
         return pulumi.get(self, "domains")
 
     @property
     @pulumi.getter
     def dynamicsnippets(self) -> pulumi.Output[Optional[Sequence['outputs.ServiceVclDynamicsnippet']]]:
         return pulumi.get(self, "dynamicsnippets")
 
     @property
     @pulumi.getter(name="forceDestroy")
     def force_destroy(self) -> pulumi.Output[Optional[bool]]:
         """
-        Allow the ACL to be deleted, even if it contains entries. Defaults to false.
+        Services that are active cannot be destroyed. In order to destroy the Service, set `force_destroy` to `true`. Default `false`
         """
         return pulumi.get(self, "force_destroy")
 
     @property
     @pulumi.getter(name="forceRefresh")
     def force_refresh(self) -> pulumi.Output[bool]:
         """
@@ -2120,17 +2087,14 @@
     @pulumi.getter
     def headers(self) -> pulumi.Output[Optional[Sequence['outputs.ServiceVclHeader']]]:
         return pulumi.get(self, "headers")
 
     @property
     @pulumi.getter
     def healthchecks(self) -> pulumi.Output[Optional[Sequence['outputs.ServiceVclHealthcheck']]]:
-        """
-        Name of a defined `healthcheck` to assign to this backend
-        """
         return pulumi.get(self, "healthchecks")
 
     @property
     @pulumi.getter
     def http3(self) -> pulumi.Output[Optional[bool]]:
         """
         Enables support for the HTTP/3 (QUIC) protocol
@@ -2280,15 +2244,15 @@
     def logging_syslogs(self) -> pulumi.Output[Optional[Sequence['outputs.ServiceVclLoggingSyslog']]]:
         return pulumi.get(self, "logging_syslogs")
 
     @property
     @pulumi.getter
     def name(self) -> pulumi.Output[str]:
         """
-        A unique name to identify this ACL. It is important to note that changing this attribute will delete and recreate the ACL, and discard the current items in the ACL
+        The unique name for the Service to create
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter(name="productEnablement")
     def product_enablement(self) -> pulumi.Output[Optional['outputs.ServiceVclProductEnablement']]:
         return pulumi.get(self, "product_enablement")
@@ -2302,17 +2266,14 @@
     @pulumi.getter(name="requestSettings")
     def request_settings(self) -> pulumi.Output[Optional[Sequence['outputs.ServiceVclRequestSetting']]]:
         return pulumi.get(self, "request_settings")
 
     @property
     @pulumi.getter(name="responseObjects")
     def response_objects(self) -> pulumi.Output[Optional[Sequence['outputs.ServiceVclResponseObject']]]:
-        """
-        The name of the response object used by the Web Application Firewall
-        """
         return pulumi.get(self, "response_objects")
 
     @property
     @pulumi.getter
     def reuse(self) -> pulumi.Output[Optional[bool]]:
         """
         Services that are active cannot be destroyed. If set to `true` a service Terraform intends to destroy will instead be
```

### Comparing `pulumi_fastly-8.6.0a1713812915/pulumi_fastly/service_waf_configuration.py` & `pulumi_fastly-8.7.0a1713897687/pulumi_fastly/service_waf_configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -580,15 +580,15 @@
         :param pulumi.Input[str] high_risk_country_codes: A space-separated list of country codes in ISO 3166-1 (two-letter) format
         :param pulumi.Input[int] http_violation_score_threshold: HTTP violation threshold
         :param pulumi.Input[int] inbound_anomaly_score_threshold: Inbound anomaly threshold
         :param pulumi.Input[int] lfi_score_threshold: Local file inclusion attack threshold
         :param pulumi.Input[int] max_file_size: The maximum allowed file size, in bytes
         :param pulumi.Input[int] max_num_args: The maximum number of arguments allowed
         :param pulumi.Input[int] notice_anomaly_score: Score value to add for notice anomalies
-        :param pulumi.Input[int] number: The numeric ID assigned to the WAF Rule Exclusion
+        :param pulumi.Input[int] number: The WAF firewall version
         :param pulumi.Input[int] paranoia_level: The configured paranoia level
         :param pulumi.Input[int] php_injection_score_threshold: PHP injection threshold
         :param pulumi.Input[int] rce_score_threshold: Remote code execution threshold
         :param pulumi.Input[str] restricted_extensions: A space-separated list of allowed file extensions
         :param pulumi.Input[str] restricted_headers: A space-separated list of allowed header names
         :param pulumi.Input[int] rfi_score_threshold: Remote file inclusion attack threshold
         :param pulumi.Input[int] session_fixation_score_threshold: Session fixation attack threshold
@@ -909,15 +909,15 @@
     def notice_anomaly_score(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "notice_anomaly_score", value)
 
     @property
     @pulumi.getter
     def number(self) -> Optional[pulumi.Input[int]]:
         """
-        The numeric ID assigned to the WAF Rule Exclusion
+        The WAF firewall version
         """
         return pulumi.get(self, "number")
 
     @number.setter
     def number(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "number", value)
 
@@ -1127,15 +1127,14 @@
 
         > **Warning:** This provider will take precedence over any changes you make in the UI or API. Such changes are likely to be reversed if you run the provider again.
 
         ## Example Usage
 
         Basic usage:
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_fastly as fastly
 
         demo = fastly.ServiceVcl("demo",
             name="demofastly",
             domains=[fastly.ServiceVclDomainArgs(
@@ -1172,19 +1171,17 @@
                 response_object="WAF_Response",
             ),
             force_destroy=True)
         waf = fastly.ServiceWafConfiguration("waf",
             waf_id=demo.waf.waf_id,
             http_violation_score_threshold=100)
         ```
-        <!--End PulumiCodeChooser -->
 
         Usage with rules:
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_fastly as fastly
 
         demo = fastly.ServiceVcl("demo",
             name="demofastly",
             domains=[fastly.ServiceVclDomainArgs(
@@ -1226,21 +1223,19 @@
             http_violation_score_threshold=100,
             rules=[fastly.ServiceWafConfigurationRuleArgs(
                 modsec_rule_id=1010090,
                 revision=1,
                 status="log",
             )])
         ```
-        <!--End PulumiCodeChooser -->
 
         Usage with rule exclusions:
 
         > **Warning:** Rule exclusions are part of a **beta release**, which may be subject to breaking changes and improvements over time. For more information, see our [product and feature lifecycle](https://docs.fastly.com/products/fastly-product-lifecycle#beta) descriptions.
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_fastly as fastly
 
         demo = fastly.ServiceVcl("demo",
             name="demofastly",
             domains=[fastly.ServiceVclDomainArgs(
@@ -1288,15 +1283,14 @@
             rule_exclusions=[fastly.ServiceWafConfigurationRuleExclusionArgs(
                 name="index page",
                 exclusion_type="rule",
                 condition="req.url.basename == \\"index.html\\"",
                 modsec_rule_ids=[2029718],
             )])
         ```
-        <!--End PulumiCodeChooser -->
 
         Usage with rules from data source:
 
         ## Import
 
         This is an example of the import command being applied to the resource named `fastly_service_waf_configuration.waf`
 
@@ -1350,15 +1344,14 @@
 
         > **Warning:** This provider will take precedence over any changes you make in the UI or API. Such changes are likely to be reversed if you run the provider again.
 
         ## Example Usage
 
         Basic usage:
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_fastly as fastly
 
         demo = fastly.ServiceVcl("demo",
             name="demofastly",
             domains=[fastly.ServiceVclDomainArgs(
@@ -1395,19 +1388,17 @@
                 response_object="WAF_Response",
             ),
             force_destroy=True)
         waf = fastly.ServiceWafConfiguration("waf",
             waf_id=demo.waf.waf_id,
             http_violation_score_threshold=100)
         ```
-        <!--End PulumiCodeChooser -->
 
         Usage with rules:
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_fastly as fastly
 
         demo = fastly.ServiceVcl("demo",
             name="demofastly",
             domains=[fastly.ServiceVclDomainArgs(
@@ -1449,21 +1440,19 @@
             http_violation_score_threshold=100,
             rules=[fastly.ServiceWafConfigurationRuleArgs(
                 modsec_rule_id=1010090,
                 revision=1,
                 status="log",
             )])
         ```
-        <!--End PulumiCodeChooser -->
 
         Usage with rule exclusions:
 
         > **Warning:** Rule exclusions are part of a **beta release**, which may be subject to breaking changes and improvements over time. For more information, see our [product and feature lifecycle](https://docs.fastly.com/products/fastly-product-lifecycle#beta) descriptions.
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_fastly as fastly
 
         demo = fastly.ServiceVcl("demo",
             name="demofastly",
             domains=[fastly.ServiceVclDomainArgs(
@@ -1511,15 +1500,14 @@
             rule_exclusions=[fastly.ServiceWafConfigurationRuleExclusionArgs(
                 name="index page",
                 exclusion_type="rule",
                 condition="req.url.basename == \\"index.html\\"",
                 modsec_rule_ids=[2029718],
             )])
         ```
-        <!--End PulumiCodeChooser -->
 
         Usage with rules from data source:
 
         ## Import
 
         This is an example of the import command being applied to the resource named `fastly_service_waf_configuration.waf`
 
@@ -1690,15 +1678,15 @@
         :param pulumi.Input[str] high_risk_country_codes: A space-separated list of country codes in ISO 3166-1 (two-letter) format
         :param pulumi.Input[int] http_violation_score_threshold: HTTP violation threshold
         :param pulumi.Input[int] inbound_anomaly_score_threshold: Inbound anomaly threshold
         :param pulumi.Input[int] lfi_score_threshold: Local file inclusion attack threshold
         :param pulumi.Input[int] max_file_size: The maximum allowed file size, in bytes
         :param pulumi.Input[int] max_num_args: The maximum number of arguments allowed
         :param pulumi.Input[int] notice_anomaly_score: Score value to add for notice anomalies
-        :param pulumi.Input[int] number: The numeric ID assigned to the WAF Rule Exclusion
+        :param pulumi.Input[int] number: The WAF firewall version
         :param pulumi.Input[int] paranoia_level: The configured paranoia level
         :param pulumi.Input[int] php_injection_score_threshold: PHP injection threshold
         :param pulumi.Input[int] rce_score_threshold: Remote code execution threshold
         :param pulumi.Input[str] restricted_extensions: A space-separated list of allowed file extensions
         :param pulumi.Input[str] restricted_headers: A space-separated list of allowed header names
         :param pulumi.Input[int] rfi_score_threshold: Remote file inclusion attack threshold
         :param pulumi.Input[int] session_fixation_score_threshold: Session fixation attack threshold
@@ -1909,15 +1897,15 @@
         """
         return pulumi.get(self, "notice_anomaly_score")
 
     @property
     @pulumi.getter
     def number(self) -> pulumi.Output[int]:
         """
-        The numeric ID assigned to the WAF Rule Exclusion
+        The WAF firewall version
         """
         return pulumi.get(self, "number")
 
     @property
     @pulumi.getter(name="paranoiaLevel")
     def paranoia_level(self) -> pulumi.Output[int]:
         """
```

### Comparing `pulumi_fastly-8.6.0a1713812915/pulumi_fastly/tls_activation.py` & `pulumi_fastly-8.7.0a1713897687/pulumi_fastly/tls_activation.py`

 * *Files 1% similar despite different names*

```diff
@@ -184,15 +184,14 @@
 
         > **Note:** The Fastly service must be provisioned _prior_ to enabling TLS on it. This can be achieved in Pulumi using `depends_on`.
 
         ## Example Usage
 
         Basic usage:
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_fastly as fastly
 
         demo = fastly.ServiceVcl("demo",
             name="my-service",
             domains=[fastly.ServiceVclDomainArgs(
@@ -211,15 +210,14 @@
             name="demo-cert",
             opts=pulumi.ResourceOptions(depends_on=[demo_tls_private_key]))
         test = fastly.TlsActivation("test",
             certificate_id=demo_tls_certificate.id,
             domain="example.com",
             opts=pulumi.ResourceOptions(depends_on=[demo]))
         ```
-        <!--End PulumiCodeChooser -->
 
         > **Warning:** Updating the `TlsPrivateKey`/`TlsCertificate` resources should be done in multiple plan/apply steps to avoid potential downtime. The new certificate and associated private key must first be created so they exist alongside the currently active resources. Once the new resources have been created, then the `TlsActivation` can be updated to point to the new certificate. Finally, the original key/certificate resources can be deleted.
 
         ## Import
 
         A TLS activation can be imported using its ID, e.g.
 
@@ -245,15 +243,14 @@
 
         > **Note:** The Fastly service must be provisioned _prior_ to enabling TLS on it. This can be achieved in Pulumi using `depends_on`.
 
         ## Example Usage
 
         Basic usage:
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_fastly as fastly
 
         demo = fastly.ServiceVcl("demo",
             name="my-service",
             domains=[fastly.ServiceVclDomainArgs(
@@ -272,15 +269,14 @@
             name="demo-cert",
             opts=pulumi.ResourceOptions(depends_on=[demo_tls_private_key]))
         test = fastly.TlsActivation("test",
             certificate_id=demo_tls_certificate.id,
             domain="example.com",
             opts=pulumi.ResourceOptions(depends_on=[demo]))
         ```
-        <!--End PulumiCodeChooser -->
 
         > **Warning:** Updating the `TlsPrivateKey`/`TlsCertificate` resources should be done in multiple plan/apply steps to avoid potential downtime. The new certificate and associated private key must first be created so they exist alongside the currently active resources. Once the new resources have been created, then the `TlsActivation` can be updated to point to the new certificate. Finally, the original key/certificate resources can be deleted.
 
         ## Import
 
         A TLS activation can be imported using its ID, e.g.
```

### Comparing `pulumi_fastly-8.6.0a1713812915/pulumi_fastly/tls_certificate.py` & `pulumi_fastly-8.7.0a1713897687/pulumi_fastly/tls_certificate.py`

 * *Files 1% similar despite different names*

```diff
@@ -232,15 +232,14 @@
         > Each TLS certificate **must** have its corresponding private key uploaded _prior_ to uploading the certificate. This
         can be achieved in Pulumi using `depends_on`
 
         ## Example Usage
 
         Basic usage:
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_fastly as fastly
         import pulumi_tls as tls
 
         key = tls.index.PrivateKey("key", algorithm=RSA)
         cert = tls.index.SelfSignedCert("cert",
@@ -260,15 +259,14 @@
             key_pem=key["privateKeyPem"],
             name="tf-demo")
         example = fastly.TlsCertificate("example",
             name="tf-demo",
             certificate_body=cert["certPem"],
             opts=pulumi.ResourceOptions(depends_on=[key_tls_private_key]))
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Updating certificates
 
         There are three scenarios for updating a certificate:
 
         1. The certificate is about to expire but the private key stays the same.
         2. The certificate is about to expire but the private key is changing.
@@ -303,15 +301,14 @@
         > Each TLS certificate **must** have its corresponding private key uploaded _prior_ to uploading the certificate. This
         can be achieved in Pulumi using `depends_on`
 
         ## Example Usage
 
         Basic usage:
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_fastly as fastly
         import pulumi_tls as tls
 
         key = tls.index.PrivateKey("key", algorithm=RSA)
         cert = tls.index.SelfSignedCert("cert",
@@ -331,15 +328,14 @@
             key_pem=key["privateKeyPem"],
             name="tf-demo")
         example = fastly.TlsCertificate("example",
             name="tf-demo",
             certificate_body=cert["certPem"],
             opts=pulumi.ResourceOptions(depends_on=[key_tls_private_key]))
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Updating certificates
 
         There are three scenarios for updating a certificate:
 
         1. The certificate is about to expire but the private key stays the same.
         2. The certificate is about to expire but the private key is changing.
```

### Comparing `pulumi_fastly-8.6.0a1713812915/pulumi_fastly/tls_mutual_authentication.py` & `pulumi_fastly-8.7.0a1713897687/pulumi_fastly/tls_mutual_authentication.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.6.0a1713812915/pulumi_fastly/tls_platform_certificate.py` & `pulumi_fastly-8.7.0a1713897687/pulumi_fastly/tls_platform_certificate.py`

 * *Files 0% similar despite different names*

```diff
@@ -264,15 +264,14 @@
         > Each TLS certificate **must** have its corresponding private key uploaded _prior_ to uploading the certificate. This
         can be achieved in Pulumi using `depends_on`
 
         ## Example Usage
 
         Basic usage with self-signed CA:
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_fastly as fastly
         import pulumi_tls as tls
 
         ca_key = tls.index.PrivateKey("ca_key", algorithm=RSA)
         key = tls.index.PrivateKey("key", algorithm=RSA)
@@ -315,15 +314,14 @@
         cert_tls_platform_certificate = fastly.TlsPlatformCertificate("cert",
             certificate_body=cert["certPem"],
             intermediates_blob=ca["certPem"],
             configuration_id=config.id,
             allow_untrusted_root=True,
             opts=pulumi.ResourceOptions(depends_on=[key_tls_private_key]))
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         A certificate can be imported using its Fastly certificate ID, e.g.
 
         ```sh
         $ pulumi import fastly:index/tlsPlatformCertificate:TlsPlatformCertificate demo xxxxxxxxxxx
@@ -348,15 +346,14 @@
         > Each TLS certificate **must** have its corresponding private key uploaded _prior_ to uploading the certificate. This
         can be achieved in Pulumi using `depends_on`
 
         ## Example Usage
 
         Basic usage with self-signed CA:
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_fastly as fastly
         import pulumi_tls as tls
 
         ca_key = tls.index.PrivateKey("ca_key", algorithm=RSA)
         key = tls.index.PrivateKey("key", algorithm=RSA)
@@ -399,15 +396,14 @@
         cert_tls_platform_certificate = fastly.TlsPlatformCertificate("cert",
             certificate_body=cert["certPem"],
             intermediates_blob=ca["certPem"],
             configuration_id=config.id,
             allow_untrusted_root=True,
             opts=pulumi.ResourceOptions(depends_on=[key_tls_private_key]))
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         A certificate can be imported using its Fastly certificate ID, e.g.
 
         ```sh
         $ pulumi import fastly:index/tlsPlatformCertificate:TlsPlatformCertificate demo xxxxxxxxxxx
```

### Comparing `pulumi_fastly-8.6.0a1713812915/pulumi_fastly/tls_private_key.py` & `pulumi_fastly-8.7.0a1713897687/pulumi_fastly/tls_private_key.py`

 * *Files 2% similar despite different names*

```diff
@@ -183,26 +183,24 @@
 
         The Private Key resource requires a key in PEM format, and a name to identify it.
 
         ## Example Usage
 
         Basic usage:
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_fastly as fastly
         import pulumi_tls as tls
 
         demo = tls.index.PrivateKey("demo", algorithm=RSA)
         demo_tls_private_key = fastly.TlsPrivateKey("demo",
             key_pem=demo["privateKeyPem"],
             name="tf-demo")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         A Private Key can be imported using its ID, e.g.
 
         ```sh
         $ pulumi import fastly:index/tlsPrivateKey:TlsPrivateKey demo xxxxxxxxxxx
@@ -224,26 +222,24 @@
 
         The Private Key resource requires a key in PEM format, and a name to identify it.
 
         ## Example Usage
 
         Basic usage:
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_fastly as fastly
         import pulumi_tls as tls
 
         demo = tls.index.PrivateKey("demo", algorithm=RSA)
         demo_tls_private_key = fastly.TlsPrivateKey("demo",
             key_pem=demo["privateKeyPem"],
             name="tf-demo")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         A Private Key can be imported using its ID, e.g.
 
         ```sh
         $ pulumi import fastly:index/tlsPrivateKey:TlsPrivateKey demo xxxxxxxxxxx
```

### Comparing `pulumi_fastly-8.6.0a1713812915/pulumi_fastly/tls_subscription.py` & `pulumi_fastly-8.7.0a1713897687/pulumi_fastly/tls_subscription.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.6.0a1713812915/pulumi_fastly/tls_subscription_validation.py` & `pulumi_fastly-8.7.0a1713897687/pulumi_fastly/tls_subscription_validation.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.6.0a1713812915/pulumi_fastly/user.py` & `pulumi_fastly-8.7.0a1713897687/pulumi_fastly/user.py`

 * *Files 2% similar despite different names*

```diff
@@ -136,24 +136,22 @@
 
         The User resource requires a login and name, and optionally a role.
 
         ## Example Usage
 
         Basic usage:
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_fastly as fastly
 
         demo = fastly.User("demo",
             login="demo@example.com",
             name="Demo User")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         A Fastly User can be imported using their user ID, e.g.
 
         ```sh
         $ pulumi import fastly:index/user:User demo xxxxxxxxxxxxxxxxxxxx
@@ -176,24 +174,22 @@
 
         The User resource requires a login and name, and optionally a role.
 
         ## Example Usage
 
         Basic usage:
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_fastly as fastly
 
         demo = fastly.User("demo",
             login="demo@example.com",
             name="Demo User")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         A Fastly User can be imported using their user ID, e.g.
 
         ```sh
         $ pulumi import fastly:index/user:User demo xxxxxxxxxxxxxxxxxxxx
```

### Comparing `pulumi_fastly-8.6.0a1713812915/pulumi_fastly.egg-info/PKG-INFO` & `pulumi_fastly-8.7.0a1713897687/pulumi_fastly.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_fastly
-Version: 8.6.0a1713812915
+Version: 8.7.0a1713897687
 Summary: A Pulumi package for creating and managing fastly cloud resources.
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.io
 Project-URL: Repository, https://github.com/pulumi/pulumi-fastly
 Keywords: pulumi,fastly
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_fastly-8.6.0a1713812915/pulumi_fastly.egg-info/SOURCES.txt` & `pulumi_fastly-8.7.0a1713897687/pulumi_fastly.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.6.0a1713812915/pyproject.toml` & `pulumi_fastly-8.7.0a1713897687/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [project]
   name = "pulumi_fastly"
   description = "A Pulumi package for creating and managing fastly cloud resources."
   dependencies = ["parver>=0.2.1", "pulumi>=3.0.0,<4.0.0", "semver>=2.8.1"]
   keywords = ["pulumi", "fastly"]
   readme = "README.md"
   requires-python = ">=3.8"
-  version = "8.6.0a1713812915"
+  version = "8.7.0a1713897687"
   [project.license]
     text = "Apache-2.0"
   [project.urls]
     Homepage = "https://pulumi.io"
     Repository = "https://github.com/pulumi/pulumi-fastly"
 
 [build-system]
```

