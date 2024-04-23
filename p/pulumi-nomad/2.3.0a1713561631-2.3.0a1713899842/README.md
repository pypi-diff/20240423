# Comparing `tmp/pulumi_nomad-2.3.0a1713561631.tar.gz` & `tmp/pulumi_nomad-2.3.0a1713899842.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_nomad-2.3.0a1713561631.tar", last modified: Fri Apr 19 21:30:04 2024, max compression
+gzip compressed data, was "pulumi_nomad-2.3.0a1713899842.tar", last modified: Tue Apr 23 19:47:43 2024, max compression
```

## Comparing `pulumi_nomad-2.3.0a1713561631.tar` & `pulumi_nomad-2.3.0a1713899842.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:30:04.172101 pulumi_nomad-2.3.0a1713561631/
--rw-r--r--   0 runner    (1001) docker     (127)     4727 2024-04-19 21:30:04.172101 pulumi_nomad-2.3.0a1713561631/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4279 2024-04-19 21:29:57.000000 pulumi_nomad-2.3.0a1713561631/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:30:04.168101 pulumi_nomad-2.3.0a1713561631/pulumi_nomad/
--rw-r--r--   0 runner    (1001) docker     (127)     4332 2024-04-19 21:29:57.000000 pulumi_nomad-2.3.0a1713561631/pulumi_nomad/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    73944 2024-04-19 21:29:57.000000 pulumi_nomad-2.3.0a1713561631/pulumi_nomad/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-04-19 21:29:57.000000 pulumi_nomad-2.3.0a1713561631/pulumi_nomad/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)    23930 2024-04-19 21:29:57.000000 pulumi_nomad-2.3.0a1713561631/pulumi_nomad/acl_auth_method.py
--rw-r--r--   0 runner    (1001) docker     (127)    16396 2024-04-19 21:29:57.000000 pulumi_nomad-2.3.0a1713561631/pulumi_nomad/acl_binding_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)    12176 2024-04-19 21:29:57.000000 pulumi_nomad-2.3.0a1713561631/pulumi_nomad/acl_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)    10526 2024-04-19 21:29:57.000000 pulumi_nomad-2.3.0a1713561631/pulumi_nomad/acl_role.py
--rw-r--r--   0 runner    (1001) docker     (127)    29351 2024-04-19 21:29:57.000000 pulumi_nomad-2.3.0a1713561631/pulumi_nomad/acl_token.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:30:04.172101 pulumi_nomad-2.3.0a1713561631/pulumi_nomad/config/
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-19 21:29:57.000000 pulumi_nomad-2.3.0a1713561631/pulumi_nomad/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1865 2024-04-19 21:29:57.000000 pulumi_nomad-2.3.0a1713561631/pulumi_nomad/config/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-04-19 21:29:57.000000 pulumi_nomad-2.3.0a1713561631/pulumi_nomad/config/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     3432 2024-04-19 21:29:57.000000 pulumi_nomad-2.3.0a1713561631/pulumi_nomad/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (127)    50670 2024-04-19 21:29:57.000000 pulumi_nomad-2.3.0a1713561631/pulumi_nomad/csi_volume.py
--rw-r--r--   0 runner    (1001) docker     (127)    52609 2024-04-19 21:29:57.000000 pulumi_nomad-2.3.0a1713561631/pulumi_nomad/csi_volume_registration.py
--rw-r--r--   0 runner    (1001) docker     (127)    52663 2024-04-19 21:29:57.000000 pulumi_nomad-2.3.0a1713561631/pulumi_nomad/external_volume.py
--rw-r--r--   0 runner    (1001) docker     (127)     3690 2024-04-19 21:29:57.000000 pulumi_nomad-2.3.0a1713561631/pulumi_nomad/get_acl_policies.py
--rw-r--r--   0 runner    (1001) docker     (127)     3940 2024-04-19 21:29:57.000000 pulumi_nomad-2.3.0a1713561631/pulumi_nomad/get_acl_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)     4013 2024-04-19 21:29:57.000000 pulumi_nomad-2.3.0a1713561631/pulumi_nomad/get_acl_role.py
--rw-r--r--   0 runner    (1001) docker     (127)     3586 2024-04-19 21:29:57.000000 pulumi_nomad-2.3.0a1713561631/pulumi_nomad/get_acl_roles.py
--rw-r--r--   0 runner    (1001) docker     (127)     7770 2024-04-19 21:29:57.000000 pulumi_nomad-2.3.0a1713561631/pulumi_nomad/get_acl_token.py
--rw-r--r--   0 runner    (1001) docker     (127)     3559 2024-04-19 21:29:57.000000 pulumi_nomad-2.3.0a1713561631/pulumi_nomad/get_acl_tokens.py
--rw-r--r--   0 runner    (1001) docker     (127)     5490 2024-04-19 21:29:57.000000 pulumi_nomad-2.3.0a1713561631/pulumi_nomad/get_allocations.py
--rw-r--r--   0 runner    (1001) docker     (127)     4787 2024-04-19 21:29:57.000000 pulumi_nomad-2.3.0a1713561631/pulumi_nomad/get_datacenters.py
--rw-r--r--   0 runner    (1001) docker     (127)     2855 2024-04-19 21:29:57.000000 pulumi_nomad-2.3.0a1713561631/pulumi_nomad/get_deployments.py
--rw-r--r--   0 runner    (1001) docker     (127)    13544 2024-04-19 21:29:57.000000 pulumi_nomad-2.3.0a1713561631/pulumi_nomad/get_job.py
--rw-r--r--   0 runner    (1001) docker     (127)     4001 2024-04-19 21:29:57.000000 pulumi_nomad-2.3.0a1713561631/pulumi_nomad/get_job_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     5484 2024-04-19 21:29:57.000000 pulumi_nomad-2.3.0a1713561631/pulumi_nomad/get_namespace.py
--rw-r--r--   0 runner    (1001) docker     (127)     3701 2024-04-19 21:29:57.000000 pulumi_nomad-2.3.0a1713561631/pulumi_nomad/get_namespaces.py
--rw-r--r--   0 runner    (1001) docker     (127)     4567 2024-04-19 21:29:57.000000 pulumi_nomad-2.3.0a1713561631/pulumi_nomad/get_node_pool.py
--rw-r--r--   0 runner    (1001) docker     (127)     4510 2024-04-19 21:29:57.000000 pulumi_nomad-2.3.0a1713561631/pulumi_nomad/get_node_pools.py
--rw-r--r--   0 runner    (1001) docker     (127)    10872 2024-04-19 21:29:57.000000 pulumi_nomad-2.3.0a1713561631/pulumi_nomad/get_plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     3249 2024-04-19 21:29:57.000000 pulumi_nomad-2.3.0a1713561631/pulumi_nomad/get_plugins.py
--rw-r--r--   0 runner    (1001) docker     (127)     3426 2024-04-19 21:29:57.000000 pulumi_nomad-2.3.0a1713561631/pulumi_nomad/get_regions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4798 2024-04-19 21:29:57.000000 pulumi_nomad-2.3.0a1713561631/pulumi_nomad/get_scaling_policies.py
--rw-r--r--   0 runner    (1001) docker     (127)     5256 2024-04-19 21:29:57.000000 pulumi_nomad-2.3.0a1713561631/pulumi_nomad/get_scaling_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)     4686 2024-04-19 21:29:57.000000 pulumi_nomad-2.3.0a1713561631/pulumi_nomad/get_scheduler_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)     4253 2024-04-19 21:29:57.000000 pulumi_nomad-2.3.0a1713561631/pulumi_nomad/get_variable.py
--rw-r--r--   0 runner    (1001) docker     (127)     5560 2024-04-19 21:29:57.000000 pulumi_nomad-2.3.0a1713561631/pulumi_nomad/get_volumes.py
--rw-r--r--   0 runner    (1001) docker     (127)    51951 2024-04-19 21:29:57.000000 pulumi_nomad-2.3.0a1713561631/pulumi_nomad/job.py
--rw-r--r--   0 runner    (1001) docker     (127)    20817 2024-04-19 21:29:57.000000 pulumi_nomad-2.3.0a1713561631/pulumi_nomad/namespace.py
--rw-r--r--   0 runner    (1001) docker     (127)    13282 2024-04-19 21:29:57.000000 pulumi_nomad-2.3.0a1713561631/pulumi_nomad/node_pool.py
--rw-r--r--   0 runner    (1001) docker     (127)   100555 2024-04-19 21:29:57.000000 pulumi_nomad-2.3.0a1713561631/pulumi_nomad/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    21549 2024-04-19 21:29:57.000000 pulumi_nomad-2.3.0a1713561631/pulumi_nomad/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-19 21:29:57.000000 pulumi_nomad-2.3.0a1713561631/pulumi_nomad/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 21:29:57.000000 pulumi_nomad-2.3.0a1713561631/pulumi_nomad/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    12269 2024-04-19 21:29:57.000000 pulumi_nomad-2.3.0a1713561631/pulumi_nomad/quote_specification.py
--rw-r--r--   0 runner    (1001) docker     (127)    14266 2024-04-19 21:29:57.000000 pulumi_nomad-2.3.0a1713561631/pulumi_nomad/scheduler_config.py
--rw-r--r--   0 runner    (1001) docker     (127)    17214 2024-04-19 21:29:57.000000 pulumi_nomad-2.3.0a1713561631/pulumi_nomad/sentinel_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)    11841 2024-04-19 21:29:57.000000 pulumi_nomad-2.3.0a1713561631/pulumi_nomad/variable.py
--rw-r--r--   0 runner    (1001) docker     (127)    57678 2024-04-19 21:29:57.000000 pulumi_nomad-2.3.0a1713561631/pulumi_nomad/volume.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:30:04.172101 pulumi_nomad-2.3.0a1713561631/pulumi_nomad.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4727 2024-04-19 21:30:04.000000 pulumi_nomad-2.3.0a1713561631/pulumi_nomad.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1675 2024-04-19 21:30:04.000000 pulumi_nomad-2.3.0a1713561631/pulumi_nomad.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 21:30:04.000000 pulumi_nomad-2.3.0a1713561631/pulumi_nomad.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-19 21:30:04.000000 pulumi_nomad-2.3.0a1713561631/pulumi_nomad.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-19 21:30:04.000000 pulumi_nomad-2.3.0a1713561631/pulumi_nomad.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      674 2024-04-19 21:29:57.000000 pulumi_nomad-2.3.0a1713561631/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 21:30:04.172101 pulumi_nomad-2.3.0a1713561631/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:47:43.238381 pulumi_nomad-2.3.0a1713899842/
+-rw-r--r--   0 runner    (1001) docker     (127)     4727 2024-04-23 19:47:43.238381 pulumi_nomad-2.3.0a1713899842/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4279 2024-04-23 19:47:37.000000 pulumi_nomad-2.3.0a1713899842/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:47:43.238381 pulumi_nomad-2.3.0a1713899842/pulumi_nomad/
+-rw-r--r--   0 runner    (1001) docker     (127)     4332 2024-04-23 19:47:37.000000 pulumi_nomad-2.3.0a1713899842/pulumi_nomad/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    68669 2024-04-23 19:47:37.000000 pulumi_nomad-2.3.0a1713899842/pulumi_nomad/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-04-23 19:47:37.000000 pulumi_nomad-2.3.0a1713899842/pulumi_nomad/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23774 2024-04-23 19:47:37.000000 pulumi_nomad-2.3.0a1713899842/pulumi_nomad/acl_auth_method.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16396 2024-04-23 19:47:37.000000 pulumi_nomad-2.3.0a1713899842/pulumi_nomad/acl_binding_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12176 2024-04-23 19:47:37.000000 pulumi_nomad-2.3.0a1713899842/pulumi_nomad/acl_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10526 2024-04-23 19:47:37.000000 pulumi_nomad-2.3.0a1713899842/pulumi_nomad/acl_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28727 2024-04-23 19:47:37.000000 pulumi_nomad-2.3.0a1713899842/pulumi_nomad/acl_token.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:47:43.238381 pulumi_nomad-2.3.0a1713899842/pulumi_nomad/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-23 19:47:37.000000 pulumi_nomad-2.3.0a1713899842/pulumi_nomad/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1865 2024-04-23 19:47:37.000000 pulumi_nomad-2.3.0a1713899842/pulumi_nomad/config/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-04-23 19:47:37.000000 pulumi_nomad-2.3.0a1713899842/pulumi_nomad/config/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3432 2024-04-23 19:47:37.000000 pulumi_nomad-2.3.0a1713899842/pulumi_nomad/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48598 2024-04-23 19:47:37.000000 pulumi_nomad-2.3.0a1713899842/pulumi_nomad/csi_volume.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50513 2024-04-23 19:47:37.000000 pulumi_nomad-2.3.0a1713899842/pulumi_nomad/csi_volume_registration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50425 2024-04-23 19:47:37.000000 pulumi_nomad-2.3.0a1713899842/pulumi_nomad/external_volume.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3550 2024-04-23 19:47:37.000000 pulumi_nomad-2.3.0a1713899842/pulumi_nomad/get_acl_policies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3800 2024-04-23 19:47:37.000000 pulumi_nomad-2.3.0a1713899842/pulumi_nomad/get_acl_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3873 2024-04-23 19:47:37.000000 pulumi_nomad-2.3.0a1713899842/pulumi_nomad/get_acl_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3446 2024-04-23 19:47:37.000000 pulumi_nomad-2.3.0a1713899842/pulumi_nomad/get_acl_roles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7630 2024-04-23 19:47:37.000000 pulumi_nomad-2.3.0a1713899842/pulumi_nomad/get_acl_token.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3419 2024-04-23 19:47:37.000000 pulumi_nomad-2.3.0a1713899842/pulumi_nomad/get_acl_tokens.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5350 2024-04-23 19:47:37.000000 pulumi_nomad-2.3.0a1713899842/pulumi_nomad/get_allocations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4647 2024-04-23 19:47:37.000000 pulumi_nomad-2.3.0a1713899842/pulumi_nomad/get_datacenters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2715 2024-04-23 19:47:37.000000 pulumi_nomad-2.3.0a1713899842/pulumi_nomad/get_deployments.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13404 2024-04-23 19:47:37.000000 pulumi_nomad-2.3.0a1713899842/pulumi_nomad/get_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4001 2024-04-23 19:47:37.000000 pulumi_nomad-2.3.0a1713899842/pulumi_nomad/get_job_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5344 2024-04-23 19:47:37.000000 pulumi_nomad-2.3.0a1713899842/pulumi_nomad/get_namespace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3561 2024-04-23 19:47:37.000000 pulumi_nomad-2.3.0a1713899842/pulumi_nomad/get_namespaces.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4427 2024-04-23 19:47:37.000000 pulumi_nomad-2.3.0a1713899842/pulumi_nomad/get_node_pool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4370 2024-04-23 19:47:37.000000 pulumi_nomad-2.3.0a1713899842/pulumi_nomad/get_node_pools.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10732 2024-04-23 19:47:37.000000 pulumi_nomad-2.3.0a1713899842/pulumi_nomad/get_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3109 2024-04-23 19:47:37.000000 pulumi_nomad-2.3.0a1713899842/pulumi_nomad/get_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3286 2024-04-23 19:47:37.000000 pulumi_nomad-2.3.0a1713899842/pulumi_nomad/get_regions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4658 2024-04-23 19:47:37.000000 pulumi_nomad-2.3.0a1713899842/pulumi_nomad/get_scaling_policies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5116 2024-04-23 19:47:37.000000 pulumi_nomad-2.3.0a1713899842/pulumi_nomad/get_scaling_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4546 2024-04-23 19:47:37.000000 pulumi_nomad-2.3.0a1713899842/pulumi_nomad/get_scheduler_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4113 2024-04-23 19:47:37.000000 pulumi_nomad-2.3.0a1713899842/pulumi_nomad/get_variable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5420 2024-04-23 19:47:37.000000 pulumi_nomad-2.3.0a1713899842/pulumi_nomad/get_volumes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51951 2024-04-23 19:47:37.000000 pulumi_nomad-2.3.0a1713899842/pulumi_nomad/job.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20505 2024-04-23 19:47:37.000000 pulumi_nomad-2.3.0a1713899842/pulumi_nomad/namespace.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13126 2024-04-23 19:47:37.000000 pulumi_nomad-2.3.0a1713899842/pulumi_nomad/node_pool.py
+-rw-r--r--   0 runner    (1001) docker     (127)    95392 2024-04-23 19:47:37.000000 pulumi_nomad-2.3.0a1713899842/pulumi_nomad/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21549 2024-04-23 19:47:37.000000 pulumi_nomad-2.3.0a1713899842/pulumi_nomad/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-23 19:47:37.000000 pulumi_nomad-2.3.0a1713899842/pulumi_nomad/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 19:47:37.000000 pulumi_nomad-2.3.0a1713899842/pulumi_nomad/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    12113 2024-04-23 19:47:37.000000 pulumi_nomad-2.3.0a1713899842/pulumi_nomad/quote_specification.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14110 2024-04-23 19:47:37.000000 pulumi_nomad-2.3.0a1713899842/pulumi_nomad/scheduler_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17058 2024-04-23 19:47:37.000000 pulumi_nomad-2.3.0a1713899842/pulumi_nomad/sentinel_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11529 2024-04-23 19:47:37.000000 pulumi_nomad-2.3.0a1713899842/pulumi_nomad/variable.py
+-rw-r--r--   0 runner    (1001) docker     (127)    55456 2024-04-23 19:47:37.000000 pulumi_nomad-2.3.0a1713899842/pulumi_nomad/volume.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:47:43.238381 pulumi_nomad-2.3.0a1713899842/pulumi_nomad.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4727 2024-04-23 19:47:43.000000 pulumi_nomad-2.3.0a1713899842/pulumi_nomad.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1675 2024-04-23 19:47:43.000000 pulumi_nomad-2.3.0a1713899842/pulumi_nomad.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 19:47:43.000000 pulumi_nomad-2.3.0a1713899842/pulumi_nomad.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-23 19:47:43.000000 pulumi_nomad-2.3.0a1713899842/pulumi_nomad.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-23 19:47:43.000000 pulumi_nomad-2.3.0a1713899842/pulumi_nomad.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      674 2024-04-23 19:47:37.000000 pulumi_nomad-2.3.0a1713899842/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 19:47:43.238381 pulumi_nomad-2.3.0a1713899842/setup.cfg
```

### Comparing `pulumi_nomad-2.3.0a1713561631/PKG-INFO` & `pulumi_nomad-2.3.0a1713899842/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_nomad
-Version: 2.3.0a1713561631
+Version: 2.3.0a1713899842
 Summary: A Pulumi package for creating and managing nomad cloud resources.
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.io
 Project-URL: Repository, https://github.com/pulumi/pulumi-nomad
 Keywords: pulumi,nomad
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_nomad-2.3.0a1713561631/README.md` & `pulumi_nomad-2.3.0a1713899842/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_nomad-2.3.0a1713561631/pulumi_nomad/__init__.py` & `pulumi_nomad-2.3.0a1713899842/pulumi_nomad/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_nomad-2.3.0a1713561631/pulumi_nomad/_inputs.py` & `pulumi_nomad-2.3.0a1713899842/pulumi_nomad/_inputs.py`

 * *Files 4% similar despite different names*

```diff
@@ -262,78 +262,68 @@
 class AclPolicyJobAclArgs:
     def __init__(__self__, *,
                  job_id: pulumi.Input[str],
                  group: Optional[pulumi.Input[str]] = None,
                  namespace: Optional[pulumi.Input[str]] = None,
                  task: Optional[pulumi.Input[str]] = None):
         """
-        :param pulumi.Input[str] job_id: `(string: <optional>` - The job to attach the policy. Required if
-               `group` is set.
-        :param pulumi.Input[str] group: `(string: <optional>` - The group to attach the policy. Required if
-               `task` is set.
-        :param pulumi.Input[str] namespace: `(string: "default")` - The namespace to attach the policy.
-               Required if `job_id` is set.
-        :param pulumi.Input[str] task: `(string: <optional>` - The task to attach the policy.
-               
-               [nomad_docs_wi]: https://www.nomadproject.io/docs/concepts/workload-identity#workload-associated-acl-policies
+        :param pulumi.Input[str] job_id: Job
+        :param pulumi.Input[str] group: Group
+        :param pulumi.Input[str] namespace: Namespace
+        :param pulumi.Input[str] task: Task
         """
         pulumi.set(__self__, "job_id", job_id)
         if group is not None:
             pulumi.set(__self__, "group", group)
         if namespace is not None:
             pulumi.set(__self__, "namespace", namespace)
         if task is not None:
             pulumi.set(__self__, "task", task)
 
     @property
     @pulumi.getter(name="jobId")
     def job_id(self) -> pulumi.Input[str]:
         """
-        `(string: <optional>` - The job to attach the policy. Required if
-        `group` is set.
+        Job
         """
         return pulumi.get(self, "job_id")
 
     @job_id.setter
     def job_id(self, value: pulumi.Input[str]):
         pulumi.set(self, "job_id", value)
 
     @property
     @pulumi.getter
     def group(self) -> Optional[pulumi.Input[str]]:
         """
-        `(string: <optional>` - The group to attach the policy. Required if
-        `task` is set.
+        Group
         """
         return pulumi.get(self, "group")
 
     @group.setter
     def group(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "group", value)
 
     @property
     @pulumi.getter
     def namespace(self) -> Optional[pulumi.Input[str]]:
         """
-        `(string: "default")` - The namespace to attach the policy.
-        Required if `job_id` is set.
+        Namespace
         """
         return pulumi.get(self, "namespace")
 
     @namespace.setter
     def namespace(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "namespace", value)
 
     @property
     @pulumi.getter
     def task(self) -> Optional[pulumi.Input[str]]:
         """
-        `(string: <optional>` - The task to attach the policy.
-
-        [nomad_docs_wi]: https://www.nomadproject.io/docs/concepts/workload-identity#workload-associated-acl-policies
+        Task
         """
         return pulumi.get(self, "task")
 
     @task.setter
     def task(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "task", value)
 
@@ -578,32 +568,20 @@
         pulumi.set(self, "mount_flags", value)
 
 
 @pulumi.input_type
 class CsiVolumeRegistrationTopologyArgs:
     def __init__(__self__, *,
                  segments: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None):
-        """
-        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] segments: `(map[string]string)` - Define the attributes for the topology request.
-               
-               In addition to the above arguments, the following attributes are exported and
-               can be referenced:
-        """
         if segments is not None:
             pulumi.set(__self__, "segments", segments)
 
     @property
     @pulumi.getter
     def segments(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
-        """
-        `(map[string]string)` - Define the attributes for the topology request.
-
-        In addition to the above arguments, the following attributes are exported and
-        can be referenced:
-        """
         return pulumi.get(self, "segments")
 
     @segments.setter
     def segments(self, value: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]):
         pulumi.set(self, "segments", value)
 
 
@@ -631,81 +609,63 @@
 
 
 @pulumi.input_type
 class CsiVolumeRegistrationTopologyRequestRequiredArgs:
     def __init__(__self__, *,
                  topologies: pulumi.Input[Sequence[pulumi.Input['CsiVolumeRegistrationTopologyRequestRequiredTopologyArgs']]]):
         """
-        :param pulumi.Input[Sequence[pulumi.Input['CsiVolumeRegistrationTopologyRequestRequiredTopologyArgs']]] topologies: `(List of segments: <required>)` - Defines the location for the volume.
+        :param pulumi.Input[Sequence[pulumi.Input['CsiVolumeRegistrationTopologyRequestRequiredTopologyArgs']]] topologies: Defines the location for the volume.
         """
         pulumi.set(__self__, "topologies", topologies)
 
     @property
     @pulumi.getter
     def topologies(self) -> pulumi.Input[Sequence[pulumi.Input['CsiVolumeRegistrationTopologyRequestRequiredTopologyArgs']]]:
         """
-        `(List of segments: <required>)` - Defines the location for the volume.
+        Defines the location for the volume.
         """
         return pulumi.get(self, "topologies")
 
     @topologies.setter
     def topologies(self, value: pulumi.Input[Sequence[pulumi.Input['CsiVolumeRegistrationTopologyRequestRequiredTopologyArgs']]]):
         pulumi.set(self, "topologies", value)
 
 
 @pulumi.input_type
 class CsiVolumeRegistrationTopologyRequestRequiredTopologyArgs:
     def __init__(__self__, *,
                  segments: pulumi.Input[Mapping[str, pulumi.Input[str]]]):
         """
-        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] segments: `(map[string]string)` - Define the attributes for the topology request.
-               
-               In addition to the above arguments, the following attributes are exported and
-               can be referenced:
+        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] segments: Define attributes for the topology request.
         """
         pulumi.set(__self__, "segments", segments)
 
     @property
     @pulumi.getter
     def segments(self) -> pulumi.Input[Mapping[str, pulumi.Input[str]]]:
         """
-        `(map[string]string)` - Define the attributes for the topology request.
-
-        In addition to the above arguments, the following attributes are exported and
-        can be referenced:
+        Define attributes for the topology request.
         """
         return pulumi.get(self, "segments")
 
     @segments.setter
     def segments(self, value: pulumi.Input[Mapping[str, pulumi.Input[str]]]):
         pulumi.set(self, "segments", value)
 
 
 @pulumi.input_type
 class CsiVolumeTopologyArgs:
     def __init__(__self__, *,
                  segments: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None):
-        """
-        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] segments: `(map[string]string)` - Define the attributes for the topology request.
-               
-               In addition to the above arguments, the following attributes are exported and
-               can be referenced:
-        """
         if segments is not None:
             pulumi.set(__self__, "segments", segments)
 
     @property
     @pulumi.getter
     def segments(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
-        """
-        `(map[string]string)` - Define the attributes for the topology request.
-
-        In addition to the above arguments, the following attributes are exported and
-        can be referenced:
-        """
         return pulumi.get(self, "segments")
 
     @segments.setter
     def segments(self, value: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]):
         pulumi.set(self, "segments", value)
 
 
@@ -749,101 +709,89 @@
 
 
 @pulumi.input_type
 class CsiVolumeTopologyRequestPreferredArgs:
     def __init__(__self__, *,
                  topologies: pulumi.Input[Sequence[pulumi.Input['CsiVolumeTopologyRequestPreferredTopologyArgs']]]):
         """
-        :param pulumi.Input[Sequence[pulumi.Input['CsiVolumeTopologyRequestPreferredTopologyArgs']]] topologies: `(List of segments: <required>)` - Defines the location for the volume.
+        :param pulumi.Input[Sequence[pulumi.Input['CsiVolumeTopologyRequestPreferredTopologyArgs']]] topologies: Defines the location for the volume.
         """
         pulumi.set(__self__, "topologies", topologies)
 
     @property
     @pulumi.getter
     def topologies(self) -> pulumi.Input[Sequence[pulumi.Input['CsiVolumeTopologyRequestPreferredTopologyArgs']]]:
         """
-        `(List of segments: <required>)` - Defines the location for the volume.
+        Defines the location for the volume.
         """
         return pulumi.get(self, "topologies")
 
     @topologies.setter
     def topologies(self, value: pulumi.Input[Sequence[pulumi.Input['CsiVolumeTopologyRequestPreferredTopologyArgs']]]):
         pulumi.set(self, "topologies", value)
 
 
 @pulumi.input_type
 class CsiVolumeTopologyRequestPreferredTopologyArgs:
     def __init__(__self__, *,
                  segments: pulumi.Input[Mapping[str, pulumi.Input[str]]]):
         """
-        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] segments: `(map[string]string)` - Define the attributes for the topology request.
-               
-               In addition to the above arguments, the following attributes are exported and
-               can be referenced:
+        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] segments: Define the attributes for the topology request.
         """
         pulumi.set(__self__, "segments", segments)
 
     @property
     @pulumi.getter
     def segments(self) -> pulumi.Input[Mapping[str, pulumi.Input[str]]]:
         """
-        `(map[string]string)` - Define the attributes for the topology request.
-
-        In addition to the above arguments, the following attributes are exported and
-        can be referenced:
+        Define the attributes for the topology request.
         """
         return pulumi.get(self, "segments")
 
     @segments.setter
     def segments(self, value: pulumi.Input[Mapping[str, pulumi.Input[str]]]):
         pulumi.set(self, "segments", value)
 
 
 @pulumi.input_type
 class CsiVolumeTopologyRequestRequiredArgs:
     def __init__(__self__, *,
                  topologies: pulumi.Input[Sequence[pulumi.Input['CsiVolumeTopologyRequestRequiredTopologyArgs']]]):
         """
-        :param pulumi.Input[Sequence[pulumi.Input['CsiVolumeTopologyRequestRequiredTopologyArgs']]] topologies: `(List of segments: <required>)` - Defines the location for the volume.
+        :param pulumi.Input[Sequence[pulumi.Input['CsiVolumeTopologyRequestRequiredTopologyArgs']]] topologies: Defines the location for the volume.
         """
         pulumi.set(__self__, "topologies", topologies)
 
     @property
     @pulumi.getter
     def topologies(self) -> pulumi.Input[Sequence[pulumi.Input['CsiVolumeTopologyRequestRequiredTopologyArgs']]]:
         """
-        `(List of segments: <required>)` - Defines the location for the volume.
+        Defines the location for the volume.
         """
         return pulumi.get(self, "topologies")
 
     @topologies.setter
     def topologies(self, value: pulumi.Input[Sequence[pulumi.Input['CsiVolumeTopologyRequestRequiredTopologyArgs']]]):
         pulumi.set(self, "topologies", value)
 
 
 @pulumi.input_type
 class CsiVolumeTopologyRequestRequiredTopologyArgs:
     def __init__(__self__, *,
                  segments: pulumi.Input[Mapping[str, pulumi.Input[str]]]):
         """
-        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] segments: `(map[string]string)` - Define the attributes for the topology request.
-               
-               In addition to the above arguments, the following attributes are exported and
-               can be referenced:
+        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] segments: Define the attributes for the topology request.
         """
         pulumi.set(__self__, "segments", segments)
 
     @property
     @pulumi.getter
     def segments(self) -> pulumi.Input[Mapping[str, pulumi.Input[str]]]:
         """
-        `(map[string]string)` - Define the attributes for the topology request.
-
-        In addition to the above arguments, the following attributes are exported and
-        can be referenced:
+        Define the attributes for the topology request.
         """
         return pulumi.get(self, "segments")
 
     @segments.setter
     def segments(self, value: pulumi.Input[Mapping[str, pulumi.Input[str]]]):
         pulumi.set(self, "segments", value)
 
@@ -938,32 +886,20 @@
         pulumi.set(self, "mount_flags", value)
 
 
 @pulumi.input_type
 class ExternalVolumeTopologyArgs:
     def __init__(__self__, *,
                  segments: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None):
-        """
-        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] segments: `(map[string]string)` - Define the attributes for the topology request.
-               
-               In addition to the above arguments, the following attributes are exported and
-               can be referenced:
-        """
         if segments is not None:
             pulumi.set(__self__, "segments", segments)
 
     @property
     @pulumi.getter
     def segments(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
-        """
-        `(map[string]string)` - Define the attributes for the topology request.
-
-        In addition to the above arguments, the following attributes are exported and
-        can be referenced:
-        """
         return pulumi.get(self, "segments")
 
     @segments.setter
     def segments(self, value: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]):
         pulumi.set(self, "segments", value)
 
 
@@ -1007,101 +943,89 @@
 
 
 @pulumi.input_type
 class ExternalVolumeTopologyRequestPreferredArgs:
     def __init__(__self__, *,
                  topologies: pulumi.Input[Sequence[pulumi.Input['ExternalVolumeTopologyRequestPreferredTopologyArgs']]]):
         """
-        :param pulumi.Input[Sequence[pulumi.Input['ExternalVolumeTopologyRequestPreferredTopologyArgs']]] topologies: `(List of segments: <required>)` - Defines the location for the volume.
+        :param pulumi.Input[Sequence[pulumi.Input['ExternalVolumeTopologyRequestPreferredTopologyArgs']]] topologies: Defines the location for the volume.
         """
         pulumi.set(__self__, "topologies", topologies)
 
     @property
     @pulumi.getter
     def topologies(self) -> pulumi.Input[Sequence[pulumi.Input['ExternalVolumeTopologyRequestPreferredTopologyArgs']]]:
         """
-        `(List of segments: <required>)` - Defines the location for the volume.
+        Defines the location for the volume.
         """
         return pulumi.get(self, "topologies")
 
     @topologies.setter
     def topologies(self, value: pulumi.Input[Sequence[pulumi.Input['ExternalVolumeTopologyRequestPreferredTopologyArgs']]]):
         pulumi.set(self, "topologies", value)
 
 
 @pulumi.input_type
 class ExternalVolumeTopologyRequestPreferredTopologyArgs:
     def __init__(__self__, *,
                  segments: pulumi.Input[Mapping[str, pulumi.Input[str]]]):
         """
-        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] segments: `(map[string]string)` - Define the attributes for the topology request.
-               
-               In addition to the above arguments, the following attributes are exported and
-               can be referenced:
+        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] segments: Define the attributes for the topology request.
         """
         pulumi.set(__self__, "segments", segments)
 
     @property
     @pulumi.getter
     def segments(self) -> pulumi.Input[Mapping[str, pulumi.Input[str]]]:
         """
-        `(map[string]string)` - Define the attributes for the topology request.
-
-        In addition to the above arguments, the following attributes are exported and
-        can be referenced:
+        Define the attributes for the topology request.
         """
         return pulumi.get(self, "segments")
 
     @segments.setter
     def segments(self, value: pulumi.Input[Mapping[str, pulumi.Input[str]]]):
         pulumi.set(self, "segments", value)
 
 
 @pulumi.input_type
 class ExternalVolumeTopologyRequestRequiredArgs:
     def __init__(__self__, *,
                  topologies: pulumi.Input[Sequence[pulumi.Input['ExternalVolumeTopologyRequestRequiredTopologyArgs']]]):
         """
-        :param pulumi.Input[Sequence[pulumi.Input['ExternalVolumeTopologyRequestRequiredTopologyArgs']]] topologies: `(List of segments: <required>)` - Defines the location for the volume.
+        :param pulumi.Input[Sequence[pulumi.Input['ExternalVolumeTopologyRequestRequiredTopologyArgs']]] topologies: Defines the location for the volume.
         """
         pulumi.set(__self__, "topologies", topologies)
 
     @property
     @pulumi.getter
     def topologies(self) -> pulumi.Input[Sequence[pulumi.Input['ExternalVolumeTopologyRequestRequiredTopologyArgs']]]:
         """
-        `(List of segments: <required>)` - Defines the location for the volume.
+        Defines the location for the volume.
         """
         return pulumi.get(self, "topologies")
 
     @topologies.setter
     def topologies(self, value: pulumi.Input[Sequence[pulumi.Input['ExternalVolumeTopologyRequestRequiredTopologyArgs']]]):
         pulumi.set(self, "topologies", value)
 
 
 @pulumi.input_type
 class ExternalVolumeTopologyRequestRequiredTopologyArgs:
     def __init__(__self__, *,
                  segments: pulumi.Input[Mapping[str, pulumi.Input[str]]]):
         """
-        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] segments: `(map[string]string)` - Define the attributes for the topology request.
-               
-               In addition to the above arguments, the following attributes are exported and
-               can be referenced:
+        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] segments: Define the attributes for the topology request.
         """
         pulumi.set(__self__, "segments", segments)
 
     @property
     @pulumi.getter
     def segments(self) -> pulumi.Input[Mapping[str, pulumi.Input[str]]]:
         """
-        `(map[string]string)` - Define the attributes for the topology request.
-
-        In addition to the above arguments, the following attributes are exported and
-        can be referenced:
+        Define the attributes for the topology request.
         """
         return pulumi.get(self, "segments")
 
     @segments.setter
     def segments(self, value: pulumi.Input[Mapping[str, pulumi.Input[str]]]):
         pulumi.set(self, "segments", value)
 
