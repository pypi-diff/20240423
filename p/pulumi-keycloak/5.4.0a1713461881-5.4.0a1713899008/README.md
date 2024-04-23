# Comparing `tmp/pulumi_keycloak-5.4.0a1713461881.tar.gz` & `tmp/pulumi_keycloak-5.4.0a1713899008.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_keycloak-5.4.0a1713461881.tar", last modified: Thu Apr 18 17:41:39 2024, max compression
+gzip compressed data, was "pulumi_keycloak-5.4.0a1713899008.tar", last modified: Tue Apr 23 19:37:01 2024, max compression
```

## Comparing `pulumi_keycloak-5.4.0a1713461881.tar` & `pulumi_keycloak-5.4.0a1713899008.tar`

### file list

```diff
@@ -1,142 +1,142 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 17:41:39.297069 pulumi_keycloak-5.4.0a1713461881/
--rw-r--r--   0 runner    (1001) docker     (127)     4393 2024-04-18 17:41:39.297069 pulumi_keycloak-5.4.0a1713461881/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3933 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 17:41:39.281069 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/
--rw-r--r--   0 runner    (1001) docker     (127)    20942 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    91136 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)    22242 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/attribute_importer_identity_provider_mapper.py
--rw-r--r--   0 runner    (1001) docker     (127)    28002 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/attribute_to_role_identity_mapper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 17:41:39.281069 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/authentication/
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/authentication/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24684 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/authentication/bindings.py
--rw-r--r--   0 runner    (1001) docker     (127)    16915 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/authentication/execution.py
--rw-r--r--   0 runner    (1001) docker     (127)    15662 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/authentication/execution_config.py
--rw-r--r--   0 runner    (1001) docker     (127)    15266 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/authentication/flow.py
--rw-r--r--   0 runner    (1001) docker     (127)    23414 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/authentication/subflow.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 17:41:39.281069 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/config/
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/config/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2631 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (127)    19118 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/custom_identity_provider_mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)    28593 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/custom_user_federation.py
--rw-r--r--   0 runner    (1001) docker     (127)     8836 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/default_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)    10273 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/default_roles.py
--rw-r--r--   0 runner    (1001) docker     (127)    22695 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/generic_client_protocol_mapper.py
--rw-r--r--   0 runner    (1001) docker     (127)    23725 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/generic_client_role_mapper.py
--rw-r--r--   0 runner    (1001) docker     (127)    24138 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/generic_protocol_mapper.py
--rw-r--r--   0 runner    (1001) docker     (127)    23287 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/generic_role_mapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     5858 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/get_authentication_execution.py
--rw-r--r--   0 runner    (1001) docker     (127)     4203 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/get_authentication_flow.py
--rw-r--r--   0 runner    (1001) docker     (127)    26780 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/get_client_description_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     4243 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/get_group.py
--rw-r--r--   0 runner    (1001) docker     (127)    38724 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/get_realm.py
--rw-r--r--   0 runner    (1001) docker     (127)     4624 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/get_realm_keys.py
--rw-r--r--   0 runner    (1001) docker     (127)     4978 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/get_role.py
--rw-r--r--   0 runner    (1001) docker     (127)     8282 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/get_user.py
--rw-r--r--   0 runner    (1001) docker     (127)     5285 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/get_user_realm_roles.py
--rw-r--r--   0 runner    (1001) docker     (127)    14199 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/group.py
--rw-r--r--   0 runner    (1001) docker     (127)    11789 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/group_memberships.py
--rw-r--r--   0 runner    (1001) docker     (127)    20301 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/group_permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)    14053 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/group_roles.py
--rw-r--r--   0 runner    (1001) docker     (127)    20514 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/hardcoded_attribute_identity_provider_mapper.py
--rw-r--r--   0 runner    (1001) docker     (127)    15800 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/hardcoded_role_identity_mapper.py
--rw-r--r--   0 runner    (1001) docker     (127)    24704 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/identity_provider_token_exchange_scope_permission.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 17:41:39.285069 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/ldap/
--rw-r--r--   0 runner    (1001) docker     (127)      715 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/ldap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6465 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/ldap/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    21281 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/ldap/custom_mapper.py
--rw-r--r--   0 runner    (1001) docker     (127)    19383 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/ldap/full_name_mapper.py
--rw-r--r--   0 runner    (1001) docker     (127)    45150 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/ldap/group_mapper.py
--rw-r--r--   0 runner    (1001) docker     (127)    18755 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/ldap/hardcoded_attribute_mapper.py
--rw-r--r--   0 runner    (1001) docker     (127)    15933 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/ldap/hardcoded_group_mapper.py
--rw-r--r--   0 runner    (1001) docker     (127)    15688 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/ldap/hardcoded_role_mapper.py
--rw-r--r--   0 runner    (1001) docker     (127)    14664 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/ldap/msad_lds_user_account_control_mapper.py
--rw-r--r--   0 runner    (1001) docker     (127)    17302 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/ldap/msad_user_account_control_mapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     6467 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/ldap/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    46827 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/ldap/role_mapper.py
--rw-r--r--   0 runner    (1001) docker     (127)    32560 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/ldap/user_attribute_mapper.py
--rw-r--r--   0 runner    (1001) docker     (127)    89338 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/ldap/user_federation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 17:41:39.285069 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/oidc/
--rw-r--r--   0 runner    (1001) docker     (127)      342 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/oidc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    70182 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/oidc/google_identity_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)    82528 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/oidc/identity_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 17:41:39.293069 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/openid/
--rw-r--r--   0 runner    (1001) docker     (127)     1680 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/openid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16629 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/openid/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    29119 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/openid/audience_protocol_mapper.py
--rw-r--r--   0 runner    (1001) docker     (127)    18744 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/openid/audience_resolve_protocol_mapper.py
--rw-r--r--   0 runner    (1001) docker     (127)    19279 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/openid/audience_resolve_protocol_mappter.py
--rw-r--r--   0 runner    (1001) docker     (127)    90769 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/openid/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    13673 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/openid/client_aggregate_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)    18810 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/openid/client_authorization_permission.py
--rw-r--r--   0 runner    (1001) docker     (127)    17909 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/openid/client_authorization_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)    10842 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/openid/client_authorization_scope.py
--rw-r--r--   0 runner    (1001) docker     (127)    11230 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/openid/client_default_scopes.py
--rw-r--r--   0 runner    (1001) docker     (127)    15292 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/openid/client_group_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)    14315 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/openid/client_js_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)    11287 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/openid/client_optional_scopes.py
--rw-r--r--   0 runner    (1001) docker     (127)    24772 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/openid/client_permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)    22120 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/openid/client_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)    14933 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/openid/client_role_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)    15773 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/openid/client_scope.py
--rw-r--r--   0 runner    (1001) docker     (127)    13597 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/openid/client_service_account_realm_role.py
--rw-r--r--   0 runner    (1001) docker     (127)    16204 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/openid/client_service_account_role.py
--rw-r--r--   0 runner    (1001) docker     (127)    27525 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/openid/client_time_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)    13479 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/openid/client_user_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)    23154 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/openid/full_name_protocol_mapper.py
--rw-r--r--   0 runner    (1001) docker     (127)    31487 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/openid/get_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    12158 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/openid/get_client_authorization_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)     6363 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/openid/get_client_scope.py
--rw-r--r--   0 runner    (1001) docker     (127)    10323 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/openid/get_client_service_account_user.py
--rw-r--r--   0 runner    (1001) docker     (127)    26636 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/openid/group_membership_protocol_mapper.py
--rw-r--r--   0 runner    (1001) docker     (127)    31401 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/openid/hardcoded_claim_protocol_mapper.py
--rw-r--r--   0 runner    (1001) docker     (127)    19804 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/openid/hardcoded_role_protocol_mapper.py
--rw-r--r--   0 runner    (1001) docker     (127)    20335 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/openid/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    35520 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/openid/script_protocol_mapper.py
--rw-r--r--   0 runner    (1001) docker     (127)    36474 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/openid/user_attribute_protocol_mapper.py
--rw-r--r--   0 runner    (1001) docker     (127)    39329 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/openid/user_client_role_protocol_mapper.py
--rw-r--r--   0 runner    (1001) docker     (127)    31502 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/openid/user_property_protocol_mapper.py
--rw-r--r--   0 runner    (1001) docker     (127)    34658 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/openid/user_realm_role_protocol_mapper.py
--rw-r--r--   0 runner    (1001) docker     (127)    30939 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/openid/user_session_note_protocol_mapper.py
--rw-r--r--   0 runner    (1001) docker     (127)    82512 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    16755 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)   107528 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/realm.py
--rw-r--r--   0 runner    (1001) docker     (127)    19093 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/realm_events.py
--rw-r--r--   0 runner    (1001) docker     (127)    18452 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/realm_keystore_aes_generated.py
--rw-r--r--   0 runner    (1001) docker     (127)    17705 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/realm_keystore_ecdsa_generated.py
--rw-r--r--   0 runner    (1001) docker     (127)    19426 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/realm_keystore_hmac_generated.py
--rw-r--r--   0 runner    (1001) docker     (127)    25332 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/realm_keystore_java_generated.py
--rw-r--r--   0 runner    (1001) docker     (127)    22162 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/realm_keystore_rsa.py
--rw-r--r--   0 runner    (1001) docker     (127)    19223 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/realm_keystore_rsa_generated.py
--rw-r--r--   0 runner    (1001) docker     (127)    18252 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/realm_user_profile.py
--rw-r--r--   0 runner    (1001) docker     (127)    17424 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/required_action.py
--rw-r--r--   0 runner    (1001) docker     (127)    19448 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/role.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 17:41:39.293069 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/saml/
--rw-r--r--   0 runner    (1001) docker     (127)      636 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/saml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1457 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/saml/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    63709 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/saml/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    10682 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/saml/client_default_scope.py
--rw-r--r--   0 runner    (1001) docker     (127)    17029 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/saml/client_scope.py
--rw-r--r--   0 runner    (1001) docker     (127)    24405 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/saml/get_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     5376 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/saml/get_client_installation_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)   101076 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/saml/identity_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     2476 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/saml/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    28553 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/saml/script_protocol_mapper.py
--rw-r--r--   0 runner    (1001) docker     (127)    20758 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/saml/user_attribute_protocol_mapper.py
--rw-r--r--   0 runner    (1001) docker     (127)    20651 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/saml/user_property_protocol_mapper.py
--rw-r--r--   0 runner    (1001) docker     (127)    24618 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/user.py
--rw-r--r--   0 runner    (1001) docker     (127)    14644 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/user_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)    17054 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/user_roles.py
--rw-r--r--   0 runner    (1001) docker     (127)    20447 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/user_template_importer_identity_provider_mapper.py
--rw-r--r--   0 runner    (1001) docker     (127)    21446 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/users_permissions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 17:41:39.297069 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4393 2024-04-18 17:41:39.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5570 2024-04-18 17:41:39.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 17:41:39.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-18 17:41:39.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-18 17:41:39.000000 pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      689 2024-04-18 17:41:32.000000 pulumi_keycloak-5.4.0a1713461881/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 17:41:39.297069 pulumi_keycloak-5.4.0a1713461881/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:37:01.822273 pulumi_keycloak-5.4.0a1713899008/
+-rw-r--r--   0 runner    (1001) docker     (127)     4393 2024-04-23 19:37:01.822273 pulumi_keycloak-5.4.0a1713899008/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3933 2024-04-23 19:36:55.000000 pulumi_keycloak-5.4.0a1713899008/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:37:01.806273 pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/
+-rw-r--r--   0 runner    (1001) docker     (127)    20942 2024-04-23 19:36:55.000000 pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    87704 2024-04-23 19:36:55.000000 pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-04-23 19:36:55.000000 pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22086 2024-04-23 19:36:55.000000 pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/attribute_importer_identity_provider_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27846 2024-04-23 19:36:55.000000 pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/attribute_to_role_identity_mapper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:37:01.810273 pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/authentication/
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-04-23 19:36:55.000000 pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/authentication/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24528 2024-04-23 19:36:55.000000 pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/authentication/bindings.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16759 2024-04-23 19:36:55.000000 pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/authentication/execution.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15506 2024-04-23 19:36:55.000000 pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/authentication/execution_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15110 2024-04-23 19:36:55.000000 pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/authentication/flow.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23258 2024-04-23 19:36:55.000000 pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/authentication/subflow.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:37:01.810273 pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-23 19:36:55.000000 pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-04-23 19:36:55.000000 pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/config/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2631 2024-04-23 19:36:55.000000 pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18962 2024-04-23 19:36:55.000000 pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/custom_identity_provider_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28437 2024-04-23 19:36:55.000000 pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/custom_user_federation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8680 2024-04-23 19:36:55.000000 pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/default_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10117 2024-04-23 19:36:55.000000 pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/default_roles.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22539 2024-04-23 19:36:55.000000 pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/generic_client_protocol_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23101 2024-04-23 19:36:55.000000 pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/generic_client_role_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23982 2024-04-23 19:36:55.000000 pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/generic_protocol_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22663 2024-04-23 19:36:55.000000 pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/generic_role_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5718 2024-04-23 19:36:55.000000 pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/get_authentication_execution.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4063 2024-04-23 19:36:55.000000 pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/get_authentication_flow.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27392 2024-04-23 19:36:55.000000 pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/get_client_description_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4243 2024-04-23 19:36:55.000000 pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/get_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38584 2024-04-23 19:36:55.000000 pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/get_realm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4624 2024-04-23 19:36:55.000000 pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/get_realm_keys.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4978 2024-04-23 19:36:55.000000 pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/get_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8142 2024-04-23 19:36:55.000000 pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/get_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5145 2024-04-23 19:36:55.000000 pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/get_user_realm_roles.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14043 2024-04-23 19:36:55.000000 pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/group.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11633 2024-04-23 19:36:55.000000 pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/group_memberships.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20301 2024-04-23 19:36:55.000000 pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/group_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13897 2024-04-23 19:36:55.000000 pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/group_roles.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20358 2024-04-23 19:36:55.000000 pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/hardcoded_attribute_identity_provider_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15644 2024-04-23 19:36:55.000000 pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/hardcoded_role_identity_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24548 2024-04-23 19:36:55.000000 pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/identity_provider_token_exchange_scope_permission.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:37:01.814273 pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/ldap/
+-rw-r--r--   0 runner    (1001) docker     (127)      715 2024-04-23 19:36:55.000000 pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/ldap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6465 2024-04-23 19:36:55.000000 pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/ldap/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21125 2024-04-23 19:36:55.000000 pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/ldap/custom_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19227 2024-04-23 19:36:55.000000 pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/ldap/full_name_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44994 2024-04-23 19:36:55.000000 pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/ldap/group_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18599 2024-04-23 19:36:55.000000 pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/ldap/hardcoded_attribute_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15777 2024-04-23 19:36:55.000000 pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/ldap/hardcoded_group_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15532 2024-04-23 19:36:55.000000 pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/ldap/hardcoded_role_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14508 2024-04-23 19:36:55.000000 pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/ldap/msad_lds_user_account_control_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17146 2024-04-23 19:36:55.000000 pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/ldap/msad_user_account_control_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6467 2024-04-23 19:36:55.000000 pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/ldap/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46671 2024-04-23 19:36:55.000000 pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/ldap/role_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32404 2024-04-23 19:36:55.000000 pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/ldap/user_attribute_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    89182 2024-04-23 19:36:55.000000 pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/ldap/user_federation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:37:01.814273 pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/oidc/
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-04-23 19:36:55.000000 pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/oidc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    70026 2024-04-23 19:36:55.000000 pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/oidc/google_identity_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)    82372 2024-04-23 19:36:55.000000 pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/oidc/identity_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:37:01.822273 pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/openid/
+-rw-r--r--   0 runner    (1001) docker     (127)     1680 2024-04-23 19:36:55.000000 pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/openid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16629 2024-04-23 19:36:55.000000 pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/openid/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28807 2024-04-23 19:36:55.000000 pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/openid/audience_protocol_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18432 2024-04-23 19:36:55.000000 pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/openid/audience_resolve_protocol_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18967 2024-04-23 19:36:55.000000 pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/openid/audience_resolve_protocol_mappter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    90613 2024-04-23 19:36:55.000000 pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/openid/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13673 2024-04-23 19:36:55.000000 pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/openid/client_aggregate_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18810 2024-04-23 19:36:55.000000 pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/openid/client_authorization_permission.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17909 2024-04-23 19:36:55.000000 pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/openid/client_authorization_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10842 2024-04-23 19:36:55.000000 pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/openid/client_authorization_scope.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11074 2024-04-23 19:36:55.000000 pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/openid/client_default_scopes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15292 2024-04-23 19:36:55.000000 pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/openid/client_group_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14315 2024-04-23 19:36:55.000000 pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/openid/client_js_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11131 2024-04-23 19:36:55.000000 pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/openid/client_optional_scopes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24772 2024-04-23 19:36:55.000000 pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/openid/client_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21964 2024-04-23 19:36:55.000000 pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/openid/client_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14933 2024-04-23 19:36:55.000000 pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/openid/client_role_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15617 2024-04-23 19:36:55.000000 pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/openid/client_scope.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13441 2024-04-23 19:36:55.000000 pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/openid/client_service_account_realm_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16048 2024-04-23 19:36:55.000000 pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/openid/client_service_account_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27525 2024-04-23 19:36:55.000000 pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/openid/client_time_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13479 2024-04-23 19:36:55.000000 pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/openid/client_user_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22842 2024-04-23 19:36:55.000000 pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/openid/full_name_protocol_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31347 2024-04-23 19:36:55.000000 pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/openid/get_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12018 2024-04-23 19:36:55.000000 pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/openid/get_client_authorization_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6223 2024-04-23 19:36:55.000000 pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/openid/get_client_scope.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10183 2024-04-23 19:36:55.000000 pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/openid/get_client_service_account_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26324 2024-04-23 19:36:55.000000 pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/openid/group_membership_protocol_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31089 2024-04-23 19:36:55.000000 pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/openid/hardcoded_claim_protocol_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19492 2024-04-23 19:36:55.000000 pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/openid/hardcoded_role_protocol_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20335 2024-04-23 19:36:55.000000 pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/openid/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35208 2024-04-23 19:36:55.000000 pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/openid/script_protocol_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36162 2024-04-23 19:36:55.000000 pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/openid/user_attribute_protocol_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39017 2024-04-23 19:36:55.000000 pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/openid/user_client_role_protocol_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31190 2024-04-23 19:36:55.000000 pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/openid/user_property_protocol_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34346 2024-04-23 19:36:55.000000 pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/openid/user_realm_role_protocol_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30627 2024-04-23 19:36:55.000000 pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/openid/user_session_note_protocol_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    79430 2024-04-23 19:36:55.000000 pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16755 2024-04-23 19:36:55.000000 pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-23 19:36:55.000000 pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 19:36:55.000000 pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)   107528 2024-04-23 19:36:55.000000 pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/realm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18937 2024-04-23 19:36:55.000000 pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/realm_events.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18296 2024-04-23 19:36:55.000000 pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/realm_keystore_aes_generated.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17549 2024-04-23 19:36:55.000000 pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/realm_keystore_ecdsa_generated.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19270 2024-04-23 19:36:55.000000 pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/realm_keystore_hmac_generated.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25176 2024-04-23 19:36:55.000000 pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/realm_keystore_java_generated.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22162 2024-04-23 19:36:55.000000 pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/realm_keystore_rsa.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19067 2024-04-23 19:36:55.000000 pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/realm_keystore_rsa_generated.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18096 2024-04-23 19:36:55.000000 pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/realm_user_profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17268 2024-04-23 19:36:55.000000 pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/required_action.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18980 2024-04-23 19:36:55.000000 pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/role.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:37:01.822273 pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/saml/
+-rw-r--r--   0 runner    (1001) docker     (127)      636 2024-04-23 19:36:55.000000 pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/saml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1457 2024-04-23 19:36:55.000000 pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/saml/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    63709 2024-04-23 19:36:55.000000 pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/saml/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10682 2024-04-23 19:36:55.000000 pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/saml/client_default_scope.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16873 2024-04-23 19:36:55.000000 pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/saml/client_scope.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24265 2024-04-23 19:36:55.000000 pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/saml/get_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5376 2024-04-23 19:36:55.000000 pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/saml/get_client_installation_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)   100920 2024-04-23 19:36:55.000000 pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/saml/identity_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2476 2024-04-23 19:36:55.000000 pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/saml/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28397 2024-04-23 19:36:55.000000 pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/saml/script_protocol_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20602 2024-04-23 19:36:55.000000 pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/saml/user_attribute_protocol_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20495 2024-04-23 19:36:55.000000 pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/saml/user_property_protocol_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24462 2024-04-23 19:36:55.000000 pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14488 2024-04-23 19:36:55.000000 pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/user_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16898 2024-04-23 19:36:55.000000 pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/user_roles.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20291 2024-04-23 19:36:55.000000 pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/user_template_importer_identity_provider_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21446 2024-04-23 19:36:55.000000 pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/users_permissions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:37:01.822273 pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4393 2024-04-23 19:37:01.000000 pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5570 2024-04-23 19:37:01.000000 pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 19:37:01.000000 pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-23 19:37:01.000000 pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-23 19:37:01.000000 pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      689 2024-04-23 19:36:55.000000 pulumi_keycloak-5.4.0a1713899008/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 19:37:01.822273 pulumi_keycloak-5.4.0a1713899008/setup.cfg
```

### Comparing `pulumi_keycloak-5.4.0a1713461881/PKG-INFO` & `pulumi_keycloak-5.4.0a1713899008/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_keycloak
-Version: 5.4.0a1713461881
+Version: 5.4.0a1713899008
 Summary: A Pulumi package for creating and managing keycloak cloud resources.
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.io
 Project-URL: Repository, https://github.com/pulumi/pulumi-keycloak
 Keywords: pulumi,keycloak
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_keycloak-5.4.0a1713461881/README.md` & `pulumi_keycloak-5.4.0a1713899008/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/__init__.py` & `pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/_inputs.py` & `pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/_inputs.py`

 * *Files 4% similar despite different names*

```diff
@@ -744,23 +744,15 @@
                  enabled_when_scopes: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  group: Optional[pulumi.Input[str]] = None,
                  permissions: Optional[pulumi.Input['RealmUserProfileAttributePermissionsArgs']] = None,
                  required_for_roles: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  required_for_scopes: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  validators: Optional[pulumi.Input[Sequence[pulumi.Input['RealmUserProfileAttributeValidatorArgs']]]] = None):
         """
-        :param pulumi.Input[str] name: The name of the attribute.
-        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] annotations: A map of annotations for the attribute. Values can be a String or a json object.
-        :param pulumi.Input[str] display_name: The display name of the attribute.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] enabled_when_scopes: A list of scopes. The attribute will only be enabled when these scopes are requested by clients.
         :param pulumi.Input[str] group: A list of groups.
-        :param pulumi.Input['RealmUserProfileAttributePermissionsArgs'] permissions: The permissions configuration information.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] required_for_roles: A list of roles for which the attribute will be required.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] required_for_scopes: A list of scopes for which the attribute will be required.
-        :param pulumi.Input[Sequence[pulumi.Input['RealmUserProfileAttributeValidatorArgs']]] validators: A list of validators for the attribute.
         """
         pulumi.set(__self__, "name", name)
         if annotations is not None:
             pulumi.set(__self__, "annotations", annotations)
         if display_name is not None:
             pulumi.set(__self__, "display_name", display_name)
         if enabled_when_scopes is not None:
@@ -775,53 +767,41 @@
             pulumi.set(__self__, "required_for_scopes", required_for_scopes)
         if validators is not None:
             pulumi.set(__self__, "validators", validators)
 
     @property
     @pulumi.getter
     def name(self) -> pulumi.Input[str]:
-        """
-        The name of the attribute.
-        """
         return pulumi.get(self, "name")
 
     @name.setter
     def name(self, value: pulumi.Input[str]):
         pulumi.set(self, "name", value)
 
     @property
     @pulumi.getter
     def annotations(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
-        """
-        A map of annotations for the attribute. Values can be a String or a json object.
-        """
         return pulumi.get(self, "annotations")
 
     @annotations.setter
     def annotations(self, value: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]):
         pulumi.set(self, "annotations", value)
 
     @property
     @pulumi.getter(name="displayName")
     def display_name(self) -> Optional[pulumi.Input[str]]:
-        """
-        The display name of the attribute.
-        """
         return pulumi.get(self, "display_name")
 
     @display_name.setter
     def display_name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "display_name", value)
 
     @property
     @pulumi.getter(name="enabledWhenScopes")
     def enabled_when_scopes(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
-        """
-        A list of scopes. The attribute will only be enabled when these scopes are requested by clients.
-        """
         return pulumi.get(self, "enabled_when_scopes")
 
     @enabled_when_scopes.setter
     def enabled_when_scopes(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "enabled_when_scopes", value)
 
     @property
@@ -835,198 +815,148 @@
     @group.setter
     def group(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "group", value)
 
     @property
     @pulumi.getter
     def permissions(self) -> Optional[pulumi.Input['RealmUserProfileAttributePermissionsArgs']]:
-        """
-        The permissions configuration information.
-        """
         return pulumi.get(self, "permissions")
 
     @permissions.setter
     def permissions(self, value: Optional[pulumi.Input['RealmUserProfileAttributePermissionsArgs']]):
         pulumi.set(self, "permissions", value)
 
     @property
     @pulumi.getter(name="requiredForRoles")
     def required_for_roles(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
-        """
-        A list of roles for which the attribute will be required.
-        """
         return pulumi.get(self, "required_for_roles")
 
     @required_for_roles.setter
     def required_for_roles(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "required_for_roles", value)
 
     @property
     @pulumi.getter(name="requiredForScopes")
     def required_for_scopes(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
-        """
-        A list of scopes for which the attribute will be required.
-        """
         return pulumi.get(self, "required_for_scopes")
 
     @required_for_scopes.setter
     def required_for_scopes(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "required_for_scopes", value)
 
     @property
     @pulumi.getter
     def validators(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['RealmUserProfileAttributeValidatorArgs']]]]:
-        """
-        A list of validators for the attribute.
-        """
         return pulumi.get(self, "validators")
 
     @validators.setter
     def validators(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['RealmUserProfileAttributeValidatorArgs']]]]):
         pulumi.set(self, "validators", value)
 
 
 @pulumi.input_type
 class RealmUserProfileAttributePermissionsArgs:
     def __init__(__self__, *,
                  edits: pulumi.Input[Sequence[pulumi.Input[str]]],
                  views: pulumi.Input[Sequence[pulumi.Input[str]]]):
