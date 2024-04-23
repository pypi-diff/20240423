# Comparing `tmp/pulumi_vault-6.2.0a1713339773.tar.gz` & `tmp/pulumi_vault-6.2.0a1713561465.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_vault-6.2.0a1713339773.tar", last modified: Wed Apr 17 07:47:16 2024, max compression
+gzip compressed data, was "pulumi_vault-6.2.0a1713561465.tar", last modified: Fri Apr 19 21:28:20 2024, max compression
```

## Comparing `pulumi_vault-6.2.0a1713339773.tar` & `pulumi_vault-6.2.0a1713561465.tar`

### file list

```diff
@@ -1,289 +1,289 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:47:16.789774 pulumi_vault-6.2.0a1713339773/
--rw-r--r--   0 runner    (1001) docker     (127)     4857 2024-04-17 07:47:16.789774 pulumi_vault-6.2.0a1713339773/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4399 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:47:16.741773 pulumi_vault-6.2.0a1713339773/pulumi_vault/
--rw-r--r--   0 runner    (1001) docker     (127)    31033 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    73552 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/_utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:47:16.745773 pulumi_vault-6.2.0a1713339773/pulumi_vault/ad/
--rw-r--r--   0 runner    (1001) docker     (127)      394 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/ad/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6522 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/ad/get_access_credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)    92297 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/ad/secret_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)    23836 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/ad/secret_library.py
--rw-r--r--   0 runner    (1001) docker     (127)    20632 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/ad/secret_role.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:47:16.745773 pulumi_vault-6.2.0a1713339773/pulumi_vault/alicloud/
--rw-r--r--   0 runner    (1001) docker     (127)      302 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/alicloud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    45928 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/alicloud/auth_backend_role.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:47:16.745773 pulumi_vault-6.2.0a1713339773/pulumi_vault/approle/
--rw-r--r--   0 runner    (1001) docker     (127)      419 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/approle/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23505 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/approle/auth_backend_login.py
--rw-r--r--   0 runner    (1001) docker     (127)    56646 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/approle/auth_backend_role.py
--rw-r--r--   0 runner    (1001) docker     (127)    31940 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/approle/auth_backend_role_secret_id.py
--rw-r--r--   0 runner    (1001) docker     (127)     5916 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/approle/get_auth_backend_role_id.py
--rw-r--r--   0 runner    (1001) docker     (127)    20655 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/audit.py
--rw-r--r--   0 runner    (1001) docker     (127)    10369 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/audit_request_header.py
--rw-r--r--   0 runner    (1001) docker     (127)    21605 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/auth_backend.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:47:16.749773 pulumi_vault-6.2.0a1713339773/pulumi_vault/aws/
--rw-r--r--   0 runner    (1001) docker     (127)      805 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/aws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18369 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/aws/auth_backend_cert.py
--rw-r--r--   0 runner    (1001) docker     (127)    32902 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/aws/auth_backend_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    23288 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/aws/auth_backend_config_identity.py
--rw-r--r--   0 runner    (1001) docker     (127)    17226 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/aws/auth_backend_identity_whitelist.py
--rw-r--r--   0 runner    (1001) docker     (127)    43043 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/aws/auth_backend_login.py
--rw-r--r--   0 runner    (1001) docker     (127)   110667 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/aws/auth_backend_role.py
--rw-r--r--   0 runner    (1001) docker     (127)    26592 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/aws/auth_backend_role_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)    16794 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/aws/auth_backend_roletag_blacklist.py
--rw-r--r--   0 runner    (1001) docker     (127)    15623 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/aws/auth_backend_sts_role.py
--rw-r--r--   0 runner    (1001) docker     (127)    12282 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/aws/get_access_credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)     4742 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/aws/get_static_access_credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)    49429 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/aws/secret_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)    48260 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/aws/secret_backend_role.py
--rw-r--r--   0 runner    (1001) docker     (127)    17927 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/aws/secret_backend_static_role.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:47:16.749773 pulumi_vault-6.2.0a1713339773/pulumi_vault/azure/
--rw-r--r--   0 runner    (1001) docker     (127)      471 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/azure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2564 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/azure/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    23762 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/azure/auth_backend_config.py
--rw-r--r--   0 runner    (1001) docker     (127)    64878 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/azure/auth_backend_role.py
--rw-r--r--   0 runner    (1001) docker     (127)    29406 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/azure/backend.py
--rw-r--r--   0 runner    (1001) docker     (127)    39236 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/azure/backend_role.py
--rw-r--r--   0 runner    (1001) docker     (127)    17943 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/azure/get_access_credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)     3097 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/azure/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    83407 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/cert_auth_backend_role.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:47:16.753773 pulumi_vault-6.2.0a1713339773/pulumi_vault/config/
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3140 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/config/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1361 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/config/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    42626 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/config/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    22482 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/config/ui_custom_message.py
--rw-r--r--   0 runner    (1001) docker     (127)     6525 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/config/vars.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:47:16.753773 pulumi_vault-6.2.0a1713339773/pulumi_vault/consul/
--rw-r--r--   0 runner    (1001) docker     (127)      334 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/consul/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    39828 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/consul/secret_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)    41615 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/consul/secret_backend_role.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:47:16.753773 pulumi_vault-6.2.0a1713339773/pulumi_vault/database/
--rw-r--r--   0 runner    (1001) docker     (127)      461 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/database/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   298321 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/database/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)   261078 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/database/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    73279 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/database/secret_backend_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)    36912 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/database/secret_backend_role.py
--rw-r--r--   0 runner    (1001) docker     (127)    30731 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/database/secret_backend_static_role.py
--rw-r--r--   0 runner    (1001) docker     (127)    98130 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/database/secrets_mount.py
--rw-r--r--   0 runner    (1001) docker     (127)    16697 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/egp_policy.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:47:16.757773 pulumi_vault-6.2.0a1713339773/pulumi_vault/gcp/
--rw-r--r--   0 runner    (1001) docker     (127)      552 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/gcp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14698 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/gcp/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    38638 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/gcp/auth_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)    73886 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/gcp/auth_backend_role.py
--rw-r--r--   0 runner    (1001) docker     (127)    22936 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/gcp/get_auth_backend_role.py
--rw-r--r--   0 runner    (1001) docker     (127)    12613 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/gcp/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    24908 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/gcp/secret_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)    18919 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/gcp/secret_impersonated_account.py
--rw-r--r--   0 runner    (1001) docker     (127)    26079 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/gcp/secret_roleset.py
--rw-r--r--   0 runner    (1001) docker     (127)    27423 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/gcp/secret_static_account.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:47:16.757773 pulumi_vault-6.2.0a1713339773/pulumi_vault/generic/
--rw-r--r--   0 runner    (1001) docker     (127)      341 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/generic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    39221 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/generic/endpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)    10380 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/generic/get_secret.py
--rw-r--r--   0 runner    (1001) docker     (127)    22847 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/generic/secret.py
--rw-r--r--   0 runner    (1001) docker     (127)     7897 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/get_auth_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)     5587 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/get_auth_backends.py
--rw-r--r--   0 runner    (1001) docker     (127)     7495 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/get_namespace.py
--rw-r--r--   0 runner    (1001) docker     (127)     4666 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/get_namespaces.py
--rw-r--r--   0 runner    (1001) docker     (127)     7389 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/get_nomad_access_token.py
--rw-r--r--   0 runner    (1001) docker     (127)     5136 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/get_policy_document.py
--rw-r--r--   0 runner    (1001) docker     (127)    10007 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/get_raft_autopilot_state.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:47:16.761774 pulumi_vault-6.2.0a1713339773/pulumi_vault/github/
--rw-r--r--   0 runner    (1001) docker     (127)      382 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/github/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8032 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/github/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    56571 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/github/auth_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)     7320 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/github/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    15482 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/github/team.py
--rw-r--r--   0 runner    (1001) docker     (127)    15280 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/github/user.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:47:16.765774 pulumi_vault-6.2.0a1713339773/pulumi_vault/identity/
--rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/identity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19932 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/identity/entity.py
--rw-r--r--   0 runner    (1001) docker     (127)    18641 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/identity/entity_alias.py
--rw-r--r--   0 runner    (1001) docker     (127)    20083 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/identity/entity_policies.py
--rw-r--r--   0 runner    (1001) docker     (127)    14491 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/identity/get_entity.py
--rw-r--r--   0 runner    (1001) docker     (127)    18096 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/identity/get_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     6011 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/identity/get_oidc_client_creds.py
--rw-r--r--   0 runner    (1001) docker     (127)    13522 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/identity/get_oidc_openid_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     6000 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/identity/get_oidc_public_keys.py
--rw-r--r--   0 runner    (1001) docker     (127)    37780 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/identity/group.py
--rw-r--r--   0 runner    (1001) docker     (127)    17404 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/identity/group_alias.py
--rw-r--r--   0 runner    (1001) docker     (127)    20554 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/identity/group_member_entity_ids.py
--rw-r--r--   0 runner    (1001) docker     (127)    20180 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/identity/group_member_group_ids.py
--rw-r--r--   0 runner    (1001) docker     (127)    20431 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/identity/group_policies.py
--rw-r--r--   0 runner    (1001) docker     (127)    25146 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/identity/mfa_duo.py
--rw-r--r--   0 runner    (1001) docker     (127)    23785 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/identity/mfa_login_enforcement.py
--rw-r--r--   0 runner    (1001) docker     (127)    23189 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/identity/mfa_okta.py
--rw-r--r--   0 runner    (1001) docker     (127)    23924 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/identity/mfa_pingid.py
--rw-r--r--   0 runner    (1001) docker     (127)    29583 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/identity/mfa_totp.py
--rw-r--r--   0 runner    (1001) docker     (127)    12422 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/identity/oidc.py
--rw-r--r--   0 runner    (1001) docker     (127)    15261 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/identity/oidc_assignment.py
--rw-r--r--   0 runner    (1001) docker     (127)    29879 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/identity/oidc_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    21120 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/identity/oidc_key.py
--rw-r--r--   0 runner    (1001) docker     (127)    12876 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/identity/oidc_key_allowed_client_id.py
--rw-r--r--   0 runner    (1001) docker     (127)    24334 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/identity/oidc_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)    22020 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/identity/oidc_role.py
--rw-r--r--   0 runner    (1001) docker     (127)    14701 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/identity/oidc_scope.py
--rw-r--r--   0 runner    (1001) docker     (127)     4154 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/identity/outputs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:47:16.765774 pulumi_vault-6.2.0a1713339773/pulumi_vault/jwt/
--rw-r--r--   0 runner    (1001) docker     (127)      375 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/jwt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8032 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/jwt/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    66520 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/jwt/auth_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)    97651 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/jwt/auth_backend_role.py
--rw-r--r--   0 runner    (1001) docker     (127)     7320 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/jwt/outputs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:47:16.765774 pulumi_vault-6.2.0a1713339773/pulumi_vault/kmip/
--rw-r--r--   0 runner    (1001) docker     (127)      354 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/kmip/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    37931 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/kmip/secret_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)    54561 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/kmip/secret_role.py
--rw-r--r--   0 runner    (1001) docker     (127)    14926 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/kmip/secret_scope.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:47:16.769774 pulumi_vault-6.2.0a1713339773/pulumi_vault/kubernetes/
--rw-r--r--   0 runner    (1001) docker     (127)      519 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/kubernetes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    31330 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/kubernetes/auth_backend_config.py
--rw-r--r--   0 runner    (1001) docker     (127)    57046 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/kubernetes/auth_backend_role.py
--rw-r--r--   0 runner    (1001) docker     (127)    10609 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/kubernetes/get_auth_backend_config.py
--rw-r--r--   0 runner    (1001) docker     (127)    21357 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/kubernetes/get_auth_backend_role.py
--rw-r--r--   0 runner    (1001) docker     (127)    13847 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/kubernetes/get_service_account_token.py
--rw-r--r--   0 runner    (1001) docker     (127)    50850 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/kubernetes/secret_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)    55835 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/kubernetes/secret_backend_role.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:47:16.769774 pulumi_vault-6.2.0a1713339773/pulumi_vault/kv/
--rw-r--r--   0 runner    (1001) docker     (127)      553 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/kv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3628 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/kv/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     7962 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/kv/get_secret.py
--rw-r--r--   0 runner    (1001) docker     (127)     9548 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/kv/get_secret_subkeys_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)     9093 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/kv/get_secret_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)     5993 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/kv/get_secrets_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     7923 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/kv/get_secrets_list_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3639 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/kv/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    16069 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/kv/secret.py
--rw-r--r--   0 runner    (1001) docker     (127)    19135 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/kv/secret_backend_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)    35933 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/kv/secret_v2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:47:16.773774 pulumi_vault-6.2.0a1713339773/pulumi_vault/ldap/
--rw-r--r--   0 runner    (1001) docker     (127)      598 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/ldap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    92297 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/ldap/auth_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)    16577 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/ldap/auth_backend_group.py
--rw-r--r--   0 runner    (1001) docker     (127)    18645 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/ldap/auth_backend_user.py
--rw-r--r--   0 runner    (1001) docker     (127)     6535 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/ldap/get_dynamic_credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)     6722 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/ldap/get_static_credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)    77631 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/ldap/secret_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)    37953 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/ldap/secret_backend_dynamic_role.py
--rw-r--r--   0 runner    (1001) docker     (127)    24038 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/ldap/secret_backend_library_set.py
--rw-r--r--   0 runner    (1001) docker     (127)    24131 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/ldap/secret_backend_static_role.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:47:16.773774 pulumi_vault-6.2.0a1713339773/pulumi_vault/managed/
--rw-r--r--   0 runner    (1001) docker     (127)      334 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/managed/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    29364 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/managed/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    14395 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/managed/keys.py
--rw-r--r--   0 runner    (1001) docker     (127)    25252 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/managed/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    28337 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/mfa_duo.py
--rw-r--r--   0 runner    (1001) docker     (127)    29601 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/mfa_okta.py
--rw-r--r--   0 runner    (1001) docker     (127)    31066 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/mfa_pingid.py
--rw-r--r--   0 runner    (1001) docker     (127)    25442 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/mfa_totp.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:47:16.773774 pulumi_vault-6.2.0a1713339773/pulumi_vault/mongodbatlas/
--rw-r--r--   0 runner    (1001) docker     (127)      326 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/mongodbatlas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16287 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/mongodbatlas/secret_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)    33705 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/mongodbatlas/secret_role.py
--rw-r--r--   0 runner    (1001) docker     (127)    41533 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/mount.py
--rw-r--r--   0 runner    (1001) docker     (127)    18077 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/namespace.py
--rw-r--r--   0 runner    (1001) docker     (127)    42174 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/nomad_secret_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)    20302 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/nomad_secret_role.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:47:16.773774 pulumi_vault-6.2.0a1713339773/pulumi_vault/okta/
--rw-r--r--   0 runner    (1001) docker     (127)      409 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/okta/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3527 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/okta/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    38494 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/okta/auth_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)    15131 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/okta/auth_backend_group.py
--rw-r--r--   0 runner    (1001) docker     (127)    17093 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/okta/auth_backend_user.py
--rw-r--r--   0 runner    (1001) docker     (127)     3083 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/okta/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    13760 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    12329 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/password_policy.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:47:16.781774 pulumi_vault-6.2.0a1713339773/pulumi_vault/pkisecret/
--rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/pkisecret/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2090 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/pkisecret/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    16085 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/pkisecret/backend_config_cluster.py
--rw-r--r--   0 runner    (1001) docker     (127)     8853 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/pkisecret/get_backend_issuer.py
--rw-r--r--   0 runner    (1001) docker     (127)     6538 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/pkisecret/get_backend_issuers.py
--rw-r--r--   0 runner    (1001) docker     (127)     7076 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/pkisecret/get_backend_key.py
--rw-r--r--   0 runner    (1001) docker     (127)     6443 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/pkisecret/get_backend_keys.py
--rw-r--r--   0 runner    (1001) docker     (127)     1631 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/pkisecret/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    49885 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/pkisecret/secret_backend_cert.py
--rw-r--r--   0 runner    (1001) docker     (127)    19122 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/pkisecret/secret_backend_config_ca.py
--rw-r--r--   0 runner    (1001) docker     (127)    17134 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/pkisecret/secret_backend_config_issuers.py
--rw-r--r--   0 runner    (1001) docker     (127)    22199 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/pkisecret/secret_backend_config_urls.py
--rw-r--r--   0 runner    (1001) docker     (127)    36965 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/pkisecret/secret_backend_crl_config.py
--rw-r--r--   0 runner    (1001) docker     (127)    62005 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/pkisecret/secret_backend_intermediate_cert_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    20552 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/pkisecret/secret_backend_intermediate_set_signed.py
--rw-r--r--   0 runner    (1001) docker     (127)    36781 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/pkisecret/secret_backend_issuer.py
--rw-r--r--   0 runner    (1001) docker     (127)    25523 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/pkisecret/secret_backend_key.py
--rw-r--r--   0 runner    (1001) docker     (127)   116321 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/pkisecret/secret_backend_role.py
--rw-r--r--   0 runner    (1001) docker     (127)    69049 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/pkisecret/secret_backend_root_cert.py
--rw-r--r--   0 runner    (1001) docker     (127)    58798 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/pkisecret/secret_backend_root_sign_intermediate.py
--rw-r--r--   0 runner    (1001) docker     (127)    48764 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/pkisecret/secret_backend_sign.py
--rw-r--r--   0 runner    (1001) docker     (127)    10935 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/policy.py
--rw-r--r--   0 runner    (1001) docker     (127)    42332 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    21122 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/quota_lease_count.py
--rw-r--r--   0 runner    (1001) docker     (127)    25727 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/quota_rate_limit.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:47:16.781774 pulumi_vault-6.2.0a1713339773/pulumi_vault/rabbitmq/
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/rabbitmq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5281 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/rabbitmq/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     3853 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/rabbitmq/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    34778 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/rabbitmq/secret_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)    21960 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/rabbitmq/secret_backend_role.py
--rw-r--r--   0 runner    (1001) docker     (127)    30215 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/raft_autopilot.py
--rw-r--r--   0 runner    (1001) docker     (127)    84163 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/raft_snapshot_agent_config.py
--rw-r--r--   0 runner    (1001) docker     (127)    14494 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/rgp_policy.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:47:16.781774 pulumi_vault-6.2.0a1713339773/pulumi_vault/saml/
--rw-r--r--   0 runner    (1001) docker     (127)      330 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/saml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    33638 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/saml/auth_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)    55597 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/saml/auth_backend_role.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:47:16.785774 pulumi_vault-6.2.0a1713339773/pulumi_vault/secrets/
--rw-r--r--   0 runner    (1001) docker     (127)      589 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/secrets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3000 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/secrets/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     3202 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/secrets/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    17933 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/secrets/sync_association.py
--rw-r--r--   0 runner    (1001) docker     (127)    38691 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/secrets/sync_aws_destination.py
--rw-r--r--   0 runner    (1001) docker     (127)    32430 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/secrets/sync_azure_destination.py
--rw-r--r--   0 runner    (1001) docker     (127)    12446 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/secrets/sync_config.py
--rw-r--r--   0 runner    (1001) docker     (127)    26301 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/secrets/sync_gcp_destination.py
--rw-r--r--   0 runner    (1001) docker     (127)    32305 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/secrets/sync_gh_destination.py
--rw-r--r--   0 runner    (1001) docker     (127)    15288 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/secrets/sync_github_apps.py
--rw-r--r--   0 runner    (1001) docker     (127)    26768 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/secrets/sync_vercel_destination.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:47:16.785774 pulumi_vault-6.2.0a1713339773/pulumi_vault/ssh/
--rw-r--r--   0 runner    (1001) docker     (127)      382 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/ssh/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2971 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/ssh/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2603 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/ssh/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    18031 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/ssh/secret_backend_ca.py
--rw-r--r--   0 runner    (1001) docker     (127)    72441 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/ssh/secret_backend_role.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:47:16.785774 pulumi_vault-6.2.0a1713339773/pulumi_vault/terraformcloud/
--rw-r--r--   0 runner    (1001) docker     (127)      354 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/terraformcloud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    26449 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/terraformcloud/secret_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)    18612 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/terraformcloud/secret_creds.py
--rw-r--r--   0 runner    (1001) docker     (127)    22952 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/terraformcloud/secret_role.py
--rw-r--r--   0 runner    (1001) docker     (127)    43519 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/token.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:47:16.785774 pulumi_vault-6.2.0a1713339773/pulumi_vault/tokenauth/
--rw-r--r--   0 runner    (1001) docker     (127)      302 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/tokenauth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    61380 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/tokenauth/auth_backend_role.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:47:16.785774 pulumi_vault-6.2.0a1713339773/pulumi_vault/transform/
--rw-r--r--   0 runner    (1001) docker     (127)      419 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/transform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13773 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/transform/alphabet.py
--rw-r--r--   0 runner    (1001) docker     (127)    11281 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/transform/get_decode.py
--rw-r--r--   0 runner    (1001) docker     (127)    11347 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/transform/get_encode.py
--rw-r--r--   0 runner    (1001) docker     (127)    14508 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/transform/role.py
--rw-r--r--   0 runner    (1001) docker     (127)    25649 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/transform/template.py
--rw-r--r--   0 runner    (1001) docker     (127)    26624 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/transform/transformation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:47:16.789774 pulumi_vault-6.2.0a1713339773/pulumi_vault/transit/
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/transit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6474 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/transit/get_decrypt.py
--rw-r--r--   0 runner    (1001) docker     (127)     6790 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/transit/get_encrypt.py
--rw-r--r--   0 runner    (1001) docker     (127)    53364 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/transit/secret_backend_key.py
--rw-r--r--   0 runner    (1001) docker     (127)    12639 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault/transit/secret_cache_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:47:16.789774 pulumi_vault-6.2.0a1713339773/pulumi_vault.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4857 2024-04-17 07:47:16.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9466 2024-04-17 07:47:16.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 07:47:16.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-17 07:47:16.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-17 07:47:16.000000 pulumi_vault-6.2.0a1713339773/pulumi_vault.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      684 2024-04-17 07:47:10.000000 pulumi_vault-6.2.0a1713339773/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 07:47:16.789774 pulumi_vault-6.2.0a1713339773/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:28:20.666124 pulumi_vault-6.2.0a1713561465/
+-rw-r--r--   0 runner    (1001) docker     (127)     4857 2024-04-19 21:28:20.666124 pulumi_vault-6.2.0a1713561465/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4399 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:28:20.626124 pulumi_vault-6.2.0a1713561465/pulumi_vault/
+-rw-r--r--   0 runner    (1001) docker     (127)    31033 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    73552 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:28:20.626124 pulumi_vault-6.2.0a1713561465/pulumi_vault/ad/
+-rw-r--r--   0 runner    (1001) docker     (127)      394 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/ad/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6522 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/ad/get_access_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)    92297 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/ad/secret_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23882 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/ad/secret_library.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20632 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/ad/secret_role.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:28:20.626124 pulumi_vault-6.2.0a1713561465/pulumi_vault/alicloud/
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/alicloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45824 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/alicloud/auth_backend_role.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:28:20.626124 pulumi_vault-6.2.0a1713561465/pulumi_vault/approle/
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/approle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23505 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/approle/auth_backend_login.py
+-rw-r--r--   0 runner    (1001) docker     (127)    56646 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/approle/auth_backend_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31940 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/approle/auth_backend_role_secret_id.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5916 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/approle/get_auth_backend_role_id.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20655 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/audit.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10469 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/audit_request_header.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21605 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/auth_backend.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:28:20.630124 pulumi_vault-6.2.0a1713561465/pulumi_vault/aws/
+-rw-r--r--   0 runner    (1001) docker     (127)      805 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/aws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18369 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/aws/auth_backend_cert.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32794 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/aws/auth_backend_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23288 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/aws/auth_backend_config_identity.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17096 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/aws/auth_backend_identity_whitelist.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43043 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/aws/auth_backend_login.py
+-rw-r--r--   0 runner    (1001) docker     (127)   110667 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/aws/auth_backend_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26592 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/aws/auth_backend_role_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16666 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/aws/auth_backend_roletag_blacklist.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15623 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/aws/auth_backend_sts_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12282 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/aws/get_access_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4742 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/aws/get_static_access_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49429 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/aws/secret_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48314 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/aws/secret_backend_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17977 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/aws/secret_backend_static_role.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:28:20.630124 pulumi_vault-6.2.0a1713561465/pulumi_vault/azure/
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/azure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2564 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/azure/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23654 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/azure/auth_backend_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    64878 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/azure/auth_backend_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29406 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/azure/backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39172 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/azure/backend_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17943 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/azure/get_access_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3097 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/azure/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    83387 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/cert_auth_backend_role.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:28:20.634124 pulumi_vault-6.2.0a1713561465/pulumi_vault/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3140 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/config/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1361 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/config/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42626 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/config/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22482 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/config/ui_custom_message.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6525 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/config/vars.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:28:20.634124 pulumi_vault-6.2.0a1713561465/pulumi_vault/consul/
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/consul/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39828 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/consul/secret_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41675 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/consul/secret_backend_role.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:28:20.634124 pulumi_vault-6.2.0a1713561465/pulumi_vault/database/
+-rw-r--r--   0 runner    (1001) docker     (127)      461 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   298321 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/database/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)   261078 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/database/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    73337 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/database/secret_backend_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37018 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/database/secret_backend_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30937 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/database/secret_backend_static_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)    98230 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/database/secrets_mount.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16755 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/egp_policy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:28:20.638124 pulumi_vault-6.2.0a1713561465/pulumi_vault/gcp/
+-rw-r--r--   0 runner    (1001) docker     (127)      552 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/gcp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14698 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/gcp/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37432 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/gcp/auth_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)    73886 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/gcp/auth_backend_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22936 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/gcp/get_auth_backend_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12613 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/gcp/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24952 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/gcp/secret_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18979 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/gcp/secret_impersonated_account.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26123 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/gcp/secret_roleset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27427 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/gcp/secret_static_account.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:28:20.638124 pulumi_vault-6.2.0a1713561465/pulumi_vault/generic/
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/generic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39225 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/generic/endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11524 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/generic/get_secret.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22847 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/generic/secret.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7897 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/get_auth_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5587 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/get_auth_backends.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7495 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/get_namespace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4680 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/get_namespaces.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7389 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/get_nomad_access_token.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5138 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/get_policy_document.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10007 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/get_raft_autopilot_state.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:28:20.638124 pulumi_vault-6.2.0a1713561465/pulumi_vault/github/
+-rw-r--r--   0 runner    (1001) docker     (127)      382 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/github/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8032 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/github/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    56571 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/github/auth_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7320 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/github/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15484 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/github/team.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15282 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/github/user.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:28:20.642124 pulumi_vault-6.2.0a1713561465/pulumi_vault/identity/
+-rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/identity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19988 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/identity/entity.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18695 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/identity/entity_alias.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20239 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/identity/entity_policies.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14491 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/identity/get_entity.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18096 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/identity/get_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6067 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/identity/get_oidc_client_creds.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13622 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/identity/get_oidc_openid_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6100 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/identity/get_oidc_public_keys.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37922 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/identity/group.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17454 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/identity/group_alias.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20794 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/identity/group_member_entity_ids.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20480 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/identity/group_member_group_ids.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20547 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/identity/group_policies.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25146 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/identity/mfa_duo.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23783 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/identity/mfa_login_enforcement.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23189 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/identity/mfa_okta.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23924 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/identity/mfa_pingid.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29583 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/identity/mfa_totp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12422 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/identity/oidc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15455 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/identity/oidc_assignment.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29889 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/identity/oidc_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21166 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/identity/oidc_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12922 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/identity/oidc_key_allowed_client_id.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24498 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/identity/oidc_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22232 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/identity/oidc_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14755 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/identity/oidc_scope.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4154 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/identity/outputs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:28:20.646124 pulumi_vault-6.2.0a1713561465/pulumi_vault/jwt/
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/jwt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8032 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/jwt/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    66520 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/jwt/auth_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)    97651 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/jwt/auth_backend_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7320 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/jwt/outputs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:28:20.646124 pulumi_vault-6.2.0a1713561465/pulumi_vault/kmip/
+-rw-r--r--   0 runner    (1001) docker     (127)      354 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/kmip/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37931 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/kmip/secret_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)    54561 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/kmip/secret_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14926 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/kmip/secret_scope.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:28:20.646124 pulumi_vault-6.2.0a1713561465/pulumi_vault/kubernetes/
+-rw-r--r--   0 runner    (1001) docker     (127)      519 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/kubernetes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31330 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/kubernetes/auth_backend_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    57046 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/kubernetes/auth_backend_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10609 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/kubernetes/get_auth_backend_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21357 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/kubernetes/get_auth_backend_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13945 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/kubernetes/get_service_account_token.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50872 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/kubernetes/secret_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)    56177 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/kubernetes/secret_backend_role.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:28:20.650124 pulumi_vault-6.2.0a1713561465/pulumi_vault/kv/
+-rw-r--r--   0 runner    (1001) docker     (127)      553 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/kv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3628 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/kv/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7962 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/kv/get_secret.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9604 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/kv/get_secret_subkeys_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10693 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/kv/get_secret_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5997 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/kv/get_secrets_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8127 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/kv/get_secrets_list_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3639 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/kv/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16069 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/kv/secret.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19135 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/kv/secret_backend_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35987 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/kv/secret_v2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:28:20.650124 pulumi_vault-6.2.0a1713561465/pulumi_vault/ldap/
+-rw-r--r--   0 runner    (1001) docker     (127)      598 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/ldap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    92297 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/ldap/auth_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16577 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/ldap/auth_backend_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18645 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/ldap/auth_backend_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6535 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/ldap/get_dynamic_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6722 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/ldap/get_static_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)    77631 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/ldap/secret_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37953 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/ldap/secret_backend_dynamic_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24084 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/ldap/secret_backend_library_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24131 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/ldap/secret_backend_static_role.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:28:20.650124 pulumi_vault-6.2.0a1713561465/pulumi_vault/managed/
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/managed/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29364 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/managed/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14395 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/managed/keys.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25252 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/managed/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28393 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/mfa_duo.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29659 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/mfa_okta.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31128 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/mfa_pingid.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25500 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/mfa_totp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:28:20.654124 pulumi_vault-6.2.0a1713561465/pulumi_vault/mongodbatlas/
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/mongodbatlas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16287 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/mongodbatlas/secret_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33771 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/mongodbatlas/secret_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41533 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/mount.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18077 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/namespace.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42174 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/nomad_secret_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20302 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/nomad_secret_role.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:28:20.654124 pulumi_vault-6.2.0a1713561465/pulumi_vault/okta/
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/okta/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3527 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/okta/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38494 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/okta/auth_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15131 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/okta/auth_backend_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17093 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/okta/auth_backend_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3083 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/okta/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13760 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12397 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/password_policy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:28:20.658124 pulumi_vault-6.2.0a1713561465/pulumi_vault/pkisecret/
+-rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/pkisecret/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2090 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/pkisecret/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16085 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/pkisecret/backend_config_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10049 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/pkisecret/get_backend_issuer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6538 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/pkisecret/get_backend_issuers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7070 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/pkisecret/get_backend_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6443 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/pkisecret/get_backend_keys.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1631 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/pkisecret/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49851 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/pkisecret/secret_backend_cert.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19110 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/pkisecret/secret_backend_config_ca.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17134 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/pkisecret/secret_backend_config_issuers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22199 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/pkisecret/secret_backend_config_urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36967 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/pkisecret/secret_backend_crl_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    61945 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/pkisecret/secret_backend_intermediate_cert_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20204 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/pkisecret/secret_backend_intermediate_set_signed.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36781 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/pkisecret/secret_backend_issuer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25523 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/pkisecret/secret_backend_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)   116377 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/pkisecret/secret_backend_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)    68989 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/pkisecret/secret_backend_root_cert.py
+-rw-r--r--   0 runner    (1001) docker     (127)    58576 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/pkisecret/secret_backend_root_sign_intermediate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48732 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/pkisecret/secret_backend_sign.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10935 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42332 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    21176 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/quota_lease_count.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25781 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/quota_rate_limit.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:28:20.658124 pulumi_vault-6.2.0a1713561465/pulumi_vault/rabbitmq/
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/rabbitmq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5281 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/rabbitmq/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3853 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/rabbitmq/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34778 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/rabbitmq/secret_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22014 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/rabbitmq/secret_backend_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30215 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/raft_autopilot.py
+-rw-r--r--   0 runner    (1001) docker     (127)    84333 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/raft_snapshot_agent_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14552 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/rgp_policy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:28:20.658124 pulumi_vault-6.2.0a1713561465/pulumi_vault/saml/
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/saml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33638 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/saml/auth_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)    55549 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/saml/auth_backend_role.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:28:20.662124 pulumi_vault-6.2.0a1713561465/pulumi_vault/secrets/
+-rw-r--r--   0 runner    (1001) docker     (127)      589 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/secrets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3000 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/secrets/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3202 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/secrets/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18067 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/secrets/sync_association.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38721 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/secrets/sync_aws_destination.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32430 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/secrets/sync_azure_destination.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12448 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/secrets/sync_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26389 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/secrets/sync_gcp_destination.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32333 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/secrets/sync_gh_destination.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15360 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/secrets/sync_github_apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26804 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/secrets/sync_vercel_destination.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:28:20.662124 pulumi_vault-6.2.0a1713561465/pulumi_vault/ssh/
+-rw-r--r--   0 runner    (1001) docker     (127)      382 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/ssh/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2659 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/ssh/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2291 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/ssh/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18031 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/ssh/secret_backend_ca.py
+-rw-r--r--   0 runner    (1001) docker     (127)    72555 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/ssh/secret_backend_role.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:28:20.662124 pulumi_vault-6.2.0a1713561465/pulumi_vault/terraformcloud/
+-rw-r--r--   0 runner    (1001) docker     (127)      354 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/terraformcloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26449 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/terraformcloud/secret_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18672 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/terraformcloud/secret_creds.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23012 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/terraformcloud/secret_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43519 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/token.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:28:20.662124 pulumi_vault-6.2.0a1713561465/pulumi_vault/tokenauth/
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/tokenauth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    61380 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/tokenauth/auth_backend_role.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:28:20.662124 pulumi_vault-6.2.0a1713561465/pulumi_vault/transform/
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/transform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13833 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/transform/alphabet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11379 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/transform/get_decode.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11445 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/transform/get_encode.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14568 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/transform/role.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25755 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/transform/template.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26624 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/transform/transformation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:28:20.666124 pulumi_vault-6.2.0a1713561465/pulumi_vault/transit/
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/transit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6474 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/transit/get_decrypt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6790 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/transit/get_encrypt.py
+-rw-r--r--   0 runner    (1001) docker     (127)    53442 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/transit/secret_backend_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12639 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault/transit/secret_cache_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:28:20.666124 pulumi_vault-6.2.0a1713561465/pulumi_vault.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4857 2024-04-19 21:28:20.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9466 2024-04-19 21:28:20.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 21:28:20.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-19 21:28:20.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-19 21:28:20.000000 pulumi_vault-6.2.0a1713561465/pulumi_vault.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      684 2024-04-19 21:28:13.000000 pulumi_vault-6.2.0a1713561465/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 21:28:20.666124 pulumi_vault-6.2.0a1713561465/setup.cfg
```

### Comparing `pulumi_vault-6.2.0a1713339773/PKG-INFO` & `pulumi_vault-6.2.0a1713561465/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_vault
-Version: 6.2.0a1713339773
+Version: 6.2.0a1713561465
 Summary: A Pulumi package for creating and managing HashiCorp Vault cloud resources.
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.io
 Project-URL: Repository, https://github.com/pulumi/pulumi-vault
 Keywords: pulumi,vault
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_vault-6.2.0a1713339773/README.md` & `pulumi_vault-6.2.0a1713561465/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1713339773/pulumi_vault/__init__.py` & `pulumi_vault-6.2.0a1713561465/pulumi_vault/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1713339773/pulumi_vault/_inputs.py` & `pulumi_vault-6.2.0a1713561465/pulumi_vault/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1713339773/pulumi_vault/_utilities.py` & `pulumi_vault-6.2.0a1713561465/pulumi_vault/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1713339773/pulumi_vault/ad/get_access_credentials.py` & `pulumi_vault-6.2.0a1713561465/pulumi_vault/ad/get_access_credentials.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1713339773/pulumi_vault/ad/secret_backend.py` & `pulumi_vault-6.2.0a1713561465/pulumi_vault/ad/secret_backend.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1257,16 +1257,16 @@
         import pulumi
         import pulumi_vault as vault
 
         config = vault.ad.SecretBackend("config",
             backend="ad",
             binddn="CN=Administrator,CN=Users,DC=corp,DC=example,DC=net",
             bindpass="SuperSecretPassw0rd",
-            insecure_tls=True,
             url="ldaps://ad",
+            insecure_tls=True,
             userdn="CN=Users,DC=corp,DC=example,DC=net")
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
 
         AD secret backend can be imported using the `backend`, e.g.