@@ -1747,32 +1671,20 @@
         pulumi.set(self, "mount_flags", value)
 
 
 @pulumi.input_type
 class VolumeTopologyArgs:
     def __init__(__self__, *,
                  segments: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None):
-        """
-        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] segments: `(map[string]string)` - Define the attributes for the topology request.
-               
-               In addition to the above arguments, the following attributes are exported and
-               can be referenced:
-        """
         if segments is not None:
             pulumi.set(__self__, "segments", segments)
 
     @property
     @pulumi.getter
     def segments(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
-        """
-        `(map[string]string)` - Define the attributes for the topology request.
-
-        In addition to the above arguments, the following attributes are exported and
-        can be referenced:
-        """
         return pulumi.get(self, "segments")
 
     @segments.setter
     def segments(self, value: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]):
         pulumi.set(self, "segments", value)
 
 
@@ -1800,51 +1712,45 @@
 
 
 @pulumi.input_type
 class VolumeTopologyRequestRequiredArgs:
     def __init__(__self__, *,
                  topologies: pulumi.Input[Sequence[pulumi.Input['VolumeTopologyRequestRequiredTopologyArgs']]]):
         """
-        :param pulumi.Input[Sequence[pulumi.Input['VolumeTopologyRequestRequiredTopologyArgs']]] topologies: `(List of segments: <required>)` - Defines the location for the volume.
+        :param pulumi.Input[Sequence[pulumi.Input['VolumeTopologyRequestRequiredTopologyArgs']]] topologies: Defines the location for the volume.
         """
         pulumi.set(__self__, "topologies", topologies)
 
     @property
     @pulumi.getter
     def topologies(self) -> pulumi.Input[Sequence[pulumi.Input['VolumeTopologyRequestRequiredTopologyArgs']]]:
         """
-        `(List of segments: <required>)` - Defines the location for the volume.
+        Defines the location for the volume.
         """
         return pulumi.get(self, "topologies")
 
     @topologies.setter
     def topologies(self, value: pulumi.Input[Sequence[pulumi.Input['VolumeTopologyRequestRequiredTopologyArgs']]]):
         pulumi.set(self, "topologies", value)
 
 
 @pulumi.input_type
 class VolumeTopologyRequestRequiredTopologyArgs:
     def __init__(__self__, *,
                  segments: pulumi.Input[Mapping[str, pulumi.Input[str]]]):
         """
-        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] segments: `(map[string]string)` - Define the attributes for the topology request.
-               
-               In addition to the above arguments, the following attributes are exported and
-               can be referenced:
+        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] segments: Define attributes for the topology request.
         """
         pulumi.set(__self__, "segments", segments)
 
     @property
     @pulumi.getter
     def segments(self) -> pulumi.Input[Mapping[str, pulumi.Input[str]]]:
         """
-        `(map[string]string)` - Define the attributes for the topology request.
-
-        In addition to the above arguments, the following attributes are exported and
-        can be referenced:
+        Define attributes for the topology request.
         """
         return pulumi.get(self, "segments")
 
     @segments.setter
     def segments(self, value: pulumi.Input[Mapping[str, pulumi.Input[str]]]):
         pulumi.set(self, "segments", value)
```

### Comparing `pulumi_nomad-2.3.0a1713561631/pulumi_nomad/_utilities.py` & `pulumi_nomad-2.3.0a1713899842/pulumi_nomad/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_nomad-2.3.0a1713561631/pulumi_nomad/acl_auth_method.py` & `pulumi_nomad-2.3.0a1713899842/pulumi_nomad/acl_auth_method.py`

 * *Files 2% similar despite different names*

```diff
@@ -297,15 +297,14 @@
         """
         Manages an ACL Auth Method in Nomad.
 
         ## Example Usage
 
         Creating an ALC Auth Method:
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_nomad as nomad
 
         my_nomad_acl_auth_method = nomad.AclAuthMethod("my_nomad_acl_auth_method",
             name="my-nomad-acl-auth-method",
             type="OIDC",
@@ -323,15 +322,14 @@
                     "http://localhost:4646/ui/settings/tokens",
                 ],
                 list_claim_mappings={
                     "http://nomad.internal/roles": "roles",
                 },
             ))
         ```
-        <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[pulumi.InputType['AclAuthMethodConfigArgs']] config: `(block: <required>)` - Configuration specific to the auth method
                provider.
         :param pulumi.Input[bool] default: `(bool: false)` - Defines whether this ACL Auth Method is to be set
                as default.
@@ -356,15 +354,14 @@
         """
         Manages an ACL Auth Method in Nomad.
 
         ## Example Usage
 
         Creating an ALC Auth Method:
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_nomad as nomad
 
         my_nomad_acl_auth_method = nomad.AclAuthMethod("my_nomad_acl_auth_method",
             name="my-nomad-acl-auth-method",
             type="OIDC",
@@ -382,15 +379,14 @@
                     "http://localhost:4646/ui/settings/tokens",
                 ],
                 list_claim_mappings={
                     "http://nomad.internal/roles": "roles",
                 },
             ))
         ```
-        <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param AclAuthMethodArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
```

### Comparing `pulumi_nomad-2.3.0a1713561631/pulumi_nomad/acl_binding_rule.py` & `pulumi_nomad-2.3.0a1713899842/pulumi_nomad/acl_binding_rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_nomad-2.3.0a1713561631/pulumi_nomad/acl_policy.py` & `pulumi_nomad-2.3.0a1713899842/pulumi_nomad/acl_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_nomad-2.3.0a1713561631/pulumi_nomad/acl_role.py` & `pulumi_nomad-2.3.0a1713899842/pulumi_nomad/acl_role.py`

 * *Files identical despite different names*

### Comparing `pulumi_nomad-2.3.0a1713561631/pulumi_nomad/acl_token.py` & `pulumi_nomad-2.3.0a1713899842/pulumi_nomad/acl_token.py`

 * *Files 3% similar despite different names*

```diff
@@ -347,73 +347,65 @@
                  type: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         ## Example Usage
 
         Creating a token with limited policies:
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_nomad as nomad
 
         dakota = nomad.AclToken("dakota",
             name="Dakota",
             type="client",
             policies=[
                 "dev",
                 "qa",
             ])
         ```
-        <!--End PulumiCodeChooser -->
 
         Creating a global token that will be replicated to all regions:
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_nomad as nomad
 
         dakota = nomad.AclToken("dakota",
             name="Dakota",
             type="client",
             policies=[
                 "dev",
                 "qa",
             ],
             global_=True)
         ```
-        <!--End PulumiCodeChooser -->
 
         Creating a token with full access to the cluster:
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_nomad as nomad
 
         iman = nomad.AclToken("iman",
             name="Iman",
             type="management")
         ```
-        <!--End PulumiCodeChooser -->
 
         Accessing the token:
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_nomad as nomad
 
         token = nomad.AclToken("token",
             type="client",
             policies=["dev"])
         pulumi.export("nomadToken", token.secret_id)
         ```
-        <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] expiration_ttl: `(string: "")` - Provides a TTL for the token in the form of
                a time duration such as `"5m"` or `"1h"`.
                
                In addition to the above arguments, the following attributes are exported and
@@ -438,73 +430,65 @@
                  args: AclTokenArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         ## Example Usage
 
         Creating a token with limited policies:
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_nomad as nomad
 
         dakota = nomad.AclToken("dakota",
             name="Dakota",
             type="client",
             policies=[
                 "dev",
                 "qa",
             ])
         ```
-        <!--End PulumiCodeChooser -->
 
         Creating a global token that will be replicated to all regions:
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_nomad as nomad
 
         dakota = nomad.AclToken("dakota",
             name="Dakota",
             type="client",
             policies=[
                 "dev",
                 "qa",
             ],
             global_=True)
         ```
-        <!--End PulumiCodeChooser -->
 
         Creating a token with full access to the cluster:
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_nomad as nomad
 
         iman = nomad.AclToken("iman",
             name="Iman",
             type="management")
         ```
-        <!--End PulumiCodeChooser -->
 
         Accessing the token:
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_nomad as nomad
 
         token = nomad.AclToken("token",
             type="client",
             policies=["dev"])
         pulumi.export("nomadToken", token.secret_id)
         ```
-        <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param AclTokenArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
```

### Comparing `pulumi_nomad-2.3.0a1713561631/pulumi_nomad/config/__init__.pyi` & `pulumi_nomad-2.3.0a1713899842/pulumi_nomad/config/__init__.pyi`

 * *Files identical despite different names*

### Comparing `pulumi_nomad-2.3.0a1713561631/pulumi_nomad/config/outputs.py` & `pulumi_nomad-2.3.0a1713899842/pulumi_nomad/config/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_nomad-2.3.0a1713561631/pulumi_nomad/config/vars.py` & `pulumi_nomad-2.3.0a1713899842/pulumi_nomad/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_nomad-2.3.0a1713561631/pulumi_nomad/csi_volume.py` & `pulumi_nomad-2.3.0a1713899842/pulumi_nomad/csi_volume_registration.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,83 +7,87 @@
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 from . import outputs
 from ._inputs import *
 
-__all__ = ['CsiVolumeArgs', 'CsiVolume']
+__all__ = ['CsiVolumeRegistrationArgs', 'CsiVolumeRegistration']
 
 @pulumi.input_type
-class CsiVolumeArgs:
+class CsiVolumeRegistrationArgs:
     def __init__(__self__, *,
-                 capabilities: pulumi.Input[Sequence[pulumi.Input['CsiVolumeCapabilityArgs']]],
+                 external_id: pulumi.Input[str],
                  plugin_id: pulumi.Input[str],
                  volume_id: pulumi.Input[str],
+                 capabilities: Optional[pulumi.Input[Sequence[pulumi.Input['CsiVolumeRegistrationCapabilityArgs']]]] = None,
                  capacity_max: Optional[pulumi.Input[str]] = None,
                  capacity_min: Optional[pulumi.Input[str]] = None,
-                 clone_id: Optional[pulumi.Input[str]] = None,
-                 mount_options: Optional[pulumi.Input['CsiVolumeMountOptionsArgs']] = None,
+                 context: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
+                 deregister_on_destroy: Optional[pulumi.Input[bool]] = None,
+                 mount_options: Optional[pulumi.Input['CsiVolumeRegistrationMountOptionsArgs']] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  namespace: Optional[pulumi.Input[str]] = None,
                  parameters: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  secrets: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
-                 snapshot_id: Optional[pulumi.Input[str]] = None,
-                 topology_request: Optional[pulumi.Input['CsiVolumeTopologyRequestArgs']] = None):
+                 topology_request: Optional[pulumi.Input['CsiVolumeRegistrationTopologyRequestArgs']] = None):
         """
-        The set of arguments for constructing a CsiVolume resource.
-        :param pulumi.Input[Sequence[pulumi.Input['CsiVolumeCapabilityArgs']]] capabilities: `(``Capability``: <required>)` - Options for validating the capability of a volume.
+        The set of arguments for constructing a CsiVolumeRegistration resource.
+        :param pulumi.Input[str] external_id: `(string: <required>)` - The ID of the physical volume from the storage provider.
         :param pulumi.Input[str] plugin_id: `(string: <required>)` - The ID of the Nomad plugin for registering this volume.
         :param pulumi.Input[str] volume_id: `(string: <required>)` - The unique ID of the volume.
+        :param pulumi.Input[Sequence[pulumi.Input['CsiVolumeRegistrationCapabilityArgs']]] capabilities: `(``Capability``: <required>)` - Options for validating the capability of a volume.
         :param pulumi.Input[str] capacity_max: `(string: <optional>)` - Option to signal a maximum volume size. This may not be supported by all storage providers.
         :param pulumi.Input[str] capacity_min: `(string: <optional>)` - Option to signal a minimum volume size. This may not be supported by all storage providers.
-        :param pulumi.Input[str] clone_id: `(string: <optional>)` - The external ID of an existing volume to restore. If ommited, the volume will be created from scratch. Conflicts with `snapshot_id`.
-        :param pulumi.Input['CsiVolumeMountOptionsArgs'] mount_options: `(block: optional)` Options for mounting `block-device` volumes without a pre-formatted file system.
+        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] context: `(map[string]string: <optional>)` - An optional key-value map of strings passed directly to the CSI plugin to validate the volume.
+        :param pulumi.Input[bool] deregister_on_destroy: `(boolean: true)` - If true, the volume will be deregistered on destroy.
+        :param pulumi.Input['CsiVolumeRegistrationMountOptionsArgs'] mount_options: `(block: <optional>)` Options for mounting `block-device` volumes without a pre-formatted file system.
         :param pulumi.Input[str] name: `(string: <required>)` - The display name for the volume.
         :param pulumi.Input[str] namespace: `(string: "default")` - The namespace in which to register the volume.
-        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] parameters: `(map[string]string: optional)` An optional key-value map of strings passed directly to the CSI plugin to configure the volume.
-        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] secrets: `(map[string]string: optional)` An optional key-value map of strings used as credentials for publishing and unpublishing volumes.
-        :param pulumi.Input[str] snapshot_id: `(string: <optional>)` - The external ID of a snapshot to restore. If ommited, the volume will be created from scratch. Conflicts with `clone_id`.
-        :param pulumi.Input['CsiVolumeTopologyRequestArgs'] topology_request: `(``TopologyRequest``: <optional>)` - Specify locations (region, zone, rack, etc.) where the provisioned volume is accessible from.
+        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] parameters: `(map[string]string: <optional>)` - An optional key-value map of strings passed directly to the CSI plugin to configure the volume.
+        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] secrets: `(map[string]string: <optional>)` - An optional key-value map of strings used as credentials for publishing and unpublishing volumes.
+        :param pulumi.Input['CsiVolumeRegistrationTopologyRequestArgs'] topology_request: `(``TopologyRequest``: <optional>)` - Specify locations (region, zone, rack, etc.) where the provisioned volume is accessible from.
         """
-        pulumi.set(__self__, "capabilities", capabilities)
+        pulumi.set(__self__, "external_id", external_id)
         pulumi.set(__self__, "plugin_id", plugin_id)
         pulumi.set(__self__, "volume_id", volume_id)
+        if capabilities is not None:
+            pulumi.set(__self__, "capabilities", capabilities)
         if capacity_max is not None:
             pulumi.set(__self__, "capacity_max", capacity_max)
         if capacity_min is not None:
             pulumi.set(__self__, "capacity_min", capacity_min)
-        if clone_id is not None:
-            pulumi.set(__self__, "clone_id", clone_id)
+        if context is not None:
+            pulumi.set(__self__, "context", context)
+        if deregister_on_destroy is not None:
+            pulumi.set(__self__, "deregister_on_destroy", deregister_on_destroy)
         if mount_options is not None:
             pulumi.set(__self__, "mount_options", mount_options)
         if name is not None:
             pulumi.set(__self__, "name", name)
         if namespace is not None:
             pulumi.set(__self__, "namespace", namespace)
         if parameters is not None:
             pulumi.set(__self__, "parameters", parameters)
         if secrets is not None:
             pulumi.set(__self__, "secrets", secrets)
-        if snapshot_id is not None:
-            pulumi.set(__self__, "snapshot_id", snapshot_id)
         if topology_request is not None:
             pulumi.set(__self__, "topology_request", topology_request)
 
     @property
-    @pulumi.getter
-    def capabilities(self) -> pulumi.Input[Sequence[pulumi.Input['CsiVolumeCapabilityArgs']]]:
+    @pulumi.getter(name="externalId")
+    def external_id(self) -> pulumi.Input[str]:
         """
-        `(``Capability``: <required>)` - Options for validating the capability of a volume.
+        `(string: <required>)` - The ID of the physical volume from the storage provider.
         """
-        return pulumi.get(self, "capabilities")
+        return pulumi.get(self, "external_id")
 
-    @capabilities.setter
-    def capabilities(self, value: pulumi.Input[Sequence[pulumi.Input['CsiVolumeCapabilityArgs']]]):
-        pulumi.set(self, "capabilities", value)
+    @external_id.setter
+    def external_id(self, value: pulumi.Input[str]):
+        pulumi.set(self, "external_id", value)
 
     @property
     @pulumi.getter(name="pluginId")
     def plugin_id(self) -> pulumi.Input[str]:
         """
         `(string: <required>)` - The ID of the Nomad plugin for registering this volume.
         """
@@ -102,14 +106,26 @@
         return pulumi.get(self, "volume_id")
 
     @volume_id.setter
     def volume_id(self, value: pulumi.Input[str]):
         pulumi.set(self, "volume_id", value)
 
     @property
+    @pulumi.getter
+    def capabilities(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['CsiVolumeRegistrationCapabilityArgs']]]]:
+        """
+        `(``Capability``: <required>)` - Options for validating the capability of a volume.
+        """
+        return pulumi.get(self, "capabilities")
+
+    @capabilities.setter
+    def capabilities(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['CsiVolumeRegistrationCapabilityArgs']]]]):
+        pulumi.set(self, "capabilities", value)
+
+    @property
     @pulumi.getter(name="capacityMax")
     def capacity_max(self) -> Optional[pulumi.Input[str]]:
         """
         `(string: <optional>)` - Option to signal a maximum volume size. This may not be supported by all storage providers.
         """
         return pulumi.get(self, "capacity_max")
 
@@ -126,35 +142,47 @@
         return pulumi.get(self, "capacity_min")
 
     @capacity_min.setter
     def capacity_min(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "capacity_min", value)
 
     @property
-    @pulumi.getter(name="cloneId")
-    def clone_id(self) -> Optional[pulumi.Input[str]]:
+    @pulumi.getter
+    def context(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
+        """
+        `(map[string]string: <optional>)` - An optional key-value map of strings passed directly to the CSI plugin to validate the volume.
+        """
+        return pulumi.get(self, "context")
+
+    @context.setter
+    def context(self, value: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]):
+        pulumi.set(self, "context", value)
+
+    @property
+    @pulumi.getter(name="deregisterOnDestroy")
+    def deregister_on_destroy(self) -> Optional[pulumi.Input[bool]]:
         """
-        `(string: <optional>)` - The external ID of an existing volume to restore. If ommited, the volume will be created from scratch. Conflicts with `snapshot_id`.
+        `(boolean: true)` - If true, the volume will be deregistered on destroy.
         """
-        return pulumi.get(self, "clone_id")
+        return pulumi.get(self, "deregister_on_destroy")
 
-    @clone_id.setter
-    def clone_id(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "clone_id", value)
+    @deregister_on_destroy.setter
+    def deregister_on_destroy(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "deregister_on_destroy", value)
 
     @property
     @pulumi.getter(name="mountOptions")
-    def mount_options(self) -> Optional[pulumi.Input['CsiVolumeMountOptionsArgs']]:
+    def mount_options(self) -> Optional[pulumi.Input['CsiVolumeRegistrationMountOptionsArgs']]:
         """
-        `(block: optional)` Options for mounting `block-device` volumes without a pre-formatted file system.
+        `(block: <optional>)` Options for mounting `block-device` volumes without a pre-formatted file system.
         """
         return pulumi.get(self, "mount_options")
 
     @mount_options.setter
-    def mount_options(self, value: Optional[pulumi.Input['CsiVolumeMountOptionsArgs']]):
+    def mount_options(self, value: Optional[pulumi.Input['CsiVolumeRegistrationMountOptionsArgs']]):
         pulumi.set(self, "mount_options", value)
 
     @property
     @pulumi.getter
     def name(self) -> Optional[pulumi.Input[str]]:
         """
         `(string: <required>)` - The display name for the volume.
@@ -177,134 +205,115 @@
     def namespace(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "namespace", value)
 
     @property
     @pulumi.getter
     def parameters(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
         """
-        `(map[string]string: optional)` An optional key-value map of strings passed directly to the CSI plugin to configure the volume.
+        `(map[string]string: <optional>)` - An optional key-value map of strings passed directly to the CSI plugin to configure the volume.
         """
         return pulumi.get(self, "parameters")
 
     @parameters.setter
     def parameters(self, value: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]):
         pulumi.set(self, "parameters", value)
 
     @property
     @pulumi.getter
     def secrets(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
         """
-        `(map[string]string: optional)` An optional key-value map of strings used as credentials for publishing and unpublishing volumes.
+        `(map[string]string: <optional>)` - An optional key-value map of strings used as credentials for publishing and unpublishing volumes.
         """
         return pulumi.get(self, "secrets")
 
     @secrets.setter
     def secrets(self, value: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]):
         pulumi.set(self, "secrets", value)
 
     @property
-    @pulumi.getter(name="snapshotId")
-    def snapshot_id(self) -> Optional[pulumi.Input[str]]:
-        """
-        `(string: <optional>)` - The external ID of a snapshot to restore. If ommited, the volume will be created from scratch. Conflicts with `clone_id`.
-        """
-        return pulumi.get(self, "snapshot_id")
-
-    @snapshot_id.setter
-    def snapshot_id(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "snapshot_id", value)
-
-    @property
     @pulumi.getter(name="topologyRequest")
-    def topology_request(self) -> Optional[pulumi.Input['CsiVolumeTopologyRequestArgs']]:
+    def topology_request(self) -> Optional[pulumi.Input['CsiVolumeRegistrationTopologyRequestArgs']]:
         """
         `(``TopologyRequest``: <optional>)` - Specify locations (region, zone, rack, etc.) where the provisioned volume is accessible from.
         """
         return pulumi.get(self, "topology_request")
 
     @topology_request.setter
-    def topology_request(self, value: Optional[pulumi.Input['CsiVolumeTopologyRequestArgs']]):
+    def topology_request(self, value: Optional[pulumi.Input['CsiVolumeRegistrationTopologyRequestArgs']]):
         pulumi.set(self, "topology_request", value)
 
 
 @pulumi.input_type
-class _CsiVolumeState:
+class _CsiVolumeRegistrationState:
     def __init__(__self__, *,
-                 capabilities: Optional[pulumi.Input[Sequence[pulumi.Input['CsiVolumeCapabilityArgs']]]] = None,
+                 capabilities: Optional[pulumi.Input[Sequence[pulumi.Input['CsiVolumeRegistrationCapabilityArgs']]]] = None,
                  capacity: Optional[pulumi.Input[int]] = None,
                  capacity_max: Optional[pulumi.Input[str]] = None,
                  capacity_max_bytes: Optional[pulumi.Input[int]] = None,
                  capacity_min: Optional[pulumi.Input[str]] = None,
                  capacity_min_bytes: Optional[pulumi.Input[int]] = None,
-                 clone_id: Optional[pulumi.Input[str]] = None,
+                 context: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  controller_required: Optional[pulumi.Input[bool]] = None,
                  controllers_expected: Optional[pulumi.Input[int]] = None,
                  controllers_healthy: Optional[pulumi.Input[int]] = None,
+                 deregister_on_destroy: Optional[pulumi.Input[bool]] = None,
                  external_id: Optional[pulumi.Input[str]] = None,
-                 mount_options: Optional[pulumi.Input['CsiVolumeMountOptionsArgs']] = None,
+                 mount_options: Optional[pulumi.Input['CsiVolumeRegistrationMountOptionsArgs']] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  namespace: Optional[pulumi.Input[str]] = None,
                  nodes_expected: Optional[pulumi.Input[int]] = None,
                  nodes_healthy: Optional[pulumi.Input[int]] = None,
                  parameters: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  plugin_id: Optional[pulumi.Input[str]] = None,
                  plugin_provider: Optional[pulumi.Input[str]] = None,
                  plugin_provider_version: Optional[pulumi.Input[str]] = None,
                  schedulable: Optional[pulumi.Input[bool]] = None,
                  secrets: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
-                 snapshot_id: Optional[pulumi.Input[str]] = None,
-                 topologies: Optional[pulumi.Input[Sequence[pulumi.Input['CsiVolumeTopologyArgs']]]] = None,
-                 topology_request: Optional[pulumi.Input['CsiVolumeTopologyRequestArgs']] = None,
+                 topologies: Optional[pulumi.Input[Sequence[pulumi.Input['CsiVolumeRegistrationTopologyArgs']]]] = None,
+                 topology_request: Optional[pulumi.Input['CsiVolumeRegistrationTopologyRequestArgs']] = None,
                  volume_id: Optional[pulumi.Input[str]] = None):
         """
-        Input properties used for looking up and filtering CsiVolume resources.
-        :param pulumi.Input[Sequence[pulumi.Input['CsiVolumeCapabilityArgs']]] capabilities: `(``Capability``: <required>)` - Options for validating the capability of a volume.
+        Input properties used for looking up and filtering CsiVolumeRegistration resources.
+        :param pulumi.Input[Sequence[pulumi.Input['CsiVolumeRegistrationCapabilityArgs']]] capabilities: `(``Capability``: <required>)` - Options for validating the capability of a volume.
         :param pulumi.Input[str] capacity_max: `(string: <optional>)` - Option to signal a maximum volume size. This may not be supported by all storage providers.
         :param pulumi.Input[str] capacity_min: `(string: <optional>)` - Option to signal a minimum volume size. This may not be supported by all storage providers.
-        :param pulumi.Input[str] clone_id: `(string: <optional>)` - The external ID of an existing volume to restore. If ommited, the volume will be created from scratch. Conflicts with `snapshot_id`.
-        :param pulumi.Input[bool] controller_required: `(boolean)`
-        :param pulumi.Input[int] controllers_expected: `(integer)`
-        :param pulumi.Input[int] controllers_healthy: `(integer)`
-        :param pulumi.Input[str] external_id: The ID of the physical volume from the storage provider.
-        :param pulumi.Input['CsiVolumeMountOptionsArgs'] mount_options: `(block: optional)` Options for mounting `block-device` volumes without a pre-formatted file system.
+        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] context: `(map[string]string: <optional>)` - An optional key-value map of strings passed directly to the CSI plugin to validate the volume.
+        :param pulumi.Input[bool] deregister_on_destroy: `(boolean: true)` - If true, the volume will be deregistered on destroy.
+        :param pulumi.Input[str] external_id: `(string: <required>)` - The ID of the physical volume from the storage provider.
+        :param pulumi.Input['CsiVolumeRegistrationMountOptionsArgs'] mount_options: `(block: <optional>)` Options for mounting `block-device` volumes without a pre-formatted file system.
         :param pulumi.Input[str] name: `(string: <required>)` - The display name for the volume.
         :param pulumi.Input[str] namespace: `(string: "default")` - The namespace in which to register the volume.
-        :param pulumi.Input[int] nodes_expected: `(integer)`
-        :param pulumi.Input[int] nodes_healthy: `(integer)`
-        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] parameters: `(map[string]string: optional)` An optional key-value map of strings passed directly to the CSI plugin to configure the volume.
+        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] parameters: `(map[string]string: <optional>)` - An optional key-value map of strings passed directly to the CSI plugin to configure the volume.
         :param pulumi.Input[str] plugin_id: `(string: <required>)` - The ID of the Nomad plugin for registering this volume.
-        :param pulumi.Input[str] plugin_provider: `(string)`
-        :param pulumi.Input[str] plugin_provider_version: `(string)`
-        :param pulumi.Input[bool] schedulable: `(boolean)`
-        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] secrets: `(map[string]string: optional)` An optional key-value map of strings used as credentials for publishing and unpublishing volumes.
-        :param pulumi.Input[str] snapshot_id: `(string: <optional>)` - The external ID of a snapshot to restore. If ommited, the volume will be created from scratch. Conflicts with `clone_id`.
-        :param pulumi.Input[Sequence[pulumi.Input['CsiVolumeTopologyArgs']]] topologies: `(List of topologies)`
-        :param pulumi.Input['CsiVolumeTopologyRequestArgs'] topology_request: `(``TopologyRequest``: <optional>)` - Specify locations (region, zone, rack, etc.) where the provisioned volume is accessible from.
+        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] secrets: `(map[string]string: <optional>)` - An optional key-value map of strings used as credentials for publishing and unpublishing volumes.
+        :param pulumi.Input['CsiVolumeRegistrationTopologyRequestArgs'] topology_request: `(``TopologyRequest``: <optional>)` - Specify locations (region, zone, rack, etc.) where the provisioned volume is accessible from.
         :param pulumi.Input[str] volume_id: `(string: <required>)` - The unique ID of the volume.
         """
         if capabilities is not None:
             pulumi.set(__self__, "capabilities", capabilities)
         if capacity is not None:
             pulumi.set(__self__, "capacity", capacity)
         if capacity_max is not None:
             pulumi.set(__self__, "capacity_max", capacity_max)
         if capacity_max_bytes is not None:
             pulumi.set(__self__, "capacity_max_bytes", capacity_max_bytes)
         if capacity_min is not None:
             pulumi.set(__self__, "capacity_min", capacity_min)
         if capacity_min_bytes is not None:
             pulumi.set(__self__, "capacity_min_bytes", capacity_min_bytes)
-        if clone_id is not None:
-            pulumi.set(__self__, "clone_id", clone_id)
+        if context is not None:
+            pulumi.set(__self__, "context", context)
         if controller_required is not None:
             pulumi.set(__self__, "controller_required", controller_required)
         if controllers_expected is not None:
             pulumi.set(__self__, "controllers_expected", controllers_expected)
         if controllers_healthy is not None:
             pulumi.set(__self__, "controllers_healthy", controllers_healthy)
+        if deregister_on_destroy is not None:
+            pulumi.set(__self__, "deregister_on_destroy", deregister_on_destroy)
         if external_id is not None:
             pulumi.set(__self__, "external_id", external_id)
         if mount_options is not None:
             pulumi.set(__self__, "mount_options", mount_options)
         if name is not None:
             pulumi.set(__self__, "name", name)
         if namespace is not None:
@@ -321,33 +330,31 @@
             pulumi.set(__self__, "plugin_provider", plugin_provider)
         if plugin_provider_version is not None:
             pulumi.set(__self__, "plugin_provider_version", plugin_provider_version)
         if schedulable is not None:
             pulumi.set(__self__, "schedulable", schedulable)
         if secrets is not None:
             pulumi.set(__self__, "secrets", secrets)
-        if snapshot_id is not None:
-            pulumi.set(__self__, "snapshot_id", snapshot_id)
         if topologies is not None:
             pulumi.set(__self__, "topologies", topologies)
         if topology_request is not None:
             pulumi.set(__self__, "topology_request", topology_request)
         if volume_id is not None:
             pulumi.set(__self__, "volume_id", volume_id)
 
     @property
     @pulumi.getter
-    def capabilities(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['CsiVolumeCapabilityArgs']]]]:
+    def capabilities(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['CsiVolumeRegistrationCapabilityArgs']]]]:
         """
         `(``Capability``: <required>)` - Options for validating the capability of a volume.
         """
         return pulumi.get(self, "capabilities")
 
     @capabilities.setter
-    def capabilities(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['CsiVolumeCapabilityArgs']]]]):
+    def capabilities(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['CsiVolumeRegistrationCapabilityArgs']]]]):
         pulumi.set(self, "capabilities", value)
 
     @property
     @pulumi.getter
     def capacity(self) -> Optional[pulumi.Input[int]]:
         return pulumi.get(self, "capacity")
 
@@ -394,83 +401,86 @@
         return pulumi.get(self, "capacity_min_bytes")
 
     @capacity_min_bytes.setter
     def capacity_min_bytes(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "capacity_min_bytes", value)
 
     @property
-    @pulumi.getter(name="cloneId")
-    def clone_id(self) -> Optional[pulumi.Input[str]]:
+    @pulumi.getter
+    def context(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
         """
-        `(string: <optional>)` - The external ID of an existing volume to restore. If ommited, the volume will be created from scratch. Conflicts with `snapshot_id`.
+        `(map[string]string: <optional>)` - An optional key-value map of strings passed directly to the CSI plugin to validate the volume.
         """
-        return pulumi.get(self, "clone_id")
+        return pulumi.get(self, "context")
 
-    @clone_id.setter
-    def clone_id(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "clone_id", value)
+    @context.setter
+    def context(self, value: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]):
+        pulumi.set(self, "context", value)
 
     @property
     @pulumi.getter(name="controllerRequired")
     def controller_required(self) -> Optional[pulumi.Input[bool]]:
-        """
-        `(boolean)`
-        """
         return pulumi.get(self, "controller_required")
 
     @controller_required.setter
     def controller_required(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "controller_required", value)
 
     @property
     @pulumi.getter(name="controllersExpected")
     def controllers_expected(self) -> Optional[pulumi.Input[int]]:
-        """
-        `(integer)`
-        """
         return pulumi.get(self, "controllers_expected")
 
     @controllers_expected.setter
     def controllers_expected(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "controllers_expected", value)
 
     @property
     @pulumi.getter(name="controllersHealthy")
     def controllers_healthy(self) -> Optional[pulumi.Input[int]]:
-        """
-        `(integer)`
-        """
         return pulumi.get(self, "controllers_healthy")
 
     @controllers_healthy.setter
     def controllers_healthy(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "controllers_healthy", value)
 
     @property
+    @pulumi.getter(name="deregisterOnDestroy")
+    def deregister_on_destroy(self) -> Optional[pulumi.Input[bool]]:
+        """
+        `(boolean: true)` - If true, the volume will be deregistered on destroy.
+        """
+        return pulumi.get(self, "deregister_on_destroy")
+
+    @deregister_on_destroy.setter
+    def deregister_on_destroy(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "deregister_on_destroy", value)
+
+    @property
     @pulumi.getter(name="externalId")
     def external_id(self) -> Optional[pulumi.Input[str]]:
         """
-        The ID of the physical volume from the storage provider.
+        `(string: <required>)` - The ID of the physical volume from the storage provider.
         """
         return pulumi.get(self, "external_id")
 
     @external_id.setter
     def external_id(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "external_id", value)
 
     @property
     @pulumi.getter(name="mountOptions")
-    def mount_options(self) -> Optional[pulumi.Input['CsiVolumeMountOptionsArgs']]:
+    def mount_options(self) -> Optional[pulumi.Input['CsiVolumeRegistrationMountOptionsArgs']]:
         """
-        `(block: optional)` Options for mounting `block-device` volumes without a pre-formatted file system.
+        `(block: <optional>)` Options for mounting `block-device` volumes without a pre-formatted file system.
         """
         return pulumi.get(self, "mount_options")
 
     @mount_options.setter
-    def mount_options(self, value: Optional[pulumi.Input['CsiVolumeMountOptionsArgs']]):
+    def mount_options(self, value: Optional[pulumi.Input['CsiVolumeRegistrationMountOptionsArgs']]):
         pulumi.set(self, "mount_options", value)
 
     @property
     @pulumi.getter
     def name(self) -> Optional[pulumi.Input[str]]:
         """
         `(string: <required>)` - The display name for the volume.
@@ -492,40 +502,34 @@
     @namespace.setter
     def namespace(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "namespace", value)
 
     @property
     @pulumi.getter(name="nodesExpected")
     def nodes_expected(self) -> Optional[pulumi.Input[int]]:
-        """
-        `(integer)`
-        """
         return pulumi.get(self, "nodes_expected")
 
     @nodes_expected.setter
     def nodes_expected(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "nodes_expected", value)
 
     @property
     @pulumi.getter(name="nodesHealthy")
     def nodes_healthy(self) -> Optional[pulumi.Input[int]]:
-        """
-        `(integer)`
-        """
         return pulumi.get(self, "nodes_healthy")
 
     @nodes_healthy.setter
     def nodes_healthy(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "nodes_healthy", value)
 
     @property
     @pulumi.getter
     def parameters(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
         """
-        `(map[string]string: optional)` An optional key-value map of strings passed directly to the CSI plugin to configure the volume.
+        `(map[string]string: <optional>)` - An optional key-value map of strings passed directly to the CSI plugin to configure the volume.
         """
         return pulumi.get(self, "parameters")
 
     @parameters.setter
     def parameters(self, value: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]):
         pulumi.set(self, "parameters", value)
 
@@ -540,93 +544,69 @@
     @plugin_id.setter
     def plugin_id(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "plugin_id", value)
 
     @property
     @pulumi.getter(name="pluginProvider")
     def plugin_provider(self) -> Optional[pulumi.Input[str]]:
-        """
-        `(string)`
-        """
         return pulumi.get(self, "plugin_provider")
 
     @plugin_provider.setter
     def plugin_provider(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "plugin_provider", value)
 
     @property
     @pulumi.getter(name="pluginProviderVersion")
     def plugin_provider_version(self) -> Optional[pulumi.Input[str]]:
-        """
-        `(string)`
-        """
         return pulumi.get(self, "plugin_provider_version")
 
     @plugin_provider_version.setter
     def plugin_provider_version(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "plugin_provider_version", value)
 
     @property
     @pulumi.getter
     def schedulable(self) -> Optional[pulumi.Input[bool]]:
-        """
-        `(boolean)`
-        """
         return pulumi.get(self, "schedulable")
 
     @schedulable.setter
     def schedulable(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "schedulable", value)
 
     @property
     @pulumi.getter
     def secrets(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
         """
-        `(map[string]string: optional)` An optional key-value map of strings used as credentials for publishing and unpublishing volumes.
+        `(map[string]string: <optional>)` - An optional key-value map of strings used as credentials for publishing and unpublishing volumes.
         """
         return pulumi.get(self, "secrets")
 
     @secrets.setter
     def secrets(self, value: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]):
         pulumi.set(self, "secrets", value)
 
     @property
-    @pulumi.getter(name="snapshotId")
-    def snapshot_id(self) -> Optional[pulumi.Input[str]]:
-        """
-        `(string: <optional>)` - The external ID of a snapshot to restore. If ommited, the volume will be created from scratch. Conflicts with `clone_id`.
-        """
-        return pulumi.get(self, "snapshot_id")
-
-    @snapshot_id.setter
-    def snapshot_id(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "snapshot_id", value)
-
-    @property
     @pulumi.getter
-    def topologies(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['CsiVolumeTopologyArgs']]]]:
-        """
-        `(List of topologies)`
-        """
+    def topologies(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['CsiVolumeRegistrationTopologyArgs']]]]:
         return pulumi.get(self, "topologies")
 
     @topologies.setter
-    def topologies(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['CsiVolumeTopologyArgs']]]]):
+    def topologies(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['CsiVolumeRegistrationTopologyArgs']]]]):
         pulumi.set(self, "topologies", value)
 
     @property
     @pulumi.getter(name="topologyRequest")
-    def topology_request(self) -> Optional[pulumi.Input['CsiVolumeTopologyRequestArgs']]:
+    def topology_request(self) -> Optional[pulumi.Input['CsiVolumeRegistrationTopologyRequestArgs']]:
         """
         `(``TopologyRequest``: <optional>)` - Specify locations (region, zone, rack, etc.) where the provisioned volume is accessible from.
         """
         return pulumi.get(self, "topology_request")
 
     @topology_request.setter
-    def topology_request(self, value: Optional[pulumi.Input['CsiVolumeTopologyRequestArgs']]):
+    def topology_request(self, value: Optional[pulumi.Input['CsiVolumeRegistrationTopologyRequestArgs']]):
         pulumi.set(self, "topology_request", value)
 
     @property
     @pulumi.getter(name="volumeId")
     def volume_id(self) -> Optional[pulumi.Input[str]]:
         """
         `(string: <required>)` - The unique ID of the volume.
@@ -634,232 +614,226 @@
         return pulumi.get(self, "volume_id")
 
     @volume_id.setter
     def volume_id(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "volume_id", value)
 
 
-class CsiVolume(pulumi.CustomResource):
+class CsiVolumeRegistration(pulumi.CustomResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
-                 capabilities: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['CsiVolumeCapabilityArgs']]]]] = None,
+                 capabilities: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['CsiVolumeRegistrationCapabilityArgs']]]]] = None,
                  capacity_max: Optional[pulumi.Input[str]] = None,
                  capacity_min: Optional[pulumi.Input[str]] = None,
-                 clone_id: Optional[pulumi.Input[str]] = None,
-                 mount_options: Optional[pulumi.Input[pulumi.InputType['CsiVolumeMountOptionsArgs']]] = None,
+                 context: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
+                 deregister_on_destroy: Optional[pulumi.Input[bool]] = None,
+                 external_id: Optional[pulumi.Input[str]] = None,
+                 mount_options: Optional[pulumi.Input[pulumi.InputType['CsiVolumeRegistrationMountOptionsArgs']]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  namespace: Optional[pulumi.Input[str]] = None,
                  parameters: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  plugin_id: Optional[pulumi.Input[str]] = None,
                  secrets: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
-                 snapshot_id: Optional[pulumi.Input[str]] = None,
-                 topology_request: Optional[pulumi.Input[pulumi.InputType['CsiVolumeTopologyRequestArgs']]] = None,
+                 topology_request: Optional[pulumi.Input[pulumi.InputType['CsiVolumeRegistrationTopologyRequestArgs']]] = None,
                  volume_id: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
-        Create a CsiVolume resource with the given unique name, props, and options.
+        Create a CsiVolumeRegistration resource with the given unique name, props, and options.
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['CsiVolumeCapabilityArgs']]]] capabilities: `(``Capability``: <required>)` - Options for validating the capability of a volume.
+        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['CsiVolumeRegistrationCapabilityArgs']]]] capabilities: `(``Capability``: <required>)` - Options for validating the capability of a volume.
         :param pulumi.Input[str] capacity_max: `(string: <optional>)` - Option to signal a maximum volume size. This may not be supported by all storage providers.
         :param pulumi.Input[str] capacity_min: `(string: <optional>)` - Option to signal a minimum volume size. This may not be supported by all storage providers.
-        :param pulumi.Input[str] clone_id: `(string: <optional>)` - The external ID of an existing volume to restore. If ommited, the volume will be created from scratch. Conflicts with `snapshot_id`.
-        :param pulumi.Input[pulumi.InputType['CsiVolumeMountOptionsArgs']] mount_options: `(block: optional)` Options for mounting `block-device` volumes without a pre-formatted file system.
+        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] context: `(map[string]string: <optional>)` - An optional key-value map of strings passed directly to the CSI plugin to validate the volume.
+        :param pulumi.Input[bool] deregister_on_destroy: `(boolean: true)` - If true, the volume will be deregistered on destroy.
+        :param pulumi.Input[str] external_id: `(string: <required>)` - The ID of the physical volume from the storage provider.
+        :param pulumi.Input[pulumi.InputType['CsiVolumeRegistrationMountOptionsArgs']] mount_options: `(block: <optional>)` Options for mounting `block-device` volumes without a pre-formatted file system.
         :param pulumi.Input[str] name: `(string: <required>)` - The display name for the volume.
         :param pulumi.Input[str] namespace: `(string: "default")` - The namespace in which to register the volume.
-        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] parameters: `(map[string]string: optional)` An optional key-value map of strings passed directly to the CSI plugin to configure the volume.
+        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] parameters: `(map[string]string: <optional>)` - An optional key-value map of strings passed directly to the CSI plugin to configure the volume.
         :param pulumi.Input[str] plugin_id: `(string: <required>)` - The ID of the Nomad plugin for registering this volume.
-        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] secrets: `(map[string]string: optional)` An optional key-value map of strings used as credentials for publishing and unpublishing volumes.
-        :param pulumi.Input[str] snapshot_id: `(string: <optional>)` - The external ID of a snapshot to restore. If ommited, the volume will be created from scratch. Conflicts with `clone_id`.
-        :param pulumi.Input[pulumi.InputType['CsiVolumeTopologyRequestArgs']] topology_request: `(``TopologyRequest``: <optional>)` - Specify locations (region, zone, rack, etc.) where the provisioned volume is accessible from.
+        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] secrets: `(map[string]string: <optional>)` - An optional key-value map of strings used as credentials for publishing and unpublishing volumes.
+        :param pulumi.Input[pulumi.InputType['CsiVolumeRegistrationTopologyRequestArgs']] topology_request: `(``TopologyRequest``: <optional>)` - Specify locations (region, zone, rack, etc.) where the provisioned volume is accessible from.
         :param pulumi.Input[str] volume_id: `(string: <required>)` - The unique ID of the volume.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
-                 args: CsiVolumeArgs,
+                 args: CsiVolumeRegistrationArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
-        Create a CsiVolume resource with the given unique name, props, and options.
+        Create a CsiVolumeRegistration resource with the given unique name, props, and options.
         :param str resource_name: The name of the resource.
-        :param CsiVolumeArgs args: The arguments to use to populate this resource's properties.
+        :param CsiVolumeRegistrationArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
-        resource_args, opts = _utilities.get_resource_args_opts(CsiVolumeArgs, pulumi.ResourceOptions, *args, **kwargs)
+        resource_args, opts = _utilities.get_resource_args_opts(CsiVolumeRegistrationArgs, pulumi.ResourceOptions, *args, **kwargs)
         if resource_args is not None:
             __self__._internal_init(resource_name, opts, **resource_args.__dict__)
         else:
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
-                 capabilities: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['CsiVolumeCapabilityArgs']]]]] = None,
+                 capabilities: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['CsiVolumeRegistrationCapabilityArgs']]]]] = None,
                  capacity_max: Optional[pulumi.Input[str]] = None,
                  capacity_min: Optional[pulumi.Input[str]] = None,
-                 clone_id: Optional[pulumi.Input[str]] = None,
-                 mount_options: Optional[pulumi.Input[pulumi.InputType['CsiVolumeMountOptionsArgs']]] = None,
+                 context: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
+                 deregister_on_destroy: Optional[pulumi.Input[bool]] = None,
+                 external_id: Optional[pulumi.Input[str]] = None,
+                 mount_options: Optional[pulumi.Input[pulumi.InputType['CsiVolumeRegistrationMountOptionsArgs']]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  namespace: Optional[pulumi.Input[str]] = None,
                  parameters: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  plugin_id: Optional[pulumi.Input[str]] = None,
                  secrets: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
-                 snapshot_id: Optional[pulumi.Input[str]] = None,
-                 topology_request: Optional[pulumi.Input[pulumi.InputType['CsiVolumeTopologyRequestArgs']]] = None,
+                 topology_request: Optional[pulumi.Input[pulumi.InputType['CsiVolumeRegistrationTopologyRequestArgs']]] = None,
                  volume_id: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
-            __props__ = CsiVolumeArgs.__new__(CsiVolumeArgs)
+            __props__ = CsiVolumeRegistrationArgs.__new__(CsiVolumeRegistrationArgs)
 
-            if capabilities is None and not opts.urn:
-                raise TypeError("Missing required property 'capabilities'")
             __props__.__dict__["capabilities"] = capabilities
             __props__.__dict__["capacity_max"] = capacity_max
             __props__.__dict__["capacity_min"] = capacity_min
-            __props__.__dict__["clone_id"] = clone_id
+            __props__.__dict__["context"] = context
+            __props__.__dict__["deregister_on_destroy"] = deregister_on_destroy
+            if external_id is None and not opts.urn:
+                raise TypeError("Missing required property 'external_id'")
+            __props__.__dict__["external_id"] = external_id
             __props__.__dict__["mount_options"] = mount_options
             __props__.__dict__["name"] = name
             __props__.__dict__["namespace"] = namespace
             __props__.__dict__["parameters"] = parameters
             if plugin_id is None and not opts.urn:
                 raise TypeError("Missing required property 'plugin_id'")
             __props__.__dict__["plugin_id"] = plugin_id
             __props__.__dict__["secrets"] = None if secrets is None else pulumi.Output.secret(secrets)
-            __props__.__dict__["snapshot_id"] = snapshot_id
             __props__.__dict__["topology_request"] = topology_request
             if volume_id is None and not opts.urn:
                 raise TypeError("Missing required property 'volume_id'")
             __props__.__dict__["volume_id"] = volume_id
             __props__.__dict__["capacity"] = None
             __props__.__dict__["capacity_max_bytes"] = None
             __props__.__dict__["capacity_min_bytes"] = None
             __props__.__dict__["controller_required"] = None
             __props__.__dict__["controllers_expected"] = None
             __props__.__dict__["controllers_healthy"] = None
-            __props__.__dict__["external_id"] = None
             __props__.__dict__["nodes_expected"] = None
             __props__.__dict__["nodes_healthy"] = None
             __props__.__dict__["plugin_provider"] = None
             __props__.__dict__["plugin_provider_version"] = None
             __props__.__dict__["schedulable"] = None
             __props__.__dict__["topologies"] = None
         secret_opts = pulumi.ResourceOptions(additional_secret_outputs=["secrets"])
         opts = pulumi.ResourceOptions.merge(opts, secret_opts)
-        super(CsiVolume, __self__).__init__(
-            'nomad:index/csiVolume:CsiVolume',
+        super(CsiVolumeRegistration, __self__).__init__(
+            'nomad:index/csiVolumeRegistration:CsiVolumeRegistration',
             resource_name,
             __props__,
             opts)
 
     @staticmethod
     def get(resource_name: str,
             id: pulumi.Input[str],
             opts: Optional[pulumi.ResourceOptions] = None,
-            capabilities: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['CsiVolumeCapabilityArgs']]]]] = None,
+            capabilities: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['CsiVolumeRegistrationCapabilityArgs']]]]] = None,
             capacity: Optional[pulumi.Input[int]] = None,
             capacity_max: Optional[pulumi.Input[str]] = None,
             capacity_max_bytes: Optional[pulumi.Input[int]] = None,
             capacity_min: Optional[pulumi.Input[str]] = None,
             capacity_min_bytes: Optional[pulumi.Input[int]] = None,
-            clone_id: Optional[pulumi.Input[str]] = None,
+            context: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
             controller_required: Optional[pulumi.Input[bool]] = None,
             controllers_expected: Optional[pulumi.Input[int]] = None,
             controllers_healthy: Optional[pulumi.Input[int]] = None,
+            deregister_on_destroy: Optional[pulumi.Input[bool]] = None,
             external_id: Optional[pulumi.Input[str]] = None,
-            mount_options: Optional[pulumi.Input[pulumi.InputType['CsiVolumeMountOptionsArgs']]] = None,
+            mount_options: Optional[pulumi.Input[pulumi.InputType['CsiVolumeRegistrationMountOptionsArgs']]] = None,
             name: Optional[pulumi.Input[str]] = None,
             namespace: Optional[pulumi.Input[str]] = None,
             nodes_expected: Optional[pulumi.Input[int]] = None,
             nodes_healthy: Optional[pulumi.Input[int]] = None,
             parameters: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
             plugin_id: Optional[pulumi.Input[str]] = None,
             plugin_provider: Optional[pulumi.Input[str]] = None,
             plugin_provider_version: Optional[pulumi.Input[str]] = None,
             schedulable: Optional[pulumi.Input[bool]] = None,
             secrets: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
-            snapshot_id: Optional[pulumi.Input[str]] = None,
-            topologies: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['CsiVolumeTopologyArgs']]]]] = None,
-            topology_request: Optional[pulumi.Input[pulumi.InputType['CsiVolumeTopologyRequestArgs']]] = None,
-            volume_id: Optional[pulumi.Input[str]] = None) -> 'CsiVolume':
+            topologies: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['CsiVolumeRegistrationTopologyArgs']]]]] = None,
+            topology_request: Optional[pulumi.Input[pulumi.InputType['CsiVolumeRegistrationTopologyRequestArgs']]] = None,
+            volume_id: Optional[pulumi.Input[str]] = None) -> 'CsiVolumeRegistration':
         """
-        Get an existing CsiVolume resource's state with the given name, id, and optional extra
+        Get an existing CsiVolumeRegistration resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['CsiVolumeCapabilityArgs']]]] capabilities: `(``Capability``: <required>)` - Options for validating the capability of a volume.
+        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['CsiVolumeRegistrationCapabilityArgs']]]] capabilities: `(``Capability``: <required>)` - Options for validating the capability of a volume.
         :param pulumi.Input[str] capacity_max: `(string: <optional>)` - Option to signal a maximum volume size. This may not be supported by all storage providers.
         :param pulumi.Input[str] capacity_min: `(string: <optional>)` - Option to signal a minimum volume size. This may not be supported by all storage providers.
-        :param pulumi.Input[str] clone_id: `(string: <optional>)` - The external ID of an existing volume to restore. If ommited, the volume will be created from scratch. Conflicts with `snapshot_id`.
-        :param pulumi.Input[bool] controller_required: `(boolean)`
-        :param pulumi.Input[int] controllers_expected: `(integer)`
-        :param pulumi.Input[int] controllers_healthy: `(integer)`
-        :param pulumi.Input[str] external_id: The ID of the physical volume from the storage provider.
-        :param pulumi.Input[pulumi.InputType['CsiVolumeMountOptionsArgs']] mount_options: `(block: optional)` Options for mounting `block-device` volumes without a pre-formatted file system.
+        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] context: `(map[string]string: <optional>)` - An optional key-value map of strings passed directly to the CSI plugin to validate the volume.
+        :param pulumi.Input[bool] deregister_on_destroy: `(boolean: true)` - If true, the volume will be deregistered on destroy.
+        :param pulumi.Input[str] external_id: `(string: <required>)` - The ID of the physical volume from the storage provider.
+        :param pulumi.Input[pulumi.InputType['CsiVolumeRegistrationMountOptionsArgs']] mount_options: `(block: <optional>)` Options for mounting `block-device` volumes without a pre-formatted file system.
         :param pulumi.Input[str] name: `(string: <required>)` - The display name for the volume.
         :param pulumi.Input[str] namespace: `(string: "default")` - The namespace in which to register the volume.
-        :param pulumi.Input[int] nodes_expected: `(integer)`
-        :param pulumi.Input[int] nodes_healthy: `(integer)`
-        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] parameters: `(map[string]string: optional)` An optional key-value map of strings passed directly to the CSI plugin to configure the volume.
+        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] parameters: `(map[string]string: <optional>)` - An optional key-value map of strings passed directly to the CSI plugin to configure the volume.
         :param pulumi.Input[str] plugin_id: `(string: <required>)` - The ID of the Nomad plugin for registering this volume.
-        :param pulumi.Input[str] plugin_provider: `(string)`
-        :param pulumi.Input[str] plugin_provider_version: `(string)`
-        :param pulumi.Input[bool] schedulable: `(boolean)`
-        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] secrets: `(map[string]string: optional)` An optional key-value map of strings used as credentials for publishing and unpublishing volumes.
-        :param pulumi.Input[str] snapshot_id: `(string: <optional>)` - The external ID of a snapshot to restore. If ommited, the volume will be created from scratch. Conflicts with `clone_id`.
-        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['CsiVolumeTopologyArgs']]]] topologies: `(List of topologies)`
-        :param pulumi.Input[pulumi.InputType['CsiVolumeTopologyRequestArgs']] topology_request: `(``TopologyRequest``: <optional>)` - Specify locations (region, zone, rack, etc.) where the provisioned volume is accessible from.
+        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] secrets: `(map[string]string: <optional>)` - An optional key-value map of strings used as credentials for publishing and unpublishing volumes.
+        :param pulumi.Input[pulumi.InputType['CsiVolumeRegistrationTopologyRequestArgs']] topology_request: `(``TopologyRequest``: <optional>)` - Specify locations (region, zone, rack, etc.) where the provisioned volume is accessible from.
         :param pulumi.Input[str] volume_id: `(string: <required>)` - The unique ID of the volume.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
-        __props__ = _CsiVolumeState.__new__(_CsiVolumeState)
+        __props__ = _CsiVolumeRegistrationState.__new__(_CsiVolumeRegistrationState)
 
         __props__.__dict__["capabilities"] = capabilities
         __props__.__dict__["capacity"] = capacity
         __props__.__dict__["capacity_max"] = capacity_max
         __props__.__dict__["capacity_max_bytes"] = capacity_max_bytes
         __props__.__dict__["capacity_min"] = capacity_min
         __props__.__dict__["capacity_min_bytes"] = capacity_min_bytes
-        __props__.__dict__["clone_id"] = clone_id
+        __props__.__dict__["context"] = context
         __props__.__dict__["controller_required"] = controller_required
         __props__.__dict__["controllers_expected"] = controllers_expected
         __props__.__dict__["controllers_healthy"] = controllers_healthy
+        __props__.__dict__["deregister_on_destroy"] = deregister_on_destroy
         __props__.__dict__["external_id"] = external_id
         __props__.__dict__["mount_options"] = mount_options
         __props__.__dict__["name"] = name
         __props__.__dict__["namespace"] = namespace
         __props__.__dict__["nodes_expected"] = nodes_expected
         __props__.__dict__["nodes_healthy"] = nodes_healthy
         __props__.__dict__["parameters"] = parameters
         __props__.__dict__["plugin_id"] = plugin_id
         __props__.__dict__["plugin_provider"] = plugin_provider
         __props__.__dict__["plugin_provider_version"] = plugin_provider_version
         __props__.__dict__["schedulable"] = schedulable
         __props__.__dict__["secrets"] = secrets
-        __props__.__dict__["snapshot_id"] = snapshot_id
         __props__.__dict__["topologies"] = topologies
         __props__.__dict__["topology_request"] = topology_request
         __props__.__dict__["volume_id"] = volume_id
-        return CsiVolume(resource_name, opts=opts, __props__=__props__)
+        return CsiVolumeRegistration(resource_name, opts=opts, __props__=__props__)
 
     @property
     @pulumi.getter
-    def capabilities(self) -> pulumi.Output[Sequence['outputs.CsiVolumeCapability']]:
+    def capabilities(self) -> pulumi.Output[Optional[Sequence['outputs.CsiVolumeRegistrationCapability']]]:
         """
         `(``Capability``: <required>)` - Options for validating the capability of a volume.
         """
         return pulumi.get(self, "capabilities")
 
     @property
     @pulumi.getter
@@ -889,58 +863,57 @@
 
     @property
     @pulumi.getter(name="capacityMinBytes")
     def capacity_min_bytes(self) -> pulumi.Output[int]:
         return pulumi.get(self, "capacity_min_bytes")
 
     @property
-    @pulumi.getter(name="cloneId")
-    def clone_id(self) -> pulumi.Output[Optional[str]]:
+    @pulumi.getter
+    def context(self) -> pulumi.Output[Optional[Mapping[str, str]]]:
         """
-        `(string: <optional>)` - The external ID of an existing volume to restore. If ommited, the volume will be created from scratch. Conflicts with `snapshot_id`.
+        `(map[string]string: <optional>)` - An optional key-value map of strings passed directly to the CSI plugin to validate the volume.
         """
-        return pulumi.get(self, "clone_id")
+        return pulumi.get(self, "context")
 
     @property
     @pulumi.getter(name="controllerRequired")
     def controller_required(self) -> pulumi.Output[bool]:
-        """
-        `(boolean)`
-        """
         return pulumi.get(self, "controller_required")
 
     @property
     @pulumi.getter(name="controllersExpected")
     def controllers_expected(self) -> pulumi.Output[int]:
-        """
-        `(integer)`
-        """
         return pulumi.get(self, "controllers_expected")
 
     @property
     @pulumi.getter(name="controllersHealthy")
     def controllers_healthy(self) -> pulumi.Output[int]:
+        return pulumi.get(self, "controllers_healthy")
+
+    @property
+    @pulumi.getter(name="deregisterOnDestroy")
+    def deregister_on_destroy(self) -> pulumi.Output[Optional[bool]]:
         """
-        `(integer)`
+        `(boolean: true)` - If true, the volume will be deregistered on destroy.
         """
-        return pulumi.get(self, "controllers_healthy")
+        return pulumi.get(self, "deregister_on_destroy")
 
     @property
     @pulumi.getter(name="externalId")
     def external_id(self) -> pulumi.Output[str]:
         """
-        The ID of the physical volume from the storage provider.
+        `(string: <required>)` - The ID of the physical volume from the storage provider.
         """
         return pulumi.get(self, "external_id")
 
     @property
     @pulumi.getter(name="mountOptions")
-    def mount_options(self) -> pulumi.Output[Optional['outputs.CsiVolumeMountOptions']]:
+    def mount_options(self) -> pulumi.Output[Optional['outputs.CsiVolumeRegistrationMountOptions']]:
         """
-        `(block: optional)` Options for mounting `block-device` volumes without a pre-formatted file system.
+        `(block: <optional>)` Options for mounting `block-device` volumes without a pre-formatted file system.
         """
         return pulumi.get(self, "mount_options")
 
     @property
     @pulumi.getter
     def name(self) -> pulumi.Output[str]:
         """
@@ -955,94 +928,68 @@
         `(string: "default")` - The namespace in which to register the volume.
         """
         return pulumi.get(self, "namespace")
 
     @property
     @pulumi.getter(name="nodesExpected")
     def nodes_expected(self) -> pulumi.Output[int]:
-        """
-        `(integer)`
-        """
         return pulumi.get(self, "nodes_expected")
 
     @property
     @pulumi.getter(name="nodesHealthy")
     def nodes_healthy(self) -> pulumi.Output[int]:
-        """
-        `(integer)`
-        """
         return pulumi.get(self, "nodes_healthy")
 
     @property
     @pulumi.getter
     def parameters(self) -> pulumi.Output[Optional[Mapping[str, str]]]:
         """
-        `(map[string]string: optional)` An optional key-value map of strings passed directly to the CSI plugin to configure the volume.
+        `(map[string]string: <optional>)` - An optional key-value map of strings passed directly to the CSI plugin to configure the volume.
         """
         return pulumi.get(self, "parameters")
 
     @property
     @pulumi.getter(name="pluginId")
     def plugin_id(self) -> pulumi.Output[str]:
         """
         `(string: <required>)` - The ID of the Nomad plugin for registering this volume.
         """
         return pulumi.get(self, "plugin_id")
 
     @property
     @pulumi.getter(name="pluginProvider")
     def plugin_provider(self) -> pulumi.Output[str]:
-        """
-        `(string)`
-        """
         return pulumi.get(self, "plugin_provider")
 
     @property
     @pulumi.getter(name="pluginProviderVersion")
     def plugin_provider_version(self) -> pulumi.Output[str]:
-        """
-        `(string)`
-        """
         return pulumi.get(self, "plugin_provider_version")
 
     @property
     @pulumi.getter
     def schedulable(self) -> pulumi.Output[bool]:
-        """
-        `(boolean)`
-        """
         return pulumi.get(self, "schedulable")
 
     @property
     @pulumi.getter
     def secrets(self) -> pulumi.Output[Optional[Mapping[str, str]]]:
         """
-        `(map[string]string: optional)` An optional key-value map of strings used as credentials for publishing and unpublishing volumes.
+        `(map[string]string: <optional>)` - An optional key-value map of strings used as credentials for publishing and unpublishing volumes.
         """
         return pulumi.get(self, "secrets")
 
     @property
-    @pulumi.getter(name="snapshotId")
-    def snapshot_id(self) -> pulumi.Output[Optional[str]]:
-        """
-        `(string: <optional>)` - The external ID of a snapshot to restore. If ommited, the volume will be created from scratch. Conflicts with `clone_id`.
-        """
-        return pulumi.get(self, "snapshot_id")
-
-    @property
     @pulumi.getter
-    def topologies(self) -> pulumi.Output[Sequence['outputs.CsiVolumeTopology']]:
-        """
-        `(List of topologies)`
-        """
+    def topologies(self) -> pulumi.Output[Sequence['outputs.CsiVolumeRegistrationTopology']]:
         return pulumi.get(self, "topologies")
 
     @property
     @pulumi.getter(name="topologyRequest")
-    def topology_request(self) -> pulumi.Output[Optional['outputs.CsiVolumeTopologyRequest']]:
+    def topology_request(self) -> pulumi.Output[Optional['outputs.CsiVolumeRegistrationTopologyRequest']]:
         """
         `(``TopologyRequest``: <optional>)` - Specify locations (region, zone, rack, etc.) where the provisioned volume is accessible from.
         """
         return pulumi.get(self, "topology_request")
 
     @property
     @pulumi.getter(name="volumeId")
```

### Comparing `pulumi_nomad-2.3.0a1713561631/pulumi_nomad/csi_volume_registration.py` & `pulumi_nomad-2.3.0a1713899842/pulumi_nomad/external_volume.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,87 +7,87 @@
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 from . import outputs
 from ._inputs import *
 
-__all__ = ['CsiVolumeRegistrationArgs', 'CsiVolumeRegistration']
+__all__ = ['ExternalVolumeArgs', 'ExternalVolume']
 
 @pulumi.input_type
-class CsiVolumeRegistrationArgs:
+class ExternalVolumeArgs:
     def __init__(__self__, *,
-                 external_id: pulumi.Input[str],
+                 capabilities: pulumi.Input[Sequence[pulumi.Input['ExternalVolumeCapabilityArgs']]],
                  plugin_id: pulumi.Input[str],
                  volume_id: pulumi.Input[str],
-                 capabilities: Optional[pulumi.Input[Sequence[pulumi.Input['CsiVolumeRegistrationCapabilityArgs']]]] = None,
                  capacity_max: Optional[pulumi.Input[str]] = None,
                  capacity_min: Optional[pulumi.Input[str]] = None,
-                 context: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
-                 deregister_on_destroy: Optional[pulumi.Input[bool]] = None,
-                 mount_options: Optional[pulumi.Input['CsiVolumeRegistrationMountOptionsArgs']] = None,
+                 clone_id: Optional[pulumi.Input[str]] = None,
+                 mount_options: Optional[pulumi.Input['ExternalVolumeMountOptionsArgs']] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  namespace: Optional[pulumi.Input[str]] = None,
                  parameters: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  secrets: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
-                 topology_request: Optional[pulumi.Input['CsiVolumeRegistrationTopologyRequestArgs']] = None):
+                 snapshot_id: Optional[pulumi.Input[str]] = None,
+                 topology_request: Optional[pulumi.Input['ExternalVolumeTopologyRequestArgs']] = None,
+                 type: Optional[pulumi.Input[str]] = None):
         """
-        The set of arguments for constructing a CsiVolumeRegistration resource.
-        :param pulumi.Input[str] external_id: `(string: <required>)` - The ID of the physical volume from the storage provider.
+        The set of arguments for constructing a ExternalVolume resource.
+        :param pulumi.Input[Sequence[pulumi.Input['ExternalVolumeCapabilityArgs']]] capabilities: `(``Capability``: <required>)` - Options for validating the capability of a volume.
         :param pulumi.Input[str] plugin_id: `(string: <required>)` - The ID of the Nomad plugin for registering this volume.
         :param pulumi.Input[str] volume_id: `(string: <required>)` - The unique ID of the volume.
-        :param pulumi.Input[Sequence[pulumi.Input['CsiVolumeRegistrationCapabilityArgs']]] capabilities: `(``Capability``: <required>)` - Options for validating the capability of a volume.
         :param pulumi.Input[str] capacity_max: `(string: <optional>)` - Option to signal a maximum volume size. This may not be supported by all storage providers.
         :param pulumi.Input[str] capacity_min: `(string: <optional>)` - Option to signal a minimum volume size. This may not be supported by all storage providers.
-        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] context: `(map[string]string: <optional>)` - An optional key-value map of strings passed directly to the CSI plugin to validate the volume.
-        :param pulumi.Input[bool] deregister_on_destroy: `(boolean: true)` - If true, the volume will be deregistered on destroy.
-        :param pulumi.Input['CsiVolumeRegistrationMountOptionsArgs'] mount_options: `(block: <optional>)` Options for mounting `block-device` volumes without a pre-formatted file system.
+        :param pulumi.Input[str] clone_id: `(string: <optional>)` - The external ID of an existing volume to restore. If ommited, the volume will be created from scratch. Conflicts with `snapshot_id`.
+        :param pulumi.Input['ExternalVolumeMountOptionsArgs'] mount_options: `(block: optional)` Options for mounting `block-device` volumes without a pre-formatted file system.
         :param pulumi.Input[str] name: `(string: <required>)` - The display name for the volume.
         :param pulumi.Input[str] namespace: `(string: "default")` - The namespace in which to register the volume.
-        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] parameters: `(map[string]string: <optional>)` - An optional key-value map of strings passed directly to the CSI plugin to configure the volume.
-        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] secrets: `(map[string]string: <optional>)` - An optional key-value map of strings used as credentials for publishing and unpublishing volumes.
-        :param pulumi.Input['CsiVolumeRegistrationTopologyRequestArgs'] topology_request: `(``TopologyRequest``: <optional>)` - Specify locations (region, zone, rack, etc.) where the provisioned volume is accessible from.
+        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] parameters: `(map[string]string: optional)` An optional key-value map of strings passed directly to the CSI plugin to configure the volume.
+        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] secrets: `(map[string]string: optional)` An optional key-value map of strings used as credentials for publishing and unpublishing volumes.
+        :param pulumi.Input[str] snapshot_id: `(string: <optional>)` - The external ID of a snapshot to restore. If ommited, the volume will be created from scratch. Conflicts with `clone_id`.
+        :param pulumi.Input['ExternalVolumeTopologyRequestArgs'] topology_request: `(``TopologyRequest``: <optional>)` - Specify locations (region, zone, rack, etc.) where the provisioned volume is accessible from.
+        :param pulumi.Input[str] type: `(string: <required>)` - The type of the volume. Currently, only `csi` is supported.
         """
-        pulumi.set(__self__, "external_id", external_id)
+        pulumi.set(__self__, "capabilities", capabilities)
         pulumi.set(__self__, "plugin_id", plugin_id)
         pulumi.set(__self__, "volume_id", volume_id)
-        if capabilities is not None:
-            pulumi.set(__self__, "capabilities", capabilities)
         if capacity_max is not None:
             pulumi.set(__self__, "capacity_max", capacity_max)
         if capacity_min is not None:
             pulumi.set(__self__, "capacity_min", capacity_min)
-        if context is not None:
-            pulumi.set(__self__, "context", context)
-        if deregister_on_destroy is not None:
-            pulumi.set(__self__, "deregister_on_destroy", deregister_on_destroy)
+        if clone_id is not None:
+            pulumi.set(__self__, "clone_id", clone_id)
         if mount_options is not None:
             pulumi.set(__self__, "mount_options", mount_options)
         if name is not None:
             pulumi.set(__self__, "name", name)
         if namespace is not None:
             pulumi.set(__self__, "namespace", namespace)
         if parameters is not None:
             pulumi.set(__self__, "parameters", parameters)
         if secrets is not None:
             pulumi.set(__self__, "secrets", secrets)