-        """
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] edits: A list of profiles that will be able to edit the attribute. One of `admin`, `user`.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] views: A list of profiles that will be able to view the attribute. One of `admin`, `user`.
-        """
         pulumi.set(__self__, "edits", edits)
         pulumi.set(__self__, "views", views)
 
     @property
     @pulumi.getter
     def edits(self) -> pulumi.Input[Sequence[pulumi.Input[str]]]:
-        """
-        A list of profiles that will be able to edit the attribute. One of `admin`, `user`.
-        """
         return pulumi.get(self, "edits")
 
     @edits.setter
     def edits(self, value: pulumi.Input[Sequence[pulumi.Input[str]]]):
         pulumi.set(self, "edits", value)
 
     @property
     @pulumi.getter
     def views(self) -> pulumi.Input[Sequence[pulumi.Input[str]]]:
-        """
-        A list of profiles that will be able to view the attribute. One of `admin`, `user`.
-        """
         return pulumi.get(self, "views")
 
     @views.setter
     def views(self, value: pulumi.Input[Sequence[pulumi.Input[str]]]):
         pulumi.set(self, "views", value)
 
 
 @pulumi.input_type
 class RealmUserProfileAttributeValidatorArgs:
     def __init__(__self__, *,
                  name: pulumi.Input[str],
                  config: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None):
-        """
-        :param pulumi.Input[str] name: The name of the attribute.
-        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] config: A map defining the configuration of the validator. Values can be a String or a json object.
-        """
         pulumi.set(__self__, "name", name)
         if config is not None:
             pulumi.set(__self__, "config", config)
 
     @property
     @pulumi.getter
     def name(self) -> pulumi.Input[str]:
-        """
-        The name of the attribute.
-        """
         return pulumi.get(self, "name")
 
     @name.setter
     def name(self, value: pulumi.Input[str]):
         pulumi.set(self, "name", value)
 
     @property
     @pulumi.getter
     def config(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
-        """
-        A map defining the configuration of the validator. Values can be a String or a json object.
-        """
         return pulumi.get(self, "config")
 
     @config.setter
     def config(self, value: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]):
         pulumi.set(self, "config", value)
 
 
 @pulumi.input_type
 class RealmUserProfileGroupArgs:
     def __init__(__self__, *,
                  name: pulumi.Input[str],
                  annotations: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  display_description: Optional[pulumi.Input[str]] = None,
                  display_header: Optional[pulumi.Input[str]] = None):
-        """
-        :param pulumi.Input[str] name: The name of the attribute.
-        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] annotations: A map of annotations for the attribute. Values can be a String or a json object.
-        :param pulumi.Input[str] display_description: The display description of the group.
-        :param pulumi.Input[str] display_header: The display header of the group.
-        """
         pulumi.set(__self__, "name", name)
         if annotations is not None:
             pulumi.set(__self__, "annotations", annotations)
         if display_description is not None:
             pulumi.set(__self__, "display_description", display_description)
         if display_header is not None:
             pulumi.set(__self__, "display_header", display_header)
 
     @property
     @pulumi.getter
     def name(self) -> pulumi.Input[str]:
-        """
-        The name of the attribute.
-        """
         return pulumi.get(self, "name")
 
     @name.setter
     def name(self, value: pulumi.Input[str]):
         pulumi.set(self, "name", value)
 
     @property
     @pulumi.getter
     def annotations(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
-        """
-        A map of annotations for the attribute. Values can be a String or a json object.
-        """
         return pulumi.get(self, "annotations")
 
     @annotations.setter
     def annotations(self, value: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]):
         pulumi.set(self, "annotations", value)
 
     @property
     @pulumi.getter(name="displayDescription")
     def display_description(self) -> Optional[pulumi.Input[str]]:
-        """
-        The display description of the group.
-        """
         return pulumi.get(self, "display_description")
 
     @display_description.setter
     def display_description(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "display_description", value)
 
     @property
     @pulumi.getter(name="displayHeader")
     def display_header(self) -> Optional[pulumi.Input[str]]:
-        """
-        The display header of the group.
-        """
         return pulumi.get(self, "display_header")
 
     @display_header.setter
     def display_header(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "display_header", value)
```

### Comparing `pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/_utilities.py` & `pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/attribute_importer_identity_provider_mapper.py` & `pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/attribute_importer_identity_provider_mapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -289,27 +289,25 @@
         """
         ## # AttributeImporterIdentityProviderMapper
 
         Allows to create and manage identity provider mappers within Keycloak.
 
         ### Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         test_mapper = keycloak.AttributeImporterIdentityProviderMapper("test_mapper",
             realm="my-realm",
             name="my-mapper",
             identity_provider_alias="idp_alias",
             attribute_name="http://schemas.xmlsoap.org/ws/2005/05/identity/claims/surname",
             user_attribute="lastName")
         ```
-        <!--End PulumiCodeChooser -->
 
         ### Argument Reference
 
         The following arguments are supported:
 
         - `realm` - (Required) The name of the realm.
         - `name` - (Required) The name of the mapper.
@@ -345,27 +343,25 @@
         """
         ## # AttributeImporterIdentityProviderMapper
 
         Allows to create and manage identity provider mappers within Keycloak.
 
         ### Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         test_mapper = keycloak.AttributeImporterIdentityProviderMapper("test_mapper",
             realm="my-realm",
             name="my-mapper",
             identity_provider_alias="idp_alias",
             attribute_name="http://schemas.xmlsoap.org/ws/2005/05/identity/claims/surname",
             user_attribute="lastName")
         ```
-        <!--End PulumiCodeChooser -->
 
         ### Argument Reference
 
         The following arguments are supported:
 
         - `realm` - (Required) The name of the realm.
         - `name` - (Required) The name of the mapper.
```

### Comparing `pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/attribute_to_role_identity_mapper.py` & `pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/attribute_to_role_identity_mapper.py`

 * *Files 0% similar despite different names*

```diff
@@ -363,15 +363,14 @@
         """
         Allows for creating and managing an attribute to role identity provider mapper within Keycloak.
 
         > If you are using Keycloak 10 or higher, you will need to specify the `extra_config` argument in order to define a `syncMode` for the mapper.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
             realm="my-realm",
             enabled=True)
@@ -394,15 +393,14 @@
             role="my-realm-role",
             claim_name="my-claim",
             claim_value="my-value",
             extra_config={
                 "syncMode": "INHERIT",
             })
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Identity provider mappers can be imported using the format `{{realm_id}}/{{idp_alias}}/{{idp_mapper_id}}`, where `idp_alias` is the identity provider alias, and `idp_mapper_id` is the unique ID that Keycloak
 
         assigns to the mapper upon creation. This value can be found in the URI when editing this mapper in the GUI, and is typically a GUID.
 
@@ -436,15 +434,14 @@
         """
         Allows for creating and managing an attribute to role identity provider mapper within Keycloak.
 
         > If you are using Keycloak 10 or higher, you will need to specify the `extra_config` argument in order to define a `syncMode` for the mapper.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
             realm="my-realm",
             enabled=True)
@@ -467,15 +464,14 @@
             role="my-realm-role",
             claim_name="my-claim",
             claim_value="my-value",
             extra_config={
                 "syncMode": "INHERIT",
             })
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Identity provider mappers can be imported using the format `{{realm_id}}/{{idp_alias}}/{{idp_mapper_id}}`, where `idp_alias` is the identity provider alias, and `idp_mapper_id` is the unique ID that Keycloak
 
         assigns to the mapper upon creation. This value can be found in the URI when editing this mapper in the GUI, and is typically a GUID.
```

### Comparing `pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/authentication/bindings.py` & `pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/authentication/bindings.py`

 * *Files 0% similar despite different names*

```diff
@@ -276,15 +276,14 @@
         Note that you can also use the `Realm` resource to assign authentication flow bindings at the realm level. This
         resource is useful if you would like to create a realm and an authentication flow, and assign this flow to the realm within
         a single run of `pulumi up`. In any case, do not attempt to use both the arguments within the `Realm` resource
         and this resource to manage authentication flow bindings, you should choose one or the other.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
             realm="my-realm",
             enabled=True)
@@ -304,15 +303,14 @@
             authenticator="identity-provider-redirector",
             requirement="ALTERNATIVE",
             opts=pulumi.ResourceOptions(depends_on=[execution_one]))
         browser_authentication_binding = keycloak.authentication.Bindings("browser_authentication_binding",
             realm_id=realm.id,
             browser_flow=flow.alias)
         ```
-        <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] browser_flow: The alias of the flow to assign to the realm BrowserFlow.
         :param pulumi.Input[str] client_authentication_flow: The alias of the flow to assign to the realm ClientAuthenticationFlow.
         :param pulumi.Input[str] direct_grant_flow: The alias of the flow to assign to the realm DirectGrantFlow.
         :param pulumi.Input[str] docker_authentication_flow: The alias of the flow to assign to the realm DockerAuthenticationFlow.
@@ -339,15 +337,14 @@
         Note that you can also use the `Realm` resource to assign authentication flow bindings at the realm level. This
         resource is useful if you would like to create a realm and an authentication flow, and assign this flow to the realm within
         a single run of `pulumi up`. In any case, do not attempt to use both the arguments within the `Realm` resource
         and this resource to manage authentication flow bindings, you should choose one or the other.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
             realm="my-realm",
             enabled=True)
@@ -367,15 +364,14 @@
             authenticator="identity-provider-redirector",
             requirement="ALTERNATIVE",
             opts=pulumi.ResourceOptions(depends_on=[execution_one]))
         browser_authentication_binding = keycloak.authentication.Bindings("browser_authentication_binding",
             realm_id=realm.id,
             browser_flow=flow.alias)
         ```
-        <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param BindingsArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
```

### Comparing `pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/authentication/execution.py` & `pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/authentication/execution.py`

 * *Files 2% similar despite different names*

```diff
@@ -168,15 +168,14 @@
         An authentication execution is an action that the user or service may or may not take when authenticating through an authentication
         flow.
 
         > Due to limitations in the Keycloak API, the ordering of authentication executions within a flow must be specified using `depends_on`. Authentication executions that are created first will appear first within the flow.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
             realm="my-realm",
             enabled=True)
@@ -193,15 +192,14 @@
         execution_two = keycloak.authentication.Execution("execution_two",
             realm_id=realm.id,
             parent_flow_alias=flow.alias,
             authenticator="identity-provider-redirector",
             requirement="ALTERNATIVE",
             opts=pulumi.ResourceOptions(depends_on=[execution_one]))
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Authentication executions can be imported using the formats: `{{realmId}}/{{parentFlowAlias}}/{{authenticationExecutionId}}`.
 
         Example:
 
@@ -230,15 +228,14 @@
         An authentication execution is an action that the user or service may or may not take when authenticating through an authentication
         flow.
 
         > Due to limitations in the Keycloak API, the ordering of authentication executions within a flow must be specified using `depends_on`. Authentication executions that are created first will appear first within the flow.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
             realm="my-realm",
             enabled=True)
@@ -255,15 +252,14 @@
         execution_two = keycloak.authentication.Execution("execution_two",
             realm_id=realm.id,
             parent_flow_alias=flow.alias,
             authenticator="identity-provider-redirector",
             requirement="ALTERNATIVE",
             opts=pulumi.ResourceOptions(depends_on=[execution_one]))
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Authentication executions can be imported using the formats: `{{realmId}}/{{parentFlowAlias}}/{{authenticationExecutionId}}`.
 
         Example:
```