@@ -1350,16 +1350,16 @@
         import pulumi
         import pulumi_vault as vault
 
         config = vault.ad.SecretBackend("config",
             backend="ad",
             binddn="CN=Administrator,CN=Users,DC=corp,DC=example,DC=net",
             bindpass="SuperSecretPassw0rd",
-            insecure_tls=True,
             url="ldaps://ad",
+            insecure_tls=True,
             userdn="CN=Users,DC=corp,DC=example,DC=net")
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
 
         AD secret backend can be imported using the `backend`, e.g.
```

### Comparing `pulumi_vault-6.2.0a1713339773/pulumi_vault/ad/secret_library.py` & `pulumi_vault-6.2.0a1713561465/pulumi_vault/ad/secret_library.py`

 * *Files 1% similar despite different names*

```diff
@@ -303,14 +303,15 @@
             binddn="CN=Administrator,CN=Users,DC=corp,DC=example,DC=net",
             bindpass="SuperSecretPassw0rd",
             url="ldaps://ad",
             insecure_tls=True,
             userdn="CN=Users,DC=corp,DC=example,DC=net")
         qa = vault.ad.SecretLibrary("qa",
             backend=config.backend,
+            name="qa",
             service_account_names=[
                 "Bob",
                 "Mary",
             ],
             ttl=60,
             disable_check_in_enforcement=True,
             max_ttl=120)
@@ -361,14 +362,15 @@
             binddn="CN=Administrator,CN=Users,DC=corp,DC=example,DC=net",
             bindpass="SuperSecretPassw0rd",
             url="ldaps://ad",
             insecure_tls=True,
             userdn="CN=Users,DC=corp,DC=example,DC=net")
         qa = vault.ad.SecretLibrary("qa",
             backend=config.backend,
+            name="qa",
             service_account_names=[
                 "Bob",
                 "Mary",
             ],
             ttl=60,
             disable_check_in_enforcement=True,
             max_ttl=120)
```

### Comparing `pulumi_vault-6.2.0a1713339773/pulumi_vault/ad/secret_role.py` & `pulumi_vault-6.2.0a1713561465/pulumi_vault/ad/secret_role.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1713339773/pulumi_vault/alicloud/auth_backend_role.py` & `pulumi_vault-6.2.0a1713561465/pulumi_vault/alicloud/auth_backend_role.py`

 * *Files 1% similar despite different names*

```diff
@@ -562,19 +562,19 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_vault as vault
 
-        alicloud_auth_backend = vault.AuthBackend("alicloudAuthBackend",
+        alicloud = vault.AuthBackend("alicloud",
             type="alicloud",
             path="alicloud")
-        alicloud_auth_backend_role = vault.alicloud.AuthBackendRole("alicloudAuthBackendRole",
-            backend=alicloud_auth_backend.path,
+        alicloud_auth_backend_role = vault.alicloud.AuthBackendRole("alicloud",
+            backend=alicloud.path,
             role="example",
             arn="acs:ram:123456:tf:role/foobar")
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
 
@@ -636,19 +636,19 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_vault as vault
 
-        alicloud_auth_backend = vault.AuthBackend("alicloudAuthBackend",
+        alicloud = vault.AuthBackend("alicloud",
             type="alicloud",
             path="alicloud")
-        alicloud_auth_backend_role = vault.alicloud.AuthBackendRole("alicloudAuthBackendRole",
-            backend=alicloud_auth_backend.path,
+        alicloud_auth_backend_role = vault.alicloud.AuthBackendRole("alicloud",
+            backend=alicloud.path,
             role="example",
             arn="acs:ram:123456:tf:role/foobar")
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
```

### Comparing `pulumi_vault-6.2.0a1713339773/pulumi_vault/approle/auth_backend_login.py` & `pulumi_vault-6.2.0a1713561465/pulumi_vault/approle/auth_backend_login.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1713339773/pulumi_vault/approle/auth_backend_role.py` & `pulumi_vault-6.2.0a1713561465/pulumi_vault/approle/auth_backend_role.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1713339773/pulumi_vault/approle/auth_backend_role_secret_id.py` & `pulumi_vault-6.2.0a1713561465/pulumi_vault/approle/auth_backend_role_secret_id.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1713339773/pulumi_vault/approle/get_auth_backend_role_id.py` & `pulumi_vault-6.2.0a1713561465/pulumi_vault/approle/get_auth_backend_role_id.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1713339773/pulumi_vault/audit.py` & `pulumi_vault-6.2.0a1713561465/pulumi_vault/audit.py`

 * *Files 1% similar despite different names*

```diff
@@ -256,37 +256,37 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_vault as vault
 
         test = vault.Audit("test",
+            type="file",
             options={
                 "file_path": "C:/temp/audit.txt",
-            },
-            type="file")
+            })
         ```
         <!--End PulumiCodeChooser -->
 
         ### Socket Audit Device)
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_vault as vault
 
         test = vault.Audit("test",
+            type="socket",
+            path="app_socket",
             local=False,
             options={
                 "address": "127.0.0.1:8000",
-                "description": "application x socket",
                 "socket_type": "tcp",
-            },
-            path="app_socket",
-            type="socket")
+                "description": "application x socket",
+            })
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
 
         Audit devices can be imported using the `path`, e.g.
 
@@ -321,37 +321,37 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_vault as vault
 
         test = vault.Audit("test",
+            type="file",
             options={
                 "file_path": "C:/temp/audit.txt",
-            },
-            type="file")
+            })
         ```
         <!--End PulumiCodeChooser -->
 
         ### Socket Audit Device)
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_vault as vault
 
         test = vault.Audit("test",
+            type="socket",
+            path="app_socket",
             local=False,
             options={
                 "address": "127.0.0.1:8000",
-                "description": "application x socket",
                 "socket_type": "tcp",
-            },
-            path="app_socket",
-            type="socket")
+                "description": "application x socket",
+            })
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
 
         Audit devices can be imported using the `path`, e.g.
```

### Comparing `pulumi_vault-6.2.0a1713339773/pulumi_vault/audit_request_header.py` & `pulumi_vault-6.2.0a1713561465/pulumi_vault/audit_request_header.py`

 * *Files 2% similar despite different names*

```diff
@@ -143,15 +143,17 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_vault as vault
 
-        x_forwarded_for = vault.AuditRequestHeader("xForwardedFor", hmac=False)
+        x_forwarded_for = vault.AuditRequestHeader("x_forwarded_for",
+            name="X-Forwarded-For",
+            hmac=False)
         ```
         <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[bool] hmac: Whether this header's value should be HMAC'd in the audit logs.
         :param pulumi.Input[str] name: The name of the request header to audit.
@@ -174,15 +176,17 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_vault as vault
 
-        x_forwarded_for = vault.AuditRequestHeader("xForwardedFor", hmac=False)
+        x_forwarded_for = vault.AuditRequestHeader("x_forwarded_for",
+            name="X-Forwarded-For",
+            hmac=False)
         ```
         <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param AuditRequestHeaderArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
```

### Comparing `pulumi_vault-6.2.0a1713339773/pulumi_vault/auth_backend.py` & `pulumi_vault-6.2.0a1713561465/pulumi_vault/auth_backend.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1713339773/pulumi_vault/aws/__init__.py` & `pulumi_vault-6.2.0a1713561465/pulumi_vault/aws/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1713339773/pulumi_vault/aws/auth_backend_cert.py` & `pulumi_vault-6.2.0a1713561465/pulumi_vault/aws/auth_backend_cert.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1713339773/pulumi_vault/aws/auth_backend_client.py` & `pulumi_vault-6.2.0a1713561465/pulumi_vault/aws/auth_backend_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -431,17 +431,17 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_vault as vault
 