+        if snapshot_id is not None:
+            pulumi.set(__self__, "snapshot_id", snapshot_id)
         if topology_request is not None:
             pulumi.set(__self__, "topology_request", topology_request)
+        if type is not None:
+            pulumi.set(__self__, "type", type)
 
     @property
-    @pulumi.getter(name="externalId")
-    def external_id(self) -> pulumi.Input[str]:
+    @pulumi.getter
+    def capabilities(self) -> pulumi.Input[Sequence[pulumi.Input['ExternalVolumeCapabilityArgs']]]:
         """
-        `(string: <required>)` - The ID of the physical volume from the storage provider.
+        `(``Capability``: <required>)` - Options for validating the capability of a volume.
         """
-        return pulumi.get(self, "external_id")
+        return pulumi.get(self, "capabilities")
 
-    @external_id.setter
-    def external_id(self, value: pulumi.Input[str]):
-        pulumi.set(self, "external_id", value)
+    @capabilities.setter
+    def capabilities(self, value: pulumi.Input[Sequence[pulumi.Input['ExternalVolumeCapabilityArgs']]]):
+        pulumi.set(self, "capabilities", value)
 
     @property
     @pulumi.getter(name="pluginId")
     def plugin_id(self) -> pulumi.Input[str]:
         """
         `(string: <required>)` - The ID of the Nomad plugin for registering this volume.
         """
@@ -106,26 +106,14 @@
         return pulumi.get(self, "volume_id")
 
     @volume_id.setter
     def volume_id(self, value: pulumi.Input[str]):
         pulumi.set(self, "volume_id", value)
 
     @property
-    @pulumi.getter
-    def capabilities(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['CsiVolumeRegistrationCapabilityArgs']]]]:
-        """
-        `(``Capability``: <required>)` - Options for validating the capability of a volume.
-        """
-        return pulumi.get(self, "capabilities")
-
-    @capabilities.setter
-    def capabilities(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['CsiVolumeRegistrationCapabilityArgs']]]]):
-        pulumi.set(self, "capabilities", value)
-
-    @property
     @pulumi.getter(name="capacityMax")
     def capacity_max(self) -> Optional[pulumi.Input[str]]:
         """
         `(string: <optional>)` - Option to signal a maximum volume size. This may not be supported by all storage providers.
         """
         return pulumi.get(self, "capacity_max")
 
@@ -142,47 +130,35 @@
         return pulumi.get(self, "capacity_min")
 
     @capacity_min.setter
     def capacity_min(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "capacity_min", value)
 
     @property
-    @pulumi.getter
-    def context(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
-        """
-        `(map[string]string: <optional>)` - An optional key-value map of strings passed directly to the CSI plugin to validate the volume.
-        """
-        return pulumi.get(self, "context")
-
-    @context.setter
-    def context(self, value: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]):
-        pulumi.set(self, "context", value)
-
-    @property
-    @pulumi.getter(name="deregisterOnDestroy")
-    def deregister_on_destroy(self) -> Optional[pulumi.Input[bool]]:
+    @pulumi.getter(name="cloneId")
+    def clone_id(self) -> Optional[pulumi.Input[str]]:
         """
-        `(boolean: true)` - If true, the volume will be deregistered on destroy.
+        `(string: <optional>)` - The external ID of an existing volume to restore. If ommited, the volume will be created from scratch. Conflicts with `snapshot_id`.
         """
-        return pulumi.get(self, "deregister_on_destroy")
+        return pulumi.get(self, "clone_id")
 
-    @deregister_on_destroy.setter
-    def deregister_on_destroy(self, value: Optional[pulumi.Input[bool]]):
-        pulumi.set(self, "deregister_on_destroy", value)
+    @clone_id.setter
+    def clone_id(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "clone_id", value)
 
     @property
     @pulumi.getter(name="mountOptions")
-    def mount_options(self) -> Optional[pulumi.Input['CsiVolumeRegistrationMountOptionsArgs']]:
+    def mount_options(self) -> Optional[pulumi.Input['ExternalVolumeMountOptionsArgs']]:
         """
-        `(block: <optional>)` Options for mounting `block-device` volumes without a pre-formatted file system.
+        `(block: optional)` Options for mounting `block-device` volumes without a pre-formatted file system.
         """
         return pulumi.get(self, "mount_options")
 
     @mount_options.setter
-    def mount_options(self, value: Optional[pulumi.Input['CsiVolumeRegistrationMountOptionsArgs']]):
+    def mount_options(self, value: Optional[pulumi.Input['ExternalVolumeMountOptionsArgs']]):
         pulumi.set(self, "mount_options", value)
 
     @property
     @pulumi.getter
     def name(self) -> Optional[pulumi.Input[str]]:
         """
         `(string: <required>)` - The display name for the volume.
@@ -205,126 +181,128 @@
     def namespace(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "namespace", value)
 
     @property
     @pulumi.getter
     def parameters(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
         """
-        `(map[string]string: <optional>)` - An optional key-value map of strings passed directly to the CSI plugin to configure the volume.
+        `(map[string]string: optional)` An optional key-value map of strings passed directly to the CSI plugin to configure the volume.
         """
         return pulumi.get(self, "parameters")
 
     @parameters.setter
     def parameters(self, value: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]):
         pulumi.set(self, "parameters", value)
 
     @property
     @pulumi.getter
     def secrets(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
         """
-        `(map[string]string: <optional>)` - An optional key-value map of strings used as credentials for publishing and unpublishing volumes.
+        `(map[string]string: optional)` An optional key-value map of strings used as credentials for publishing and unpublishing volumes.
         """
         return pulumi.get(self, "secrets")
 
     @secrets.setter
     def secrets(self, value: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]):
         pulumi.set(self, "secrets", value)
 
     @property
+    @pulumi.getter(name="snapshotId")
+    def snapshot_id(self) -> Optional[pulumi.Input[str]]:
+        """
+        `(string: <optional>)` - The external ID of a snapshot to restore. If ommited, the volume will be created from scratch. Conflicts with `clone_id`.
+        """
+        return pulumi.get(self, "snapshot_id")
+
+    @snapshot_id.setter
+    def snapshot_id(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "snapshot_id", value)
+
+    @property
     @pulumi.getter(name="topologyRequest")
-    def topology_request(self) -> Optional[pulumi.Input['CsiVolumeRegistrationTopologyRequestArgs']]:
+    def topology_request(self) -> Optional[pulumi.Input['ExternalVolumeTopologyRequestArgs']]:
         """
         `(``TopologyRequest``: <optional>)` - Specify locations (region, zone, rack, etc.) where the provisioned volume is accessible from.
         """
         return pulumi.get(self, "topology_request")
 
     @topology_request.setter
-    def topology_request(self, value: Optional[pulumi.Input['CsiVolumeRegistrationTopologyRequestArgs']]):
+    def topology_request(self, value: Optional[pulumi.Input['ExternalVolumeTopologyRequestArgs']]):
         pulumi.set(self, "topology_request", value)
 
+    @property
+    @pulumi.getter
+    def type(self) -> Optional[pulumi.Input[str]]:
+        """
+        `(string: <required>)` - The type of the volume. Currently, only `csi` is supported.
+        """
+        return pulumi.get(self, "type")
+
+    @type.setter
+    def type(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "type", value)
+
 
 @pulumi.input_type
-class _CsiVolumeRegistrationState:
+class _ExternalVolumeState:
     def __init__(__self__, *,
-                 capabilities: Optional[pulumi.Input[Sequence[pulumi.Input['CsiVolumeRegistrationCapabilityArgs']]]] = None,
-                 capacity: Optional[pulumi.Input[int]] = None,
+                 capabilities: Optional[pulumi.Input[Sequence[pulumi.Input['ExternalVolumeCapabilityArgs']]]] = None,
                  capacity_max: Optional[pulumi.Input[str]] = None,
-                 capacity_max_bytes: Optional[pulumi.Input[int]] = None,
                  capacity_min: Optional[pulumi.Input[str]] = None,
-                 capacity_min_bytes: Optional[pulumi.Input[int]] = None,
-                 context: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
+                 clone_id: Optional[pulumi.Input[str]] = None,
                  controller_required: Optional[pulumi.Input[bool]] = None,
                  controllers_expected: Optional[pulumi.Input[int]] = None,
                  controllers_healthy: Optional[pulumi.Input[int]] = None,
-                 deregister_on_destroy: Optional[pulumi.Input[bool]] = None,
-                 external_id: Optional[pulumi.Input[str]] = None,
-                 mount_options: Optional[pulumi.Input['CsiVolumeRegistrationMountOptionsArgs']] = None,
+                 mount_options: Optional[pulumi.Input['ExternalVolumeMountOptionsArgs']] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  namespace: Optional[pulumi.Input[str]] = None,
                  nodes_expected: Optional[pulumi.Input[int]] = None,
                  nodes_healthy: Optional[pulumi.Input[int]] = None,
                  parameters: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  plugin_id: Optional[pulumi.Input[str]] = None,
                  plugin_provider: Optional[pulumi.Input[str]] = None,
                  plugin_provider_version: Optional[pulumi.Input[str]] = None,
                  schedulable: Optional[pulumi.Input[bool]] = None,
                  secrets: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
-                 topologies: Optional[pulumi.Input[Sequence[pulumi.Input['CsiVolumeRegistrationTopologyArgs']]]] = None,
-                 topology_request: Optional[pulumi.Input['CsiVolumeRegistrationTopologyRequestArgs']] = None,
+                 snapshot_id: Optional[pulumi.Input[str]] = None,
+                 topologies: Optional[pulumi.Input[Sequence[pulumi.Input['ExternalVolumeTopologyArgs']]]] = None,
+                 topology_request: Optional[pulumi.Input['ExternalVolumeTopologyRequestArgs']] = None,
+                 type: Optional[pulumi.Input[str]] = None,
                  volume_id: Optional[pulumi.Input[str]] = None):
         """
-        Input properties used for looking up and filtering CsiVolumeRegistration resources.
-        :param pulumi.Input[Sequence[pulumi.Input['CsiVolumeRegistrationCapabilityArgs']]] capabilities: `(``Capability``: <required>)` - Options for validating the capability of a volume.
+        Input properties used for looking up and filtering ExternalVolume resources.
+        :param pulumi.Input[Sequence[pulumi.Input['ExternalVolumeCapabilityArgs']]] capabilities: `(``Capability``: <required>)` - Options for validating the capability of a volume.
         :param pulumi.Input[str] capacity_max: `(string: <optional>)` - Option to signal a maximum volume size. This may not be supported by all storage providers.
         :param pulumi.Input[str] capacity_min: `(string: <optional>)` - Option to signal a minimum volume size. This may not be supported by all storage providers.
-        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] context: `(map[string]string: <optional>)` - An optional key-value map of strings passed directly to the CSI plugin to validate the volume.
-        :param pulumi.Input[bool] controller_required: `(boolean)`
-        :param pulumi.Input[int] controllers_expected: `(integer)`
-        :param pulumi.Input[int] controllers_healthy: `(integer)`
-        :param pulumi.Input[bool] deregister_on_destroy: `(boolean: true)` - If true, the volume will be deregistered on destroy.
-        :param pulumi.Input[str] external_id: `(string: <required>)` - The ID of the physical volume from the storage provider.
-        :param pulumi.Input['CsiVolumeRegistrationMountOptionsArgs'] mount_options: `(block: <optional>)` Options for mounting `block-device` volumes without a pre-formatted file system.
+        :param pulumi.Input[str] clone_id: `(string: <optional>)` - The external ID of an existing volume to restore. If ommited, the volume will be created from scratch. Conflicts with `snapshot_id`.
+        :param pulumi.Input['ExternalVolumeMountOptionsArgs'] mount_options: `(block: optional)` Options for mounting `block-device` volumes without a pre-formatted file system.
         :param pulumi.Input[str] name: `(string: <required>)` - The display name for the volume.
         :param pulumi.Input[str] namespace: `(string: "default")` - The namespace in which to register the volume.
-        :param pulumi.Input[int] nodes_expected: `(integer)`
-        :param pulumi.Input[int] nodes_healthy: `(integer)`
-        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] parameters: `(map[string]string: <optional>)` - An optional key-value map of strings passed directly to the CSI plugin to configure the volume.
+        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] parameters: `(map[string]string: optional)` An optional key-value map of strings passed directly to the CSI plugin to configure the volume.
         :param pulumi.Input[str] plugin_id: `(string: <required>)` - The ID of the Nomad plugin for registering this volume.
-        :param pulumi.Input[str] plugin_provider: `(string)`
-        :param pulumi.Input[str] plugin_provider_version: `(string)`
-        :param pulumi.Input[bool] schedulable: `(boolean)`
-        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] secrets: `(map[string]string: <optional>)` - An optional key-value map of strings used as credentials for publishing and unpublishing volumes.
-        :param pulumi.Input[Sequence[pulumi.Input['CsiVolumeRegistrationTopologyArgs']]] topologies: `(List of topologies)`
-        :param pulumi.Input['CsiVolumeRegistrationTopologyRequestArgs'] topology_request: `(``TopologyRequest``: <optional>)` - Specify locations (region, zone, rack, etc.) where the provisioned volume is accessible from.
+        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] secrets: `(map[string]string: optional)` An optional key-value map of strings used as credentials for publishing and unpublishing volumes.
+        :param pulumi.Input[str] snapshot_id: `(string: <optional>)` - The external ID of a snapshot to restore. If ommited, the volume will be created from scratch. Conflicts with `clone_id`.
+        :param pulumi.Input['ExternalVolumeTopologyRequestArgs'] topology_request: `(``TopologyRequest``: <optional>)` - Specify locations (region, zone, rack, etc.) where the provisioned volume is accessible from.
+        :param pulumi.Input[str] type: `(string: <required>)` - The type of the volume. Currently, only `csi` is supported.
         :param pulumi.Input[str] volume_id: `(string: <required>)` - The unique ID of the volume.
         """
         if capabilities is not None:
             pulumi.set(__self__, "capabilities", capabilities)
-        if capacity is not None:
-            pulumi.set(__self__, "capacity", capacity)
         if capacity_max is not None:
             pulumi.set(__self__, "capacity_max", capacity_max)
-        if capacity_max_bytes is not None:
-            pulumi.set(__self__, "capacity_max_bytes", capacity_max_bytes)
         if capacity_min is not None:
             pulumi.set(__self__, "capacity_min", capacity_min)
-        if capacity_min_bytes is not None:
-            pulumi.set(__self__, "capacity_min_bytes", capacity_min_bytes)
-        if context is not None:
-            pulumi.set(__self__, "context", context)
+        if clone_id is not None:
+            pulumi.set(__self__, "clone_id", clone_id)
         if controller_required is not None:
             pulumi.set(__self__, "controller_required", controller_required)
         if controllers_expected is not None:
             pulumi.set(__self__, "controllers_expected", controllers_expected)
         if controllers_healthy is not None:
             pulumi.set(__self__, "controllers_healthy", controllers_healthy)
-        if deregister_on_destroy is not None:
-            pulumi.set(__self__, "deregister_on_destroy", deregister_on_destroy)
-        if external_id is not None:
-            pulumi.set(__self__, "external_id", external_id)
         if mount_options is not None:
             pulumi.set(__self__, "mount_options", mount_options)
         if name is not None:
             pulumi.set(__self__, "name", name)
         if namespace is not None:
             pulumi.set(__self__, "namespace", namespace)
         if nodes_expected is not None:
@@ -339,166 +317,110 @@
             pulumi.set(__self__, "plugin_provider", plugin_provider)
         if plugin_provider_version is not None:
             pulumi.set(__self__, "plugin_provider_version", plugin_provider_version)
         if schedulable is not None:
             pulumi.set(__self__, "schedulable", schedulable)
         if secrets is not None:
             pulumi.set(__self__, "secrets", secrets)
+        if snapshot_id is not None:
+            pulumi.set(__self__, "snapshot_id", snapshot_id)
         if topologies is not None:
             pulumi.set(__self__, "topologies", topologies)
         if topology_request is not None:
             pulumi.set(__self__, "topology_request", topology_request)
+        if type is not None:
+            pulumi.set(__self__, "type", type)
         if volume_id is not None:
             pulumi.set(__self__, "volume_id", volume_id)
 
     @property
     @pulumi.getter
-    def capabilities(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['CsiVolumeRegistrationCapabilityArgs']]]]:
+    def capabilities(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['ExternalVolumeCapabilityArgs']]]]:
         """
         `(``Capability``: <required>)` - Options for validating the capability of a volume.
         """
         return pulumi.get(self, "capabilities")
 
     @capabilities.setter
-    def capabilities(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['CsiVolumeRegistrationCapabilityArgs']]]]):
+    def capabilities(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['ExternalVolumeCapabilityArgs']]]]):
         pulumi.set(self, "capabilities", value)
 
     @property
-    @pulumi.getter
-    def capacity(self) -> Optional[pulumi.Input[int]]:
-        return pulumi.get(self, "capacity")
-
-    @capacity.setter
-    def capacity(self, value: Optional[pulumi.Input[int]]):
-        pulumi.set(self, "capacity", value)
-
-    @property
     @pulumi.getter(name="capacityMax")
     def capacity_max(self) -> Optional[pulumi.Input[str]]:
         """
         `(string: <optional>)` - Option to signal a maximum volume size. This may not be supported by all storage providers.
         """
         return pulumi.get(self, "capacity_max")
 
     @capacity_max.setter
     def capacity_max(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "capacity_max", value)
 
     @property
-    @pulumi.getter(name="capacityMaxBytes")
-    def capacity_max_bytes(self) -> Optional[pulumi.Input[int]]:
-        return pulumi.get(self, "capacity_max_bytes")
-
-    @capacity_max_bytes.setter
-    def capacity_max_bytes(self, value: Optional[pulumi.Input[int]]):
-        pulumi.set(self, "capacity_max_bytes", value)
-
-    @property
     @pulumi.getter(name="capacityMin")
     def capacity_min(self) -> Optional[pulumi.Input[str]]:
         """
         `(string: <optional>)` - Option to signal a minimum volume size. This may not be supported by all storage providers.
         """
         return pulumi.get(self, "capacity_min")
 
     @capacity_min.setter
     def capacity_min(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "capacity_min", value)
 
     @property
-    @pulumi.getter(name="capacityMinBytes")
-    def capacity_min_bytes(self) -> Optional[pulumi.Input[int]]:
-        return pulumi.get(self, "capacity_min_bytes")
-
-    @capacity_min_bytes.setter
-    def capacity_min_bytes(self, value: Optional[pulumi.Input[int]]):
-        pulumi.set(self, "capacity_min_bytes", value)
-
-    @property
-    @pulumi.getter
-    def context(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
+    @pulumi.getter(name="cloneId")
+    def clone_id(self) -> Optional[pulumi.Input[str]]:
         """
-        `(map[string]string: <optional>)` - An optional key-value map of strings passed directly to the CSI plugin to validate the volume.
+        `(string: <optional>)` - The external ID of an existing volume to restore. If ommited, the volume will be created from scratch. Conflicts with `snapshot_id`.
         """
-        return pulumi.get(self, "context")
+        return pulumi.get(self, "clone_id")
 
-    @context.setter
-    def context(self, value: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]):
-        pulumi.set(self, "context", value)
+    @clone_id.setter
+    def clone_id(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "clone_id", value)
 
     @property
     @pulumi.getter(name="controllerRequired")
     def controller_required(self) -> Optional[pulumi.Input[bool]]:
-        """
-        `(boolean)`
-        """
         return pulumi.get(self, "controller_required")
 
     @controller_required.setter
     def controller_required(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "controller_required", value)
 
     @property
     @pulumi.getter(name="controllersExpected")
     def controllers_expected(self) -> Optional[pulumi.Input[int]]:
-        """
-        `(integer)`
-        """
         return pulumi.get(self, "controllers_expected")
 
     @controllers_expected.setter
     def controllers_expected(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "controllers_expected", value)
 
     @property
     @pulumi.getter(name="controllersHealthy")
     def controllers_healthy(self) -> Optional[pulumi.Input[int]]:
-        """
-        `(integer)`
-        """
         return pulumi.get(self, "controllers_healthy")
 
     @controllers_healthy.setter
     def controllers_healthy(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "controllers_healthy", value)
 
     @property
-    @pulumi.getter(name="deregisterOnDestroy")
-    def deregister_on_destroy(self) -> Optional[pulumi.Input[bool]]:
-        """
-        `(boolean: true)` - If true, the volume will be deregistered on destroy.
-        """
-        return pulumi.get(self, "deregister_on_destroy")
-
-    @deregister_on_destroy.setter
-    def deregister_on_destroy(self, value: Optional[pulumi.Input[bool]]):
-        pulumi.set(self, "deregister_on_destroy", value)
-
-    @property
-    @pulumi.getter(name="externalId")
-    def external_id(self) -> Optional[pulumi.Input[str]]:
-        """
-        `(string: <required>)` - The ID of the physical volume from the storage provider.
-        """
-        return pulumi.get(self, "external_id")
-
-    @external_id.setter
-    def external_id(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "external_id", value)
-
-    @property
     @pulumi.getter(name="mountOptions")
-    def mount_options(self) -> Optional[pulumi.Input['CsiVolumeRegistrationMountOptionsArgs']]:
+    def mount_options(self) -> Optional[pulumi.Input['ExternalVolumeMountOptionsArgs']]:
         """
-        `(block: <optional>)` Options for mounting `block-device` volumes without a pre-formatted file system.
+        `(block: optional)` Options for mounting `block-device` volumes without a pre-formatted file system.
         """
         return pulumi.get(self, "mount_options")
 
     @mount_options.setter
-    def mount_options(self, value: Optional[pulumi.Input['CsiVolumeRegistrationMountOptionsArgs']]):
+    def mount_options(self, value: Optional[pulumi.Input['ExternalVolumeMountOptionsArgs']]):
         pulumi.set(self, "mount_options", value)
 
     @property
     @pulumi.getter
     def name(self) -> Optional[pulumi.Input[str]]:
         """
         `(string: <required>)` - The display name for the volume.
@@ -520,40 +442,34 @@
     @namespace.setter
     def namespace(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "namespace", value)
 
     @property
     @pulumi.getter(name="nodesExpected")
     def nodes_expected(self) -> Optional[pulumi.Input[int]]:
-        """
-        `(integer)`
-        """
         return pulumi.get(self, "nodes_expected")
 
     @nodes_expected.setter
     def nodes_expected(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "nodes_expected", value)
 
     @property
     @pulumi.getter(name="nodesHealthy")
     def nodes_healthy(self) -> Optional[pulumi.Input[int]]:
-        """
-        `(integer)`
-        """
         return pulumi.get(self, "nodes_healthy")
 
     @nodes_healthy.setter
     def nodes_healthy(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "nodes_healthy", value)
 
     @property
     @pulumi.getter
     def parameters(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
         """
-        `(map[string]string: <optional>)` - An optional key-value map of strings passed directly to the CSI plugin to configure the volume.
+        `(map[string]string: optional)` An optional key-value map of strings passed directly to the CSI plugin to configure the volume.
         """
         return pulumi.get(self, "parameters")
 
     @parameters.setter
     def parameters(self, value: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]):
         pulumi.set(self, "parameters", value)
 
@@ -568,406 +484,448 @@
     @plugin_id.setter
     def plugin_id(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "plugin_id", value)
 
     @property
     @pulumi.getter(name="pluginProvider")
     def plugin_provider(self) -> Optional[pulumi.Input[str]]:
-        """
-        `(string)`
-        """
         return pulumi.get(self, "plugin_provider")
 
     @plugin_provider.setter
     def plugin_provider(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "plugin_provider", value)
 
     @property
     @pulumi.getter(name="pluginProviderVersion")
     def plugin_provider_version(self) -> Optional[pulumi.Input[str]]:
-        """
-        `(string)`
-        """
         return pulumi.get(self, "plugin_provider_version")
 
     @plugin_provider_version.setter
     def plugin_provider_version(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "plugin_provider_version", value)
 
     @property
     @pulumi.getter
     def schedulable(self) -> Optional[pulumi.Input[bool]]:
-        """
-        `(boolean)`
-        """
         return pulumi.get(self, "schedulable")
 
     @schedulable.setter
     def schedulable(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "schedulable", value)
 
     @property
     @pulumi.getter
     def secrets(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
         """
-        `(map[string]string: <optional>)` - An optional key-value map of strings used as credentials for publishing and unpublishing volumes.
+        `(map[string]string: optional)` An optional key-value map of strings used as credentials for publishing and unpublishing volumes.
         """
         return pulumi.get(self, "secrets")
 
     @secrets.setter
     def secrets(self, value: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]):
         pulumi.set(self, "secrets", value)
 
     @property
-    @pulumi.getter
-    def topologies(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['CsiVolumeRegistrationTopologyArgs']]]]:
+    @pulumi.getter(name="snapshotId")
+    def snapshot_id(self) -> Optional[pulumi.Input[str]]:
         """
-        `(List of topologies)`
+        `(string: <optional>)` - The external ID of a snapshot to restore. If ommited, the volume will be created from scratch. Conflicts with `clone_id`.
         """
+        return pulumi.get(self, "snapshot_id")
+
+    @snapshot_id.setter
+    def snapshot_id(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "snapshot_id", value)
+
+    @property
+    @pulumi.getter
+    def topologies(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['ExternalVolumeTopologyArgs']]]]:
         return pulumi.get(self, "topologies")
 
     @topologies.setter
-    def topologies(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['CsiVolumeRegistrationTopologyArgs']]]]):
+    def topologies(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['ExternalVolumeTopologyArgs']]]]):
         pulumi.set(self, "topologies", value)
 
     @property
     @pulumi.getter(name="topologyRequest")
-    def topology_request(self) -> Optional[pulumi.Input['CsiVolumeRegistrationTopologyRequestArgs']]:
+    def topology_request(self) -> Optional[pulumi.Input['ExternalVolumeTopologyRequestArgs']]:
         """
         `(``TopologyRequest``: <optional>)` - Specify locations (region, zone, rack, etc.) where the provisioned volume is accessible from.
         """
         return pulumi.get(self, "topology_request")
 
     @topology_request.setter
-    def topology_request(self, value: Optional[pulumi.Input['CsiVolumeRegistrationTopologyRequestArgs']]):
+    def topology_request(self, value: Optional[pulumi.Input['ExternalVolumeTopologyRequestArgs']]):
         pulumi.set(self, "topology_request", value)
 
     @property
+    @pulumi.getter
+    def type(self) -> Optional[pulumi.Input[str]]:
+        """
+        `(string: <required>)` - The type of the volume. Currently, only `csi` is supported.
+        """
+        return pulumi.get(self, "type")
+
+    @type.setter
+    def type(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "type", value)
+
+    @property
     @pulumi.getter(name="volumeId")
     def volume_id(self) -> Optional[pulumi.Input[str]]:
         """
         `(string: <required>)` - The unique ID of the volume.
         """
         return pulumi.get(self, "volume_id")
 
     @volume_id.setter
     def volume_id(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "volume_id", value)
 
 
-class CsiVolumeRegistration(pulumi.CustomResource):
+class ExternalVolume(pulumi.CustomResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
-                 capabilities: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['CsiVolumeRegistrationCapabilityArgs']]]]] = None,
+                 capabilities: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ExternalVolumeCapabilityArgs']]]]] = None,
                  capacity_max: Optional[pulumi.Input[str]] = None,
                  capacity_min: Optional[pulumi.Input[str]] = None,
-                 context: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
-                 deregister_on_destroy: Optional[pulumi.Input[bool]] = None,
-                 external_id: Optional[pulumi.Input[str]] = None,
-                 mount_options: Optional[pulumi.Input[pulumi.InputType['CsiVolumeRegistrationMountOptionsArgs']]] = None,
+                 clone_id: Optional[pulumi.Input[str]] = None,
+                 mount_options: Optional[pulumi.Input[pulumi.InputType['ExternalVolumeMountOptionsArgs']]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  namespace: Optional[pulumi.Input[str]] = None,
                  parameters: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  plugin_id: Optional[pulumi.Input[str]] = None,
                  secrets: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
-                 topology_request: Optional[pulumi.Input[pulumi.InputType['CsiVolumeRegistrationTopologyRequestArgs']]] = None,
+                 snapshot_id: Optional[pulumi.Input[str]] = None,
+                 topology_request: Optional[pulumi.Input[pulumi.InputType['ExternalVolumeTopologyRequestArgs']]] = None,
+                 type: Optional[pulumi.Input[str]] = None,
                  volume_id: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
-        Create a CsiVolumeRegistration resource with the given unique name, props, and options.
+        ## Example Usage
+
+        Creating a volume:
+
+        ```python
+        import pulumi
+        import pulumi_nomad as nomad
+
+        # It can sometimes be helpful to wait for a particular plugin to be available
+        ebs = nomad.get_plugin(plugin_id="aws-ebs0",
+            wait_for_healthy=True)
+        mysql_volume = nomad.ExternalVolume("mysql_volume",
+            type="csi",
+            plugin_id="aws-ebs0",
+            volume_id="mysql_volume",
+            name="mysql_volume",
+            capacity_min="10GiB",
+            capacity_max="20GiB",
+            capabilities=[nomad.ExternalVolumeCapabilityArgs(
+                access_mode="single-node-writer",
+                attachment_mode="file-system",
+            )],
+            mount_options=nomad.ExternalVolumeMountOptionsArgs(
+                fs_type="ext4",
+            ),
+            topology_request=nomad.ExternalVolumeTopologyRequestArgs(
+                required=nomad.ExternalVolumeTopologyRequestRequiredArgs(
+                    topologies=[
+                        nomad.ExternalVolumeTopologyRequestRequiredTopologyArgs(
+                            segments={
+                                "rack": "R1",
+                                "zone": "us-east-1a",
+                            },
+                        ),
+                        nomad.ExternalVolumeTopologyRequestRequiredTopologyArgs(
+                            segments={
+                                "rack": "R2",
+                            },
+                        ),
+                    ],
+                ),
+            ),
+            opts=pulumi.ResourceOptions(depends_on=[ebs]))
+        ```
+
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['CsiVolumeRegistrationCapabilityArgs']]]] capabilities: `(``Capability``: <required>)` - Options for validating the capability of a volume.
+        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ExternalVolumeCapabilityArgs']]]] capabilities: `(``Capability``: <required>)` - Options for validating the capability of a volume.
         :param pulumi.Input[str] capacity_max: `(string: <optional>)` - Option to signal a maximum volume size. This may not be supported by all storage providers.
         :param pulumi.Input[str] capacity_min: `(string: <optional>)` - Option to signal a minimum volume size. This may not be supported by all storage providers.
-        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] context: `(map[string]string: <optional>)` - An optional key-value map of strings passed directly to the CSI plugin to validate the volume.
-        :param pulumi.Input[bool] deregister_on_destroy: `(boolean: true)` - If true, the volume will be deregistered on destroy.
-        :param pulumi.Input[str] external_id: `(string: <required>)` - The ID of the physical volume from the storage provider.
-        :param pulumi.Input[pulumi.InputType['CsiVolumeRegistrationMountOptionsArgs']] mount_options: `(block: <optional>)` Options for mounting `block-device` volumes without a pre-formatted file system.
+        :param pulumi.Input[str] clone_id: `(string: <optional>)` - The external ID of an existing volume to restore. If ommited, the volume will be created from scratch. Conflicts with `snapshot_id`.
+        :param pulumi.Input[pulumi.InputType['ExternalVolumeMountOptionsArgs']] mount_options: `(block: optional)` Options for mounting `block-device` volumes without a pre-formatted file system.
         :param pulumi.Input[str] name: `(string: <required>)` - The display name for the volume.
         :param pulumi.Input[str] namespace: `(string: "default")` - The namespace in which to register the volume.
-        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] parameters: `(map[string]string: <optional>)` - An optional key-value map of strings passed directly to the CSI plugin to configure the volume.
+        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] parameters: `(map[string]string: optional)` An optional key-value map of strings passed directly to the CSI plugin to configure the volume.
         :param pulumi.Input[str] plugin_id: `(string: <required>)` - The ID of the Nomad plugin for registering this volume.
-        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] secrets: `(map[string]string: <optional>)` - An optional key-value map of strings used as credentials for publishing and unpublishing volumes.
-        :param pulumi.Input[pulumi.InputType['CsiVolumeRegistrationTopologyRequestArgs']] topology_request: `(``TopologyRequest``: <optional>)` - Specify locations (region, zone, rack, etc.) where the provisioned volume is accessible from.
+        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] secrets: `(map[string]string: optional)` An optional key-value map of strings used as credentials for publishing and unpublishing volumes.
+        :param pulumi.Input[str] snapshot_id: `(string: <optional>)` - The external ID of a snapshot to restore. If ommited, the volume will be created from scratch. Conflicts with `clone_id`.
+        :param pulumi.Input[pulumi.InputType['ExternalVolumeTopologyRequestArgs']] topology_request: `(``TopologyRequest``: <optional>)` - Specify locations (region, zone, rack, etc.) where the provisioned volume is accessible from.
+        :param pulumi.Input[str] type: `(string: <required>)` - The type of the volume. Currently, only `csi` is supported.
         :param pulumi.Input[str] volume_id: `(string: <required>)` - The unique ID of the volume.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
-                 args: CsiVolumeRegistrationArgs,
+                 args: ExternalVolumeArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
-        Create a CsiVolumeRegistration resource with the given unique name, props, and options.
+        ## Example Usage
+
+        Creating a volume:
+
+        ```python
+        import pulumi
+        import pulumi_nomad as nomad
+
+        # It can sometimes be helpful to wait for a particular plugin to be available
+        ebs = nomad.get_plugin(plugin_id="aws-ebs0",
+            wait_for_healthy=True)
+        mysql_volume = nomad.ExternalVolume("mysql_volume",
+            type="csi",
+            plugin_id="aws-ebs0",
+            volume_id="mysql_volume",
+            name="mysql_volume",
+            capacity_min="10GiB",
+            capacity_max="20GiB",
+            capabilities=[nomad.ExternalVolumeCapabilityArgs(
+                access_mode="single-node-writer",
+                attachment_mode="file-system",
+            )],
+            mount_options=nomad.ExternalVolumeMountOptionsArgs(
+                fs_type="ext4",
+            ),
+            topology_request=nomad.ExternalVolumeTopologyRequestArgs(
+                required=nomad.ExternalVolumeTopologyRequestRequiredArgs(
+                    topologies=[
+                        nomad.ExternalVolumeTopologyRequestRequiredTopologyArgs(
+                            segments={
+                                "rack": "R1",
+                                "zone": "us-east-1a",
+                            },
+                        ),
+                        nomad.ExternalVolumeTopologyRequestRequiredTopologyArgs(
+                            segments={
+                                "rack": "R2",
+                            },
+                        ),
+                    ],
+                ),
+            ),
+            opts=pulumi.ResourceOptions(depends_on=[ebs]))
+        ```
+
         :param str resource_name: The name of the resource.