### Comparing `pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/authentication/execution_config.py` & `pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/authentication/execution_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -163,15 +163,14 @@
                  __props__=None):
         """
         Allows for managing an authentication execution's configuration. If a particular authentication execution supports additional
         configuration (such as with the `identity-provider-redirector` execution), this can be managed with this resource.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
             realm="my-realm",
             enabled=True)
@@ -186,15 +185,14 @@
             realm_id=realm.id,
             execution_id=execution.id,
             alias="my-config-alias",
             config={
                 "defaultProvider": "my-config-default-idp",
             })
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Configurations can be imported using the format `{{realm}}/{{authenticationExecutionId}}/{{authenticationExecutionConfigId}}`.
 
         If the `authenticationExecutionId` is incorrect, the import will still be successful.
 
@@ -223,15 +221,14 @@
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         Allows for managing an authentication execution's configuration. If a particular authentication execution supports additional
         configuration (such as with the `identity-provider-redirector` execution), this can be managed with this resource.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
             realm="my-realm",
             enabled=True)
@@ -246,15 +243,14 @@
             realm_id=realm.id,
             execution_id=execution.id,
             alias="my-config-alias",
             config={
                 "defaultProvider": "my-config-default-idp",
             })
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Configurations can be imported using the format `{{realm}}/{{authenticationExecutionId}}/{{authenticationExecutionConfigId}}`.
 
         If the `authenticationExecutionId` is incorrect, the import will still be successful.
```

### Comparing `pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/authentication/flow.py` & `pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/authentication/flow.py`

 * *Files 2% similar despite different names*

```diff
@@ -168,15 +168,14 @@
 
         [Authentication flows](https://www.keycloak.org/docs/11.0/server_admin/index.html#_authentication-flows) describe a sequence
         of actions that a user or service must perform in order to be authenticated to Keycloak. The authentication flow itself
         is a container for these actions, which are otherwise known as executions.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
             realm="my-realm",
             enabled=True)
@@ -185,15 +184,14 @@
             alias="my-flow-alias")
         execution = keycloak.authentication.Execution("execution",
             realm_id=realm.id,
             parent_flow_alias=flow.alias,
             authenticator="identity-provider-redirector",
             requirement="REQUIRED")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Authentication flows can be imported using the format `{{realmId}}/{{authenticationFlowId}}`. The authentication flow ID is
 
         typically a GUID which is autogenerated when the flow is created via Keycloak.
 
@@ -229,15 +227,14 @@
 
         [Authentication flows](https://www.keycloak.org/docs/11.0/server_admin/index.html#_authentication-flows) describe a sequence
         of actions that a user or service must perform in order to be authenticated to Keycloak. The authentication flow itself
         is a container for these actions, which are otherwise known as executions.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
             realm="my-realm",
             enabled=True)
@@ -246,15 +243,14 @@
             alias="my-flow-alias")
         execution = keycloak.authentication.Execution("execution",
             realm_id=realm.id,
             parent_flow_alias=flow.alias,
             authenticator="identity-provider-redirector",
             requirement="REQUIRED")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Authentication flows can be imported using the format `{{realmId}}/{{authenticationFlowId}}`. The authentication flow ID is
 
         typically a GUID which is autogenerated when the flow is created via Keycloak.
```

### Comparing `pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/authentication/subflow.py` & `pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/authentication/subflow.py`

 * *Files 2% similar despite different names*

```diff
@@ -277,15 +277,14 @@
         Allows for creating and managing an authentication subflow within Keycloak.
 
         Like authentication flows, authentication subflows are containers for authentication executions.
         As its name implies, an authentication subflow is contained in an authentication flow.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
             realm="my-realm",
             enabled=True)
@@ -295,15 +294,14 @@
         subflow = keycloak.authentication.Subflow("subflow",
             realm_id=realm.id,
             alias="my-subflow-alias",
             parent_flow_alias=flow.alias,
             provider_id="basic-flow",
             requirement="ALTERNATIVE")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Authentication flows can be imported using the format `{{realmId}}/{{parentFlowAlias}}/{{authenticationSubflowId}}`.
 
         The authentication subflow ID is typically a GUID which is autogenerated when the subflow is created via Keycloak.
 
@@ -346,15 +344,14 @@
         Allows for creating and managing an authentication subflow within Keycloak.
 
         Like authentication flows, authentication subflows are containers for authentication executions.
         As its name implies, an authentication subflow is contained in an authentication flow.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
             realm="my-realm",
             enabled=True)
@@ -364,15 +361,14 @@
         subflow = keycloak.authentication.Subflow("subflow",
             realm_id=realm.id,
             alias="my-subflow-alias",
             parent_flow_alias=flow.alias,
             provider_id="basic-flow",
             requirement="ALTERNATIVE")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Authentication flows can be imported using the format `{{realmId}}/{{parentFlowAlias}}/{{authenticationSubflowId}}`.
 
         The authentication subflow ID is typically a GUID which is autogenerated when the subflow is created via Keycloak.
```

### Comparing `pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/config/__init__.pyi` & `pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/config/__init__.pyi`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/config/vars.py` & `pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/custom_identity_provider_mapping.py` & `pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/custom_identity_provider_mapping.py`

 * *Files 1% similar despite different names*

```diff
@@ -194,15 +194,14 @@
                  identity_provider_mapper: Optional[pulumi.Input[str]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  realm: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
             realm="my-realm",
             enabled=True)
@@ -221,15 +220,14 @@
             identity_provider_mapper="%s-user-attribute-idp-mapper",
             extra_config={
                 "syncMode": "INHERIT",
                 "Claim": "my-email-claim",
                 "UserAttribute": "email",
             })
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Identity provider mappers can be imported using the format `{{realm_id}}/{{idp_alias}}/{{idp_mapper_id}}`, where `idp_alias` is the identity provider alias, and `idp_mapper_id` is the unique ID that Keycloak
 
         assigns to the mapper upon creation. This value can be found in the URI when editing this mapper in the GUI, and is typically a GUID.
 
@@ -254,15 +252,14 @@
     def __init__(__self__,
                  resource_name: str,
                  args: CustomIdentityProviderMappingArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
             realm="my-realm",
             enabled=True)
@@ -281,15 +278,14 @@
             identity_provider_mapper="%s-user-attribute-idp-mapper",
             extra_config={
                 "syncMode": "INHERIT",
                 "Claim": "my-email-claim",
                 "UserAttribute": "email",
             })
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Identity provider mappers can be imported using the format `{{realm_id}}/{{idp_alias}}/{{idp_mapper_id}}`, where `idp_alias` is the identity provider alias, and `idp_mapper_id` is the unique ID that Keycloak
 
         assigns to the mapper upon creation. This value can be found in the URI when editing this mapper in the GUI, and is typically a GUID.
```

### Comparing `pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/custom_user_federation.py` & `pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/custom_user_federation.py`

 * *Files 1% similar despite different names*

```diff
@@ -360,29 +360,27 @@
 
         A custom user federation provider is an implementation of Keycloak's
         [User Storage SPI](https://www.keycloak.org/docs/4.2/server_development/index.html#_user-storage-spi).
         An example of this implementation can be found here.
 
         ### Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
             realm="test",
             enabled=True)
         custom_user_federation = keycloak.CustomUserFederation("custom_user_federation",
             name="custom",
             realm_id=realm.id,
             provider_id="custom",
             enabled=True)
         ```
-        <!--End PulumiCodeChooser -->
 
         ### Argument Reference
 
         The following arguments are supported:
 
         - `realm_id` - (Required) The realm that this provider will provide user federation for.
         - `name` - (Required) Display name of the provider when displayed in the console.
@@ -422,29 +420,27 @@
 
         A custom user federation provider is an implementation of Keycloak's
         [User Storage SPI](https://www.keycloak.org/docs/4.2/server_development/index.html#_user-storage-spi).
         An example of this implementation can be found here.
 
         ### Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
             realm="test",
             enabled=True)
         custom_user_federation = keycloak.CustomUserFederation("custom_user_federation",
             name="custom",
             realm_id=realm.id,
             provider_id="custom",
             enabled=True)
         ```
-        <!--End PulumiCodeChooser -->
 
         ### Argument Reference
 
         The following arguments are supported:
 
         - `realm_id` - (Required) The realm that this provider will provide user federation for.
         - `name` - (Required) Display name of the provider when displayed in the console.
```

### Comparing `pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/default_groups.py` & `pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/default_groups.py`

 * *Files 5% similar despite different names*

```diff
@@ -87,30 +87,28 @@
         Allows for managing a realm's default groups.
 
         Note that you should not use `DefaultGroups` with a group with memberships managed
         by `GroupMemberships`.
 
         ### Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
             realm="my-realm",
             enabled=True)
         group = keycloak.Group("group",
             realm_id=realm.id,
             name="my-group")
         default = keycloak.DefaultGroups("default",
             realm_id=realm.id,
             group_ids=[group.id])
         ```
-        <!--End PulumiCodeChooser -->
 
         ### Argument Reference
 
         The following arguments are supported:
 
         - `realm_id` - (Required) The realm this group exists in.
         - `group_ids` - (Required) A set of group ids that should be default groups on the realm referenced by `realm_id`.
@@ -136,30 +134,28 @@
         Allows for managing a realm's default groups.
 
         Note that you should not use `DefaultGroups` with a group with memberships managed
         by `GroupMemberships`.
 
         ### Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
             realm="my-realm",
             enabled=True)
         group = keycloak.Group("group",
             realm_id=realm.id,
             name="my-group")
         default = keycloak.DefaultGroups("default",
             realm_id=realm.id,
             group_ids=[group.id])
         ```
-        <!--End PulumiCodeChooser -->
 
         ### Argument Reference
 
         The following arguments are supported:
 
         - `realm_id` - (Required) The realm this group exists in.
         - `group_ids` - (Required) A set of group ids that should be default groups on the realm referenced by `realm_id`.
```

### Comparing `pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/default_roles.py` & `pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/default_roles.py`

 * *Files 1% similar despite different names*

```diff
@@ -102,27 +102,25 @@
 
         Note: This feature was added in Keycloak v13, so this resource will not work on older versions of Keycloak.
 
         ## Example Usage
 
         ### Realm Role)
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
             realm="my-realm",
             enabled=True)
         default_roles = keycloak.DefaultRoles("default_roles",
             realm_id=realm.id,
             default_roles=["uma_authorization"])
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Default roles can be imported using the format `{{realm_id}}/{{default_role_id}}`, where `default_role_id` is the unique ID of the composite
 
         role that Keycloak uses to control default realm level roles. The ID is not easy to find in the GUI, but it appears in the dev tools when editing
 
@@ -152,27 +150,25 @@
 
         Note: This feature was added in Keycloak v13, so this resource will not work on older versions of Keycloak.
 
         ## Example Usage
 
         ### Realm Role)
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
             realm="my-realm",
             enabled=True)
         default_roles = keycloak.DefaultRoles("default_roles",
             realm_id=realm.id,
             default_roles=["uma_authorization"])
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Default roles can be imported using the format `{{realm_id}}/{{default_role_id}}`, where `default_role_id` is the unique ID of the composite
 
         role that Keycloak uses to control default realm level roles. The ID is not easy to find in the GUI, but it appears in the dev tools when editing
```

### Comparing `pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/generic_client_protocol_mapper.py` & `pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/generic_client_protocol_mapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -262,15 +262,14 @@
         * If the provider doesn't support a particular protocol mapper, this resource can be used instead.
 
         Due to the generic nature of this mapper, it is less user-friendly and more prone to configuration errors.
         Therefore, if possible, a specific mapper should be used.
 
         ### Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
             realm="my-realm",
             enabled=True)
@@ -286,15 +285,14 @@
             config={
                 "attribute.name": "name",
                 "attribute.nameformat": "Basic",
                 "attribute.value": "value",
                 "friendly.name": "display name",
             })
         ```
-        <!--End PulumiCodeChooser -->
 
         ### Argument Reference
 
         The following arguments are supported:
 
         - `realm_id` - (Required) The realm this protocol mapper exists within.
         - `client_id` - (Required) The client this protocol mapper is attached to.
@@ -335,15 +333,14 @@
         * If the provider doesn't support a particular protocol mapper, this resource can be used instead.
 
         Due to the generic nature of this mapper, it is less user-friendly and more prone to configuration errors.
         Therefore, if possible, a specific mapper should be used.
 
         ### Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
             realm="my-realm",
             enabled=True)
@@ -359,15 +356,14 @@
             config={
                 "attribute.name": "name",
                 "attribute.nameformat": "Basic",
                 "attribute.value": "value",
                 "friendly.name": "display name",
             })
         ```
-        <!--End PulumiCodeChooser -->
 
         ### Argument Reference
 
         The following arguments are supported:
 
         - `realm_id` - (Required) The realm this protocol mapper exists within.
         - `client_id` - (Required) The client this protocol mapper is attached to.
```

### Comparing `pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/generic_client_role_mapper.py` & `pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/generic_client_role_mapper.py`

 * *Files 10% similar despite different names*

```diff
@@ -172,15 +172,14 @@
         `full_scope_allowed` is set to `false` for a client, role scope mapping allows you to limit the roles that get declared
         inside an access token for a client.
 
         ## Example Usage
 
         ### Realm Role To Client)
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
             realm="my-realm",
             enabled=True)
@@ -195,19 +194,17 @@
             name="my-realm-role",
             description="My Realm Role")
         client_role_mapper = keycloak.GenericClientRoleMapper("client_role_mapper",
             realm_id=realm.id,
             client_id=client.id,
             role_id=realm_role.id)
         ```
-        <!--End PulumiCodeChooser -->
 
         ### Client Role To Client)
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
             realm="my-realm",
             enabled=True)
@@ -235,19 +232,17 @@
             name="my-client-role",
             description="My Client Role")
         client_b_role_mapper = keycloak.GenericClientRoleMapper("client_b_role_mapper",
             realm_id=realm.id,
             client_id=client_b.id,
             role_id=client_role_a.id)
         ```
-        <!--End PulumiCodeChooser -->
 
         ### Realm Role To Client Scope)
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
             realm="my-realm",
             enabled=True)
@@ -259,19 +254,17 @@
             name="my-realm-role",
             description="My Realm Role")
         client_role_mapper = keycloak.GenericClientRoleMapper("client_role_mapper",
             realm_id=realm.id,
             client_scope_id=client_scope.id,
             role_id=realm_role.id)
         ```
-        <!--End PulumiCodeChooser -->
 
         ### Client Role To Client Scope)
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
             realm="my-realm",
             enabled=True)
@@ -290,15 +283,14 @@
             realm_id=realm.id,
             name="my-client-scope")
         client_b_role_mapper = keycloak.GenericClientRoleMapper("client_b_role_mapper",
             realm_id=realm.id,
             client_scope_id=client_scope.id,
             role_id=client_role.id)
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Generic client role mappers can be imported using one of the following two formats:
 
         - When mapping a role to a client, use the format `{{realmId}}/client/{{clientId}}/scope-mappings/{{roleClientId}}/{{roleId}}`
 
@@ -334,15 +326,14 @@
         `full_scope_allowed` is set to `false` for a client, role scope mapping allows you to limit the roles that get declared
         inside an access token for a client.
 
         ## Example Usage
 
         ### Realm Role To Client)
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
             realm="my-realm",
             enabled=True)
@@ -357,19 +348,17 @@
             name="my-realm-role",
             description="My Realm Role")
         client_role_mapper = keycloak.GenericClientRoleMapper("client_role_mapper",
             realm_id=realm.id,
             client_id=client.id,
             role_id=realm_role.id)
         ```
-        <!--End PulumiCodeChooser -->
 
         ### Client Role To Client)
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
             realm="my-realm",
             enabled=True)
@@ -397,19 +386,17 @@
             name="my-client-role",
             description="My Client Role")
         client_b_role_mapper = keycloak.GenericClientRoleMapper("client_b_role_mapper",
             realm_id=realm.id,
             client_id=client_b.id,
             role_id=client_role_a.id)
         ```
-        <!--End PulumiCodeChooser -->
 
         ### Realm Role To Client Scope)
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
             realm="my-realm",
             enabled=True)
@@ -421,19 +408,17 @@
             name="my-realm-role",
             description="My Realm Role")
         client_role_mapper = keycloak.GenericClientRoleMapper("client_role_mapper",
             realm_id=realm.id,
             client_scope_id=client_scope.id,
             role_id=realm_role.id)
         ```
-        <!--End PulumiCodeChooser -->
 
         ### Client Role To Client Scope)
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
             realm="my-realm",
             enabled=True)
@@ -452,15 +437,14 @@
             realm_id=realm.id,
             name="my-client-scope")
         client_b_role_mapper = keycloak.GenericClientRoleMapper("client_b_role_mapper",
             realm_id=realm.id,
             client_scope_id=client_scope.id,
             role_id=client_role.id)
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Generic client role mappers can be imported using one of the following two formats:
 
         - When mapping a role to a client, use the format `{{realmId}}/client/{{clientId}}/scope-mappings/{{roleClientId}}/{{roleId}}`
```

### Comparing `pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/generic_protocol_mapper.py` & `pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/generic_protocol_mapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -268,15 +268,14 @@
         * If the provider doesn't support a particular protocol mapper, this resource can be used instead.
 
         Due to the generic nature of this mapper, it is less user-friendly and more prone to configuration errors.
         Therefore, if possible, a specific mapper should be used instead.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
             realm="my-realm",
             enabled=True)
@@ -292,15 +291,14 @@
             config={
                 "attribute.name": "name",
                 "attribute.nameformat": "Basic",
                 "attribute.value": "value",
                 "friendly.name": "display name",
             })
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Protocol mappers can be imported using the following format: `{{realm_id}}/client/{{client_keycloak_id}}/{{protocol_mapper_id}}`
 
         Example:
 
@@ -334,15 +332,14 @@
         * If the provider doesn't support a particular protocol mapper, this resource can be used instead.
 
         Due to the generic nature of this mapper, it is less user-friendly and more prone to configuration errors.
         Therefore, if possible, a specific mapper should be used instead.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
             realm="my-realm",
             enabled=True)
@@ -358,15 +355,14 @@
             config={
                 "attribute.name": "name",
                 "attribute.nameformat": "Basic",
                 "attribute.value": "value",
                 "friendly.name": "display name",
             })
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Protocol mappers can be imported using the following format: `{{realm_id}}/client/{{client_keycloak_id}}/{{protocol_mapper_id}}`
 
         Example:
```

### Comparing `pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/generic_role_mapper.py` & `pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/generic_role_mapper.py`

 * *Files 8% similar despite different names*

```diff
@@ -170,15 +170,14 @@
         `full_scope_allowed` is set to `false` for a client, role scope mapping allows you to limit the roles that get declared
         inside an access token for a client.
 
         ## Example Usage
 
         ### Realm Role To Client)
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
             realm="my-realm",
             enabled=True)
@@ -193,19 +192,17 @@
             name="my-realm-role",
             description="My Realm Role")
         client_role_mapper = keycloak.GenericRoleMapper("client_role_mapper",
             realm_id=realm.id,
             client_id=client.id,
             role_id=realm_role.id)
         ```
-        <!--End PulumiCodeChooser -->
 
         ### Client Role To Client)
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
             realm="my-realm",
             enabled=True)
@@ -233,19 +230,17 @@
             name="my-client-role",
             description="My Client Role")
         client_b_role_mapper = keycloak.GenericRoleMapper("client_b_role_mapper",
             realm_id=realm.id,
             client_id=client_b.id,
             role_id=client_role_a.id)
         ```
-        <!--End PulumiCodeChooser -->
 
         ### Realm Role To Client Scope)
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
             realm="my-realm",
             enabled=True)
@@ -257,19 +252,17 @@
             name="my-realm-role",
             description="My Realm Role")
         client_role_mapper = keycloak.GenericRoleMapper("client_role_mapper",
             realm_id=realm.id,
             client_scope_id=client_scope.id,
             role_id=realm_role.id)
         ```
-        <!--End PulumiCodeChooser -->
 
         ### Client Role To Client Scope)
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
             realm="my-realm",
             enabled=True)
@@ -288,15 +281,14 @@
             realm_id=realm.id,
             name="my-client-scope")
         client_b_role_mapper = keycloak.GenericRoleMapper("client_b_role_mapper",
             realm_id=realm.id,
             client_scope_id=client_scope.id,
             role_id=client_role.id)
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Generic client role mappers can be imported using one of the following two formats:
 
         - When mapping a role to a client, use the format `{{realmId}}/client/{{clientId}}/scope-mappings/{{roleClientId}}/{{roleId}}`
 
@@ -330,15 +322,14 @@
         `full_scope_allowed` is set to `false` for a client, role scope mapping allows you to limit the roles that get declared
         inside an access token for a client.
 
         ## Example Usage
 
         ### Realm Role To Client)
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
             realm="my-realm",
             enabled=True)
@@ -353,19 +344,17 @@
             name="my-realm-role",
             description="My Realm Role")
         client_role_mapper = keycloak.GenericRoleMapper("client_role_mapper",
             realm_id=realm.id,
             client_id=client.id,
             role_id=realm_role.id)
         ```
-        <!--End PulumiCodeChooser -->
 
         ### Client Role To Client)
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
             realm="my-realm",
             enabled=True)
@@ -393,19 +382,17 @@
             name="my-client-role",
             description="My Client Role")
         client_b_role_mapper = keycloak.GenericRoleMapper("client_b_role_mapper",
             realm_id=realm.id,
             client_id=client_b.id,
             role_id=client_role_a.id)
         ```
-        <!--End PulumiCodeChooser -->
 
         ### Realm Role To Client Scope)
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
             realm="my-realm",
             enabled=True)
@@ -417,19 +404,17 @@
             name="my-realm-role",
             description="My Realm Role")
         client_role_mapper = keycloak.GenericRoleMapper("client_role_mapper",
             realm_id=realm.id,
             client_scope_id=client_scope.id,
             role_id=realm_role.id)
         ```
-        <!--End PulumiCodeChooser -->
 
         ### Client Role To Client Scope)
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
             realm="my-realm",
             enabled=True)
@@ -448,15 +433,14 @@
             realm_id=realm.id,
             name="my-client-scope")
         client_b_role_mapper = keycloak.GenericRoleMapper("client_b_role_mapper",
             realm_id=realm.id,
             client_scope_id=client_scope.id,
             role_id=client_role.id)
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Generic client role mappers can be imported using one of the following two formats:
 
         - When mapping a role to a client, use the format `{{realmId}}/client/{{clientId}}/scope-mappings/{{roleClientId}}/{{roleId}}`
```

### Comparing `pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/get_authentication_execution.py` & `pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/get_authentication_execution.py`

 * *Files 4% similar despite different names*

```diff
@@ -76,27 +76,25 @@
                                  realm_id: Optional[str] = None,
                                  opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetAuthenticationExecutionResult:
     """
     This data source can be used to fetch the ID of an authentication execution within Keycloak.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_keycloak as keycloak
 
     realm = keycloak.Realm("realm",
         realm="my-realm",
         enabled=True)
     browser_auth_cookie = keycloak.get_authentication_execution_output(realm_id=realm.id,
         parent_flow_alias="browser",
         provider_id="auth-cookie")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str parent_flow_alias: The alias of the flow this execution is attached to.
     :param str provider_id: The name of the provider. This can be found by experimenting with the GUI and looking at HTTP requests within the network tab of your browser's development tools. This was previously known as the "authenticator".
     :param str realm_id: The realm the authentication execution exists in.
     """
     __args__ = dict()
@@ -119,27 +117,25 @@
                                         realm_id: Optional[pulumi.Input[str]] = None,
                                         opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetAuthenticationExecutionResult]:
     """
     This data source can be used to fetch the ID of an authentication execution within Keycloak.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_keycloak as keycloak
 
     realm = keycloak.Realm("realm",
         realm="my-realm",
         enabled=True)
     browser_auth_cookie = keycloak.get_authentication_execution_output(realm_id=realm.id,
         parent_flow_alias="browser",
         provider_id="auth-cookie")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str parent_flow_alias: The alias of the flow this execution is attached to.
     :param str provider_id: The name of the provider. This can be found by experimenting with the GUI and looking at HTTP requests within the network tab of your browser's development tools. This was previously known as the "authenticator".
     :param str realm_id: The realm the authentication execution exists in.
     """
     ...
```

### Comparing `pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/get_authentication_flow.py` & `pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/get_authentication_flow.py`

 * *Files 6% similar despite different names*

```diff
@@ -66,26 +66,24 @@
                             realm_id: Optional[str] = None,
                             opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetAuthenticationFlowResult:
     """
     This data source can be used to fetch the ID of an authentication flow within Keycloak.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_keycloak as keycloak
 
     realm = keycloak.Realm("realm",
         realm="my-realm",
         enabled=True)
     browser_auth_cookie = keycloak.get_authentication_flow_output(realm_id=realm.id,
         alias="browser")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str alias: The alias of the flow.
     :param str realm_id: The realm the authentication flow exists in.
     """
     __args__ = dict()
     __args__['alias'] = alias
@@ -104,25 +102,23 @@
                                    realm_id: Optional[pulumi.Input[str]] = None,
                                    opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetAuthenticationFlowResult]:
     """
     This data source can be used to fetch the ID of an authentication flow within Keycloak.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_keycloak as keycloak
 
     realm = keycloak.Realm("realm",
         realm="my-realm",
         enabled=True)
     browser_auth_cookie = keycloak.get_authentication_flow_output(realm_id=realm.id,
         alias="browser")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str alias: The alias of the flow.
     :param str realm_id: The realm the authentication flow exists in.
     """
     ...
```

### Comparing `pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/get_client_description_converter.py` & `pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/get_client_description_converter.py`

 * *Files 15% similar despite different names*

```diff
@@ -383,56 +383,54 @@
                                      opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetClientDescriptionConverterResult:
     """
     This data source uses the [ClientDescriptionConverter](https://www.keycloak.org/docs-api/6.0/javadocs/org/keycloak/exportimport/ClientDescriptionConverter.html) API to convert a generic client description into a Keycloak
     client. This data can then be used to manage the client within Keycloak.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_keycloak as keycloak
 
     realm = keycloak.Realm("realm",
         realm="my-realm",
         enabled=True)
     saml_client = keycloak.get_client_description_converter_output(realm_id=realm.id,
-        body=\"\"\"	<md:EntityDescriptor xmlns:md="urn:oasis:names:tc:SAML:2.0:metadata" validUntil="2021-04-17T12:41:46Z" cacheDuration="PT604800S" entityID="FakeEntityId">
+        body=\"\"\"\\x09<md:EntityDescriptor xmlns:md="urn:oasis:names:tc:SAML:2.0:metadata" validUntil="2021-04-17T12:41:46Z" cacheDuration="PT604800S" entityID="FakeEntityId">
         <md:SPSSODescriptor AuthnRequestsSigned="false" WantAssertionsSigned="false" protocolSupportEnumeration="urn:oasis:names:tc:SAML:2.0:protocol">
             <md:KeyDescriptor use="signing">
-    			<ds:KeyInfo xmlns:ds="http://www.w3.org/2000/09/xmldsig#">
-    				<ds:X509Data>
-    					<ds:X509Certificate>MIICyDCCAjGgAwIBAgIBADANBgkqhkiG9w0BAQ0FADCBgDELMAkGA1UEBhMCdXMx
-    					CzAJBgNVBAgMAklBMSQwIgYDVQQKDBt0ZXJyYWZvcm0tcHJvdmlkZXIta2V5Y2xv
-    					YWsxHDAaBgNVBAMME21ycGFya2Vycy5naXRodWIuaW8xIDAeBgkqhkiG9w0BCQEW
-    					EW1pY2hhZWxAcGFya2VyLmdnMB4XDTE5MDEwODE0NDYzNloXDTI5MDEwNTE0NDYz
-    					NlowgYAxCzAJBgNVBAYTAnVzMQswCQYDVQQIDAJJQTEkMCIGA1UECgwbdGVycmFm
-    					b3JtLXByb3ZpZGVyLWtleWNsb2FrMRwwGgYDVQQDDBNtcnBhcmtlcnMuZ2l0aHVi
-    					LmlvMSAwHgYJKoZIhvcNAQkBFhFtaWNoYWVsQHBhcmtlci5nZzCBnzANBgkqhkiG
-    					9w0BAQEFAAOBjQAwgYkCgYEAxuZny7uyYxGVPtpie14gNQC4tT9sAvO2sVNDhuoe
-    					qIKLRpNwkHnwQmwe5OxSh9K0BPHp/DNuuVWUqvo4tniEYn3jBr7FwLYLTKojQIxj
-    					53S1UTT9EXq3eP5HsHMD0QnTuca2nlNYUDBm6ud2fQj0Jt5qLx86EbEC28N56IRv
-    					GX8CAwEAAaNQME4wHQYDVR0OBBYEFMLnbQh77j7vhGTpAhKpDhCrBsPZMB8GA1Ud
-    					IwQYMBaAFMLnbQh77j7vhGTpAhKpDhCrBsPZMAwGA1UdEwQFMAMBAf8wDQYJKoZI
-    					hvcNAQENBQADgYEAB8wGrAQY0pAfwbnYSyBt4STbebeRTu1/q1ucfrtc3qsegcd5
-    					n01xTR+T2uZJwqHFPpFjr4IPORiHx3+4BWCweslPD53qBjKUPXcbMO1Revjef6Tj
-    					K3K0AuJ94fxgXVoT61Nzu/a6Lj6RhzU/Dao9mlSbJY+YSbm+ZBpsuRUQ84s=</ds:X509Certificate>
-    				</ds:X509Data>
-    			</ds:KeyInfo>
-    		</md:KeyDescriptor>
-    		<md:NameIDFormat>urn:oasis:names:tc:SAML:1.1:nameid-format:unspecified</md:NameIDFormat>
+    \\x09\\x09\\x09<ds:KeyInfo xmlns:ds="http://www.w3.org/2000/09/xmldsig#">
+    \\x09\\x09\\x09\\x09<ds:X509Data>
+    \\x09\\x09\\x09\\x09\\x09<ds:X509Certificate>MIICyDCCAjGgAwIBAgIBADANBgkqhkiG9w0BAQ0FADCBgDELMAkGA1UEBhMCdXMx
+    \\x09\\x09\\x09\\x09\\x09CzAJBgNVBAgMAklBMSQwIgYDVQQKDBt0ZXJyYWZvcm0tcHJvdmlkZXIta2V5Y2xv
+    \\x09\\x09\\x09\\x09\\x09YWsxHDAaBgNVBAMME21ycGFya2Vycy5naXRodWIuaW8xIDAeBgkqhkiG9w0BCQEW
+    \\x09\\x09\\x09\\x09\\x09EW1pY2hhZWxAcGFya2VyLmdnMB4XDTE5MDEwODE0NDYzNloXDTI5MDEwNTE0NDYz
+    \\x09\\x09\\x09\\x09\\x09NlowgYAxCzAJBgNVBAYTAnVzMQswCQYDVQQIDAJJQTEkMCIGA1UECgwbdGVycmFm
+    \\x09\\x09\\x09\\x09\\x09b3JtLXByb3ZpZGVyLWtleWNsb2FrMRwwGgYDVQQDDBNtcnBhcmtlcnMuZ2l0aHVi
+    \\x09\\x09\\x09\\x09\\x09LmlvMSAwHgYJKoZIhvcNAQkBFhFtaWNoYWVsQHBhcmtlci5nZzCBnzANBgkqhkiG
+    \\x09\\x09\\x09\\x09\\x099w0BAQEFAAOBjQAwgYkCgYEAxuZny7uyYxGVPtpie14gNQC4tT9sAvO2sVNDhuoe
+    \\x09\\x09\\x09\\x09\\x09qIKLRpNwkHnwQmwe5OxSh9K0BPHp/DNuuVWUqvo4tniEYn3jBr7FwLYLTKojQIxj
+    \\x09\\x09\\x09\\x09\\x0953S1UTT9EXq3eP5HsHMD0QnTuca2nlNYUDBm6ud2fQj0Jt5qLx86EbEC28N56IRv
+    \\x09\\x09\\x09\\x09\\x09GX8CAwEAAaNQME4wHQYDVR0OBBYEFMLnbQh77j7vhGTpAhKpDhCrBsPZMB8GA1Ud
+    \\x09\\x09\\x09\\x09\\x09IwQYMBaAFMLnbQh77j7vhGTpAhKpDhCrBsPZMAwGA1UdEwQFMAMBAf8wDQYJKoZI
+    \\x09\\x09\\x09\\x09\\x09hvcNAQENBQADgYEAB8wGrAQY0pAfwbnYSyBt4STbebeRTu1/q1ucfrtc3qsegcd5
+    \\x09\\x09\\x09\\x09\\x09n01xTR+T2uZJwqHFPpFjr4IPORiHx3+4BWCweslPD53qBjKUPXcbMO1Revjef6Tj
+    \\x09\\x09\\x09\\x09\\x09K3K0AuJ94fxgXVoT61Nzu/a6Lj6RhzU/Dao9mlSbJY+YSbm+ZBpsuRUQ84s=</ds:X509Certificate>
+    \\x09\\x09\\x09\\x09</ds:X509Data>
+    \\x09\\x09\\x09</ds:KeyInfo>
+    \\x09\\x09</md:KeyDescriptor>
+    \\x09\\x09<md:NameIDFormat>urn:oasis:names:tc:SAML:1.1:nameid-format:unspecified</md:NameIDFormat>
             <md:AssertionConsumerService Binding="urn:oasis:names:tc:SAML:2.0:bindings:HTTP-POST" Location="https://localhost/acs/saml/" index="1"/>
         </md:SPSSODescriptor>
     </md:EntityDescriptor>
     \"\"\")
     saml_client_client = keycloak.saml.Client("saml_client",
         realm_id=realm.id,
         client_id=saml_client.client_id)
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str body: The body of the request to convert.
     :param str realm_id: The realm to use for the client description converter API call.
     """
     __args__ = dict()
     __args__['body'] = body
@@ -487,55 +485,53 @@
                                             opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetClientDescriptionConverterResult]:
     """
     This data source uses the [ClientDescriptionConverter](https://www.keycloak.org/docs-api/6.0/javadocs/org/keycloak/exportimport/ClientDescriptionConverter.html) API to convert a generic client description into a Keycloak
     client. This data can then be used to manage the client within Keycloak.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_keycloak as keycloak
 
     realm = keycloak.Realm("realm",
         realm="my-realm",
         enabled=True)
     saml_client = keycloak.get_client_description_converter_output(realm_id=realm.id,
-        body=\"\"\"	<md:EntityDescriptor xmlns:md="urn:oasis:names:tc:SAML:2.0:metadata" validUntil="2021-04-17T12:41:46Z" cacheDuration="PT604800S" entityID="FakeEntityId">
+        body=\"\"\"\\x09<md:EntityDescriptor xmlns:md="urn:oasis:names:tc:SAML:2.0:metadata" validUntil="2021-04-17T12:41:46Z" cacheDuration="PT604800S" entityID="FakeEntityId">
         <md:SPSSODescriptor AuthnRequestsSigned="false" WantAssertionsSigned="false" protocolSupportEnumeration="urn:oasis:names:tc:SAML:2.0:protocol">
             <md:KeyDescriptor use="signing">
-    			<ds:KeyInfo xmlns:ds="http://www.w3.org/2000/09/xmldsig#">
-    				<ds:X509Data>
-    					<ds:X509Certificate>MIICyDCCAjGgAwIBAgIBADANBgkqhkiG9w0BAQ0FADCBgDELMAkGA1UEBhMCdXMx
-    					CzAJBgNVBAgMAklBMSQwIgYDVQQKDBt0ZXJyYWZvcm0tcHJvdmlkZXIta2V5Y2xv
-    					YWsxHDAaBgNVBAMME21ycGFya2Vycy5naXRodWIuaW8xIDAeBgkqhkiG9w0BCQEW
-    					EW1pY2hhZWxAcGFya2VyLmdnMB4XDTE5MDEwODE0NDYzNloXDTI5MDEwNTE0NDYz
-    					NlowgYAxCzAJBgNVBAYTAnVzMQswCQYDVQQIDAJJQTEkMCIGA1UECgwbdGVycmFm
-    					b3JtLXByb3ZpZGVyLWtleWNsb2FrMRwwGgYDVQQDDBNtcnBhcmtlcnMuZ2l0aHVi
-    					LmlvMSAwHgYJKoZIhvcNAQkBFhFtaWNoYWVsQHBhcmtlci5nZzCBnzANBgkqhkiG
-    					9w0BAQEFAAOBjQAwgYkCgYEAxuZny7uyYxGVPtpie14gNQC4tT9sAvO2sVNDhuoe
-    					qIKLRpNwkHnwQmwe5OxSh9K0BPHp/DNuuVWUqvo4tniEYn3jBr7FwLYLTKojQIxj
-    					53S1UTT9EXq3eP5HsHMD0QnTuca2nlNYUDBm6ud2fQj0Jt5qLx86EbEC28N56IRv
-    					GX8CAwEAAaNQME4wHQYDVR0OBBYEFMLnbQh77j7vhGTpAhKpDhCrBsPZMB8GA1Ud
-    					IwQYMBaAFMLnbQh77j7vhGTpAhKpDhCrBsPZMAwGA1UdEwQFMAMBAf8wDQYJKoZI
-    					hvcNAQENBQADgYEAB8wGrAQY0pAfwbnYSyBt4STbebeRTu1/q1ucfrtc3qsegcd5
-    					n01xTR+T2uZJwqHFPpFjr4IPORiHx3+4BWCweslPD53qBjKUPXcbMO1Revjef6Tj
-    					K3K0AuJ94fxgXVoT61Nzu/a6Lj6RhzU/Dao9mlSbJY+YSbm+ZBpsuRUQ84s=</ds:X509Certificate>
-    				</ds:X509Data>
-    			</ds:KeyInfo>
-    		</md:KeyDescriptor>
-    		<md:NameIDFormat>urn:oasis:names:tc:SAML:1.1:nameid-format:unspecified</md:NameIDFormat>
+    \\x09\\x09\\x09<ds:KeyInfo xmlns:ds="http://www.w3.org/2000/09/xmldsig#">
+    \\x09\\x09\\x09\\x09<ds:X509Data>
+    \\x09\\x09\\x09\\x09\\x09<ds:X509Certificate>MIICyDCCAjGgAwIBAgIBADANBgkqhkiG9w0BAQ0FADCBgDELMAkGA1UEBhMCdXMx
+    \\x09\\x09\\x09\\x09\\x09CzAJBgNVBAgMAklBMSQwIgYDVQQKDBt0ZXJyYWZvcm0tcHJvdmlkZXIta2V5Y2xv
+    \\x09\\x09\\x09\\x09\\x09YWsxHDAaBgNVBAMME21ycGFya2Vycy5naXRodWIuaW8xIDAeBgkqhkiG9w0BCQEW
+    \\x09\\x09\\x09\\x09\\x09EW1pY2hhZWxAcGFya2VyLmdnMB4XDTE5MDEwODE0NDYzNloXDTI5MDEwNTE0NDYz
+    \\x09\\x09\\x09\\x09\\x09NlowgYAxCzAJBgNVBAYTAnVzMQswCQYDVQQIDAJJQTEkMCIGA1UECgwbdGVycmFm
+    \\x09\\x09\\x09\\x09\\x09b3JtLXByb3ZpZGVyLWtleWNsb2FrMRwwGgYDVQQDDBNtcnBhcmtlcnMuZ2l0aHVi
+    \\x09\\x09\\x09\\x09\\x09LmlvMSAwHgYJKoZIhvcNAQkBFhFtaWNoYWVsQHBhcmtlci5nZzCBnzANBgkqhkiG
+    \\x09\\x09\\x09\\x09\\x099w0BAQEFAAOBjQAwgYkCgYEAxuZny7uyYxGVPtpie14gNQC4tT9sAvO2sVNDhuoe
+    \\x09\\x09\\x09\\x09\\x09qIKLRpNwkHnwQmwe5OxSh9K0BPHp/DNuuVWUqvo4tniEYn3jBr7FwLYLTKojQIxj
+    \\x09\\x09\\x09\\x09\\x0953S1UTT9EXq3eP5HsHMD0QnTuca2nlNYUDBm6ud2fQj0Jt5qLx86EbEC28N56IRv
+    \\x09\\x09\\x09\\x09\\x09GX8CAwEAAaNQME4wHQYDVR0OBBYEFMLnbQh77j7vhGTpAhKpDhCrBsPZMB8GA1Ud
+    \\x09\\x09\\x09\\x09\\x09IwQYMBaAFMLnbQh77j7vhGTpAhKpDhCrBsPZMAwGA1UdEwQFMAMBAf8wDQYJKoZI
+    \\x09\\x09\\x09\\x09\\x09hvcNAQENBQADgYEAB8wGrAQY0pAfwbnYSyBt4STbebeRTu1/q1ucfrtc3qsegcd5
+    \\x09\\x09\\x09\\x09\\x09n01xTR+T2uZJwqHFPpFjr4IPORiHx3+4BWCweslPD53qBjKUPXcbMO1Revjef6Tj
+    \\x09\\x09\\x09\\x09\\x09K3K0AuJ94fxgXVoT61Nzu/a6Lj6RhzU/Dao9mlSbJY+YSbm+ZBpsuRUQ84s=</ds:X509Certificate>
+    \\x09\\x09\\x09\\x09</ds:X509Data>
+    \\x09\\x09\\x09</ds:KeyInfo>
+    \\x09\\x09</md:KeyDescriptor>
+    \\x09\\x09<md:NameIDFormat>urn:oasis:names:tc:SAML:1.1:nameid-format:unspecified</md:NameIDFormat>
             <md:AssertionConsumerService Binding="urn:oasis:names:tc:SAML:2.0:bindings:HTTP-POST" Location="https://localhost/acs/saml/" index="1"/>
         </md:SPSSODescriptor>
     </md:EntityDescriptor>
     \"\"\")
     saml_client_client = keycloak.saml.Client("saml_client",
         realm_id=realm.id,
         client_id=saml_client.client_id)
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str body: The body of the request to convert.
     :param str realm_id: The realm to use for the client description converter API call.
     """
     ...
```

### Comparing `pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/get_group.py` & `pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/get_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/get_realm.py` & `pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/get_realm.py`

 * *Files 1% similar despite different names*

```diff
@@ -566,26 +566,24 @@
     ## # Realm data source
 
     This data source can be used to fetch properties of a Keycloak realm for
     usage with other resources.
 
     ### Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_keycloak as keycloak
 
     realm = keycloak.get_realm(realm="my-realm")
     # use the data source
     group = keycloak.Role("group",
         realm_id=id,
         name="group")
     ```
-    <!--End PulumiCodeChooser -->
 
     ### Argument Reference
 
     The following arguments are supported:
 
     - `realm` - (Required) The realm name.
 
@@ -685,26 +683,24 @@
     ## # Realm data source
 
     This data source can be used to fetch properties of a Keycloak realm for
     usage with other resources.
 
     ### Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_keycloak as keycloak
 
     realm = keycloak.get_realm(realm="my-realm")
     # use the data source
     group = keycloak.Role("group",
         realm_id=id,
         name="group")
     ```
-    <!--End PulumiCodeChooser -->
 
     ### Argument Reference
 
     The following arguments are supported:
 
     - `realm` - (Required) The realm name.
```

### Comparing `pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/get_realm_keys.py` & `pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/get_realm_keys.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/get_role.py` & `pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/get_role.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/get_user.py` & `pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/get_user.py`

 * *Files 4% similar despite different names*

```diff
@@ -159,26 +159,24 @@
              username: Optional[str] = None,
              opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetUserResult:
     """
     This data source can be used to fetch properties of a user within Keycloak.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_keycloak as keycloak
 
     master_realm = keycloak.get_realm(realm="master")
     # use the keycloak_user data source to grab the admin user's ID
     default_admin_user = keycloak.get_user(realm_id=master_realm.id,
         username="keycloak")
     pulumi.export("keycloakUserId", default_admin_user.id)
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str realm_id: The realm this user belongs to.
     :param str username: The unique username of this user.
     """
     __args__ = dict()
     __args__['realmId'] = realm_id
@@ -205,25 +203,23 @@
                     username: Optional[pulumi.Input[str]] = None,
                     opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetUserResult]:
     """
     This data source can be used to fetch properties of a user within Keycloak.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_keycloak as keycloak
 
     master_realm = keycloak.get_realm(realm="master")
     # use the keycloak_user data source to grab the admin user's ID
     default_admin_user = keycloak.get_user(realm_id=master_realm.id,
         username="keycloak")
     pulumi.export("keycloakUserId", default_admin_user.id)
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str realm_id: The realm this user belongs to.
     :param str username: The unique username of this user.
     """
     ...
```

### Comparing `pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/get_user_realm_roles.py` & `pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/get_user_realm_roles.py`

 * *Files 6% similar despite different names*

```diff
@@ -78,29 +78,27 @@
                          user_id: Optional[str] = None,
                          opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetUserRealmRolesResult:
     """
     This data source can be used to fetch the realm roles of a user within Keycloak.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_keycloak as keycloak
 
     master_realm = keycloak.get_realm(realm="master")
     # use the keycloak_user data source to grab the admin user's ID
     default_admin_user = keycloak.get_user(realm_id=master_realm.id,
         username="keycloak")
     # use the keycloak_user_realm_roles data source to list role names
     user_realm_roles = keycloak.get_user_realm_roles(realm_id=master_realm.id,
         user_id=default_admin_user.id)
     pulumi.export("keycloakUserRoleNames", user_realm_roles.role_names)
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str realm_id: The realm this user belongs to.
     :param str user_id: The ID of the user to query realm roles for.
     """
     __args__ = dict()
     __args__['realmId'] = realm_id
@@ -120,28 +118,26 @@
                                 user_id: Optional[pulumi.Input[str]] = None,
                                 opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetUserRealmRolesResult]:
     """
     This data source can be used to fetch the realm roles of a user within Keycloak.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_keycloak as keycloak
 
     master_realm = keycloak.get_realm(realm="master")
     # use the keycloak_user data source to grab the admin user's ID
     default_admin_user = keycloak.get_user(realm_id=master_realm.id,
         username="keycloak")
     # use the keycloak_user_realm_roles data source to list role names
     user_realm_roles = keycloak.get_user_realm_roles(realm_id=master_realm.id,
         user_id=default_admin_user.id)
     pulumi.export("keycloakUserRoleNames", user_realm_roles.role_names)
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str realm_id: The realm this user belongs to.
     :param str user_id: The ID of the user to query realm roles for.
     """
     ...
```

### Comparing `pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/group.py` & `pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/group.py`

 * *Files 1% similar despite different names*

```diff
@@ -156,15 +156,14 @@
         Attributes can also be defined on Groups.
 
         Groups can also be federated from external data sources, such as LDAP or Active Directory.
         This resource **should not** be used to manage groups that were created this way.
 
         ### Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
             realm="my-realm",
             enabled=True)
@@ -180,15 +179,14 @@
             parent_id=parent_group.id,
             name="child-group-with-optional-attributes",
             attributes={
                 "key1": "value1",
                 "key2": "value2",
             })
         ```
-        <!--End PulumiCodeChooser -->
 
         ### Argument Reference
 
         The following arguments are supported:
 
         - `realm_id` - (Required) The realm this group exists in.
         - `parent_id` - (Optional) The ID of this group's parent. If omitted, this group will be defined at the root level.
@@ -229,15 +227,14 @@
         Attributes can also be defined on Groups.
 
         Groups can also be federated from external data sources, such as LDAP or Active Directory.
         This resource **should not** be used to manage groups that were created this way.
 
         ### Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
             realm="my-realm",
             enabled=True)
@@ -253,15 +250,14 @@
             parent_id=parent_group.id,
             name="child-group-with-optional-attributes",
             attributes={
                 "key1": "value1",
                 "key2": "value2",
             })
         ```
-        <!--End PulumiCodeChooser -->
 
         ### Argument Reference
 
         The following arguments are supported:
 
         - `realm_id` - (Required) The realm this group exists in.
         - `parent_id` - (Optional) The ID of this group's parent. If omitted, this group will be defined at the root level.
```

### Comparing `pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/group_memberships.py` & `pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/group_memberships.py`

 * *Files 2% similar despite different names*

```diff
@@ -121,15 +121,14 @@
         as a default group via `DefaultGroups`.
 
         This resource **should not** be used to control membership of a group that has its members
         federated from an external source via group mapping.
 
         ### Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
             realm="my-realm",
             enabled=True)
@@ -140,15 +139,14 @@
             realm_id=realm.id,
             username="my-user")
         group_members = keycloak.GroupMemberships("group_members",
             realm_id=realm.id,
             group_id=group.id,
             members=[user.username])
         ```
-        <!--End PulumiCodeChooser -->
 
         ### Argument Reference
 
         The following arguments are supported:
 
         - `realm_id` - (Required) The realm this group exists in.
         - `group_id` - (Required) The ID of the group this resource should manage memberships for.
@@ -183,15 +181,14 @@
         as a default group via `DefaultGroups`.
 
         This resource **should not** be used to control membership of a group that has its members
         federated from an external source via group mapping.
 
         ### Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
             realm="my-realm",
             enabled=True)
@@ -202,15 +199,14 @@
             realm_id=realm.id,
             username="my-user")
         group_members = keycloak.GroupMemberships("group_members",
             realm_id=realm.id,
             group_id=group.id,
             members=[user.username])
         ```
-        <!--End PulumiCodeChooser -->
 
         ### Argument Reference
 
         The following arguments are supported:
 
         - `realm_id` - (Required) The realm this group exists in.
         - `group_id` - (Required) The ID of the group this resource should manage memberships for.
```

### Comparing `pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/group_permissions.py` & `pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/group_permissions.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/group_roles.py` & `pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/group_roles.py`

 * *Files 2% similar despite different names*

```diff
@@ -143,15 +143,14 @@
 
         Note that when assigning composite roles to a group, you may see a
         non-empty plan following a `pulumi up` if you assign a role and a
         composite that includes that role to the same group.
 
         ### Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
             realm="my-realm",
             enabled=True)
@@ -177,15 +176,14 @@
             realm_id=realm.id,
             group_id=group.id,
             role_ids=[
                 realm_role.id,
                 client_role.id,
             ])
         ```
-        <!--End PulumiCodeChooser -->
 
         ### Argument Reference
 
         The following arguments are supported:
 
         - `realm_id` - (Required) The realm this group exists in.
         - `group_id` - (Required) The ID of the group this resource should
@@ -223,15 +221,14 @@
 
         Note that when assigning composite roles to a group, you may see a
         non-empty plan following a `pulumi up` if you assign a role and a
         composite that includes that role to the same group.
 
         ### Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
             realm="my-realm",
             enabled=True)
@@ -257,15 +254,14 @@
             realm_id=realm.id,
             group_id=group.id,
             role_ids=[
                 realm_role.id,
                 client_role.id,
             ])
         ```
-        <!--End PulumiCodeChooser -->
 
         ### Argument Reference
 
         The following arguments are supported:
 
         - `realm_id` - (Required) The realm this group exists in.
         - `group_id` - (Required) The ID of the group this resource should
```

### Comparing `pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/hardcoded_attribute_identity_provider_mapper.py` & `pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/hardcoded_attribute_identity_provider_mapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -256,15 +256,14 @@
         """
         Allows for creating and managing hardcoded attribute mappers for Keycloak identity provider.
 
         The identity provider hardcoded attribute mapper will set the specified value to the IDP attribute.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
             realm="my-realm",
             enabled=True)
@@ -282,15 +281,14 @@
             attribute_name="attribute",
             attribute_value="value",
             user_session=True,
             extra_config={
                 "syncMode": "INHERIT",
             })
         ```
-        <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] attribute_name: The name of the IDP attribute to set.
         :param pulumi.Input[str] attribute_value: The value to set to the attribute. You can hardcode any value like 'foo'.
         :param pulumi.Input[str] identity_provider_alias: The IDP alias of the attribute to set.
         :param pulumi.Input[str] name: Display name of this mapper when displayed in the console.
@@ -306,15 +304,14 @@
         """
         Allows for creating and managing hardcoded attribute mappers for Keycloak identity provider.
 
         The identity provider hardcoded attribute mapper will set the specified value to the IDP attribute.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
             realm="my-realm",
             enabled=True)
@@ -332,15 +329,14 @@
             attribute_name="attribute",
             attribute_value="value",
             user_session=True,
             extra_config={
                 "syncMode": "INHERIT",
             })
         ```
-        <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param HardcodedAttributeIdentityProviderMapperArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
```

### Comparing `pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/hardcoded_role_identity_mapper.py` & `pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/hardcoded_role_identity_mapper.py`

 * *Files 2% similar despite different names*

```diff
@@ -191,15 +191,14 @@
         """
         Allows for creating and managing hardcoded role mappers for Keycloak identity provider.
 
         The identity provider hardcoded role mapper grants a specified Keycloak role to each Keycloak user from the LDAP provider.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
             realm="my-realm",
             enabled=True)
@@ -219,15 +218,14 @@
             name="hardcodedRole",
             identity_provider_alias=oidc.alias,
             role="my-realm-role",
             extra_config={
                 "syncMode": "INHERIT",
             })
         ```
-        <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] identity_provider_alias: The IDP alias of the attribute to set.
         :param pulumi.Input[str] name: Display name of this mapper when displayed in the console.
         :param pulumi.Input[str] realm: The realm ID that this mapper will exist in.
         :param pulumi.Input[str] role: The name of the role which should be assigned to the users.
@@ -241,15 +239,14 @@
         """
         Allows for creating and managing hardcoded role mappers for Keycloak identity provider.
 
         The identity provider hardcoded role mapper grants a specified Keycloak role to each Keycloak user from the LDAP provider.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
             realm="my-realm",
             enabled=True)
@@ -269,15 +266,14 @@
             name="hardcodedRole",
             identity_provider_alias=oidc.alias,
             role="my-realm-role",
             extra_config={
                 "syncMode": "INHERIT",
             })
         ```
-        <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param HardcodedRoleIdentityMapperArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
```