-        example_auth_backend = vault.AuthBackend("exampleAuthBackend", type="aws")
-        example_auth_backend_client = vault.aws.AuthBackendClient("exampleAuthBackendClient",
-            backend=example_auth_backend.path,
+        example = vault.AuthBackend("example", type="aws")
+        example_auth_backend_client = vault.aws.AuthBackendClient("example",
+            backend=example.path,
             access_key="INSERT_AWS_ACCESS_KEY",
             secret_key="INSERT_AWS_SECRET_KEY")
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
 
@@ -490,17 +490,17 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_vault as vault
 
-        example_auth_backend = vault.AuthBackend("exampleAuthBackend", type="aws")
-        example_auth_backend_client = vault.aws.AuthBackendClient("exampleAuthBackendClient",
-            backend=example_auth_backend.path,
+        example = vault.AuthBackend("example", type="aws")
+        example_auth_backend_client = vault.aws.AuthBackendClient("example",
+            backend=example.path,
             access_key="INSERT_AWS_ACCESS_KEY",
             secret_key="INSERT_AWS_SECRET_KEY")
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
```

### Comparing `pulumi_vault-6.2.0a1713339773/pulumi_vault/aws/auth_backend_config_identity.py` & `pulumi_vault-6.2.0a1713561465/pulumi_vault/aws/auth_backend_config_identity.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1713339773/pulumi_vault/aws/auth_backend_identity_whitelist.py` & `pulumi_vault-6.2.0a1713561465/pulumi_vault/aws/auth_backend_identity_whitelist.py`

 * *Files 4% similar despite different names*

```diff
@@ -198,17 +198,17 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_vault as vault
 
-        example_auth_backend = vault.AuthBackend("exampleAuthBackend", type="aws")
-        example_auth_backend_identity_whitelist = vault.aws.AuthBackendIdentityWhitelist("exampleAuthBackendIdentityWhitelist",
-            backend=example_auth_backend.path,
+        example = vault.AuthBackend("example", type="aws")
+        example_auth_backend_identity_whitelist = vault.aws.AuthBackendIdentityWhitelist("example",
+            backend=example.path,
             safety_buffer=3600)
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
 
         AWS auth backend identity whitelists can be imported using `auth/`, the `backend` path, and `/config/tidy/identity-whitelist` e.g.
@@ -245,17 +245,17 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_vault as vault
 
-        example_auth_backend = vault.AuthBackend("exampleAuthBackend", type="aws")
-        example_auth_backend_identity_whitelist = vault.aws.AuthBackendIdentityWhitelist("exampleAuthBackendIdentityWhitelist",
-            backend=example_auth_backend.path,
+        example = vault.AuthBackend("example", type="aws")
+        example_auth_backend_identity_whitelist = vault.aws.AuthBackendIdentityWhitelist("example",
+            backend=example.path,
             safety_buffer=3600)
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
 
         AWS auth backend identity whitelists can be imported using `auth/`, the `backend` path, and `/config/tidy/identity-whitelist` e.g.
```

### Comparing `pulumi_vault-6.2.0a1713339773/pulumi_vault/aws/auth_backend_login.py` & `pulumi_vault-6.2.0a1713561465/pulumi_vault/aws/auth_backend_login.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1713339773/pulumi_vault/aws/auth_backend_role.py` & `pulumi_vault-6.2.0a1713561465/pulumi_vault/aws/auth_backend_role.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1713339773/pulumi_vault/aws/auth_backend_role_tag.py` & `pulumi_vault-6.2.0a1713561465/pulumi_vault/aws/auth_backend_role_tag.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1713339773/pulumi_vault/aws/auth_backend_roletag_blacklist.py` & `pulumi_vault-6.2.0a1713561465/pulumi_vault/aws/auth_backend_roletag_blacklist.py`

 * *Files 2% similar despite different names*

```diff
@@ -198,17 +198,17 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_vault as vault
 
-        example_auth_backend = vault.AuthBackend("exampleAuthBackend", type="aws")
-        example_auth_backend_roletag_blacklist = vault.aws.AuthBackendRoletagBlacklist("exampleAuthBackendRoletagBlacklist",
-            backend=example_auth_backend.path,
+        example = vault.AuthBackend("example", type="aws")
+        example_auth_backend_roletag_blacklist = vault.aws.AuthBackendRoletagBlacklist("example",
+            backend=example.path,
             safety_buffer=360)
         ```
         <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] backend: The path the AWS auth backend being configured was
@@ -235,17 +235,17 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_vault as vault
 
-        example_auth_backend = vault.AuthBackend("exampleAuthBackend", type="aws")
-        example_auth_backend_roletag_blacklist = vault.aws.AuthBackendRoletagBlacklist("exampleAuthBackendRoletagBlacklist",
-            backend=example_auth_backend.path,
+        example = vault.AuthBackend("example", type="aws")
+        example_auth_backend_roletag_blacklist = vault.aws.AuthBackendRoletagBlacklist("example",
+            backend=example.path,
             safety_buffer=360)
         ```
         <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param AuthBackendRoletagBlacklistArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
```

### Comparing `pulumi_vault-6.2.0a1713339773/pulumi_vault/aws/auth_backend_sts_role.py` & `pulumi_vault-6.2.0a1713561465/pulumi_vault/aws/auth_backend_sts_role.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1713339773/pulumi_vault/aws/get_access_credentials.py` & `pulumi_vault-6.2.0a1713561465/pulumi_vault/aws/get_access_credentials.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1713339773/pulumi_vault/aws/get_static_access_credentials.py` & `pulumi_vault-6.2.0a1713561465/pulumi_vault/aws/get_static_access_credentials.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1713339773/pulumi_vault/aws/secret_backend.py` & `pulumi_vault-6.2.0a1713561465/pulumi_vault/aws/secret_backend.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1713339773/pulumi_vault/aws/secret_backend_role.py` & `pulumi_vault-6.2.0a1713561465/pulumi_vault/aws/secret_backend_role.py`

 * *Files 0% similar despite different names*

```diff
@@ -572,14 +572,15 @@
         import pulumi_vault as vault
 
         aws = vault.aws.SecretBackend("aws",
             access_key="AKIA.....",
             secret_key="AWS secret key")
         role = vault.aws.SecretBackendRole("role",
             backend=aws.path,
+            name="deploy",
             credential_type="iam_user",
             policy_document=\"\"\"{
           "Version": "2012-10-17",
           "Statement": [
             {
               "Effect": "Allow",
               "Action": "iam:*",
@@ -663,14 +664,15 @@
         import pulumi_vault as vault
 
         aws = vault.aws.SecretBackend("aws",
             access_key="AKIA.....",
             secret_key="AWS secret key")
         role = vault.aws.SecretBackendRole("role",
             backend=aws.path,
+            name="deploy",
             credential_type="iam_user",
             policy_document=\"\"\"{
           "Version": "2012-10-17",
           "Statement": [
             {
               "Effect": "Allow",
               "Action": "iam:*",
```

### Comparing `pulumi_vault-6.2.0a1713339773/pulumi_vault/aws/secret_backend_static_role.py` & `pulumi_vault-6.2.0a1713561465/pulumi_vault/aws/secret_backend_static_role.py`

 * *Files 1% similar despite different names*

```diff
@@ -225,14 +225,15 @@
         import pulumi_vault as vault
 
         aws = vault.aws.SecretBackend("aws",
             path="my-aws",
             description="Obtain AWS credentials.")
         role = vault.aws.SecretBackendStaticRole("role",
             backend=aws.path,
+            name="test",
             username="my-test-user",
             rotation_period=3600)
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
 
@@ -271,14 +272,15 @@
         import pulumi_vault as vault
 
         aws = vault.aws.SecretBackend("aws",
             path="my-aws",
             description="Obtain AWS credentials.")
         role = vault.aws.SecretBackendStaticRole("role",
             backend=aws.path,
+            name="test",
             username="my-test-user",
             rotation_period=3600)
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
```

### Comparing `pulumi_vault-6.2.0a1713339773/pulumi_vault/azure/_inputs.py` & `pulumi_vault-6.2.0a1713561465/pulumi_vault/azure/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1713339773/pulumi_vault/azure/auth_backend_config.py` & `pulumi_vault-6.2.0a1713561465/pulumi_vault/azure/auth_backend_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -306,17 +306,17 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_vault as vault
 
-        example_auth_backend = vault.AuthBackend("exampleAuthBackend", type="azure")
-        example_auth_backend_config = vault.azure.AuthBackendConfig("exampleAuthBackendConfig",
-            backend=example_auth_backend.path,
+        example = vault.AuthBackend("example", type="azure")
+        example_auth_backend_config = vault.azure.AuthBackendConfig("example",
+            backend=example.path,
             tenant_id="11111111-2222-3333-4444-555555555555",
             client_id="11111111-2222-3333-4444-555555555555",
             client_secret="01234567890123456789",
             resource="https://vault.hashicorp.com")
         ```
         <!--End PulumiCodeChooser -->
 
@@ -358,17 +358,17 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_vault as vault
 
-        example_auth_backend = vault.AuthBackend("exampleAuthBackend", type="azure")
-        example_auth_backend_config = vault.azure.AuthBackendConfig("exampleAuthBackendConfig",
-            backend=example_auth_backend.path,
+        example = vault.AuthBackend("example", type="azure")
+        example_auth_backend_config = vault.azure.AuthBackendConfig("example",
+            backend=example.path,
             tenant_id="11111111-2222-3333-4444-555555555555",
             client_id="11111111-2222-3333-4444-555555555555",
             client_secret="01234567890123456789",
             resource="https://vault.hashicorp.com")
         ```
         <!--End PulumiCodeChooser -->
```

### Comparing `pulumi_vault-6.2.0a1713339773/pulumi_vault/azure/auth_backend_role.py` & `pulumi_vault-6.2.0a1713561465/pulumi_vault/azure/auth_backend_role.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1713339773/pulumi_vault/azure/backend.py` & `pulumi_vault-6.2.0a1713561465/pulumi_vault/azure/backend.py`

 * *Files 0% similar despite different names*

```diff
@@ -384,37 +384,37 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_vault as vault
 
         azure = vault.azure.Backend("azure",
-            client_id="11111111-2222-3333-4444-333333333333",
-            client_secret="12345678901234567890",
-            environment="AzurePublicCloud",
+            use_microsoft_graph_api=True,
             subscription_id="11111111-2222-3333-4444-111111111111",
             tenant_id="11111111-2222-3333-4444-222222222222",
-            use_microsoft_graph_api=True)
+            client_id="11111111-2222-3333-4444-333333333333",
+            client_secret="12345678901234567890",
+            environment="AzurePublicCloud")
         ```
         <!--End PulumiCodeChooser -->
 
         ### *Vault-1.8 And Below*
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_vault as vault
 
         azure = vault.azure.Backend("azure",
-            client_id="11111111-2222-3333-4444-333333333333",
-            client_secret="12345678901234567890",
-            environment="AzurePublicCloud",
+            use_microsoft_graph_api=False,
             subscription_id="11111111-2222-3333-4444-111111111111",
             tenant_id="11111111-2222-3333-4444-222222222222",
-            use_microsoft_graph_api=False)
+            client_id="11111111-2222-3333-4444-333333333333",
+            client_secret="12345678901234567890",
+            environment="AzurePublicCloud")
         ```
         <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] client_id: The OAuth2 client id to connect to Azure.
         :param pulumi.Input[str] client_secret: The OAuth2 client secret to connect to Azure.
@@ -444,37 +444,37 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_vault as vault
 
         azure = vault.azure.Backend("azure",
-            client_id="11111111-2222-3333-4444-333333333333",
-            client_secret="12345678901234567890",
-            environment="AzurePublicCloud",
+            use_microsoft_graph_api=True,
             subscription_id="11111111-2222-3333-4444-111111111111",
             tenant_id="11111111-2222-3333-4444-222222222222",
-            use_microsoft_graph_api=True)
+            client_id="11111111-2222-3333-4444-333333333333",
+            client_secret="12345678901234567890",
+            environment="AzurePublicCloud")
         ```
         <!--End PulumiCodeChooser -->
 
         ### *Vault-1.8 And Below*
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_vault as vault
 
         azure = vault.azure.Backend("azure",
-            client_id="11111111-2222-3333-4444-333333333333",
-            client_secret="12345678901234567890",
-            environment="AzurePublicCloud",
+            use_microsoft_graph_api=False,
             subscription_id="11111111-2222-3333-4444-111111111111",
             tenant_id="11111111-2222-3333-4444-222222222222",
-            use_microsoft_graph_api=False)
+            client_id="11111111-2222-3333-4444-333333333333",
+            client_secret="12345678901234567890",
+            environment="AzurePublicCloud")
         ```
         <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param BackendArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
```

### Comparing `pulumi_vault-6.2.0a1713339773/pulumi_vault/azure/backend_role.py` & `pulumi_vault-6.2.0a1713561465/pulumi_vault/azure/backend_role.py`

 * *Files 0% similar despite different names*

```diff
@@ -467,33 +467,33 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_vault as vault
 
         azure = vault.azure.Backend("azure",
-            subscription_id=var["subscription_id"],
-            tenant_id=var["tenant_id"],
-            client_secret=var["client_secret"],
-            client_id=var["client_id"])
-        generated_role = vault.azure.BackendRole("generatedRole",
+            subscription_id=subscription_id,
+            tenant_id=tenant_id,
+            client_secret=client_secret,
+            client_id=client_id)
+        generated_role = vault.azure.BackendRole("generated_role",
             backend=azure.path,
             role="generated_role",
             sign_in_audience="AzureADMyOrg",
             tags=[
                 "team:engineering",
                 "environment:development",
             ],
             ttl="300",
             max_ttl="600",
             azure_roles=[vault.azure.BackendRoleAzureRoleArgs(
                 role_name="Reader",
-                scope=f"/subscriptions/{var['subscription_id']}/resourceGroups/azure-vault-group",
+                scope=f"/subscriptions/{subscription_id}/resourceGroups/azure-vault-group",
             )])
-        existing_object_id = vault.azure.BackendRole("existingObjectId",
+        existing_object_id = vault.azure.BackendRole("existing_object_id",
             backend=azure.path,
             role="existing_object_id",
             application_object_id="11111111-2222-3333-4444-44444444444",
             ttl="300",
             max_ttl="600")
         ```
         <!--End PulumiCodeChooser -->
@@ -532,33 +532,33 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_vault as vault
 
         azure = vault.azure.Backend("azure",
-            subscription_id=var["subscription_id"],
-            tenant_id=var["tenant_id"],
-            client_secret=var["client_secret"],
-            client_id=var["client_id"])
-        generated_role = vault.azure.BackendRole("generatedRole",
+            subscription_id=subscription_id,
+            tenant_id=tenant_id,
+            client_secret=client_secret,
+            client_id=client_id)
+        generated_role = vault.azure.BackendRole("generated_role",
             backend=azure.path,
             role="generated_role",
             sign_in_audience="AzureADMyOrg",
             tags=[
                 "team:engineering",
                 "environment:development",
             ],
             ttl="300",
             max_ttl="600",
             azure_roles=[vault.azure.BackendRoleAzureRoleArgs(
                 role_name="Reader",
-                scope=f"/subscriptions/{var['subscription_id']}/resourceGroups/azure-vault-group",
+                scope=f"/subscriptions/{subscription_id}/resourceGroups/azure-vault-group",
             )])
-        existing_object_id = vault.azure.BackendRole("existingObjectId",
+        existing_object_id = vault.azure.BackendRole("existing_object_id",
             backend=azure.path,
             role="existing_object_id",
             application_object_id="11111111-2222-3333-4444-44444444444",
             ttl="300",
             max_ttl="600")
         ```
         <!--End PulumiCodeChooser -->
```

### Comparing `pulumi_vault-6.2.0a1713339773/pulumi_vault/azure/get_access_credentials.py` & `pulumi_vault-6.2.0a1713561465/pulumi_vault/azure/get_access_credentials.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1713339773/pulumi_vault/azure/outputs.py` & `pulumi_vault-6.2.0a1713561465/pulumi_vault/azure/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1713339773/pulumi_vault/cert_auth_backend_role.py` & `pulumi_vault-6.2.0a1713561465/pulumi_vault/cert_auth_backend_role.py`

 * *Files 1% similar despite different names*

```diff
@@ -1034,22 +1034,24 @@
         Provides a resource to create a role in an [Cert auth backend within Vault](https://www.vaultproject.io/docs/auth/cert.html).
 
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
+        import pulumi_std as std
         import pulumi_vault as vault
 
-        cert_auth_backend = vault.AuthBackend("certAuthBackend",
+        cert = vault.AuthBackend("cert",
             path="cert",
             type="cert")
-        cert_cert_auth_backend_role = vault.CertAuthBackendRole("certCertAuthBackendRole",
-            certificate=(lambda path: open(path).read())("/path/to/certs/ca-cert.pem"),
-            backend=cert_auth_backend.path,
+        cert_cert_auth_backend_role = vault.CertAuthBackendRole("cert",
+            name="foo",
+            certificate=std.file(input="/path/to/certs/ca-cert.pem").result,
+            backend=cert.path,
             allowed_names=[
                 "foo.example.org",
                 "baz.example.org",
             ],
             token_ttl=300,
             token_max_ttl=600,
             token_policies=["foo"])
@@ -1130,22 +1132,24 @@
         Provides a resource to create a role in an [Cert auth backend within Vault](https://www.vaultproject.io/docs/auth/cert.html).
 
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
+        import pulumi_std as std
         import pulumi_vault as vault
 
-        cert_auth_backend = vault.AuthBackend("certAuthBackend",
+        cert = vault.AuthBackend("cert",
             path="cert",
             type="cert")
-        cert_cert_auth_backend_role = vault.CertAuthBackendRole("certCertAuthBackendRole",
-            certificate=(lambda path: open(path).read())("/path/to/certs/ca-cert.pem"),
-            backend=cert_auth_backend.path,
+        cert_cert_auth_backend_role = vault.CertAuthBackendRole("cert",
+            name="foo",
+            certificate=std.file(input="/path/to/certs/ca-cert.pem").result,
+            backend=cert.path,
             allowed_names=[
                 "foo.example.org",
                 "baz.example.org",
             ],
             token_ttl=300,
             token_max_ttl=600,
             token_policies=["foo"])
```

### Comparing `pulumi_vault-6.2.0a1713339773/pulumi_vault/config/__init__.pyi` & `pulumi_vault-6.2.0a1713561465/pulumi_vault/config/__init__.pyi`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1713339773/pulumi_vault/config/_inputs.py` & `pulumi_vault-6.2.0a1713561465/pulumi_vault/config/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1713339773/pulumi_vault/config/outputs.py` & `pulumi_vault-6.2.0a1713561465/pulumi_vault/config/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1713339773/pulumi_vault/config/ui_custom_message.py` & `pulumi_vault-6.2.0a1713561465/pulumi_vault/config/ui_custom_message.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1713339773/pulumi_vault/config/vars.py` & `pulumi_vault-6.2.0a1713561465/pulumi_vault/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1713339773/pulumi_vault/consul/secret_backend.py` & `pulumi_vault-6.2.0a1713561465/pulumi_vault/consul/secret_backend.py`

 * *Files 0% similar despite different names*

```diff
@@ -532,32 +532,32 @@
         ### Creating a standard backend resource:
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_vault as vault
 
         test = vault.consul.SecretBackend("test",
-            address="127.0.0.1:8500",
-            description="Manages the Consul backend",
             path="consul",
+            description="Manages the Consul backend",
+            address="127.0.0.1:8500",
             token="4240861b-ce3d-8530-115a-521ff070dd29")
         ```
         <!--End PulumiCodeChooser -->
 
         ### Creating a backend resource to bootstrap a new Consul instance:
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_vault as vault
 
         test = vault.consul.SecretBackend("test",
-            address="127.0.0.1:8500",
-            bootstrap=True,
+            path="consul",
             description="Bootstrap the Consul backend",
-            path="consul")
+            address="127.0.0.1:8500",
+            bootstrap=True)
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
 
         Consul secret backends can be imported using the `path`, e.g.
 
@@ -602,32 +602,32 @@
         ### Creating a standard backend resource:
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_vault as vault
 
         test = vault.consul.SecretBackend("test",
-            address="127.0.0.1:8500",
-            description="Manages the Consul backend",
             path="consul",
+            description="Manages the Consul backend",
+            address="127.0.0.1:8500",
             token="4240861b-ce3d-8530-115a-521ff070dd29")
         ```
         <!--End PulumiCodeChooser -->
 
         ### Creating a backend resource to bootstrap a new Consul instance:
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_vault as vault
 
         test = vault.consul.SecretBackend("test",
-            address="127.0.0.1:8500",
-            bootstrap=True,
+            path="consul",
             description="Bootstrap the Consul backend",
-            path="consul")
+            address="127.0.0.1:8500",
+            bootstrap=True)
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
 
         Consul secret backends can be imported using the `path`, e.g.
```

### Comparing `pulumi_vault-6.2.0a1713339773/pulumi_vault/consul/secret_backend_role.py` & `pulumi_vault-6.2.0a1713561465/pulumi_vault/consul/secret_backend_role.py`

 * *Files 0% similar despite different names*

```diff
@@ -514,14 +514,15 @@
 
         test = vault.consul.SecretBackend("test",
             path="consul",
             description="Manages the Consul backend",
             address="127.0.0.1:8500",
             token="4240861b-ce3d-8530-115a-521ff070dd29")
         example = vault.consul.SecretBackendRole("example",
+            name="test-role",
             backend=test.path,
             consul_policies=["example-policy"])
         ```
         <!--End PulumiCodeChooser -->
 
         ## Note About Required Arguments
 
@@ -581,14 +582,15 @@
 
         test = vault.consul.SecretBackend("test",
             path="consul",
             description="Manages the Consul backend",
             address="127.0.0.1:8500",
             token="4240861b-ce3d-8530-115a-521ff070dd29")
         example = vault.consul.SecretBackendRole("example",
+            name="test-role",
             backend=test.path,
             consul_policies=["example-policy"])
         ```
         <!--End PulumiCodeChooser -->
 
         ## Note About Required Arguments
```

### Comparing `pulumi_vault-6.2.0a1713339773/pulumi_vault/database/_inputs.py` & `pulumi_vault-6.2.0a1713561465/pulumi_vault/database/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1713339773/pulumi_vault/database/outputs.py` & `pulumi_vault-6.2.0a1713561465/pulumi_vault/database/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1713339773/pulumi_vault/database/secret_backend_connection.py` & `pulumi_vault-6.2.0a1713561465/pulumi_vault/database/secret_backend_connection.py`

 * *Files 0% similar despite different names*

```diff
@@ -929,14 +929,15 @@
         import pulumi_vault as vault
 
         db = vault.Mount("db",
             path="postgres",
             type="database")
         postgres = vault.database.SecretBackendConnection("postgres",
             backend=db.path,
+            name="postgres",
             allowed_roles=[
                 "dev",
                 "prod",
             ],
             postgresql=vault.database.SecretBackendConnectionPostgresqlArgs(
                 connection_url="postgres://username:password@host:port/database",
             ))
@@ -1002,14 +1003,15 @@
         import pulumi_vault as vault
 
         db = vault.Mount("db",
             path="postgres",
             type="database")
         postgres = vault.database.SecretBackendConnection("postgres",
             backend=db.path,
+            name="postgres",
             allowed_roles=[
                 "dev",
                 "prod",
             ],
             postgresql=vault.database.SecretBackendConnectionPostgresqlArgs(
                 connection_url="postgres://username:password@host:port/database",
             ))
```

### Comparing `pulumi_vault-6.2.0a1713339773/pulumi_vault/database/secret_backend_role.py` & `pulumi_vault-6.2.0a1713561465/pulumi_vault/database/secret_backend_role.py`

 * *Files 1% similar despite different names*

```diff
@@ -495,23 +495,25 @@
         import pulumi_vault as vault
 
         db = vault.Mount("db",
             path="postgres",
             type="database")
         postgres = vault.database.SecretBackendConnection("postgres",
             backend=db.path,
+            name="postgres",
             allowed_roles=[
                 "dev",
                 "prod",
             ],
             postgresql=vault.database.SecretBackendConnectionPostgresqlArgs(
                 connection_url="postgres://username:password@host:port/database",
             ))
         role = vault.database.SecretBackendRole("role",
             backend=db.path,
+            name="dev",
             db_name=postgres.name,
             creation_statements=["CREATE ROLE \\"{{name}}\\" WITH LOGIN PASSWORD '{{password}}' VALID UNTIL '{{expiration}}';"])
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
 
@@ -566,23 +568,25 @@
         import pulumi_vault as vault
 
         db = vault.Mount("db",
             path="postgres",
             type="database")
         postgres = vault.database.SecretBackendConnection("postgres",
             backend=db.path,
+            name="postgres",
             allowed_roles=[
                 "dev",
                 "prod",
             ],
             postgresql=vault.database.SecretBackendConnectionPostgresqlArgs(
                 connection_url="postgres://username:password@host:port/database",
             ))
         role = vault.database.SecretBackendRole("role",
             backend=db.path,
+            name="dev",
             db_name=postgres.name,
             creation_statements=["CREATE ROLE \\"{{name}}\\" WITH LOGIN PASSWORD '{{password}}' VALID UNTIL '{{expiration}}';"])
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
```

### Comparing `pulumi_vault-6.2.0a1713339773/pulumi_vault/database/secret_backend_static_role.py` & `pulumi_vault-6.2.0a1713561465/pulumi_vault/database/secret_backend_static_role.py`

 * *Files 1% similar despite different names*

```diff
@@ -376,28 +376,31 @@
         import pulumi_vault as vault
 
         db = vault.Mount("db",
             path="postgres",
             type="database")
         postgres = vault.database.SecretBackendConnection("postgres",
             backend=db.path,
+            name="postgres",
             allowed_roles=["*"],
             postgresql=vault.database.SecretBackendConnectionPostgresqlArgs(
                 connection_url="postgres://username:password@host:port/database",
             ))
         # configure a static role with period-based rotations
-        period_role = vault.database.SecretBackendStaticRole("periodRole",
+        period_role = vault.database.SecretBackendStaticRole("period_role",
             backend=db.path,
+            name="my-period-role",
             db_name=postgres.name,
             username="example",
             rotation_period=3600,
             rotation_statements=["ALTER USER \\"{{name}}\\" WITH PASSWORD '{{password}}';"])
         # configure a static role with schedule-based rotations
-        schedule_role = vault.database.SecretBackendStaticRole("scheduleRole",
+        schedule_role = vault.database.SecretBackendStaticRole("schedule_role",
             backend=db.path,
+            name="my-schedule-role",
             db_name=postgres.name,
             username="example",
             rotation_schedule="0 0 * * SAT",
             rotation_window=172800,
             rotation_statements=["ALTER USER \\"{{name}}\\" WITH PASSWORD '{{password}}';"])
         ```
         <!--End PulumiCodeChooser -->
@@ -450,28 +453,31 @@
         import pulumi_vault as vault
 
         db = vault.Mount("db",
             path="postgres",
             type="database")
         postgres = vault.database.SecretBackendConnection("postgres",
             backend=db.path,
+            name="postgres",
             allowed_roles=["*"],
             postgresql=vault.database.SecretBackendConnectionPostgresqlArgs(
                 connection_url="postgres://username:password@host:port/database",
             ))
         # configure a static role with period-based rotations
-        period_role = vault.database.SecretBackendStaticRole("periodRole",
+        period_role = vault.database.SecretBackendStaticRole("period_role",
             backend=db.path,
+            name="my-period-role",
             db_name=postgres.name,
             username="example",
             rotation_period=3600,
             rotation_statements=["ALTER USER \\"{{name}}\\" WITH PASSWORD '{{password}}';"])
         # configure a static role with schedule-based rotations
-        schedule_role = vault.database.SecretBackendStaticRole("scheduleRole",
+        schedule_role = vault.database.SecretBackendStaticRole("schedule_role",
             backend=db.path,
+            name="my-schedule-role",
             db_name=postgres.name,
             username="example",
             rotation_schedule="0 0 * * SAT",
             rotation_window=172800,
             rotation_statements=["ALTER USER \\"{{name}}\\" WITH PASSWORD '{{password}}';"])
         ```
         <!--End PulumiCodeChooser -->
```

### Comparing `pulumi_vault-6.2.0a1713339773/pulumi_vault/database/secrets_mount.py` & `pulumi_vault-6.2.0a1713561465/pulumi_vault/database/secrets_mount.py`

 * *Files 0% similar despite different names*

```diff
@@ -1158,22 +1158,24 @@
                 username="postgres",
                 password="super_secret_2",
                 connection_url="postgresql://{{username}}:{{password}}@127.0.0.1:5432/postgres",
                 verify_connection=True,
                 allowed_roles=["dev2"],
             )])
         dev1 = vault.database.SecretBackendRole("dev1",
+            name="dev1",
             backend=db.path,
             db_name=db.mssqls[0].name,
             creation_statements=[
                 "CREATE LOGIN [{{name}}] WITH PASSWORD = '{{password}}';",
                 "CREATE USER [{{name}}] FOR LOGIN [{{name}}];",
                 "GRANT SELECT ON SCHEMA::dbo TO [{{name}}];",
             ])
         dev2 = vault.database.SecretBackendRole("dev2",
+            name="dev2",
             backend=db.path,
             db_name=db.postgresqls[0].name,
             creation_statements=[
                 "CREATE ROLE \\"{{name}}\\" WITH LOGIN PASSWORD '{{password}}' VALID UNTIL '{{expiration}}';",
                 "GRANT SELECT ON ALL TABLES IN SCHEMA public TO \\"{{name}}\\";",
             ])
         ```
@@ -1268,22 +1270,24 @@
                 username="postgres",
                 password="super_secret_2",
                 connection_url="postgresql://{{username}}:{{password}}@127.0.0.1:5432/postgres",
                 verify_connection=True,
                 allowed_roles=["dev2"],
             )])
         dev1 = vault.database.SecretBackendRole("dev1",
+            name="dev1",
             backend=db.path,
             db_name=db.mssqls[0].name,
             creation_statements=[
                 "CREATE LOGIN [{{name}}] WITH PASSWORD = '{{password}}';",
                 "CREATE USER [{{name}}] FOR LOGIN [{{name}}];",
                 "GRANT SELECT ON SCHEMA::dbo TO [{{name}}];",
             ])
         dev2 = vault.database.SecretBackendRole("dev2",
+            name="dev2",
             backend=db.path,
             db_name=db.postgresqls[0].name,
             creation_statements=[
                 "CREATE ROLE \\"{{name}}\\" WITH LOGIN PASSWORD '{{password}}' VALID UNTIL '{{expiration}}';",
                 "GRANT SELECT ON ALL TABLES IN SCHEMA public TO \\"{{name}}\\";",
             ])
         ```
```

### Comparing `pulumi_vault-6.2.0a1713339773/pulumi_vault/egp_policy.py` & `pulumi_vault-6.2.0a1713561465/pulumi_vault/egp_policy.py`

 * *Files 1% similar despite different names*

```diff
@@ -216,20 +216,20 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_vault as vault
 
         allow_all = vault.EgpPolicy("allow-all",
-            enforcement_level="soft-mandatory",
+            name="allow-all",
             paths=["*"],
+            enforcement_level="soft-mandatory",
             policy=\"\"\"main = rule {
           true
         }
-
         \"\"\")
         ```
         <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] enforcement_level: Enforcement level of Sentinel policy. Can be either `advisory` or `soft-mandatory` or `hard-mandatory`
@@ -256,20 +256,20 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_vault as vault
 
         allow_all = vault.EgpPolicy("allow-all",
-            enforcement_level="soft-mandatory",
+            name="allow-all",
             paths=["*"],
+            enforcement_level="soft-mandatory",
             policy=\"\"\"main = rule {
           true
         }
-
         \"\"\")
         ```
         <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param EgpPolicyArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
```

### Comparing `pulumi_vault-6.2.0a1713339773/pulumi_vault/gcp/__init__.py` & `pulumi_vault-6.2.0a1713561465/pulumi_vault/gcp/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1713339773/pulumi_vault/gcp/_inputs.py` & `pulumi_vault-6.2.0a1713561465/pulumi_vault/gcp/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1713339773/pulumi_vault/gcp/auth_backend.py` & `pulumi_vault-6.2.0a1713561465/pulumi_vault/gcp/auth_backend.py`

 * *Files 2% similar despite different names*

```diff
@@ -494,32 +494,14 @@
                  private_key_id: Optional[pulumi.Input[str]] = None,
                  project_id: Optional[pulumi.Input[str]] = None,
                  tune: Optional[pulumi.Input[pulumi.InputType['AuthBackendTuneArgs']]] = None,
                  __props__=None):
         """
         Provides a resource to configure the [GCP auth backend within Vault](https://www.vaultproject.io/docs/auth/gcp.html).
 
-        ## Example Usage
-
-        <!--Start PulumiCodeChooser -->
-        ```python
-        import pulumi
-        import pulumi_vault as vault
-
-        gcp = vault.gcp.AuthBackend("gcp",
-            credentials=(lambda path: open(path).read())("vault-gcp-credentials.json"),
-            custom_endpoint=vault.gcp.AuthBackendCustomEndpointArgs(
-                api="www.googleapis.com",
-                iam="iam.googleapis.com",
-                crm="cloudresourcemanager.googleapis.com",
-                compute="compute.googleapis.com",
-            ))
-        ```
-        <!--End PulumiCodeChooser -->
-
         ## Import
 
         GCP authentication backends can be imported using the backend name, e.g.
 
         ```sh
         $ pulumi import vault:gcp/authBackend:AuthBackend gcp gcp
         ```
@@ -556,32 +538,14 @@
     def __init__(__self__,
                  resource_name: str,
                  args: Optional[AuthBackendArgs] = None,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         Provides a resource to configure the [GCP auth backend within Vault](https://www.vaultproject.io/docs/auth/gcp.html).
 
-        ## Example Usage
-
-        <!--Start PulumiCodeChooser -->
-        ```python
-        import pulumi
-        import pulumi_vault as vault
-
-        gcp = vault.gcp.AuthBackend("gcp",
-            credentials=(lambda path: open(path).read())("vault-gcp-credentials.json"),
-            custom_endpoint=vault.gcp.AuthBackendCustomEndpointArgs(
-                api="www.googleapis.com",
-                iam="iam.googleapis.com",
-                crm="cloudresourcemanager.googleapis.com",
-                compute="compute.googleapis.com",
-            ))
-        ```
-        <!--End PulumiCodeChooser -->
-
         ## Import
 
         GCP authentication backends can be imported using the backend name, e.g.
 
         ```sh
         $ pulumi import vault:gcp/authBackend:AuthBackend gcp gcp
         ```
```

### Comparing `pulumi_vault-6.2.0a1713339773/pulumi_vault/gcp/auth_backend_role.py` & `pulumi_vault-6.2.0a1713561465/pulumi_vault/gcp/auth_backend_role.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1713339773/pulumi_vault/gcp/get_auth_backend_role.py` & `pulumi_vault-6.2.0a1713561465/pulumi_vault/gcp/get_auth_backend_role.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1713339773/pulumi_vault/gcp/outputs.py` & `pulumi_vault-6.2.0a1713561465/pulumi_vault/gcp/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1713339773/pulumi_vault/gcp/secret_backend.py` & `pulumi_vault-6.2.0a1713561465/pulumi_vault/gcp/secret_backend.py`

 * *Files 1% similar despite different names*

```diff
@@ -327,17 +327,18 @@
                  __props__=None):
         """
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
+        import pulumi_std as std
         import pulumi_vault as vault
 
-        gcp = vault.gcp.SecretBackend("gcp", credentials=(lambda path: open(path).read())("credentials.json"))
+        gcp = vault.gcp.SecretBackend("gcp", credentials=std.file(input="credentials.json").result)
         ```
         <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] credentials: JSON-encoded credentials to use to connect to GCP
         :param pulumi.Input[int] default_lease_ttl_seconds: The default TTL for credentials
@@ -363,17 +364,18 @@
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
+        import pulumi_std as std
         import pulumi_vault as vault
 
-        gcp = vault.gcp.SecretBackend("gcp", credentials=(lambda path: open(path).read())("credentials.json"))
+        gcp = vault.gcp.SecretBackend("gcp", credentials=std.file(input="credentials.json").result)
         ```
         <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param SecretBackendArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
```

### Comparing `pulumi_vault-6.2.0a1713339773/pulumi_vault/gcp/secret_impersonated_account.py` & `pulumi_vault-6.2.0a1713561465/pulumi_vault/gcp/secret_impersonated_account.py`

 * *Files 2% similar despite different names*

```diff
@@ -218,25 +218,26 @@
         Service Account.
 
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
-        import pulumi_gcp as gcp
+        import pulumi_google as google
+        import pulumi_std as std
         import pulumi_vault as vault
 
-        this = gcp.service_account.Account("this", account_id="my-awesome-account")
+        this = google.index.ServiceAccount("this", account_id=my-awesome-account)
         gcp = vault.gcp.SecretBackend("gcp",
             path="gcp",
-            credentials=(lambda path: open(path).read())("credentials.json"))
-        impersonated_account = vault.gcp.SecretImpersonatedAccount("impersonatedAccount",
+            credentials=std.file(input="credentials.json").result)
+        impersonated_account = vault.gcp.SecretImpersonatedAccount("impersonated_account",
             backend=gcp.path,
             impersonated_account="this",
-            service_account_email=this.email,
+            service_account_email=this["email"],
             token_scopes=["https://www.googleapis.com/auth/cloud-platform"])
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
 
         A impersonated account can be imported using its Vault Path. For example, referencing the example above,
@@ -266,25 +267,26 @@
         Service Account.
 
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
-        import pulumi_gcp as gcp
+        import pulumi_google as google
+        import pulumi_std as std
         import pulumi_vault as vault
 
-        this = gcp.service_account.Account("this", account_id="my-awesome-account")
+        this = google.index.ServiceAccount("this", account_id=my-awesome-account)
         gcp = vault.gcp.SecretBackend("gcp",
             path="gcp",
-            credentials=(lambda path: open(path).read())("credentials.json"))
-        impersonated_account = vault.gcp.SecretImpersonatedAccount("impersonatedAccount",
+            credentials=std.file(input="credentials.json").result)
+        impersonated_account = vault.gcp.SecretImpersonatedAccount("impersonated_account",
             backend=gcp.path,
             impersonated_account="this",
-            service_account_email=this.email,
+            service_account_email=this["email"],
             token_scopes=["https://www.googleapis.com/auth/cloud-platform"])
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
 
         A impersonated account can be imported using its Vault Path. For example, referencing the example above,
```

### Comparing `pulumi_vault-6.2.0a1713339773/pulumi_vault/gcp/secret_roleset.py` & `pulumi_vault-6.2.0a1713561465/pulumi_vault/gcp/secret_roleset.py`

 * *Files 0% similar despite different names*

```diff
@@ -296,20 +296,21 @@
         Each Roleset is [tied](https://www.vaultproject.io/docs/secrets/gcp/index.html#service-accounts-are-tied-to-rolesets) to a Service Account, and can have one or more [bindings](https://www.vaultproject.io/docs/secrets/gcp/index.html#roleset-bindings) associated with it.
 
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
+        import pulumi_std as std
         import pulumi_vault as vault
 
         project = "my-awesome-project"
         gcp = vault.gcp.SecretBackend("gcp",
             path="gcp",
-            credentials=(lambda path: open(path).read())("credentials.json"))
+            credentials=std.file(input="credentials.json").result)
         roleset = vault.gcp.SecretRoleset("roleset",
             backend=gcp.path,
             roleset="project_viewer",
             secret_type="access_token",
             project=project,
             token_scopes=["https://www.googleapis.com/auth/cloud-platform"],
             bindings=[vault.gcp.SecretRolesetBindingArgs(
@@ -352,20 +353,21 @@
         Each Roleset is [tied](https://www.vaultproject.io/docs/secrets/gcp/index.html#service-accounts-are-tied-to-rolesets) to a Service Account, and can have one or more [bindings](https://www.vaultproject.io/docs/secrets/gcp/index.html#roleset-bindings) associated with it.
 
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
+        import pulumi_std as std
         import pulumi_vault as vault
 
         project = "my-awesome-project"
         gcp = vault.gcp.SecretBackend("gcp",
             path="gcp",
-            credentials=(lambda path: open(path).read())("credentials.json"))
+            credentials=std.file(input="credentials.json").result)
         roleset = vault.gcp.SecretRoleset("roleset",
             backend=gcp.path,
             roleset="project_viewer",
             secret_type="access_token",
             project=project,
             token_scopes=["https://www.googleapis.com/auth/cloud-platform"],
             bindings=[vault.gcp.SecretRolesetBindingArgs(
```

### Comparing `pulumi_vault-6.2.0a1713339773/pulumi_vault/gcp/secret_static_account.py` & `pulumi_vault-6.2.0a1713561465/pulumi_vault/gcp/secret_static_account.py`

 * *Files 2% similar despite different names*

```diff
@@ -298,29 +298,30 @@
         Service Account, and can have one or more [bindings](https://www.vaultproject.io/docs/secrets/gcp/index.html#bindings) associated with it.
 
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
-        import pulumi_gcp as gcp
+        import pulumi_google as google
+        import pulumi_std as std
         import pulumi_vault as vault
 
-        this = gcp.service_account.Account("this", account_id="my-awesome-account")
+        this = google.index.ServiceAccount("this", account_id=my-awesome-account)
         gcp = vault.gcp.SecretBackend("gcp",
             path="gcp",
-            credentials=(lambda path: open(path).read())("credentials.json"))
-        static_account = vault.gcp.SecretStaticAccount("staticAccount",
+            credentials=std.file(input="credentials.json").result)
+        static_account = vault.gcp.SecretStaticAccount("static_account",
             backend=gcp.path,
             static_account="project_viewer",
             secret_type="access_token",
             token_scopes=["https://www.googleapis.com/auth/cloud-platform"],
-            service_account_email=this.email,
+            service_account_email=this["email"],
             bindings=[vault.gcp.SecretStaticAccountBindingArgs(
-                resource=this.project.apply(lambda project: f"//cloudresourcemanager.googleapis.com/projects/{project}"),
+                resource=f"//cloudresourcemanager.googleapis.com/projects/{this['project']}",
                 roles=["roles/viewer"],
             )])
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
 
@@ -356,29 +357,30 @@
         Service Account, and can have one or more [bindings](https://www.vaultproject.io/docs/secrets/gcp/index.html#bindings) associated with it.
 
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
-        import pulumi_gcp as gcp
+        import pulumi_google as google
+        import pulumi_std as std
         import pulumi_vault as vault
 
-        this = gcp.service_account.Account("this", account_id="my-awesome-account")
+        this = google.index.ServiceAccount("this", account_id=my-awesome-account)
         gcp = vault.gcp.SecretBackend("gcp",
             path="gcp",
-            credentials=(lambda path: open(path).read())("credentials.json"))
-        static_account = vault.gcp.SecretStaticAccount("staticAccount",
+            credentials=std.file(input="credentials.json").result)
+        static_account = vault.gcp.SecretStaticAccount("static_account",
             backend=gcp.path,
             static_account="project_viewer",
             secret_type="access_token",
             token_scopes=["https://www.googleapis.com/auth/cloud-platform"],
-            service_account_email=this.email,
+            service_account_email=this["email"],
             bindings=[vault.gcp.SecretStaticAccountBindingArgs(
-                resource=this.project.apply(lambda project: f"//cloudresourcemanager.googleapis.com/projects/{project}"),
+                resource=f"//cloudresourcemanager.googleapis.com/projects/{this['project']}",
                 roles=["roles/viewer"],
             )])
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
```

### Comparing `pulumi_vault-6.2.0a1713339773/pulumi_vault/generic/endpoint.py` & `pulumi_vault-6.2.0a1713561465/pulumi_vault/generic/endpoint.py`

 * *Files 1% similar despite different names*

```diff
@@ -418,24 +418,24 @@
             ignore_absent_fields=True,
             data_json=\"\"\"{
           "policies": ["p1"],
           "password": "changeme"
         }
         \"\"\",
             opts=pulumi.ResourceOptions(depends_on=[userpass]))
-        u1_token = vault.generic.Endpoint("u1Token",
+        u1_token = vault.generic.Endpoint("u1_token",
             path="auth/userpass/login/u1",
             disable_read=True,
             disable_delete=True,
             data_json=\"\"\"{
           "password": "changeme"
         }
         \"\"\",
             opts=pulumi.ResourceOptions(depends_on=[u1]))
-        u1_entity = vault.generic.Endpoint("u1Entity",
+        u1_entity = vault.generic.Endpoint("u1_entity",
             disable_read=True,
             disable_delete=True,
             path="identity/lookup/entity",
             ignore_absent_fields=True,
             write_fields=["id"],
             data_json=\"\"\"{
           "alias_name": "u1",
@@ -513,24 +513,24 @@
             ignore_absent_fields=True,
             data_json=\"\"\"{
           "policies": ["p1"],
           "password": "changeme"
         }
         \"\"\",
             opts=pulumi.ResourceOptions(depends_on=[userpass]))
-        u1_token = vault.generic.Endpoint("u1Token",
+        u1_token = vault.generic.Endpoint("u1_token",
             path="auth/userpass/login/u1",
             disable_read=True,
             disable_delete=True,
             data_json=\"\"\"{
           "password": "changeme"
         }
         \"\"\",
             opts=pulumi.ResourceOptions(depends_on=[u1]))
-        u1_entity = vault.generic.Endpoint("u1Entity",
+        u1_entity = vault.generic.Endpoint("u1_entity",
             disable_read=True,
             disable_delete=True,
             path="identity/lookup/entity",
             ignore_absent_fields=True,
             write_fields=["id"],
             data_json=\"\"\"{
           "alias_name": "u1",
```

### Comparing `pulumi_vault-6.2.0a1713339773/pulumi_vault/generic/get_secret.py` & `pulumi_vault-6.2.0a1713561465/pulumi_vault/generic/get_secret.py`

 * *Files 6% similar despite different names*

```diff
@@ -167,14 +167,36 @@
     import pulumi
     import pulumi_vault as vault
 
     rundeck_auth = vault.generic.get_secret(path="secret/rundeck_auth")
     ```
     <!--End PulumiCodeChooser -->
 
+    ### KV
+
+    For this example, consider `example` as a path for a KV engine.
+
+    <!--Start PulumiCodeChooser -->
+    ```python
+    import pulumi
+    import pulumi_vault as vault
+
+
+    def not_implemented(msg):
+        raise NotImplementedError(msg)
+
+    example_creds = vault.generic.get_secret(path="example/creds")
+    example_template = not_implemented("The template_file data resource is not yet supported.")
+    ```
+    <!--End PulumiCodeChooser -->
+
+    ## Required Vault Capabilities
+
+    Use of this resource requires the `read` capability on the given path.
+
 
     :param str namespace: The namespace of the target resource.
            The value should not contain leading or trailing forward slashes.
            The `namespace` is always relative to the provider's configured [namespace](https://www.terraform.io/docs/providers/vault/index.html#namespace).
            *Available only for Vault Enterprise*.
     :param str path: The full logical path from which to request data.
            To read data from the "generic" secret backend mounted in Vault by
@@ -226,14 +248,36 @@
     import pulumi
     import pulumi_vault as vault
 
     rundeck_auth = vault.generic.get_secret(path="secret/rundeck_auth")
     ```
     <!--End PulumiCodeChooser -->
 
+    ### KV
+
+    For this example, consider `example` as a path for a KV engine.
+
+    <!--Start PulumiCodeChooser -->
+    ```python
+    import pulumi
+    import pulumi_vault as vault
+
+
+    def not_implemented(msg):
+        raise NotImplementedError(msg)
+
+    example_creds = vault.generic.get_secret(path="example/creds")
+    example_template = not_implemented("The template_file data resource is not yet supported.")
+    ```
+    <!--End PulumiCodeChooser -->
+
+    ## Required Vault Capabilities
+
+    Use of this resource requires the `read` capability on the given path.
+
 
     :param str namespace: The namespace of the target resource.
            The value should not contain leading or trailing forward slashes.
            The `namespace` is always relative to the provider's configured [namespace](https://www.terraform.io/docs/providers/vault/index.html#namespace).
            *Available only for Vault Enterprise*.
     :param str path: The full logical path from which to request data.
            To read data from the "generic" secret backend mounted in Vault by
```

### Comparing `pulumi_vault-6.2.0a1713339773/pulumi_vault/generic/secret.py` & `pulumi_vault-6.2.0a1713561465/pulumi_vault/generic/secret.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1713339773/pulumi_vault/get_auth_backend.py` & `pulumi_vault-6.2.0a1713561465/pulumi_vault/get_auth_backend.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1713339773/pulumi_vault/get_auth_backends.py` & `pulumi_vault-6.2.0a1713561465/pulumi_vault/get_auth_backends.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1713339773/pulumi_vault/get_namespace.py` & `pulumi_vault-6.2.0a1713561465/pulumi_vault/get_namespace.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1713339773/pulumi_vault/get_namespaces.py` & `pulumi_vault-6.2.0a1713561465/pulumi_vault/get_namespaces.py`

 * *Files 4% similar despite different names*

```diff
@@ -87,16 +87,16 @@
 
     <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_vault as vault
 
     children = vault.get_namespaces(namespace="parent")
-    child = [vault.get_namespace(namespace=children.namespace,
-        path=__key) for __key, __value in children.paths]
+    child = {__key: vault.get_namespace(namespace=children.namespace,
+        path=__key) for __key, __value in children.paths}
     ```
     <!--End PulumiCodeChooser -->
 
 
     :param str namespace: The namespace to provision the resource in.
            The value should not contain leading or trailing forward slashes.
            The `namespace` is always relative to the provider's configured [namespace](https://www.terraform.io/docs/providers/vault#namespace).
@@ -135,16 +135,16 @@
 
     <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_vault as vault
 
     children = vault.get_namespaces(namespace="parent")
-    child = [vault.get_namespace(namespace=children.namespace,
-        path=__key) for __key, __value in children.paths]
+    child = {__key: vault.get_namespace(namespace=children.namespace,
+        path=__key) for __key, __value in children.paths}
     ```
     <!--End PulumiCodeChooser -->
 
 
     :param str namespace: The namespace to provision the resource in.
            The value should not contain leading or trailing forward slashes.
            The `namespace` is always relative to the provider's configured [namespace](https://www.terraform.io/docs/providers/vault#namespace).
```

### Comparing `pulumi_vault-6.2.0a1713339773/pulumi_vault/get_nomad_access_token.py` & `pulumi_vault-6.2.0a1713561465/pulumi_vault/get_nomad_access_token.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1713339773/pulumi_vault/get_policy_document.py` & `pulumi_vault-6.2.0a1713561465/pulumi_vault/get_policy_document.py`

 * *Files 4% similar despite different names*

```diff
@@ -85,26 +85,28 @@
     ## Example Usage
 
     <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_vault as vault
 
-    example_policy_document = vault.get_policy_document(rules=[vault.GetPolicyDocumentRuleArgs(
+    example = vault.get_policy_document(rules=[vault.GetPolicyDocumentRuleArgs(
         path="secret/*",
         capabilities=[
             "create",
             "read",
             "update",
             "delete",
             "list",
         ],
         description="allow all on secrets",
     )])
-    example_policy = vault.Policy("examplePolicy", policy=example_policy_document.hcl)
+    example_policy = vault.Policy("example",
+        name="example_policy",
+        policy=example.hcl)
     ```
     <!--End PulumiCodeChooser -->
     """
     __args__ = dict()
     __args__['namespace'] = namespace
     __args__['rules'] = rules
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
@@ -127,23 +129,25 @@
     ## Example Usage
 
     <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_vault as vault
 
-    example_policy_document = vault.get_policy_document(rules=[vault.GetPolicyDocumentRuleArgs(
+    example = vault.get_policy_document(rules=[vault.GetPolicyDocumentRuleArgs(
         path="secret/*",
         capabilities=[
             "create",
             "read",
             "update",
             "delete",
             "list",
         ],
         description="allow all on secrets",
     )])
-    example_policy = vault.Policy("examplePolicy", policy=example_policy_document.hcl)
+    example_policy = vault.Policy("example",
+        name="example_policy",
+        policy=example.hcl)
     ```
     <!--End PulumiCodeChooser -->
     """
     ...
```

### Comparing `pulumi_vault-6.2.0a1713339773/pulumi_vault/get_raft_autopilot_state.py` & `pulumi_vault-6.2.0a1713561465/pulumi_vault/get_raft_autopilot_state.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1713339773/pulumi_vault/github/_inputs.py` & `pulumi_vault-6.2.0a1713561465/pulumi_vault/github/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1713339773/pulumi_vault/github/auth_backend.py` & `pulumi_vault-6.2.0a1713561465/pulumi_vault/github/auth_backend.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1713339773/pulumi_vault/github/outputs.py` & `pulumi_vault-6.2.0a1713561465/pulumi_vault/github/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1713339773/pulumi_vault/github/team.py` & `pulumi_vault-6.2.0a1713561465/pulumi_vault/github/team.py`

 * *Files 1% similar despite different names*

```diff
@@ -193,15 +193,15 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_vault as vault
 
         example = vault.github.AuthBackend("example", organization="myorg")
-        tf_devs = vault.github.Team("tfDevs",
+        tf_devs = vault.github.Team("tf_devs",
             backend=example.id,
             team="terraform-developers",
             policies=[
                 "developer",
                 "read-only",
             ])
         ```
@@ -242,15 +242,15 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_vault as vault
 
         example = vault.github.AuthBackend("example", organization="myorg")
-        tf_devs = vault.github.Team("tfDevs",
+        tf_devs = vault.github.Team("tf_devs",
             backend=example.id,
             team="terraform-developers",
             policies=[
                 "developer",
                 "read-only",
             ])
         ```
```

### Comparing `pulumi_vault-6.2.0a1713339773/pulumi_vault/github/user.py` & `pulumi_vault-6.2.0a1713561465/pulumi_vault/github/user.py`

 * *Files 0% similar despite different names*

```diff
@@ -193,15 +193,15 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_vault as vault
 
         example = vault.github.AuthBackend("example", organization="myorg")
-        tf_user = vault.github.User("tfUser",
+        tf_user = vault.github.User("tf_user",
             backend=example.id,
             user="john.doe",
             policies=[
                 "developer",
                 "read-only",
             ])
         ```
@@ -242,15 +242,15 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_vault as vault
 
         example = vault.github.AuthBackend("example", organization="myorg")
-        tf_user = vault.github.User("tfUser",
+        tf_user = vault.github.User("tf_user",
             backend=example.id,
             user="john.doe",
             policies=[
                 "developer",
                 "read-only",
             ])
         ```
```

### Comparing `pulumi_vault-6.2.0a1713339773/pulumi_vault/identity/__init__.py` & `pulumi_vault-6.2.0a1713561465/pulumi_vault/identity/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1713339773/pulumi_vault/identity/entity.py` & `pulumi_vault-6.2.0a1713561465/pulumi_vault/identity/entity.py`

 * *Files 1% similar despite different names*

```diff
@@ -248,18 +248,19 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_vault as vault
 
         test = vault.identity.Entity("test",
+            name="tester1",
+            policies=["test"],
             metadata={
                 "foo": "bar",
-            },
-            policies=["test"])
+            })
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
 
         Identity entity can be imported using the `id`, e.g.
 
@@ -290,18 +291,19 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_vault as vault
 
         test = vault.identity.Entity("test",
+            name="tester1",
+            policies=["test"],
             metadata={
                 "foo": "bar",
-            },
-            policies=["test"])
+            })
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
 
         Identity entity can be imported using the `id`, e.g.
```

### Comparing `pulumi_vault-6.2.0a1713339773/pulumi_vault/identity/entity_alias.py` & `pulumi_vault-6.2.0a1713561465/pulumi_vault/identity/entity_alias.py`

 * *Files 1% similar despite different names*

```diff
@@ -213,16 +213,17 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_vault as vault
 
         test = vault.identity.EntityAlias("test",
-            canonical_id="49877D63-07AD-4B85-BDA8-B61626C477E8",
-            mount_accessor="token_1f2bd5")
+            name="user_1",
+            mount_accessor="token_1f2bd5",
+            canonical_id="49877D63-07AD-4B85-BDA8-B61626C477E8")
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
 
         Identity entity alias can be imported using the `id`, e.g.
 
@@ -252,16 +253,17 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_vault as vault
 
         test = vault.identity.EntityAlias("test",
-            canonical_id="49877D63-07AD-4B85-BDA8-B61626C477E8",
-            mount_accessor="token_1f2bd5")
+            name="user_1",
+            mount_accessor="token_1f2bd5",
+            canonical_id="49877D63-07AD-4B85-BDA8-B61626C477E8")
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
 
         Identity entity alias can be imported using the `id`, e.g.
```

### Comparing `pulumi_vault-6.2.0a1713339773/pulumi_vault/identity/entity_policies.py` & `pulumi_vault-6.2.0a1713561465/pulumi_vault/identity/entity_policies.py`

 * *Files 0% similar despite different names*

```diff
@@ -215,15 +215,17 @@
         ### Exclusive Policies
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_vault as vault
 
-        entity = vault.identity.Entity("entity", external_policies=True)
+        entity = vault.identity.Entity("entity",
+            name="entity",
+            external_policies=True)
         policies = vault.identity.EntityPolicies("policies",
             policies=[
                 "default",
                 "test",
             ],
             exclusive=True,
             entity_id=entity.id)
@@ -233,15 +235,17 @@
         ### Non-exclusive Policies
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_vault as vault
 
-        entity = vault.identity.Entity("entity", external_policies=True)
+        entity = vault.identity.Entity("entity",
+            name="entity",
+            external_policies=True)
         default = vault.identity.EntityPolicies("default",
             policies=[
                 "default",
                 "test",
             ],
             exclusive=False,
             entity_id=entity.id)
@@ -280,15 +284,17 @@
         ### Exclusive Policies
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_vault as vault
 
-        entity = vault.identity.Entity("entity", external_policies=True)
+        entity = vault.identity.Entity("entity",
+            name="entity",
+            external_policies=True)
         policies = vault.identity.EntityPolicies("policies",
             policies=[
                 "default",
                 "test",
             ],
             exclusive=True,
             entity_id=entity.id)
@@ -298,15 +304,17 @@
         ### Non-exclusive Policies
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_vault as vault
 
-        entity = vault.identity.Entity("entity", external_policies=True)
+        entity = vault.identity.Entity("entity",
+            name="entity",
+            external_policies=True)
         default = vault.identity.EntityPolicies("default",
             policies=[
                 "default",
                 "test",
             ],
             exclusive=False,
             entity_id=entity.id)
```

### Comparing `pulumi_vault-6.2.0a1713339773/pulumi_vault/identity/get_entity.py` & `pulumi_vault-6.2.0a1713561465/pulumi_vault/identity/get_entity.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1713339773/pulumi_vault/identity/get_group.py` & `pulumi_vault-6.2.0a1713561465/pulumi_vault/identity/get_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1713339773/pulumi_vault/identity/get_oidc_client_creds.py` & `pulumi_vault-6.2.0a1713561465/pulumi_vault/identity/get_oidc_client_creds.py`

 * *Files 2% similar despite different names*

```diff
@@ -95,14 +95,15 @@
 
     <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_vault as vault
 
     app = vault.identity.OidcClient("app",
+        name="application",
         redirect_uris=[
             "http://127.0.0.1:9200/v1/auth-methods/oidc:authenticate:callback",
             "http://127.0.0.1:8251/callback",
             "http://127.0.0.1:8080/callback",
         ],
         id_token_ttl=2400,
         access_token_ttl=7200)
@@ -140,14 +141,15 @@
 
     <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_vault as vault
 
     app = vault.identity.OidcClient("app",
+        name="application",
         redirect_uris=[
             "http://127.0.0.1:9200/v1/auth-methods/oidc:authenticate:callback",
             "http://127.0.0.1:8251/callback",
             "http://127.0.0.1:8080/callback",
         ],
         id_token_ttl=2400,
         access_token_ttl=7200)
```

### Comparing `pulumi_vault-6.2.0a1713339773/pulumi_vault/identity/get_oidc_openid_config.py` & `pulumi_vault-6.2.0a1713561465/pulumi_vault/identity/get_oidc_openid_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -216,27 +216,31 @@
 
     <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_vault as vault
 
     key = vault.identity.OidcKey("key",
+        name="key",
         allowed_client_ids=["*"],
         rotation_period=3600,
         verification_ttl=3600)
     app = vault.identity.OidcClient("app",
+        name="application",
         key=key.name,
         redirect_uris=[
             "http://127.0.0.1:9200/v1/auth-methods/oidc:authenticate:callback",
             "http://127.0.0.1:8251/callback",
             "http://127.0.0.1:8080/callback",
         ],
         id_token_ttl=2400,
         access_token_ttl=7200)
-    provider = vault.identity.OidcProvider("provider", allowed_client_ids=[vault_identity_oidc_client["test"]["client_id"]])
+    provider = vault.identity.OidcProvider("provider",
+        name="provider",
+        allowed_client_ids=[test["clientId"]])
     config = vault.identity.get_oidc_openid_config_output(name=provider.name)
     ```
     <!--End PulumiCodeChooser -->
 
 
     :param str name: The name of the OIDC Provider in Vault.
     :param str namespace: The namespace of the target resource.
@@ -277,27 +281,31 @@
 
     <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_vault as vault
 
     key = vault.identity.OidcKey("key",
+        name="key",
         allowed_client_ids=["*"],
         rotation_period=3600,
         verification_ttl=3600)
     app = vault.identity.OidcClient("app",
+        name="application",
         key=key.name,
         redirect_uris=[
             "http://127.0.0.1:9200/v1/auth-methods/oidc:authenticate:callback",
             "http://127.0.0.1:8251/callback",
             "http://127.0.0.1:8080/callback",
         ],
         id_token_ttl=2400,
         access_token_ttl=7200)
-    provider = vault.identity.OidcProvider("provider", allowed_client_ids=[vault_identity_oidc_client["test"]["client_id"]])
+    provider = vault.identity.OidcProvider("provider",
+        name="provider",
+        allowed_client_ids=[test["clientId"]])
     config = vault.identity.get_oidc_openid_config_output(name=provider.name)
     ```
     <!--End PulumiCodeChooser -->
 
 
     :param str name: The name of the OIDC Provider in Vault.
     :param str namespace: The namespace of the target resource.
```

### Comparing `pulumi_vault-6.2.0a1713339773/pulumi_vault/identity/get_oidc_public_keys.py` & `pulumi_vault-6.2.0a1713561465/pulumi_vault/identity/get_oidc_public_keys.py`

 * *Files 3% similar despite different names*

```diff
@@ -83,27 +83,31 @@
 
     <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_vault as vault
 
     key = vault.identity.OidcKey("key",
+        name="key",
         allowed_client_ids=["*"],
         rotation_period=3600,
         verification_ttl=3600)
     app = vault.identity.OidcClient("app",
+        name="application",
         key=key.name,
         redirect_uris=[
             "http://127.0.0.1:9200/v1/auth-methods/oidc:authenticate:callback",
             "http://127.0.0.1:8251/callback",
             "http://127.0.0.1:8080/callback",
         ],
         id_token_ttl=2400,
         access_token_ttl=7200)
-    provider = vault.identity.OidcProvider("provider", allowed_client_ids=[vault_identity_oidc_client["test"]["client_id"]])
+    provider = vault.identity.OidcProvider("provider",
+        name="provider",
+        allowed_client_ids=[test["clientId"]])
     public_keys = vault.identity.get_oidc_public_keys_output(name=provider.name)
     ```
     <!--End PulumiCodeChooser -->
 
 
     :param str name: The name of the OIDC Provider in Vault.
     :param str namespace: The namespace of the target resource.
@@ -133,27 +137,31 @@
 
     <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_vault as vault
 
     key = vault.identity.OidcKey("key",
+        name="key",
         allowed_client_ids=["*"],
         rotation_period=3600,
         verification_ttl=3600)
     app = vault.identity.OidcClient("app",
+        name="application",
         key=key.name,
         redirect_uris=[
             "http://127.0.0.1:9200/v1/auth-methods/oidc:authenticate:callback",
             "http://127.0.0.1:8251/callback",
             "http://127.0.0.1:8080/callback",
         ],
         id_token_ttl=2400,
         access_token_ttl=7200)
-    provider = vault.identity.OidcProvider("provider", allowed_client_ids=[vault_identity_oidc_client["test"]["client_id"]])
+    provider = vault.identity.OidcProvider("provider",
+        name="provider",
+        allowed_client_ids=[test["clientId"]])
     public_keys = vault.identity.get_oidc_public_keys_output(name=provider.name)
     ```
     <!--End PulumiCodeChooser -->
 
 
     :param str name: The name of the OIDC Provider in Vault.
     :param str namespace: The namespace of the target resource.
```

### Comparing `pulumi_vault-6.2.0a1713339773/pulumi_vault/identity/group.py` & `pulumi_vault-6.2.0a1713561465/pulumi_vault/identity/group.py`

 * *Files 1% similar despite different names*

```diff
@@ -418,70 +418,74 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_vault as vault
 
         internal = vault.identity.Group("internal",
-            metadata={
-                "version": "2",
-            },
+            name="internal",
+            type="internal",
             policies=[
                 "dev",
                 "test",
             ],
-            type="internal")
+            metadata={
+                "version": "2",
+            })
         ```
         <!--End PulumiCodeChooser -->
 
         ### External Group
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_vault as vault
 
         group = vault.identity.Group("group",
+            name="external",
+            type="external",
+            policies=["test"],
             metadata={
                 "version": "1",
-            },
-            policies=["test"],
-            type="external")
+            })
         ```
         <!--End PulumiCodeChooser -->
 
         ## Caveats
 
         It's important to note that Vault identity groups names are *case-insensitive*. For example the following resources would be equivalent.
         Applying this configuration would result in the provider failing to create one of the identity groups, since the resources share the same `name`.
 
         This sort of pattern should be avoided:
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_vault as vault
 
-        internal_identity_group_group = vault.identity.Group("internalIdentity/groupGroup",
-            metadata={
-                "version": "2",
-            },
+        internal = vault.identity.Group("internal",
+            name="internal",
+            type="internal",
             policies=[
                 "dev",
                 "test",
             ],
-            type="internal")
-        internal_group = vault.identity.Group("internalGroup",
             metadata={
                 "version": "2",
-            },
+            })
+        internal_group = vault.identity.Group("Internal",
+            name="Internal",
+            type="internal",
             policies=[
                 "dev",
                 "test",
             ],
-            type="internal")
+            metadata={
+                "version": "2",
+            })
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
 
         Identity group can be imported using the `id`, e.g.
 
@@ -530,70 +534,74 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_vault as vault
 
         internal = vault.identity.Group("internal",
-            metadata={
-                "version": "2",
-            },
+            name="internal",
+            type="internal",
             policies=[
                 "dev",
                 "test",
             ],
-            type="internal")
+            metadata={
+                "version": "2",
+            })
         ```
         <!--End PulumiCodeChooser -->
 
         ### External Group
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_vault as vault
 
         group = vault.identity.Group("group",
+            name="external",
+            type="external",
+            policies=["test"],
             metadata={
                 "version": "1",
-            },
-            policies=["test"],
-            type="external")
+            })
         ```
         <!--End PulumiCodeChooser -->
 
         ## Caveats
 
         It's important to note that Vault identity groups names are *case-insensitive*. For example the following resources would be equivalent.
         Applying this configuration would result in the provider failing to create one of the identity groups, since the resources share the same `name`.
 
         This sort of pattern should be avoided:
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_vault as vault
 
-        internal_identity_group_group = vault.identity.Group("internalIdentity/groupGroup",
-            metadata={
-                "version": "2",
-            },
+        internal = vault.identity.Group("internal",
+            name="internal",
+            type="internal",
             policies=[
                 "dev",
                 "test",
             ],
-            type="internal")
-        internal_group = vault.identity.Group("internalGroup",
             metadata={
                 "version": "2",
-            },
+            })
+        internal_group = vault.identity.Group("Internal",
+            name="Internal",
+            type="internal",
             policies=[
                 "dev",
                 "test",
             ],
-            type="internal")
+            metadata={
+                "version": "2",
+            })
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
 
         Identity group can be imported using the `id`, e.g.
```

### Comparing `pulumi_vault-6.2.0a1713339773/pulumi_vault/identity/group_alias.py` & `pulumi_vault-6.2.0a1713561465/pulumi_vault/identity/group_alias.py`

 * *Files 0% similar despite different names*

```diff
@@ -183,14 +183,15 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_vault as vault
 
         group = vault.identity.Group("group",
+            name="test",
             type="external",
             policies=["test"])
         github = vault.AuthBackend("github",
             type="github",
             path="github")
         group_alias = vault.identity.GroupAlias("group-alias",
             name="Github_Team_Slug",
@@ -238,14 +239,15 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_vault as vault
 
         group = vault.identity.Group("group",
+            name="test",
             type="external",
             policies=["test"])
         github = vault.AuthBackend("github",
             type="github",
             path="github")
         group_alias = vault.identity.GroupAlias("group-alias",
             name="Github_Team_Slug",
```

### Comparing `pulumi_vault-6.2.0a1713339773/pulumi_vault/identity/group_member_entity_ids.py` & `pulumi_vault-6.2.0a1713561465/pulumi_vault/identity/group_member_entity_ids.py`

 * *Files 2% similar despite different names*

```diff
@@ -201,20 +201,21 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_vault as vault
 
         internal = vault.identity.Group("internal",
+            name="internal",
             type="internal",
             external_member_entity_ids=True,
             metadata={
                 "version": "2",
             })
-        user = vault.identity.Entity("user")
+        user = vault.identity.Entity("user", name="user")
         members = vault.identity.GroupMemberEntityIds("members",
             exclusive=True,
             member_entity_ids=[user.id],
             group_id=internal.id)
         ```
         <!--End PulumiCodeChooser -->
 
@@ -222,22 +223,23 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_vault as vault
 
         internal = vault.identity.Group("internal",
+            name="internal",
             type="internal",
             external_member_entity_ids=True,
             metadata={
                 "version": "2",
             })
-        test_user = vault.identity.Entity("testUser")
-        second_test_user = vault.identity.Entity("secondTestUser")
-        dev_user = vault.identity.Entity("devUser")
+        test_user = vault.identity.Entity("test_user", name="test")
+        second_test_user = vault.identity.Entity("second_test_user", name="second_test")
+        dev_user = vault.identity.Entity("dev_user", name="dev")
         test = vault.identity.GroupMemberEntityIds("test",
             member_entity_ids=[
                 test_user.id,
                 second_test_user.id,
             ],
             exclusive=False,
             group_id=internal.id)
@@ -277,20 +279,21 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_vault as vault
 
         internal = vault.identity.Group("internal",
+            name="internal",
             type="internal",
             external_member_entity_ids=True,
             metadata={
                 "version": "2",
             })
-        user = vault.identity.Entity("user")
+        user = vault.identity.Entity("user", name="user")
         members = vault.identity.GroupMemberEntityIds("members",
             exclusive=True,
             member_entity_ids=[user.id],
             group_id=internal.id)
         ```
         <!--End PulumiCodeChooser -->
 
@@ -298,22 +301,23 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_vault as vault
 
         internal = vault.identity.Group("internal",
+            name="internal",
             type="internal",
             external_member_entity_ids=True,
             metadata={
                 "version": "2",
             })
-        test_user = vault.identity.Entity("testUser")
-        second_test_user = vault.identity.Entity("secondTestUser")
-        dev_user = vault.identity.Entity("devUser")
+        test_user = vault.identity.Entity("test_user", name="test")
+        second_test_user = vault.identity.Entity("second_test_user", name="second_test")
+        dev_user = vault.identity.Entity("dev_user", name="dev")
         test = vault.identity.GroupMemberEntityIds("test",
             member_entity_ids=[
                 test_user.id,
                 second_test_user.id,
             ],
             exclusive=False,
             group_id=internal.id)
```

### Comparing `pulumi_vault-6.2.0a1713339773/pulumi_vault/identity/group_member_group_ids.py` & `pulumi_vault-6.2.0a1713561465/pulumi_vault/identity/group_member_group_ids.py`

 * *Files 1% similar despite different names*

```diff
@@ -215,22 +215,25 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_vault as vault
 
         internal = vault.identity.Group("internal",
+            name="internal",
             type="internal",
             external_member_group_ids=True,
             metadata={
                 "version": "2",
             })
-        users = vault.identity.Group("users", metadata={
-            "version": "2",
-        })
+        users = vault.identity.Group("users",
+            name="users",
+            metadata={
+                "version": "2",
+            })
         members = vault.identity.GroupMemberGroupIds("members",
             exclusive=True,
             member_group_ids=[users.id],
             group_id=internal.id)
         ```
         <!--End PulumiCodeChooser -->
 
@@ -238,22 +241,25 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_vault as vault
 
         internal = vault.identity.Group("internal",
+            name="internal",
             type="internal",
             external_member_group_ids=True,
             metadata={
                 "version": "2",
             })
-        users = vault.identity.Group("users", metadata={
-            "version": "2",
-        })
+        users = vault.identity.Group("users",
+            name="users",
+            metadata={
+                "version": "2",
+            })
         members = vault.identity.GroupMemberGroupIds("members",
             exclusive=False,
             member_group_ids=[users.id],
             group_id=internal.id)
         ```
         <!--End PulumiCodeChooser -->
 
@@ -291,22 +297,25 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_vault as vault
 
         internal = vault.identity.Group("internal",
+            name="internal",
             type="internal",
             external_member_group_ids=True,
             metadata={
                 "version": "2",
             })
-        users = vault.identity.Group("users", metadata={
-            "version": "2",
-        })
+        users = vault.identity.Group("users",
+            name="users",
+            metadata={
+                "version": "2",
+            })
         members = vault.identity.GroupMemberGroupIds("members",
             exclusive=True,
             member_group_ids=[users.id],
             group_id=internal.id)
         ```
         <!--End PulumiCodeChooser -->
 
@@ -314,22 +323,25 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_vault as vault
 
         internal = vault.identity.Group("internal",
+            name="internal",
             type="internal",
             external_member_group_ids=True,
             metadata={
                 "version": "2",
             })
-        users = vault.identity.Group("users", metadata={
-            "version": "2",
-        })
+        users = vault.identity.Group("users",
+            name="users",
+            metadata={
+                "version": "2",
+            })
         members = vault.identity.GroupMemberGroupIds("members",
             exclusive=False,
             member_group_ids=[users.id],
             group_id=internal.id)
         ```
         <!--End PulumiCodeChooser -->
```

### Comparing `pulumi_vault-6.2.0a1713339773/pulumi_vault/identity/group_policies.py` & `pulumi_vault-6.2.0a1713561465/pulumi_vault/identity/group_policies.py`

 * *Files 1% similar despite different names*

```diff
@@ -216,14 +216,15 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_vault as vault
 
         internal = vault.identity.Group("internal",
+            name="internal",
             type="internal",
             external_policies=True,
             metadata={
                 "version": "2",
             })
         policies = vault.identity.GroupPolicies("policies",
             policies=[
@@ -239,14 +240,15 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_vault as vault
 
         internal = vault.identity.Group("internal",
+            name="internal",
             type="internal",
             external_policies=True,
             metadata={
                 "version": "2",
             })
         default = vault.identity.GroupPolicies("default",
             policies=[
@@ -291,14 +293,15 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_vault as vault
 
         internal = vault.identity.Group("internal",
+            name="internal",
             type="internal",
             external_policies=True,
             metadata={
                 "version": "2",
             })
         policies = vault.identity.GroupPolicies("policies",
             policies=[
@@ -314,14 +317,15 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_vault as vault
 
         internal = vault.identity.Group("internal",
+            name="internal",
             type="internal",
             external_policies=True,
             metadata={
                 "version": "2",
             })
         default = vault.identity.GroupPolicies("default",
             policies=[
```

### Comparing `pulumi_vault-6.2.0a1713339773/pulumi_vault/identity/mfa_duo.py` & `pulumi_vault-6.2.0a1713561465/pulumi_vault/identity/mfa_duo.py`

 * *Files 0% similar despite different names*

```diff
@@ -381,16 +381,16 @@
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_vault as vault
 
         example = vault.identity.MfaDuo("example",
             api_hostname="api-xxxxxxxx.duosecurity.com",
-            integration_key="secret-int-key",
-            secret_key="secret-key")
+            secret_key="secret-key",
+            integration_key="secret-int-key")
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
 
         Resource can be imported using its `uuid` field, e.g.
 
@@ -422,16 +422,16 @@
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_vault as vault
 
         example = vault.identity.MfaDuo("example",
             api_hostname="api-xxxxxxxx.duosecurity.com",
-            integration_key="secret-int-key",
-            secret_key="secret-key")
+            secret_key="secret-key",
+            integration_key="secret-int-key")
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
 
         Resource can be imported using its `uuid` field, e.g.
```

### Comparing `pulumi_vault-6.2.0a1713339773/pulumi_vault/identity/mfa_login_enforcement.py` & `pulumi_vault-6.2.0a1713561465/pulumi_vault/identity/mfa_login_enforcement.py`

 * *Files 1% similar despite different names*

```diff
@@ -317,20 +317,22 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_vault as vault
 
-        example_mfa_duo = vault.identity.MfaDuo("exampleMfaDuo",
+        example = vault.identity.MfaDuo("example",
             secret_key="secret-key",
             integration_key="int-key",
             api_hostname="foo.baz",
             push_info="push-info")
-        example_mfa_login_enforcement = vault.identity.MfaLoginEnforcement("exampleMfaLoginEnforcement", mfa_method_ids=[example_mfa_duo.method_id])
+        example_mfa_login_enforcement = vault.identity.MfaLoginEnforcement("example",
+            name="default",
+            mfa_method_ids=[example.method_id])
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
 
         Resource can be imported using its `name` field, e.g.
 
@@ -360,20 +362,22 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_vault as vault
 
-        example_mfa_duo = vault.identity.MfaDuo("exampleMfaDuo",
+        example = vault.identity.MfaDuo("example",
             secret_key="secret-key",
             integration_key="int-key",
             api_hostname="foo.baz",
             push_info="push-info")
-        example_mfa_login_enforcement = vault.identity.MfaLoginEnforcement("exampleMfaLoginEnforcement", mfa_method_ids=[example_mfa_duo.method_id])
+        example_mfa_login_enforcement = vault.identity.MfaLoginEnforcement("example",
+            name="default",
+            mfa_method_ids=[example.method_id])
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
 
         Resource can be imported using its `name` field, e.g.
```

### Comparing `pulumi_vault-6.2.0a1713339773/pulumi_vault/identity/mfa_okta.py` & `pulumi_vault-6.2.0a1713561465/pulumi_vault/identity/mfa_okta.py`

 * *Files 0% similar despite different names*

```diff
@@ -348,17 +348,17 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_vault as vault
 
         example = vault.identity.MfaOkta("example",
+            org_name="org1",
             api_token="token1",
-            base_url="qux.baz.com",
-            org_name="org1")
+            base_url="qux.baz.com")
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
 
         Resource can be imported using its `uuid` field, e.g.
 
@@ -388,17 +388,17 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_vault as vault
 
         example = vault.identity.MfaOkta("example",
+            org_name="org1",
             api_token="token1",
-            base_url="qux.baz.com",
-            org_name="org1")
+            base_url="qux.baz.com")
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
 
         Resource can be imported using its `uuid` field, e.g.
```

### Comparing `pulumi_vault-6.2.0a1713339773/pulumi_vault/identity/mfa_pingid.py` & `pulumi_vault-6.2.0a1713561465/pulumi_vault/identity/mfa_pingid.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1713339773/pulumi_vault/identity/mfa_totp.py` & `pulumi_vault-6.2.0a1713561465/pulumi_vault/identity/mfa_totp.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1713339773/pulumi_vault/identity/oidc.py` & `pulumi_vault-6.2.0a1713561465/pulumi_vault/identity/oidc.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1713339773/pulumi_vault/identity/oidc_assignment.py` & `pulumi_vault-6.2.0a1713561465/pulumi_vault/identity/oidc_assignment.py`

 * *Files 2% similar despite different names*

```diff
@@ -185,21 +185,25 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_vault as vault
 
         internal = vault.identity.Group("internal",
+            name="internal",
             type="internal",
             policies=[
                 "dev",
                 "test",
             ])
-        test = vault.identity.Entity("test", policies=["test"])
+        test = vault.identity.Entity("test",
+            name="test",
+            policies=["test"])
         default = vault.identity.OidcAssignment("default",
+            name="assignment",
             entity_ids=[test.id],
             group_ids=[internal.id])
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
 
@@ -233,21 +237,25 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_vault as vault
 
         internal = vault.identity.Group("internal",
+            name="internal",
             type="internal",
             policies=[
                 "dev",
                 "test",
             ])
-        test = vault.identity.Entity("test", policies=["test"])
+        test = vault.identity.Entity("test",
+            name="test",
+            policies=["test"])
         default = vault.identity.OidcAssignment("default",
+            name="assignment",
             entity_ids=[test.id],
             group_ids=[internal.id])
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
```

### Comparing `pulumi_vault-6.2.0a1713339773/pulumi_vault/identity/oidc_client.py` & `pulumi_vault-6.2.0a1713561465/pulumi_vault/identity/oidc_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -374,24 +374,26 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_vault as vault
 
-        test_oidc_assignment = vault.identity.OidcAssignment("testOidcAssignment",
+        test = vault.identity.OidcAssignment("test",
+            name="my-assignment",
             entity_ids=["ascbascas-2231a-sdfaa"],
             group_ids=["sajkdsad-32414-sfsada"])
-        test_oidc_client = vault.identity.OidcClient("testOidcClient",
+        test_oidc_client = vault.identity.OidcClient("test",
+            name="my-app",
             redirect_uris=[
                 "http://127.0.0.1:9200/v1/auth-methods/oidc:authenticate:callback",
                 "http://127.0.0.1:8251/callback",
                 "http://127.0.0.1:8080/callback",
             ],
-            assignments=[test_oidc_assignment.name],
+            assignments=[test.name],
             id_token_ttl=2400,
             access_token_ttl=7200)
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
 
@@ -434,24 +436,26 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_vault as vault
 
-        test_oidc_assignment = vault.identity.OidcAssignment("testOidcAssignment",
+        test = vault.identity.OidcAssignment("test",
+            name="my-assignment",
             entity_ids=["ascbascas-2231a-sdfaa"],
             group_ids=["sajkdsad-32414-sfsada"])
-        test_oidc_client = vault.identity.OidcClient("testOidcClient",
+        test_oidc_client = vault.identity.OidcClient("test",
+            name="my-app",
             redirect_uris=[
                 "http://127.0.0.1:9200/v1/auth-methods/oidc:authenticate:callback",
                 "http://127.0.0.1:8251/callback",
                 "http://127.0.0.1:8080/callback",
             ],
-            assignments=[test_oidc_assignment.name],
+            assignments=[test.name],
             id_token_ttl=2400,
             access_token_ttl=7200)
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
```

### Comparing `pulumi_vault-6.2.0a1713339773/pulumi_vault/identity/oidc_key.py` & `pulumi_vault-6.2.0a1713561465/pulumi_vault/identity/oidc_key.py`

 * *Files 2% similar despite different names*

```diff
@@ -259,19 +259,23 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_vault as vault
 
-        key = vault.identity.OidcKey("key", algorithm="RS256")
-        role_oidc_role = vault.identity.OidcRole("roleOidcRole", key=key.name)
-        role_oidc_key_allowed_client_id = vault.identity.OidcKeyAllowedClientID("roleOidcKeyAllowedClientID",
+        key = vault.identity.OidcKey("key",
+            name="key",
+            algorithm="RS256")
+        role = vault.identity.OidcRole("role",
+            name="role",
+            key=key.name)
+        role_oidc_key_allowed_client_id = vault.identity.OidcKeyAllowedClientID("role",
             key_name=key.name,
-            allowed_client_id=role_oidc_role.client_id)
+            allowed_client_id=role.client_id)
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
 
         The key can be imported with the key name, for example:
 
@@ -304,19 +308,23 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_vault as vault
 
-        key = vault.identity.OidcKey("key", algorithm="RS256")
-        role_oidc_role = vault.identity.OidcRole("roleOidcRole", key=key.name)
-        role_oidc_key_allowed_client_id = vault.identity.OidcKeyAllowedClientID("roleOidcKeyAllowedClientID",
+        key = vault.identity.OidcKey("key",
+            name="key",
+            algorithm="RS256")
+        role = vault.identity.OidcRole("role",
+            name="role",
+            key=key.name)
+        role_oidc_key_allowed_client_id = vault.identity.OidcKeyAllowedClientID("role",
             key_name=key.name,
-            allowed_client_id=role_oidc_role.client_id)
+            allowed_client_id=role.client_id)
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
 
         The key can be imported with the key name, for example:
```

### Comparing `pulumi_vault-6.2.0a1713339773/pulumi_vault/identity/oidc_key_allowed_client_id.py` & `pulumi_vault-6.2.0a1713561465/pulumi_vault/identity/oidc_key_allowed_client_id.py`

 * *Files 5% similar despite different names*

```diff
@@ -146,19 +146,23 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_vault as vault
 
-        key = vault.identity.OidcKey("key", algorithm="RS256")
-        role_oidc_role = vault.identity.OidcRole("roleOidcRole", key=key.name)
-        role_oidc_key_allowed_client_id = vault.identity.OidcKeyAllowedClientID("roleOidcKeyAllowedClientID",
+        key = vault.identity.OidcKey("key",
+            name="key",
+            algorithm="RS256")
+        role = vault.identity.OidcRole("role",
+            name="role",
+            key=key.name)
+        role_oidc_key_allowed_client_id = vault.identity.OidcKeyAllowedClientID("role",
             key_name=key.name,
-            allowed_client_id=role_oidc_role.client_id)
+            allowed_client_id=role.client_id)
         ```
         <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] allowed_client_id: Client ID to allow usage with the OIDC named key
         :param pulumi.Input[str] key_name: Name of the OIDC Key allow the Client ID.
@@ -177,19 +181,23 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_vault as vault
 
-        key = vault.identity.OidcKey("key", algorithm="RS256")
-        role_oidc_role = vault.identity.OidcRole("roleOidcRole", key=key.name)
-        role_oidc_key_allowed_client_id = vault.identity.OidcKeyAllowedClientID("roleOidcKeyAllowedClientID",
+        key = vault.identity.OidcKey("key",
+            name="key",
+            algorithm="RS256")
+        role = vault.identity.OidcRole("role",
+            name="role",
+            key=key.name)
+        role_oidc_key_allowed_client_id = vault.identity.OidcKeyAllowedClientID("role",
             key_name=key.name,
-            allowed_client_id=role_oidc_role.client_id)
+            allowed_client_id=role.client_id)
         ```
         <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param OidcKeyAllowedClientIDArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
```

### Comparing `pulumi_vault-6.2.0a1713339773/pulumi_vault/identity/oidc_provider.py` & `pulumi_vault-6.2.0a1713561465/pulumi_vault/identity/oidc_provider.py`

 * *Files 1% similar despite different names*

```diff
@@ -275,37 +275,42 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import json
         import pulumi_vault as vault
 
-        test_oidc_key = vault.identity.OidcKey("testOidcKey",
+        test = vault.identity.OidcKey("test",
+            name="my-key",
             allowed_client_ids=["*"],
             rotation_period=3600,
             verification_ttl=3600)
-        test_oidc_assignment = vault.identity.OidcAssignment("testOidcAssignment",
+        test_oidc_assignment = vault.identity.OidcAssignment("test",
+            name="my-assignment",
             entity_ids=["fake-ascbascas-2231a-sdfaa"],
             group_ids=["fake-sajkdsad-32414-sfsada"])
-        test_oidc_client = vault.identity.OidcClient("testOidcClient",
-            key=test_oidc_key.name,
+        test_oidc_client = vault.identity.OidcClient("test",
+            name="application",
+            key=test.name,
             redirect_uris=[
                 "http://127.0.0.1:9200/v1/auth-methods/oidc:authenticate:callback",
                 "http://127.0.0.1:8251/callback",
                 "http://127.0.0.1:8080/callback",
             ],
             assignments=[test_oidc_assignment.name],
             id_token_ttl=2400,
             access_token_ttl=7200)
-        test_oidc_scope = vault.identity.OidcScope("testOidcScope",
+        test_oidc_scope = vault.identity.OidcScope("test",
+            name="groups",
             template=json.dumps({
                 "groups": "{{identity.entity.groups.names}}",
             }),
             description="Groups scope.")
-        test_oidc_provider = vault.identity.OidcProvider("testOidcProvider",
+        test_oidc_provider = vault.identity.OidcProvider("test",
+            name="my-provider",
             https_enabled=False,
             issuer_host="127.0.0.1:8200",
             allowed_client_ids=[test_oidc_client.client_id],
             scopes_supporteds=[test_oidc_scope.name])
         ```
         <!--End PulumiCodeChooser -->
 
@@ -344,37 +349,42 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import json
         import pulumi_vault as vault
 
-        test_oidc_key = vault.identity.OidcKey("testOidcKey",
+        test = vault.identity.OidcKey("test",
+            name="my-key",
             allowed_client_ids=["*"],
             rotation_period=3600,
             verification_ttl=3600)
-        test_oidc_assignment = vault.identity.OidcAssignment("testOidcAssignment",
+        test_oidc_assignment = vault.identity.OidcAssignment("test",
+            name="my-assignment",
             entity_ids=["fake-ascbascas-2231a-sdfaa"],
             group_ids=["fake-sajkdsad-32414-sfsada"])
-        test_oidc_client = vault.identity.OidcClient("testOidcClient",
-            key=test_oidc_key.name,
+        test_oidc_client = vault.identity.OidcClient("test",
+            name="application",
+            key=test.name,
             redirect_uris=[
                 "http://127.0.0.1:9200/v1/auth-methods/oidc:authenticate:callback",
                 "http://127.0.0.1:8251/callback",
                 "http://127.0.0.1:8080/callback",
             ],
             assignments=[test_oidc_assignment.name],
             id_token_ttl=2400,
             access_token_ttl=7200)
-        test_oidc_scope = vault.identity.OidcScope("testOidcScope",
+        test_oidc_scope = vault.identity.OidcScope("test",
+            name="groups",
             template=json.dumps({
                 "groups": "{{identity.entity.groups.names}}",
             }),
             description="Groups scope.")
-        test_oidc_provider = vault.identity.OidcProvider("testOidcProvider",
+        test_oidc_provider = vault.identity.OidcProvider("test",
+            name="my-provider",
             https_enabled=False,
             issuer_host="127.0.0.1:8200",
             allowed_client_ids=[test_oidc_client.client_id],
             scopes_supporteds=[test_oidc_scope.name])
         ```
         <!--End PulumiCodeChooser -->
```

### Comparing `pulumi_vault-6.2.0a1713339773/pulumi_vault/identity/oidc_role.py` & `pulumi_vault-6.2.0a1713561465/pulumi_vault/identity/oidc_role.py`

 * *Files 5% similar despite different names*

```diff
@@ -272,38 +272,46 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_vault as vault
 
         config = pulumi.Config()
+        # Name of the OIDC Key
         key = config.get("key")
         if key is None:
             key = "key"
-        role = vault.identity.OidcRole("role", key=key)
-        key_oidc_key = vault.identity.OidcKey("keyOidcKey",
+        role = vault.identity.OidcRole("role",
+            name="role",
+            key=key)
+        key_oidc_key = vault.identity.OidcKey("key",
+            name=key,
             algorithm="RS256",
             allowed_client_ids=[role.client_id])
         ```
         <!--End PulumiCodeChooser -->
 
         If you want to create the key first before creating the role, you can use a separate
         resource to configure the allowed Client ID on
         the key.
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_vault as vault
 
-        key = vault.identity.OidcKey("key", algorithm="RS256")
-        role_oidc_role = vault.identity.OidcRole("roleOidcRole", key=key.name)
-        role_oidc_key_allowed_client_id = vault.identity.OidcKeyAllowedClientID("roleOidcKeyAllowedClientID",
+        key = vault.identity.OidcKey("key",
+            name="key",
+            algorithm="RS256")
+        role = vault.identity.OidcRole("role",
+            name="role",
+            key=key.name)
+        role_oidc_key_allowed_client_id = vault.identity.OidcKeyAllowedClientID("role",
             key_name=key.name,
-            allowed_client_id=role_oidc_role.client_id)
+            allowed_client_id=role.client_id)
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
 
         The key can be imported with the role name, for example:
 
@@ -344,38 +352,46 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_vault as vault
 
         config = pulumi.Config()
+        # Name of the OIDC Key
         key = config.get("key")
         if key is None:
             key = "key"
-        role = vault.identity.OidcRole("role", key=key)
-        key_oidc_key = vault.identity.OidcKey("keyOidcKey",
+        role = vault.identity.OidcRole("role",
+            name="role",
+            key=key)
+        key_oidc_key = vault.identity.OidcKey("key",
+            name=key,
             algorithm="RS256",
             allowed_client_ids=[role.client_id])
         ```
         <!--End PulumiCodeChooser -->
 
         If you want to create the key first before creating the role, you can use a separate
         resource to configure the allowed Client ID on
         the key.
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_vault as vault
 
-        key = vault.identity.OidcKey("key", algorithm="RS256")
-        role_oidc_role = vault.identity.OidcRole("roleOidcRole", key=key.name)
-        role_oidc_key_allowed_client_id = vault.identity.OidcKeyAllowedClientID("roleOidcKeyAllowedClientID",
+        key = vault.identity.OidcKey("key",
+            name="key",
+            algorithm="RS256")
+        role = vault.identity.OidcRole("role",
+            name="role",
+            key=key.name)
+        role_oidc_key_allowed_client_id = vault.identity.OidcKeyAllowedClientID("role",
             key_name=key.name,
-            allowed_client_id=role_oidc_role.client_id)
+            allowed_client_id=role.client_id)
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
 
         The key can be imported with the role name, for example:
```

### Comparing `pulumi_vault-6.2.0a1713339773/pulumi_vault/identity/oidc_scope.py` & `pulumi_vault-6.2.0a1713561465/pulumi_vault/identity/oidc_scope.py`

 * *Files 1% similar despite different names*

```diff
@@ -185,16 +185,17 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_vault as vault
 
         groups = vault.identity.OidcScope("groups",
-            description="Vault OIDC Groups Scope",
-            template="{\\"groups\\":{{identity.entity.groups.names}}}")
+            name="groups",
+            template="{\\"groups\\":{{identity.entity.groups.names}}}",
+            description="Vault OIDC Groups Scope")
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
 
         OIDC Scopes can be imported using the `name`, e.g.
 
@@ -226,16 +227,17 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_vault as vault
 
         groups = vault.identity.OidcScope("groups",
-            description="Vault OIDC Groups Scope",
-            template="{\\"groups\\":{{identity.entity.groups.names}}}")
+            name="groups",
+            template="{\\"groups\\":{{identity.entity.groups.names}}}",
+            description="Vault OIDC Groups Scope")
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
 
         OIDC Scopes can be imported using the `name`, e.g.
```

### Comparing `pulumi_vault-6.2.0a1713339773/pulumi_vault/identity/outputs.py` & `pulumi_vault-6.2.0a1713561465/pulumi_vault/identity/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1713339773/pulumi_vault/jwt/_inputs.py` & `pulumi_vault-6.2.0a1713561465/pulumi_vault/jwt/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1713339773/pulumi_vault/jwt/auth_backend.py` & `pulumi_vault-6.2.0a1713561465/pulumi_vault/jwt/auth_backend.py`

 * *Files 1% similar despite different names*

```diff
@@ -778,60 +778,60 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_vault as vault
 
         example = vault.jwt.AuthBackend("example",
-            bound_issuer="https://myco.auth0.com/",
             description="Demonstration of the Terraform JWT auth backend",
+            path="jwt",
             oidc_discovery_url="https://myco.auth0.com/",
-            path="jwt")
+            bound_issuer="https://myco.auth0.com/")
         ```
         <!--End PulumiCodeChooser -->
 
         Manage OIDC auth backend:
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_vault as vault
 
         example = vault.jwt.AuthBackend("example",
-            bound_issuer="https://myco.auth0.com/",
             description="Demonstration of the Terraform JWT auth backend",
+            path="oidc",
+            type="oidc",
+            oidc_discovery_url="https://myco.auth0.com/",
             oidc_client_id="1234567890",
             oidc_client_secret="secret123456",
-            oidc_discovery_url="https://myco.auth0.com/",
-            path="oidc",
+            bound_issuer="https://myco.auth0.com/",
             tune=vault.jwt.AuthBackendTuneArgs(
                 listing_visibility="unauth",
-            ),
-            type="oidc")
+            ))
         ```
         <!--End PulumiCodeChooser -->
 
         Configuring the auth backend with a `provider_config:
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_vault as vault
 
         gsuite = vault.jwt.AuthBackend("gsuite",
             description="OIDC backend",
             oidc_discovery_url="https://accounts.google.com",
             path="oidc",
+            type="oidc",
             provider_config={
+                "provider": "gsuite",
                 "fetch_groups": "true",
                 "fetch_user_info": "true",
                 "groups_recurse_max_depth": "1",
-                "provider": "gsuite",
-            },
-            type="oidc")
+            })
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
 
         JWT auth backend can be imported using the `path`, e.g.
 
@@ -891,60 +891,60 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_vault as vault
 
         example = vault.jwt.AuthBackend("example",
-            bound_issuer="https://myco.auth0.com/",
             description="Demonstration of the Terraform JWT auth backend",
+            path="jwt",
             oidc_discovery_url="https://myco.auth0.com/",
-            path="jwt")
+            bound_issuer="https://myco.auth0.com/")
         ```
         <!--End PulumiCodeChooser -->
 
         Manage OIDC auth backend:
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_vault as vault
 
         example = vault.jwt.AuthBackend("example",
-            bound_issuer="https://myco.auth0.com/",
             description="Demonstration of the Terraform JWT auth backend",
+            path="oidc",
+            type="oidc",
+            oidc_discovery_url="https://myco.auth0.com/",
             oidc_client_id="1234567890",
             oidc_client_secret="secret123456",
-            oidc_discovery_url="https://myco.auth0.com/",
-            path="oidc",
+            bound_issuer="https://myco.auth0.com/",
             tune=vault.jwt.AuthBackendTuneArgs(
                 listing_visibility="unauth",
-            ),
-            type="oidc")
+            ))
         ```
         <!--End PulumiCodeChooser -->
 
         Configuring the auth backend with a `provider_config:
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_vault as vault
 
         gsuite = vault.jwt.AuthBackend("gsuite",
             description="OIDC backend",
             oidc_discovery_url="https://accounts.google.com",
             path="oidc",
+            type="oidc",
             provider_config={
+                "provider": "gsuite",
                 "fetch_groups": "true",
                 "fetch_user_info": "true",
                 "groups_recurse_max_depth": "1",
-                "provider": "gsuite",
-            },
-            type="oidc")
+            })
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
 
         JWT auth backend can be imported using the `path`, e.g.
```

### Comparing `pulumi_vault-6.2.0a1713339773/pulumi_vault/jwt/auth_backend_role.py` & `pulumi_vault-6.2.0a1713561465/pulumi_vault/jwt/auth_backend_role.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1713339773/pulumi_vault/jwt/outputs.py` & `pulumi_vault-6.2.0a1713561465/pulumi_vault/jwt/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1713339773/pulumi_vault/kmip/secret_backend.py` & `pulumi_vault-6.2.0a1713561465/pulumi_vault/kmip/secret_backend.py`

 * *Files 0% similar despite different names*

```diff
@@ -490,25 +490,25 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_vault as vault
 
         default = vault.kmip.SecretBackend("default",
-            default_tls_client_key_bits=4096,
-            default_tls_client_key_type="rsa",
-            default_tls_client_ttl=86400,
+            path="kmip",
             description="Vault KMIP backend",
             listen_addrs=[
                 "127.0.0.1:5696",
                 "127.0.0.1:8080",
             ],
-            path="kmip",
+            tls_ca_key_type="rsa",
             tls_ca_key_bits=4096,
-            tls_ca_key_type="rsa")
+            default_tls_client_key_type="rsa",
+            default_tls_client_key_bits=4096,
+            default_tls_client_ttl=86400)
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
 
         KMIP Secret backend can be imported using the `path`, e.g.
 
@@ -552,25 +552,25 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_vault as vault
 
         default = vault.kmip.SecretBackend("default",
-            default_tls_client_key_bits=4096,
-            default_tls_client_key_type="rsa",
-            default_tls_client_ttl=86400,
+            path="kmip",
             description="Vault KMIP backend",
             listen_addrs=[
                 "127.0.0.1:5696",
                 "127.0.0.1:8080",
             ],
-            path="kmip",
+            tls_ca_key_type="rsa",
             tls_ca_key_bits=4096,
-            tls_ca_key_type="rsa")
+            default_tls_client_key_type="rsa",
+            default_tls_client_key_bits=4096,
+            default_tls_client_ttl=86400)
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
 
         KMIP Secret backend can be imported using the `path`, e.g.
```

### Comparing `pulumi_vault-6.2.0a1713339773/pulumi_vault/kmip/secret_role.py` & `pulumi_vault-6.2.0a1713561465/pulumi_vault/kmip/secret_role.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1713339773/pulumi_vault/kmip/secret_scope.py` & `pulumi_vault-6.2.0a1713561465/pulumi_vault/kmip/secret_scope.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1713339773/pulumi_vault/kubernetes/__init__.py` & `pulumi_vault-6.2.0a1713561465/pulumi_vault/kubernetes/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1713339773/pulumi_vault/kubernetes/auth_backend_config.py` & `pulumi_vault-6.2.0a1713561465/pulumi_vault/kubernetes/auth_backend_config.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1713339773/pulumi_vault/kubernetes/auth_backend_role.py` & `pulumi_vault-6.2.0a1713561465/pulumi_vault/kubernetes/auth_backend_role.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1713339773/pulumi_vault/kubernetes/get_auth_backend_config.py` & `pulumi_vault-6.2.0a1713561465/pulumi_vault/kubernetes/get_auth_backend_config.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1713339773/pulumi_vault/kubernetes/get_auth_backend_role.py` & `pulumi_vault-6.2.0a1713561465/pulumi_vault/kubernetes/get_auth_backend_role.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1713339773/pulumi_vault/kubernetes/get_service_account_token.py` & `pulumi_vault-6.2.0a1713561465/pulumi_vault/kubernetes/get_service_account_token.py`

 * *Files 4% similar despite different names*

```diff
@@ -179,25 +179,27 @@
                               opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetServiceAccountTokenResult:
     """
     ## Example Usage
 
     <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
+    import pulumi_std as std
     import pulumi_vault as vault
 
     config = vault.kubernetes.SecretBackend("config",
         path="kubernetes",
         description="kubernetes secrets engine description",
         kubernetes_host="https://127.0.0.1:61233",
-        kubernetes_ca_cert=(lambda path: open(path).read())("/path/to/cert"),
-        service_account_jwt=(lambda path: open(path).read())("/path/to/token"),
+        kubernetes_ca_cert=std.file(input="/path/to/cert").result,
+        service_account_jwt=std.file(input="/path/to/token").result,
         disable_local_ca_jwt=False)
     role = vault.kubernetes.SecretBackendRole("role",
         backend=config.path,
+        name="service-account-name-role",
         allowed_kubernetes_namespaces=["*"],
         token_max_ttl=43200,
         token_default_ttl=21600,
         service_account_name="test-service-account-with-generated-token",
         extra_labels={
             "id": "abc123",
             "name": "some_name",
@@ -266,25 +268,27 @@
                                      opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetServiceAccountTokenResult]:
     """
     ## Example Usage
 
     <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
+    import pulumi_std as std
     import pulumi_vault as vault
 
     config = vault.kubernetes.SecretBackend("config",
         path="kubernetes",
         description="kubernetes secrets engine description",
         kubernetes_host="https://127.0.0.1:61233",
-        kubernetes_ca_cert=(lambda path: open(path).read())("/path/to/cert"),
-        service_account_jwt=(lambda path: open(path).read())("/path/to/token"),
+        kubernetes_ca_cert=std.file(input="/path/to/cert").result,
+        service_account_jwt=std.file(input="/path/to/token").result,
         disable_local_ca_jwt=False)
     role = vault.kubernetes.SecretBackendRole("role",
         backend=config.path,
+        name="service-account-name-role",
         allowed_kubernetes_namespaces=["*"],
         token_max_ttl=43200,
         token_default_ttl=21600,
         service_account_name="test-service-account-with-generated-token",
         extra_labels={
             "id": "abc123",
             "name": "some_name",
```

### Comparing `pulumi_vault-6.2.0a1713339773/pulumi_vault/kubernetes/secret_backend.py` & `pulumi_vault-6.2.0a1713561465/pulumi_vault/kubernetes/secret_backend.py`

 * *Files 1% similar despite different names*

```diff
@@ -622,24 +622,25 @@
                  __props__=None):
         """
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
+        import pulumi_std as std
         import pulumi_vault as vault
 
         config = vault.kubernetes.SecretBackend("config",
             path="kubernetes",
             description="kubernetes secrets engine description",
             default_lease_ttl_seconds=43200,
             max_lease_ttl_seconds=86400,
             kubernetes_host="https://127.0.0.1:61233",
-            kubernetes_ca_cert=(lambda path: open(path).read())("/path/to/cert"),
-            service_account_jwt=(lambda path: open(path).read())("/path/to/token"),
+            kubernetes_ca_cert=std.file(input="/path/to/cert").result,
+            service_account_jwt=std.file(input="/path/to/token").result,
             disable_local_ca_jwt=False)
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
 
         The Kubernetes secret backend can be imported using its `path` e.g.
@@ -686,24 +687,25 @@
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
+        import pulumi_std as std
         import pulumi_vault as vault
 
         config = vault.kubernetes.SecretBackend("config",
             path="kubernetes",
             description="kubernetes secrets engine description",
             default_lease_ttl_seconds=43200,
             max_lease_ttl_seconds=86400,
             kubernetes_host="https://127.0.0.1:61233",
-            kubernetes_ca_cert=(lambda path: open(path).read())("/path/to/cert"),
-            service_account_jwt=(lambda path: open(path).read())("/path/to/token"),
+            kubernetes_ca_cert=std.file(input="/path/to/cert").result,
+            service_account_jwt=std.file(input="/path/to/token").result,
             disable_local_ca_jwt=False)
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
 
         The Kubernetes secret backend can be imported using its `path` e.g.
```

### Comparing `pulumi_vault-6.2.0a1713339773/pulumi_vault/kubernetes/secret_backend_role.py` & `pulumi_vault-6.2.0a1713561465/pulumi_vault/kubernetes/secret_backend_role.py`

 * *Files 2% similar despite different names*

```diff
@@ -590,25 +590,27 @@
         ## Example Usage
 
         Example using `service_account_name` mode:
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
+        import pulumi_std as std
         import pulumi_vault as vault
 
         config = vault.kubernetes.SecretBackend("config",
             path="kubernetes",
             description="kubernetes secrets engine description",
             kubernetes_host="https://127.0.0.1:61233",
-            kubernetes_ca_cert=(lambda path: open(path).read())("/path/to/cert"),
-            service_account_jwt=(lambda path: open(path).read())("/path/to/token"),
+            kubernetes_ca_cert=std.file(input="/path/to/cert").result,
+            service_account_jwt=std.file(input="/path/to/token").result,
             disable_local_ca_jwt=False)
         sa_example = vault.kubernetes.SecretBackendRole("sa-example",
             backend=config.path,
+            name="service-account-name-role",
             allowed_kubernetes_namespaces=["*"],
             token_max_ttl=43200,
             token_default_ttl=21600,
             service_account_name="test-service-account-with-generated-token",
             extra_labels={
                 "id": "abc123",
                 "name": "some_name",
@@ -621,25 +623,27 @@
         <!--End PulumiCodeChooser -->
 
         Example using `kubernetes_role_name` mode:
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
+        import pulumi_std as std
         import pulumi_vault as vault
 
         config = vault.kubernetes.SecretBackend("config",
             path="kubernetes",
             description="kubernetes secrets engine description",
             kubernetes_host="https://127.0.0.1:61233",
-            kubernetes_ca_cert=(lambda path: open(path).read())("/path/to/cert"),
-            service_account_jwt=(lambda path: open(path).read())("/path/to/token"),
+            kubernetes_ca_cert=std.file(input="/path/to/cert").result,
+            service_account_jwt=std.file(input="/path/to/token").result,
             disable_local_ca_jwt=False)
         name_example = vault.kubernetes.SecretBackendRole("name-example",
             backend=config.path,
+            name="service-account-name-role",
             allowed_kubernetes_namespaces=["*"],
             token_max_ttl=43200,
             token_default_ttl=21600,
             kubernetes_role_name="vault-k8s-secrets-role",
             extra_labels={
                 "id": "abc123",
                 "name": "some_name",
@@ -652,25 +656,27 @@
         <!--End PulumiCodeChooser -->
 
         Example using `generated_role_rules` mode:
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
+        import pulumi_std as std
         import pulumi_vault as vault
 
         config = vault.kubernetes.SecretBackend("config",
             path="kubernetes",
             description="kubernetes secrets engine description",
             kubernetes_host="https://127.0.0.1:61233",
-            kubernetes_ca_cert=(lambda path: open(path).read())("/path/to/cert"),
-            service_account_jwt=(lambda path: open(path).read())("/path/to/token"),
+            kubernetes_ca_cert=std.file(input="/path/to/cert").result,
+            service_account_jwt=std.file(input="/path/to/token").result,
             disable_local_ca_jwt=False)
         rules_example = vault.kubernetes.SecretBackendRole("rules-example",
             backend=config.path,
+            name="service-account-name-role",
             allowed_kubernetes_namespaces=["*"],
             token_max_ttl=43200,
             token_default_ttl=21600,
             kubernetes_role_type="Role",
             generated_role_rules=\"\"\"rules:
         - apiGroups: [""]
           resources: ["pods"]
@@ -747,25 +753,27 @@
         ## Example Usage
 
         Example using `service_account_name` mode:
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
+        import pulumi_std as std
         import pulumi_vault as vault
 
         config = vault.kubernetes.SecretBackend("config",
             path="kubernetes",
             description="kubernetes secrets engine description",
             kubernetes_host="https://127.0.0.1:61233",
-            kubernetes_ca_cert=(lambda path: open(path).read())("/path/to/cert"),
-            service_account_jwt=(lambda path: open(path).read())("/path/to/token"),
+            kubernetes_ca_cert=std.file(input="/path/to/cert").result,
+            service_account_jwt=std.file(input="/path/to/token").result,
             disable_local_ca_jwt=False)
         sa_example = vault.kubernetes.SecretBackendRole("sa-example",
             backend=config.path,
+            name="service-account-name-role",
             allowed_kubernetes_namespaces=["*"],
             token_max_ttl=43200,
             token_default_ttl=21600,
             service_account_name="test-service-account-with-generated-token",
             extra_labels={
                 "id": "abc123",
                 "name": "some_name",
@@ -778,25 +786,27 @@
         <!--End PulumiCodeChooser -->
 
         Example using `kubernetes_role_name` mode:
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
+        import pulumi_std as std
         import pulumi_vault as vault
 
         config = vault.kubernetes.SecretBackend("config",
             path="kubernetes",
             description="kubernetes secrets engine description",
             kubernetes_host="https://127.0.0.1:61233",
-            kubernetes_ca_cert=(lambda path: open(path).read())("/path/to/cert"),
-            service_account_jwt=(lambda path: open(path).read())("/path/to/token"),
+            kubernetes_ca_cert=std.file(input="/path/to/cert").result,
+            service_account_jwt=std.file(input="/path/to/token").result,
             disable_local_ca_jwt=False)
         name_example = vault.kubernetes.SecretBackendRole("name-example",
             backend=config.path,
+            name="service-account-name-role",
             allowed_kubernetes_namespaces=["*"],
             token_max_ttl=43200,
             token_default_ttl=21600,
             kubernetes_role_name="vault-k8s-secrets-role",
             extra_labels={
                 "id": "abc123",
                 "name": "some_name",
@@ -809,25 +819,27 @@
         <!--End PulumiCodeChooser -->
 
         Example using `generated_role_rules` mode:
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
+        import pulumi_std as std
         import pulumi_vault as vault
 
         config = vault.kubernetes.SecretBackend("config",
             path="kubernetes",
             description="kubernetes secrets engine description",
             kubernetes_host="https://127.0.0.1:61233",
-            kubernetes_ca_cert=(lambda path: open(path).read())("/path/to/cert"),
-            service_account_jwt=(lambda path: open(path).read())("/path/to/token"),
+            kubernetes_ca_cert=std.file(input="/path/to/cert").result,
+            service_account_jwt=std.file(input="/path/to/token").result,
             disable_local_ca_jwt=False)
         rules_example = vault.kubernetes.SecretBackendRole("rules-example",
             backend=config.path,
+            name="service-account-name-role",
             allowed_kubernetes_namespaces=["*"],
             token_max_ttl=43200,
             token_default_ttl=21600,
             kubernetes_role_type="Role",
             generated_role_rules=\"\"\"rules:
         - apiGroups: [""]
           resources: ["pods"]
```

### Comparing `pulumi_vault-6.2.0a1713339773/pulumi_vault/kv/__init__.py` & `pulumi_vault-6.2.0a1713561465/pulumi_vault/kv/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1713339773/pulumi_vault/kv/_inputs.py` & `pulumi_vault-6.2.0a1713561465/pulumi_vault/kv/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1713339773/pulumi_vault/kv/get_secret.py` & `pulumi_vault-6.2.0a1713561465/pulumi_vault/kv/get_secret.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1713339773/pulumi_vault/kv/get_secret_subkeys_v2.py` & `pulumi_vault-6.2.0a1713561465/pulumi_vault/kv/get_secret_subkeys_v2.py`

 * *Files 1% similar despite different names*

```diff
@@ -143,16 +143,17 @@
     kvv2 = vault.Mount("kvv2",
         path="kvv2",
         type="kv",
         options={
             "version": "2",
         },
         description="KV Version 2 secret engine mount")
-    aws_secret = vault.kv.SecretV2("awsSecret",
+    aws_secret = vault.kv.SecretV2("aws_secret",
         mount=kvv2.path,
+        name="aws_secret",
         data_json=json.dumps({
             "zip": "zap",
             "foo": "bar",
         }))
     test = vault.kv.get_secret_subkeys_v2_output(mount=kvv2.path,
         name=aws_secret.name)
     ```
@@ -219,16 +220,17 @@
     kvv2 = vault.Mount("kvv2",
         path="kvv2",
         type="kv",
         options={
             "version": "2",
         },
         description="KV Version 2 secret engine mount")
-    aws_secret = vault.kv.SecretV2("awsSecret",
+    aws_secret = vault.kv.SecretV2("aws_secret",
         mount=kvv2.path,
+        name="aws_secret",
         data_json=json.dumps({
             "zip": "zap",
             "foo": "bar",
         }))
     test = vault.kv.get_secret_subkeys_v2_output(mount=kvv2.path,
         name=aws_secret.name)
     ```
```

### Comparing `pulumi_vault-6.2.0a1713339773/pulumi_vault/kv/get_secret_v2.py` & `pulumi_vault-6.2.0a1713561465/pulumi_vault/kv/get_secret_v2.py`

 * *Files 7% similar despite different names*

```diff
@@ -175,14 +175,45 @@
                   name: Optional[str] = None,
                   namespace: Optional[str] = None,
                   version: Optional[int] = None,
                   opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetSecretV2Result:
     """
     ## Example Usage
 
+    <!--Start PulumiCodeChooser -->
+    ```python
+    import pulumi
+    import json
+    import pulumi_vault as vault
+
+    kvv2 = vault.Mount("kvv2",
+        path="kvv2",
+        type="kv",
+        options={
+            "version": "2",
+        },
+        description="KV Version 2 secret engine mount")
+    example_secret_v2 = vault.kv.SecretV2("example",
+        mount=kvv2.path,
+        name="secret",
+        cas=1,
+        delete_all_versions=True,
+        data_json=json.dumps({
+            "zip": "zap",
+            "foo": "bar",
+        }))
+    example = vault.kv.get_secret_v2_output(mount=kvv2.path,
+        name=example_secret_v2.name)
+    ```
+    <!--End PulumiCodeChooser -->
+
+    ## Required Vault Capabilities
+
+    Use of this resource requires the `read` capability on the given path.
+
 
     :param str mount: Path where KV-V2 engine is mounted.
     :param str name: Full name of the secret. For a nested secret
            the name is the nested path excluding the mount and data
            prefix. For example, for a secret at `kvv2/data/foo/bar/baz`
            the name is `foo/bar/baz`.
     :param str namespace: The namespace of the target resource.
@@ -219,14 +250,45 @@
                          name: Optional[pulumi.Input[str]] = None,
                          namespace: Optional[pulumi.Input[Optional[str]]] = None,
                          version: Optional[pulumi.Input[Optional[int]]] = None,
                          opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetSecretV2Result]:
     """
     ## Example Usage
 
+    <!--Start PulumiCodeChooser -->
+    ```python
+    import pulumi
+    import json
+    import pulumi_vault as vault
+
+    kvv2 = vault.Mount("kvv2",
+        path="kvv2",
+        type="kv",
+        options={
+            "version": "2",
+        },
+        description="KV Version 2 secret engine mount")
+    example_secret_v2 = vault.kv.SecretV2("example",
+        mount=kvv2.path,
+        name="secret",
+        cas=1,
+        delete_all_versions=True,
+        data_json=json.dumps({
+            "zip": "zap",
+            "foo": "bar",
+        }))
+    example = vault.kv.get_secret_v2_output(mount=kvv2.path,
+        name=example_secret_v2.name)
+    ```
+    <!--End PulumiCodeChooser -->
+
+    ## Required Vault Capabilities
+
+    Use of this resource requires the `read` capability on the given path.
+
 
     :param str mount: Path where KV-V2 engine is mounted.
     :param str name: Full name of the secret. For a nested secret
            the name is the nested path excluding the mount and data
            prefix. For example, for a secret at `kvv2/data/foo/bar/baz`
            the name is `foo/bar/baz`.
     :param str namespace: The namespace of the target resource.
```

### Comparing `pulumi_vault-6.2.0a1713339773/pulumi_vault/kv/get_secrets_list.py` & `pulumi_vault-6.2.0a1713561465/pulumi_vault/kv/get_secrets_list.py`

 * *Files 2% similar despite different names*

```diff
@@ -89,20 +89,20 @@
     kvv1 = vault.Mount("kvv1",
         path="kvv1",
         type="kv",
         options={
             "version": "1",
         },
         description="KV Version 1 secret engine mount")
-    aws_secret = vault.kv.Secret("awsSecret",
+    aws_secret = vault.kv.Secret("aws_secret",
         path=kvv1.path.apply(lambda path: f"{path}/aws-secret"),
         data_json=json.dumps({
             "zip": "zap",
         }))
-    azure_secret = vault.kv.Secret("azureSecret",
+    azure_secret = vault.kv.Secret("azure_secret",
         path=kvv1.path.apply(lambda path: f"{path}/azure-secret"),
         data_json=json.dumps({
             "foo": "bar",
         }))
     secrets = vault.kv.get_secrets_list_output(path=kvv1.path)
     ```
     <!--End PulumiCodeChooser -->
@@ -147,20 +147,20 @@
     kvv1 = vault.Mount("kvv1",
         path="kvv1",
         type="kv",
         options={
             "version": "1",
         },
         description="KV Version 1 secret engine mount")
-    aws_secret = vault.kv.Secret("awsSecret",
+    aws_secret = vault.kv.Secret("aws_secret",
         path=kvv1.path.apply(lambda path: f"{path}/aws-secret"),
         data_json=json.dumps({
             "zip": "zap",
         }))
-    azure_secret = vault.kv.Secret("azureSecret",
+    azure_secret = vault.kv.Secret("azure_secret",
         path=kvv1.path.apply(lambda path: f"{path}/azure-secret"),
         data_json=json.dumps({
             "foo": "bar",
         }))
     secrets = vault.kv.get_secrets_list_output(path=kvv1.path)
     ```
     <!--End PulumiCodeChooser -->
```

### Comparing `pulumi_vault-6.2.0a1713339773/pulumi_vault/kv/get_secrets_list_v2.py` & `pulumi_vault-6.2.0a1713561465/pulumi_vault/kv/get_secrets_list_v2.py`

 * *Files 6% similar despite different names*

```diff
@@ -111,32 +111,35 @@
     kvv2 = vault.Mount("kvv2",
         path="kvv2",
         type="kv",
         options={
             "version": "2",
         },
         description="KV Version 2 secret engine mount")
-    aws_secret = vault.kv.SecretV2("awsSecret",
+    aws_secret = vault.kv.SecretV2("aws_secret",
         mount=kvv2.path,
+        name="aws_secret",
         data_json=json.dumps({
             "zip": "zap",
         }))
-    azure_secret = vault.kv.SecretV2("azureSecret",
+    azure_secret = vault.kv.SecretV2("azure_secret",
         mount=kvv2.path,
+        name="azure_secret",
         data_json=json.dumps({
             "foo": "bar",
         }))
-    nested_secret = vault.kv.SecretV2("nestedSecret",
+    nested_secret = vault.kv.SecretV2("nested_secret",
         mount=kvv2.path,
+        name=azure_secret.name.apply(lambda name: f"{name}/dev"),
         data_json=json.dumps({
             "password": "test",
         }))
     secrets = vault.kv.get_secrets_list_v2_output(mount=kvv2.path)
     nested_secrets = kvv2.path.apply(lambda path: vault.kv.get_secrets_list_v2_output(mount=path,
-        name=vault_kv_secret_v2["test_2"]["name"]))
+        name=test2["name"]))
     ```
     <!--End PulumiCodeChooser -->
 
     ## Required Vault Capabilities
 
     Use of this resource requires the `read` capability on the given path.
 
@@ -184,32 +187,35 @@
     kvv2 = vault.Mount("kvv2",
         path="kvv2",
         type="kv",
         options={
             "version": "2",
         },
         description="KV Version 2 secret engine mount")
-    aws_secret = vault.kv.SecretV2("awsSecret",
+    aws_secret = vault.kv.SecretV2("aws_secret",
         mount=kvv2.path,
+        name="aws_secret",
         data_json=json.dumps({
             "zip": "zap",
         }))
-    azure_secret = vault.kv.SecretV2("azureSecret",
+    azure_secret = vault.kv.SecretV2("azure_secret",
         mount=kvv2.path,
+        name="azure_secret",
         data_json=json.dumps({
             "foo": "bar",
         }))
-    nested_secret = vault.kv.SecretV2("nestedSecret",
+    nested_secret = vault.kv.SecretV2("nested_secret",
         mount=kvv2.path,
+        name=azure_secret.name.apply(lambda name: f"{name}/dev"),
         data_json=json.dumps({
             "password": "test",
         }))
     secrets = vault.kv.get_secrets_list_v2_output(mount=kvv2.path)
     nested_secrets = kvv2.path.apply(lambda path: vault.kv.get_secrets_list_v2_output(mount=path,
-        name=vault_kv_secret_v2["test_2"]["name"]))
+        name=test2["name"]))
     ```
     <!--End PulumiCodeChooser -->
 
     ## Required Vault Capabilities
 
     Use of this resource requires the `read` capability on the given path.
```

### Comparing `pulumi_vault-6.2.0a1713339773/pulumi_vault/kv/outputs.py` & `pulumi_vault-6.2.0a1713561465/pulumi_vault/kv/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1713339773/pulumi_vault/kv/secret.py` & `pulumi_vault-6.2.0a1713561465/pulumi_vault/kv/secret.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1713339773/pulumi_vault/kv/secret_backend_v2.py` & `pulumi_vault-6.2.0a1713561465/pulumi_vault/kv/secret_backend_v2.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1713339773/pulumi_vault/kv/secret_v2.py` & `pulumi_vault-6.2.0a1713561465/pulumi_vault/kv/secret_v2.py`

 * *Files 0% similar despite different names*

```diff
@@ -459,14 +459,15 @@
             type="kv",
             options={
                 "version": "2",
             },
             description="KV Version 2 secret engine mount")
         example = vault.kv.SecretV2("example",
             mount=kvv2.path,
+            name="secret",
             cas=1,
             delete_all_versions=True,
             data_json=json.dumps({
                 "zip": "zap",
                 "foo": "bar",
             }),
             custom_metadata=vault.kv.SecretV2CustomMetadataArgs(
@@ -557,14 +558,15 @@
             type="kv",
             options={
                 "version": "2",
             },
             description="KV Version 2 secret engine mount")
         example = vault.kv.SecretV2("example",
             mount=kvv2.path,
+            name="secret",
             cas=1,
             delete_all_versions=True,
             data_json=json.dumps({
                 "zip": "zap",
                 "foo": "bar",
             }),
             custom_metadata=vault.kv.SecretV2CustomMetadataArgs(
```

### Comparing `pulumi_vault-6.2.0a1713339773/pulumi_vault/ldap/__init__.py` & `pulumi_vault-6.2.0a1713561465/pulumi_vault/ldap/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1713339773/pulumi_vault/ldap/auth_backend.py` & `pulumi_vault-6.2.0a1713561465/pulumi_vault/ldap/auth_backend.py`

 * *Files 0% similar despite different names*

```diff
@@ -1332,22 +1332,22 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_vault as vault
 
         ldap = vault.ldap.AuthBackend("ldap",
-            discoverdn=False,
-            groupdn="OU=Groups,DC=example,DC=org",
-            groupfilter="(&(objectClass=group)(member:1.2.840.113556.1.4.1941:={{.UserDN}}))",
             path="ldap",
-            upndomain="EXAMPLE.ORG",
             url="ldaps://dc-01.example.org",
+            userdn="OU=Users,OU=Accounts,DC=example,DC=org",
             userattr="sAMAccountName",
-            userdn="OU=Users,OU=Accounts,DC=example,DC=org")
+            upndomain="EXAMPLE.ORG",
+            discoverdn=False,
+            groupdn="OU=Groups,DC=example,DC=org",
+            groupfilter="(&(objectClass=group)(member:1.2.840.113556.1.4.1941:={{.UserDN}}))")
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
 
         LDAP authentication backends can be imported using the `path`, e.g.
 
@@ -1424,22 +1424,22 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_vault as vault
 
         ldap = vault.ldap.AuthBackend("ldap",
-            discoverdn=False,
-            groupdn="OU=Groups,DC=example,DC=org",
-            groupfilter="(&(objectClass=group)(member:1.2.840.113556.1.4.1941:={{.UserDN}}))",
             path="ldap",
-            upndomain="EXAMPLE.ORG",
             url="ldaps://dc-01.example.org",
+            userdn="OU=Users,OU=Accounts,DC=example,DC=org",
             userattr="sAMAccountName",
-            userdn="OU=Users,OU=Accounts,DC=example,DC=org")
+            upndomain="EXAMPLE.ORG",
+            discoverdn=False,
+            groupdn="OU=Groups,DC=example,DC=org",
+            groupfilter="(&(objectClass=group)(member:1.2.840.113556.1.4.1941:={{.UserDN}}))")
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
 
         LDAP authentication backends can be imported using the `path`, e.g.
```

### Comparing `pulumi_vault-6.2.0a1713339773/pulumi_vault/ldap/auth_backend_group.py` & `pulumi_vault-6.2.0a1713561465/pulumi_vault/ldap/auth_backend_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1713339773/pulumi_vault/ldap/auth_backend_user.py` & `pulumi_vault-6.2.0a1713561465/pulumi_vault/ldap/auth_backend_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1713339773/pulumi_vault/ldap/get_dynamic_credentials.py` & `pulumi_vault-6.2.0a1713561465/pulumi_vault/ldap/get_dynamic_credentials.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1713339773/pulumi_vault/ldap/get_static_credentials.py` & `pulumi_vault-6.2.0a1713561465/pulumi_vault/ldap/get_static_credentials.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1713339773/pulumi_vault/ldap/secret_backend.py` & `pulumi_vault-6.2.0a1713561465/pulumi_vault/ldap/secret_backend.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1053,19 +1053,19 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_vault as vault
 
         config = vault.ldap.SecretBackend("config",
+            path="my-custom-ldap",
             binddn="CN=Administrator,CN=Users,DC=corp,DC=example,DC=net",
             bindpass="SuperSecretPassw0rd",
-            insecure_tls=True,
-            path="my-custom-ldap",
             url="ldaps://localhost",
+            insecure_tls=True,
             userdn="CN=Users,DC=corp,DC=example,DC=net")
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
 
         LDAP secret backend can be imported using the `${mount}/config`, e.g.
@@ -1128,19 +1128,19 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_vault as vault
 
         config = vault.ldap.SecretBackend("config",
+            path="my-custom-ldap",
             binddn="CN=Administrator,CN=Users,DC=corp,DC=example,DC=net",
             bindpass="SuperSecretPassw0rd",
-            insecure_tls=True,
-            path="my-custom-ldap",
             url="ldaps://localhost",
+            insecure_tls=True,
             userdn="CN=Users,DC=corp,DC=example,DC=net")
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
 
         LDAP secret backend can be imported using the `${mount}/config`, e.g.
```

### Comparing `pulumi_vault-6.2.0a1713339773/pulumi_vault/ldap/secret_backend_dynamic_role.py` & `pulumi_vault-6.2.0a1713561465/pulumi_vault/ldap/secret_backend_dynamic_role.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1713339773/pulumi_vault/ldap/secret_backend_library_set.py` & `pulumi_vault-6.2.0a1713561465/pulumi_vault/ldap/secret_backend_library_set.py`

 * *Files 0% similar despite different names*

```diff
@@ -308,14 +308,15 @@
             binddn="CN=Administrator,CN=Users,DC=corp,DC=example,DC=net",
             bindpass="SuperSecretPassw0rd",
             url="ldaps://localhost",
             insecure_tls=True,
             userdn="CN=Users,DC=corp,DC=example,DC=net")
         qa = vault.ldap.SecretBackendLibrarySet("qa",
             mount=config.path,
+            name="qa",
             service_account_names=[
                 "Bob",
                 "Mary",
             ],
             ttl=60,
             disable_check_in_enforcement=True,
             max_ttl=120)
@@ -367,14 +368,15 @@
             binddn="CN=Administrator,CN=Users,DC=corp,DC=example,DC=net",
             bindpass="SuperSecretPassw0rd",
             url="ldaps://localhost",
             insecure_tls=True,
             userdn="CN=Users,DC=corp,DC=example,DC=net")
         qa = vault.ldap.SecretBackendLibrarySet("qa",
             mount=config.path,
+            name="qa",
             service_account_names=[
                 "Bob",
                 "Mary",
             ],
             ttl=60,
             disable_check_in_enforcement=True,
             max_ttl=120)
```

### Comparing `pulumi_vault-6.2.0a1713339773/pulumi_vault/ldap/secret_backend_static_role.py` & `pulumi_vault-6.2.0a1713561465/pulumi_vault/ldap/secret_backend_static_role.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1713339773/pulumi_vault/managed/_inputs.py` & `pulumi_vault-6.2.0a1713561465/pulumi_vault/managed/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1713339773/pulumi_vault/managed/keys.py` & `pulumi_vault-6.2.0a1713561465/pulumi_vault/managed/keys.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1713339773/pulumi_vault/managed/outputs.py` & `pulumi_vault-6.2.0a1713561465/pulumi_vault/managed/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1713339773/pulumi_vault/mfa_duo.py` & `pulumi_vault-6.2.0a1713561465/pulumi_vault/mfa_duo.py`

 * *Files 0% similar despite different names*

```diff
@@ -332,15 +332,16 @@
         ```python
         import pulumi
         import pulumi_vault as vault
 
         userpass = vault.AuthBackend("userpass",
             type="userpass",
             path="userpass")
-        my_duo = vault.MfaDuo("myDuo",
+        my_duo = vault.MfaDuo("my_duo",
+            name="my_duo",
             mount_accessor=userpass.accessor,
             secret_key="8C7THtrIigh2rPZQMbguugt8IUftWhMRCOBzbuyz",
             integration_key="BIACEUEAXI20BNWTEYXT",
             api_hostname="api-2b5c39f5.duosecurity.com")
         ```
         <!--End PulumiCodeChooser -->
 
@@ -387,15 +388,16 @@
         ```python
         import pulumi
         import pulumi_vault as vault
 
         userpass = vault.AuthBackend("userpass",
             type="userpass",
             path="userpass")
-        my_duo = vault.MfaDuo("myDuo",
+        my_duo = vault.MfaDuo("my_duo",
+            name="my_duo",
             mount_accessor=userpass.accessor,
             secret_key="8C7THtrIigh2rPZQMbguugt8IUftWhMRCOBzbuyz",
             integration_key="BIACEUEAXI20BNWTEYXT",
             api_hostname="api-2b5c39f5.duosecurity.com")
         ```
         <!--End PulumiCodeChooser -->
```

### Comparing `pulumi_vault-6.2.0a1713339773/pulumi_vault/mfa_okta.py` & `pulumi_vault-6.2.0a1713561465/pulumi_vault/mfa_okta.py`

 * *Files 1% similar despite different names*

```diff
@@ -353,15 +353,16 @@
         ```python
         import pulumi
         import pulumi_vault as vault
 
         userpass = vault.AuthBackend("userpass",
             type="userpass",
             path="userpass")
-        my_okta = vault.MfaOkta("myOkta",
+        my_okta = vault.MfaOkta("my_okta",
+            name="my_okta",
             mount_accessor=userpass.accessor,
             username_format="user@example.com",
             org_name="hashicorp",
             api_token="eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9")
         ```
         <!--End PulumiCodeChooser -->
 
@@ -413,15 +414,16 @@
         ```python
         import pulumi
         import pulumi_vault as vault
 
         userpass = vault.AuthBackend("userpass",
             type="userpass",
             path="userpass")
-        my_okta = vault.MfaOkta("myOkta",
+        my_okta = vault.MfaOkta("my_okta",
+            name="my_okta",
             mount_accessor=userpass.accessor,
             username_format="user@example.com",
             org_name="hashicorp",
             api_token="eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9")
         ```
         <!--End PulumiCodeChooser -->
```

### Comparing `pulumi_vault-6.2.0a1713339773/pulumi_vault/mfa_pingid.py` & `pulumi_vault-6.2.0a1713561465/pulumi_vault/mfa_pingid.py`

 * *Files 2% similar despite different names*

```diff
@@ -365,15 +365,16 @@
         import pulumi_vault as vault
 
         config = pulumi.Config()
         settings_file = config.require_object("settingsFile")
         userpass = vault.AuthBackend("userpass",
             type="userpass",
             path="userpass")
-        my_pingid = vault.MfaPingid("myPingid",
+        my_pingid = vault.MfaPingid("my_pingid",
+            name="my_pingid",
             mount_accessor=userpass.accessor,
             username_format="user@example.com",
             settings_file_base64=settings_file)
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
@@ -422,15 +423,16 @@
         import pulumi_vault as vault
 
         config = pulumi.Config()
         settings_file = config.require_object("settingsFile")
         userpass = vault.AuthBackend("userpass",
             type="userpass",
             path="userpass")
-        my_pingid = vault.MfaPingid("myPingid",
+        my_pingid = vault.MfaPingid("my_pingid",
+            name="my_pingid",
             mount_accessor=userpass.accessor,
             username_format="user@example.com",
             settings_file_base64=settings_file)
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
```

### Comparing `pulumi_vault-6.2.0a1713339773/pulumi_vault/mfa_totp.py` & `pulumi_vault-6.2.0a1713561465/pulumi_vault/mfa_totp.py`

 * *Files 0% similar despite different names*

```diff
@@ -361,20 +361,21 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_vault as vault
 
-        my_totp = vault.MfaTotp("myTotp",
+        my_totp = vault.MfaTotp("my_totp",
+            name="my_totp",
+            issuer="hashicorp",
+            period=60,
             algorithm="SHA256",
             digits=8,
-            issuer="hashicorp",
-            key_size=20,
-            period=60)
+            key_size=20)
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
 
         Mounts can be imported using the `path`, e.g.
 
@@ -414,20 +415,21 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_vault as vault
 
-        my_totp = vault.MfaTotp("myTotp",
+        my_totp = vault.MfaTotp("my_totp",
+            name="my_totp",
+            issuer="hashicorp",
+            period=60,
             algorithm="SHA256",
             digits=8,
-            issuer="hashicorp",
-            key_size=20,
-            period=60)
+            key_size=20)
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
 
         Mounts can be imported using the `path`, e.g.
```

### Comparing `pulumi_vault-6.2.0a1713339773/pulumi_vault/mongodbatlas/secret_backend.py` & `pulumi_vault-6.2.0a1713561465/pulumi_vault/mongodbatlas/secret_backend.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1713339773/pulumi_vault/mongodbatlas/secret_role.py` & `pulumi_vault-6.2.0a1713561465/pulumi_vault/mongodbatlas/secret_role.py`

 * *Files 0% similar despite different names*

```diff
@@ -428,14 +428,15 @@
             description="MongoDB Atlas secret engine mount")
         config = vault.mongodbatlas.SecretBackend("config",
             mount=mongo.path,
             private_key="privateKey",
             public_key="publicKey")
         role = vault.mongodbatlas.SecretRole("role",
             mount=mongo.path,
+            name="tf-test-role",
             organization_id="7cf5a45a9ccf6400e60981b7",
             project_id="5cf5a45a9ccf6400e60981b6",
             roles=["ORG_READ_ONLY"],
             ip_addresses="192.168.1.5, 192.168.1.6",
             cidr_blocks="192.168.1.3/35",
             project_roles=["GROUP_READ_ONLY"],
             ttl="60",
@@ -491,14 +492,15 @@
             description="MongoDB Atlas secret engine mount")
         config = vault.mongodbatlas.SecretBackend("config",
             mount=mongo.path,
             private_key="privateKey",
             public_key="publicKey")
         role = vault.mongodbatlas.SecretRole("role",
             mount=mongo.path,
+            name="tf-test-role",
             organization_id="7cf5a45a9ccf6400e60981b7",
             project_id="5cf5a45a9ccf6400e60981b6",
             roles=["ORG_READ_ONLY"],
             ip_addresses="192.168.1.5, 192.168.1.6",
             cidr_blocks="192.168.1.3/35",
             project_roles=["GROUP_READ_ONLY"],
             ttl="60",
```

### Comparing `pulumi_vault-6.2.0a1713339773/pulumi_vault/mount.py` & `pulumi_vault-6.2.0a1713561465/pulumi_vault/mount.py`

 * *Files 0% similar despite different names*

```diff
@@ -495,62 +495,62 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_vault as vault
 
         example = vault.Mount("example",
-            description="This is an example mount",
             path="dummy",
-            type="generic")
+            type="generic",
+            description="This is an example mount")
         ```
         <!--End PulumiCodeChooser -->
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_vault as vault
 
         kvv2_example = vault.Mount("kvv2-example",
-            description="This is an example KV Version 2 secret engine mount",
+            path="version2-example",
+            type="kv-v2",
             options={
-                "type": "kv-v2",
                 "version": "2",
+                "type": "kv-v2",
             },
-            path="version2-example",
-            type="kv-v2")
+            description="This is an example KV Version 2 secret engine mount")
         ```
         <!--End PulumiCodeChooser -->
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_vault as vault
 
         transit_example = vault.Mount("transit-example",
+            path="transit-example",
+            type="transit",
             description="This is an example transit secret engine mount",
             options={
                 "convergent_encryption": False,
-            },
-            path="transit-example",
-            type="transit")
+            })
         ```
         <!--End PulumiCodeChooser -->
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_vault as vault
 
         pki_example = vault.Mount("pki-example",
-            default_lease_ttl_seconds=3600,
-            description="This is an example PKI mount",
-            max_lease_ttl_seconds=86400,
             path="pki-example",
-            type="pki")
+            type="pki",
+            description="This is an example PKI mount",
+            default_lease_ttl_seconds=3600,
+            max_lease_ttl_seconds=86400)
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
 
         Mounts can be imported using the `path`, e.g.
 
@@ -590,62 +590,62 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_vault as vault
 
         example = vault.Mount("example",
-            description="This is an example mount",
             path="dummy",
-            type="generic")
+            type="generic",
+            description="This is an example mount")
         ```
         <!--End PulumiCodeChooser -->
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_vault as vault
 
         kvv2_example = vault.Mount("kvv2-example",
-            description="This is an example KV Version 2 secret engine mount",
+            path="version2-example",
+            type="kv-v2",
             options={
-                "type": "kv-v2",
                 "version": "2",
+                "type": "kv-v2",
             },
-            path="version2-example",
-            type="kv-v2")
+            description="This is an example KV Version 2 secret engine mount")
         ```
         <!--End PulumiCodeChooser -->
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_vault as vault
 
         transit_example = vault.Mount("transit-example",
+            path="transit-example",
+            type="transit",
             description="This is an example transit secret engine mount",
             options={
                 "convergent_encryption": False,
-            },
-            path="transit-example",
-            type="transit")
+            })
         ```
         <!--End PulumiCodeChooser -->
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_vault as vault
 
         pki_example = vault.Mount("pki-example",
-            default_lease_ttl_seconds=3600,
-            description="This is an example PKI mount",
-            max_lease_ttl_seconds=86400,
             path="pki-example",
-            type="pki")
+            type="pki",
+            description="This is an example PKI mount",
+            default_lease_ttl_seconds=3600,
+            max_lease_ttl_seconds=86400)
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
 
         Mounts can be imported using the `path`, e.g.
```

### Comparing `pulumi_vault-6.2.0a1713339773/pulumi_vault/namespace.py` & `pulumi_vault-6.2.0a1713561465/pulumi_vault/namespace.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1713339773/pulumi_vault/nomad_secret_backend.py` & `pulumi_vault-6.2.0a1713561465/pulumi_vault/nomad_secret_backend.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -573,20 +573,20 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_vault as vault
 
         config = vault.NomadSecretBackend("config",
-            address="https://127.0.0.1:4646",
             backend="nomad",
-            default_lease_ttl_seconds=3600,
             description="test description",
+            default_lease_ttl_seconds=3600,
             max_lease_ttl_seconds=7200,
             max_ttl=240,
+            address="https://127.0.0.1:4646",
             token="ae20ceaa-...",
             ttl=120)
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
 
@@ -635,20 +635,20 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_vault as vault
 
         config = vault.NomadSecretBackend("config",
-            address="https://127.0.0.1:4646",
             backend="nomad",
-            default_lease_ttl_seconds=3600,
             description="test description",
+            default_lease_ttl_seconds=3600,
             max_lease_ttl_seconds=7200,
             max_ttl=240,
+            address="https://127.0.0.1:4646",
             token="ae20ceaa-...",
             ttl=120)
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
```

### Comparing `pulumi_vault-6.2.0a1713339773/pulumi_vault/nomad_secret_role.py` & `pulumi_vault-6.2.0a1713561465/pulumi_vault/nomad_secret_role.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1713339773/pulumi_vault/okta/_inputs.py` & `pulumi_vault-6.2.0a1713561465/pulumi_vault/okta/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1713339773/pulumi_vault/okta/auth_backend.py` & `pulumi_vault-6.2.0a1713561465/pulumi_vault/okta/auth_backend.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -491,26 +491,26 @@
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_vault as vault
 
         example = vault.okta.AuthBackend("example",
             description="Demonstration of the Terraform Okta auth backend",
+            organization="example",
+            token="something that should be kept secret",
             groups=[vault.okta.AuthBackendGroupArgs(
                 group_name="foo",
                 policies=[
                     "one",
                     "two",
                 ],
             )],
-            organization="example",
-            token="something that should be kept secret",
             users=[vault.okta.AuthBackendUserArgs(
-                groups=["foo"],
                 username="bar",
+                groups=["foo"],
             )])
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
 
         Okta authentication backends can be imported using its `path`, e.g.
@@ -558,26 +558,26 @@
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_vault as vault
 
         example = vault.okta.AuthBackend("example",
             description="Demonstration of the Terraform Okta auth backend",
+            organization="example",
+            token="something that should be kept secret",
             groups=[vault.okta.AuthBackendGroupArgs(
                 group_name="foo",
                 policies=[
                     "one",
                     "two",
                 ],
             )],
-            organization="example",
-            token="something that should be kept secret",
             users=[vault.okta.AuthBackendUserArgs(
-                groups=["foo"],
                 username="bar",
+                groups=["foo"],
             )])
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
 
         Okta authentication backends can be imported using its `path`, e.g.
```

### Comparing `pulumi_vault-6.2.0a1713339773/pulumi_vault/okta/auth_backend_group.py` & `pulumi_vault-6.2.0a1713561465/pulumi_vault/okta/auth_backend_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1713339773/pulumi_vault/okta/auth_backend_user.py` & `pulumi_vault-6.2.0a1713561465/pulumi_vault/okta/auth_backend_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1713339773/pulumi_vault/okta/outputs.py` & `pulumi_vault-6.2.0a1713561465/pulumi_vault/okta/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1713339773/pulumi_vault/outputs.py` & `pulumi_vault-6.2.0a1713561465/pulumi_vault/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1713339773/pulumi_vault/password_policy.py` & `pulumi_vault-6.2.0a1713561465/pulumi_vault/password_policy.py`

 * *Files 2% similar despite different names*

```diff
@@ -151,19 +151,20 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_vault as vault
 
-        alphanumeric = vault.PasswordPolicy("alphanumeric", policy=\"\"\"    length = 20
+        alphanumeric = vault.PasswordPolicy("alphanumeric",
+            name="alphanumeric",
+            policy=\"\"\"    length = 20
             rule "charset" {
               charset = "abcdefghijklmnopqrstuvwxyz0123456789"
             }
-          
         \"\"\")
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
 
         Password policies can be imported using the `name`, e.g.
@@ -195,19 +196,20 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_vault as vault
 
-        alphanumeric = vault.PasswordPolicy("alphanumeric", policy=\"\"\"    length = 20
+        alphanumeric = vault.PasswordPolicy("alphanumeric",
+            name="alphanumeric",
+            policy=\"\"\"    length = 20
             rule "charset" {
               charset = "abcdefghijklmnopqrstuvwxyz0123456789"
             }
-          
         \"\"\")
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
 
         Password policies can be imported using the `name`, e.g.
```

### Comparing `pulumi_vault-6.2.0a1713339773/pulumi_vault/pkisecret/__init__.py` & `pulumi_vault-6.2.0a1713561465/pulumi_vault/pkisecret/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1713339773/pulumi_vault/pkisecret/_inputs.py` & `pulumi_vault-6.2.0a1713561465/pulumi_vault/pkisecret/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1713339773/pulumi_vault/pkisecret/backend_config_cluster.py` & `pulumi_vault-6.2.0a1713561465/pulumi_vault/pkisecret/backend_config_cluster.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1713339773/pulumi_vault/pkisecret/get_backend_issuer.py` & `pulumi_vault-6.2.0a1713561465/pulumi_vault/pkisecret/get_backend_issuer.py`

 * *Files 12% similar despite different names*

```diff
@@ -171,14 +171,34 @@
 def get_backend_issuer(backend: Optional[str] = None,
                        issuer_ref: Optional[str] = None,
                        namespace: Optional[str] = None,
                        opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetBackendIssuerResult:
     """
     ## Example Usage
 
+    <!--Start PulumiCodeChooser -->
+    ```python
+    import pulumi
+    import pulumi_vault as vault
+
+    pki = vault.Mount("pki",
+        path="pki",
+        type="pki",
+        description="PKI secret engine mount")
+    root = vault.pki_secret.SecretBackendRootCert("root",
+        backend=pki.path,
+        type="internal",
+        common_name="example",
+        ttl="86400",
+        issuer_name="example")
+    example = root.issuer_id.apply(lambda issuer_id: vault.pkiSecret.get_backend_issuer_output(backend=root.path,
+        issuer_ref=issuer_id))
+    ```
+    <!--End PulumiCodeChooser -->
+
 
     :param str backend: The path to the PKI secret backend to
            read the issuer from, with no leading or trailing `/`s.
     :param str issuer_ref: Reference to an existing issuer.
     :param str namespace: The namespace of the target resource.
            The value should not contain leading or trailing forward slashes.
            The `namespace` is always relative to the provider's configured [namespace](https://www.terraform.io/docs/providers/vault/index.html#namespace).
@@ -210,14 +230,34 @@
 def get_backend_issuer_output(backend: Optional[pulumi.Input[str]] = None,
                               issuer_ref: Optional[pulumi.Input[str]] = None,
                               namespace: Optional[pulumi.Input[Optional[str]]] = None,
                               opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetBackendIssuerResult]:
     """
     ## Example Usage
 
+    <!--Start PulumiCodeChooser -->
+    ```python
+    import pulumi
+    import pulumi_vault as vault
+
+    pki = vault.Mount("pki",
+        path="pki",
+        type="pki",
+        description="PKI secret engine mount")
+    root = vault.pki_secret.SecretBackendRootCert("root",
+        backend=pki.path,
+        type="internal",
+        common_name="example",
+        ttl="86400",
+        issuer_name="example")
+    example = root.issuer_id.apply(lambda issuer_id: vault.pkiSecret.get_backend_issuer_output(backend=root.path,
+        issuer_ref=issuer_id))
+    ```
+    <!--End PulumiCodeChooser -->
+
 
     :param str backend: The path to the PKI secret backend to
            read the issuer from, with no leading or trailing `/`s.
     :param str issuer_ref: Reference to an existing issuer.
     :param str namespace: The namespace of the target resource.
            The value should not contain leading or trailing forward slashes.
            The `namespace` is always relative to the provider's configured [namespace](https://www.terraform.io/docs/providers/vault/index.html#namespace).
```

### Comparing `pulumi_vault-6.2.0a1713339773/pulumi_vault/pkisecret/get_backend_issuers.py` & `pulumi_vault-6.2.0a1713561465/pulumi_vault/pkisecret/get_backend_issuers.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1713339773/pulumi_vault/pkisecret/get_backend_key.py` & `pulumi_vault-6.2.0a1713561465/pulumi_vault/pkisecret/get_backend_key.py`

 * *Files 4% similar despite different names*

```diff
@@ -125,15 +125,15 @@
         description="PKI secret engine mount")
     key = vault.pki_secret.SecretBackendKey("key",
         backend=pki.path,
         type="internal",
         key_name="example",
         key_type="rsa",
         key_bits=4096)
-    example = key.key_id.apply(lambda key_id: vault.pkiSecret.get_backend_key_output(backend=vault_mount["key"]["path"],
+    example = key.key_id.apply(lambda key_id: vault.pkiSecret.get_backend_key_output(backend=key_vault_mount["path"],
         key_ref=key_id))
     ```
     <!--End PulumiCodeChooser -->
 
 
     :param str backend: The path to the PKI secret backend to
            read the key from, with no leading or trailing `/`s.
@@ -179,15 +179,15 @@
         description="PKI secret engine mount")
     key = vault.pki_secret.SecretBackendKey("key",
         backend=pki.path,
         type="internal",
         key_name="example",
         key_type="rsa",
         key_bits=4096)
-    example = key.key_id.apply(lambda key_id: vault.pkiSecret.get_backend_key_output(backend=vault_mount["key"]["path"],
+    example = key.key_id.apply(lambda key_id: vault.pkiSecret.get_backend_key_output(backend=key_vault_mount["path"],
         key_ref=key_id))
     ```
     <!--End PulumiCodeChooser -->
 
 
     :param str backend: The path to the PKI secret backend to
            read the key from, with no leading or trailing `/`s.
```

### Comparing `pulumi_vault-6.2.0a1713339773/pulumi_vault/pkisecret/get_backend_keys.py` & `pulumi_vault-6.2.0a1713561465/pulumi_vault/pkisecret/get_backend_keys.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1713339773/pulumi_vault/pkisecret/outputs.py` & `pulumi_vault-6.2.0a1713561465/pulumi_vault/pkisecret/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1713339773/pulumi_vault/pkisecret/secret_backend_cert.py` & `pulumi_vault-6.2.0a1713561465/pulumi_vault/pkisecret/secret_backend_cert.py`

 * *Files 0% similar despite different names*

```diff
@@ -737,17 +737,18 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_vault as vault
 
         app = vault.pki_secret.SecretBackendCert("app",
-            backend=vault_mount["intermediate"]["path"],
+            backend=intermediate["path"],
+            name=test["name"],
             common_name="app.my.domain",
-            opts=pulumi.ResourceOptions(depends_on=[vault_pki_secret_backend_role["admin"]]))
+            opts=pulumi.ResourceOptions(depends_on=[admin]))
         ```
         <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] alt_names: List of alternative names
         :param pulumi.Input[bool] auto_renew: If set to `true`, certs will be renewed if the expiration is within `min_seconds_remaining`. Default `false`
@@ -781,17 +782,18 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_vault as vault
 
         app = vault.pki_secret.SecretBackendCert("app",
-            backend=vault_mount["intermediate"]["path"],
+            backend=intermediate["path"],
+            name=test["name"],
             common_name="app.my.domain",
-            opts=pulumi.ResourceOptions(depends_on=[vault_pki_secret_backend_role["admin"]]))
+            opts=pulumi.ResourceOptions(depends_on=[admin]))
         ```
         <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param SecretBackendCertArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
```

### Comparing `pulumi_vault-6.2.0a1713339773/pulumi_vault/pkisecret/secret_backend_config_ca.py` & `pulumi_vault-6.2.0a1713561465/pulumi_vault/pkisecret/secret_backend_config_ca.py`

 * *Files 2% similar despite different names*

```diff
@@ -147,15 +147,15 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_vault as vault
 
         intermediate = vault.pki_secret.SecretBackendConfigCa("intermediate",
-            backend=vault_mount["intermediate"]["path"],
+            backend=intermediate_vault_mount["path"],
             pem_bundle=\"\"\"-----BEGIN RSA PRIVATE KEY-----
         MIIEowIBAAKCAQEAwvEHeJCXnFgi88rE1dTX6FHdBPK0wSjedh0ywVnCZxLWbBv/
         5PytjTcCPdrfW7g2sfbPwOge/WF3X2KeYSP8SxZA0czmz6QDspeG921JkZWtyp5o
         ++N0leLTIUAhq339p3O1onAOUO1k4sHfmCwfrDpTn2hcx4URa5Pzzb1fHigusjIH
         1mcGdncaA6Z2CzO1w4E8kPOUukIDrcZT4faOZrWUIQZKQw2JzTyKJ+ZMDCZq2TFz
         WwpL3eG48wB7J7mibFQ/9nFvxpIflBjDAZ8QiqkwYr5N0DNsTxcfTCSeubfJDCUf
         IWwFZhLitzwOxazazUQKXX/SPMQ1l/L9o3nnHwIDAQABAoIBAAQidJQcDPsl62fc
@@ -197,15 +197,15 @@
         JbV5aRetovGOcV//8vbxkZm/ntQ8Oo+2sfGR5lIzd0UdlOr5pkD6g3bFy/zJ+4DR
         DAe8fklUacfz6CFmD+H8GyHm+fKmF+mjr4oOGQW6OegRDJHuiipUk2lJyuXdlPSa
         FpNRO2sGbjn000ANinFgnFiVzGDnx0/G1Kii/6GWrI6rrdVmXioQzF+8AloWckeB
         +hbmbwkwQa/JrLb5SWcBDOXSgtn1Li3XF5AQQBBjA3pOlyBXqnI94Irw89Lv9uPT
         MUR4qFxeUOW/GJGccMUd
         -----END CERTIFICATE-----
         \"\"\",
-            opts=pulumi.ResourceOptions(depends_on=[vault_mount["intermediate"]]))
+            opts=pulumi.ResourceOptions(depends_on=[intermediate_vault_mount]))
         ```
         <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] backend: The PKI secret backend the resource belongs to.
         :param pulumi.Input[str] namespace: The namespace to provision the resource in.
@@ -225,15 +225,15 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_vault as vault
 
         intermediate = vault.pki_secret.SecretBackendConfigCa("intermediate",
-            backend=vault_mount["intermediate"]["path"],
+            backend=intermediate_vault_mount["path"],
             pem_bundle=\"\"\"-----BEGIN RSA PRIVATE KEY-----
         MIIEowIBAAKCAQEAwvEHeJCXnFgi88rE1dTX6FHdBPK0wSjedh0ywVnCZxLWbBv/
         5PytjTcCPdrfW7g2sfbPwOge/WF3X2KeYSP8SxZA0czmz6QDspeG921JkZWtyp5o
         ++N0leLTIUAhq339p3O1onAOUO1k4sHfmCwfrDpTn2hcx4URa5Pzzb1fHigusjIH
         1mcGdncaA6Z2CzO1w4E8kPOUukIDrcZT4faOZrWUIQZKQw2JzTyKJ+ZMDCZq2TFz
         WwpL3eG48wB7J7mibFQ/9nFvxpIflBjDAZ8QiqkwYr5N0DNsTxcfTCSeubfJDCUf
         IWwFZhLitzwOxazazUQKXX/SPMQ1l/L9o3nnHwIDAQABAoIBAAQidJQcDPsl62fc
@@ -275,15 +275,15 @@
         JbV5aRetovGOcV//8vbxkZm/ntQ8Oo+2sfGR5lIzd0UdlOr5pkD6g3bFy/zJ+4DR
         DAe8fklUacfz6CFmD+H8GyHm+fKmF+mjr4oOGQW6OegRDJHuiipUk2lJyuXdlPSa
         FpNRO2sGbjn000ANinFgnFiVzGDnx0/G1Kii/6GWrI6rrdVmXioQzF+8AloWckeB
         +hbmbwkwQa/JrLb5SWcBDOXSgtn1Li3XF5AQQBBjA3pOlyBXqnI94Irw89Lv9uPT
         MUR4qFxeUOW/GJGccMUd
         -----END CERTIFICATE-----
         \"\"\",
-            opts=pulumi.ResourceOptions(depends_on=[vault_mount["intermediate"]]))
+            opts=pulumi.ResourceOptions(depends_on=[intermediate_vault_mount]))
         ```
         <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param SecretBackendConfigCaArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
```

### Comparing `pulumi_vault-6.2.0a1713339773/pulumi_vault/pkisecret/secret_backend_config_issuers.py` & `pulumi_vault-6.2.0a1713561465/pulumi_vault/pkisecret/secret_backend_config_issuers.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1713339773/pulumi_vault/pkisecret/secret_backend_config_urls.py` & `pulumi_vault-6.2.0a1713561465/pulumi_vault/pkisecret/secret_backend_config_urls.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1713339773/pulumi_vault/pkisecret/secret_backend_crl_config.py` & `pulumi_vault-6.2.0a1713561465/pulumi_vault/pkisecret/secret_backend_crl_config.py`

 * *Files 0% similar despite different names*

```diff
@@ -496,15 +496,15 @@
         import pulumi_vault as vault
 
         pki = vault.Mount("pki",
             path="%s",
             type="pki",
             default_lease_ttl_seconds=3600,
             max_lease_ttl_seconds=86400)
-        crl_config = vault.pki_secret.SecretBackendCrlConfig("crlConfig",
+        crl_config = vault.pki_secret.SecretBackendCrlConfig("crl_config",
             backend=pki.path,
             expiry="72h",
             disable=False)
         ```
         <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
@@ -546,15 +546,15 @@
         import pulumi_vault as vault
 
         pki = vault.Mount("pki",
             path="%s",
             type="pki",
             default_lease_ttl_seconds=3600,
             max_lease_ttl_seconds=86400)
-        crl_config = vault.pki_secret.SecretBackendCrlConfig("crlConfig",
+        crl_config = vault.pki_secret.SecretBackendCrlConfig("crl_config",
             backend=pki.path,
             expiry="72h",
             disable=False)
         ```
         <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
```

### Comparing `pulumi_vault-6.2.0a1713339773/pulumi_vault/pkisecret/secret_backend_intermediate_cert_request.py` & `pulumi_vault-6.2.0a1713561465/pulumi_vault/pkisecret/secret_backend_intermediate_cert_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -964,18 +964,18 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_vault as vault
 
         test = vault.pki_secret.SecretBackendIntermediateCertRequest("test",
-            backend=vault_mount["pki"]["path"],
+            backend=pki["path"],
             type="internal",
             common_name="app.my.domain",
-            opts=pulumi.ResourceOptions(depends_on=[vault_mount["pki"]]))
+            opts=pulumi.ResourceOptions(depends_on=[pki]))
         ```
         <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[bool] add_basic_constraints: Adds a Basic Constraints extension with 'CA: true'.
                Only needed as a workaround in some compatibility scenarios with Active Directory
@@ -1024,18 +1024,18 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_vault as vault
 
         test = vault.pki_secret.SecretBackendIntermediateCertRequest("test",
-            backend=vault_mount["pki"]["path"],
+            backend=pki["path"],
             type="internal",
             common_name="app.my.domain",
-            opts=pulumi.ResourceOptions(depends_on=[vault_mount["pki"]]))
+            opts=pulumi.ResourceOptions(depends_on=[pki]))
         ```
         <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param SecretBackendIntermediateCertRequestArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
```

### Comparing `pulumi_vault-6.2.0a1713339773/pulumi_vault/pkisecret/secret_backend_intermediate_set_signed.py` & `pulumi_vault-6.2.0a1713561465/pulumi_vault/pkisecret/secret_backend_intermediate_set_signed.py`

 * *Files 3% similar despite different names*

```diff
@@ -200,45 +200,45 @@
             max_lease_ttl_seconds=8640000)
         intermediate = vault.Mount("intermediate",
             path="pki-int",
             type=root.type,
             description="intermediate",
             default_lease_ttl_seconds=86400,
             max_lease_ttl_seconds=86400)
-        example_secret_backend_root_cert = vault.pki_secret.SecretBackendRootCert("exampleSecretBackendRootCert",
+        example = vault.pki_secret.SecretBackendRootCert("example",
             backend=root.path,
             type="internal",
             common_name="RootOrg Root CA",
             ttl="86400",
             format="pem",
             private_key_format="der",
             key_type="rsa",
             key_bits=4096,
             exclude_cn_from_sans=True,
             ou="Organizational Unit",
             organization="RootOrg",
             country="US",
             locality="San Francisco",
             province="CA")
-        example_secret_backend_intermediate_cert_request = vault.pki_secret.SecretBackendIntermediateCertRequest("exampleSecretBackendIntermediateCertRequest",
+        example_secret_backend_intermediate_cert_request = vault.pki_secret.SecretBackendIntermediateCertRequest("example",
             backend=intermediate.path,
-            type=example_secret_backend_root_cert.type,
+            type=example.type,
             common_name="SubOrg Intermediate CA")
-        example_secret_backend_root_sign_intermediate = vault.pki_secret.SecretBackendRootSignIntermediate("exampleSecretBackendRootSignIntermediate",
+        example_secret_backend_root_sign_intermediate = vault.pki_secret.SecretBackendRootSignIntermediate("example",
             backend=root.path,
             csr=example_secret_backend_intermediate_cert_request.csr,
             common_name="SubOrg Intermediate CA",
             exclude_cn_from_sans=True,
             ou="SubUnit",
             organization="SubOrg",
             country="US",
             locality="San Francisco",
             province="CA",
             revoke=True)
-        example_secret_backend_intermediate_set_signed = vault.pki_secret.SecretBackendIntermediateSetSigned("exampleSecretBackendIntermediateSetSigned",
+        example_secret_backend_intermediate_set_signed = vault.pki_secret.SecretBackendIntermediateSetSigned("example",
             backend=intermediate.path,
             certificate=example_secret_backend_root_sign_intermediate.certificate)
         ```
         <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
@@ -273,45 +273,45 @@
             max_lease_ttl_seconds=8640000)
         intermediate = vault.Mount("intermediate",
             path="pki-int",
             type=root.type,
             description="intermediate",
             default_lease_ttl_seconds=86400,
             max_lease_ttl_seconds=86400)
-        example_secret_backend_root_cert = vault.pki_secret.SecretBackendRootCert("exampleSecretBackendRootCert",
+        example = vault.pki_secret.SecretBackendRootCert("example",
             backend=root.path,
             type="internal",
             common_name="RootOrg Root CA",
             ttl="86400",
             format="pem",
             private_key_format="der",
             key_type="rsa",
             key_bits=4096,
             exclude_cn_from_sans=True,
             ou="Organizational Unit",
             organization="RootOrg",
             country="US",
             locality="San Francisco",
             province="CA")
-        example_secret_backend_intermediate_cert_request = vault.pki_secret.SecretBackendIntermediateCertRequest("exampleSecretBackendIntermediateCertRequest",
+        example_secret_backend_intermediate_cert_request = vault.pki_secret.SecretBackendIntermediateCertRequest("example",
             backend=intermediate.path,
-            type=example_secret_backend_root_cert.type,
+            type=example.type,
             common_name="SubOrg Intermediate CA")
-        example_secret_backend_root_sign_intermediate = vault.pki_secret.SecretBackendRootSignIntermediate("exampleSecretBackendRootSignIntermediate",
+        example_secret_backend_root_sign_intermediate = vault.pki_secret.SecretBackendRootSignIntermediate("example",
             backend=root.path,
             csr=example_secret_backend_intermediate_cert_request.csr,
             common_name="SubOrg Intermediate CA",
             exclude_cn_from_sans=True,
             ou="SubUnit",
             organization="SubOrg",
             country="US",
             locality="San Francisco",
             province="CA",
             revoke=True)
-        example_secret_backend_intermediate_set_signed = vault.pki_secret.SecretBackendIntermediateSetSigned("exampleSecretBackendIntermediateSetSigned",
+        example_secret_backend_intermediate_set_signed = vault.pki_secret.SecretBackendIntermediateSetSigned("example",
             backend=intermediate.path,
             certificate=example_secret_backend_root_sign_intermediate.certificate)
         ```
         <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param SecretBackendIntermediateSetSignedArgs args: The arguments to use to populate this resource's properties.
```

### Comparing `pulumi_vault-6.2.0a1713339773/pulumi_vault/pkisecret/secret_backend_issuer.py` & `pulumi_vault-6.2.0a1713561465/pulumi_vault/pkisecret/secret_backend_issuer.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1713339773/pulumi_vault/pkisecret/secret_backend_key.py` & `pulumi_vault-6.2.0a1713561465/pulumi_vault/pkisecret/secret_backend_key.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1713339773/pulumi_vault/pkisecret/secret_backend_role.py` & `pulumi_vault-6.2.0a1713561465/pulumi_vault/pkisecret/secret_backend_role.py`

 * *Files 0% similar despite different names*

```diff
@@ -1601,14 +1601,15 @@
         pki = vault.Mount("pki",
             path="pki",
             type="pki",
             default_lease_ttl_seconds=3600,
             max_lease_ttl_seconds=86400)
         role = vault.pki_secret.SecretBackendRole("role",
             backend=pki.path,
+            name="my_role",
             ttl="3600",
             allow_ip_sans=True,
             key_type="rsa",
             key_bits=4096,
             allowed_domains=[
                 "example.com",
                 "my.domain",
@@ -1702,14 +1703,15 @@
         pki = vault.Mount("pki",
             path="pki",
             type="pki",
             default_lease_ttl_seconds=3600,
             max_lease_ttl_seconds=86400)
         role = vault.pki_secret.SecretBackendRole("role",
             backend=pki.path,
+            name="my_role",
             ttl="3600",
             allow_ip_sans=True,
             key_type="rsa",
             key_bits=4096,
             allowed_domains=[
                 "example.com",
                 "my.domain",
```

### Comparing `pulumi_vault-6.2.0a1713339773/pulumi_vault/pkisecret/secret_backend_root_cert.py` & `pulumi_vault-6.2.0a1713561465/pulumi_vault/pkisecret/secret_backend_root_cert.py`

 * *Files 0% similar despite different names*

```diff
@@ -1075,26 +1075,26 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_vault as vault
 
         test = vault.pki_secret.SecretBackendRootCert("test",
-            backend=vault_mount["pki"]["path"],
+            backend=pki["path"],
             type="internal",
             common_name="Root CA",
             ttl="315360000",
             format="pem",
             private_key_format="der",
             key_type="rsa",
             key_bits=4096,
             exclude_cn_from_sans=True,
             ou="My OU",
             organization="My organization",
-            opts=pulumi.ResourceOptions(depends_on=[vault_mount["pki"]]))
+            opts=pulumi.ResourceOptions(depends_on=[pki]))
         ```
         <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] alt_names: List of alternative names
         :param pulumi.Input[str] backend: The PKI secret backend the resource belongs to.
@@ -1145,26 +1145,26 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_vault as vault
 
         test = vault.pki_secret.SecretBackendRootCert("test",
-            backend=vault_mount["pki"]["path"],
+            backend=pki["path"],
             type="internal",
             common_name="Root CA",
             ttl="315360000",
             format="pem",
             private_key_format="der",
             key_type="rsa",
             key_bits=4096,
             exclude_cn_from_sans=True,
             ou="My OU",
             organization="My organization",
-            opts=pulumi.ResourceOptions(depends_on=[vault_mount["pki"]]))
+            opts=pulumi.ResourceOptions(depends_on=[pki]))
         ```
         <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param SecretBackendRootCertArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
```

### Comparing `pulumi_vault-6.2.0a1713339773/pulumi_vault/pkisecret/secret_backend_root_sign_intermediate.py` & `pulumi_vault-6.2.0a1713561465/pulumi_vault/pkisecret/secret_backend_root_sign_intermediate.py`

 * *Files 2% similar despite different names*

```diff
@@ -902,21 +902,21 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_vault as vault
 
         root = vault.pki_secret.SecretBackendRootSignIntermediate("root",
-            backend=vault_mount["root"]["path"],
-            csr=vault_pki_secret_backend_intermediate_cert_request["intermediate"]["csr"],
+            backend=root_vault_mount["path"],
+            csr=intermediate["csr"],
             common_name="Intermediate CA",
             exclude_cn_from_sans=True,
             ou="My OU",
             organization="My organization",
-            opts=pulumi.ResourceOptions(depends_on=[vault_pki_secret_backend_intermediate_cert_request["intermediate"]]))
+            opts=pulumi.ResourceOptions(depends_on=[intermediate]))
         ```
         <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] alt_names: List of alternative names
         :param pulumi.Input[str] backend: The PKI secret backend the resource belongs to.
@@ -961,21 +961,21 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_vault as vault
 
         root = vault.pki_secret.SecretBackendRootSignIntermediate("root",
-            backend=vault_mount["root"]["path"],
-            csr=vault_pki_secret_backend_intermediate_cert_request["intermediate"]["csr"],
+            backend=root_vault_mount["path"],
+            csr=intermediate["csr"],
             common_name="Intermediate CA",
             exclude_cn_from_sans=True,
             ou="My OU",
             organization="My organization",
-            opts=pulumi.ResourceOptions(depends_on=[vault_pki_secret_backend_intermediate_cert_request["intermediate"]]))
+            opts=pulumi.ResourceOptions(depends_on=[intermediate]))
         ```
         <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param SecretBackendRootSignIntermediateArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
```

### Comparing `pulumi_vault-6.2.0a1713339773/pulumi_vault/pkisecret/secret_backend_sign.py` & `pulumi_vault-6.2.0a1713561465/pulumi_vault/pkisecret/secret_backend_sign.py`

 * *Files 0% similar despite different names*

```diff
@@ -650,15 +650,16 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_vault as vault
 
         test = vault.pki_secret.SecretBackendSign("test",
-            backend=vault_mount["pki"]["path"],
+            backend=pki["path"],
+            name=admin["name"],
             csr=\"\"\"-----BEGIN CERTIFICATE REQUEST-----
         MIIEqDCCApACAQAwYzELMAkGA1UEBhMCQVUxEzARBgNVBAgMClNvbWUtU3RhdGUx
         ITAfBgNVBAoMGEludGVybmV0IFdpZGdpdHMgUHR5IEx0ZDEcMBoGA1UEAwwTY2Vy
         dC50ZXN0Lm15LmRvbWFpbjCCAiIwDQYJKoZIhvcNAQEBBQADggIPADCCAgoCggIB
         AJupYCQ8UVCWII1Zof1c6YcSSaM9hEaDU78cfKP5RoSeH10BvrWRfT+mzCONVpNP
         CW9Iabtvk6hm0ot6ilnndEyVJbc0g7hdDLBX5BM25D+DGZGJRKUz1V+uBrWmXtIt
         Vonj7JTDTe7ViH0GDsB7CvqXFGXO2a2cDYBchLkL6vQiFPshxvUsLtwxuy/qdYgy
@@ -680,15 +681,15 @@
         dBKRNDfC4lS3jYJgs55jHqonZgkpSi3bamlxpfpW0ukGBcmq91wRe4bOw/4uD/vf
         UwqMWOdCYcU3mdYNjTWy22ORW3SGFQxMBwpUEURCSoeqWr6aJeQ7KAYkx1PrB5T8
         OTEc13lWf+B0PU9UJuGTsmpIuImPDVd0EVDayr3mT5dDbqTVDbe8ppf2IswABmf0
         o3DybUeUmknYjl109rdSf+76nuREICHatxXgN3xCMFuBaN4WLO+ksd6Y1Ys=
         -----END CERTIFICATE REQUEST-----
         \"\"\",
             common_name="test.my.domain",
-            opts=pulumi.ResourceOptions(depends_on=[vault_pki_secret_backend_role["admin"]]))
+            opts=pulumi.ResourceOptions(depends_on=[admin]))
         ```
         <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] alt_names: List of alternative names
         :param pulumi.Input[bool] auto_renew: If set to `true`, certs will be renewed if the expiration is within `min_seconds_remaining`. Default `false`
@@ -723,15 +724,16 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_vault as vault
 
         test = vault.pki_secret.SecretBackendSign("test",
-            backend=vault_mount["pki"]["path"],
+            backend=pki["path"],
+            name=admin["name"],
             csr=\"\"\"-----BEGIN CERTIFICATE REQUEST-----
         MIIEqDCCApACAQAwYzELMAkGA1UEBhMCQVUxEzARBgNVBAgMClNvbWUtU3RhdGUx
         ITAfBgNVBAoMGEludGVybmV0IFdpZGdpdHMgUHR5IEx0ZDEcMBoGA1UEAwwTY2Vy
         dC50ZXN0Lm15LmRvbWFpbjCCAiIwDQYJKoZIhvcNAQEBBQADggIPADCCAgoCggIB
         AJupYCQ8UVCWII1Zof1c6YcSSaM9hEaDU78cfKP5RoSeH10BvrWRfT+mzCONVpNP
         CW9Iabtvk6hm0ot6ilnndEyVJbc0g7hdDLBX5BM25D+DGZGJRKUz1V+uBrWmXtIt
         Vonj7JTDTe7ViH0GDsB7CvqXFGXO2a2cDYBchLkL6vQiFPshxvUsLtwxuy/qdYgy
@@ -753,15 +755,15 @@
         dBKRNDfC4lS3jYJgs55jHqonZgkpSi3bamlxpfpW0ukGBcmq91wRe4bOw/4uD/vf
         UwqMWOdCYcU3mdYNjTWy22ORW3SGFQxMBwpUEURCSoeqWr6aJeQ7KAYkx1PrB5T8
         OTEc13lWf+B0PU9UJuGTsmpIuImPDVd0EVDayr3mT5dDbqTVDbe8ppf2IswABmf0
         o3DybUeUmknYjl109rdSf+76nuREICHatxXgN3xCMFuBaN4WLO+ksd6Y1Ys=
         -----END CERTIFICATE REQUEST-----
         \"\"\",
             common_name="test.my.domain",
-            opts=pulumi.ResourceOptions(depends_on=[vault_pki_secret_backend_role["admin"]]))
+            opts=pulumi.ResourceOptions(depends_on=[admin]))
         ```
         <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param SecretBackendSignArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
```

### Comparing `pulumi_vault-6.2.0a1713339773/pulumi_vault/policy.py` & `pulumi_vault-6.2.0a1713561465/pulumi_vault/policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1713339773/pulumi_vault/provider.py` & `pulumi_vault-6.2.0a1713561465/pulumi_vault/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1713339773/pulumi_vault/quota_lease_count.py` & `pulumi_vault-6.2.0a1713561465/pulumi_vault/quota_lease_count.py`

 * *Files 1% similar despite different names*

```diff
@@ -247,16 +247,17 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_vault as vault
 
         global_ = vault.QuotaLeaseCount("global",
-            max_leases=100,
-            path="")
+            name="global",
+            path="",
+            max_leases=100)
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
 
         Lease count quotas can be imported using their names
 
@@ -301,16 +302,17 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_vault as vault
 
         global_ = vault.QuotaLeaseCount("global",
-            max_leases=100,
-            path="")
+            name="global",
+            path="",
+            max_leases=100)
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
 
         Lease count quotas can be imported using their names
```

### Comparing `pulumi_vault-6.2.0a1713339773/pulumi_vault/quota_rate_limit.py` & `pulumi_vault-6.2.0a1713561465/pulumi_vault/quota_rate_limit.py`

 * *Files 1% similar despite different names*

```diff
@@ -315,14 +315,15 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_vault as vault
 
         global_ = vault.QuotaRateLimit("global",
+            name="global",
             path="",
             rate=100)
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
 
@@ -370,14 +371,15 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_vault as vault
 
         global_ = vault.QuotaRateLimit("global",
+            name="global",
             path="",
             rate=100)
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
```

### Comparing `pulumi_vault-6.2.0a1713339773/pulumi_vault/rabbitmq/_inputs.py` & `pulumi_vault-6.2.0a1713561465/pulumi_vault/rabbitmq/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1713339773/pulumi_vault/rabbitmq/outputs.py` & `pulumi_vault-6.2.0a1713561465/pulumi_vault/rabbitmq/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1713339773/pulumi_vault/rabbitmq/secret_backend.py` & `pulumi_vault-6.2.0a1713561465/pulumi_vault/rabbitmq/secret_backend.py`

 * *Files 0% similar despite different names*

```diff
@@ -464,16 +464,16 @@
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_vault as vault
 
         rabbitmq = vault.rabbit_mq.SecretBackend("rabbitmq",
             connection_uri="https://.....",
-            password="password",
-            username="user")
+            username="user",
+            password="password")
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
 
         RabbitMQ secret backends can be imported using the `path`, e.g.
 
@@ -516,16 +516,16 @@
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_vault as vault
 
         rabbitmq = vault.rabbit_mq.SecretBackend("rabbitmq",
             connection_uri="https://.....",
-            password="password",
-            username="user")
+            username="user",
+            password="password")
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
 
         RabbitMQ secret backends can be imported using the `path`, e.g.
```

### Comparing `pulumi_vault-6.2.0a1713339773/pulumi_vault/rabbitmq/secret_backend_role.py` & `pulumi_vault-6.2.0a1713561465/pulumi_vault/rabbitmq/secret_backend_role.py`

 * *Files 0% similar despite different names*

```diff
@@ -262,14 +262,15 @@
 
         rabbitmq = vault.rabbit_mq.SecretBackend("rabbitmq",
             connection_uri="https://.....",
             username="user",
             password="password")
         role = vault.rabbit_mq.SecretBackendRole("role",
             backend=rabbitmq.path,
+            name="deploy",
             tags="tag1,tag2",
             vhosts=[vault.rabbit_mq.SecretBackendRoleVhostArgs(
                 host="/",
                 configure="",
                 read=".*",
                 write="",
             )],
@@ -322,14 +323,15 @@
 
         rabbitmq = vault.rabbit_mq.SecretBackend("rabbitmq",
             connection_uri="https://.....",
             username="user",
             password="password")
         role = vault.rabbit_mq.SecretBackendRole("role",
             backend=rabbitmq.path,
+            name="deploy",
             tags="tag1,tag2",
             vhosts=[vault.rabbit_mq.SecretBackendRoleVhostArgs(
                 host="/",
                 configure="",
                 read=".*",
                 write="",
             )],
```

### Comparing `pulumi_vault-6.2.0a1713339773/pulumi_vault/raft_autopilot.py` & `pulumi_vault-6.2.0a1713561465/pulumi_vault/raft_autopilot.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1713339773/pulumi_vault/raft_snapshot_agent_config.py` & `pulumi_vault-6.2.0a1713561465/pulumi_vault/raft_snapshot_agent_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -1115,35 +1115,37 @@
 
         ### Local Storage
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_vault as vault
 
-        local_backups = vault.RaftSnapshotAgentConfig("localBackups",
+        local_backups = vault.RaftSnapshotAgentConfig("local_backups",
+            name="local",
             interval_seconds=86400,
-            local_max_space=10000000,
-            path_prefix="/opt/vault/snapshots/",
             retain=7,
-            storage_type="local")
+            path_prefix="/opt/vault/snapshots/",
+            storage_type="local",
+            local_max_space=10000000)
         ```
         <!--End PulumiCodeChooser -->
 
         ### AWS S3
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_aws as aws
         import pulumi_vault as vault
 
         config = pulumi.Config()
         aws_access_key_id = config.require_object("awsAccessKeyId")
         aws_secret_access_key = config.require_object("awsSecretAccessKey")
         current = aws.get_region()
-        s3_backups = vault.RaftSnapshotAgentConfig("s3Backups",
+        s3_backups = vault.RaftSnapshotAgentConfig("s3_backups",
+            name="s3",
             interval_seconds=86400,
             retain=7,
             path_prefix="/path/in/bucket",
             storage_type="aws-s3",
             aws_s3_bucket="my-bucket",
             aws_s3_region=current.name,
             aws_access_key_id=aws_access_key_id,
@@ -1158,15 +1160,16 @@
         ```python
         import pulumi
         import pulumi_vault as vault
 
         config = pulumi.Config()
         azure_account_name = config.require_object("azureAccountName")
         azure_account_key = config.require_object("azureAccountKey")
-        azure_backups = vault.RaftSnapshotAgentConfig("azureBackups",
+        azure_backups = vault.RaftSnapshotAgentConfig("azure_backups",
+            name="azure_backup",
             interval_seconds=86400,
             retain=7,
             path_prefix="/",
             storage_type="azure-blob",
             azure_container_name="vault-blob",
             azure_account_name=azure_account_name,
             azure_account_key=azure_account_key)
@@ -1262,35 +1265,37 @@
 
         ### Local Storage
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_vault as vault
 
-        local_backups = vault.RaftSnapshotAgentConfig("localBackups",
+        local_backups = vault.RaftSnapshotAgentConfig("local_backups",
+            name="local",
             interval_seconds=86400,
-            local_max_space=10000000,
-            path_prefix="/opt/vault/snapshots/",
             retain=7,
-            storage_type="local")
+            path_prefix="/opt/vault/snapshots/",
+            storage_type="local",
+            local_max_space=10000000)
         ```
         <!--End PulumiCodeChooser -->
 
         ### AWS S3
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_aws as aws
         import pulumi_vault as vault
 
         config = pulumi.Config()
         aws_access_key_id = config.require_object("awsAccessKeyId")
         aws_secret_access_key = config.require_object("awsSecretAccessKey")
         current = aws.get_region()
-        s3_backups = vault.RaftSnapshotAgentConfig("s3Backups",
+        s3_backups = vault.RaftSnapshotAgentConfig("s3_backups",
+            name="s3",
             interval_seconds=86400,
             retain=7,
             path_prefix="/path/in/bucket",
             storage_type="aws-s3",
             aws_s3_bucket="my-bucket",
             aws_s3_region=current.name,
             aws_access_key_id=aws_access_key_id,
@@ -1305,15 +1310,16 @@
         ```python
         import pulumi
         import pulumi_vault as vault
 
         config = pulumi.Config()
         azure_account_name = config.require_object("azureAccountName")
         azure_account_key = config.require_object("azureAccountKey")
-        azure_backups = vault.RaftSnapshotAgentConfig("azureBackups",
+        azure_backups = vault.RaftSnapshotAgentConfig("azure_backups",
+            name="azure_backup",
             interval_seconds=86400,
             retain=7,
             path_prefix="/",
             storage_type="azure-blob",
             azure_container_name="vault-blob",
             azure_account_name=azure_account_name,
             azure_account_key=azure_account_key)
```

### Comparing `pulumi_vault-6.2.0a1713339773/pulumi_vault/rgp_policy.py` & `pulumi_vault-6.2.0a1713561465/pulumi_vault/rgp_policy.py`

 * *Files 1% similar despite different names*

```diff
@@ -184,19 +184,19 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_vault as vault
 
         allow_all = vault.RgpPolicy("allow-all",
+            name="allow-all",
             enforcement_level="soft-mandatory",
             policy=\"\"\"main = rule {
           true
         }
-
         \"\"\")
         ```
         <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] enforcement_level: Enforcement level of Sentinel policy. Can be either `advisory` or `soft-mandatory` or `hard-mandatory`
@@ -222,19 +222,19 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_vault as vault
 
         allow_all = vault.RgpPolicy("allow-all",
+            name="allow-all",
             enforcement_level="soft-mandatory",
             policy=\"\"\"main = rule {
           true
         }
-
         \"\"\")
         ```
         <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param RgpPolicyArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
```

### Comparing `pulumi_vault-6.2.0a1713339773/pulumi_vault/saml/auth_backend.py` & `pulumi_vault-6.2.0a1713561465/pulumi_vault/saml/auth_backend.py`

 * *Files 0% similar despite different names*

```diff
@@ -447,19 +447,19 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_vault as vault
 
         test = vault.saml.AuthBackend("test",
-            acs_urls=["https://my.vault.primary/v1/auth/saml/callback"],
-            default_role="admin",
-            entity_id="https://my.vault/v1/auth/saml",
+            path="saml",
             idp_metadata_url="https://company.okta.com/app/abc123eb9xnIfzlaf697/sso/saml/metadata",
-            path="saml")
+            entity_id="https://my.vault/v1/auth/saml",
+            acs_urls=["https://my.vault.primary/v1/auth/saml/callback"],
+            default_role="admin")
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
 
         SAML authentication mounts can be imported using the `path`, e.g.
 
@@ -507,19 +507,19 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_vault as vault
 
         test = vault.saml.AuthBackend("test",
-            acs_urls=["https://my.vault.primary/v1/auth/saml/callback"],
-            default_role="admin",
-            entity_id="https://my.vault/v1/auth/saml",
+            path="saml",
             idp_metadata_url="https://company.okta.com/app/abc123eb9xnIfzlaf697/sso/saml/metadata",
-            path="saml")
+            entity_id="https://my.vault/v1/auth/saml",
+            acs_urls=["https://my.vault.primary/v1/auth/saml/callback"],
+            default_role="admin")
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
 
         SAML authentication mounts can be imported using the `path`, e.g.
```

### Comparing `pulumi_vault-6.2.0a1713339773/pulumi_vault/saml/auth_backend_role.py` & `pulumi_vault-6.2.0a1713561465/pulumi_vault/saml/auth_backend_role.py`

 * *Files 1% similar despite different names*

```diff
@@ -689,22 +689,23 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_vault as vault
 
-        example_auth_backend = vault.saml.AuthBackend("exampleAuthBackend",
+        example = vault.saml.AuthBackend("example",
             path="saml",
             idp_metadata_url="https://company.okta.com/app/abc123eb9xnIfzlaf697/sso/saml/metadata",
             entity_id="https://my.vault/v1/auth/saml",
             acs_urls=["https://my.vault.primary/v1/auth/saml/callback"],
             default_role="default-role")
-        example_auth_backend_role = vault.saml.AuthBackendRole("exampleAuthBackendRole",
-            path=example_auth_backend.path,
+        example_auth_backend_role = vault.saml.AuthBackendRole("example",
+            path=example.path,
+            name="my-role",
             groups_attribute="groups",
             bound_attributes={
                 "group": "admin",
             },
             bound_subjects=["*example.com"],
             token_policies=["writer"],
             token_ttl=86400)
@@ -775,22 +776,23 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_vault as vault
 
-        example_auth_backend = vault.saml.AuthBackend("exampleAuthBackend",
+        example = vault.saml.AuthBackend("example",
             path="saml",
             idp_metadata_url="https://company.okta.com/app/abc123eb9xnIfzlaf697/sso/saml/metadata",
             entity_id="https://my.vault/v1/auth/saml",
             acs_urls=["https://my.vault.primary/v1/auth/saml/callback"],
             default_role="default-role")
-        example_auth_backend_role = vault.saml.AuthBackendRole("exampleAuthBackendRole",
-            path=example_auth_backend.path,
+        example_auth_backend_role = vault.saml.AuthBackendRole("example",
+            path=example.path,
+            name="my-role",
             groups_attribute="groups",
             bound_attributes={
                 "group": "admin",
             },
             bound_subjects=["*example.com"],
             token_policies=["writer"],
             token_ttl=86400)
```

### Comparing `pulumi_vault-6.2.0a1713339773/pulumi_vault/secrets/__init__.py` & `pulumi_vault-6.2.0a1713561465/pulumi_vault/secrets/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1713339773/pulumi_vault/secrets/_inputs.py` & `pulumi_vault-6.2.0a1713561465/pulumi_vault/secrets/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1713339773/pulumi_vault/secrets/outputs.py` & `pulumi_vault-6.2.0a1713561465/pulumi_vault/secrets/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1713339773/pulumi_vault/secrets/sync_association.py` & `pulumi_vault-6.2.0a1713561465/pulumi_vault/secrets/sync_association.py`

 * *Files 2% similar despite different names*

```diff
@@ -235,24 +235,27 @@
             type="kv",
             options={
                 "version": "2",
             },
             description="KV Version 2 secret engine mount")
         token = vault.kv.SecretV2("token",
             mount=kvv2.path,
+            name="token",
             data_json=json.dumps({
                 "dev": "B!gS3cr3t",
                 "prod": "S3cureP4$$",
             }))
         gh = vault.secrets.SyncGhDestination("gh",
-            access_token=var["access_token"],
-            repository_owner=var["repo_owner"],
+            name="gh-dest",
+            access_token=access_token,
+            repository_owner=repo_owner,
             repository_name="repo-name-example",
             secret_name_template="vault_{{ .MountAccessor | lowercase }}_{{ .SecretPath | lowercase }}")
-        gh_token = vault.secrets.SyncAssociation("ghToken",
+        gh_token = vault.secrets.SyncAssociation("gh_token",
+            name=gh.name,
             type=gh.type,
             mount=kvv2.path,
             secret_name=token.name)
         ```
         <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
@@ -285,24 +288,27 @@
             type="kv",
             options={
                 "version": "2",
             },
             description="KV Version 2 secret engine mount")
         token = vault.kv.SecretV2("token",
             mount=kvv2.path,
+            name="token",
             data_json=json.dumps({
                 "dev": "B!gS3cr3t",
                 "prod": "S3cureP4$$",
             }))
         gh = vault.secrets.SyncGhDestination("gh",
-            access_token=var["access_token"],
-            repository_owner=var["repo_owner"],
+            name="gh-dest",
+            access_token=access_token,
+            repository_owner=repo_owner,
             repository_name="repo-name-example",
             secret_name_template="vault_{{ .MountAccessor | lowercase }}_{{ .SecretPath | lowercase }}")
-        gh_token = vault.secrets.SyncAssociation("ghToken",
+        gh_token = vault.secrets.SyncAssociation("gh_token",
+            name=gh.name,
             type=gh.type,
             mount=kvv2.path,
             secret_name=token.name)
         ```
         <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
```

### Comparing `pulumi_vault-6.2.0a1713339773/pulumi_vault/secrets/sync_aws_destination.py` & `pulumi_vault-6.2.0a1713561465/pulumi_vault/secrets/sync_aws_destination.py`

 * *Files 0% similar despite different names*

```diff
@@ -456,16 +456,17 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_vault as vault
 
         aws = vault.secrets.SyncAwsDestination("aws",
-            access_key_id=var["access_key_id"],
-            secret_access_key=var["secret_access_key"],
+            name="aws-dest",
+            access_key_id=access_key_id,
+            secret_access_key=secret_access_key,
             region="us-east-1",
             role_arn="role-arn",
             external_id="external-id",
             secret_name_template="vault_{{ .MountAccessor | lowercase }}_{{ .SecretPath | lowercase }}",
             custom_tags={
                 "foo": "bar",
             })
@@ -522,16 +523,17 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_vault as vault
 
         aws = vault.secrets.SyncAwsDestination("aws",
-            access_key_id=var["access_key_id"],
-            secret_access_key=var["secret_access_key"],
+            name="aws-dest",
+            access_key_id=access_key_id,
+            secret_access_key=secret_access_key,
             region="us-east-1",
             role_arn="role-arn",
             external_id="external-id",
             secret_name_template="vault_{{ .MountAccessor | lowercase }}_{{ .SecretPath | lowercase }}",
             custom_tags={
                 "foo": "bar",
             })
```

### Comparing `pulumi_vault-6.2.0a1713339773/pulumi_vault/secrets/sync_azure_destination.py` & `pulumi_vault-6.2.0a1713561465/pulumi_vault/secrets/sync_azure_destination.py`

 * *Files 2% similar despite different names*

```diff
@@ -432,18 +432,19 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_vault as vault
 
         az = vault.secrets.SyncAzureDestination("az",
-            key_vault_uri=var["key_vault_uri"],
-            client_id=var["client_id"],
-            client_secret=var["client_secret"],
-            tenant_id=var["tenant_id"],
+            name="az-dest",
+            key_vault_uri=key_vault_uri,
+            client_id=client_id,
+            client_secret=client_secret,
+            tenant_id=tenant_id,
             secret_name_template="vault_{{ .MountAccessor | lowercase }}_{{ .SecretPath | lowercase }}",
             custom_tags={
                 "foo": "bar",
             })
         ```
         <!--End PulumiCodeChooser -->
 
@@ -491,18 +492,19 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_vault as vault
 
         az = vault.secrets.SyncAzureDestination("az",
-            key_vault_uri=var["key_vault_uri"],
-            client_id=var["client_id"],
-            client_secret=var["client_secret"],
-            tenant_id=var["tenant_id"],
+            name="az-dest",
+            key_vault_uri=key_vault_uri,
+            client_id=client_id,
+            client_secret=client_secret,
+            tenant_id=tenant_id,
             secret_name_template="vault_{{ .MountAccessor | lowercase }}_{{ .SecretPath | lowercase }}",
             custom_tags={
                 "foo": "bar",
             })
         ```
         <!--End PulumiCodeChooser -->
```

### Comparing `pulumi_vault-6.2.0a1713339773/pulumi_vault/secrets/sync_config.py` & `pulumi_vault-6.2.0a1713561465/pulumi_vault/secrets/sync_config.py`

 * *Files 0% similar despite different names*

```diff
@@ -151,15 +151,15 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_vault as vault
 
-        global_config = vault.secrets.SyncConfig("globalConfig",
+        global_config = vault.secrets.SyncConfig("global_config",
             disabled=True,
             queue_capacity=500000)
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
 
@@ -192,15 +192,15 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_vault as vault
 
-        global_config = vault.secrets.SyncConfig("globalConfig",
+        global_config = vault.secrets.SyncConfig("global_config",
             disabled=True,
             queue_capacity=500000)
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
```

### Comparing `pulumi_vault-6.2.0a1713339773/pulumi_vault/secrets/sync_gcp_destination.py` & `pulumi_vault-6.2.0a1713561465/pulumi_vault/secrets/sync_gcp_destination.py`

 * *Files 1% similar despite different names*

```diff
@@ -318,19 +318,21 @@
                  __props__=None):
         """
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
+        import pulumi_std as std
         import pulumi_vault as vault
 
         gcp = vault.secrets.SyncGcpDestination("gcp",
+            name="gcp-dest",
             project_id="gcp-project-id",
-            credentials=(lambda path: open(path).read())(var["credentials_file"]),
+            credentials=std.file(input=credentials_file).result,
             secret_name_template="vault_{{ .MountAccessor | lowercase }}_{{ .SecretPath | lowercase }}",
             custom_tags={
                 "foo": "bar",
             })
         ```
         <!--End PulumiCodeChooser -->
 
@@ -369,19 +371,21 @@
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
+        import pulumi_std as std
         import pulumi_vault as vault
 
         gcp = vault.secrets.SyncGcpDestination("gcp",
+            name="gcp-dest",
             project_id="gcp-project-id",
-            credentials=(lambda path: open(path).read())(var["credentials_file"]),
+            credentials=std.file(input=credentials_file).result,
             secret_name_template="vault_{{ .MountAccessor | lowercase }}_{{ .SecretPath | lowercase }}",
             custom_tags={
                 "foo": "bar",
             })
         ```
         <!--End PulumiCodeChooser -->
```

### Comparing `pulumi_vault-6.2.0a1713339773/pulumi_vault/secrets/sync_gh_destination.py` & `pulumi_vault-6.2.0a1713561465/pulumi_vault/secrets/sync_gh_destination.py`

 * *Files 0% similar despite different names*

```diff
@@ -403,16 +403,17 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_vault as vault
 
         gh = vault.secrets.SyncGhDestination("gh",
-            access_token=var["access_token"],
-            repository_owner=var["repo_owner"],
+            name="gh-dest",
+            access_token=access_token,
+            repository_owner=repo_owner,
             repository_name="repo-name-example",
             secret_name_template="vault_{{ .MountAccessor | lowercase }}_{{ .SecretPath | lowercase }}")
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
 
@@ -458,16 +459,17 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_vault as vault
 
         gh = vault.secrets.SyncGhDestination("gh",
-            access_token=var["access_token"],
-            repository_owner=var["repo_owner"],
+            name="gh-dest",
+            access_token=access_token,
+            repository_owner=repo_owner,
             repository_name="repo-name-example",
             secret_name_template="vault_{{ .MountAccessor | lowercase }}_{{ .SecretPath | lowercase }}")
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
```

### Comparing `pulumi_vault-6.2.0a1713339773/pulumi_vault/secrets/sync_github_apps.py` & `pulumi_vault-6.2.0a1713561465/pulumi_vault/secrets/sync_github_apps.py`

 * *Files 2% similar despite different names*

```diff
@@ -189,19 +189,21 @@
                  __props__=None):
         """
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
+        import pulumi_std as std
         import pulumi_vault as vault
 
         github_apps = vault.secrets.SyncGithubApps("github-apps",
-            app_id=var["app_id"],
-            private_key=(lambda path: open(path).read())(var["privatekey_file"]))
+            name="gh-apps",
+            app_id=app_id,
+            private_key=std.file(input=privatekey_file).result)
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
 
         GitHub Apps Secrets sync configuration endpoint can be imported using the `name`, e.g.
 
@@ -226,19 +228,21 @@
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
+        import pulumi_std as std
         import pulumi_vault as vault
 
         github_apps = vault.secrets.SyncGithubApps("github-apps",
-            app_id=var["app_id"],
-            private_key=(lambda path: open(path).read())(var["privatekey_file"]))
+            name="gh-apps",
+            app_id=app_id,
+            private_key=std.file(input=privatekey_file).result)
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
 
         GitHub Apps Secrets sync configuration endpoint can be imported using the `name`, e.g.
```

### Comparing `pulumi_vault-6.2.0a1713339773/pulumi_vault/secrets/sync_vercel_destination.py` & `pulumi_vault-6.2.0a1713561465/pulumi_vault/secrets/sync_vercel_destination.py`

 * *Files 1% similar despite different names*

```diff
@@ -339,16 +339,17 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_vault as vault
 
         vercel = vault.secrets.SyncVercelDestination("vercel",
-            access_token=var["access_token"],
-            project_id=var["project_id"],
+            name="vercel-dest",
+            access_token=access_token,
+            project_id=project_id,
             deployment_environments=[
                 "development",
                 "preview",
                 "production",
             ],
             secret_name_template="vault_{{ .MountAccessor | lowercase }}_{{ .SecretPath | lowercase }}")
         ```
@@ -390,16 +391,17 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_vault as vault
 
         vercel = vault.secrets.SyncVercelDestination("vercel",
-            access_token=var["access_token"],
-            project_id=var["project_id"],
+            name="vercel-dest",
+            access_token=access_token,
+            project_id=project_id,
             deployment_environments=[
                 "development",
                 "preview",
                 "production",
             ],
             secret_name_template="vault_{{ .MountAccessor | lowercase }}_{{ .SecretPath | lowercase }}")
         ```
```

### Comparing `pulumi_vault-6.2.0a1713339773/pulumi_vault/ssh/_inputs.py` & `pulumi_vault-6.2.0a1713561465/pulumi_vault/ssh/_inputs.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,20 +21,14 @@
         """
         :param pulumi.Input[Sequence[pulumi.Input[int]]] lengths: A list of allowed key lengths as integers. 
                For key types that do not support setting the length a value of `[0]` should be used.
                Setting multiple lengths is only supported on Vault 1.10+. For prior releases `length`
                must be set to a single element list.
                
                Example configuration blocks that might be included in the `ssh.SecretBackendRole`
-               
-               <!--Start PulumiCodeChooser -->
-               ```python
-               import pulumi
-               ```
-               <!--End PulumiCodeChooser -->
         :param pulumi.Input[str] type: The SSH public key type.  
                *Supported key types are:*
                `rsa`, `ecdsa`, `ec`, `dsa`, `ed25519`, `ssh-rsa`, `ssh-dss`, `ssh-ed25519`,
                `ecdsa-sha2-nistp256`, `ecdsa-sha2-nistp384`, `ecdsa-sha2-nistp521`
         """
         pulumi.set(__self__, "lengths", lengths)
         pulumi.set(__self__, "type", type)
@@ -45,20 +39,14 @@
         """
         A list of allowed key lengths as integers. 
         For key types that do not support setting the length a value of `[0]` should be used.
         Setting multiple lengths is only supported on Vault 1.10+. For prior releases `length`
         must be set to a single element list.
 
         Example configuration blocks that might be included in the `ssh.SecretBackendRole`
-
-        <!--Start PulumiCodeChooser -->
-        ```python
-        import pulumi
-        ```
-        <!--End PulumiCodeChooser -->
         """
         return pulumi.get(self, "lengths")
 
     @lengths.setter
     def lengths(self, value: pulumi.Input[Sequence[pulumi.Input[int]]]):
         pulumi.set(self, "lengths", value)
```

### Comparing `pulumi_vault-6.2.0a1713339773/pulumi_vault/ssh/outputs.py` & `pulumi_vault-6.2.0a1713561465/pulumi_vault/ssh/outputs.py`

 * *Files 13% similar despite different names*

```diff
@@ -21,20 +21,14 @@
         """
         :param Sequence[int] lengths: A list of allowed key lengths as integers. 
                For key types that do not support setting the length a value of `[0]` should be used.
                Setting multiple lengths is only supported on Vault 1.10+. For prior releases `length`
                must be set to a single element list.
                
                Example configuration blocks that might be included in the `ssh.SecretBackendRole`
-               
-               <!--Start PulumiCodeChooser -->
-               ```python
-               import pulumi
-               ```
-               <!--End PulumiCodeChooser -->
         :param str type: The SSH public key type.  
                *Supported key types are:*
                `rsa`, `ecdsa`, `ec`, `dsa`, `ed25519`, `ssh-rsa`, `ssh-dss`, `ssh-ed25519`,
                `ecdsa-sha2-nistp256`, `ecdsa-sha2-nistp384`, `ecdsa-sha2-nistp521`
         """
         pulumi.set(__self__, "lengths", lengths)
         pulumi.set(__self__, "type", type)
@@ -45,20 +39,14 @@
         """
         A list of allowed key lengths as integers. 
         For key types that do not support setting the length a value of `[0]` should be used.
         Setting multiple lengths is only supported on Vault 1.10+. For prior releases `length`
         must be set to a single element list.
 
         Example configuration blocks that might be included in the `ssh.SecretBackendRole`
-
-        <!--Start PulumiCodeChooser -->
-        ```python
-        import pulumi
-        ```
-        <!--End PulumiCodeChooser -->
         """
         return pulumi.get(self, "lengths")
 
     @property
     @pulumi.getter
     def type(self) -> str:
         """
```

### Comparing `pulumi_vault-6.2.0a1713339773/pulumi_vault/ssh/secret_backend_ca.py` & `pulumi_vault-6.2.0a1713561465/pulumi_vault/ssh/secret_backend_ca.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1713339773/pulumi_vault/ssh/secret_backend_role.py` & `pulumi_vault-6.2.0a1713561465/pulumi_vault/ssh/secret_backend_role.py`

 * *Files 0% similar despite different names*

```diff
@@ -924,18 +924,20 @@
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_vault as vault
 
         example = vault.Mount("example", type="ssh")
         foo = vault.ssh.SecretBackendRole("foo",
+            name="my-role",
             backend=example.path,
             key_type="ca",
             allow_user_certificates=True)
         bar = vault.ssh.SecretBackendRole("bar",
+            name="otp-role",
             backend=example.path,
             key_type="otp",
             default_user="default",
             allowed_users="default,baz",
             cidr_list="0.0.0.0/0")
         ```
         <!--End PulumiCodeChooser -->
@@ -998,18 +1000,20 @@
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_vault as vault
 
         example = vault.Mount("example", type="ssh")
         foo = vault.ssh.SecretBackendRole("foo",
+            name="my-role",
             backend=example.path,
             key_type="ca",
             allow_user_certificates=True)
         bar = vault.ssh.SecretBackendRole("bar",
+            name="otp-role",
             backend=example.path,
             key_type="otp",
             default_user="default",
             allowed_users="default,baz",
             cidr_list="0.0.0.0/0")
         ```
         <!--End PulumiCodeChooser -->
```

### Comparing `pulumi_vault-6.2.0a1713339773/pulumi_vault/terraformcloud/secret_backend.py` & `pulumi_vault-6.2.0a1713561465/pulumi_vault/terraformcloud/secret_backend.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1713339773/pulumi_vault/terraformcloud/secret_creds.py` & `pulumi_vault-6.2.0a1713561465/pulumi_vault/terraformcloud/secret_creds.py`

 * *Files 0% similar despite different names*

```diff
@@ -238,14 +238,15 @@
 
         test = vault.terraformcloud.SecretBackend("test",
             backend="terraform",
             description="Manages the Terraform Cloud backend",
             token="V0idfhi2iksSDU234ucdbi2nidsi...")
         example = vault.terraformcloud.SecretRole("example",
             backend=test.backend,
+            name="test-role",
             organization="example-organization-name",
             team_id="team-ieF4isC...")
         token = vault.terraformcloud.SecretCreds("token",
             backend=test.backend,
             role=example.name)
         ```
         <!--End PulumiCodeChooser -->
@@ -275,14 +276,15 @@
 
         test = vault.terraformcloud.SecretBackend("test",
             backend="terraform",
             description="Manages the Terraform Cloud backend",
             token="V0idfhi2iksSDU234ucdbi2nidsi...")
         example = vault.terraformcloud.SecretRole("example",
             backend=test.backend,
+            name="test-role",
             organization="example-organization-name",
             team_id="team-ieF4isC...")
         token = vault.terraformcloud.SecretCreds("token",
             backend=test.backend,
             role=example.name)
         ```
         <!--End PulumiCodeChooser -->
```

### Comparing `pulumi_vault-6.2.0a1713339773/pulumi_vault/terraformcloud/secret_role.py` & `pulumi_vault-6.2.0a1713561465/pulumi_vault/terraformcloud/secret_role.py`

 * *Files 1% similar despite different names*

```diff
@@ -319,14 +319,15 @@
 
         test = vault.terraformcloud.SecretBackend("test",
             backend="terraform",
             description="Manages the Terraform Cloud backend",
             token="V0idfhi2iksSDU234ucdbi2nidsi...")
         example = vault.terraformcloud.SecretRole("example",
             backend=test.backend,
+            name="test-role",
             organization="example-organization-name",
             team_id="team-ieF4isC...")
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
 
@@ -366,14 +367,15 @@
 
         test = vault.terraformcloud.SecretBackend("test",
             backend="terraform",
             description="Manages the Terraform Cloud backend",
             token="V0idfhi2iksSDU234ucdbi2nidsi...")
         example = vault.terraformcloud.SecretRole("example",
             backend=test.backend,
+            name="test-role",
             organization="example-organization-name",
             team_id="team-ieF4isC...")
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
```

### Comparing `pulumi_vault-6.2.0a1713339773/pulumi_vault/token.py` & `pulumi_vault-6.2.0a1713561465/pulumi_vault/token.py`

 * *Files 0% similar despite different names*

```diff
@@ -625,26 +625,26 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_vault as vault
 
         example = vault.Token("example",
-            metadata={
-                "purpose": "service-account",
-            },
+            role_name="app",
             policies=[
                 "policy1",
                 "policy2",
             ],
-            renew_increment=86400,
-            renew_min_lease=43200,
             renewable=True,
-            role_name="app",
-            ttl="24h")
+            ttl="24h",
+            renew_min_lease=43200,
+            renew_increment=86400,
+            metadata={
+                "purpose": "service-account",
+            })
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
 
         Tokens can be imported using its `id` as accessor id, e.g.
 
@@ -684,26 +684,26 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_vault as vault
 
         example = vault.Token("example",
-            metadata={
-                "purpose": "service-account",
-            },
+            role_name="app",
             policies=[
                 "policy1",
                 "policy2",
             ],
-            renew_increment=86400,
-            renew_min_lease=43200,
             renewable=True,
-            role_name="app",
-            ttl="24h")
+            ttl="24h",
+            renew_min_lease=43200,
+            renew_increment=86400,
+            metadata={
+                "purpose": "service-account",
+            })
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
 
         Tokens can be imported using its `id` as accessor id, e.g.
```

### Comparing `pulumi_vault-6.2.0a1713339773/pulumi_vault/tokenauth/auth_backend_role.py` & `pulumi_vault-6.2.0a1713561465/pulumi_vault/tokenauth/auth_backend_role.py`

 * *Files 0% similar despite different names*

```diff
@@ -752,26 +752,26 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_vault as vault
 
         example = vault.tokenauth.AuthBackendRole("example",
-            allowed_entity_aliases=["test_entity"],
+            role_name="my-role",
             allowed_policies=[
                 "dev",
                 "test",
             ],
             disallowed_policies=["default"],
+            allowed_entity_aliases=["test_entity"],
             orphan=True,
-            path_suffix="path-suffix",
+            token_period=86400,
             renewable=True,
-            role_name="my-role",
             token_explicit_max_ttl=115200,
-            token_period=86400)
+            path_suffix="path-suffix")
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
 
         Token auth backend roles can be imported with `auth/token/roles/` followed by the `role_name`, e.g.
 
@@ -837,26 +837,26 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_vault as vault
 
         example = vault.tokenauth.AuthBackendRole("example",
-            allowed_entity_aliases=["test_entity"],
+            role_name="my-role",
             allowed_policies=[
                 "dev",
                 "test",
             ],
             disallowed_policies=["default"],
+            allowed_entity_aliases=["test_entity"],
             orphan=True,
-            path_suffix="path-suffix",
+            token_period=86400,
             renewable=True,
-            role_name="my-role",
             token_explicit_max_ttl=115200,
-            token_period=86400)
+            path_suffix="path-suffix")
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
 
         Token auth backend roles can be imported with `auth/token/roles/` followed by the `role_name`, e.g.
```

### Comparing `pulumi_vault-6.2.0a1713339773/pulumi_vault/transform/alphabet.py` & `pulumi_vault-6.2.0a1713561465/pulumi_vault/transform/alphabet.py`

 * *Files 1% similar despite different names*

```diff
@@ -184,19 +184,20 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_vault as vault
 
-        mount_transform = vault.Mount("mountTransform",
+        mount_transform = vault.Mount("mount_transform",
             path="transform",
             type="transform")
         test = vault.transform.Alphabet("test",
             path=mount_transform.path,
+            name="numerics",
             alphabet="0123456789")
         ```
         <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] alphabet: A string of characters that contains the alphabet set.
@@ -221,19 +222,20 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_vault as vault
 
-        mount_transform = vault.Mount("mountTransform",
+        mount_transform = vault.Mount("mount_transform",
             path="transform",
             type="transform")
         test = vault.transform.Alphabet("test",
             path=mount_transform.path,
+            name="numerics",
             alphabet="0123456789")
         ```
         <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param AlphabetArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
```

### Comparing `pulumi_vault-6.2.0a1713339773/pulumi_vault/transform/get_decode.py` & `pulumi_vault-6.2.0a1713561465/pulumi_vault/transform/get_decode.py`

 * *Files 1% similar despite different names*

```diff
@@ -148,20 +148,22 @@
     import pulumi_vault as vault
 
     transform = vault.Mount("transform",
         path="transform",
         type="transform")
     ccn_fpe = vault.transform.Transformation("ccn-fpe",
         path=transform.path,
+        name="ccn-fpe",
         type="fpe",
         template="builtin/creditcardnumber",
         tweak_source="internal",
         allowed_roles=["payments"])
     payments = vault.transform.Role("payments",
         path=ccn_fpe.path,
+        name="payments",
         transformations=["ccn-fpe"])
     test = vault.transform.get_decode_output(path=payments.path,
         role_name="payments",
         value="9300-3376-4943-8903")
     ```
     <!--End PulumiCodeChooser -->
 
@@ -229,20 +231,22 @@
     import pulumi_vault as vault
 
     transform = vault.Mount("transform",
         path="transform",
         type="transform")
     ccn_fpe = vault.transform.Transformation("ccn-fpe",
         path=transform.path,
+        name="ccn-fpe",
         type="fpe",
         template="builtin/creditcardnumber",
         tweak_source="internal",
         allowed_roles=["payments"])
     payments = vault.transform.Role("payments",
         path=ccn_fpe.path,
+        name="payments",
         transformations=["ccn-fpe"])
     test = vault.transform.get_decode_output(path=payments.path,
         role_name="payments",
         value="9300-3376-4943-8903")
     ```
     <!--End PulumiCodeChooser -->
```

### Comparing `pulumi_vault-6.2.0a1713339773/pulumi_vault/transform/get_encode.py` & `pulumi_vault-6.2.0a1713561465/pulumi_vault/transform/get_encode.py`

 * *Files 1% similar despite different names*

```diff
@@ -148,20 +148,22 @@
     import pulumi_vault as vault
 
     transform = vault.Mount("transform",
         path="transform",
         type="transform")
     ccn_fpe = vault.transform.Transformation("ccn-fpe",
         path=transform.path,
+        name="ccn-fpe",
         type="fpe",
         template="builtin/creditcardnumber",
         tweak_source="internal",
         allowed_roles=["payments"])
     payments = vault.transform.Role("payments",
         path=ccn_fpe.path,
+        name="payments",
         transformations=["ccn-fpe"])
     test = vault.transform.get_encode_output(path=payments.path,
         role_name="payments",
         batch_inputs=[{
             "value": "1111-2222-3333-4444",
         }])
     ```
@@ -231,20 +233,22 @@
     import pulumi_vault as vault
 
     transform = vault.Mount("transform",
         path="transform",
         type="transform")
     ccn_fpe = vault.transform.Transformation("ccn-fpe",
         path=transform.path,
+        name="ccn-fpe",
         type="fpe",
         template="builtin/creditcardnumber",
         tweak_source="internal",
         allowed_roles=["payments"])
     payments = vault.transform.Role("payments",
         path=ccn_fpe.path,
+        name="payments",
         transformations=["ccn-fpe"])
     test = vault.transform.get_encode_output(path=payments.path,
         role_name="payments",
         batch_inputs=[{
             "value": "1111-2222-3333-4444",
         }])
     ```
```

### Comparing `pulumi_vault-6.2.0a1713339773/pulumi_vault/transform/role.py` & `pulumi_vault-6.2.0a1713561465/pulumi_vault/transform/role.py`

 * *Files 1% similar despite different names*

```diff
@@ -185,19 +185,20 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_vault as vault
 
-        mount_transform = vault.Mount("mountTransform",
+        mount_transform = vault.Mount("mount_transform",
             path="transform",
             type="transform")
         test = vault.transform.Role("test",
             path=mount_transform.path,
+            name="payments",
             transformations=["ccn-fpe"])
         ```
         <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] name: The name of the role.
@@ -223,19 +224,20 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_vault as vault
 
-        mount_transform = vault.Mount("mountTransform",
+        mount_transform = vault.Mount("mount_transform",
             path="transform",
             type="transform")
         test = vault.transform.Role("test",
             path=mount_transform.path,
+            name="payments",
             transformations=["ccn-fpe"])
         ```
         <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param RoleArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
```

### Comparing `pulumi_vault-6.2.0a1713339773/pulumi_vault/transform/template.py` & `pulumi_vault-6.2.0a1713561465/pulumi_vault/transform/template.py`

 * *Files 2% similar despite different names*

```diff
@@ -340,17 +340,19 @@
         import pulumi_vault as vault
 
         transform = vault.Mount("transform",
             path="transform",
             type="transform")
         numerics = vault.transform.Alphabet("numerics",
             path=transform.path,
+            name="numerics",
             alphabet="0123456789")
         test = vault.transform.Template("test",
             path=numerics.path,
+            name="ccn",
             type="regex",
             pattern="(\\\\d{4})[- ](\\\\d{4})[- ](\\\\d{4})[- ](\\\\d{4})",
             alphabet="numerics",
             encode_format="$1-$2-$3-$4",
             decode_formats={
                 "last-four-digits": "$4",
             })
@@ -403,17 +405,19 @@
         import pulumi_vault as vault
 
         transform = vault.Mount("transform",
             path="transform",
             type="transform")
         numerics = vault.transform.Alphabet("numerics",
             path=transform.path,
+            name="numerics",
             alphabet="0123456789")
         test = vault.transform.Template("test",
             path=numerics.path,
+            name="ccn",
             type="regex",
             pattern="(\\\\d{4})[- ](\\\\d{4})[- ](\\\\d{4})[- ](\\\\d{4})",
             alphabet="numerics",
             encode_format="$1-$2-$3-$4",
             decode_formats={
                 "last-four-digits": "$4",
             })
```

### Comparing `pulumi_vault-6.2.0a1713339773/pulumi_vault/transform/transformation.py` & `pulumi_vault-6.2.0a1713561465/pulumi_vault/transform/transformation.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1713339773/pulumi_vault/transit/get_decrypt.py` & `pulumi_vault-6.2.0a1713561465/pulumi_vault/transit/get_decrypt.py`

 * *Files 0% similar despite different names*

```diff
@@ -114,16 +114,16 @@
 
     <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_vault as vault
 
     test = vault.transit.get_decrypt(backend="transit",
-        ciphertext="vault:v1:S3GtnJ5GUNCWV+/pdL9+g1Feu/nzAv+RlmTmE91Tu0rBkeIU8MEb2nSspC/1IQ==",
-        key="test")
+        key="test",
+        ciphertext="vault:v1:S3GtnJ5GUNCWV+/pdL9+g1Feu/nzAv+RlmTmE91Tu0rBkeIU8MEb2nSspC/1IQ==")
     ```
     <!--End PulumiCodeChooser -->
 
 
     :param str backend: The path the transit secret backend is mounted at, with no leading or trailing `/`.
     :param str ciphertext: Ciphertext to be decoded.
     :param str context: Context for key derivation. This is required if key derivation is enabled for this key.
@@ -162,16 +162,16 @@
 
     <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_vault as vault
 
     test = vault.transit.get_decrypt(backend="transit",
-        ciphertext="vault:v1:S3GtnJ5GUNCWV+/pdL9+g1Feu/nzAv+RlmTmE91Tu0rBkeIU8MEb2nSspC/1IQ==",
-        key="test")
+        key="test",
+        ciphertext="vault:v1:S3GtnJ5GUNCWV+/pdL9+g1Feu/nzAv+RlmTmE91Tu0rBkeIU8MEb2nSspC/1IQ==")
     ```
     <!--End PulumiCodeChooser -->
 
 
     :param str backend: The path the transit secret backend is mounted at, with no leading or trailing `/`.
     :param str ciphertext: Ciphertext to be decoded.
     :param str context: Context for key derivation. This is required if key derivation is enabled for this key.
```

### Comparing `pulumi_vault-6.2.0a1713339773/pulumi_vault/transit/get_encrypt.py` & `pulumi_vault-6.2.0a1713561465/pulumi_vault/transit/get_encrypt.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1713339773/pulumi_vault/transit/secret_backend_key.py` & `pulumi_vault-6.2.0a1713561465/pulumi_vault/transit/secret_backend_key.py`

 * *Files 0% similar despite different names*

```diff
@@ -613,15 +613,17 @@
 
         transit = vault.Mount("transit",
             path="transit",
             type="transit",
             description="Example description",
             default_lease_ttl_seconds=3600,
             max_lease_ttl_seconds=86400)
-        key = vault.transit.SecretBackendKey("key", backend=transit.path)
+        key = vault.transit.SecretBackendKey("key",
+            backend=transit.path,
+            name="my_key")
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
 
         Transit secret backend keys can be imported using the `path`, e.g.
 
@@ -669,15 +671,17 @@
 
         transit = vault.Mount("transit",
             path="transit",
             type="transit",
             description="Example description",
             default_lease_ttl_seconds=3600,
             max_lease_ttl_seconds=86400)
-        key = vault.transit.SecretBackendKey("key", backend=transit.path)
+        key = vault.transit.SecretBackendKey("key",
+            backend=transit.path,
+            name="my_key")
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
 
         Transit secret backend keys can be imported using the `path`, e.g.
```

### Comparing `pulumi_vault-6.2.0a1713339773/pulumi_vault/transit/secret_cache_config.py` & `pulumi_vault-6.2.0a1713561465/pulumi_vault/transit/secret_cache_config.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1713339773/pulumi_vault.egg-info/PKG-INFO` & `pulumi_vault-6.2.0a1713561465/pulumi_vault.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_vault
-Version: 6.2.0a1713339773
+Version: 6.2.0a1713561465
 Summary: A Pulumi package for creating and managing HashiCorp Vault cloud resources.
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.io
 Project-URL: Repository, https://github.com/pulumi/pulumi-vault
 Keywords: pulumi,vault
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_vault-6.2.0a1713339773/pulumi_vault.egg-info/SOURCES.txt` & `pulumi_vault-6.2.0a1713561465/pulumi_vault.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_vault-6.2.0a1713339773/pyproject.toml` & `pulumi_vault-6.2.0a1713561465/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [project]
   name = "pulumi_vault"
   description = "A Pulumi package for creating and managing HashiCorp Vault cloud resources."
   dependencies = ["parver>=0.2.1", "pulumi>=3.0.0,<4.0.0", "semver>=2.8.1"]
   keywords = ["pulumi", "vault"]
   readme = "README.md"
   requires-python = ">=3.8"
-  version = "6.2.0a1713339773"
+  version = "6.2.0a1713561465"
   [project.license]
     text = "Apache-2.0"
   [project.urls]
     Homepage = "https://pulumi.io"
     Repository = "https://github.com/pulumi/pulumi-vault"
 
 [build-system]
```