-        :param CsiVolumeRegistrationArgs args: The arguments to use to populate this resource's properties.
+        :param ExternalVolumeArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
-        resource_args, opts = _utilities.get_resource_args_opts(CsiVolumeRegistrationArgs, pulumi.ResourceOptions, *args, **kwargs)
+        resource_args, opts = _utilities.get_resource_args_opts(ExternalVolumeArgs, pulumi.ResourceOptions, *args, **kwargs)
         if resource_args is not None:
             __self__._internal_init(resource_name, opts, **resource_args.__dict__)
         else:
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
-                 capabilities: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['CsiVolumeRegistrationCapabilityArgs']]]]] = None,
+                 capabilities: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ExternalVolumeCapabilityArgs']]]]] = None,
                  capacity_max: Optional[pulumi.Input[str]] = None,
                  capacity_min: Optional[pulumi.Input[str]] = None,
-                 context: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
-                 deregister_on_destroy: Optional[pulumi.Input[bool]] = None,
-                 external_id: Optional[pulumi.Input[str]] = None,
-                 mount_options: Optional[pulumi.Input[pulumi.InputType['CsiVolumeRegistrationMountOptionsArgs']]] = None,
+                 clone_id: Optional[pulumi.Input[str]] = None,
+                 mount_options: Optional[pulumi.Input[pulumi.InputType['ExternalVolumeMountOptionsArgs']]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  namespace: Optional[pulumi.Input[str]] = None,
                  parameters: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  plugin_id: Optional[pulumi.Input[str]] = None,
                  secrets: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
-                 topology_request: Optional[pulumi.Input[pulumi.InputType['CsiVolumeRegistrationTopologyRequestArgs']]] = None,
+                 snapshot_id: Optional[pulumi.Input[str]] = None,
+                 topology_request: Optional[pulumi.Input[pulumi.InputType['ExternalVolumeTopologyRequestArgs']]] = None,
+                 type: Optional[pulumi.Input[str]] = None,
                  volume_id: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
-            __props__ = CsiVolumeRegistrationArgs.__new__(CsiVolumeRegistrationArgs)
+            __props__ = ExternalVolumeArgs.__new__(ExternalVolumeArgs)
 
+            if capabilities is None and not opts.urn:
+                raise TypeError("Missing required property 'capabilities'")
             __props__.__dict__["capabilities"] = capabilities
             __props__.__dict__["capacity_max"] = capacity_max
             __props__.__dict__["capacity_min"] = capacity_min
-            __props__.__dict__["context"] = context
-            __props__.__dict__["deregister_on_destroy"] = deregister_on_destroy
-            if external_id is None and not opts.urn:
-                raise TypeError("Missing required property 'external_id'")
-            __props__.__dict__["external_id"] = external_id
+            __props__.__dict__["clone_id"] = clone_id
             __props__.__dict__["mount_options"] = mount_options
             __props__.__dict__["name"] = name
             __props__.__dict__["namespace"] = namespace
             __props__.__dict__["parameters"] = parameters
             if plugin_id is None and not opts.urn:
                 raise TypeError("Missing required property 'plugin_id'")
             __props__.__dict__["plugin_id"] = plugin_id
             __props__.__dict__["secrets"] = None if secrets is None else pulumi.Output.secret(secrets)
+            __props__.__dict__["snapshot_id"] = snapshot_id
             __props__.__dict__["topology_request"] = topology_request
+            __props__.__dict__["type"] = type
             if volume_id is None and not opts.urn:
                 raise TypeError("Missing required property 'volume_id'")
             __props__.__dict__["volume_id"] = volume_id
-            __props__.__dict__["capacity"] = None
-            __props__.__dict__["capacity_max_bytes"] = None
-            __props__.__dict__["capacity_min_bytes"] = None
             __props__.__dict__["controller_required"] = None
             __props__.__dict__["controllers_expected"] = None
             __props__.__dict__["controllers_healthy"] = None
             __props__.__dict__["nodes_expected"] = None
             __props__.__dict__["nodes_healthy"] = None
             __props__.__dict__["plugin_provider"] = None
             __props__.__dict__["plugin_provider_version"] = None
             __props__.__dict__["schedulable"] = None
             __props__.__dict__["topologies"] = None
         secret_opts = pulumi.ResourceOptions(additional_secret_outputs=["secrets"])
         opts = pulumi.ResourceOptions.merge(opts, secret_opts)
-        super(CsiVolumeRegistration, __self__).__init__(
-            'nomad:index/csiVolumeRegistration:CsiVolumeRegistration',
+        super(ExternalVolume, __self__).__init__(
+            'nomad:index/externalVolume:ExternalVolume',
             resource_name,
             __props__,
             opts)
 
     @staticmethod
     def get(resource_name: str,
             id: pulumi.Input[str],
             opts: Optional[pulumi.ResourceOptions] = None,
-            capabilities: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['CsiVolumeRegistrationCapabilityArgs']]]]] = None,
-            capacity: Optional[pulumi.Input[int]] = None,
+            capabilities: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ExternalVolumeCapabilityArgs']]]]] = None,
             capacity_max: Optional[pulumi.Input[str]] = None,
-            capacity_max_bytes: Optional[pulumi.Input[int]] = None,
             capacity_min: Optional[pulumi.Input[str]] = None,
-            capacity_min_bytes: Optional[pulumi.Input[int]] = None,
-            context: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
+            clone_id: Optional[pulumi.Input[str]] = None,
             controller_required: Optional[pulumi.Input[bool]] = None,
             controllers_expected: Optional[pulumi.Input[int]] = None,
             controllers_healthy: Optional[pulumi.Input[int]] = None,
-            deregister_on_destroy: Optional[pulumi.Input[bool]] = None,
-            external_id: Optional[pulumi.Input[str]] = None,
-            mount_options: Optional[pulumi.Input[pulumi.InputType['CsiVolumeRegistrationMountOptionsArgs']]] = None,
+            mount_options: Optional[pulumi.Input[pulumi.InputType['ExternalVolumeMountOptionsArgs']]] = None,
             name: Optional[pulumi.Input[str]] = None,
             namespace: Optional[pulumi.Input[str]] = None,
             nodes_expected: Optional[pulumi.Input[int]] = None,
             nodes_healthy: Optional[pulumi.Input[int]] = None,
             parameters: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
             plugin_id: Optional[pulumi.Input[str]] = None,
             plugin_provider: Optional[pulumi.Input[str]] = None,
             plugin_provider_version: Optional[pulumi.Input[str]] = None,
             schedulable: Optional[pulumi.Input[bool]] = None,
             secrets: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
-            topologies: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['CsiVolumeRegistrationTopologyArgs']]]]] = None,
-            topology_request: Optional[pulumi.Input[pulumi.InputType['CsiVolumeRegistrationTopologyRequestArgs']]] = None,
-            volume_id: Optional[pulumi.Input[str]] = None) -> 'CsiVolumeRegistration':
+            snapshot_id: Optional[pulumi.Input[str]] = None,
+            topologies: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ExternalVolumeTopologyArgs']]]]] = None,
+            topology_request: Optional[pulumi.Input[pulumi.InputType['ExternalVolumeTopologyRequestArgs']]] = None,
+            type: Optional[pulumi.Input[str]] = None,
+            volume_id: Optional[pulumi.Input[str]] = None) -> 'ExternalVolume':
         """
-        Get an existing CsiVolumeRegistration resource's state with the given name, id, and optional extra
+        Get an existing ExternalVolume resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['CsiVolumeRegistrationCapabilityArgs']]]] capabilities: `(``Capability``: <required>)` - Options for validating the capability of a volume.
+        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ExternalVolumeCapabilityArgs']]]] capabilities: `(``Capability``: <required>)` - Options for validating the capability of a volume.
         :param pulumi.Input[str] capacity_max: `(string: <optional>)` - Option to signal a maximum volume size. This may not be supported by all storage providers.
         :param pulumi.Input[str] capacity_min: `(string: <optional>)` - Option to signal a minimum volume size. This may not be supported by all storage providers.
-        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] context: `(map[string]string: <optional>)` - An optional key-value map of strings passed directly to the CSI plugin to validate the volume.
-        :param pulumi.Input[bool] controller_required: `(boolean)`
-        :param pulumi.Input[int] controllers_expected: `(integer)`
-        :param pulumi.Input[int] controllers_healthy: `(integer)`
-        :param pulumi.Input[bool] deregister_on_destroy: `(boolean: true)` - If true, the volume will be deregistered on destroy.
-        :param pulumi.Input[str] external_id: `(string: <required>)` - The ID of the physical volume from the storage provider.
-        :param pulumi.Input[pulumi.InputType['CsiVolumeRegistrationMountOptionsArgs']] mount_options: `(block: <optional>)` Options for mounting `block-device` volumes without a pre-formatted file system.
+        :param pulumi.Input[str] clone_id: `(string: <optional>)` - The external ID of an existing volume to restore. If ommited, the volume will be created from scratch. Conflicts with `snapshot_id`.
+        :param pulumi.Input[pulumi.InputType['ExternalVolumeMountOptionsArgs']] mount_options: `(block: optional)` Options for mounting `block-device` volumes without a pre-formatted file system.
         :param pulumi.Input[str] name: `(string: <required>)` - The display name for the volume.
         :param pulumi.Input[str] namespace: `(string: "default")` - The namespace in which to register the volume.
-        :param pulumi.Input[int] nodes_expected: `(integer)`
-        :param pulumi.Input[int] nodes_healthy: `(integer)`
-        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] parameters: `(map[string]string: <optional>)` - An optional key-value map of strings passed directly to the CSI plugin to configure the volume.
+        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] parameters: `(map[string]string: optional)` An optional key-value map of strings passed directly to the CSI plugin to configure the volume.
         :param pulumi.Input[str] plugin_id: `(string: <required>)` - The ID of the Nomad plugin for registering this volume.
-        :param pulumi.Input[str] plugin_provider: `(string)`
-        :param pulumi.Input[str] plugin_provider_version: `(string)`
-        :param pulumi.Input[bool] schedulable: `(boolean)`
-        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] secrets: `(map[string]string: <optional>)` - An optional key-value map of strings used as credentials for publishing and unpublishing volumes.
-        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['CsiVolumeRegistrationTopologyArgs']]]] topologies: `(List of topologies)`
-        :param pulumi.Input[pulumi.InputType['CsiVolumeRegistrationTopologyRequestArgs']] topology_request: `(``TopologyRequest``: <optional>)` - Specify locations (region, zone, rack, etc.) where the provisioned volume is accessible from.
+        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] secrets: `(map[string]string: optional)` An optional key-value map of strings used as credentials for publishing and unpublishing volumes.
+        :param pulumi.Input[str] snapshot_id: `(string: <optional>)` - The external ID of a snapshot to restore. If ommited, the volume will be created from scratch. Conflicts with `clone_id`.
+        :param pulumi.Input[pulumi.InputType['ExternalVolumeTopologyRequestArgs']] topology_request: `(``TopologyRequest``: <optional>)` - Specify locations (region, zone, rack, etc.) where the provisioned volume is accessible from.
+        :param pulumi.Input[str] type: `(string: <required>)` - The type of the volume. Currently, only `csi` is supported.
         :param pulumi.Input[str] volume_id: `(string: <required>)` - The unique ID of the volume.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
-        __props__ = _CsiVolumeRegistrationState.__new__(_CsiVolumeRegistrationState)
+        __props__ = _ExternalVolumeState.__new__(_ExternalVolumeState)
 
         __props__.__dict__["capabilities"] = capabilities
-        __props__.__dict__["capacity"] = capacity
         __props__.__dict__["capacity_max"] = capacity_max
-        __props__.__dict__["capacity_max_bytes"] = capacity_max_bytes
         __props__.__dict__["capacity_min"] = capacity_min
-        __props__.__dict__["capacity_min_bytes"] = capacity_min_bytes
-        __props__.__dict__["context"] = context
+        __props__.__dict__["clone_id"] = clone_id
         __props__.__dict__["controller_required"] = controller_required
         __props__.__dict__["controllers_expected"] = controllers_expected
         __props__.__dict__["controllers_healthy"] = controllers_healthy
-        __props__.__dict__["deregister_on_destroy"] = deregister_on_destroy
-        __props__.__dict__["external_id"] = external_id
         __props__.__dict__["mount_options"] = mount_options
         __props__.__dict__["name"] = name
         __props__.__dict__["namespace"] = namespace
         __props__.__dict__["nodes_expected"] = nodes_expected
         __props__.__dict__["nodes_healthy"] = nodes_healthy
         __props__.__dict__["parameters"] = parameters
         __props__.__dict__["plugin_id"] = plugin_id
         __props__.__dict__["plugin_provider"] = plugin_provider
         __props__.__dict__["plugin_provider_version"] = plugin_provider_version
         __props__.__dict__["schedulable"] = schedulable
         __props__.__dict__["secrets"] = secrets
+        __props__.__dict__["snapshot_id"] = snapshot_id
         __props__.__dict__["topologies"] = topologies
         __props__.__dict__["topology_request"] = topology_request
+        __props__.__dict__["type"] = type
         __props__.__dict__["volume_id"] = volume_id
-        return CsiVolumeRegistration(resource_name, opts=opts, __props__=__props__)
+        return ExternalVolume(resource_name, opts=opts, __props__=__props__)
 
     @property
     @pulumi.getter
-    def capabilities(self) -> pulumi.Output[Optional[Sequence['outputs.CsiVolumeRegistrationCapability']]]:
+    def capabilities(self) -> pulumi.Output[Sequence['outputs.ExternalVolumeCapability']]:
         """
         `(``Capability``: <required>)` - Options for validating the capability of a volume.
         """
         return pulumi.get(self, "capabilities")
 
     @property
-    @pulumi.getter
-    def capacity(self) -> pulumi.Output[int]:
-        return pulumi.get(self, "capacity")
-
-    @property
     @pulumi.getter(name="capacityMax")
     def capacity_max(self) -> pulumi.Output[Optional[str]]:
         """
         `(string: <optional>)` - Option to signal a maximum volume size. This may not be supported by all storage providers.
         """
         return pulumi.get(self, "capacity_max")
 
     @property
-    @pulumi.getter(name="capacityMaxBytes")
-    def capacity_max_bytes(self) -> pulumi.Output[int]:
-        return pulumi.get(self, "capacity_max_bytes")
-
-    @property
     @pulumi.getter(name="capacityMin")
     def capacity_min(self) -> pulumi.Output[Optional[str]]:
         """
         `(string: <optional>)` - Option to signal a minimum volume size. This may not be supported by all storage providers.
         """
         return pulumi.get(self, "capacity_min")
 
     @property
-    @pulumi.getter(name="capacityMinBytes")
-    def capacity_min_bytes(self) -> pulumi.Output[int]:
-        return pulumi.get(self, "capacity_min_bytes")
-
-    @property
-    @pulumi.getter
-    def context(self) -> pulumi.Output[Optional[Mapping[str, str]]]:
+    @pulumi.getter(name="cloneId")
+    def clone_id(self) -> pulumi.Output[Optional[str]]:
         """
-        `(map[string]string: <optional>)` - An optional key-value map of strings passed directly to the CSI plugin to validate the volume.
+        `(string: <optional>)` - The external ID of an existing volume to restore. If ommited, the volume will be created from scratch. Conflicts with `snapshot_id`.
         """
-        return pulumi.get(self, "context")
+        return pulumi.get(self, "clone_id")
 
     @property
     @pulumi.getter(name="controllerRequired")
     def controller_required(self) -> pulumi.Output[bool]:
-        """
-        `(boolean)`
-        """
         return pulumi.get(self, "controller_required")
 
     @property
     @pulumi.getter(name="controllersExpected")
     def controllers_expected(self) -> pulumi.Output[int]:
-        """
-        `(integer)`
-        """
         return pulumi.get(self, "controllers_expected")
 
     @property
     @pulumi.getter(name="controllersHealthy")
     def controllers_healthy(self) -> pulumi.Output[int]:
-        """
-        `(integer)`
-        """
         return pulumi.get(self, "controllers_healthy")
 
     @property
-    @pulumi.getter(name="deregisterOnDestroy")
-    def deregister_on_destroy(self) -> pulumi.Output[Optional[bool]]:
-        """
-        `(boolean: true)` - If true, the volume will be deregistered on destroy.
-        """
-        return pulumi.get(self, "deregister_on_destroy")
-
-    @property
-    @pulumi.getter(name="externalId")
-    def external_id(self) -> pulumi.Output[str]:
-        """
-        `(string: <required>)` - The ID of the physical volume from the storage provider.
-        """
-        return pulumi.get(self, "external_id")
-
-    @property
     @pulumi.getter(name="mountOptions")
-    def mount_options(self) -> pulumi.Output[Optional['outputs.CsiVolumeRegistrationMountOptions']]:
+    def mount_options(self) -> pulumi.Output[Optional['outputs.ExternalVolumeMountOptions']]:
         """
-        `(block: <optional>)` Options for mounting `block-device` volumes without a pre-formatted file system.
+        `(block: optional)` Options for mounting `block-device` volumes without a pre-formatted file system.
         """
         return pulumi.get(self, "mount_options")
 
     @property
     @pulumi.getter
     def name(self) -> pulumi.Output[str]:
         """
@@ -982,92 +940,90 @@
         `(string: "default")` - The namespace in which to register the volume.
         """
         return pulumi.get(self, "namespace")
 
     @property
     @pulumi.getter(name="nodesExpected")
     def nodes_expected(self) -> pulumi.Output[int]:
-        """
-        `(integer)`
-        """
         return pulumi.get(self, "nodes_expected")
 
     @property
     @pulumi.getter(name="nodesHealthy")
     def nodes_healthy(self) -> pulumi.Output[int]:
-        """
-        `(integer)`
-        """
         return pulumi.get(self, "nodes_healthy")
 
     @property
     @pulumi.getter
     def parameters(self) -> pulumi.Output[Optional[Mapping[str, str]]]:
         """
-        `(map[string]string: <optional>)` - An optional key-value map of strings passed directly to the CSI plugin to configure the volume.
+        `(map[string]string: optional)` An optional key-value map of strings passed directly to the CSI plugin to configure the volume.
         """
         return pulumi.get(self, "parameters")
 
     @property
     @pulumi.getter(name="pluginId")
     def plugin_id(self) -> pulumi.Output[str]:
         """
         `(string: <required>)` - The ID of the Nomad plugin for registering this volume.
         """
         return pulumi.get(self, "plugin_id")
 
     @property
     @pulumi.getter(name="pluginProvider")
     def plugin_provider(self) -> pulumi.Output[str]:
-        """
-        `(string)`
-        """
         return pulumi.get(self, "plugin_provider")
 
     @property
     @pulumi.getter(name="pluginProviderVersion")
     def plugin_provider_version(self) -> pulumi.Output[str]:
-        """
-        `(string)`
-        """
         return pulumi.get(self, "plugin_provider_version")
 
     @property
     @pulumi.getter
     def schedulable(self) -> pulumi.Output[bool]:
-        """
-        `(boolean)`
-        """
         return pulumi.get(self, "schedulable")
 
     @property
     @pulumi.getter
     def secrets(self) -> pulumi.Output[Optional[Mapping[str, str]]]:
         """
-        `(map[string]string: <optional>)` - An optional key-value map of strings used as credentials for publishing and unpublishing volumes.
+        `(map[string]string: optional)` An optional key-value map of strings used as credentials for publishing and unpublishing volumes.
         """
         return pulumi.get(self, "secrets")
 
     @property
-    @pulumi.getter
-    def topologies(self) -> pulumi.Output[Sequence['outputs.CsiVolumeRegistrationTopology']]:
+    @pulumi.getter(name="snapshotId")
+    def snapshot_id(self) -> pulumi.Output[Optional[str]]:
         """
-        `(List of topologies)`
+        `(string: <optional>)` - The external ID of a snapshot to restore. If ommited, the volume will be created from scratch. Conflicts with `clone_id`.
         """
+        return pulumi.get(self, "snapshot_id")
+
+    @property
+    @pulumi.getter
+    def topologies(self) -> pulumi.Output[Sequence['outputs.ExternalVolumeTopology']]:
         return pulumi.get(self, "topologies")
 
     @property
     @pulumi.getter(name="topologyRequest")
-    def topology_request(self) -> pulumi.Output[Optional['outputs.CsiVolumeRegistrationTopologyRequest']]:
+    def topology_request(self) -> pulumi.Output[Optional['outputs.ExternalVolumeTopologyRequest']]:
         """
         `(``TopologyRequest``: <optional>)` - Specify locations (region, zone, rack, etc.) where the provisioned volume is accessible from.
         """
         return pulumi.get(self, "topology_request")
 
     @property
+    @pulumi.getter
+    def type(self) -> pulumi.Output[Optional[str]]:
+        """
+        `(string: <required>)` - The type of the volume. Currently, only `csi` is supported.
+        """
+        return pulumi.get(self, "type")
+
+    @property
     @pulumi.getter(name="volumeId")
     def volume_id(self) -> pulumi.Output[str]:
         """
         `(string: <required>)` - The unique ID of the volume.
         """
         return pulumi.get(self, "volume_id")
```

### Comparing `pulumi_nomad-2.3.0a1713561631/pulumi_nomad/external_volume.py` & `pulumi_nomad-2.3.0a1713899842/pulumi_nomad/csi_volume.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,49 +7,47 @@
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 from . import outputs
 from ._inputs import *
 
-__all__ = ['ExternalVolumeArgs', 'ExternalVolume']
+__all__ = ['CsiVolumeArgs', 'CsiVolume']
 
 @pulumi.input_type
-class ExternalVolumeArgs:
+class CsiVolumeArgs:
     def __init__(__self__, *,
-                 capabilities: pulumi.Input[Sequence[pulumi.Input['ExternalVolumeCapabilityArgs']]],
+                 capabilities: pulumi.Input[Sequence[pulumi.Input['CsiVolumeCapabilityArgs']]],
                  plugin_id: pulumi.Input[str],
                  volume_id: pulumi.Input[str],
                  capacity_max: Optional[pulumi.Input[str]] = None,
                  capacity_min: Optional[pulumi.Input[str]] = None,
                  clone_id: Optional[pulumi.Input[str]] = None,
-                 mount_options: Optional[pulumi.Input['ExternalVolumeMountOptionsArgs']] = None,
+                 mount_options: Optional[pulumi.Input['CsiVolumeMountOptionsArgs']] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  namespace: Optional[pulumi.Input[str]] = None,
                  parameters: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  secrets: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  snapshot_id: Optional[pulumi.Input[str]] = None,
-                 topology_request: Optional[pulumi.Input['ExternalVolumeTopologyRequestArgs']] = None,
-                 type: Optional[pulumi.Input[str]] = None):
+                 topology_request: Optional[pulumi.Input['CsiVolumeTopologyRequestArgs']] = None):
         """
-        The set of arguments for constructing a ExternalVolume resource.
-        :param pulumi.Input[Sequence[pulumi.Input['ExternalVolumeCapabilityArgs']]] capabilities: `(``Capability``: <required>)` - Options for validating the capability of a volume.
+        The set of arguments for constructing a CsiVolume resource.
+        :param pulumi.Input[Sequence[pulumi.Input['CsiVolumeCapabilityArgs']]] capabilities: `(``Capability``: <required>)` - Options for validating the capability of a volume.
         :param pulumi.Input[str] plugin_id: `(string: <required>)` - The ID of the Nomad plugin for registering this volume.
         :param pulumi.Input[str] volume_id: `(string: <required>)` - The unique ID of the volume.
         :param pulumi.Input[str] capacity_max: `(string: <optional>)` - Option to signal a maximum volume size. This may not be supported by all storage providers.
         :param pulumi.Input[str] capacity_min: `(string: <optional>)` - Option to signal a minimum volume size. This may not be supported by all storage providers.
         :param pulumi.Input[str] clone_id: `(string: <optional>)` - The external ID of an existing volume to restore. If ommited, the volume will be created from scratch. Conflicts with `snapshot_id`.
-        :param pulumi.Input['ExternalVolumeMountOptionsArgs'] mount_options: `(block: optional)` Options for mounting `block-device` volumes without a pre-formatted file system.
+        :param pulumi.Input['CsiVolumeMountOptionsArgs'] mount_options: `(block: optional)` Options for mounting `block-device` volumes without a pre-formatted file system.
         :param pulumi.Input[str] name: `(string: <required>)` - The display name for the volume.
         :param pulumi.Input[str] namespace: `(string: "default")` - The namespace in which to register the volume.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] parameters: `(map[string]string: optional)` An optional key-value map of strings passed directly to the CSI plugin to configure the volume.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] secrets: `(map[string]string: optional)` An optional key-value map of strings used as credentials for publishing and unpublishing volumes.
         :param pulumi.Input[str] snapshot_id: `(string: <optional>)` - The external ID of a snapshot to restore. If ommited, the volume will be created from scratch. Conflicts with `clone_id`.
-        :param pulumi.Input['ExternalVolumeTopologyRequestArgs'] topology_request: `(``TopologyRequest``: <optional>)` - Specify locations (region, zone, rack, etc.) where the provisioned volume is accessible from.
-        :param pulumi.Input[str] type: `(string: <required>)` - The type of the volume. Currently, only `csi` is supported.
+        :param pulumi.Input['CsiVolumeTopologyRequestArgs'] topology_request: `(``TopologyRequest``: <optional>)` - Specify locations (region, zone, rack, etc.) where the provisioned volume is accessible from.
         """
         pulumi.set(__self__, "capabilities", capabilities)
         pulumi.set(__self__, "plugin_id", plugin_id)
         pulumi.set(__self__, "volume_id", volume_id)
         if capacity_max is not None:
             pulumi.set(__self__, "capacity_max", capacity_max)
         if capacity_min is not None:
@@ -66,27 +64,25 @@
             pulumi.set(__self__, "parameters", parameters)
         if secrets is not None:
             pulumi.set(__self__, "secrets", secrets)
         if snapshot_id is not None:
             pulumi.set(__self__, "snapshot_id", snapshot_id)
         if topology_request is not None:
             pulumi.set(__self__, "topology_request", topology_request)
-        if type is not None:
-            pulumi.set(__self__, "type", type)
 
     @property
     @pulumi.getter
-    def capabilities(self) -> pulumi.Input[Sequence[pulumi.Input['ExternalVolumeCapabilityArgs']]]:
+    def capabilities(self) -> pulumi.Input[Sequence[pulumi.Input['CsiVolumeCapabilityArgs']]]:
         """
         `(``Capability``: <required>)` - Options for validating the capability of a volume.
         """
         return pulumi.get(self, "capabilities")
 
     @capabilities.setter
-    def capabilities(self, value: pulumi.Input[Sequence[pulumi.Input['ExternalVolumeCapabilityArgs']]]):
+    def capabilities(self, value: pulumi.Input[Sequence[pulumi.Input['CsiVolumeCapabilityArgs']]]):
         pulumi.set(self, "capabilities", value)
 
     @property
     @pulumi.getter(name="pluginId")
     def plugin_id(self) -> pulumi.Input[str]:
         """
         `(string: <required>)` - The ID of the Nomad plugin for registering this volume.
@@ -143,22 +139,22 @@
 
     @clone_id.setter
     def clone_id(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "clone_id", value)
 
     @property
     @pulumi.getter(name="mountOptions")
-    def mount_options(self) -> Optional[pulumi.Input['ExternalVolumeMountOptionsArgs']]:
+    def mount_options(self) -> Optional[pulumi.Input['CsiVolumeMountOptionsArgs']]:
         """
         `(block: optional)` Options for mounting `block-device` volumes without a pre-formatted file system.
         """
         return pulumi.get(self, "mount_options")
 
     @mount_options.setter
-    def mount_options(self, value: Optional[pulumi.Input['ExternalVolumeMountOptionsArgs']]):
+    def mount_options(self, value: Optional[pulumi.Input['CsiVolumeMountOptionsArgs']]):
         pulumi.set(self, "mount_options", value)
 
     @property
     @pulumi.getter
     def name(self) -> Optional[pulumi.Input[str]]:
         """
         `(string: <required>)` - The display name for the volume.
@@ -215,103 +211,93 @@
 
     @snapshot_id.setter
     def snapshot_id(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "snapshot_id", value)
 
     @property
     @pulumi.getter(name="topologyRequest")
-    def topology_request(self) -> Optional[pulumi.Input['ExternalVolumeTopologyRequestArgs']]:
+    def topology_request(self) -> Optional[pulumi.Input['CsiVolumeTopologyRequestArgs']]:
         """
         `(``TopologyRequest``: <optional>)` - Specify locations (region, zone, rack, etc.) where the provisioned volume is accessible from.
         """
         return pulumi.get(self, "topology_request")
 
     @topology_request.setter
-    def topology_request(self, value: Optional[pulumi.Input['ExternalVolumeTopologyRequestArgs']]):
+    def topology_request(self, value: Optional[pulumi.Input['CsiVolumeTopologyRequestArgs']]):
         pulumi.set(self, "topology_request", value)
 
-    @property
-    @pulumi.getter
-    def type(self) -> Optional[pulumi.Input[str]]:
-        """
-        `(string: <required>)` - The type of the volume. Currently, only `csi` is supported.
-        """
-        return pulumi.get(self, "type")
-
-    @type.setter
-    def type(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "type", value)
-
 
 @pulumi.input_type
-class _ExternalVolumeState:
+class _CsiVolumeState:
     def __init__(__self__, *,
-                 capabilities: Optional[pulumi.Input[Sequence[pulumi.Input['ExternalVolumeCapabilityArgs']]]] = None,
+                 capabilities: Optional[pulumi.Input[Sequence[pulumi.Input['CsiVolumeCapabilityArgs']]]] = None,
+                 capacity: Optional[pulumi.Input[int]] = None,
                  capacity_max: Optional[pulumi.Input[str]] = None,
+                 capacity_max_bytes: Optional[pulumi.Input[int]] = None,
                  capacity_min: Optional[pulumi.Input[str]] = None,
+                 capacity_min_bytes: Optional[pulumi.Input[int]] = None,
                  clone_id: Optional[pulumi.Input[str]] = None,
                  controller_required: Optional[pulumi.Input[bool]] = None,
                  controllers_expected: Optional[pulumi.Input[int]] = None,
                  controllers_healthy: Optional[pulumi.Input[int]] = None,
-                 mount_options: Optional[pulumi.Input['ExternalVolumeMountOptionsArgs']] = None,
+                 external_id: Optional[pulumi.Input[str]] = None,
+                 mount_options: Optional[pulumi.Input['CsiVolumeMountOptionsArgs']] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  namespace: Optional[pulumi.Input[str]] = None,
                  nodes_expected: Optional[pulumi.Input[int]] = None,
                  nodes_healthy: Optional[pulumi.Input[int]] = None,
                  parameters: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  plugin_id: Optional[pulumi.Input[str]] = None,
                  plugin_provider: Optional[pulumi.Input[str]] = None,
                  plugin_provider_version: Optional[pulumi.Input[str]] = None,
                  schedulable: Optional[pulumi.Input[bool]] = None,
                  secrets: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  snapshot_id: Optional[pulumi.Input[str]] = None,
-                 topologies: Optional[pulumi.Input[Sequence[pulumi.Input['ExternalVolumeTopologyArgs']]]] = None,
-                 topology_request: Optional[pulumi.Input['ExternalVolumeTopologyRequestArgs']] = None,
-                 type: Optional[pulumi.Input[str]] = None,
+                 topologies: Optional[pulumi.Input[Sequence[pulumi.Input['CsiVolumeTopologyArgs']]]] = None,
+                 topology_request: Optional[pulumi.Input['CsiVolumeTopologyRequestArgs']] = None,
                  volume_id: Optional[pulumi.Input[str]] = None):
         """
-        Input properties used for looking up and filtering ExternalVolume resources.
-        :param pulumi.Input[Sequence[pulumi.Input['ExternalVolumeCapabilityArgs']]] capabilities: `(``Capability``: <required>)` - Options for validating the capability of a volume.
+        Input properties used for looking up and filtering CsiVolume resources.
+        :param pulumi.Input[Sequence[pulumi.Input['CsiVolumeCapabilityArgs']]] capabilities: `(``Capability``: <required>)` - Options for validating the capability of a volume.
         :param pulumi.Input[str] capacity_max: `(string: <optional>)` - Option to signal a maximum volume size. This may not be supported by all storage providers.
         :param pulumi.Input[str] capacity_min: `(string: <optional>)` - Option to signal a minimum volume size. This may not be supported by all storage providers.
         :param pulumi.Input[str] clone_id: `(string: <optional>)` - The external ID of an existing volume to restore. If ommited, the volume will be created from scratch. Conflicts with `snapshot_id`.
-        :param pulumi.Input[bool] controller_required: `(boolean)`
-        :param pulumi.Input[int] controllers_expected: `(integer)`
-        :param pulumi.Input[int] controllers_healthy: `(integer)`
-        :param pulumi.Input['ExternalVolumeMountOptionsArgs'] mount_options: `(block: optional)` Options for mounting `block-device` volumes without a pre-formatted file system.
+        :param pulumi.Input[str] external_id: The ID of the physical volume from the storage provider.
+        :param pulumi.Input['CsiVolumeMountOptionsArgs'] mount_options: `(block: optional)` Options for mounting `block-device` volumes without a pre-formatted file system.
         :param pulumi.Input[str] name: `(string: <required>)` - The display name for the volume.
         :param pulumi.Input[str] namespace: `(string: "default")` - The namespace in which to register the volume.
-        :param pulumi.Input[int] nodes_expected: `(integer)`
-        :param pulumi.Input[int] nodes_healthy: `(integer)`
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] parameters: `(map[string]string: optional)` An optional key-value map of strings passed directly to the CSI plugin to configure the volume.
         :param pulumi.Input[str] plugin_id: `(string: <required>)` - The ID of the Nomad plugin for registering this volume.
-        :param pulumi.Input[str] plugin_provider: `(string)`
-        :param pulumi.Input[str] plugin_provider_version: `(string)`
-        :param pulumi.Input[bool] schedulable: `(boolean)`
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] secrets: `(map[string]string: optional)` An optional key-value map of strings used as credentials for publishing and unpublishing volumes.
         :param pulumi.Input[str] snapshot_id: `(string: <optional>)` - The external ID of a snapshot to restore. If ommited, the volume will be created from scratch. Conflicts with `clone_id`.