### Comparing `pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/identity_provider_token_exchange_scope_permission.py` & `pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/identity_provider_token_exchange_scope_permission.py`

 * *Files 0% similar despite different names*

```diff
@@ -225,15 +225,14 @@
                  policy_type: Optional[pulumi.Input[str]] = None,
                  provider_alias: Optional[pulumi.Input[str]] = None,
                  realm_id: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         token_exchange_realm = keycloak.Realm("token_exchange_realm",
             realm="token-exchange_destination_realm",
             enabled=True)
@@ -257,15 +256,14 @@
         #relevant part
         oidc_idp_permission = keycloak.IdentityProviderTokenExchangeScopePermission("oidc_idp_permission",
             realm_id=token_exchange_realm.id,
             provider_alias=token_exchange_my_oidc_idp.alias,
             policy_type="client",
             clients=[token_exchange_webapp_client.id])
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         This resource can be imported using the format `{{realm_id}}/{{provider_alias}}`, where `provider_alias` is the alias that
 
         you assign to the identity provider upon creation.
 
@@ -289,15 +287,14 @@
     def __init__(__self__,
                  resource_name: str,
                  args: IdentityProviderTokenExchangeScopePermissionArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         token_exchange_realm = keycloak.Realm("token_exchange_realm",
             realm="token-exchange_destination_realm",
             enabled=True)
@@ -321,15 +318,14 @@
         #relevant part
         oidc_idp_permission = keycloak.IdentityProviderTokenExchangeScopePermission("oidc_idp_permission",
             realm_id=token_exchange_realm.id,
             provider_alias=token_exchange_my_oidc_idp.alias,
             policy_type="client",
             clients=[token_exchange_webapp_client.id])
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         This resource can be imported using the format `{{realm_id}}/{{provider_alias}}`, where `provider_alias` is the alias that
 
         you assign to the identity provider upon creation.
```

### Comparing `pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/ldap/__init__.py` & `pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/ldap/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/ldap/_inputs.py` & `pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/ldap/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/ldap/custom_mapper.py` & `pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/ldap/custom_mapper.py`

 * *Files 2% similar despite different names*

```diff
@@ -234,15 +234,14 @@
         specify the custom id and custom implementation class of the self-implemented attribute mapper as well as additional
         properties via config map.
 
         The custom mapper should already be deployed into keycloak in order to be correctly configured.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
             realm="my-realm",
             enabled=True)
@@ -267,15 +266,14 @@
             provider_id="custom-provider-registered-in-keycloak",
             provider_type="com.example.custom.ldap.mappers.CustomMapper",
             config={
                 "attribute.name": "name",
                 "attribute.value": "value",
             })
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         LDAP mappers can be imported using the format `{{realm_id}}/{{ldap_user_federation_id}}/{{ldap_mapper_id}}`.
 
         The ID of the LDAP user federation provider and the mapper can be found within the Keycloak GUI, and they are typically GUIDs.
 
@@ -309,15 +307,14 @@
         specify the custom id and custom implementation class of the self-implemented attribute mapper as well as additional
         properties via config map.
 
         The custom mapper should already be deployed into keycloak in order to be correctly configured.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
             realm="my-realm",
             enabled=True)
@@ -342,15 +339,14 @@
             provider_id="custom-provider-registered-in-keycloak",
             provider_type="com.example.custom.ldap.mappers.CustomMapper",
             config={
                 "attribute.name": "name",
                 "attribute.value": "value",
             })
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         LDAP mappers can be imported using the format `{{realm_id}}/{{ldap_user_federation_id}}/{{ldap_mapper_id}}`.
 
         The ID of the LDAP user federation provider and the mapper can be found within the Keycloak GUI, and they are typically GUIDs.
```

### Comparing `pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/ldap/full_name_mapper.py` & `pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/ldap/full_name_mapper.py`

 * *Files 2% similar despite different names*

```diff
@@ -211,15 +211,14 @@
         via LDAP.
 
         The LDAP full name mapper can map a user's full name from an LDAP attribute
         to the first and last name attributes of a Keycloak user.
 
         ### Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
             realm="test",
             enabled=True)
@@ -239,15 +238,14 @@
             bind_credential="admin")
         ldap_full_name_mapper = keycloak.ldap.FullNameMapper("ldap_full_name_mapper",
             realm_id=realm.id,
             ldap_user_federation_id=ldap_user_federation.id,
             name="full-name-mapper",
             ldap_full_name_attribute="cn")
         ```
-        <!--End PulumiCodeChooser -->
 
         ### Argument Reference
 
         The following arguments are supported:
 
         - `realm_id` - (Required) The realm that this LDAP mapper will exist in.
         - `ldap_user_federation_id` - (Required) The ID of the LDAP user federation provider to attach this mapper to.
@@ -281,15 +279,14 @@
         via LDAP.
 
         The LDAP full name mapper can map a user's full name from an LDAP attribute
         to the first and last name attributes of a Keycloak user.
 
         ### Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
             realm="test",
             enabled=True)
@@ -309,15 +306,14 @@
             bind_credential="admin")
         ldap_full_name_mapper = keycloak.ldap.FullNameMapper("ldap_full_name_mapper",
             realm_id=realm.id,
             ldap_user_federation_id=ldap_user_federation.id,
             name="full-name-mapper",
             ldap_full_name_attribute="cn")
         ```
-        <!--End PulumiCodeChooser -->
 
         ### Argument Reference
 
         The following arguments are supported:
 
         - `realm_id` - (Required) The realm that this LDAP mapper will exist in.
         - `ldap_user_federation_id` - (Required) The ID of the LDAP user federation provider to attach this mapper to.
```

### Comparing `pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/ldap/group_mapper.py` & `pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/ldap/group_mapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -508,15 +508,14 @@
 
         The LDAP group mapper can be used to map an LDAP user's groups from some DN
         to Keycloak groups. This group mapper will also create the groups within Keycloak
         if they do not already exist.
 
         ### Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
             realm="test",
             enabled=True)
@@ -542,15 +541,14 @@
             group_name_ldap_attribute="cn",
             group_object_classes=["groupOfNames"],
             membership_attribute_type="DN",
             membership_ldap_attribute="member",
             membership_user_ldap_attribute="cn",
             memberof_ldap_attribute="memberOf")
         ```
-        <!--End PulumiCodeChooser -->
 
         ### Argument Reference
 
         The following arguments are supported:
 
         - `realm_id` - (Required) The realm that this LDAP mapper will exist in.
         - `ldap_user_federation_id` - (Required) The ID of the LDAP user federation provider to attach this mapper to.
@@ -596,15 +594,14 @@
 
         The LDAP group mapper can be used to map an LDAP user's groups from some DN
         to Keycloak groups. This group mapper will also create the groups within Keycloak
         if they do not already exist.
 
         ### Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
             realm="test",
             enabled=True)
@@ -630,15 +627,14 @@
             group_name_ldap_attribute="cn",
             group_object_classes=["groupOfNames"],
             membership_attribute_type="DN",
             membership_ldap_attribute="member",
             membership_user_ldap_attribute="cn",
             memberof_ldap_attribute="memberOf")
         ```
-        <!--End PulumiCodeChooser -->
 
         ### Argument Reference
 
         The following arguments are supported:
 
         - `realm_id` - (Required) The realm that this LDAP mapper will exist in.
         - `ldap_user_federation_id` - (Required) The ID of the LDAP user federation provider to attach this mapper to.
```

### Comparing `pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/ldap/hardcoded_attribute_mapper.py` & `pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/ldap/hardcoded_attribute_mapper.py`

 * *Files 2% similar despite different names*

```diff
@@ -199,15 +199,14 @@
 
         The LDAP hardcoded attribute mapper will set the specified value to the LDAP attribute.
 
         **NOTE**: This mapper only works when the `sync_registrations` attribute on the `ldap.UserFederation` resource is set to `true`.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
             realm="my-realm",
             enabled=True)
@@ -229,15 +228,14 @@
         assign_bar_to_foo = keycloak.ldap.HardcodedAttributeMapper("assign_bar_to_foo",
             realm_id=realm.id,
             ldap_user_federation_id=ldap_user_federation.id,
             name="assign-foo-to-bar",
             attribute_name="foo",
             attribute_value="bar")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         LDAP mappers can be imported using the format `{{realm_id}}/{{ldap_user_federation_id}}/{{ldap_mapper_id}}`.
 
         The ID of the LDAP user federation provider and the mapper can be found within the Keycloak GUI, and they are typically GUIDs.
 
@@ -268,15 +266,14 @@
 
         The LDAP hardcoded attribute mapper will set the specified value to the LDAP attribute.
 
         **NOTE**: This mapper only works when the `sync_registrations` attribute on the `ldap.UserFederation` resource is set to `true`.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
             realm="my-realm",
             enabled=True)
@@ -298,15 +295,14 @@
         assign_bar_to_foo = keycloak.ldap.HardcodedAttributeMapper("assign_bar_to_foo",
             realm_id=realm.id,
             ldap_user_federation_id=ldap_user_federation.id,
             name="assign-foo-to-bar",
             attribute_name="foo",
             attribute_value="bar")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         LDAP mappers can be imported using the format `{{realm_id}}/{{ldap_user_federation_id}}/{{ldap_mapper_id}}`.
 
         The ID of the LDAP user federation provider and the mapper can be found within the Keycloak GUI, and they are typically GUIDs.
```

### Comparing `pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/ldap/hardcoded_group_mapper.py` & `pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/ldap/hardcoded_group_mapper.py`

 * *Files 2% similar despite different names*

```diff
@@ -165,15 +165,14 @@
         """
         Allows for creating and managing hardcoded group mappers for Keycloak users federated via LDAP.
 
         The LDAP hardcoded group mapper will grant a specified Keycloak group to each Keycloak user linked with LDAP.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
             realm="my-realm",
             enabled=True)
@@ -196,15 +195,14 @@
             name="my-group")
         assign_group_to_users = keycloak.ldap.HardcodedGroupMapper("assign_group_to_users",
             realm_id=realm.id,
             ldap_user_federation_id=ldap_user_federation.id,
             name="assign-group-to-users",
             group=realm_group.name)
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         LDAP mappers can be imported using the format `{{realm_id}}/{{ldap_user_federation_id}}/{{ldap_mapper_id}}`.
 
         The ID of the LDAP user federation provider and the mapper can be found within the Keycloak GUI, and they are typically GUIDs.
 
@@ -232,15 +230,14 @@
         """
         Allows for creating and managing hardcoded group mappers for Keycloak users federated via LDAP.
 
         The LDAP hardcoded group mapper will grant a specified Keycloak group to each Keycloak user linked with LDAP.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
             realm="my-realm",
             enabled=True)
@@ -263,15 +260,14 @@
             name="my-group")
         assign_group_to_users = keycloak.ldap.HardcodedGroupMapper("assign_group_to_users",
             realm_id=realm.id,
             ldap_user_federation_id=ldap_user_federation.id,
             name="assign-group-to-users",
             group=realm_group.name)
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         LDAP mappers can be imported using the format `{{realm_id}}/{{ldap_user_federation_id}}/{{ldap_mapper_id}}`.
 
         The ID of the LDAP user federation provider and the mapper can be found within the Keycloak GUI, and they are typically GUIDs.
```

### Comparing `pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/ldap/hardcoded_role_mapper.py` & `pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/ldap/hardcoded_role_mapper.py`

 * *Files 2% similar despite different names*

```diff
@@ -165,15 +165,14 @@
         """
         ## # ldap.HardcodedRoleMapper
 
         This mapper will grant a specified Keycloak role to each Keycloak user linked with LDAP.
 
         ### Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
             realm="test",
             enabled=True)
@@ -193,15 +192,14 @@
             bind_credential="admin")
         assign_admin_role_to_all_users = keycloak.ldap.HardcodedRoleMapper("assign_admin_role_to_all_users",
             realm_id=realm.id,
             ldap_user_federation_id=ldap_user_federation.id,
             name="assign-admin-role-to-all-users",
             role="admin")
         ```
-        <!--End PulumiCodeChooser -->
 
         ### Argument Reference
 
         The following arguments are supported:
 
         - `realm_id` - (Required) The realm that this LDAP mapper will exist in.
         - `ldap_user_federation_id` - (Required) The ID of the LDAP user federation provider to attach this mapper to.
@@ -230,15 +228,14 @@
         """
         ## # ldap.HardcodedRoleMapper
 
         This mapper will grant a specified Keycloak role to each Keycloak user linked with LDAP.
 
         ### Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
             realm="test",
             enabled=True)
@@ -258,15 +255,14 @@
             bind_credential="admin")
         assign_admin_role_to_all_users = keycloak.ldap.HardcodedRoleMapper("assign_admin_role_to_all_users",
             realm_id=realm.id,
             ldap_user_federation_id=ldap_user_federation.id,
             name="assign-admin-role-to-all-users",
             role="admin")
         ```
-        <!--End PulumiCodeChooser -->
 
         ### Argument Reference
 
         The following arguments are supported:
 
         - `realm_id` - (Required) The realm that this LDAP mapper will exist in.
         - `ldap_user_federation_id` - (Required) The ID of the LDAP user federation provider to attach this mapper to.
```

### Comparing `pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/ldap/msad_lds_user_account_control_mapper.py` & `pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/ldap/msad_lds_user_account_control_mapper.py`

 * *Files 4% similar despite different names*

```diff
@@ -137,15 +137,14 @@
         The MSAD-LDS (Microsoft Active Directory Lightweight Directory Service) user account control mapper is specific
         to LDAP user federation providers that are pulling from AD-LDS, and it can propagate
         AD-LDS user state to Keycloak in order to enforce settings like expired passwords
         or disabled accounts.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
             realm="my-realm",
             enabled=True)
@@ -165,15 +164,14 @@
             bind_dn="cn=admin,dc=example,dc=org",
             bind_credential="admin")
         msad_lds_user_account_control_mapper = keycloak.ldap.MsadLdsUserAccountControlMapper("msad_lds_user_account_control_mapper",
             realm_id=realm.id,
             ldap_user_federation_id=ldap_user_federation.id,
             name="msad-lds-user-account-control-mapper")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         LDAP mappers can be imported using the format `{{realm_id}}/{{ldap_user_federation_id}}/{{ldap_mapper_id}}`.
 
         The ID of the LDAP user federation provider and the mapper can be found within the Keycloak GUI, and they are typically GUIDs.
 
@@ -204,15 +202,14 @@
         The MSAD-LDS (Microsoft Active Directory Lightweight Directory Service) user account control mapper is specific
         to LDAP user federation providers that are pulling from AD-LDS, and it can propagate
         AD-LDS user state to Keycloak in order to enforce settings like expired passwords
         or disabled accounts.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
             realm="my-realm",
             enabled=True)
@@ -232,15 +229,14 @@
             bind_dn="cn=admin,dc=example,dc=org",
             bind_credential="admin")
         msad_lds_user_account_control_mapper = keycloak.ldap.MsadLdsUserAccountControlMapper("msad_lds_user_account_control_mapper",
             realm_id=realm.id,
             ldap_user_federation_id=ldap_user_federation.id,
             name="msad-lds-user-account-control-mapper")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         LDAP mappers can be imported using the format `{{realm_id}}/{{ldap_user_federation_id}}/{{ldap_mapper_id}}`.
 
         The ID of the LDAP user federation provider and the mapper can be found within the Keycloak GUI, and they are typically GUIDs.
```

### Comparing `pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/ldap/msad_user_account_control_mapper.py` & `pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/ldap/msad_user_account_control_mapper.py`

 * *Files 2% similar despite different names*

```diff
@@ -164,15 +164,14 @@
         The MSAD (Microsoft Active Directory) user account control mapper is specific
         to LDAP user federation providers that are pulling from AD, and it can propagate
         AD user state to Keycloak in order to enforce settings like expired passwords
         or disabled accounts.
 
         ### Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
             realm="test",
             enabled=True)
@@ -192,15 +191,14 @@
             bind_dn="cn=admin,dc=example,dc=org",
             bind_credential="admin")
         msad_user_account_control_mapper = keycloak.ldap.MsadUserAccountControlMapper("msad_user_account_control_mapper",
             realm_id=realm.id,
             ldap_user_federation_id=ldap_user_federation.id,
             name="msad-user-account-control-mapper")
         ```
-        <!--End PulumiCodeChooser -->
 
         ### Argument Reference
 
         The following arguments are supported:
 
         - `realm_id` - (Required) The realm that this LDAP mapper will exist in.
         - `ldap_user_federation_id` - (Required) The ID of the LDAP user federation provider to attach this mapper to.
@@ -234,15 +232,14 @@
         The MSAD (Microsoft Active Directory) user account control mapper is specific
         to LDAP user federation providers that are pulling from AD, and it can propagate
         AD user state to Keycloak in order to enforce settings like expired passwords
         or disabled accounts.
 
         ### Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
             realm="test",
             enabled=True)
@@ -262,15 +259,14 @@
             bind_dn="cn=admin,dc=example,dc=org",
             bind_credential="admin")
         msad_user_account_control_mapper = keycloak.ldap.MsadUserAccountControlMapper("msad_user_account_control_mapper",
             realm_id=realm.id,
             ldap_user_federation_id=ldap_user_federation.id,
             name="msad-user-account-control-mapper")
         ```
-        <!--End PulumiCodeChooser -->
 
         ### Argument Reference
 
         The following arguments are supported:
 
         - `realm_id` - (Required) The realm that this LDAP mapper will exist in.
         - `ldap_user_federation_id` - (Required) The ID of the LDAP user federation provider to attach this mapper to.
```

### Comparing `pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/ldap/outputs.py` & `pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/ldap/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/ldap/role_mapper.py` & `pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/ldap/role_mapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -524,15 +524,14 @@
         """
         Allows for creating and managing role mappers for Keycloak users federated via LDAP.
 
         The LDAP group mapper can be used to map an LDAP user's roles from some DN to Keycloak roles.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
             realm="my-realm",
             enabled=True)
@@ -559,15 +558,14 @@
             role_object_classes=["groupOfNames"],
             membership_attribute_type="DN",
             membership_ldap_attribute="member",
             membership_user_ldap_attribute="cn",
             user_roles_retrieve_strategy="GET_ROLES_FROM_USER_MEMBEROF_ATTRIBUTE",
             memberof_ldap_attribute="memberOf")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         LDAP mappers can be imported using the format `{{realm_id}}/{{ldap_user_federation_id}}/{{ldap_mapper_id}}`.
 
         The ID of the LDAP user federation provider and the mapper can be found within the Keycloak GUI, and they are typically GUIDs.
 
@@ -606,15 +604,14 @@
         """
         Allows for creating and managing role mappers for Keycloak users federated via LDAP.
 
         The LDAP group mapper can be used to map an LDAP user's roles from some DN to Keycloak roles.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
             realm="my-realm",
             enabled=True)
@@ -641,15 +638,14 @@
             role_object_classes=["groupOfNames"],
             membership_attribute_type="DN",
             membership_ldap_attribute="member",
             membership_user_ldap_attribute="cn",
             user_roles_retrieve_strategy="GET_ROLES_FROM_USER_MEMBEROF_ATTRIBUTE",
             memberof_ldap_attribute="memberOf")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         LDAP mappers can be imported using the format `{{realm_id}}/{{ldap_user_federation_id}}/{{ldap_mapper_id}}`.
 
         The ID of the LDAP user federation provider and the mapper can be found within the Keycloak GUI, and they are typically GUIDs.
```

### Comparing `pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/ldap/user_attribute_mapper.py` & `pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/ldap/user_attribute_mapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -366,15 +366,14 @@
         federated via LDAP.
 
         The LDAP user attribute mapper can be used to map a single LDAP attribute
         to an attribute on the Keycloak user model.
 
         ### Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
             realm="test",
             enabled=True)
@@ -395,15 +394,14 @@
         ldap_user_attribute_mapper = keycloak.ldap.UserAttributeMapper("ldap_user_attribute_mapper",
             realm_id=realm.id,
             ldap_user_federation_id=ldap_user_federation.id,
             name="user-attribute-mapper",
             user_model_attribute="foo",
             ldap_attribute="bar")
         ```
-        <!--End PulumiCodeChooser -->
 
         ### Argument Reference
 
         The following arguments are supported:
 
         - `realm_id` - (Required) The realm that this LDAP mapper will exist in.
         - `ldap_user_federation_id` - (Required) The ID of the LDAP user federation provider to attach this mapper to.
@@ -446,15 +444,14 @@
         federated via LDAP.
 
         The LDAP user attribute mapper can be used to map a single LDAP attribute
         to an attribute on the Keycloak user model.
 
         ### Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
             realm="test",
             enabled=True)
@@ -475,15 +472,14 @@
         ldap_user_attribute_mapper = keycloak.ldap.UserAttributeMapper("ldap_user_attribute_mapper",
             realm_id=realm.id,
             ldap_user_federation_id=ldap_user_federation.id,
             name="user-attribute-mapper",
             user_model_attribute="foo",
             ldap_attribute="bar")
         ```
-        <!--End PulumiCodeChooser -->
 
         ### Argument Reference
 
         The following arguments are supported:
 
         - `realm_id` - (Required) The realm that this LDAP mapper will exist in.
         - `ldap_user_federation_id` - (Required) The ID of the LDAP user federation provider to attach this mapper to.
```

### Comparing `pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/ldap/user_federation.py` & `pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/ldap/user_federation.py`

 * *Files 0% similar despite different names*

```diff
@@ -1092,15 +1092,14 @@
         Keycloak can use an LDAP user federation provider to federate users to Keycloak
         from a directory system such as LDAP or Active Directory. Federated users
         will exist within the realm and will be able to log in to clients. Federated
         users can have their attributes defined using mappers.
 
         ### Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
             realm="test",
             enabled=True)
@@ -1118,15 +1117,14 @@
             connection_url="ldap://openldap",
             users_dn="dc=example,dc=org",
             bind_dn="cn=admin,dc=example,dc=org",
             bind_credential="admin",
             connection_timeout="5s",
             read_timeout="10s")
         ```
-        <!--End PulumiCodeChooser -->
 
         ### Argument Reference
 
         The following arguments are supported:
 
         - `realm_id` - (Required) The realm that this provider will provide user federation for.
         - `name` - (Required) Display name of the provider when displayed in the console.
@@ -1216,15 +1214,14 @@
         Keycloak can use an LDAP user federation provider to federate users to Keycloak
         from a directory system such as LDAP or Active Directory. Federated users
         will exist within the realm and will be able to log in to clients. Federated
         users can have their attributes defined using mappers.
 
         ### Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
             realm="test",
             enabled=True)
@@ -1242,15 +1239,14 @@
             connection_url="ldap://openldap",
             users_dn="dc=example,dc=org",
             bind_dn="cn=admin,dc=example,dc=org",
             bind_credential="admin",
             connection_timeout="5s",
             read_timeout="10s")
         ```
-        <!--End PulumiCodeChooser -->
 
         ### Argument Reference
 
         The following arguments are supported:
 
         - `realm_id` - (Required) The realm that this provider will provide user federation for.
         - `name` - (Required) Display name of the provider when displayed in the console.
```

### Comparing `pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/oidc/google_identity_provider.py` & `pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/oidc/google_identity_provider.py`

 * *Files 1% similar despite different names*

```diff
@@ -799,15 +799,14 @@
         """
         Allows for creating and managing OIDC Identity Providers within Keycloak.
 
         OIDC (OpenID Connect) identity providers allows users to authenticate through a third party system using the OIDC standard.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
             realm="my-realm",
             enabled=True)
@@ -818,15 +817,14 @@
             trust_email=True,
             hosted_domain="example.com",
             sync_mode="IMPORT",
             extra_config={
                 "myCustomConfigKey": "myValue",
             })
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Google Identity providers can be imported using the format {{realm_id}}/{{idp_alias}}, where idp_alias is the identity provider alias.
 
         Example:
 
@@ -869,15 +867,14 @@
         """
         Allows for creating and managing OIDC Identity Providers within Keycloak.
 
         OIDC (OpenID Connect) identity providers allows users to authenticate through a third party system using the OIDC standard.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
             realm="my-realm",
             enabled=True)
@@ -888,15 +885,14 @@
             trust_email=True,
             hosted_domain="example.com",
             sync_mode="IMPORT",
             extra_config={
                 "myCustomConfigKey": "myValue",
             })
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Google Identity providers can be imported using the format {{realm_id}}/{{idp_alias}}, where idp_alias is the identity provider alias.
 
         Example:
```

### Comparing `pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/oidc/identity_provider.py` & `pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/oidc/identity_provider.py`

 * *Files 0% similar despite different names*

```diff
@@ -1061,15 +1061,14 @@
         """
         Allows for creating and managing OIDC Identity Providers within Keycloak.
 
         OIDC (OpenID Connect) identity providers allows users to authenticate through a third party system using the OIDC standard.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
             realm="my-realm",
             enabled=True)
@@ -1080,15 +1079,14 @@
             client_id="clientID",
             client_secret="clientSecret",
             token_url="https://tokenurl.com",
             extra_config={
                 "clientAuthMethod": "client_secret_post",
             })
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Identity providers can be imported using the format `{{realm_id}}/{{idp_alias}}`, where `idp_alias` is the identity provider alias.
 
         Example:
 
@@ -1140,15 +1138,14 @@
         """
         Allows for creating and managing OIDC Identity Providers within Keycloak.
 
         OIDC (OpenID Connect) identity providers allows users to authenticate through a third party system using the OIDC standard.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
             realm="my-realm",
             enabled=True)
@@ -1159,15 +1156,14 @@
             client_id="clientID",
             client_secret="clientSecret",
             token_url="https://tokenurl.com",
             extra_config={
                 "clientAuthMethod": "client_secret_post",
             })
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Identity providers can be imported using the format `{{realm_id}}/{{idp_alias}}`, where `idp_alias` is the identity provider alias.
 
         Example:
```

### Comparing `pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/openid/__init__.py` & `pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/openid/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/openid/_inputs.py` & `pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/openid/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/openid/audience_protocol_mapper.py` & `pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/openid/audience_protocol_mapper.py`

 * *Files 2% similar despite different names*

```diff
@@ -304,15 +304,14 @@
 
         Audience protocol mappers allow you add audiences to the `aud` claim
         within issued tokens. The audience can be a custom string, or it can be
         mapped to the ID of a pre-existing client.
 
         ### Example Usage (Client)
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
             realm="my-realm",
             enabled=True)
@@ -325,19 +324,17 @@
             valid_redirect_uris=["http://localhost:8080/openid-callback"])
         audience_mapper = keycloak.openid.AudienceProtocolMapper("audience_mapper",
             realm_id=realm.id,
             client_id=openid_client.id,
             name="audience-mapper",
             included_custom_audience="foo")
         ```
-        <!--End PulumiCodeChooser -->
 
         ### Example Usage (Client Scope)
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
             realm="my-realm",
             enabled=True)
@@ -346,15 +343,14 @@
             name="test-client-scope")
         audience_mapper = keycloak.openid.AudienceProtocolMapper("audience_mapper",
             realm_id=realm.id,
             client_scope_id=client_scope.id,
             name="audience-mapper",
             included_custom_audience="foo")
         ```
-        <!--End PulumiCodeChooser -->
 
         ### Argument Reference
 
         The following arguments are supported:
 
         - `realm_id` - (Required) The realm this protocol mapper exists within.
         - `client_id` - (Required if `client_scope_id` is not specified) The client this protocol mapper is attached to.
@@ -398,15 +394,14 @@
 
         Audience protocol mappers allow you add audiences to the `aud` claim
         within issued tokens. The audience can be a custom string, or it can be
         mapped to the ID of a pre-existing client.
 
         ### Example Usage (Client)
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
             realm="my-realm",
             enabled=True)
@@ -419,19 +414,17 @@
             valid_redirect_uris=["http://localhost:8080/openid-callback"])
         audience_mapper = keycloak.openid.AudienceProtocolMapper("audience_mapper",
             realm_id=realm.id,
             client_id=openid_client.id,
             name="audience-mapper",
             included_custom_audience="foo")
         ```
-        <!--End PulumiCodeChooser -->
 
         ### Example Usage (Client Scope)
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
             realm="my-realm",
             enabled=True)
@@ -440,15 +433,14 @@
             name="test-client-scope")
         audience_mapper = keycloak.openid.AudienceProtocolMapper("audience_mapper",
             realm_id=realm.id,
             client_scope_id=client_scope.id,
             name="audience-mapper",
             included_custom_audience="foo")
         ```
-        <!--End PulumiCodeChooser -->
 
         ### Argument Reference
 
         The following arguments are supported:
 
         - `realm_id` - (Required) The realm this protocol mapper exists within.
         - `client_id` - (Required if `client_scope_id` is not specified) The client this protocol mapper is attached to.
```

### Comparing `pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/openid/audience_resolve_protocol_mapper.py` & `pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/openid/audience_resolve_protocol_mapper.py`

 * *Files 2% similar despite different names*

```diff
@@ -171,15 +171,14 @@
         to imply which audiences are appropriate for the token. See the
         [Keycloak docs](https://www.keycloak.org/docs/latest/server_admin/#_audience_resolve) for more details.
 
         ## Example Usage
 
         ### Client)
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
             realm="my-realm",
             enabled=True)
@@ -191,34 +190,31 @@
             access_type="CONFIDENTIAL",
             valid_redirect_uris=["http://localhost:8080/openid-callback"])
         audience_mapper = keycloak.openid.AudienceResolveProtocolMapper("audience_mapper",
             realm_id=realm.id,
             client_id=openid_client.id,
             name="my-audience-resolve-mapper")
         ```
-        <!--End PulumiCodeChooser -->
 
         ### Client Scope)
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
             realm="my-realm",
             enabled=True)
         client_scope = keycloak.openid.ClientScope("client_scope",
             realm_id=realm.id,
             name="test-client-scope")
         audience_mapper = keycloak.openid.AudienceProtocolMapper("audience_mapper",
             realm_id=realm.id,
             client_scope_id=client_scope.id)
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Protocol mappers can be imported using one of the following formats:
 
         - Client: `{{realm_id}}/client/{{client_keycloak_id}}/{{protocol_mapper_id}}`
 
@@ -256,15 +252,14 @@
         to imply which audiences are appropriate for the token. See the
         [Keycloak docs](https://www.keycloak.org/docs/latest/server_admin/#_audience_resolve) for more details.
 
         ## Example Usage
 
         ### Client)
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
             realm="my-realm",
             enabled=True)
@@ -276,34 +271,31 @@
             access_type="CONFIDENTIAL",
             valid_redirect_uris=["http://localhost:8080/openid-callback"])
         audience_mapper = keycloak.openid.AudienceResolveProtocolMapper("audience_mapper",
             realm_id=realm.id,
             client_id=openid_client.id,
             name="my-audience-resolve-mapper")
         ```
-        <!--End PulumiCodeChooser -->
 
         ### Client Scope)
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
             realm="my-realm",
             enabled=True)
         client_scope = keycloak.openid.ClientScope("client_scope",
             realm_id=realm.id,
             name="test-client-scope")
         audience_mapper = keycloak.openid.AudienceProtocolMapper("audience_mapper",
             realm_id=realm.id,
             client_scope_id=client_scope.id)
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Protocol mappers can be imported using one of the following formats:
 
         - Client: `{{realm_id}}/client/{{client_keycloak_id}}/{{protocol_mapper_id}}`
```

### Comparing `pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/openid/audience_resolve_protocol_mappter.py` & `pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/openid/audience_resolve_protocol_mappter.py`

 * *Files 2% similar despite different names*

```diff
@@ -176,15 +176,14 @@
         to imply which audiences are appropriate for the token. See the
         [Keycloak docs](https://www.keycloak.org/docs/latest/server_admin/#_audience_resolve) for more details.
 
         ## Example Usage
 
         ### Client)
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
             realm="my-realm",
             enabled=True)
@@ -196,34 +195,31 @@
             access_type="CONFIDENTIAL",
             valid_redirect_uris=["http://localhost:8080/openid-callback"])
         audience_mapper = keycloak.openid.AudienceResolveProtocolMapper("audience_mapper",
             realm_id=realm.id,
             client_id=openid_client.id,
             name="my-audience-resolve-mapper")
         ```
-        <!--End PulumiCodeChooser -->
 
         ### Client Scope)
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
             realm="my-realm",
             enabled=True)
         client_scope = keycloak.openid.ClientScope("client_scope",
             realm_id=realm.id,
             name="test-client-scope")
         audience_mapper = keycloak.openid.AudienceProtocolMapper("audience_mapper",
             realm_id=realm.id,
             client_scope_id=client_scope.id)
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Protocol mappers can be imported using one of the following formats:
 
         - Client: `{{realm_id}}/client/{{client_keycloak_id}}/{{protocol_mapper_id}}`
 
@@ -261,15 +257,14 @@
         to imply which audiences are appropriate for the token. See the
         [Keycloak docs](https://www.keycloak.org/docs/latest/server_admin/#_audience_resolve) for more details.
 
         ## Example Usage
 
         ### Client)
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
             realm="my-realm",
             enabled=True)
@@ -281,34 +276,31 @@
             access_type="CONFIDENTIAL",
             valid_redirect_uris=["http://localhost:8080/openid-callback"])
         audience_mapper = keycloak.openid.AudienceResolveProtocolMapper("audience_mapper",
             realm_id=realm.id,
             client_id=openid_client.id,
             name="my-audience-resolve-mapper")
         ```
-        <!--End PulumiCodeChooser -->
 
         ### Client Scope)
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
             realm="my-realm",
             enabled=True)
         client_scope = keycloak.openid.ClientScope("client_scope",
             realm_id=realm.id,
             name="test-client-scope")
         audience_mapper = keycloak.openid.AudienceProtocolMapper("audience_mapper",
             realm_id=realm.id,
             client_scope_id=client_scope.id)
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Protocol mappers can be imported using one of the following formats:
 
         - Client: `{{realm_id}}/client/{{client_keycloak_id}}/{{protocol_mapper_id}}`
```

### Comparing `pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/openid/client.py` & `pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/openid/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1163,15 +1163,14 @@
 
         Clients are entities that can use Keycloak for user authentication. Typically,
         clients are applications that redirect users to Keycloak for authentication
         in order to take advantage of Keycloak's user sessions for SSO.
 
         ### Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
             realm="my-realm",
             enabled=True)
@@ -1179,15 +1178,14 @@
             realm_id=realm.id,
             client_id="test-client",
             name="test client",
             enabled=True,
             access_type="CONFIDENTIAL",
             valid_redirect_uris=["http://localhost:8080/openid-callback"])
         ```
-        <!--End PulumiCodeChooser -->
 
         ### Argument Reference
 
         The following arguments are supported:
 
         - `realm_id` - (Required) The realm this client is attached to.
         - `client_id` - (Required) The unique ID of this client, referenced in the URI during authentication and in issued tokens.
@@ -1244,15 +1242,14 @@
 
         Clients are entities that can use Keycloak for user authentication. Typically,
         clients are applications that redirect users to Keycloak for authentication
         in order to take advantage of Keycloak's user sessions for SSO.
 
         ### Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
             realm="my-realm",
             enabled=True)
@@ -1260,15 +1257,14 @@
             realm_id=realm.id,
             client_id="test-client",
             name="test client",
             enabled=True,
             access_type="CONFIDENTIAL",
             valid_redirect_uris=["http://localhost:8080/openid-callback"])
         ```
-        <!--End PulumiCodeChooser -->
 
         ### Argument Reference
 
         The following arguments are supported:
 
         - `realm_id` - (Required) The realm this client is attached to.
         - `client_id` - (Required) The unique ID of this client, referenced in the URI during authentication and in issued tokens.
```

### Comparing `pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/openid/client_aggregate_policy.py` & `pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/openid/client_aggregate_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/openid/client_authorization_permission.py` & `pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/openid/client_authorization_permission.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/openid/client_authorization_resource.py` & `pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/openid/client_authorization_resource.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/openid/client_authorization_scope.py` & `pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/openid/client_authorization_scope.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/openid/client_default_scopes.py` & `pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/openid/client_default_scopes.py`

 * *Files 2% similar despite different names*

```diff
@@ -104,15 +104,14 @@
                  client_id: Optional[pulumi.Input[str]] = None,
                  default_scopes: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  realm_id: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
             realm="my-realm",
             enabled=True)
@@ -130,15 +129,14 @@
                 "profile",
                 "email",
                 "roles",
                 "web-origins",
                 client_scope.name,
             ])
         ```
-        <!--End PulumiCodeChooser -->
 
         ### Argument Reference
 
         The following arguments are supported:
 
         - `realm_id` - (Required) The realm this client and scopes exists in.
         - `client_id` - (Required) The ID of the client to attach default scopes to. Note that this is the unique ID of the client generated by Keycloak.
@@ -157,15 +155,14 @@
     def __init__(__self__,
                  resource_name: str,
                  args: ClientDefaultScopesArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
             realm="my-realm",
             enabled=True)
@@ -183,15 +180,14 @@
                 "profile",
                 "email",
                 "roles",
                 "web-origins",
                 client_scope.name,
             ])
         ```
-        <!--End PulumiCodeChooser -->
 
         ### Argument Reference
 
         The following arguments are supported:
 
         - `realm_id` - (Required) The realm this client and scopes exists in.
         - `client_id` - (Required) The ID of the client to attach default scopes to. Note that this is the unique ID of the client generated by Keycloak.
```

### Comparing `pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/openid/client_group_policy.py` & `pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/openid/client_group_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/openid/client_js_policy.py` & `pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/openid/client_js_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/openid/client_optional_scopes.py` & `pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/openid/client_optional_scopes.py`

 * *Files 2% similar despite different names*

```diff
@@ -104,15 +104,14 @@
                  client_id: Optional[pulumi.Input[str]] = None,
                  optional_scopes: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  realm_id: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
             realm="my-realm",
             enabled=True)
@@ -129,15 +128,14 @@
             optional_scopes=[
                 "address",
                 "phone",
                 "offline_access",
                 client_scope.name,
             ])
         ```
-        <!--End PulumiCodeChooser -->
 
         ### Argument Reference
 
         The following arguments are supported:
 
         - `realm_id` - (Required) The realm this client and scopes exists in.
         - `client_id` - (Required) The ID of the client to attach optional scopes to. Note that this is the unique ID of the client generated by Keycloak.
@@ -156,15 +154,14 @@
     def __init__(__self__,
                  resource_name: str,
                  args: ClientOptionalScopesArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
             realm="my-realm",
             enabled=True)
@@ -181,15 +178,14 @@
             optional_scopes=[
                 "address",
                 "phone",
                 "offline_access",
                 client_scope.name,
             ])
         ```
-        <!--End PulumiCodeChooser -->
 
         ### Argument Reference
 
         The following arguments are supported:
 
         - `realm_id` - (Required) The realm this client and scopes exists in.
         - `client_id` - (Required) The ID of the client to attach optional scopes to. Note that this is the unique ID of the client generated by Keycloak.
```

### Comparing `pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/openid/client_permissions.py` & `pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/openid/client_permissions.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/openid/client_policy.py` & `pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/openid/client_policy.py`

 * *Files 0% similar despite different names*

```diff
@@ -264,15 +264,14 @@
         """
         This resource can be used to create client policy.
 
         ## Example Usage
 
         In this example, we'll create a new OpenID client, then enabled permissions for the client. A client without permissions disabled cannot be assigned by a client policy. We'll use the `openid.ClientPolicy` resource to create a new client policy, which could be applied to many clients, for a realm and a resource_server_id.
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
             realm="my-realm",
             enabled=True)
@@ -291,15 +290,14 @@
             resource_server_id=realm_management.id,
             realm_id=realm.id,
             name="my-policy",
             logic="POSITIVE",
             decision_strategy="UNANIMOUS",
             clients=[openid_client.id])
         ```
-        <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] clients: The clients allowed by this client policy.
         :param pulumi.Input[str] decision_strategy: (Computed) Dictates how the policies associated with a given permission are evaluated and how a final decision is obtained. Could be one of `AFFIRMATIVE`, `CONSENSUS`, or `UNANIMOUS`. Applies to permissions.
         :param pulumi.Input[str] description: The description of this client policy.
         :param pulumi.Input[str] logic: (Computed) Dictates how the policy decision should be made. Can be either `POSITIVE` or `NEGATIVE`. Applies to policies.
@@ -316,15 +314,14 @@
         """
         This resource can be used to create client policy.
 
         ## Example Usage
 
         In this example, we'll create a new OpenID client, then enabled permissions for the client. A client without permissions disabled cannot be assigned by a client policy. We'll use the `openid.ClientPolicy` resource to create a new client policy, which could be applied to many clients, for a realm and a resource_server_id.
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
             realm="my-realm",
             enabled=True)