-        :param pulumi.Input[Sequence[pulumi.Input['ExternalVolumeTopologyArgs']]] topologies: `(List of topologies)`
-        :param pulumi.Input['ExternalVolumeTopologyRequestArgs'] topology_request: `(``TopologyRequest``: <optional>)` - Specify locations (region, zone, rack, etc.) where the provisioned volume is accessible from.
-        :param pulumi.Input[str] type: `(string: <required>)` - The type of the volume. Currently, only `csi` is supported.
+        :param pulumi.Input['CsiVolumeTopologyRequestArgs'] topology_request: `(``TopologyRequest``: <optional>)` - Specify locations (region, zone, rack, etc.) where the provisioned volume is accessible from.
         :param pulumi.Input[str] volume_id: `(string: <required>)` - The unique ID of the volume.
         """
         if capabilities is not None:
             pulumi.set(__self__, "capabilities", capabilities)
+        if capacity is not None:
+            pulumi.set(__self__, "capacity", capacity)
         if capacity_max is not None:
             pulumi.set(__self__, "capacity_max", capacity_max)
+        if capacity_max_bytes is not None:
+            pulumi.set(__self__, "capacity_max_bytes", capacity_max_bytes)
         if capacity_min is not None:
             pulumi.set(__self__, "capacity_min", capacity_min)
+        if capacity_min_bytes is not None:
+            pulumi.set(__self__, "capacity_min_bytes", capacity_min_bytes)
         if clone_id is not None:
             pulumi.set(__self__, "clone_id", clone_id)
         if controller_required is not None:
             pulumi.set(__self__, "controller_required", controller_required)
         if controllers_expected is not None:
             pulumi.set(__self__, "controllers_expected", controllers_expected)
         if controllers_healthy is not None:
             pulumi.set(__self__, "controllers_healthy", controllers_healthy)
+        if external_id is not None:
+            pulumi.set(__self__, "external_id", external_id)
         if mount_options is not None:
             pulumi.set(__self__, "mount_options", mount_options)
         if name is not None:
             pulumi.set(__self__, "name", name)
         if namespace is not None:
             pulumi.set(__self__, "namespace", namespace)
         if nodes_expected is not None:
@@ -332,113 +318,141 @@
             pulumi.set(__self__, "secrets", secrets)
         if snapshot_id is not None:
             pulumi.set(__self__, "snapshot_id", snapshot_id)
         if topologies is not None:
             pulumi.set(__self__, "topologies", topologies)
         if topology_request is not None:
             pulumi.set(__self__, "topology_request", topology_request)
-        if type is not None:
-            pulumi.set(__self__, "type", type)
         if volume_id is not None:
             pulumi.set(__self__, "volume_id", volume_id)
 
     @property
     @pulumi.getter
-    def capabilities(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['ExternalVolumeCapabilityArgs']]]]:
+    def capabilities(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['CsiVolumeCapabilityArgs']]]]:
         """
         `(``Capability``: <required>)` - Options for validating the capability of a volume.
         """
         return pulumi.get(self, "capabilities")
 
     @capabilities.setter
-    def capabilities(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['ExternalVolumeCapabilityArgs']]]]):
+    def capabilities(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['CsiVolumeCapabilityArgs']]]]):
         pulumi.set(self, "capabilities", value)
 
     @property
+    @pulumi.getter
+    def capacity(self) -> Optional[pulumi.Input[int]]:
+        return pulumi.get(self, "capacity")
+
+    @capacity.setter
+    def capacity(self, value: Optional[pulumi.Input[int]]):
+        pulumi.set(self, "capacity", value)
+
+    @property
     @pulumi.getter(name="capacityMax")
     def capacity_max(self) -> Optional[pulumi.Input[str]]:
         """
         `(string: <optional>)` - Option to signal a maximum volume size. This may not be supported by all storage providers.
         """
         return pulumi.get(self, "capacity_max")
 
     @capacity_max.setter
     def capacity_max(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "capacity_max", value)
 
     @property
+    @pulumi.getter(name="capacityMaxBytes")
+    def capacity_max_bytes(self) -> Optional[pulumi.Input[int]]:
+        return pulumi.get(self, "capacity_max_bytes")
+
+    @capacity_max_bytes.setter
+    def capacity_max_bytes(self, value: Optional[pulumi.Input[int]]):
+        pulumi.set(self, "capacity_max_bytes", value)
+
+    @property
     @pulumi.getter(name="capacityMin")
     def capacity_min(self) -> Optional[pulumi.Input[str]]:
         """
         `(string: <optional>)` - Option to signal a minimum volume size. This may not be supported by all storage providers.
         """
         return pulumi.get(self, "capacity_min")
 
     @capacity_min.setter
     def capacity_min(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "capacity_min", value)
 
     @property
+    @pulumi.getter(name="capacityMinBytes")
+    def capacity_min_bytes(self) -> Optional[pulumi.Input[int]]:
+        return pulumi.get(self, "capacity_min_bytes")
+
+    @capacity_min_bytes.setter
+    def capacity_min_bytes(self, value: Optional[pulumi.Input[int]]):
+        pulumi.set(self, "capacity_min_bytes", value)
+
+    @property
     @pulumi.getter(name="cloneId")
     def clone_id(self) -> Optional[pulumi.Input[str]]:
         """
         `(string: <optional>)` - The external ID of an existing volume to restore. If ommited, the volume will be created from scratch. Conflicts with `snapshot_id`.
         """
         return pulumi.get(self, "clone_id")
 
     @clone_id.setter
     def clone_id(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "clone_id", value)
 
     @property
     @pulumi.getter(name="controllerRequired")
     def controller_required(self) -> Optional[pulumi.Input[bool]]:
-        """
-        `(boolean)`
-        """
         return pulumi.get(self, "controller_required")
 
     @controller_required.setter
     def controller_required(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "controller_required", value)
 
     @property
     @pulumi.getter(name="controllersExpected")
     def controllers_expected(self) -> Optional[pulumi.Input[int]]:
-        """
-        `(integer)`
-        """
         return pulumi.get(self, "controllers_expected")
 
     @controllers_expected.setter
     def controllers_expected(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "controllers_expected", value)
 
     @property
     @pulumi.getter(name="controllersHealthy")
     def controllers_healthy(self) -> Optional[pulumi.Input[int]]:
-        """
-        `(integer)`
-        """
         return pulumi.get(self, "controllers_healthy")
 
     @controllers_healthy.setter
     def controllers_healthy(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "controllers_healthy", value)
 
     @property
+    @pulumi.getter(name="externalId")
+    def external_id(self) -> Optional[pulumi.Input[str]]:
+        """
+        The ID of the physical volume from the storage provider.
+        """
+        return pulumi.get(self, "external_id")
+
+    @external_id.setter
+    def external_id(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "external_id", value)
+
+    @property
     @pulumi.getter(name="mountOptions")
-    def mount_options(self) -> Optional[pulumi.Input['ExternalVolumeMountOptionsArgs']]:
+    def mount_options(self) -> Optional[pulumi.Input['CsiVolumeMountOptionsArgs']]:
         """
         `(block: optional)` Options for mounting `block-device` volumes without a pre-formatted file system.
         """
         return pulumi.get(self, "mount_options")
 
     @mount_options.setter
-    def mount_options(self, value: Optional[pulumi.Input['ExternalVolumeMountOptionsArgs']]):
+    def mount_options(self, value: Optional[pulumi.Input['CsiVolumeMountOptionsArgs']]):
         pulumi.set(self, "mount_options", value)
 
     @property
     @pulumi.getter
     def name(self) -> Optional[pulumi.Input[str]]:
         """
         `(string: <required>)` - The display name for the volume.
@@ -460,29 +474,23 @@
     @namespace.setter
     def namespace(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "namespace", value)
 
     @property
     @pulumi.getter(name="nodesExpected")
     def nodes_expected(self) -> Optional[pulumi.Input[int]]:
-        """
-        `(integer)`
-        """
         return pulumi.get(self, "nodes_expected")
 
     @nodes_expected.setter
     def nodes_expected(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "nodes_expected", value)
 
     @property
     @pulumi.getter(name="nodesHealthy")
     def nodes_healthy(self) -> Optional[pulumi.Input[int]]:
-        """
-        `(integer)`
-        """
         return pulumi.get(self, "nodes_healthy")
 
     @nodes_healthy.setter
     def nodes_healthy(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "nodes_healthy", value)
 
     @property
@@ -508,41 +516,32 @@
     @plugin_id.setter
     def plugin_id(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "plugin_id", value)
 
     @property
     @pulumi.getter(name="pluginProvider")
     def plugin_provider(self) -> Optional[pulumi.Input[str]]:
-        """
-        `(string)`
-        """
         return pulumi.get(self, "plugin_provider")
 
     @plugin_provider.setter
     def plugin_provider(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "plugin_provider", value)
 
     @property
     @pulumi.getter(name="pluginProviderVersion")
     def plugin_provider_version(self) -> Optional[pulumi.Input[str]]:
-        """
-        `(string)`
-        """
         return pulumi.get(self, "plugin_provider_version")
 
     @plugin_provider_version.setter
     def plugin_provider_version(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "plugin_provider_version", value)
 
     @property
     @pulumi.getter
     def schedulable(self) -> Optional[pulumi.Input[bool]]:
-        """
-        `(boolean)`
-        """
         return pulumi.get(self, "schedulable")
 
     @schedulable.setter
     def schedulable(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "schedulable", value)
 
     @property
@@ -567,237 +566,127 @@
 
     @snapshot_id.setter
     def snapshot_id(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "snapshot_id", value)
 
     @property
     @pulumi.getter
-    def topologies(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['ExternalVolumeTopologyArgs']]]]:
-        """
-        `(List of topologies)`
-        """
+    def topologies(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['CsiVolumeTopologyArgs']]]]:
         return pulumi.get(self, "topologies")
 
     @topologies.setter
-    def topologies(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['ExternalVolumeTopologyArgs']]]]):
+    def topologies(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['CsiVolumeTopologyArgs']]]]):
         pulumi.set(self, "topologies", value)
 
     @property
     @pulumi.getter(name="topologyRequest")
-    def topology_request(self) -> Optional[pulumi.Input['ExternalVolumeTopologyRequestArgs']]:
+    def topology_request(self) -> Optional[pulumi.Input['CsiVolumeTopologyRequestArgs']]:
         """
         `(``TopologyRequest``: <optional>)` - Specify locations (region, zone, rack, etc.) where the provisioned volume is accessible from.
         """
         return pulumi.get(self, "topology_request")
 
     @topology_request.setter
-    def topology_request(self, value: Optional[pulumi.Input['ExternalVolumeTopologyRequestArgs']]):
+    def topology_request(self, value: Optional[pulumi.Input['CsiVolumeTopologyRequestArgs']]):
         pulumi.set(self, "topology_request", value)
 
     @property
-    @pulumi.getter
-    def type(self) -> Optional[pulumi.Input[str]]:
-        """
-        `(string: <required>)` - The type of the volume. Currently, only `csi` is supported.
-        """
-        return pulumi.get(self, "type")
-
-    @type.setter
-    def type(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "type", value)
-
-    @property
     @pulumi.getter(name="volumeId")
     def volume_id(self) -> Optional[pulumi.Input[str]]:
         """
         `(string: <required>)` - The unique ID of the volume.
         """
         return pulumi.get(self, "volume_id")
 
     @volume_id.setter
     def volume_id(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "volume_id", value)
 
 
-class ExternalVolume(pulumi.CustomResource):
+class CsiVolume(pulumi.CustomResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
-                 capabilities: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ExternalVolumeCapabilityArgs']]]]] = None,
+                 capabilities: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['CsiVolumeCapabilityArgs']]]]] = None,
                  capacity_max: Optional[pulumi.Input[str]] = None,
                  capacity_min: Optional[pulumi.Input[str]] = None,
                  clone_id: Optional[pulumi.Input[str]] = None,
-                 mount_options: Optional[pulumi.Input[pulumi.InputType['ExternalVolumeMountOptionsArgs']]] = None,
+                 mount_options: Optional[pulumi.Input[pulumi.InputType['CsiVolumeMountOptionsArgs']]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  namespace: Optional[pulumi.Input[str]] = None,
                  parameters: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  plugin_id: Optional[pulumi.Input[str]] = None,
                  secrets: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  snapshot_id: Optional[pulumi.Input[str]] = None,
-                 topology_request: Optional[pulumi.Input[pulumi.InputType['ExternalVolumeTopologyRequestArgs']]] = None,
-                 type: Optional[pulumi.Input[str]] = None,
+                 topology_request: Optional[pulumi.Input[pulumi.InputType['CsiVolumeTopologyRequestArgs']]] = None,
                  volume_id: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
-        ## Example Usage
-
-        Creating a volume:
-
-        <!--Start PulumiCodeChooser -->
-        ```python
-        import pulumi
-        import pulumi_nomad as nomad
-
-        # It can sometimes be helpful to wait for a particular plugin to be available
-        ebs = nomad.get_plugin(plugin_id="aws-ebs0",
-            wait_for_healthy=True)
-        mysql_volume = nomad.ExternalVolume("mysql_volume",
-            type="csi",
-            plugin_id="aws-ebs0",
-            volume_id="mysql_volume",
-            name="mysql_volume",
-            capacity_min="10GiB",
-            capacity_max="20GiB",
-            capabilities=[nomad.ExternalVolumeCapabilityArgs(
-                access_mode="single-node-writer",
-                attachment_mode="file-system",
-            )],
-            mount_options=nomad.ExternalVolumeMountOptionsArgs(
-                fs_type="ext4",
-            ),
-            topology_request=nomad.ExternalVolumeTopologyRequestArgs(
-                required=nomad.ExternalVolumeTopologyRequestRequiredArgs(
-                    topologies=[
-                        nomad.ExternalVolumeTopologyRequestRequiredTopologyArgs(
-                            segments={
-                                "rack": "R1",
-                                "zone": "us-east-1a",
-                            },
-                        ),
-                        nomad.ExternalVolumeTopologyRequestRequiredTopologyArgs(
-                            segments={
-                                "rack": "R2",
-                            },
-                        ),
-                    ],
-                ),
-            ),
-            opts=pulumi.ResourceOptions(depends_on=[ebs]))
-        ```
-        <!--End PulumiCodeChooser -->
-
+        Create a CsiVolume resource with the given unique name, props, and options.
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ExternalVolumeCapabilityArgs']]]] capabilities: `(``Capability``: <required>)` - Options for validating the capability of a volume.
+        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['CsiVolumeCapabilityArgs']]]] capabilities: `(``Capability``: <required>)` - Options for validating the capability of a volume.
         :param pulumi.Input[str] capacity_max: `(string: <optional>)` - Option to signal a maximum volume size. This may not be supported by all storage providers.
         :param pulumi.Input[str] capacity_min: `(string: <optional>)` - Option to signal a minimum volume size. This may not be supported by all storage providers.
         :param pulumi.Input[str] clone_id: `(string: <optional>)` - The external ID of an existing volume to restore. If ommited, the volume will be created from scratch. Conflicts with `snapshot_id`.
-        :param pulumi.Input[pulumi.InputType['ExternalVolumeMountOptionsArgs']] mount_options: `(block: optional)` Options for mounting `block-device` volumes without a pre-formatted file system.
+        :param pulumi.Input[pulumi.InputType['CsiVolumeMountOptionsArgs']] mount_options: `(block: optional)` Options for mounting `block-device` volumes without a pre-formatted file system.
         :param pulumi.Input[str] name: `(string: <required>)` - The display name for the volume.
         :param pulumi.Input[str] namespace: `(string: "default")` - The namespace in which to register the volume.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] parameters: `(map[string]string: optional)` An optional key-value map of strings passed directly to the CSI plugin to configure the volume.
         :param pulumi.Input[str] plugin_id: `(string: <required>)` - The ID of the Nomad plugin for registering this volume.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] secrets: `(map[string]string: optional)` An optional key-value map of strings used as credentials for publishing and unpublishing volumes.
         :param pulumi.Input[str] snapshot_id: `(string: <optional>)` - The external ID of a snapshot to restore. If ommited, the volume will be created from scratch. Conflicts with `clone_id`.
-        :param pulumi.Input[pulumi.InputType['ExternalVolumeTopologyRequestArgs']] topology_request: `(``TopologyRequest``: <optional>)` - Specify locations (region, zone, rack, etc.) where the provisioned volume is accessible from.
-        :param pulumi.Input[str] type: `(string: <required>)` - The type of the volume. Currently, only `csi` is supported.
+        :param pulumi.Input[pulumi.InputType['CsiVolumeTopologyRequestArgs']] topology_request: `(``TopologyRequest``: <optional>)` - Specify locations (region, zone, rack, etc.) where the provisioned volume is accessible from.
         :param pulumi.Input[str] volume_id: `(string: <required>)` - The unique ID of the volume.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
-                 args: ExternalVolumeArgs,
+                 args: CsiVolumeArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
-        ## Example Usage
-
-        Creating a volume:
-
-        <!--Start PulumiCodeChooser -->
-        ```python
-        import pulumi
-        import pulumi_nomad as nomad
-
-        # It can sometimes be helpful to wait for a particular plugin to be available
-        ebs = nomad.get_plugin(plugin_id="aws-ebs0",
-            wait_for_healthy=True)
-        mysql_volume = nomad.ExternalVolume("mysql_volume",
-            type="csi",
-            plugin_id="aws-ebs0",
-            volume_id="mysql_volume",
-            name="mysql_volume",
-            capacity_min="10GiB",
-            capacity_max="20GiB",
-            capabilities=[nomad.ExternalVolumeCapabilityArgs(
-                access_mode="single-node-writer",
-                attachment_mode="file-system",
-            )],
-            mount_options=nomad.ExternalVolumeMountOptionsArgs(
-                fs_type="ext4",
-            ),
-            topology_request=nomad.ExternalVolumeTopologyRequestArgs(
-                required=nomad.ExternalVolumeTopologyRequestRequiredArgs(
-                    topologies=[
-                        nomad.ExternalVolumeTopologyRequestRequiredTopologyArgs(
-                            segments={
-                                "rack": "R1",
-                                "zone": "us-east-1a",
-                            },
-                        ),
-                        nomad.ExternalVolumeTopologyRequestRequiredTopologyArgs(
-                            segments={
-                                "rack": "R2",
-                            },
-                        ),
-                    ],
-                ),
-            ),
-            opts=pulumi.ResourceOptions(depends_on=[ebs]))
-        ```
-        <!--End PulumiCodeChooser -->
-
+        Create a CsiVolume resource with the given unique name, props, and options.
         :param str resource_name: The name of the resource.
-        :param ExternalVolumeArgs args: The arguments to use to populate this resource's properties.
+        :param CsiVolumeArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
-        resource_args, opts = _utilities.get_resource_args_opts(ExternalVolumeArgs, pulumi.ResourceOptions, *args, **kwargs)
+        resource_args, opts = _utilities.get_resource_args_opts(CsiVolumeArgs, pulumi.ResourceOptions, *args, **kwargs)
         if resource_args is not None:
             __self__._internal_init(resource_name, opts, **resource_args.__dict__)
         else:
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
-                 capabilities: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ExternalVolumeCapabilityArgs']]]]] = None,
+                 capabilities: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['CsiVolumeCapabilityArgs']]]]] = None,
                  capacity_max: Optional[pulumi.Input[str]] = None,
                  capacity_min: Optional[pulumi.Input[str]] = None,
                  clone_id: Optional[pulumi.Input[str]] = None,
-                 mount_options: Optional[pulumi.Input[pulumi.InputType['ExternalVolumeMountOptionsArgs']]] = None,
+                 mount_options: Optional[pulumi.Input[pulumi.InputType['CsiVolumeMountOptionsArgs']]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  namespace: Optional[pulumi.Input[str]] = None,
                  parameters: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  plugin_id: Optional[pulumi.Input[str]] = None,
                  secrets: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  snapshot_id: Optional[pulumi.Input[str]] = None,
-                 topology_request: Optional[pulumi.Input[pulumi.InputType['ExternalVolumeTopologyRequestArgs']]] = None,
-                 type: Optional[pulumi.Input[str]] = None,
+                 topology_request: Optional[pulumi.Input[pulumi.InputType['CsiVolumeTopologyRequestArgs']]] = None,
                  volume_id: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
-            __props__ = ExternalVolumeArgs.__new__(ExternalVolumeArgs)
+            __props__ = CsiVolumeArgs.__new__(CsiVolumeArgs)
 
             if capabilities is None and not opts.urn:
                 raise TypeError("Missing required property 'capabilities'")
             __props__.__dict__["capabilities"] = capabilities
             __props__.__dict__["capacity_max"] = capacity_max
             __props__.__dict__["capacity_min"] = capacity_min
             __props__.__dict__["clone_id"] = clone_id
@@ -807,181 +696,195 @@
             __props__.__dict__["parameters"] = parameters
             if plugin_id is None and not opts.urn:
                 raise TypeError("Missing required property 'plugin_id'")
             __props__.__dict__["plugin_id"] = plugin_id
             __props__.__dict__["secrets"] = None if secrets is None else pulumi.Output.secret(secrets)
             __props__.__dict__["snapshot_id"] = snapshot_id
             __props__.__dict__["topology_request"] = topology_request
-            __props__.__dict__["type"] = type
             if volume_id is None and not opts.urn:
                 raise TypeError("Missing required property 'volume_id'")
             __props__.__dict__["volume_id"] = volume_id
+            __props__.__dict__["capacity"] = None
+            __props__.__dict__["capacity_max_bytes"] = None
+            __props__.__dict__["capacity_min_bytes"] = None
             __props__.__dict__["controller_required"] = None
             __props__.__dict__["controllers_expected"] = None
             __props__.__dict__["controllers_healthy"] = None
+            __props__.__dict__["external_id"] = None
             __props__.__dict__["nodes_expected"] = None
             __props__.__dict__["nodes_healthy"] = None
             __props__.__dict__["plugin_provider"] = None
             __props__.__dict__["plugin_provider_version"] = None
             __props__.__dict__["schedulable"] = None
             __props__.__dict__["topologies"] = None
         secret_opts = pulumi.ResourceOptions(additional_secret_outputs=["secrets"])
         opts = pulumi.ResourceOptions.merge(opts, secret_opts)
-        super(ExternalVolume, __self__).__init__(
-            'nomad:index/externalVolume:ExternalVolume',
+        super(CsiVolume, __self__).__init__(
+            'nomad:index/csiVolume:CsiVolume',
             resource_name,
             __props__,
             opts)
 
     @staticmethod
     def get(resource_name: str,
             id: pulumi.Input[str],
             opts: Optional[pulumi.ResourceOptions] = None,
-            capabilities: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ExternalVolumeCapabilityArgs']]]]] = None,
+            capabilities: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['CsiVolumeCapabilityArgs']]]]] = None,
+            capacity: Optional[pulumi.Input[int]] = None,
             capacity_max: Optional[pulumi.Input[str]] = None,
+            capacity_max_bytes: Optional[pulumi.Input[int]] = None,
             capacity_min: Optional[pulumi.Input[str]] = None,
+            capacity_min_bytes: Optional[pulumi.Input[int]] = None,
             clone_id: Optional[pulumi.Input[str]] = None,
             controller_required: Optional[pulumi.Input[bool]] = None,
             controllers_expected: Optional[pulumi.Input[int]] = None,
             controllers_healthy: Optional[pulumi.Input[int]] = None,
-            mount_options: Optional[pulumi.Input[pulumi.InputType['ExternalVolumeMountOptionsArgs']]] = None,
+            external_id: Optional[pulumi.Input[str]] = None,
+            mount_options: Optional[pulumi.Input[pulumi.InputType['CsiVolumeMountOptionsArgs']]] = None,
             name: Optional[pulumi.Input[str]] = None,
             namespace: Optional[pulumi.Input[str]] = None,
             nodes_expected: Optional[pulumi.Input[int]] = None,
             nodes_healthy: Optional[pulumi.Input[int]] = None,
             parameters: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
             plugin_id: Optional[pulumi.Input[str]] = None,
             plugin_provider: Optional[pulumi.Input[str]] = None,
             plugin_provider_version: Optional[pulumi.Input[str]] = None,
             schedulable: Optional[pulumi.Input[bool]] = None,
             secrets: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
             snapshot_id: Optional[pulumi.Input[str]] = None,
-            topologies: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ExternalVolumeTopologyArgs']]]]] = None,
-            topology_request: Optional[pulumi.Input[pulumi.InputType['ExternalVolumeTopologyRequestArgs']]] = None,
-            type: Optional[pulumi.Input[str]] = None,
-            volume_id: Optional[pulumi.Input[str]] = None) -> 'ExternalVolume':
+            topologies: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['CsiVolumeTopologyArgs']]]]] = None,
+            topology_request: Optional[pulumi.Input[pulumi.InputType['CsiVolumeTopologyRequestArgs']]] = None,
+            volume_id: Optional[pulumi.Input[str]] = None) -> 'CsiVolume':
         """
-        Get an existing ExternalVolume resource's state with the given name, id, and optional extra
+        Get an existing CsiVolume resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ExternalVolumeCapabilityArgs']]]] capabilities: `(``Capability``: <required>)` - Options for validating the capability of a volume.
+        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['CsiVolumeCapabilityArgs']]]] capabilities: `(``Capability``: <required>)` - Options for validating the capability of a volume.
         :param pulumi.Input[str] capacity_max: `(string: <optional>)` - Option to signal a maximum volume size. This may not be supported by all storage providers.
         :param pulumi.Input[str] capacity_min: `(string: <optional>)` - Option to signal a minimum volume size. This may not be supported by all storage providers.
         :param pulumi.Input[str] clone_id: `(string: <optional>)` - The external ID of an existing volume to restore. If ommited, the volume will be created from scratch. Conflicts with `snapshot_id`.
-        :param pulumi.Input[bool] controller_required: `(boolean)`
-        :param pulumi.Input[int] controllers_expected: `(integer)`
-        :param pulumi.Input[int] controllers_healthy: `(integer)`
-        :param pulumi.Input[pulumi.InputType['ExternalVolumeMountOptionsArgs']] mount_options: `(block: optional)` Options for mounting `block-device` volumes without a pre-formatted file system.
+        :param pulumi.Input[str] external_id: The ID of the physical volume from the storage provider.
+        :param pulumi.Input[pulumi.InputType['CsiVolumeMountOptionsArgs']] mount_options: `(block: optional)` Options for mounting `block-device` volumes without a pre-formatted file system.
         :param pulumi.Input[str] name: `(string: <required>)` - The display name for the volume.
         :param pulumi.Input[str] namespace: `(string: "default")` - The namespace in which to register the volume.
-        :param pulumi.Input[int] nodes_expected: `(integer)`
-        :param pulumi.Input[int] nodes_healthy: `(integer)`
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] parameters: `(map[string]string: optional)` An optional key-value map of strings passed directly to the CSI plugin to configure the volume.
         :param pulumi.Input[str] plugin_id: `(string: <required>)` - The ID of the Nomad plugin for registering this volume.
-        :param pulumi.Input[str] plugin_provider: `(string)`
-        :param pulumi.Input[str] plugin_provider_version: `(string)`
-        :param pulumi.Input[bool] schedulable: `(boolean)`
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] secrets: `(map[string]string: optional)` An optional key-value map of strings used as credentials for publishing and unpublishing volumes.
         :param pulumi.Input[str] snapshot_id: `(string: <optional>)` - The external ID of a snapshot to restore. If ommited, the volume will be created from scratch. Conflicts with `clone_id`.
-        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ExternalVolumeTopologyArgs']]]] topologies: `(List of topologies)`
-        :param pulumi.Input[pulumi.InputType['ExternalVolumeTopologyRequestArgs']] topology_request: `(``TopologyRequest``: <optional>)` - Specify locations (region, zone, rack, etc.) where the provisioned volume is accessible from.
-        :param pulumi.Input[str] type: `(string: <required>)` - The type of the volume. Currently, only `csi` is supported.
+        :param pulumi.Input[pulumi.InputType['CsiVolumeTopologyRequestArgs']] topology_request: `(``TopologyRequest``: <optional>)` - Specify locations (region, zone, rack, etc.) where the provisioned volume is accessible from.
         :param pulumi.Input[str] volume_id: `(string: <required>)` - The unique ID of the volume.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
-        __props__ = _ExternalVolumeState.__new__(_ExternalVolumeState)
+        __props__ = _CsiVolumeState.__new__(_CsiVolumeState)
 
         __props__.__dict__["capabilities"] = capabilities
+        __props__.__dict__["capacity"] = capacity
         __props__.__dict__["capacity_max"] = capacity_max
+        __props__.__dict__["capacity_max_bytes"] = capacity_max_bytes
         __props__.__dict__["capacity_min"] = capacity_min
+        __props__.__dict__["capacity_min_bytes"] = capacity_min_bytes
         __props__.__dict__["clone_id"] = clone_id
         __props__.__dict__["controller_required"] = controller_required
         __props__.__dict__["controllers_expected"] = controllers_expected
         __props__.__dict__["controllers_healthy"] = controllers_healthy
+        __props__.__dict__["external_id"] = external_id
         __props__.__dict__["mount_options"] = mount_options
         __props__.__dict__["name"] = name
         __props__.__dict__["namespace"] = namespace
         __props__.__dict__["nodes_expected"] = nodes_expected
         __props__.__dict__["nodes_healthy"] = nodes_healthy
         __props__.__dict__["parameters"] = parameters
         __props__.__dict__["plugin_id"] = plugin_id
         __props__.__dict__["plugin_provider"] = plugin_provider
         __props__.__dict__["plugin_provider_version"] = plugin_provider_version
         __props__.__dict__["schedulable"] = schedulable
         __props__.__dict__["secrets"] = secrets
         __props__.__dict__["snapshot_id"] = snapshot_id
         __props__.__dict__["topologies"] = topologies
         __props__.__dict__["topology_request"] = topology_request
-        __props__.__dict__["type"] = type
         __props__.__dict__["volume_id"] = volume_id
-        return ExternalVolume(resource_name, opts=opts, __props__=__props__)
+        return CsiVolume(resource_name, opts=opts, __props__=__props__)
 
     @property
     @pulumi.getter
-    def capabilities(self) -> pulumi.Output[Sequence['outputs.ExternalVolumeCapability']]:
+    def capabilities(self) -> pulumi.Output[Sequence['outputs.CsiVolumeCapability']]:
         """
         `(``Capability``: <required>)` - Options for validating the capability of a volume.
         """
         return pulumi.get(self, "capabilities")
 
     @property
+    @pulumi.getter
+    def capacity(self) -> pulumi.Output[int]:
+        return pulumi.get(self, "capacity")
+
+    @property
     @pulumi.getter(name="capacityMax")
     def capacity_max(self) -> pulumi.Output[Optional[str]]:
         """
         `(string: <optional>)` - Option to signal a maximum volume size. This may not be supported by all storage providers.
         """
         return pulumi.get(self, "capacity_max")
 
     @property
+    @pulumi.getter(name="capacityMaxBytes")
+    def capacity_max_bytes(self) -> pulumi.Output[int]:
+        return pulumi.get(self, "capacity_max_bytes")
+
+    @property
     @pulumi.getter(name="capacityMin")
     def capacity_min(self) -> pulumi.Output[Optional[str]]:
         """
         `(string: <optional>)` - Option to signal a minimum volume size. This may not be supported by all storage providers.
         """
         return pulumi.get(self, "capacity_min")
 
     @property
+    @pulumi.getter(name="capacityMinBytes")
+    def capacity_min_bytes(self) -> pulumi.Output[int]:
+        return pulumi.get(self, "capacity_min_bytes")
+
+    @property
     @pulumi.getter(name="cloneId")
     def clone_id(self) -> pulumi.Output[Optional[str]]:
         """
         `(string: <optional>)` - The external ID of an existing volume to restore. If ommited, the volume will be created from scratch. Conflicts with `snapshot_id`.
         """
         return pulumi.get(self, "clone_id")
 
     @property
     @pulumi.getter(name="controllerRequired")
     def controller_required(self) -> pulumi.Output[bool]:
-        """
-        `(boolean)`
-        """
         return pulumi.get(self, "controller_required")
 
     @property
     @pulumi.getter(name="controllersExpected")
     def controllers_expected(self) -> pulumi.Output[int]:
-        """
-        `(integer)`
-        """
         return pulumi.get(self, "controllers_expected")
 
     @property
     @pulumi.getter(name="controllersHealthy")
     def controllers_healthy(self) -> pulumi.Output[int]:
+        return pulumi.get(self, "controllers_healthy")
+
+    @property
+    @pulumi.getter(name="externalId")
+    def external_id(self) -> pulumi.Output[str]:
         """
-        `(integer)`
+        The ID of the physical volume from the storage provider.
         """
-        return pulumi.get(self, "controllers_healthy")
+        return pulumi.get(self, "external_id")
 
     @property
     @pulumi.getter(name="mountOptions")
-    def mount_options(self) -> pulumi.Output[Optional['outputs.ExternalVolumeMountOptions']]:
+    def mount_options(self) -> pulumi.Output[Optional['outputs.CsiVolumeMountOptions']]:
         """
         `(block: optional)` Options for mounting `block-device` volumes without a pre-formatted file system.
         """
         return pulumi.get(self, "mount_options")
 
     @property
     @pulumi.getter
@@ -998,25 +901,19 @@
         `(string: "default")` - The namespace in which to register the volume.
         """
         return pulumi.get(self, "namespace")
 
     @property
     @pulumi.getter(name="nodesExpected")
     def nodes_expected(self) -> pulumi.Output[int]:
-        """
-        `(integer)`
-        """
         return pulumi.get(self, "nodes_expected")
 
     @property
     @pulumi.getter(name="nodesHealthy")
     def nodes_healthy(self) -> pulumi.Output[int]:
-        """
-        `(integer)`
-        """
         return pulumi.get(self, "nodes_healthy")
 
     @property
     @pulumi.getter
     def parameters(self) -> pulumi.Output[Optional[Mapping[str, str]]]:
         """
         `(map[string]string: optional)` An optional key-value map of strings passed directly to the CSI plugin to configure the volume.
@@ -1030,33 +927,24 @@
         `(string: <required>)` - The ID of the Nomad plugin for registering this volume.
         """
         return pulumi.get(self, "plugin_id")
 
     @property
     @pulumi.getter(name="pluginProvider")
     def plugin_provider(self) -> pulumi.Output[str]:
-        """
-        `(string)`
-        """
         return pulumi.get(self, "plugin_provider")
 
     @property
     @pulumi.getter(name="pluginProviderVersion")
     def plugin_provider_version(self) -> pulumi.Output[str]:
-        """
-        `(string)`
-        """
         return pulumi.get(self, "plugin_provider_version")
 
     @property
     @pulumi.getter
     def schedulable(self) -> pulumi.Output[bool]:
-        """
-        `(boolean)`
-        """
         return pulumi.get(self, "schedulable")
 
     @property
     @pulumi.getter
     def secrets(self) -> pulumi.Output[Optional[Mapping[str, str]]]:
         """
         `(map[string]string: optional)` An optional key-value map of strings used as credentials for publishing and unpublishing volumes.
@@ -1069,37 +957,26 @@
         """
         `(string: <optional>)` - The external ID of a snapshot to restore. If ommited, the volume will be created from scratch. Conflicts with `clone_id`.
         """
         return pulumi.get(self, "snapshot_id")
 
     @property
     @pulumi.getter
-    def topologies(self) -> pulumi.Output[Sequence['outputs.ExternalVolumeTopology']]:
-        """
-        `(List of topologies)`
-        """
+    def topologies(self) -> pulumi.Output[Sequence['outputs.CsiVolumeTopology']]:
         return pulumi.get(self, "topologies")
 
     @property
     @pulumi.getter(name="topologyRequest")
-    def topology_request(self) -> pulumi.Output[Optional['outputs.ExternalVolumeTopologyRequest']]:
+    def topology_request(self) -> pulumi.Output[Optional['outputs.CsiVolumeTopologyRequest']]:
         """
         `(``TopologyRequest``: <optional>)` - Specify locations (region, zone, rack, etc.) where the provisioned volume is accessible from.
         """
         return pulumi.get(self, "topology_request")
 
     @property
-    @pulumi.getter
-    def type(self) -> pulumi.Output[Optional[str]]:
-        """
-        `(string: <required>)` - The type of the volume. Currently, only `csi` is supported.
-        """
-        return pulumi.get(self, "type")
-
-    @property
     @pulumi.getter(name="volumeId")
     def volume_id(self) -> pulumi.Output[str]:
         """
         `(string: <required>)` - The unique ID of the volume.
         """
         return pulumi.get(self, "volume_id")
```

### Comparing `pulumi_nomad-2.3.0a1713561631/pulumi_nomad/get_acl_policies.py` & `pulumi_nomad-2.3.0a1713899842/pulumi_nomad/get_acl_policies.py`

 * *Files 5% similar despite different names*

```diff
@@ -69,22 +69,20 @@
 def get_acl_policies(prefix: Optional[str] = None,
                      opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetAclPoliciesResult:
     """
     Retrieve a list of ACL Policies.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_nomad as nomad
 
     example = nomad.get_acl_policies(prefix="prod")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str prefix: `(string)` An optional string to filter ACL policies based on name prefix. If not provided, all policies are returned.
     """
     __args__ = dict()
     __args__['prefix'] = prefix
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
@@ -100,20 +98,18 @@
 def get_acl_policies_output(prefix: Optional[pulumi.Input[Optional[str]]] = None,
                             opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetAclPoliciesResult]:
     """
     Retrieve a list of ACL Policies.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_nomad as nomad
 
     example = nomad.get_acl_policies(prefix="prod")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str prefix: `(string)` An optional string to filter ACL policies based on name prefix. If not provided, all policies are returned.
     """
     ...
```

### Comparing `pulumi_nomad-2.3.0a1713561631/pulumi_nomad/get_acl_policy.py` & `pulumi_nomad-2.3.0a1713899842/pulumi_nomad/get_acl_policy.py`

 * *Files 10% similar despite different names*

```diff
@@ -83,22 +83,20 @@
 def get_acl_policy(name: Optional[str] = None,
                    opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetAclPolicyResult:
     """
     Retrieve information on an ACL Policy.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_nomad as nomad
 
     my_policy = nomad.get_acl_policy(name="my-policy")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str name: `(string)` - the name of the ACL Policy.
     """
     __args__ = dict()
     __args__['name'] = name
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
@@ -115,20 +113,18 @@
 def get_acl_policy_output(name: Optional[pulumi.Input[str]] = None,
                           opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetAclPolicyResult]:
     """
     Retrieve information on an ACL Policy.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_nomad as nomad
 
     my_policy = nomad.get_acl_policy(name="my-policy")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str name: `(string)` - the name of the ACL Policy.
     """
     ...
```

### Comparing `pulumi_nomad-2.3.0a1713561631/pulumi_nomad/get_acl_role.py` & `pulumi_nomad-2.3.0a1713899842/pulumi_nomad/get_acl_role.py`

 * *Files 8% similar despite different names*

```diff
@@ -84,22 +84,20 @@
 def get_acl_role(id: Optional[str] = None,
                  opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetAclRoleResult:
     """
     Get information on an ACL Role.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_nomad as nomad
 
     example = nomad.get_acl_role(id="aa534e09-6a07-0a45-2295-a7f77063d429")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str id: `(string)` The unique identifier of the ACL Role.
     """
     __args__ = dict()
     __args__['id'] = id
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
@@ -116,20 +114,18 @@
 def get_acl_role_output(id: Optional[pulumi.Input[str]] = None,
                         opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetAclRoleResult]:
     """
     Get information on an ACL Role.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_nomad as nomad
 
     example = nomad.get_acl_role(id="aa534e09-6a07-0a45-2295-a7f77063d429")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str id: `(string)` The unique identifier of the ACL Role.
     """
     ...
```

### Comparing `pulumi_nomad-2.3.0a1713561631/pulumi_nomad/get_acl_roles.py` & `pulumi_nomad-2.3.0a1713899842/pulumi_nomad/get_acl_roles.py`

 * *Files 3% similar despite different names*

```diff
@@ -66,22 +66,20 @@
 def get_acl_roles(prefix: Optional[str] = None,
                   opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetAclRolesResult:
     """
     Retrieve a list of ACL Roles.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_nomad as nomad
 
     example = nomad.get_acl_roles(prefix="a242")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str prefix: `(string)` An optional string to filter ACL Roles based on ID
            prefix. If not provided, all policies are returned.
     """
     __args__ = dict()
     __args__['prefix'] = prefix
@@ -98,21 +96,19 @@
 def get_acl_roles_output(prefix: Optional[pulumi.Input[Optional[str]]] = None,
                          opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetAclRolesResult]:
     """
     Retrieve a list of ACL Roles.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_nomad as nomad
 
     example = nomad.get_acl_roles(prefix="a242")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str prefix: `(string)` An optional string to filter ACL Roles based on ID
            prefix. If not provided, all policies are returned.
     """
     ...
```

### Comparing `pulumi_nomad-2.3.0a1713561631/pulumi_nomad/get_acl_token.py` & `pulumi_nomad-2.3.0a1713899842/pulumi_nomad/get_acl_token.py`

 * *Files 5% similar despite different names*

```diff
@@ -169,22 +169,20 @@
 
 
 def get_acl_token(accessor_id: Optional[str] = None,
                   opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetAclTokenResult:
     """
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_nomad as nomad
 
     my_token = nomad.get_acl_token(accessor_id="aa534e09-6a07-0a45-2295-a7f77063d429")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str accessor_id: `(string)` Non-sensitive identifier for this token.
     """
     __args__ = dict()
     __args__['accessorId'] = accessor_id
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
@@ -206,20 +204,18 @@
 
 @_utilities.lift_output_func(get_acl_token)
 def get_acl_token_output(accessor_id: Optional[pulumi.Input[str]] = None,
                          opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetAclTokenResult]:
     """
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_nomad as nomad
 
     my_token = nomad.get_acl_token(accessor_id="aa534e09-6a07-0a45-2295-a7f77063d429")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str accessor_id: `(string)` Non-sensitive identifier for this token.
     """
     ...
```

### Comparing `pulumi_nomad-2.3.0a1713561631/pulumi_nomad/get_acl_tokens.py` & `pulumi_nomad-2.3.0a1713899842/pulumi_nomad/get_acl_tokens.py`

 * *Files 8% similar despite different names*

```diff
@@ -69,22 +69,20 @@
 def get_acl_tokens(prefix: Optional[str] = None,
                    opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetAclTokensResult:
     """
     Get a list of ACL tokens.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_nomad as nomad
 
     tokens = nomad.get_acl_tokens(prefix="a242")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str prefix: `(string)` Optional prefix to filter the tokens.
     """
     __args__ = dict()
     __args__['prefix'] = prefix
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
@@ -100,20 +98,18 @@
 def get_acl_tokens_output(prefix: Optional[pulumi.Input[Optional[str]]] = None,
                           opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetAclTokensResult]:
     """
     Get a list of ACL tokens.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_nomad as nomad
 
     tokens = nomad.get_acl_tokens(prefix="a242")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str prefix: `(string)` Optional prefix to filter the tokens.
     """
     ...
```

### Comparing `pulumi_nomad-2.3.0a1713561631/pulumi_nomad/get_allocations.py` & `pulumi_nomad-2.3.0a1713899842/pulumi_nomad/get_allocations.py`

 * *Files 2% similar despite different names*

```diff
@@ -93,22 +93,20 @@
                     prefix: Optional[str] = None,
                     opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetAllocationsResult:
     """
     Retrieve a list of allocations from Nomad.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_nomad as nomad
 
     example = nomad.get_allocations(filter="JobID == \\"example\\"")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str filter: `(string: <optional>)` - Specifies the
            [expression][nomad_api_filter] used to filter the results.
     :param str namespace: `(string: <optional>)` - Specifies the namespace to search for
            allocations in.
     :param str prefix: `(string: <optional>)` - Specifies a string to filter allocations
@@ -135,22 +133,20 @@
                            prefix: Optional[pulumi.Input[Optional[str]]] = None,
                            opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetAllocationsResult]:
     """
     Retrieve a list of allocations from Nomad.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_nomad as nomad
 
     example = nomad.get_allocations(filter="JobID == \\"example\\"")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str filter: `(string: <optional>)` - Specifies the
            [expression][nomad_api_filter] used to filter the results.
     :param str namespace: `(string: <optional>)` - Specifies the namespace to search for
            allocations in.
     :param str prefix: `(string: <optional>)` - Specifies a string to filter allocations
```

### Comparing `pulumi_nomad-2.3.0a1713561631/pulumi_nomad/get_datacenters.py` & `pulumi_nomad-2.3.0a1713899842/pulumi_nomad/get_datacenters.py`

 * *Files 3% similar despite different names*

```diff
@@ -78,23 +78,21 @@
                     prefix: Optional[str] = None,
                     opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetDatacentersResult:
     """
     Retrieve a list of datacenters.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_nomad as nomad
 
     datacenters = nomad.get_datacenters(prefix="prod",
         ignore_down_nodes=True)
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param bool ignore_down_nodes: `(bool: false)`: An optional flag that, if set to `true` will ignore down nodes when compiling the list of datacenters.
     :param str prefix: `(string)`: An optional string to filter datacenters based on name prefix. If not provided, all datacenters are returned.
     """
     __args__ = dict()
     __args__['ignoreDownNodes'] = ignore_down_nodes
@@ -114,22 +112,20 @@
                            prefix: Optional[pulumi.Input[Optional[str]]] = None,
                            opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetDatacentersResult]:
     """
     Retrieve a list of datacenters.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_nomad as nomad
 
     datacenters = nomad.get_datacenters(prefix="prod",
         ignore_down_nodes=True)
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param bool ignore_down_nodes: `(bool: false)`: An optional flag that, if set to `true` will ignore down nodes when compiling the list of datacenters.
     :param str prefix: `(string)`: An optional string to filter datacenters based on name prefix. If not provided, all datacenters are returned.
     """
     ...
```

### Comparing `pulumi_nomad-2.3.0a1713561631/pulumi_nomad/get_deployments.py` & `pulumi_nomad-2.3.0a1713899842/pulumi_nomad/get_deployments.py`

 * *Files 9% similar despite different names*

```diff
@@ -58,22 +58,20 @@
 
 def get_deployments(opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetDeploymentsResult:
     """
     Retrieve a list of deployments in Nomad.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_nomad as nomad
 
     example = nomad.get_deployments()
     ```
-    <!--End PulumiCodeChooser -->
     """
     __args__ = dict()
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('nomad:index/getDeployments:getDeployments', __args__, opts=opts, typ=GetDeploymentsResult).value
 
     return AwaitableGetDeploymentsResult(
         deployments=pulumi.get(__ret__, 'deployments'),
@@ -83,17 +81,15 @@
 @_utilities.lift_output_func(get_deployments)
 def get_deployments_output(opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetDeploymentsResult]:
     """
     Retrieve a list of deployments in Nomad.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_nomad as nomad
 
     example = nomad.get_deployments()
     ```
-    <!--End PulumiCodeChooser -->
     """
     ...
```

### Comparing `pulumi_nomad-2.3.0a1713561631/pulumi_nomad/get_job.py` & `pulumi_nomad-2.3.0a1713899842/pulumi_nomad/get_job.py`

 * *Files 1% similar despite different names*

```diff
@@ -297,23 +297,21 @@
 
     An error is triggered if zero or more than one result is returned by the query.
 
     ## Example Usage
 
     Get the data about a snapshot:
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_nomad as nomad
 
     example = nomad.get_job(job_id="example",
         namespace="dev")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str job_id: `(string)` ID of the job.
     :param str namespace: `(string)` Namespace of the specified job.
     """
     __args__ = dict()
     __args__['jobId'] = job_id
@@ -356,22 +354,20 @@
 
     An error is triggered if zero or more than one result is returned by the query.
 
     ## Example Usage
 
     Get the data about a snapshot:
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_nomad as nomad
 
     example = nomad.get_job(job_id="example",
         namespace="dev")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str job_id: `(string)` ID of the job.
     :param str namespace: `(string)` Namespace of the specified job.
     """
     ...
```

### Comparing `pulumi_nomad-2.3.0a1713561631/pulumi_nomad/get_job_parser.py` & `pulumi_nomad-2.3.0a1713899842/pulumi_nomad/get_job_parser.py`

 * *Files identical despite different names*

### Comparing `pulumi_nomad-2.3.0a1713561631/pulumi_nomad/get_namespace.py` & `pulumi_nomad-2.3.0a1713899842/pulumi_nomad/get_namespace.py`

 * *Files 8% similar despite different names*

```diff
@@ -114,22 +114,20 @@
 def get_namespace(name: Optional[str] = None,
                   opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetNamespaceResult:
     """
     Get information about a namespace in Nomad.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_nomad as nomad
 
     namespaces = nomad.get_namespace(name="default")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str name: `(string)` - The name of the namespace.
     """
     __args__ = dict()
     __args__['name'] = name
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
@@ -149,20 +147,18 @@
 def get_namespace_output(name: Optional[pulumi.Input[str]] = None,
                          opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetNamespaceResult]:
     """
     Get information about a namespace in Nomad.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_nomad as nomad
 
     namespaces = nomad.get_namespace(name="default")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str name: `(string)` - The name of the namespace.
     """
     ...
```

### Comparing `pulumi_nomad-2.3.0a1713561631/pulumi_nomad/get_namespaces.py` & `pulumi_nomad-2.3.0a1713899842/pulumi_nomad/get_namespaces.py`

 * *Files 7% similar despite different names*

```diff
@@ -58,15 +58,14 @@
 
 def get_namespaces(opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetNamespacesResult:
     """
     Retrieve a list of namespaces available in Nomad.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_nomad as nomad
 
     namespaces = nomad.get_namespaces()
     namespace = []
     for range in [{"value": i} for i in range(0, len(namespaces.namespaces))]:
@@ -74,15 +73,14 @@
             name=f"namespace-{namespaces[range['value']]}",
             description=f"Write to the namespace {namespaces[range['value']]}",
             rules_hcl=f\"\"\"namespace "{namespaces[range["value"]]}" {{
       policy = "write"
     }}
     \"\"\"))
     ```
-    <!--End PulumiCodeChooser -->
     """
     __args__ = dict()
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('nomad:index/getNamespaces:getNamespaces', __args__, opts=opts, typ=GetNamespacesResult).value
 
     return AwaitableGetNamespacesResult(
         id=pulumi.get(__ret__, 'id'),
@@ -92,15 +90,14 @@
 @_utilities.lift_output_func(get_namespaces)
 def get_namespaces_output(opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetNamespacesResult]:
     """
     Retrieve a list of namespaces available in Nomad.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_nomad as nomad
 
     namespaces = nomad.get_namespaces()
     namespace = []
     for range in [{"value": i} for i in range(0, len(namespaces.namespaces))]:
@@ -108,10 +105,9 @@
             name=f"namespace-{namespaces[range['value']]}",
             description=f"Write to the namespace {namespaces[range['value']]}",
             rules_hcl=f\"\"\"namespace "{namespaces[range["value"]]}" {{
       policy = "write"
     }}
     \"\"\"))
     ```
-    <!--End PulumiCodeChooser -->
     """
     ...
```

### Comparing `pulumi_nomad-2.3.0a1713561631/pulumi_nomad/get_node_pool.py` & `pulumi_nomad-2.3.0a1713899842/pulumi_nomad/get_node_pool.py`

 * *Files 3% similar despite different names*

```diff
@@ -94,22 +94,20 @@
 def get_node_pool(name: Optional[str] = None,
                   opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetNodePoolResult:
     """
     Get information about a node pool in Nomad.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_nomad as nomad
 
     dev = nomad.get_node_pool(name="dev")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str name: `(string)` - The name of the node pool to fetch.
     """
     __args__ = dict()
     __args__['name'] = name
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
@@ -127,20 +125,18 @@
 def get_node_pool_output(name: Optional[pulumi.Input[str]] = None,
                          opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetNodePoolResult]:
     """
     Get information about a node pool in Nomad.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_nomad as nomad
 
     dev = nomad.get_node_pool(name="dev")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str name: `(string)` - The name of the node pool to fetch.
     """
     ...
```

### Comparing `pulumi_nomad-2.3.0a1713561631/pulumi_nomad/get_node_pools.py` & `pulumi_nomad-2.3.0a1713899842/pulumi_nomad/get_node_pools.py`

 * *Files 4% similar despite different names*

```diff
@@ -80,22 +80,20 @@
                    prefix: Optional[str] = None,
                    opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetNodePoolsResult:
     """
     Retrieve a list of node pools available in Nomad.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_nomad as nomad
 
     prod = nomad.get_node_pools(filter="Meta.env == \\"prod\\"")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str filter: `(string)` - Specifies the [expression][nomad_api_filter] used to
            filter the results.
     :param str prefix: `(string)` - Specifies a string to filter node pools based on a name
            prefix.
     """
@@ -117,22 +115,20 @@
                           prefix: Optional[pulumi.Input[Optional[str]]] = None,
                           opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetNodePoolsResult]:
     """
     Retrieve a list of node pools available in Nomad.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_nomad as nomad
 
     prod = nomad.get_node_pools(filter="Meta.env == \\"prod\\"")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str filter: `(string)` - Specifies the [expression][nomad_api_filter] used to
            filter the results.
     :param str prefix: `(string)` - Specifies a string to filter node pools based on a name
            prefix.
     """
```

### Comparing `pulumi_nomad-2.3.0a1713561631/pulumi_nomad/get_plugin.py` & `pulumi_nomad-2.3.0a1713899842/pulumi_nomad/get_plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -182,23 +182,21 @@
     configured to wait, it will result in an error. For simple existence checks,
     use the `get_plugins` listing datasource.
 
     ## Example Usage
 
     Check for the existence of a plugin:
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_nomad as nomad
 
     ebs = nomad.get_plugin(plugin_id="aws-ebs0",
         wait_for_healthy=True)
     ```
-    <!--End PulumiCodeChooser -->
 
     This will check for a plugin with the ID `aws-ebs0`, waiting until the plugin
     is healthy before returning.
 
 
     :param str plugin_id: `(string)` ID of the plugin.
     :param bool wait_for_healthy: `(boolean)` retry until the plugin exists and all controllers are healthy
@@ -241,23 +239,21 @@
     configured to wait, it will result in an error. For simple existence checks,
     use the `get_plugins` listing datasource.
 
     ## Example Usage
 
     Check for the existence of a plugin:
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_nomad as nomad
 
     ebs = nomad.get_plugin(plugin_id="aws-ebs0",
         wait_for_healthy=True)
     ```
-    <!--End PulumiCodeChooser -->
 
     This will check for a plugin with the ID `aws-ebs0`, waiting until the plugin
     is healthy before returning.
 
 
     :param str plugin_id: `(string)` ID of the plugin.
     :param bool wait_for_healthy: `(boolean)` retry until the plugin exists and all controllers are healthy
```

### Comparing `pulumi_nomad-2.3.0a1713561631/pulumi_nomad/get_plugins.py` & `pulumi_nomad-2.3.0a1713899842/pulumi_nomad/get_plugins.py`

 * *Files 14% similar despite different names*

```diff
@@ -68,22 +68,20 @@
 def get_plugins(type: Optional[str] = None,
                 opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetPluginsResult:
     """
     Retrieve a list of dynamic plugins in Nomad.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_nomad as nomad
 
     example = nomad.get_plugins()
     ```
-    <!--End PulumiCodeChooser -->
     """
     __args__ = dict()
     __args__['type'] = type
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('nomad:index/getPlugins:getPlugins', __args__, opts=opts, typ=GetPluginsResult).value
 
     return AwaitableGetPluginsResult(
@@ -96,17 +94,15 @@
 def get_plugins_output(type: Optional[pulumi.Input[Optional[str]]] = None,
                        opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetPluginsResult]:
     """
     Retrieve a list of dynamic plugins in Nomad.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_nomad as nomad
 
     example = nomad.get_plugins()
     ```
-    <!--End PulumiCodeChooser -->
     """
     ...
```

### Comparing `pulumi_nomad-2.3.0a1713561631/pulumi_nomad/get_regions.py` & `pulumi_nomad-2.3.0a1713899842/pulumi_nomad/get_regions.py`

 * *Files 4% similar despite different names*

```diff
@@ -58,30 +58,28 @@
 
 def get_regions(opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetRegionsResult:
     """
     Retrieve a list of regions available in Nomad.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_nomad as nomad
 
 
     def not_implemented(msg):
         raise NotImplementedError(msg)
 
     my_regions = nomad.get_regions()
     jobs = not_implemented("The template_file data resource is not yet supported.")
     app = []
     for range in [{"value": i} for i in range(0, len(my_regions.regions))]:
         app.append(nomad.Job(f"app-{range['value']}", jobspec=jobs[range["value"]]["rendered"]))
     ```
-    <!--End PulumiCodeChooser -->
     """
     __args__ = dict()
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('nomad:index/getRegions:getRegions', __args__, opts=opts, typ=GetRegionsResult).value
 
     return AwaitableGetRegionsResult(
         id=pulumi.get(__ret__, 'id'),
@@ -91,25 +89,23 @@
 @_utilities.lift_output_func(get_regions)
 def get_regions_output(opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetRegionsResult]:
     """
     Retrieve a list of regions available in Nomad.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_nomad as nomad
 
 
     def not_implemented(msg):
         raise NotImplementedError(msg)
 
     my_regions = nomad.get_regions()
     jobs = not_implemented("The template_file data resource is not yet supported.")
     app = []
     for range in [{"value": i} for i in range(0, len(my_regions.regions))]:
         app.append(nomad.Job(f"app-{range['value']}", jobspec=jobs[range["value"]]["rendered"]))
     ```
-    <!--End PulumiCodeChooser -->
     """
     ...
```

### Comparing `pulumi_nomad-2.3.0a1713561631/pulumi_nomad/get_scaling_policies.py` & `pulumi_nomad-2.3.0a1713899842/pulumi_nomad/get_scaling_policies.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,23 +82,21 @@
                          type: Optional[str] = None,
                          opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetScalingPoliciesResult:
     """
     Retrieve a list of Scaling Policies.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_nomad as nomad
 
     example = nomad.get_scaling_policies(job_id="webapp",
         type="horizontal")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str job_id: `(string)` - An optional string to filter scaling policies based on the target job. If not provided, policies for all jobs are returned.
     :param str type: `(string)` - An optional string to filter scaling policies based on policy type. If not provided, policies of all types are returned.
     """
     __args__ = dict()
     __args__['jobId'] = job_id
@@ -118,22 +116,20 @@
                                 type: Optional[pulumi.Input[Optional[str]]] = None,
                                 opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetScalingPoliciesResult]:
     """
     Retrieve a list of Scaling Policies.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_nomad as nomad
 
     example = nomad.get_scaling_policies(job_id="webapp",
         type="horizontal")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str job_id: `(string)` - An optional string to filter scaling policies based on the target job. If not provided, policies for all jobs are returned.
     :param str type: `(string)` - An optional string to filter scaling policies based on policy type. If not provided, policies of all types are returned.
     """
     ...
```

### Comparing `pulumi_nomad-2.3.0a1713561631/pulumi_nomad/get_scaling_policy.py` & `pulumi_nomad-2.3.0a1713899842/pulumi_nomad/get_scaling_policy.py`

 * *Files 6% similar despite different names*

```diff
@@ -116,22 +116,20 @@
 def get_scaling_policy(id: Optional[str] = None,
                        opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetScalingPolicyResult:
     """
     Retrieve a Scaling Policy.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_nomad as nomad
 
     example = nomad.get_scaling_policy(id="ad19848d-1921-179c-affa-244a3543be88")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str id: `(string: <required>)` - The  ID of the scaling policy.
     """
     __args__ = dict()
     __args__['id'] = id
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
@@ -151,20 +149,18 @@
 def get_scaling_policy_output(id: Optional[pulumi.Input[str]] = None,
                               opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetScalingPolicyResult]:
     """
     Retrieve a Scaling Policy.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_nomad as nomad
 
     example = nomad.get_scaling_policy(id="ad19848d-1921-179c-affa-244a3543be88")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str id: `(string: <required>)` - The  ID of the scaling policy.
     """
     ...
```

### Comparing `pulumi_nomad-2.3.0a1713561631/pulumi_nomad/get_scheduler_policy.py` & `pulumi_nomad-2.3.0a1713899842/pulumi_nomad/get_scheduler_policy.py`

 * *Files 4% similar despite different names*

```diff
@@ -82,22 +82,20 @@
 
 def get_scheduler_policy(opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetSchedulerPolicyResult:
     """
     Retrieve the cluster's [scheduler configuration](https://www.nomadproject.io/api-docs/operator#sample-response-3).
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_nomad as nomad
 
     global_ = nomad.get_scheduler_policy()
     ```
-    <!--End PulumiCodeChooser -->
     """
     __args__ = dict()
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('nomad:index/getSchedulerPolicy:getSchedulerPolicy', __args__, opts=opts, typ=GetSchedulerPolicyResult).value
 
     return AwaitableGetSchedulerPolicyResult(
         id=pulumi.get(__ret__, 'id'),
@@ -109,17 +107,15 @@
 @_utilities.lift_output_func(get_scheduler_policy)
 def get_scheduler_policy_output(opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetSchedulerPolicyResult]:
     """
     Retrieve the cluster's [scheduler configuration](https://www.nomadproject.io/api-docs/operator#sample-response-3).
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_nomad as nomad
 
     global_ = nomad.get_scheduler_policy()
     ```
-    <!--End PulumiCodeChooser -->
     """
     ...
```

### Comparing `pulumi_nomad-2.3.0a1713561631/pulumi_nomad/get_variable.py` & `pulumi_nomad-2.3.0a1713899842/pulumi_nomad/get_variable.py`

 * *Files 4% similar despite different names*

```diff
@@ -82,22 +82,20 @@
 
 def get_variable(namespace: Optional[str] = None,
                  path: Optional[str] = None,
                  opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetVariableResult:
     """
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_nomad as nomad
 
     example = nomad.Variable("example", path="path/of/existing/variable")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str namespace: `(string: "default")` - The namepsace in which the variable exists.
     :param str path: `(string)` - Path to the existing variable.
     """
     __args__ = dict()
     __args__['namespace'] = namespace
@@ -115,21 +113,19 @@
 @_utilities.lift_output_func(get_variable)
 def get_variable_output(namespace: Optional[pulumi.Input[Optional[str]]] = None,
                         path: Optional[pulumi.Input[str]] = None,
                         opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetVariableResult]:
     """
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_nomad as nomad
 
     example = nomad.Variable("example", path="path/of/existing/variable")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str namespace: `(string: "default")` - The namepsace in which the variable exists.
     :param str path: `(string)` - Path to the existing variable.
     """
     ...
```

### Comparing `pulumi_nomad-2.3.0a1713561631/pulumi_nomad/get_volumes.py` & `pulumi_nomad-2.3.0a1713899842/pulumi_nomad/get_volumes.py`

 * *Files 5% similar despite different names*

```diff
@@ -101,22 +101,20 @@
                 type: Optional[str] = None,
                 opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetVolumesResult:
     """
     Retrieve a list of volumes in Nomad.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_nomad as nomad
 
     example = nomad.get_volumes()
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str namespace: `(string: "default")` Nomad namespace.
     :param str node_id: `(string: optional)` Volume node filter.
     :param str plugin_id: `(string: optional)` Plugin ID filter.
     :param str type: `(string: "csi")` Volume type (currently only supports `csi`)
     """
@@ -144,22 +142,20 @@
                        type: Optional[pulumi.Input[Optional[str]]] = None,
                        opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetVolumesResult]:
     """
     Retrieve a list of volumes in Nomad.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_nomad as nomad
 
     example = nomad.get_volumes()
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str namespace: `(string: "default")` Nomad namespace.
     :param str node_id: `(string: optional)` Volume node filter.
     :param str plugin_id: `(string: optional)` Plugin ID filter.
     :param str type: `(string: "csi")` Volume type (currently only supports `csi`)
     """
```

### Comparing `pulumi_nomad-2.3.0a1713561631/pulumi_nomad/job.py` & `pulumi_nomad-2.3.0a1713899842/pulumi_nomad/job.py`

 * *Files identical despite different names*

### Comparing `pulumi_nomad-2.3.0a1713561631/pulumi_nomad/namespace.py` & `pulumi_nomad-2.3.0a1713899842/pulumi_nomad/namespace.py`

 * *Files 2% similar despite different names*

```diff
@@ -245,33 +245,30 @@
         `name = "default"` will cause the namespace to be reset to its default
         configuration.
 
         ## Example Usage
 
         Registering a namespace:
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_nomad as nomad
 
         dev = nomad.Namespace("dev",
             name="dev",
             description="Shared development environment.",
             quota="dev",
             meta={
                 "owner": "John Doe",
                 "foo": "bar",
             })
         ```
-        <!--End PulumiCodeChooser -->
 
         Registering a namespace with a quota:
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_nomad as nomad
 
         web_team = nomad.QuoteSpecification("web_team",
             name="web-team",
             description="web team quota",
@@ -283,15 +280,14 @@
                 ),
             )])
         web = nomad.Namespace("web",
             name="web",
             description="Web team production environment.",
             quota=web_team.name)
         ```
-        <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[pulumi.InputType['NamespaceCapabilitiesArgs']] capabilities: `(block: <optional>)` - A block of capabilities for the namespace. Can't
                be repeated. See below for the structure of this block.
         :param pulumi.Input[str] description: `(string: "")` - A description of the namespace.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] meta: `(map[string]string: <optional>)` -  Specifies arbitrary KV metadata to associate with the namespace.
@@ -313,33 +309,30 @@
         `name = "default"` will cause the namespace to be reset to its default
         configuration.
 
         ## Example Usage
 
         Registering a namespace:
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_nomad as nomad
 
         dev = nomad.Namespace("dev",
             name="dev",
             description="Shared development environment.",
             quota="dev",
             meta={
                 "owner": "John Doe",
                 "foo": "bar",
             })
         ```
-        <!--End PulumiCodeChooser -->
 
         Registering a namespace with a quota:
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_nomad as nomad
 
         web_team = nomad.QuoteSpecification("web_team",
             name="web-team",
             description="web team quota",
@@ -351,15 +344,14 @@
                 ),
             )])
         web = nomad.Namespace("web",
             name="web",
             description="Web team production environment.",
             quota=web_team.name)
         ```
-        <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param NamespaceArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
```

### Comparing `pulumi_nomad-2.3.0a1713561631/pulumi_nomad/node_pool.py` & `pulumi_nomad-2.3.0a1713899842/pulumi_nomad/node_pool.py`

 * *Files 3% similar despite different names*

```diff
@@ -174,28 +174,26 @@
         """
         Provisions a node pool within a Nomad cluster.
 
         ## Example Usage
 
         Registering a node pool:
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_nomad as nomad
 
         dev = nomad.NodePool("dev",
             name="dev",
             description="Nodes for the development environment.",
             meta={
                 "department": "Engineering",
                 "env": "dev",
             })
         ```
-        <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] description: `(string)` - The description of the node pool.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] meta: `(map[string]string)` - Arbitrary KV metadata associated with the
                node pool.
         :param pulumi.Input[str] name: `(string)` - The name of the node pool.
@@ -210,28 +208,26 @@
         """
         Provisions a node pool within a Nomad cluster.
 
         ## Example Usage
 
         Registering a node pool:
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_nomad as nomad
 
         dev = nomad.NodePool("dev",
             name="dev",
             description="Nodes for the development environment.",
             meta={
                 "department": "Engineering",
                 "env": "dev",
             })
         ```