@@ -343,15 +340,14 @@
             resource_server_id=realm_management.id,
             realm_id=realm.id,
             name="my-policy",
             logic="POSITIVE",
             decision_strategy="UNANIMOUS",
             clients=[openid_client.id])
         ```
-        <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param ClientPolicyArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
```

### Comparing `pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/openid/client_role_policy.py` & `pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/openid/client_role_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/openid/client_scope.py` & `pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/openid/client_scope.py`

 * *Files 1% similar despite different names*

```diff
@@ -190,28 +190,26 @@
 
         Client Scopes can be used to share common protocol and role mappings between multiple
         clients within a realm. They can also be used by clients to conditionally request
         claims or roles for a user based on the OAuth 2.0 `scope` parameter.
 
         ### Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
             realm="my-realm",
             enabled=True)
         openid_client_scope = keycloak.openid.ClientScope("openid_client_scope",
             realm_id=realm.id,
             name="groups",
             description="When requested, this scope will map a user's group memberships to a claim")
         ```
-        <!--End PulumiCodeChooser -->
 
         ### Argument Reference
 
         The following arguments are supported:
 
         - `realm_id` - (Required) The realm this client scope belongs to.
         - `name` - (Required) The display name of this client scope in the GUI.
@@ -244,28 +242,26 @@
 
         Client Scopes can be used to share common protocol and role mappings between multiple
         clients within a realm. They can also be used by clients to conditionally request
         claims or roles for a user based on the OAuth 2.0 `scope` parameter.
 
         ### Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
             realm="my-realm",
             enabled=True)
         openid_client_scope = keycloak.openid.ClientScope("openid_client_scope",
             realm_id=realm.id,
             name="groups",
             description="When requested, this scope will map a user's group memberships to a claim")
         ```
-        <!--End PulumiCodeChooser -->
 
         ### Argument Reference
 
         The following arguments are supported:
 
         - `realm_id` - (Required) The realm this client scope belongs to.
         - `name` - (Required) The display name of this client scope in the GUI.
```

### Comparing `pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/openid/client_service_account_realm_role.py` & `pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/openid/client_service_account_realm_role.py`

 * *Files 1% similar despite different names*

```diff
@@ -134,15 +134,14 @@
         You need to set `service_accounts_enabled` to `true` for the openid client that should be assigned the role.
 
         If you'd like to attach client roles to a service account, please use the `openid.ClientServiceAccountRole`
         resource.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
             realm="my-realm",
             enabled=True)
@@ -154,15 +153,14 @@
             name="client",
             service_accounts_enabled=True)
         client_service_account_role = keycloak.openid.ClientServiceAccountRealmRole("client_service_account_role",
             realm_id=realm.id,
             service_account_user_id=client.service_account_user_id,
             role=realm_role.name)
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         This resource can be imported using the format `{{realmId}}/{{serviceAccountUserId}}/{{roleId}}`.
 
         Example:
 
@@ -189,15 +187,14 @@
         You need to set `service_accounts_enabled` to `true` for the openid client that should be assigned the role.
 
         If you'd like to attach client roles to a service account, please use the `openid.ClientServiceAccountRole`
         resource.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
             realm="my-realm",
             enabled=True)
@@ -209,15 +206,14 @@
             name="client",
             service_accounts_enabled=True)
         client_service_account_role = keycloak.openid.ClientServiceAccountRealmRole("client_service_account_role",
             realm_id=realm.id,
             service_account_user_id=client.service_account_user_id,
             role=realm_role.name)
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         This resource can be imported using the format `{{realmId}}/{{serviceAccountUserId}}/{{roleId}}`.
 
         Example:
```

### Comparing `pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/openid/client_service_account_role.py` & `pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/openid/client_service_account_role.py`

 * *Files 0% similar despite different names*

```diff
@@ -166,15 +166,14 @@
         You need to set `service_accounts_enabled` to `true` for the openid client that should be assigned the role.
 
         If you'd like to attach realm roles to a service account, please use the `openid.ClientServiceAccountRealmRole`
         resource.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
             realm="my-realm",
             enabled=True)
@@ -194,15 +193,14 @@
             service_accounts_enabled=True)
         client2_service_account_role = keycloak.openid.ClientServiceAccountRole("client2_service_account_role",
             realm_id=realm.id,
             service_account_user_id=client2.service_account_user_id,
             client_id=client1.id,
             role=client1_role.name)
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         This resource can be imported using the format `{{realmId}}/{{serviceAccountUserId}}/{{clientId}}/{{roleId}}`.
 
         Example:
 
@@ -230,15 +228,14 @@
         You need to set `service_accounts_enabled` to `true` for the openid client that should be assigned the role.
 
         If you'd like to attach realm roles to a service account, please use the `openid.ClientServiceAccountRealmRole`
         resource.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
             realm="my-realm",
             enabled=True)
@@ -258,15 +255,14 @@
             service_accounts_enabled=True)
         client2_service_account_role = keycloak.openid.ClientServiceAccountRole("client2_service_account_role",
             realm_id=realm.id,
             service_account_user_id=client2.service_account_user_id,
             client_id=client1.id,
             role=client1_role.name)
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         This resource can be imported using the format `{{realmId}}/{{serviceAccountUserId}}/{{clientId}}/{{roleId}}`.
 
         Example:
```

### Comparing `pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/openid/client_time_policy.py` & `pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/openid/client_time_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/openid/client_user_policy.py` & `pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/openid/client_user_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/openid/full_name_protocol_mapper.py` & `pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/openid/full_name_protocol_mapper.py`

 * *Files 3% similar despite different names*

```diff
@@ -248,15 +248,14 @@
         Full name protocol mappers allow you to map a user's first and last name
         to the OpenID Connect `name` claim in a token. Protocol mappers can be defined
         for a single client, or they can be defined for a client scope which can
         be shared between multiple different clients.
 
         ### Example Usage (Client)
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
             realm="my-realm",
             enabled=True)
@@ -268,19 +267,17 @@
             access_type="CONFIDENTIAL",
             valid_redirect_uris=["http://localhost:8080/openid-callback"])
         full_name_mapper = keycloak.openid.FullNameProtocolMapper("full_name_mapper",
             realm_id=realm.id,
             client_id=openid_client.id,
             name="full-name-mapper")
         ```
-        <!--End PulumiCodeChooser -->
 
         ### Example Usage (Client Scope)
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
             realm="my-realm",
             enabled=True)
@@ -288,15 +285,14 @@
             realm_id=realm.id,
             name="test-client-scope")
         full_name_mapper = keycloak.openid.FullNameProtocolMapper("full_name_mapper",
             realm_id=realm.id,
             client_scope_id=client_scope.id,
             name="full-name-mapper")
         ```
-        <!--End PulumiCodeChooser -->
 
         ### Argument Reference
 
         The following arguments are supported:
 
         - `realm_id` - (Required) The realm this protocol mapper exists within.
         - `client_id` - (Required if `client_scope_id` is not specified) The client this protocol mapper is attached to.
@@ -336,15 +332,14 @@
         Full name protocol mappers allow you to map a user's first and last name
         to the OpenID Connect `name` claim in a token. Protocol mappers can be defined
         for a single client, or they can be defined for a client scope which can
         be shared between multiple different clients.
 
         ### Example Usage (Client)
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
             realm="my-realm",
             enabled=True)
@@ -356,19 +351,17 @@
             access_type="CONFIDENTIAL",
             valid_redirect_uris=["http://localhost:8080/openid-callback"])
         full_name_mapper = keycloak.openid.FullNameProtocolMapper("full_name_mapper",
             realm_id=realm.id,
             client_id=openid_client.id,
             name="full-name-mapper")
         ```
-        <!--End PulumiCodeChooser -->
 
         ### Example Usage (Client Scope)
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
             realm="my-realm",
             enabled=True)
@@ -376,15 +369,14 @@
             realm_id=realm.id,
             name="test-client-scope")
         full_name_mapper = keycloak.openid.FullNameProtocolMapper("full_name_mapper",
             realm_id=realm.id,
             client_scope_id=client_scope.id,
             name="full-name-mapper")
         ```
-        <!--End PulumiCodeChooser -->
 
         ### Argument Reference
 
         The following arguments are supported:
 
         - `realm_id` - (Required) The realm this protocol mapper exists within.
         - `client_id` - (Required if `client_scope_id` is not specified) The client this protocol mapper is attached to.
```

### Comparing `pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/openid/get_client.py` & `pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/openid/get_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -462,27 +462,25 @@
     """
     ## # openid.Client data source
 
     This data source can be used to fetch properties of a Keycloak OpenID client for usage with other resources.
 
     ### Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_keycloak as keycloak
 
     realm_management = keycloak.openid.get_client(realm_id="my-realm",
         client_id="realm-management")
     # use the data source
     admin = keycloak.get_role(realm_id="my-realm",
         client_id=realm_management.id,
         name="realm-admin")
     ```
-    <!--End PulumiCodeChooser -->
 
     ### Argument Reference
 
     The following arguments are supported:
 
     - `realm_id` - (Required) The realm id.
     - `client_id` - (Required) The client id.
@@ -565,27 +563,25 @@
     """
     ## # openid.Client data source
 
     This data source can be used to fetch properties of a Keycloak OpenID client for usage with other resources.
 
     ### Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_keycloak as keycloak
 
     realm_management = keycloak.openid.get_client(realm_id="my-realm",
         client_id="realm-management")
     # use the data source
     admin = keycloak.get_role(realm_id="my-realm",
         client_id=realm_management.id,
         name="realm-admin")
     ```
-    <!--End PulumiCodeChooser -->
 
     ### Argument Reference
 
     The following arguments are supported:
 
     - `realm_id` - (Required) The realm id.
     - `client_id` - (Required) The client id.
```

### Comparing `pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/openid/get_client_authorization_policy.py` & `pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/openid/get_client_authorization_policy.py`

 * *Files 6% similar despite different names*

```diff
@@ -164,15 +164,14 @@
 
     ## Example Usage
 
     In this example, we'll create a new OpenID client with authorization enabled. This will cause Keycloak to create a default
     permission for this client called "Default Permission". We'll use the `openid_get_client_authorization_policy` data
     source to fetch information about this permission, so we can use it to create a new resource-based authorization permission.
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_keycloak as keycloak
 
     realm = keycloak.Realm("realm",
         realm="my-realm",
         enabled=True)
@@ -199,15 +198,14 @@
     permission = keycloak.openid.ClientAuthorizationPermission("permission",
         resource_server_id=client_with_authz.resource_server_id,
         realm_id=realm.id,
         name="authorization-permission",
         policies=[default_permission.id],
         resources=[resource.id])
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str name: The name of the authorization policy.
     :param str realm_id: The realm this authorization policy exists within.
     :param str resource_server_id: The ID of the resource server this authorization policy is attached to.
     """
     __args__ = dict()
@@ -241,15 +239,14 @@
 
     ## Example Usage
 
     In this example, we'll create a new OpenID client with authorization enabled. This will cause Keycloak to create a default
     permission for this client called "Default Permission". We'll use the `openid_get_client_authorization_policy` data
     source to fetch information about this permission, so we can use it to create a new resource-based authorization permission.
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_keycloak as keycloak
 
     realm = keycloak.Realm("realm",
         realm="my-realm",
         enabled=True)
@@ -276,15 +273,14 @@
     permission = keycloak.openid.ClientAuthorizationPermission("permission",
         resource_server_id=client_with_authz.resource_server_id,
         realm_id=realm.id,
         name="authorization-permission",
         policies=[default_permission.id],
         resources=[resource.id])
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str name: The name of the authorization policy.
     :param str realm_id: The realm this authorization policy exists within.
     :param str resource_server_id: The ID of the resource server this authorization policy is attached to.
     """
     ...
```

### Comparing `pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/openid/get_client_scope.py` & `pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/openid/get_client_scope.py`

 * *Files 2% similar despite different names*

```diff
@@ -102,29 +102,27 @@
                      realm_id: Optional[str] = None,
                      opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetClientScopeResult:
     """
     This data source can be used to fetch properties of a Keycloak OpenID client scope for usage with other resources.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_keycloak as keycloak
 
     offline_access = keycloak.openid.get_client_scope(realm_id="my-realm",
         name="offline_access")
     # use the data source
     audience_mapper = keycloak.openid.AudienceProtocolMapper("audience_mapper",
         realm_id=offline_access.realm_id,
         client_scope_id=offline_access.id,
         name="audience-mapper",
         included_custom_audience="foo")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str name: The name of the client scope.
     :param str realm_id: The realm id.
     """
     __args__ = dict()
     __args__['name'] = name
@@ -147,28 +145,26 @@
                             realm_id: Optional[pulumi.Input[str]] = None,
                             opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetClientScopeResult]:
     """
     This data source can be used to fetch properties of a Keycloak OpenID client scope for usage with other resources.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_keycloak as keycloak
 
     offline_access = keycloak.openid.get_client_scope(realm_id="my-realm",
         name="offline_access")
     # use the data source
     audience_mapper = keycloak.openid.AudienceProtocolMapper("audience_mapper",
         realm_id=offline_access.realm_id,
         client_scope_id=offline_access.id,
         name="audience-mapper",
         included_custom_audience="foo")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str name: The name of the client scope.
     :param str realm_id: The realm id.
     """
     ...
```

### Comparing `pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/openid/get_client_service_account_user.py` & `pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/openid/get_client_service_account_user.py`

 * *Files 2% similar despite different names*

```diff
@@ -153,15 +153,14 @@
 
     ## Example Usage
 
     In this example, we'll create an OpenID client with service accounts enabled. This causes Keycloak to create a special user
     that represents the service account. We'll use this data source to grab this user's ID in order to assign some roles to this
     user, using the `UserRoles` resource.
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_keycloak as keycloak
 
     realm = keycloak.Realm("realm",
         realm="my-realm",
         enabled=True)
@@ -176,15 +175,14 @@
     offline_access = keycloak.get_role_output(realm_id=realm.id,
         name="offline_access")
     service_account_user_roles = keycloak.UserRoles("service_account_user_roles",
         realm_id=realm.id,
         user_id=service_account_user.id,
         role_ids=[offline_access.id])
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str client_id: The ID of the OpenID client with service accounts enabled.
     :param str realm_id: The realm that the OpenID client exists within.
     """
     __args__ = dict()
     __args__['clientId'] = client_id
@@ -217,15 +215,14 @@
 
     ## Example Usage
 
     In this example, we'll create an OpenID client with service accounts enabled. This causes Keycloak to create a special user
     that represents the service account. We'll use this data source to grab this user's ID in order to assign some roles to this
     user, using the `UserRoles` resource.
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_keycloak as keycloak
 
     realm = keycloak.Realm("realm",
         realm="my-realm",
         enabled=True)
@@ -240,14 +237,13 @@
     offline_access = keycloak.get_role_output(realm_id=realm.id,
         name="offline_access")
     service_account_user_roles = keycloak.UserRoles("service_account_user_roles",
         realm_id=realm.id,
         user_id=service_account_user.id,
         role_ids=[offline_access.id])
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str client_id: The ID of the OpenID client with service accounts enabled.
     :param str realm_id: The realm that the OpenID client exists within.
     """
     ...
```

### Comparing `pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/openid/group_membership_protocol_mapper.py` & `pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/openid/group_membership_protocol_mapper.py`

 * *Files 2% similar despite different names*

```diff
@@ -297,15 +297,14 @@
         Group membership protocol mappers allow you to map a user's group memberships
         to a claim in a token. Protocol mappers can be defined for a single client,
         or they can be defined for a client scope which can be shared between multiple
         different clients.
 
         ### Example Usage (Client)
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
             realm="my-realm",
             enabled=True)
@@ -318,19 +317,17 @@
             valid_redirect_uris=["http://localhost:8080/openid-callback"])
         group_membership_mapper = keycloak.openid.GroupMembershipProtocolMapper("group_membership_mapper",
             realm_id=realm.id,
             client_id=openid_client.id,
             name="group-membership-mapper",
             claim_name="groups")
         ```
-        <!--End PulumiCodeChooser -->
 
         ### Example Usage (Client Scope)
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
             realm="my-realm",
             enabled=True)
@@ -339,15 +336,14 @@
             name="test-client-scope")
         group_membership_mapper = keycloak.openid.GroupMembershipProtocolMapper("group_membership_mapper",
             realm_id=realm.id,
             client_scope_id=client_scope.id,
             name="group-membership-mapper",
             claim_name="groups")
         ```
-        <!--End PulumiCodeChooser -->
 
         ### Argument Reference
 
         The following arguments are supported:
 
         - `realm_id` - (Required) The realm this protocol mapper exists within.
         - `client_id` - (Required if `client_scope_id` is not specified) The client this protocol mapper is attached to.
@@ -389,15 +385,14 @@
         Group membership protocol mappers allow you to map a user's group memberships
         to a claim in a token. Protocol mappers can be defined for a single client,
         or they can be defined for a client scope which can be shared between multiple
         different clients.
 
         ### Example Usage (Client)
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
             realm="my-realm",
             enabled=True)
@@ -410,19 +405,17 @@
             valid_redirect_uris=["http://localhost:8080/openid-callback"])
         group_membership_mapper = keycloak.openid.GroupMembershipProtocolMapper("group_membership_mapper",
             realm_id=realm.id,
             client_id=openid_client.id,
             name="group-membership-mapper",
             claim_name="groups")
         ```
-        <!--End PulumiCodeChooser -->
 
         ### Example Usage (Client Scope)
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
             realm="my-realm",
             enabled=True)
@@ -431,15 +424,14 @@
             name="test-client-scope")
         group_membership_mapper = keycloak.openid.GroupMembershipProtocolMapper("group_membership_mapper",
             realm_id=realm.id,
             client_scope_id=client_scope.id,
             name="group-membership-mapper",
             claim_name="groups")
         ```
-        <!--End PulumiCodeChooser -->
 
         ### Argument Reference
 
         The following arguments are supported:
 
         - `realm_id` - (Required) The realm this protocol mapper exists within.
         - `client_id` - (Required if `client_scope_id` is not specified) The client this protocol mapper is attached to.
```

### Comparing `pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/openid/hardcoded_claim_protocol_mapper.py` & `pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/openid/hardcoded_claim_protocol_mapper.py`

 * *Files 2% similar despite different names*

```diff
@@ -353,15 +353,14 @@
         Hardcoded claim protocol mappers allow you to define a claim with a hardcoded
         value. Protocol mappers can be defined for a single client, or they can
         be defined for a client scope which can be shared between multiple different
         clients.
 
         ### Example Usage (Client)
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
             realm="my-realm",
             enabled=True)
@@ -375,19 +374,17 @@
         hardcoded_claim_mapper = keycloak.openid.HardcodedClaimProtocolMapper("hardcoded_claim_mapper",
             realm_id=realm.id,
             client_id=openid_client.id,
             name="hardcoded-claim-mapper",
             claim_name="foo",
             claim_value="bar")
         ```
-        <!--End PulumiCodeChooser -->
 
         ### Example Usage (Client Scope)
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
             realm="my-realm",
             enabled=True)
@@ -397,15 +394,14 @@
         hardcoded_claim_mapper = keycloak.openid.HardcodedClaimProtocolMapper("hardcoded_claim_mapper",
             realm_id=realm.id,
             client_scope_id=client_scope.id,
             name="hardcoded-claim-mapper",
             claim_name="foo",
             claim_value="bar")
         ```
-        <!--End PulumiCodeChooser -->
 
         ### Argument Reference
 
         The following arguments are supported:
 
         - `realm_id` - (Required) The realm this protocol mapper exists within.
         - `client_id` - (Required if `client_scope_id` is not specified) The client this protocol mapper is attached to.
@@ -452,15 +448,14 @@
         Hardcoded claim protocol mappers allow you to define a claim with a hardcoded
         value. Protocol mappers can be defined for a single client, or they can
         be defined for a client scope which can be shared between multiple different
         clients.
 
         ### Example Usage (Client)
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
             realm="my-realm",
             enabled=True)
@@ -474,19 +469,17 @@
         hardcoded_claim_mapper = keycloak.openid.HardcodedClaimProtocolMapper("hardcoded_claim_mapper",
             realm_id=realm.id,
             client_id=openid_client.id,
             name="hardcoded-claim-mapper",
             claim_name="foo",
             claim_value="bar")
         ```
-        <!--End PulumiCodeChooser -->
 
         ### Example Usage (Client Scope)
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
             realm="my-realm",
             enabled=True)
@@ -496,15 +489,14 @@
         hardcoded_claim_mapper = keycloak.openid.HardcodedClaimProtocolMapper("hardcoded_claim_mapper",
             realm_id=realm.id,
             client_scope_id=client_scope.id,
             name="hardcoded-claim-mapper",
             claim_name="foo",
             claim_value="bar")
         ```
-        <!--End PulumiCodeChooser -->
 
         ### Argument Reference
 
         The following arguments are supported:
 
         - `realm_id` - (Required) The realm this protocol mapper exists within.
         - `client_id` - (Required if `client_scope_id` is not specified) The client this protocol mapper is attached to.
```

### Comparing `pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/openid/hardcoded_role_protocol_mapper.py` & `pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/openid/hardcoded_role_protocol_mapper.py`

 * *Files 4% similar despite different names*

```diff
@@ -197,15 +197,14 @@
         Hardcoded role protocol mappers allow you to specify a single role to
         always map to an access token for a client. Protocol mappers can be
         defined for a single client, or they can be defined for a client scope
         which can be shared between multiple different clients.
 
         ### Example Usage (Client)
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
             realm="my-realm",
             enabled=True)
@@ -221,19 +220,17 @@
             valid_redirect_uris=["http://localhost:8080/openid-callback"])
         hardcoded_role_mapper = keycloak.openid.HardcodedRoleProtocolMapper("hardcoded_role_mapper",
             realm_id=realm.id,
             client_id=openid_client.id,
             name="hardcoded-role-mapper",
             role_id=role.id)
         ```
-        <!--End PulumiCodeChooser -->
 
         ### Example Usage (Client Scope)
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
             realm="my-realm",
             enabled=True)
@@ -245,15 +242,14 @@
             name="test-client-scope")
         hardcoded_role_mapper = keycloak.openid.HardcodedRoleProtocolMapper("hardcoded_role_mapper",
             realm_id=realm.id,
             client_scope_id=client_scope.id,
             name="hardcoded-role-mapper",
             role_id=role.id)
         ```
-        <!--End PulumiCodeChooser -->
 
         ### Argument Reference
 
         The following arguments are supported:
 
         - `realm_id` - (Required) The realm this protocol mapper exists within.
         - `client_id` - (Required if `client_scope_id` is not specified) The client this protocol mapper is attached to.
@@ -292,15 +288,14 @@
         Hardcoded role protocol mappers allow you to specify a single role to
         always map to an access token for a client. Protocol mappers can be
         defined for a single client, or they can be defined for a client scope
         which can be shared between multiple different clients.
 
         ### Example Usage (Client)
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
             realm="my-realm",
             enabled=True)
@@ -316,19 +311,17 @@
             valid_redirect_uris=["http://localhost:8080/openid-callback"])
         hardcoded_role_mapper = keycloak.openid.HardcodedRoleProtocolMapper("hardcoded_role_mapper",
             realm_id=realm.id,
             client_id=openid_client.id,
             name="hardcoded-role-mapper",
             role_id=role.id)
         ```
-        <!--End PulumiCodeChooser -->
 
         ### Example Usage (Client Scope)
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
             realm="my-realm",
             enabled=True)
@@ -340,15 +333,14 @@
             name="test-client-scope")
         hardcoded_role_mapper = keycloak.openid.HardcodedRoleProtocolMapper("hardcoded_role_mapper",
             realm_id=realm.id,
             client_scope_id=client_scope.id,
             name="hardcoded-role-mapper",
             role_id=role.id)
         ```
-        <!--End PulumiCodeChooser -->
 
         ### Argument Reference
 
         The following arguments are supported:
 
         - `realm_id` - (Required) The realm this protocol mapper exists within.
         - `client_id` - (Required if `client_scope_id` is not specified) The client this protocol mapper is attached to.
```

### Comparing `pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/openid/outputs.py` & `pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/openid/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/openid/script_protocol_mapper.py` & `pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/openid/script_protocol_mapper.py`

 * *Files 5% similar despite different names*

```diff
@@ -403,15 +403,14 @@
 
         > Support for this protocol mapper was removed in Keycloak 18.
 
         ## Example Usage
 
         ### Client)
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
             realm="my-realm",
             enabled=True)
@@ -425,19 +424,17 @@
         script_mapper = keycloak.openid.ScriptProtocolMapper("script_mapper",
             realm_id=realm.id,
             client_id=openid_client.id,
             name="script-mapper",
             claim_name="foo",
             script="exports = 'foo';")
         ```
-        <!--End PulumiCodeChooser -->
 
         ### Client Scope)
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
             realm="my-realm",
             enabled=True)
@@ -447,15 +444,14 @@
         script_mapper = keycloak.openid.ScriptProtocolMapper("script_mapper",
             realm_id=realm.id,
             client_scope_id=client_scope.id,
             name="script-mapper",
             claim_name="foo",
             script="exports = 'foo';")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Protocol mappers can be imported using one of the following formats:
 
         - Client: `{{realm_id}}/client/{{client_keycloak_id}}/{{protocol_mapper_id}}`
 
@@ -503,15 +499,14 @@
 
         > Support for this protocol mapper was removed in Keycloak 18.
 
         ## Example Usage
 
         ### Client)
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
             realm="my-realm",
             enabled=True)
@@ -525,19 +520,17 @@
         script_mapper = keycloak.openid.ScriptProtocolMapper("script_mapper",
             realm_id=realm.id,
             client_id=openid_client.id,
             name="script-mapper",
             claim_name="foo",
             script="exports = 'foo';")
         ```
-        <!--End PulumiCodeChooser -->
 
         ### Client Scope)
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
             realm="my-realm",
             enabled=True)
@@ -547,15 +540,14 @@
         script_mapper = keycloak.openid.ScriptProtocolMapper("script_mapper",
             realm_id=realm.id,
             client_scope_id=client_scope.id,
             name="script-mapper",
             claim_name="foo",
             script="exports = 'foo';")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Protocol mappers can be imported using one of the following formats:
 
         - Client: `{{realm_id}}/client/{{client_keycloak_id}}/{{protocol_mapper_id}}`
```

### Comparing `pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/openid/user_attribute_protocol_mapper.py` & `pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/openid/user_attribute_protocol_mapper.py`

 * *Files 2% similar despite different names*

```diff
@@ -419,15 +419,14 @@
         User attribute protocol mappers allow you to map custom attributes defined
         for a user within Keycloak to a claim in a token. Protocol mappers can be
         defined for a single client, or they can be defined for a client scope which
         can be shared between multiple different clients.
 
         ### Example Usage (Client)
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
             realm="my-realm",
             enabled=True)
@@ -441,19 +440,17 @@
         user_attribute_mapper = keycloak.openid.UserAttributeProtocolMapper("user_attribute_mapper",
             realm_id=realm.id,
             client_id=openid_client.id,
             name="test-mapper",
             user_attribute="foo",
             claim_name="bar")
         ```
-        <!--End PulumiCodeChooser -->
 
         ### Example Usage (Client Scope)
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
             realm="my-realm",
             enabled=True)
@@ -463,15 +460,14 @@
         user_attribute_mapper = keycloak.openid.UserAttributeProtocolMapper("user_attribute_mapper",
             realm_id=realm.id,
             client_scope_id=client_scope.id,
             name="test-mapper",
             user_attribute="foo",
             claim_name="bar")
         ```
-        <!--End PulumiCodeChooser -->
 
         ### Argument Reference
 
         The following arguments are supported:
 
         - `realm_id` - (Required) The realm this protocol mapper exists within.
         - `client_id` - (Required if `client_scope_id` is not specified) The client this protocol mapper is attached to.
@@ -521,15 +517,14 @@
         User attribute protocol mappers allow you to map custom attributes defined
         for a user within Keycloak to a claim in a token. Protocol mappers can be
         defined for a single client, or they can be defined for a client scope which
         can be shared between multiple different clients.
 
         ### Example Usage (Client)
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
             realm="my-realm",
             enabled=True)
@@ -543,19 +538,17 @@
         user_attribute_mapper = keycloak.openid.UserAttributeProtocolMapper("user_attribute_mapper",
             realm_id=realm.id,
             client_id=openid_client.id,
             name="test-mapper",
             user_attribute="foo",
             claim_name="bar")
         ```
-        <!--End PulumiCodeChooser -->
 
         ### Example Usage (Client Scope)
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
             realm="my-realm",
             enabled=True)
@@ -565,15 +558,14 @@
         user_attribute_mapper = keycloak.openid.UserAttributeProtocolMapper("user_attribute_mapper",
             realm_id=realm.id,
             client_scope_id=client_scope.id,
             name="test-mapper",
             user_attribute="foo",
             claim_name="bar")
         ```
-        <!--End PulumiCodeChooser -->
 
         ### Argument Reference
 
         The following arguments are supported:
 
         - `realm_id` - (Required) The realm this protocol mapper exists within.
         - `client_id` - (Required if `client_scope_id` is not specified) The client this protocol mapper is attached to.
```

### Comparing `pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/openid/user_client_role_protocol_mapper.py` & `pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/openid/user_client_role_protocol_mapper.py`

 * *Files 2% similar despite different names*

```diff
@@ -435,15 +435,14 @@
         Protocol mappers can be defined for a single client, or they can be defined for a client scope which can be shared between
         multiple different clients.
 
         ## Example Usage
 
         ### Client)
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
             realm="my-realm",
             enabled=True)
@@ -456,19 +455,17 @@
             valid_redirect_uris=["http://localhost:8080/openid-callback"])
         user_client_role_mapper = keycloak.openid.UserClientRoleProtocolMapper("user_client_role_mapper",
             realm_id=realm.id,
             client_id=openid_client.id,
             name="user-client-role-mapper",
             claim_name="foo")
         ```
-        <!--End PulumiCodeChooser -->
 
         ### Client Scope)
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
             realm="my-realm",
             enabled=True)
@@ -477,15 +474,14 @@
             name="client-scope")
         user_client_role_mapper = keycloak.openid.UserClientRoleProtocolMapper("user_client_role_mapper",
             realm_id=realm.id,
             client_scope_id=client_scope.id,
             name="user-client-role-mapper",
             claim_name="foo")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Protocol mappers can be imported using one of the following formats:
 
         - Client: `{{realm_id}}/client/{{client_keycloak_id}}/{{protocol_mapper_id}}`
 
@@ -532,15 +528,14 @@
         Protocol mappers can be defined for a single client, or they can be defined for a client scope which can be shared between
         multiple different clients.
 
         ## Example Usage
 
         ### Client)
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
             realm="my-realm",
             enabled=True)
@@ -553,19 +548,17 @@
             valid_redirect_uris=["http://localhost:8080/openid-callback"])
         user_client_role_mapper = keycloak.openid.UserClientRoleProtocolMapper("user_client_role_mapper",
             realm_id=realm.id,
             client_id=openid_client.id,
             name="user-client-role-mapper",
             claim_name="foo")
         ```
-        <!--End PulumiCodeChooser -->
 
         ### Client Scope)
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
             realm="my-realm",
             enabled=True)
@@ -574,15 +567,14 @@
             name="client-scope")
         user_client_role_mapper = keycloak.openid.UserClientRoleProtocolMapper("user_client_role_mapper",
             realm_id=realm.id,
             client_scope_id=client_scope.id,
             name="user-client-role-mapper",
             claim_name="foo")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Protocol mappers can be imported using one of the following formats:
 
         - Client: `{{realm_id}}/client/{{client_keycloak_id}}/{{protocol_mapper_id}}`
```

### Comparing `pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/openid/user_property_protocol_mapper.py` & `pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/openid/user_property_protocol_mapper.py`

 * *Files 2% similar despite different names*

```diff
@@ -353,15 +353,14 @@
         User property protocol mappers allow you to map built in properties defined
         on the Keycloak user interface to a claim in a token. Protocol mappers can be
         defined for a single client, or they can be defined for a client scope which
         can be shared between multiple different clients.
 
         ### Example Usage (Client)
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
             realm="my-realm",
             enabled=True)
@@ -375,19 +374,17 @@
         user_property_mapper = keycloak.openid.UserPropertyProtocolMapper("user_property_mapper",
             realm_id=realm.id,
             client_id=openid_client.id,
             name="test-mapper",
             user_property="email",
             claim_name="email")
         ```
-        <!--End PulumiCodeChooser -->
 
         ### Example Usage (Client Scope)
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
             realm="my-realm",
             enabled=True)
@@ -397,15 +394,14 @@
         user_property_mapper = keycloak.openid.UserPropertyProtocolMapper("user_property_mapper",
             realm_id=realm.id,
             client_scope_id=client_scope.id,
             name="test-mapper",
             user_property="email",
             claim_name="email")
         ```
-        <!--End PulumiCodeChooser -->
 
         ### Argument Reference
 
         The following arguments are supported:
 
         - `realm_id` - (Required) The realm this protocol mapper exists within.
         - `client_id` - (Required if `client_scope_id` is not specified) The client this protocol mapper is attached to.
@@ -452,15 +448,14 @@
         User property protocol mappers allow you to map built in properties defined
         on the Keycloak user interface to a claim in a token. Protocol mappers can be
         defined for a single client, or they can be defined for a client scope which
         can be shared between multiple different clients.
 
         ### Example Usage (Client)
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
             realm="my-realm",
             enabled=True)
@@ -474,19 +469,17 @@
         user_property_mapper = keycloak.openid.UserPropertyProtocolMapper("user_property_mapper",
             realm_id=realm.id,
             client_id=openid_client.id,
             name="test-mapper",
             user_property="email",
             claim_name="email")
         ```
-        <!--End PulumiCodeChooser -->
 
         ### Example Usage (Client Scope)
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
             realm="my-realm",
             enabled=True)
@@ -496,15 +489,14 @@
         user_property_mapper = keycloak.openid.UserPropertyProtocolMapper("user_property_mapper",
             realm_id=realm.id,
             client_scope_id=client_scope.id,
             name="test-mapper",
             user_property="email",
             claim_name="email")
         ```
-        <!--End PulumiCodeChooser -->
 
         ### Argument Reference
 
         The following arguments are supported:
 
         - `realm_id` - (Required) The realm this protocol mapper exists within.
         - `client_id` - (Required if `client_scope_id` is not specified) The client this protocol mapper is attached to.
```

### Comparing `pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/openid/user_realm_role_protocol_mapper.py` & `pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/openid/user_realm_role_protocol_mapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -395,15 +395,14 @@
         User realm role protocol mappers allow you to define a claim containing the list of the realm roles.
         Protocol mappers can be defined for a single client, or they can
         be defined for a client scope which can be shared between multiple different
         clients.
 
         ### Example Usage (Client)
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
             realm="my-realm",
             enabled=True)
@@ -416,19 +415,17 @@
             valid_redirect_uris=["http://localhost:8080/openid-callback"])
         user_realm_role_mapper = keycloak.openid.UserRealmRoleProtocolMapper("user_realm_role_mapper",
             realm_id=realm.id,
             client_id=openid_client.id,
             name="user-realm-role-mapper",
             claim_name="foo")
         ```
-        <!--End PulumiCodeChooser -->
 
         ### Example Usage (Client Scope)
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
             realm="my-realm",
             enabled=True)
@@ -437,15 +434,14 @@
             name="test-client-scope")
         user_realm_role_mapper = keycloak.openid.UserRealmRoleProtocolMapper("user_realm_role_mapper",
             realm_id=realm.id,
             client_scope_id=client_scope.id,
             name="user-realm-role-mapper",
             claim_name="foo")
         ```
-        <!--End PulumiCodeChooser -->
 
         ### Argument Reference
 
         The following arguments are supported:
 
         - `realm_id` - (Required) The realm this protocol mapper exists within.
         - `client_id` - (Required if `client_scope_id` is not specified) The client this protocol mapper is attached to.
@@ -495,15 +491,14 @@
         User realm role protocol mappers allow you to define a claim containing the list of the realm roles.
         Protocol mappers can be defined for a single client, or they can
         be defined for a client scope which can be shared between multiple different
         clients.
 
         ### Example Usage (Client)
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
             realm="my-realm",
             enabled=True)
@@ -516,19 +511,17 @@
             valid_redirect_uris=["http://localhost:8080/openid-callback"])
         user_realm_role_mapper = keycloak.openid.UserRealmRoleProtocolMapper("user_realm_role_mapper",
             realm_id=realm.id,
             client_id=openid_client.id,
             name="user-realm-role-mapper",
             claim_name="foo")
         ```
-        <!--End PulumiCodeChooser -->
 
         ### Example Usage (Client Scope)
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
             realm="my-realm",
             enabled=True)
@@ -537,15 +530,14 @@
             name="test-client-scope")
         user_realm_role_mapper = keycloak.openid.UserRealmRoleProtocolMapper("user_realm_role_mapper",
             realm_id=realm.id,
             client_scope_id=client_scope.id,
             name="user-realm-role-mapper",
             claim_name="foo")
         ```
-        <!--End PulumiCodeChooser -->
 
         ### Argument Reference
 
         The following arguments are supported:
 
         - `realm_id` - (Required) The realm this protocol mapper exists within.
         - `client_id` - (Required if `client_scope_id` is not specified) The client this protocol mapper is attached to.
```

### Comparing `pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/openid/user_session_note_protocol_mapper.py` & `pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/openid/user_session_note_protocol_mapper.py`

 * *Files 4% similar despite different names*

```diff
@@ -336,15 +336,14 @@
         Protocol mappers can be defined for a single client, or they can be defined for a client scope which can be shared between
         multiple different clients.
 
         ## Example Usage
 
         ### Client)
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
             realm="my-realm",
             enabled=True)
@@ -359,19 +358,17 @@
             realm_id=realm.id,
             client_id=openid_client.id,
             name="user-session-note-mapper",
             claim_name="foo",
             claim_value_type="String",
             session_note="bar")
         ```
-        <!--End PulumiCodeChooser -->
 
         ### Client Scope)
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
             realm="my-realm",
             enabled=True)
@@ -382,15 +379,14 @@
             realm_id=realm.id,
             client_scope_id=client_scope.id,
             name="user-session-note-mapper",
             claim_name="foo",
             claim_value_type="String",
             session_note="bar")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Protocol mappers can be imported using one of the following formats:
 
         - Client: `{{realm_id}}/client/{{client_keycloak_id}}/{{protocol_mapper_id}}`
 
@@ -434,15 +430,14 @@
         Protocol mappers can be defined for a single client, or they can be defined for a client scope which can be shared between
         multiple different clients.
 
         ## Example Usage
 
         ### Client)
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
             realm="my-realm",
             enabled=True)
@@ -457,19 +452,17 @@
             realm_id=realm.id,
             client_id=openid_client.id,
             name="user-session-note-mapper",
             claim_name="foo",
             claim_value_type="String",
             session_note="bar")
         ```
-        <!--End PulumiCodeChooser -->
 
         ### Client Scope)
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
             realm="my-realm",
             enabled=True)
@@ -480,15 +473,14 @@
             realm_id=realm.id,
             client_scope_id=client_scope.id,
             name="user-session-note-mapper",
             claim_name="foo",
             claim_value_type="String",
             session_note="bar")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Protocol mappers can be imported using one of the following formats:
 
         - Client: `{{realm_id}}/client/{{client_keycloak_id}}/{{protocol_mapper_id}}`
```

### Comparing `pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/outputs.py` & `pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/outputs.py`

 * *Files 5% similar despite different names*

```diff
@@ -787,23 +787,15 @@
                  enabled_when_scopes: Optional[Sequence[str]] = None,
                  group: Optional[str] = None,
                  permissions: Optional['outputs.RealmUserProfileAttributePermissions'] = None,
                  required_for_roles: Optional[Sequence[str]] = None,
                  required_for_scopes: Optional[Sequence[str]] = None,
                  validators: Optional[Sequence['outputs.RealmUserProfileAttributeValidator']] = None):
         """
-        :param str name: The name of the attribute.
-        :param Mapping[str, str] annotations: A map of annotations for the attribute. Values can be a String or a json object.
-        :param str display_name: The display name of the attribute.
-        :param Sequence[str] enabled_when_scopes: A list of scopes. The attribute will only be enabled when these scopes are requested by clients.
         :param str group: A list of groups.
-        :param 'RealmUserProfileAttributePermissionsArgs' permissions: The permissions configuration information.
-        :param Sequence[str] required_for_roles: A list of roles for which the attribute will be required.
-        :param Sequence[str] required_for_scopes: A list of scopes for which the attribute will be required.
-        :param Sequence['RealmUserProfileAttributeValidatorArgs'] validators: A list of validators for the attribute.
         """
         pulumi.set(__self__, "name", name)
         if annotations is not None:
             pulumi.set(__self__, "annotations", annotations)
         if display_name is not None:
             pulumi.set(__self__, "display_name", display_name)
         if enabled_when_scopes is not None:
@@ -818,140 +810,96 @@
             pulumi.set(__self__, "required_for_scopes", required_for_scopes)
         if validators is not None:
             pulumi.set(__self__, "validators", validators)
 
     @property
     @pulumi.getter
     def name(self) -> str:
-        """
-        The name of the attribute.
-        """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter
     def annotations(self) -> Optional[Mapping[str, str]]:
-        """
-        A map of annotations for the attribute. Values can be a String or a json object.
-        """
         return pulumi.get(self, "annotations")
 
     @property
     @pulumi.getter(name="displayName")
     def display_name(self) -> Optional[str]:
-        """
-        The display name of the attribute.
-        """
         return pulumi.get(self, "display_name")
 
     @property
     @pulumi.getter(name="enabledWhenScopes")
     def enabled_when_scopes(self) -> Optional[Sequence[str]]:
-        """
-        A list of scopes. The attribute will only be enabled when these scopes are requested by clients.
-        """
         return pulumi.get(self, "enabled_when_scopes")
 
     @property
     @pulumi.getter
     def group(self) -> Optional[str]:
         """
         A list of groups.
         """
         return pulumi.get(self, "group")
 
     @property
     @pulumi.getter
     def permissions(self) -> Optional['outputs.RealmUserProfileAttributePermissions']:
-        """
-        The permissions configuration information.
-        """
         return pulumi.get(self, "permissions")
 
     @property
     @pulumi.getter(name="requiredForRoles")
     def required_for_roles(self) -> Optional[Sequence[str]]:
-        """
-        A list of roles for which the attribute will be required.
-        """
         return pulumi.get(self, "required_for_roles")
 
     @property
     @pulumi.getter(name="requiredForScopes")
     def required_for_scopes(self) -> Optional[Sequence[str]]:
-        """
-        A list of scopes for which the attribute will be required.
-        """
         return pulumi.get(self, "required_for_scopes")
 
     @property
     @pulumi.getter
     def validators(self) -> Optional[Sequence['outputs.RealmUserProfileAttributeValidator']]:
-        """
-        A list of validators for the attribute.
-        """
         return pulumi.get(self, "validators")
 
 
 @pulumi.output_type
 class RealmUserProfileAttributePermissions(dict):
     def __init__(__self__, *,
                  edits: Sequence[str],
                  views: Sequence[str]):
-        """
-        :param Sequence[str] edits: A list of profiles that will be able to edit the attribute. One of `admin`, `user`.
-        :param Sequence[str] views: A list of profiles that will be able to view the attribute. One of `admin`, `user`.
-        """
         pulumi.set(__self__, "edits", edits)
         pulumi.set(__self__, "views", views)
 
     @property
     @pulumi.getter
     def edits(self) -> Sequence[str]:
-        """
-        A list of profiles that will be able to edit the attribute. One of `admin`, `user`.
-        """
         return pulumi.get(self, "edits")
 
     @property
     @pulumi.getter
     def views(self) -> Sequence[str]:
-        """
-        A list of profiles that will be able to view the attribute. One of `admin`, `user`.
-        """
         return pulumi.get(self, "views")
 
 
 @pulumi.output_type
 class RealmUserProfileAttributeValidator(dict):
     def __init__(__self__, *,
                  name: str,
                  config: Optional[Mapping[str, str]] = None):
-        """
-        :param str name: The name of the attribute.
-        :param Mapping[str, str] config: A map defining the configuration of the validator. Values can be a String or a json object.
-        """
         pulumi.set(__self__, "name", name)
         if config is not None:
             pulumi.set(__self__, "config", config)
 
     @property
     @pulumi.getter
     def name(self) -> str:
-        """
-        The name of the attribute.
-        """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter
     def config(self) -> Optional[Mapping[str, str]]:
-        """
-        A map defining the configuration of the validator. Values can be a String or a json object.
-        """
         return pulumi.get(self, "config")
 
 
 @pulumi.output_type
 class RealmUserProfileGroup(dict):
     @staticmethod
     def __key_warning(key: str):
@@ -973,58 +921,40 @@
         return super().get(key, default)
 
     def __init__(__self__, *,
                  name: str,
                  annotations: Optional[Mapping[str, str]] = None,
                  display_description: Optional[str] = None,
                  display_header: Optional[str] = None):
-        """
-        :param str name: The name of the attribute.
-        :param Mapping[str, str] annotations: A map of annotations for the attribute. Values can be a String or a json object.
-        :param str display_description: The display description of the group.
-        :param str display_header: The display header of the group.
-        """
         pulumi.set(__self__, "name", name)
         if annotations is not None:
             pulumi.set(__self__, "annotations", annotations)
         if display_description is not None:
             pulumi.set(__self__, "display_description", display_description)
         if display_header is not None:
             pulumi.set(__self__, "display_header", display_header)
 
     @property
     @pulumi.getter
     def name(self) -> str:
-        """
-        The name of the attribute.
-        """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter
     def annotations(self) -> Optional[Mapping[str, str]]:
-        """
-        A map of annotations for the attribute. Values can be a String or a json object.
-        """
         return pulumi.get(self, "annotations")
 
     @property
     @pulumi.getter(name="displayDescription")
     def display_description(self) -> Optional[str]:
-        """
-        The display description of the group.
-        """
         return pulumi.get(self, "display_description")
 
     @property
     @pulumi.getter(name="displayHeader")
     def display_header(self) -> Optional[str]:
-        """
-        The display header of the group.
-        """
         return pulumi.get(self, "display_header")
 
 
 @pulumi.output_type
 class RealmWebAuthnPasswordlessPolicy(dict):
     @staticmethod
     def __key_warning(key: str):
```

### Comparing `pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/provider.py` & `pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/realm.py` & `pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/realm.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/realm_events.py` & `pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/realm_events.py`

 * *Files 2% similar despite different names*

```diff
@@ -210,15 +210,14 @@
         """
         ## # RealmEvents
 
         Allows for managing Realm Events settings within Keycloak.
 
         ### Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm", realm="test")
         realm_events = keycloak.RealmEvents("realm_events",
             realm_id=realm.id,
@@ -228,15 +227,14 @@
             admin_events_details_enabled=True,
             enabled_event_types=[
                 "LOGIN",
                 "LOGOUT",
             ],
             events_listeners=["jboss-logging"])
         ```
-        <!--End PulumiCodeChooser -->
 
         ### Argument Reference
 
         The following arguments are supported:
 
         - `realm_id` - (Required) The name of the realm the event settings apply to.
         - `admin_events_enabled` - (Optional) When true, admin events are saved to the database, making them available through the admin console. Defaults to `false`.
@@ -258,15 +256,14 @@
         """
         ## # RealmEvents
 
         Allows for managing Realm Events settings within Keycloak.
 
         ### Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm", realm="test")
         realm_events = keycloak.RealmEvents("realm_events",
             realm_id=realm.id,
@@ -276,15 +273,14 @@
             admin_events_details_enabled=True,
             enabled_event_types=[
                 "LOGIN",
                 "LOGOUT",
             ],
             events_listeners=["jboss-logging"])
         ```
-        <!--End PulumiCodeChooser -->
 
         ### Argument Reference
 
         The following arguments are supported:
 
         - `realm_id` - (Required) The name of the realm the event settings apply to.
         - `admin_events_enabled` - (Optional) When true, admin events are saved to the database, making them available through the admin console. Defaults to `false`.
```

### Comparing `pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/realm_keystore_aes_generated.py` & `pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/realm_keystore_aes_generated.py`

 * *Files 4% similar despite different names*

```diff
@@ -233,29 +233,27 @@
         """
         Allows for creating and managing `aes-generated` Realm keystores within Keycloak.
 
         A realm keystore manages generated key pairs that are used by Keycloak to perform cryptographic signatures and encryption.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm", realm="my-realm")
         keystore_aes_generated = keycloak.RealmKeystoreAesGenerated("keystore_aes_generated",
             name="my-aes-generated-key",
             realm_id=realm.id,
             enabled=True,
             active=True,
             priority=100,
             secret_size=16)
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Realm keys can be imported using realm name and keystore id, you can find it in web UI.
 
         Example:
 
@@ -283,29 +281,27 @@
         """
         Allows for creating and managing `aes-generated` Realm keystores within Keycloak.
 
         A realm keystore manages generated key pairs that are used by Keycloak to perform cryptographic signatures and encryption.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm", realm="my-realm")
         keystore_aes_generated = keycloak.RealmKeystoreAesGenerated("keystore_aes_generated",
             name="my-aes-generated-key",
             realm_id=realm.id,
             enabled=True,
             active=True,
             priority=100,
             secret_size=16)
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Realm keys can be imported using realm name and keystore id, you can find it in web UI.
 
         Example:
```

### Comparing `pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/realm_keystore_ecdsa_generated.py` & `pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/realm_keystore_ecdsa_generated.py`

 * *Files 2% similar despite different names*

```diff
@@ -233,29 +233,27 @@
         """
         Allows for creating and managing `acdsa_generated` Realm keystores within Keycloak.
 
         A realm keystore manages generated key pairs that are used by Keycloak to perform cryptographic signatures and encryption.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm", realm="my-realm")
         keystore_ecdsa_generated = keycloak.RealmKeystoreEcdsaGenerated("keystore_ecdsa_generated",
             name="my-ecdsa-generated-key",
             realm_id=realm.id,
             enabled=True,
             active=True,
             priority=100,
             elliptic_curve_key="P-256")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Realm keys can be imported using realm name and keystore id, you can find it in web UI.
 
         Example:
 
@@ -283,29 +281,27 @@
         """
         Allows for creating and managing `acdsa_generated` Realm keystores within Keycloak.
 
         A realm keystore manages generated key pairs that are used by Keycloak to perform cryptographic signatures and encryption.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm", realm="my-realm")
         keystore_ecdsa_generated = keycloak.RealmKeystoreEcdsaGenerated("keystore_ecdsa_generated",
             name="my-ecdsa-generated-key",
             realm_id=realm.id,
             enabled=True,
             active=True,
             priority=100,
             elliptic_curve_key="P-256")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Realm keys can be imported using realm name and keystore id, you can find it in web UI.
 
         Example:
```

### Comparing `pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/realm_keystore_hmac_generated.py` & `pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/realm_keystore_hmac_generated.py`

 * *Files 2% similar despite different names*

```diff
@@ -266,30 +266,28 @@
         """
         Allows for creating and managing `hmac-generated` Realm keystores within Keycloak.
 
         A realm keystore manages generated key pairs that are used by Keycloak to perform cryptographic signatures and encryption.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm", realm="my-realm")
         keystore_hmac_generated = keycloak.RealmKeystoreHmacGenerated("keystore_hmac_generated",
             name="my-hmac-generated-key",
             realm_id=realm.id,
             enabled=True,
             active=True,
             priority=100,
             algorithm="HS256",
             secret_size=64)
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Realm keys can be imported using realm name and keystore id, you can find it in web UI.
 
         Example:
 
@@ -318,30 +316,28 @@
         """
         Allows for creating and managing `hmac-generated` Realm keystores within Keycloak.
 
         A realm keystore manages generated key pairs that are used by Keycloak to perform cryptographic signatures and encryption.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm", realm="my-realm")
         keystore_hmac_generated = keycloak.RealmKeystoreHmacGenerated("keystore_hmac_generated",
             name="my-hmac-generated-key",
             realm_id=realm.id,
             enabled=True,
             active=True,
             priority=100,
             algorithm="HS256",
             secret_size=64)
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Realm keys can be imported using realm name and keystore id, you can find it in web UI.
 
         Example:
```

### Comparing `pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/realm_keystore_java_generated.py` & `pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/realm_keystore_java_generated.py`

 * *Files 0% similar despite different names*