-        <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param NodePoolArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
```

### Comparing `pulumi_nomad-2.3.0a1713561631/pulumi_nomad/outputs.py` & `pulumi_nomad-2.3.0a1713899842/pulumi_nomad/outputs.py`

 * *Files 3% similar despite different names*

```diff
@@ -293,66 +293,56 @@
 
     def __init__(__self__, *,
                  job_id: str,
                  group: Optional[str] = None,
                  namespace: Optional[str] = None,
                  task: Optional[str] = None):
         """
-        :param str job_id: `(string: <optional>` - The job to attach the policy. Required if
-               `group` is set.
-        :param str group: `(string: <optional>` - The group to attach the policy. Required if
-               `task` is set.
-        :param str namespace: `(string: "default")` - The namespace to attach the policy.
-               Required if `job_id` is set.
-        :param str task: `(string: <optional>` - The task to attach the policy.
-               
-               [nomad_docs_wi]: https://www.nomadproject.io/docs/concepts/workload-identity#workload-associated-acl-policies
+        :param str job_id: Job
+        :param str group: Group
+        :param str namespace: Namespace
+        :param str task: Task
         """
         pulumi.set(__self__, "job_id", job_id)
         if group is not None:
             pulumi.set(__self__, "group", group)
         if namespace is not None:
             pulumi.set(__self__, "namespace", namespace)
         if task is not None:
             pulumi.set(__self__, "task", task)
 
     @property
     @pulumi.getter(name="jobId")
     def job_id(self) -> str:
         """
-        `(string: <optional>` - The job to attach the policy. Required if
-        `group` is set.
+        Job
         """
         return pulumi.get(self, "job_id")
 
     @property
     @pulumi.getter
     def group(self) -> Optional[str]:
         """
-        `(string: <optional>` - The group to attach the policy. Required if
-        `task` is set.
+        Group
         """
         return pulumi.get(self, "group")
 
     @property
     @pulumi.getter
     def namespace(self) -> Optional[str]:
         """
-        `(string: "default")` - The namespace to attach the policy.
-        Required if `job_id` is set.
+        Namespace
         """
         return pulumi.get(self, "namespace")
 
     @property
     @pulumi.getter
     def task(self) -> Optional[str]:
         """
-        `(string: <optional>` - The task to attach the policy.
-
-        [nomad_docs_wi]: https://www.nomadproject.io/docs/concepts/workload-identity#workload-associated-acl-policies
+        Task
         """
         return pulumi.get(self, "task")
 
 
 @pulumi.output_type
 class AclRolePolicy(dict):
     def __init__(__self__, *,
@@ -625,32 +615,20 @@
         return pulumi.get(self, "mount_flags")
 
 
 @pulumi.output_type
 class CsiVolumeRegistrationTopology(dict):
     def __init__(__self__, *,
                  segments: Optional[Mapping[str, str]] = None):
-        """
-        :param Mapping[str, str] segments: `(map[string]string)` - Define the attributes for the topology request.
-               
-               In addition to the above arguments, the following attributes are exported and
-               can be referenced:
-        """
         if segments is not None:
             pulumi.set(__self__, "segments", segments)
 
     @property
     @pulumi.getter
     def segments(self) -> Optional[Mapping[str, str]]:
-        """
-        `(map[string]string)` - Define the attributes for the topology request.
-
-        In addition to the above arguments, the following attributes are exported and
-        can be referenced:
-        """
         return pulumi.get(self, "segments")
 
 
 @pulumi.output_type
 class CsiVolumeRegistrationTopologyRequest(dict):
     def __init__(__self__, *,
                  required: Optional['outputs.CsiVolumeRegistrationTopologyRequestRequired'] = None):
@@ -670,73 +648,55 @@
 
 
 @pulumi.output_type
 class CsiVolumeRegistrationTopologyRequestRequired(dict):
     def __init__(__self__, *,
                  topologies: Sequence['outputs.CsiVolumeRegistrationTopologyRequestRequiredTopology']):
         """
-        :param Sequence['CsiVolumeRegistrationTopologyRequestRequiredTopologyArgs'] topologies: `(List of segments: <required>)` - Defines the location for the volume.
+        :param Sequence['CsiVolumeRegistrationTopologyRequestRequiredTopologyArgs'] topologies: Defines the location for the volume.
         """
         pulumi.set(__self__, "topologies", topologies)
 
     @property
     @pulumi.getter
     def topologies(self) -> Sequence['outputs.CsiVolumeRegistrationTopologyRequestRequiredTopology']:
         """
-        `(List of segments: <required>)` - Defines the location for the volume.
+        Defines the location for the volume.
         """
         return pulumi.get(self, "topologies")
 
 
 @pulumi.output_type
 class CsiVolumeRegistrationTopologyRequestRequiredTopology(dict):
     def __init__(__self__, *,
                  segments: Mapping[str, str]):
         """
-        :param Mapping[str, str] segments: `(map[string]string)` - Define the attributes for the topology request.
-               
-               In addition to the above arguments, the following attributes are exported and
-               can be referenced:
+        :param Mapping[str, str] segments: Define attributes for the topology request.
         """
         pulumi.set(__self__, "segments", segments)
 
     @property
     @pulumi.getter
     def segments(self) -> Mapping[str, str]:
         """
-        `(map[string]string)` - Define the attributes for the topology request.
-
-        In addition to the above arguments, the following attributes are exported and
-        can be referenced:
+        Define attributes for the topology request.
         """
         return pulumi.get(self, "segments")
 
 
 @pulumi.output_type
 class CsiVolumeTopology(dict):
     def __init__(__self__, *,
                  segments: Optional[Mapping[str, str]] = None):
-        """
-        :param Mapping[str, str] segments: `(map[string]string)` - Define the attributes for the topology request.
-               
-               In addition to the above arguments, the following attributes are exported and
-               can be referenced:
-        """
         if segments is not None:
             pulumi.set(__self__, "segments", segments)
 
     @property
     @pulumi.getter
     def segments(self) -> Optional[Mapping[str, str]]:
-        """
-        `(map[string]string)` - Define the attributes for the topology request.
-
-        In addition to the above arguments, the following attributes are exported and
-        can be referenced:
-        """
         return pulumi.get(self, "segments")
 
 
 @pulumi.output_type
 class CsiVolumeTopologyRequest(dict):
     def __init__(__self__, *,
                  preferred: Optional['outputs.CsiVolumeTopologyRequestPreferred'] = None,
@@ -768,89 +728,77 @@
 
 
 @pulumi.output_type
 class CsiVolumeTopologyRequestPreferred(dict):
     def __init__(__self__, *,
                  topologies: Sequence['outputs.CsiVolumeTopologyRequestPreferredTopology']):
         """
-        :param Sequence['CsiVolumeTopologyRequestPreferredTopologyArgs'] topologies: `(List of segments: <required>)` - Defines the location for the volume.
+        :param Sequence['CsiVolumeTopologyRequestPreferredTopologyArgs'] topologies: Defines the location for the volume.
         """
         pulumi.set(__self__, "topologies", topologies)
 
     @property
     @pulumi.getter
     def topologies(self) -> Sequence['outputs.CsiVolumeTopologyRequestPreferredTopology']:
         """
-        `(List of segments: <required>)` - Defines the location for the volume.
+        Defines the location for the volume.
         """
         return pulumi.get(self, "topologies")
 
 
 @pulumi.output_type
 class CsiVolumeTopologyRequestPreferredTopology(dict):
     def __init__(__self__, *,
                  segments: Mapping[str, str]):
         """
-        :param Mapping[str, str] segments: `(map[string]string)` - Define the attributes for the topology request.
-               
-               In addition to the above arguments, the following attributes are exported and
-               can be referenced:
+        :param Mapping[str, str] segments: Define the attributes for the topology request.
         """
         pulumi.set(__self__, "segments", segments)
 
     @property
     @pulumi.getter
     def segments(self) -> Mapping[str, str]:
         """
-        `(map[string]string)` - Define the attributes for the topology request.
-
-        In addition to the above arguments, the following attributes are exported and
-        can be referenced:
+        Define the attributes for the topology request.
         """
         return pulumi.get(self, "segments")
 
 
 @pulumi.output_type
 class CsiVolumeTopologyRequestRequired(dict):
     def __init__(__self__, *,
                  topologies: Sequence['outputs.CsiVolumeTopologyRequestRequiredTopology']):
         """
-        :param Sequence['CsiVolumeTopologyRequestRequiredTopologyArgs'] topologies: `(List of segments: <required>)` - Defines the location for the volume.
+        :param Sequence['CsiVolumeTopologyRequestRequiredTopologyArgs'] topologies: Defines the location for the volume.
         """
         pulumi.set(__self__, "topologies", topologies)
 
     @property
     @pulumi.getter
     def topologies(self) -> Sequence['outputs.CsiVolumeTopologyRequestRequiredTopology']:
         """
-        `(List of segments: <required>)` - Defines the location for the volume.
+        Defines the location for the volume.
         """
         return pulumi.get(self, "topologies")
 
 
 @pulumi.output_type
 class CsiVolumeTopologyRequestRequiredTopology(dict):
     def __init__(__self__, *,
                  segments: Mapping[str, str]):
         """
-        :param Mapping[str, str] segments: `(map[string]string)` - Define the attributes for the topology request.
-               
-               In addition to the above arguments, the following attributes are exported and
-               can be referenced:
+        :param Mapping[str, str] segments: Define the attributes for the topology request.
         """
         pulumi.set(__self__, "segments", segments)
 
     @property
     @pulumi.getter
     def segments(self) -> Mapping[str, str]:
         """
-        `(map[string]string)` - Define the attributes for the topology request.
-
-        In addition to the above arguments, the following attributes are exported and
-        can be referenced:
+        Define the attributes for the topology request.
         """
         return pulumi.get(self, "segments")
 
 
 @pulumi.output_type
 class ExternalVolumeCapability(dict):
     @staticmethod
@@ -963,32 +911,20 @@
         return pulumi.get(self, "mount_flags")
 
 
 @pulumi.output_type
 class ExternalVolumeTopology(dict):
     def __init__(__self__, *,
                  segments: Optional[Mapping[str, str]] = None):
-        """
-        :param Mapping[str, str] segments: `(map[string]string)` - Define the attributes for the topology request.
-               
-               In addition to the above arguments, the following attributes are exported and
-               can be referenced:
-        """
         if segments is not None:
             pulumi.set(__self__, "segments", segments)
 
     @property
     @pulumi.getter
     def segments(self) -> Optional[Mapping[str, str]]:
-        """
-        `(map[string]string)` - Define the attributes for the topology request.
-
-        In addition to the above arguments, the following attributes are exported and
-        can be referenced:
-        """
         return pulumi.get(self, "segments")
 
 
 @pulumi.output_type
 class ExternalVolumeTopologyRequest(dict):
     def __init__(__self__, *,
                  preferred: Optional['outputs.ExternalVolumeTopologyRequestPreferred'] = None,
@@ -1020,89 +956,77 @@
 
 
 @pulumi.output_type
 class ExternalVolumeTopologyRequestPreferred(dict):
     def __init__(__self__, *,
                  topologies: Sequence['outputs.ExternalVolumeTopologyRequestPreferredTopology']):
         """
-        :param Sequence['ExternalVolumeTopologyRequestPreferredTopologyArgs'] topologies: `(List of segments: <required>)` - Defines the location for the volume.
+        :param Sequence['ExternalVolumeTopologyRequestPreferredTopologyArgs'] topologies: Defines the location for the volume.
         """
         pulumi.set(__self__, "topologies", topologies)
 
     @property
     @pulumi.getter
     def topologies(self) -> Sequence['outputs.ExternalVolumeTopologyRequestPreferredTopology']:
         """
-        `(List of segments: <required>)` - Defines the location for the volume.
+        Defines the location for the volume.
         """
         return pulumi.get(self, "topologies")
 
 
 @pulumi.output_type
 class ExternalVolumeTopologyRequestPreferredTopology(dict):
     def __init__(__self__, *,
                  segments: Mapping[str, str]):
         """
-        :param Mapping[str, str] segments: `(map[string]string)` - Define the attributes for the topology request.
-               
-               In addition to the above arguments, the following attributes are exported and
-               can be referenced:
+        :param Mapping[str, str] segments: Define the attributes for the topology request.
         """
         pulumi.set(__self__, "segments", segments)
 
     @property
     @pulumi.getter
     def segments(self) -> Mapping[str, str]:
         """
-        `(map[string]string)` - Define the attributes for the topology request.
-
-        In addition to the above arguments, the following attributes are exported and
-        can be referenced:
+        Define the attributes for the topology request.
         """
         return pulumi.get(self, "segments")
 
 
 @pulumi.output_type
 class ExternalVolumeTopologyRequestRequired(dict):
     def __init__(__self__, *,
                  topologies: Sequence['outputs.ExternalVolumeTopologyRequestRequiredTopology']):
         """
-        :param Sequence['ExternalVolumeTopologyRequestRequiredTopologyArgs'] topologies: `(List of segments: <required>)` - Defines the location for the volume.
+        :param Sequence['ExternalVolumeTopologyRequestRequiredTopologyArgs'] topologies: Defines the location for the volume.
         """
         pulumi.set(__self__, "topologies", topologies)
 
     @property
     @pulumi.getter
     def topologies(self) -> Sequence['outputs.ExternalVolumeTopologyRequestRequiredTopology']:
         """
-        `(List of segments: <required>)` - Defines the location for the volume.
+        Defines the location for the volume.
         """
         return pulumi.get(self, "topologies")
 
 
 @pulumi.output_type
 class ExternalVolumeTopologyRequestRequiredTopology(dict):
     def __init__(__self__, *,
                  segments: Mapping[str, str]):
         """
-        :param Mapping[str, str] segments: `(map[string]string)` - Define the attributes for the topology request.
-               
-               In addition to the above arguments, the following attributes are exported and
-               can be referenced:
+        :param Mapping[str, str] segments: Define the attributes for the topology request.
         """
         pulumi.set(__self__, "segments", segments)
 
     @property
     @pulumi.getter
     def segments(self) -> Mapping[str, str]:
         """
-        `(map[string]string)` - Define the attributes for the topology request.
-
-        In addition to the above arguments, the following attributes are exported and
-        can be referenced:
+        Define the attributes for the topology request.
         """
         return pulumi.get(self, "segments")
 
 
 @pulumi.output_type
 class JobHcl2(dict):
     @staticmethod
@@ -1746,32 +1670,20 @@
         return pulumi.get(self, "mount_flags")
 
 
 @pulumi.output_type
 class VolumeTopology(dict):
     def __init__(__self__, *,
                  segments: Optional[Mapping[str, str]] = None):
-        """
-        :param Mapping[str, str] segments: `(map[string]string)` - Define the attributes for the topology request.
-               
-               In addition to the above arguments, the following attributes are exported and
-               can be referenced:
-        """
         if segments is not None:
             pulumi.set(__self__, "segments", segments)
 
     @property
     @pulumi.getter
     def segments(self) -> Optional[Mapping[str, str]]:
-        """
-        `(map[string]string)` - Define the attributes for the topology request.
-
-        In addition to the above arguments, the following attributes are exported and
-        can be referenced:
-        """
         return pulumi.get(self, "segments")
 
 
 @pulumi.output_type
 class VolumeTopologyRequest(dict):
     def __init__(__self__, *,
                  required: Optional['outputs.VolumeTopologyRequestRequired'] = None):
@@ -1791,47 +1703,41 @@
 
 
 @pulumi.output_type
 class VolumeTopologyRequestRequired(dict):
     def __init__(__self__, *,
                  topologies: Sequence['outputs.VolumeTopologyRequestRequiredTopology']):
         """
-        :param Sequence['VolumeTopologyRequestRequiredTopologyArgs'] topologies: `(List of segments: <required>)` - Defines the location for the volume.
+        :param Sequence['VolumeTopologyRequestRequiredTopologyArgs'] topologies: Defines the location for the volume.
         """
         pulumi.set(__self__, "topologies", topologies)
 
     @property
     @pulumi.getter
     def topologies(self) -> Sequence['outputs.VolumeTopologyRequestRequiredTopology']:
         """
-        `(List of segments: <required>)` - Defines the location for the volume.
+        Defines the location for the volume.
         """
         return pulumi.get(self, "topologies")
 
 
 @pulumi.output_type
 class VolumeTopologyRequestRequiredTopology(dict):
     def __init__(__self__, *,
                  segments: Mapping[str, str]):
         """
-        :param Mapping[str, str] segments: `(map[string]string)` - Define the attributes for the topology request.
-               
-               In addition to the above arguments, the following attributes are exported and
-               can be referenced:
+        :param Mapping[str, str] segments: Define attributes for the topology request.
         """
         pulumi.set(__self__, "segments", segments)
 
     @property
     @pulumi.getter
     def segments(self) -> Mapping[str, str]:
         """
-        `(map[string]string)` - Define the attributes for the topology request.
-
-        In addition to the above arguments, the following attributes are exported and
-        can be referenced:
+        Define attributes for the topology request.
         """
         return pulumi.get(self, "segments")
 
 
 @pulumi.output_type
 class GetAclPoliciesPolicyResult(dict):
     def __init__(__self__, *,
```

### Comparing `pulumi_nomad-2.3.0a1713561631/pulumi_nomad/provider.py` & `pulumi_nomad-2.3.0a1713899842/pulumi_nomad/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_nomad-2.3.0a1713561631/pulumi_nomad/quote_specification.py` & `pulumi_nomad-2.3.0a1713899842/pulumi_nomad/quote_specification.py`

 * *Files 4% similar despite different names*

```diff
@@ -140,15 +140,14 @@
         """
         Manages a quota specification in a Nomad cluster.
 
         ## Example Usage
 
         Registering a quota specification:
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_nomad as nomad
 
         prod_api = nomad.QuoteSpecification("prod_api",
             name="prod-api",
             description="Production instances of backend API servers",
@@ -156,15 +155,14 @@
                 region="global",
                 region_limit=nomad.QuoteSpecificationLimitRegionLimitArgs(
                     cpu=2400,
                     memory_mb=1200,
                 ),
             )])
         ```
-        <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] description: `(string: "")` - A description of the quota specification.
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['QuoteSpecificationLimitArgs']]]] limits: `(block: <required>)` - A block of quota limits to enforce. Can
                be repeated. See below for the structure of this block.
         :param pulumi.Input[str] name: `(string: <required>)` - A unique name for the quota specification.
@@ -178,15 +176,14 @@
         """
         Manages a quota specification in a Nomad cluster.
 
         ## Example Usage
 
         Registering a quota specification:
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_nomad as nomad
 
         prod_api = nomad.QuoteSpecification("prod_api",
             name="prod-api",
             description="Production instances of backend API servers",
@@ -194,15 +191,14 @@
                 region="global",
                 region_limit=nomad.QuoteSpecificationLimitRegionLimitArgs(
                     cpu=2400,
                     memory_mb=1200,
                 ),
             )])
         ```
-        <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param QuoteSpecificationArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
```

### Comparing `pulumi_nomad-2.3.0a1713561631/pulumi_nomad/scheduler_config.py` & `pulumi_nomad-2.3.0a1713899842/pulumi_nomad/scheduler_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -140,30 +140,28 @@
         action should do. The cluster will be left as-is and only the state reference
         will be removed.
 
         ## Example Usage
 
         Set cluster scheduler configuration:
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_nomad as nomad
 
         config = nomad.SchedulerConfig("config",
             scheduler_algorithm="spread",
             memory_oversubscription_enabled=True,
             preemption_config={
                 "system_scheduler_enabled": True,
                 "batch_scheduler_enabled": True,
                 "service_scheduler_enabled": True,
                 "sysbatch_scheduler_enabled": True,
             })
         ```
-        <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[bool] memory_oversubscription_enabled: `(bool: false)` - When `true`, tasks may exceed their reserved memory limit.
         :param pulumi.Input[Mapping[str, pulumi.Input[bool]]] preemption_config: `(map[string]bool)` - Options to enable preemption for various schedulers.
         :param pulumi.Input[str] scheduler_algorithm: `(string: "binpack")` - Specifies whether scheduler binpacks or spreads allocations on available nodes. Possible values are `binpack` and `spread`.
         """
@@ -181,30 +179,28 @@
         action should do. The cluster will be left as-is and only the state reference
         will be removed.
 
         ## Example Usage
 
         Set cluster scheduler configuration:
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_nomad as nomad
 
         config = nomad.SchedulerConfig("config",
             scheduler_algorithm="spread",
             memory_oversubscription_enabled=True,
             preemption_config={
                 "system_scheduler_enabled": True,
                 "batch_scheduler_enabled": True,
                 "service_scheduler_enabled": True,
                 "sysbatch_scheduler_enabled": True,
             })
         ```
-        <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param SchedulerConfigArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
```

### Comparing `pulumi_nomad-2.3.0a1713561631/pulumi_nomad/sentinel_policy.py` & `pulumi_nomad-2.3.0a1713899842/pulumi_nomad/sentinel_policy.py`

 * *Files 1% similar despite different names*

```diff
@@ -215,15 +215,14 @@
         Manages a Sentinel policy registered in Nomad.
 
         > **Enterprise Only!** This API endpoint and functionality only exists in
            Nomad Enterprise. This is not present in the open source version of Nomad.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_nomad as nomad
 
         exec_only = nomad.SentinelPolicy("exec-only",
             name="exec-only",
             description="Only allow jobs that are based on an exec driver.",
@@ -237,15 +236,14 @@
                 }
             }
         }
         \"\"\",
             scope="submit-job",
             enforcement_level="soft-mandatory")
         ```
-        <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] description: `(string: "")` - A description of the policy.
                
                [scope]: https://www.nomadproject.io/guides/sentinel-policy.html#policy-scope
                [enforcement-level]: https://www.nomadproject.io/guides/sentinel-policy.html#enforcement-level
@@ -265,15 +263,14 @@
         Manages a Sentinel policy registered in Nomad.
 
         > **Enterprise Only!** This API endpoint and functionality only exists in
            Nomad Enterprise. This is not present in the open source version of Nomad.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_nomad as nomad
 
         exec_only = nomad.SentinelPolicy("exec-only",
             name="exec-only",
             description="Only allow jobs that are based on an exec driver.",
@@ -287,15 +284,14 @@
                 }
             }
         }
         \"\"\",
             scope="submit-job",
             enforcement_level="soft-mandatory")
         ```
-        <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param SentinelPolicyArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
```

### Comparing `pulumi_nomad-2.3.0a1713561631/pulumi_nomad/variable.py` & `pulumi_nomad-2.3.0a1713899842/pulumi_nomad/variable.py`

 * *Files 3% similar despite different names*

```diff
@@ -131,45 +131,41 @@
                  path: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         ## Example Usage
 
         Creating a variable in the default namespace:
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_nomad as nomad
 
         example = nomad.Variable("example",
             path="some/path/of/your/choosing",
             items={
                 "example_key": "example_value",
             })
         ```
-        <!--End PulumiCodeChooser -->
 
         Creating a variable in a custom namespace:
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_nomad as nomad
 
         example = nomad.Namespace("example",
             name="example",
             description="Example namespace.")
         example_variable = nomad.Variable("example",
             path="some/path/of/your/choosing",
             namespace=example.name,
             items={
                 "example_key": "example_value",
             })
         ```
-        <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[Mapping[str, Any]] items: `(map[string]string: <required>)` - An arbitrary map of items to create in the variable.
         :param pulumi.Input[str] namespace: `(string: "default")` - The namepsace to create the variable in.
         :param pulumi.Input[str] path: `(string: <required>)` - A unique path to create the variable at.
         """
@@ -180,45 +176,41 @@
                  args: VariableArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         ## Example Usage
 
         Creating a variable in the default namespace:
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_nomad as nomad
 
         example = nomad.Variable("example",
             path="some/path/of/your/choosing",
             items={
                 "example_key": "example_value",
             })
         ```
-        <!--End PulumiCodeChooser -->
 
         Creating a variable in a custom namespace:
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_nomad as nomad
 
         example = nomad.Namespace("example",
             name="example",
             description="Example namespace.")
         example_variable = nomad.Variable("example",
             path="some/path/of/your/choosing",
             namespace=example.name,
             items={
                 "example_key": "example_value",
             })
         ```
-        <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param VariableArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
```

### Comparing `pulumi_nomad-2.3.0a1713561631/pulumi_nomad/volume.py` & `pulumi_nomad-2.3.0a1713899842/pulumi_nomad/volume.py`

 * *Files 2% similar despite different names*

```diff
@@ -314,31 +314,22 @@
                - `single-node-writer`
                - `multi-node-reader-only`
                - `multi-node-single-writer`
                - `multi-node-multi-writer`
         :param pulumi.Input[str] attachment_mode: `(string: <otional>)` - **Deprecated**. Use `capability` block instead. The storage API that will be used by the volume.
         :param pulumi.Input[Sequence[pulumi.Input['VolumeCapabilityArgs']]] capabilities: `(``Capability``: <required>)` - Options for validating the capability of a volume.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] context: `(map[string]string: <optional>)` - An optional key-value map of strings passed directly to the CSI plugin to validate the volume.
-        :param pulumi.Input[bool] controller_required: `(boolean)`
-        :param pulumi.Input[int] controllers_expected: `(integer)`
-        :param pulumi.Input[int] controllers_healthy: `(integer)`
         :param pulumi.Input[bool] deregister_on_destroy: `(boolean: true)` - If true, the volume will be deregistered on destroy.
         :param pulumi.Input[str] external_id: `(string: <required>)` - The ID of the physical volume from the storage provider.
         :param pulumi.Input['VolumeMountOptionsArgs'] mount_options: `(block: <optional>)` Options for mounting `block-device` volumes without a pre-formatted file system.
         :param pulumi.Input[str] name: `(string: <required>)` - The display name for the volume.
         :param pulumi.Input[str] namespace: `(string: "default")` - The namespace in which to register the volume.
-        :param pulumi.Input[int] nodes_expected: `(integer)`
-        :param pulumi.Input[int] nodes_healthy: `(integer)`
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] parameters: `(map[string]string: <optional>)` - An optional key-value map of strings passed directly to the CSI plugin to configure the volume.
         :param pulumi.Input[str] plugin_id: `(string: <required>)` - The ID of the Nomad plugin for registering this volume.
-        :param pulumi.Input[str] plugin_provider: `(string)`
-        :param pulumi.Input[str] plugin_provider_version: `(string)`
-        :param pulumi.Input[bool] schedulable: `(boolean)`
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] secrets: `(map[string]string: <optional>)` - An optional key-value map of strings used as credentials for publishing and unpublishing volumes.
-        :param pulumi.Input[Sequence[pulumi.Input['VolumeTopologyArgs']]] topologies: `(List of topologies)`
         :param pulumi.Input['VolumeTopologyRequestArgs'] topology_request: `(``TopologyRequest``: <optional>)` - Specify locations (region, zone, rack, etc.) where the provisioned volume is accessible from.
         :param pulumi.Input[str] type: `(string: <required>)` - The type of the volume. Currently, only `csi` is supported.
         :param pulumi.Input[str] volume_id: `(string: <required>)` - The unique ID of the volume.
         """
         if access_mode is not None:
             warnings.warn("""use capability instead""", DeprecationWarning)
             pulumi.log.warn("""access_mode is deprecated: use capability instead""")
@@ -452,41 +443,32 @@
     @context.setter
     def context(self, value: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]):
         pulumi.set(self, "context", value)
 
     @property
     @pulumi.getter(name="controllerRequired")
     def controller_required(self) -> Optional[pulumi.Input[bool]]:
-        """
-        `(boolean)`
-        """
         return pulumi.get(self, "controller_required")
 
     @controller_required.setter
     def controller_required(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "controller_required", value)
 
     @property
     @pulumi.getter(name="controllersExpected")
     def controllers_expected(self) -> Optional[pulumi.Input[int]]:
-        """
-        `(integer)`
-        """
         return pulumi.get(self, "controllers_expected")
 
     @controllers_expected.setter
     def controllers_expected(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "controllers_expected", value)
 
     @property
     @pulumi.getter(name="controllersHealthy")
     def controllers_healthy(self) -> Optional[pulumi.Input[int]]:
-        """
-        `(integer)`
-        """
         return pulumi.get(self, "controllers_healthy")
 
     @controllers_healthy.setter
     def controllers_healthy(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "controllers_healthy", value)
 
     @property
@@ -548,29 +530,23 @@
     @namespace.setter
     def namespace(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "namespace", value)
 
     @property
     @pulumi.getter(name="nodesExpected")
     def nodes_expected(self) -> Optional[pulumi.Input[int]]:
-        """
-        `(integer)`
-        """
         return pulumi.get(self, "nodes_expected")
 
     @nodes_expected.setter
     def nodes_expected(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "nodes_expected", value)
 
     @property
     @pulumi.getter(name="nodesHealthy")
     def nodes_healthy(self) -> Optional[pulumi.Input[int]]:
-        """
-        `(integer)`
-        """
         return pulumi.get(self, "nodes_healthy")
 
     @nodes_healthy.setter
     def nodes_healthy(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "nodes_healthy", value)
 
     @property
@@ -596,41 +572,32 @@
     @plugin_id.setter
     def plugin_id(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "plugin_id", value)
 
     @property
     @pulumi.getter(name="pluginProvider")
     def plugin_provider(self) -> Optional[pulumi.Input[str]]:
-        """
-        `(string)`
-        """
         return pulumi.get(self, "plugin_provider")
 
     @plugin_provider.setter
     def plugin_provider(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "plugin_provider", value)
 
     @property
     @pulumi.getter(name="pluginProviderVersion")
     def plugin_provider_version(self) -> Optional[pulumi.Input[str]]:
-        """
-        `(string)`
-        """
         return pulumi.get(self, "plugin_provider_version")
 
     @plugin_provider_version.setter
     def plugin_provider_version(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "plugin_provider_version", value)
 
     @property
     @pulumi.getter
     def schedulable(self) -> Optional[pulumi.Input[bool]]:
-        """
-        `(boolean)`
-        """
         return pulumi.get(self, "schedulable")
 
     @schedulable.setter
     def schedulable(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "schedulable", value)
 
     @property
@@ -644,17 +611,14 @@
     @secrets.setter
     def secrets(self, value: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]):
         pulumi.set(self, "secrets", value)
 
     @property
     @pulumi.getter
     def topologies(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['VolumeTopologyArgs']]]]:
-        """
-        `(List of topologies)`
-        """
         return pulumi.get(self, "topologies")
 
     @topologies.setter
     def topologies(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['VolumeTopologyArgs']]]]):
         pulumi.set(self, "topologies", value)
 
     @property
@@ -716,15 +680,14 @@
                  volume_id: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         ## Example Usage
 
         Registering a volume:
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_nomad as nomad
 
         # It can sometimes be helpful to wait for a particular plugin to be available
         ebs = nomad.get_plugin(plugin_id="aws-ebs0",
             wait_for_healthy=True)
@@ -756,15 +719,14 @@
                             },
                         ),
                     ],
                 ),
             ),
             opts=pulumi.ResourceOptions(depends_on=[ebs]))
         ```
-        <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] access_mode: `(string: <optional>)` - **Deprecated**. Use `capability` block instead. Defines whether a volume should be available concurrently. Possible values are:
                - `single-node-reader-only`
                - `single-node-writer`
                - `multi-node-reader-only`
@@ -792,15 +754,14 @@
                  args: VolumeArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         ## Example Usage
 
         Registering a volume:
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_nomad as nomad
 
         # It can sometimes be helpful to wait for a particular plugin to be available
         ebs = nomad.get_plugin(plugin_id="aws-ebs0",
             wait_for_healthy=True)
@@ -832,15 +793,14 @@
                             },
                         ),
                     ],
                 ),
             ),
             opts=pulumi.ResourceOptions(depends_on=[ebs]))
         ```
-        <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param VolumeArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
@@ -955,31 +915,22 @@
                - `single-node-writer`
                - `multi-node-reader-only`
                - `multi-node-single-writer`
                - `multi-node-multi-writer`
         :param pulumi.Input[str] attachment_mode: `(string: <otional>)` - **Deprecated**. Use `capability` block instead. The storage API that will be used by the volume.
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['VolumeCapabilityArgs']]]] capabilities: `(``Capability``: <required>)` - Options for validating the capability of a volume.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] context: `(map[string]string: <optional>)` - An optional key-value map of strings passed directly to the CSI plugin to validate the volume.
-        :param pulumi.Input[bool] controller_required: `(boolean)`
-        :param pulumi.Input[int] controllers_expected: `(integer)`
-        :param pulumi.Input[int] controllers_healthy: `(integer)`
         :param pulumi.Input[bool] deregister_on_destroy: `(boolean: true)` - If true, the volume will be deregistered on destroy.
         :param pulumi.Input[str] external_id: `(string: <required>)` - The ID of the physical volume from the storage provider.
         :param pulumi.Input[pulumi.InputType['VolumeMountOptionsArgs']] mount_options: `(block: <optional>)` Options for mounting `block-device` volumes without a pre-formatted file system.
         :param pulumi.Input[str] name: `(string: <required>)` - The display name for the volume.
         :param pulumi.Input[str] namespace: `(string: "default")` - The namespace in which to register the volume.
-        :param pulumi.Input[int] nodes_expected: `(integer)`
-        :param pulumi.Input[int] nodes_healthy: `(integer)`
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] parameters: `(map[string]string: <optional>)` - An optional key-value map of strings passed directly to the CSI plugin to configure the volume.
         :param pulumi.Input[str] plugin_id: `(string: <required>)` - The ID of the Nomad plugin for registering this volume.
-        :param pulumi.Input[str] plugin_provider: `(string)`
-        :param pulumi.Input[str] plugin_provider_version: `(string)`
-        :param pulumi.Input[bool] schedulable: `(boolean)`
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] secrets: `(map[string]string: <optional>)` - An optional key-value map of strings used as credentials for publishing and unpublishing volumes.
-        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['VolumeTopologyArgs']]]] topologies: `(List of topologies)`
         :param pulumi.Input[pulumi.InputType['VolumeTopologyRequestArgs']] topology_request: `(``TopologyRequest``: <optional>)` - Specify locations (region, zone, rack, etc.) where the provisioned volume is accessible from.
         :param pulumi.Input[str] type: `(string: <required>)` - The type of the volume. Currently, only `csi` is supported.
         :param pulumi.Input[str] volume_id: `(string: <required>)` - The unique ID of the volume.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _VolumeState.__new__(_VolumeState)
@@ -1052,33 +1003,24 @@
         `(map[string]string: <optional>)` - An optional key-value map of strings passed directly to the CSI plugin to validate the volume.
         """
         return pulumi.get(self, "context")
 
     @property
     @pulumi.getter(name="controllerRequired")
     def controller_required(self) -> pulumi.Output[bool]:
-        """
-        `(boolean)`
-        """
         return pulumi.get(self, "controller_required")
 
     @property
     @pulumi.getter(name="controllersExpected")
     def controllers_expected(self) -> pulumi.Output[int]:
-        """
-        `(integer)`
-        """
         return pulumi.get(self, "controllers_expected")
 
     @property
     @pulumi.getter(name="controllersHealthy")
     def controllers_healthy(self) -> pulumi.Output[int]:
-        """
-        `(integer)`
-        """
         return pulumi.get(self, "controllers_healthy")
 
     @property
     @pulumi.getter(name="deregisterOnDestroy")
     def deregister_on_destroy(self) -> pulumi.Output[Optional[bool]]:
         """
         `(boolean: true)` - If true, the volume will be deregistered on destroy.
@@ -1116,25 +1058,19 @@
         `(string: "default")` - The namespace in which to register the volume.
         """
         return pulumi.get(self, "namespace")
 
     @property
     @pulumi.getter(name="nodesExpected")
     def nodes_expected(self) -> pulumi.Output[int]:
-        """
-        `(integer)`
-        """
         return pulumi.get(self, "nodes_expected")
 
     @property
     @pulumi.getter(name="nodesHealthy")
     def nodes_healthy(self) -> pulumi.Output[int]:
-        """
-        `(integer)`
-        """
         return pulumi.get(self, "nodes_healthy")
 
     @property
     @pulumi.getter
     def parameters(self) -> pulumi.Output[Optional[Mapping[str, str]]]:
         """
         `(map[string]string: <optional>)` - An optional key-value map of strings passed directly to the CSI plugin to configure the volume.
@@ -1148,49 +1084,37 @@
         `(string: <required>)` - The ID of the Nomad plugin for registering this volume.
         """
         return pulumi.get(self, "plugin_id")
 
     @property
     @pulumi.getter(name="pluginProvider")
     def plugin_provider(self) -> pulumi.Output[str]:
-        """
-        `(string)`
-        """
         return pulumi.get(self, "plugin_provider")
 
     @property
     @pulumi.getter(name="pluginProviderVersion")
     def plugin_provider_version(self) -> pulumi.Output[str]:
-        """
-        `(string)`
-        """
         return pulumi.get(self, "plugin_provider_version")
 
     @property
     @pulumi.getter
     def schedulable(self) -> pulumi.Output[bool]:
-        """
-        `(boolean)`
-        """
         return pulumi.get(self, "schedulable")
 
     @property
     @pulumi.getter
     def secrets(self) -> pulumi.Output[Optional[Mapping[str, str]]]:
         """
         `(map[string]string: <optional>)` - An optional key-value map of strings used as credentials for publishing and unpublishing volumes.
         """
         return pulumi.get(self, "secrets")
 
     @property
     @pulumi.getter
     def topologies(self) -> pulumi.Output[Sequence['outputs.VolumeTopology']]:
-        """
-        `(List of topologies)`
-        """
         return pulumi.get(self, "topologies")
 
     @property
     @pulumi.getter(name="topologyRequest")
     def topology_request(self) -> pulumi.Output[Optional['outputs.VolumeTopologyRequest']]:
         """
         `(``TopologyRequest``: <optional>)` - Specify locations (region, zone, rack, etc.) where the provisioned volume is accessible from.
```

### Comparing `pulumi_nomad-2.3.0a1713561631/pulumi_nomad.egg-info/PKG-INFO` & `pulumi_nomad-2.3.0a1713899842/pulumi_nomad.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_nomad
-Version: 2.3.0a1713561631
+Version: 2.3.0a1713899842
 Summary: A Pulumi package for creating and managing nomad cloud resources.
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.io
 Project-URL: Repository, https://github.com/pulumi/pulumi-nomad
 Keywords: pulumi,nomad
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_nomad-2.3.0a1713561631/pulumi_nomad.egg-info/SOURCES.txt` & `pulumi_nomad-2.3.0a1713899842/pulumi_nomad.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_nomad-2.3.0a1713561631/pyproject.toml` & `pulumi_nomad-2.3.0a1713899842/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [project]
   name = "pulumi_nomad"
   description = "A Pulumi package for creating and managing nomad cloud resources."
   dependencies = ["parver>=0.2.1", "pulumi>=3.0.0,<4.0.0", "semver>=2.8.1"]
   keywords = ["pulumi", "nomad"]
   readme = "README.md"
   requires-python = ">=3.8"
-  version = "2.3.0a1713561631"
+  version = "2.3.0a1713899842"
   [project.license]
     text = "Apache-2.0"
   [project.urls]
     Homepage = "https://pulumi.io"
     Repository = "https://github.com/pulumi/pulumi-nomad"
 
 [build-system]
```