```diff
@@ -361,15 +361,14 @@
         """
         Allows for creating and managing `java-keystore` Realm keystores within Keycloak.
 
         A realm keystore manages generated key pairs that are used by Keycloak to perform cryptographic signatures and encryption.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm", realm="my-realm")
         java_keystore = keycloak.RealmKeystoreJavaGenerated("java_keystore",
             name="my-java-keystore",
@@ -379,15 +378,14 @@
             keystore="<path to your keystore>",
             keystore_password="<password for keystore>",
             key_alias="<alias for the private key>",
             key_password="<password for the private key>",
             priority=100,
             algorithm="RS256")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Realm keys can be imported using realm name and keystore id, you can find it in web UI.
 
         Example:
 
@@ -419,15 +417,14 @@
         """
         Allows for creating and managing `java-keystore` Realm keystores within Keycloak.
 
         A realm keystore manages generated key pairs that are used by Keycloak to perform cryptographic signatures and encryption.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm", realm="my-realm")
         java_keystore = keycloak.RealmKeystoreJavaGenerated("java_keystore",
             name="my-java-keystore",
@@ -437,15 +434,14 @@
             keystore="<path to your keystore>",
             keystore_password="<password for keystore>",
             key_alias="<alias for the private key>",
             key_password="<password for the private key>",
             priority=100,
             algorithm="RS256")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Realm keys can be imported using realm name and keystore id, you can find it in web UI.
 
         Example:
```

### Comparing `pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/realm_keystore_rsa.py` & `pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/realm_keystore_rsa.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/realm_keystore_rsa_generated.py` & `pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/realm_keystore_rsa_generated.py`

 * *Files 2% similar despite different names*

```diff
@@ -266,30 +266,28 @@
         """
         Allows for creating and managing `rsa-generated` Realm keystores within Keycloak.
 
         A realm keystore manages generated key pairs that are used by Keycloak to perform cryptographic signatures and encryption.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm", realm="my-realm")
         keystore_rsa_generated = keycloak.RealmKeystoreRsaGenerated("keystore_rsa_generated",
             name="my-rsa-generated-key",
             realm_id=realm.id,
             enabled=True,
             active=True,
             priority=100,
             algorithm="RS256",
             key_size=2048)
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Realm keys can be imported using realm name and keystore id, you can find it in web UI.
 
         Example:
 
@@ -318,30 +316,28 @@
         """
         Allows for creating and managing `rsa-generated` Realm keystores within Keycloak.
 
         A realm keystore manages generated key pairs that are used by Keycloak to perform cryptographic signatures and encryption.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm", realm="my-realm")
         keystore_rsa_generated = keycloak.RealmKeystoreRsaGenerated("keystore_rsa_generated",
             name="my-rsa-generated-key",
             realm_id=realm.id,
             enabled=True,
             active=True,
             priority=100,
             algorithm="RS256",
             key_size=2048)
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Realm keys can be imported using realm name and keystore id, you can find it in web UI.
 
         Example:
```

### Comparing `pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/realm_user_profile.py` & `pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/realm_user_profile.py`

 * *Files 2% similar despite different names*

```diff
@@ -143,15 +143,14 @@
         - Quarkus distribution: `--features=preview` or `--features=declarative-user-profile`
 
         The realm linked to the `RealmUserProfile` resource must have the user profile feature enabled.
         It can be done via the administration UI, or by setting the `userProfileEnabled` realm attribute to `true`.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import json
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
             realm="my-realm",
@@ -222,15 +221,14 @@
                     },
                 ),
                 keycloak.RealmUserProfileGroupArgs(
                     name="group2",
                 ),
             ])
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         This resource currently does not support importing.
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
@@ -254,15 +252,14 @@
         - Quarkus distribution: `--features=preview` or `--features=declarative-user-profile`
 
         The realm linked to the `RealmUserProfile` resource must have the user profile feature enabled.
         It can be done via the administration UI, or by setting the `userProfileEnabled` realm attribute to `true`.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import json
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
             realm="my-realm",
@@ -333,15 +330,14 @@
                     },
                 ),
                 keycloak.RealmUserProfileGroupArgs(
                     name="group2",
                 ),
             ])
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         This resource currently does not support importing.
 
         :param str resource_name: The name of the resource.
         :param RealmUserProfileArgs args: The arguments to use to populate this resource's properties.
```

### Comparing `pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/required_action.py` & `pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/required_action.py`

 * *Files 1% similar despite different names*

```diff
@@ -232,29 +232,27 @@
         """
         Allows for creating and managing required actions within Keycloak.
 
         [Required actions](https://www.keycloak.org/docs/latest/server_admin/#con-required-actions_server_administration_guide) specify actions required before the first login of all new users.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
             realm="my-realm",
             enabled=True)
         required_action = keycloak.RequiredAction("required_action",
             realm_id=realm.realm,
             alias="webauthn-register",
             enabled=True,
             name="Webauthn Register")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Authentication executions can be imported using the formats: `{{realm}}/{{alias}}`.
 
         Example:
 
@@ -282,29 +280,27 @@
         """
         Allows for creating and managing required actions within Keycloak.
 
         [Required actions](https://www.keycloak.org/docs/latest/server_admin/#con-required-actions_server_administration_guide) specify actions required before the first login of all new users.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
             realm="my-realm",
             enabled=True)
         required_action = keycloak.RequiredAction("required_action",
             realm_id=realm.realm,
             alias="webauthn-register",
             enabled=True,
             name="Webauthn Register")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Authentication executions can be imported using the formats: `{{realm}}/{{alias}}`.
 
         Example:
```

### Comparing `pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/role.py` & `pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/role.py`

 * *Files 4% similar despite different names*

```diff
@@ -188,32 +188,29 @@
         Allows for creating and managing roles within Keycloak.
 
         Roles allow you define privileges within Keycloak and map them to users
         and groups.
 
         ### Example Usage (Realm role)
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
             realm="my-realm",
             enabled=True)
         realm_role = keycloak.Role("realm_role",
             realm_id=realm.id,
             name="my-realm-role",
             description="My Realm Role")
         ```
-        <!--End PulumiCodeChooser -->
 
         ### Example Usage (Client role)
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
             realm="my-realm",
             enabled=True)
@@ -225,19 +222,17 @@
             access_type="BEARER-ONLY")
         client_role = keycloak.Role("client_role",
             realm_id=realm.id,
             client_id=client_keycloak_client["id"],
             name="my-client-role",
             description="My Client Role")
         ```
-        <!--End PulumiCodeChooser -->
 
         ### Example Usage (Composite role)
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
             realm="my-realm",
             enabled=True)
@@ -273,15 +268,14 @@
                 "{keycloak_role.create_role.id}",
                 "{keycloak_role.read_role.id}",
                 "{keycloak_role.update_role.id}",
                 "{keycloak_role.delete_role.id}",
                 "{keycloak_role.client_role.id}",
             ])
         ```
-        <!--End PulumiCodeChooser -->
 
         ### Argument Reference
 
         The following arguments are supported:
 
         - `realm_id` - (Required) The realm this role exists within.
         - `client_id` - (Optional) When specified, this role will be created as
@@ -316,32 +310,29 @@
         Allows for creating and managing roles within Keycloak.
 
         Roles allow you define privileges within Keycloak and map them to users
         and groups.
 
         ### Example Usage (Realm role)
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
             realm="my-realm",
             enabled=True)
         realm_role = keycloak.Role("realm_role",
             realm_id=realm.id,
             name="my-realm-role",
             description="My Realm Role")
         ```
-        <!--End PulumiCodeChooser -->
 
         ### Example Usage (Client role)
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
             realm="my-realm",
             enabled=True)
@@ -353,19 +344,17 @@
             access_type="BEARER-ONLY")
         client_role = keycloak.Role("client_role",
             realm_id=realm.id,
             client_id=client_keycloak_client["id"],
             name="my-client-role",
             description="My Client Role")
         ```
-        <!--End PulumiCodeChooser -->
 
         ### Example Usage (Composite role)
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
             realm="my-realm",
             enabled=True)
@@ -401,15 +390,14 @@
                 "{keycloak_role.create_role.id}",
                 "{keycloak_role.read_role.id}",
                 "{keycloak_role.update_role.id}",
                 "{keycloak_role.delete_role.id}",
                 "{keycloak_role.client_role.id}",
             ])
         ```
-        <!--End PulumiCodeChooser -->
 
         ### Argument Reference
 
         The following arguments are supported:
 
         - `realm_id` - (Required) The realm this role exists within.
         - `client_id` - (Optional) When specified, this role will be created as
```

### Comparing `pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/saml/__init__.py` & `pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/saml/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/saml/_inputs.py` & `pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/saml/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/saml/client.py` & `pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/saml/client.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/saml/client_default_scope.py` & `pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/saml/client_default_scope.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/saml/client_scope.py` & `pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/saml/client_scope.py`

 * *Files 2% similar despite different names*

```diff
@@ -200,29 +200,27 @@
         """
         Allows for creating and managing Keycloak client scopes that can be attached to clients that use the SAML protocol.
 
         Client Scopes can be used to share common protocol and role mappings between multiple clients within a realm.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
             realm="my-realm",
             enabled=True)
         saml_client_scope = keycloak.saml.ClientScope("saml_client_scope",
             realm_id=realm.id,
             name="groups",
             description="This scope will map a user's group memberships to SAML assertion",
             gui_order=1)
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Client scopes can be imported using the format `{{realm_id}}/{{client_scope_id}}`, where `client_scope_id` is the unique ID that Keycloak
 
         assigns to the client scope upon creation. This value can be found in the URI when editing this client scope in the GUI, and is typically a GUID.
 
@@ -251,29 +249,27 @@
         """
         Allows for creating and managing Keycloak client scopes that can be attached to clients that use the SAML protocol.
 
         Client Scopes can be used to share common protocol and role mappings between multiple clients within a realm.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
             realm="my-realm",
             enabled=True)
         saml_client_scope = keycloak.saml.ClientScope("saml_client_scope",
             realm_id=realm.id,
             name="groups",
             description="This scope will map a user's group memberships to SAML assertion",
             gui_order=1)
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Client scopes can be imported using the format `{{realm_id}}/{{client_scope_id}}`, where `client_scope_id` is the unique ID that Keycloak
 
         assigns to the client scope upon creation. This value can be found in the URI when editing this client scope in the GUI, and is typically a GUID.
```

### Comparing `pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/saml/get_client.py` & `pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/saml/get_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -391,27 +391,25 @@
                realm_id: Optional[str] = None,
                opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetClientResult:
     """
     This data source can be used to fetch properties of a Keycloak client that uses the SAML protocol.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_keycloak as keycloak
 
     realm_management = keycloak.saml.get_client(realm_id="my-realm",
         client_id="realm-management")
     # use the data source
     admin = keycloak.get_role(realm_id="my-realm",
         client_id=realm_management.id,
         name="realm-admin")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str client_id: The client id (not its unique ID).
     :param str realm_id: The realm id.
     """
     __args__ = dict()
     __args__['clientId'] = client_id
@@ -466,26 +464,24 @@
                       realm_id: Optional[pulumi.Input[str]] = None,
                       opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetClientResult]:
     """
     This data source can be used to fetch properties of a Keycloak client that uses the SAML protocol.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_keycloak as keycloak
 
     realm_management = keycloak.saml.get_client(realm_id="my-realm",
         client_id="realm-management")
     # use the data source
     admin = keycloak.get_role(realm_id="my-realm",
         client_id=realm_management.id,
         name="realm-admin")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str client_id: The client id (not its unique ID).
     :param str realm_id: The realm id.
     """
     ...
```

### Comparing `pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/saml/get_client_installation_provider.py` & `pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/saml/get_client_installation_provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/saml/identity_provider.py` & `pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/saml/identity_provider.py`

 * *Files 0% similar despite different names*

```diff
@@ -1283,15 +1283,14 @@
 
         Allows to create and manage SAML Identity Providers within Keycloak.
 
         SAML (Security Assertion Markup Language) identity providers allows to authenticate through a third-party system, using SAML standard.
 
         ### Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm_identity_provider = keycloak.saml.IdentityProvider("realm_identity_provider",
             realm="my-realm",
             alias="my-idp",
@@ -1301,15 +1300,14 @@
             post_binding_response=True,
             post_binding_logout=True,
             post_binding_authn_request=True,
             store_token=False,
             trust_email=True,
             force_authn=True)
         ```
-        <!--End PulumiCodeChooser -->
 
         ### Argument Reference
 
         The following arguments are supported:
 
         - `realm` - (Required) The name of the realm. This is unique across Keycloak.
         - `alias` - (Optional) The uniq name of identity provider.
@@ -1402,15 +1400,14 @@
 
         Allows to create and manage SAML Identity Providers within Keycloak.
 
         SAML (Security Assertion Markup Language) identity providers allows to authenticate through a third-party system, using SAML standard.
 
         ### Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm_identity_provider = keycloak.saml.IdentityProvider("realm_identity_provider",
             realm="my-realm",
             alias="my-idp",
@@ -1420,15 +1417,14 @@
             post_binding_response=True,
             post_binding_logout=True,
             post_binding_authn_request=True,
             store_token=False,
             trust_email=True,
             force_authn=True)
         ```
-        <!--End PulumiCodeChooser -->
 
         ### Argument Reference
 
         The following arguments are supported:
 
         - `realm` - (Required) The name of the realm. This is unique across Keycloak.
         - `alias` - (Optional) The uniq name of identity provider.
```

### Comparing `pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/saml/outputs.py` & `pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/saml/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/saml/script_protocol_mapper.py` & `pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/saml/script_protocol_mapper.py`

 * *Files 0% similar despite different names*

```diff
@@ -332,15 +332,14 @@
         Script protocol mappers evaluate a JavaScript function to produce an attribute value based on context information.
 
         Protocol mappers can be defined for a single client, or they can be defined for a client scope which can be shared between
         multiple different clients.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
             realm="my-realm",
             enabled=True)
@@ -352,15 +351,14 @@
             realm_id=realm.id,
             client_id=saml_client.id,
             name="script-mapper",
             script="exports = 'foo';",
             saml_attribute_name="displayName",
             saml_attribute_name_format="Unspecified")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Protocol mappers can be imported using one of the following formats:
 
         - Client: `{{realm_id}}/client/{{client_keycloak_id}}/{{protocol_mapper_id}}`
 
@@ -402,15 +400,14 @@
         Script protocol mappers evaluate a JavaScript function to produce an attribute value based on context information.
 
         Protocol mappers can be defined for a single client, or they can be defined for a client scope which can be shared between
         multiple different clients.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
             realm="my-realm",
             enabled=True)
@@ -422,15 +419,14 @@
             realm_id=realm.id,
             client_id=saml_client.id,
             name="script-mapper",
             script="exports = 'foo';",
             saml_attribute_name="displayName",
             saml_attribute_name_format="Unspecified")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Protocol mappers can be imported using one of the following formats:
 
         - Client: `{{realm_id}}/client/{{client_keycloak_id}}/{{protocol_mapper_id}}`
```

### Comparing `pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/saml/user_attribute_protocol_mapper.py` & `pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/saml/user_attribute_protocol_mapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -238,15 +238,14 @@
         SAML user attribute protocol mappers allow you to map custom attributes defined
         for a user within Keycloak to an attribute in a SAML assertion. Protocol mappers
         can be defined for a single client, or they can be defined for a client scope which
         can be shared between multiple different clients.
 
         ### Example Usage (Client)
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
             realm="my-realm",
             enabled=True)
@@ -258,15 +257,14 @@
             realm_id=test["id"],
             client_id=saml_client.id,
             name="displayname-user-attribute-mapper",
             user_attribute="displayName",
             saml_attribute_name="displayName",
             saml_attribute_name_format="Unspecified")
         ```
-        <!--End PulumiCodeChooser -->
 
         ### Argument Reference
 
         The following arguments are supported:
 
         - `realm_id` - (Required) The realm this protocol mapper exists within.
         - `client_id` - (Required if `client_scope_id` is not specified) The SAML client this protocol mapper is attached to.
@@ -303,15 +301,14 @@
         SAML user attribute protocol mappers allow you to map custom attributes defined
         for a user within Keycloak to an attribute in a SAML assertion. Protocol mappers
         can be defined for a single client, or they can be defined for a client scope which
         can be shared between multiple different clients.
 
         ### Example Usage (Client)
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
             realm="my-realm",
             enabled=True)
@@ -323,15 +320,14 @@
             realm_id=test["id"],
             client_id=saml_client.id,
             name="displayname-user-attribute-mapper",
             user_attribute="displayName",
             saml_attribute_name="displayName",
             saml_attribute_name_format="Unspecified")
         ```
-        <!--End PulumiCodeChooser -->
 
         ### Argument Reference
 
         The following arguments are supported:
 
         - `realm_id` - (Required) The realm this protocol mapper exists within.
         - `client_id` - (Required if `client_scope_id` is not specified) The SAML client this protocol mapper is attached to.
```

### Comparing `pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/saml/user_property_protocol_mapper.py` & `pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/saml/user_property_protocol_mapper.py`

 * *Files 2% similar despite different names*

```diff
@@ -238,15 +238,14 @@
         SAML user property protocol mappers allow you to map properties of the Keycloak
         user model to an attribute in a SAML assertion. Protocol mappers
         can be defined for a single client, or they can be defined for a client scope which
         can be shared between multiple different clients.
 
         ### Example Usage (Client)
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
             realm="my-realm",
             enabled=True)
@@ -258,15 +257,14 @@
             realm_id=test["id"],
             client_id=saml_client.id,
             name="email-user-property-mapper",
             user_property="email",
             saml_attribute_name="email",
             saml_attribute_name_format="Unspecified")
         ```
-        <!--End PulumiCodeChooser -->
 
         ### Argument Reference
 
         The following arguments are supported:
 
         - `realm_id` - (Required) The realm this protocol mapper exists within.
         - `client_id` - (Required if `client_scope_id` is not specified) The SAML client this protocol mapper is attached to.
@@ -303,15 +301,14 @@
         SAML user property protocol mappers allow you to map properties of the Keycloak
         user model to an attribute in a SAML assertion. Protocol mappers
         can be defined for a single client, or they can be defined for a client scope which
         can be shared between multiple different clients.
 
         ### Example Usage (Client)
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
             realm="my-realm",
             enabled=True)
@@ -323,15 +320,14 @@
             realm_id=test["id"],
             client_id=saml_client.id,
             name="email-user-property-mapper",
             user_property="email",
             saml_attribute_name="email",
             saml_attribute_name_format="Unspecified")
         ```
-        <!--End PulumiCodeChooser -->
 
         ### Argument Reference
 
         The following arguments are supported:
 
         - `realm_id` - (Required) The realm this protocol mapper exists within.
         - `client_id` - (Required if `client_scope_id` is not specified) The SAML client this protocol mapper is attached to.
```

### Comparing `pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/user.py` & `pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/user.py`

 * *Files 1% similar despite different names*

```diff
@@ -315,15 +315,14 @@
 
         This resource was created primarily to enable the acceptance tests for the `Group` resource.
         Creating users within Keycloak is not recommended. Instead, users should be federated from external sources
         by configuring user federation providers or identity providers.
 
         ### Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
             realm="my-realm",
             enabled=True)
@@ -342,15 +341,14 @@
             first_name="Alice",
             last_name="Aliceberg",
             initial_password=keycloak.UserInitialPasswordArgs(
                 value="some password",
                 temporary=True,
             ))
         ```
-        <!--End PulumiCodeChooser -->
 
         ### Argument Reference
 
         The following arguments are supported:
 
         - `realm_id` - (Required) The realm this user belongs to.
         - `username` - (Required) The unique username of this user.
@@ -386,15 +384,14 @@
 
         This resource was created primarily to enable the acceptance tests for the `Group` resource.
         Creating users within Keycloak is not recommended. Instead, users should be federated from external sources
         by configuring user federation providers or identity providers.
 
         ### Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
             realm="my-realm",
             enabled=True)
@@ -413,15 +410,14 @@
             first_name="Alice",
             last_name="Aliceberg",
             initial_password=keycloak.UserInitialPasswordArgs(
                 value="some password",
                 temporary=True,
             ))
         ```
-        <!--End PulumiCodeChooser -->
 
         ### Argument Reference
 
         The following arguments are supported:
 
         - `realm_id` - (Required) The realm this user belongs to.
         - `username` - (Required) The unique username of this user.
```

### Comparing `pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/user_groups.py` & `pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/user_groups.py`

 * *Files 1% similar despite different names*

```diff
@@ -167,15 +167,14 @@
 
         If `exhaustive` is true, this resource attempts to be an **authoritative** source over user groups: groups that are manually added to the user will be removed, and groups that are manually removed from the user group will be added upon the next run of `pulumi up`.
         If `exhaustive` is false, this resource is a partial assignation of groups to a user. As a result, you can get multiple `UserGroups` for the same `user_id`.
 
         ## Example Usage
 
         ### Exhaustive Groups)
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
             realm="my-realm",
             enabled=True)
@@ -186,15 +185,14 @@
             realm_id=realm.id,
             username="my-user")
         user_groups = keycloak.UserGroups("user_groups",
             realm_id=realm.id,
             user_id=user.id,
             group_ids=[group.id])
         ```
-        <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[bool] exhaustive: Indicates if the list of the user's groups is exhaustive. In this case, groups that are manually added to the user will be removed. Defaults to `true`.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] group_ids: A list of group IDs that the user is member of.
         :param pulumi.Input[str] realm_id: The realm this group exists in.
         :param pulumi.Input[str] user_id: The ID of the user this resource should manage groups for.
@@ -210,15 +208,14 @@
 
         If `exhaustive` is true, this resource attempts to be an **authoritative** source over user groups: groups that are manually added to the user will be removed, and groups that are manually removed from the user group will be added upon the next run of `pulumi up`.
         If `exhaustive` is false, this resource is a partial assignation of groups to a user. As a result, you can get multiple `UserGroups` for the same `user_id`.
 
         ## Example Usage
 
         ### Exhaustive Groups)
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
             realm="my-realm",
             enabled=True)
@@ -229,15 +226,14 @@
             realm_id=realm.id,
             username="my-user")
         user_groups = keycloak.UserGroups("user_groups",
             realm_id=realm.id,
             user_id=user.id,
             group_ids=[group.id])
         ```
-        <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param UserGroupsArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
```

### Comparing `pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/user_roles.py` & `pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/user_roles.py`

 * *Files 1% similar despite different names*

```diff
@@ -172,15 +172,14 @@
         Note that when assigning composite roles to a user, you may see a non-empty plan following a `pulumi up` if you assign
         a role and a composite that includes that role to the same user.
 
         ## Example Usage
 
         ### Exhaustive Roles)
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
             realm="my-realm",
             enabled=True)
@@ -210,15 +209,14 @@
             realm_id=realm.id,
             user_id=user.id,
             role_ids=[
                 realm_role.id,
                 client_role.id,
             ])
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         This resource can be imported using the format `{{realm_id}}/{{user_id}}`, where `user_id` is the unique ID that Keycloak
 
         assigns to the user upon creation. This value can be found in the GUI when editing the user, and is typically a GUID.
 
@@ -253,15 +251,14 @@
         Note that when assigning composite roles to a user, you may see a non-empty plan following a `pulumi up` if you assign
         a role and a composite that includes that role to the same user.
 
         ## Example Usage
 
         ### Exhaustive Roles)
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
             realm="my-realm",
             enabled=True)
@@ -291,15 +288,14 @@
             realm_id=realm.id,
             user_id=user.id,
             role_ids=[
                 realm_role.id,
                 client_role.id,
             ])
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         This resource can be imported using the format `{{realm_id}}/{{user_id}}`, where `user_id` is the unique ID that Keycloak
 
         assigns to the user upon creation. This value can be found in the GUI when editing the user, and is typically a GUID.
```

### Comparing `pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/user_template_importer_identity_provider_mapper.py` & `pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/user_template_importer_identity_provider_mapper.py`

 * *Files 0% similar despite different names*

```diff
@@ -203,15 +203,14 @@
 
         - Substitutions are enclosed in \\${}. For example: '\\${ALIAS}.\\${CLAIM.sub}'. ALIAS is the provider alias. CLAIM.\\<NAME\\> references an ID or Access token claim.
 
         > If you are using Keycloak 10 or higher, you will need to specify the `extra_config` argument in order to define a `syncMode` for the mapper.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
             realm="my-realm",
             enabled=True)
@@ -228,15 +227,14 @@
             name="username-template-importer",
             identity_provider_alias=oidc.alias,
             template="${ALIAS}.${CLAIM.email}",
             extra_config={
                 "syncMode": "INHERIT",
             })
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Identity provider mappers can be imported using the format `{{realm_id}}/{{idp_alias}}/{{idp_mapper_id}}`, where `idp_alias` is the identity provider alias, and `idp_mapper_id` is the unique ID that Keycloak
 
         assigns to the mapper upon creation. This value can be found in the URI when editing this mapper in the GUI, and is typically a GUID.
 
@@ -269,15 +267,14 @@
 
         - Substitutions are enclosed in \\${}. For example: '\\${ALIAS}.\\${CLAIM.sub}'. ALIAS is the provider alias. CLAIM.\\<NAME\\> references an ID or Access token claim.
 
         > If you are using Keycloak 10 or higher, you will need to specify the `extra_config` argument in order to define a `syncMode` for the mapper.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
             realm="my-realm",
             enabled=True)
@@ -294,15 +291,14 @@
             name="username-template-importer",
             identity_provider_alias=oidc.alias,
             template="${ALIAS}.${CLAIM.email}",
             extra_config={
                 "syncMode": "INHERIT",
             })
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Identity provider mappers can be imported using the format `{{realm_id}}/{{idp_alias}}/{{idp_mapper_id}}`, where `idp_alias` is the identity provider alias, and `idp_mapper_id` is the unique ID that Keycloak
 
         assigns to the mapper upon creation. This value can be found in the URI when editing this mapper in the GUI, and is typically a GUID.
```

### Comparing `pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak/users_permissions.py` & `pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak/users_permissions.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak.egg-info/PKG-INFO` & `pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_keycloak
-Version: 5.4.0a1713461881
+Version: 5.4.0a1713899008
 Summary: A Pulumi package for creating and managing keycloak cloud resources.
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.io
 Project-URL: Repository, https://github.com/pulumi/pulumi-keycloak
 Keywords: pulumi,keycloak
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_keycloak-5.4.0a1713461881/pulumi_keycloak.egg-info/SOURCES.txt` & `pulumi_keycloak-5.4.0a1713899008/pulumi_keycloak.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.4.0a1713461881/pyproject.toml` & `pulumi_keycloak-5.4.0a1713899008/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [project]
   name = "pulumi_keycloak"
   description = "A Pulumi package for creating and managing keycloak cloud resources."
   dependencies = ["parver>=0.2.1", "pulumi>=3.0.0,<4.0.0", "semver>=2.8.1"]
   keywords = ["pulumi", "keycloak"]
   readme = "README.md"
   requires-python = ">=3.8"
-  version = "5.4.0a1713461881"
+  version = "5.4.0a1713899008"
   [project.license]
     text = "Apache-2.0"
   [project.urls]
     Homepage = "https://pulumi.io"
     Repository = "https://github.com/pulumi/pulumi-keycloak"
 
 [build-system]
```

