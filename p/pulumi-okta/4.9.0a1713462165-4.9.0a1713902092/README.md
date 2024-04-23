# Comparing `tmp/pulumi_okta-4.9.0a1713462165.tar.gz` & `tmp/pulumi_okta-4.9.0a1713902092.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_okta-4.9.0a1713462165.tar", last modified: Thu Apr 18 17:45:45 2024, max compression
+gzip compressed data, was "pulumi_okta-4.9.0a1713902092.tar", last modified: Tue Apr 23 20:09:12 2024, max compression
```

## Comparing `pulumi_okta-4.9.0a1713462165.tar` & `pulumi_okta-4.9.0a1713902092.tar`

### file list

```diff
@@ -1,206 +1,206 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 17:45:45.565199 pulumi_okta-4.9.0a1713462165/
--rw-r--r--   0 runner    (1001) docker     (127)     3351 2024-04-18 17:45:45.565199 pulumi_okta-4.9.0a1713462165/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2913 2024-04-18 17:45:39.000000 pulumi_okta-4.9.0a1713462165/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 17:45:45.541199 pulumi_okta-4.9.0a1713462165/pulumi_okta/
--rw-r--r--   0 runner    (1001) docker     (127)    21302 2024-04-18 17:45:39.000000 pulumi_okta-4.9.0a1713462165/pulumi_okta/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20955 2024-04-18 17:45:39.000000 pulumi_okta-4.9.0a1713462165/pulumi_okta/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-04-18 17:45:39.000000 pulumi_okta-4.9.0a1713462165/pulumi_okta/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)    21518 2024-04-18 17:45:39.000000 pulumi_okta-4.9.0a1713462165/pulumi_okta/admin_role_custom.py
--rw-r--r--   0 runner    (1001) docker     (127)    11759 2024-04-18 17:45:39.000000 pulumi_okta-4.9.0a1713462165/pulumi_okta/admin_role_custom_assignments.py
--rw-r--r--   0 runner    (1001) docker     (127)    15488 2024-04-18 17:45:39.000000 pulumi_okta-4.9.0a1713462165/pulumi_okta/admin_role_targets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 17:45:45.545199 pulumi_okta-4.9.0a1713462165/pulumi_okta/app/
--rw-r--r--   0 runner    (1001) docker     (127)      831 2024-04-18 17:45:39.000000 pulumi_okta-4.9.0a1713462165/pulumi_okta/app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16246 2024-04-18 17:45:39.000000 pulumi_okta-4.9.0a1713462165/pulumi_okta/app/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9829 2024-04-18 17:45:39.000000 pulumi_okta-4.9.0a1713462165/pulumi_okta/app/access_policy_assignment.py
--rw-r--r--   0 runner    (1001) docker     (127)    64103 2024-04-18 17:45:39.000000 pulumi_okta-4.9.0a1713462165/pulumi_okta/app/auto_login.py
--rw-r--r--   0 runner    (1001) docker     (127)    37151 2024-04-18 17:45:39.000000 pulumi_okta-4.9.0a1713462165/pulumi_okta/app/basic_auth.py
--rw-r--r--   0 runner    (1001) docker     (127)    40464 2024-04-18 17:45:39.000000 pulumi_okta-4.9.0a1713462165/pulumi_okta/app/bookmark.py
--rw-r--r--   0 runner    (1001) docker     (127)    10454 2024-04-18 17:45:39.000000 pulumi_okta-4.9.0a1713462165/pulumi_okta/app/get_app.py
--rw-r--r--   0 runner    (1001) docker     (127)     7301 2024-04-18 17:45:39.000000 pulumi_okta-4.9.0a1713462165/pulumi_okta/app/get_metadata_saml.py
--rw-r--r--   0 runner    (1001) docker     (127)    18140 2024-04-18 17:45:39.000000 pulumi_okta-4.9.0a1713462165/pulumi_okta/app/get_oauth.py
--rw-r--r--   0 runner    (1001) docker     (127)    32406 2024-04-18 17:45:39.000000 pulumi_okta-4.9.0a1713462165/pulumi_okta/app/get_saml.py
--rw-r--r--   0 runner    (1001) docker     (127)    14663 2024-04-18 17:45:39.000000 pulumi_okta-4.9.0a1713462165/pulumi_okta/app/group_assignment.py
--rw-r--r--   0 runner    (1001) docker     (127)   147044 2024-04-18 17:45:39.000000 pulumi_okta-4.9.0a1713462165/pulumi_okta/app/o_auth.py
--rw-r--r--   0 runner    (1001) docker     (127)    10193 2024-04-18 17:45:39.000000 pulumi_okta-4.9.0a1713462165/pulumi_okta/app/o_auth_post_logout_redirect_uri.py
--rw-r--r--   0 runner    (1001) docker     (127)     9587 2024-04-18 17:45:39.000000 pulumi_okta-4.9.0a1713462165/pulumi_okta/app/o_auth_redirect_uri.py
--rw-r--r--   0 runner    (1001) docker     (127)    16237 2024-04-18 17:45:39.000000 pulumi_okta-4.9.0a1713462165/pulumi_okta/app/oauth_role_assignment.py
--rw-r--r--   0 runner    (1001) docker     (127)    15884 2024-04-18 17:45:39.000000 pulumi_okta-4.9.0a1713462165/pulumi_okta/app/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)   138332 2024-04-18 17:45:39.000000 pulumi_okta-4.9.0a1713462165/pulumi_okta/app/saml.py
--rw-r--r--   0 runner    (1001) docker     (127)    72919 2024-04-18 17:45:39.000000 pulumi_okta-4.9.0a1713462165/pulumi_okta/app/secure_password_store.py
--rw-r--r--   0 runner    (1001) docker     (127)    59554 2024-04-18 17:45:39.000000 pulumi_okta-4.9.0a1713462165/pulumi_okta/app/swa.py
--rw-r--r--   0 runner    (1001) docker     (127)    67402 2024-04-18 17:45:39.000000 pulumi_okta-4.9.0a1713462165/pulumi_okta/app/three_field.py
--rw-r--r--   0 runner    (1001) docker     (127)    18188 2024-04-18 17:45:39.000000 pulumi_okta-4.9.0a1713462165/pulumi_okta/app/user.py
--rw-r--r--   0 runner    (1001) docker     (127)    10358 2024-04-18 17:45:39.000000 pulumi_okta-4.9.0a1713462165/pulumi_okta/app_group_assignments.py
--rw-r--r--   0 runner    (1001) docker     (127)    11012 2024-04-18 17:45:39.000000 pulumi_okta-4.9.0a1713462165/pulumi_okta/app_oauth_api_scope.py
--rw-r--r--   0 runner    (1001) docker     (127)    10157 2024-04-18 17:45:39.000000 pulumi_okta-4.9.0a1713462165/pulumi_okta/app_saml_app_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)    66199 2024-04-18 17:45:39.000000 pulumi_okta-4.9.0a1713462165/pulumi_okta/app_shared_credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)    10104 2024-04-18 17:45:39.000000 pulumi_okta-4.9.0a1713462165/pulumi_okta/app_signon_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)    91790 2024-04-18 17:45:39.000000 pulumi_okta-4.9.0a1713462165/pulumi_okta/app_signon_policy_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)    23715 2024-04-18 17:45:39.000000 pulumi_okta-4.9.0a1713462165/pulumi_okta/app_user_base_schema_property.py
--rw-r--r--   0 runner    (1001) docker     (127)    51605 2024-04-18 17:45:39.000000 pulumi_okta-4.9.0a1713462165/pulumi_okta/app_user_schema_property.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 17:45:45.549199 pulumi_okta-4.9.0a1713462165/pulumi_okta/auth/
--rw-r--r--   0 runner    (1001) docker     (127)      559 2024-04-18 17:45:39.000000 pulumi_okta-4.9.0a1713462165/pulumi_okta/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7829 2024-04-18 17:45:39.000000 pulumi_okta-4.9.0a1713462165/pulumi_okta/auth/get_server.py
--rw-r--r--   0 runner    (1001) docker     (127)     5536 2024-04-18 17:45:39.000000 pulumi_okta-4.9.0a1713462165/pulumi_okta/auth/get_server_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)     3796 2024-04-18 17:45:39.000000 pulumi_okta-4.9.0a1713462165/pulumi_okta/auth/get_server_scopes.py
--rw-r--r--   0 runner    (1001) docker     (127)     3495 2024-04-18 17:45:39.000000 pulumi_okta-4.9.0a1713462165/pulumi_okta/auth/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    23637 2024-04-18 17:45:39.000000 pulumi_okta-4.9.0a1713462165/pulumi_okta/auth/server.py
--rw-r--r--   0 runner    (1001) docker     (127)    24790 2024-04-18 17:45:39.000000 pulumi_okta-4.9.0a1713462165/pulumi_okta/auth/server_claim.py
--rw-r--r--   0 runner    (1001) docker     (127)    17752 2024-04-18 17:45:39.000000 pulumi_okta-4.9.0a1713462165/pulumi_okta/auth/server_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)    48011 2024-04-18 17:45:39.000000 pulumi_okta-4.9.0a1713462165/pulumi_okta/auth/server_policy_claim.py
--rw-r--r--   0 runner    (1001) docker     (127)    47653 2024-04-18 17:45:39.000000 pulumi_okta-4.9.0a1713462165/pulumi_okta/auth/server_policy_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)    22628 2024-04-18 17:45:39.000000 pulumi_okta-4.9.0a1713462165/pulumi_okta/auth/server_scope.py
--rw-r--r--   0 runner    (1001) docker     (127)    20182 2024-04-18 17:45:39.000000 pulumi_okta-4.9.0a1713462165/pulumi_okta/auth_server_claim_default.py
--rw-r--r--   0 runner    (1001) docker     (127)    24099 2024-04-18 17:45:39.000000 pulumi_okta-4.9.0a1713462165/pulumi_okta/auth_server_default.py
--rw-r--r--   0 runner    (1001) docker     (127)    47734 2024-04-18 17:45:39.000000 pulumi_okta-4.9.0a1713462165/pulumi_okta/authenticator.py
--rw-r--r--   0 runner    (1001) docker     (127)    24484 2024-04-18 17:45:39.000000 pulumi_okta-4.9.0a1713462165/pulumi_okta/behaviour.py
--rw-r--r--   0 runner    (1001) docker     (127)    30565 2024-04-18 17:45:39.000000 pulumi_okta-4.9.0a1713462165/pulumi_okta/brand.py
--rw-r--r--   0 runner    (1001) docker     (127)    13056 2024-04-18 17:45:39.000000 pulumi_okta-4.9.0a1713462165/pulumi_okta/captcha.py
--rw-r--r--   0 runner    (1001) docker     (127)    11412 2024-04-18 17:45:39.000000 pulumi_okta-4.9.0a1713462165/pulumi_okta/captcha_org_wide_settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 17:45:45.549199 pulumi_okta-4.9.0a1713462165/pulumi_okta/config/
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-18 17:45:39.000000 pulumi_okta-4.9.0a1713462165/pulumi_okta/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2358 2024-04-18 17:45:39.000000 pulumi_okta-4.9.0a1713462165/pulumi_okta/config/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4218 2024-04-18 17:45:39.000000 pulumi_okta-4.9.0a1713462165/pulumi_okta/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (127)    14318 2024-04-18 17:45:39.000000 pulumi_okta-4.9.0a1713462165/pulumi_okta/domain.py
--rw-r--r--   0 runner    (1001) docker     (127)    17490 2024-04-18 17:45:39.000000 pulumi_okta-4.9.0a1713462165/pulumi_okta/domain_certificate.py
--rw-r--r--   0 runner    (1001) docker     (127)     6883 2024-04-18 17:45:39.000000 pulumi_okta-4.9.0a1713462165/pulumi_okta/domain_verification.py
--rw-r--r--   0 runner    (1001) docker     (127)    39467 2024-04-18 17:45:39.000000 pulumi_okta-4.9.0a1713462165/pulumi_okta/email_customization.py
--rw-r--r--   0 runner    (1001) docker     (127)    13021 2024-04-18 17:45:39.000000 pulumi_okta-4.9.0a1713462165/pulumi_okta/email_sender.py
--rw-r--r--   0 runner    (1001) docker     (127)     7015 2024-04-18 17:45:39.000000 pulumi_okta-4.9.0a1713462165/pulumi_okta/email_sender_verification.py
--rw-r--r--   0 runner    (1001) docker     (127)    18582 2024-04-18 17:45:39.000000 pulumi_okta-4.9.0a1713462165/pulumi_okta/event_hook.py
--rw-r--r--   0 runner    (1001) docker     (127)     7992 2024-04-18 17:45:39.000000 pulumi_okta-4.9.0a1713462165/pulumi_okta/event_hook_verification.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 17:45:45.549199 pulumi_okta-4.9.0a1713462165/pulumi_okta/factor/
--rw-r--r--   0 runner    (1001) docker     (127)      291 2024-04-18 17:45:39.000000 pulumi_okta-4.9.0a1713462165/pulumi_okta/factor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9938 2024-04-18 17:45:39.000000 pulumi_okta-4.9.0a1713462165/pulumi_okta/factor/factor.py
--rw-r--r--   0 runner    (1001) docker     (127)    19587 2024-04-18 17:45:39.000000 pulumi_okta-4.9.0a1713462165/pulumi_okta/factor_totp.py
--rw-r--r--   0 runner    (1001) docker     (127)     3406 2024-04-18 17:45:39.000000 pulumi_okta-4.9.0a1713462165/pulumi_okta/get_app_group_assignments.py
--rw-r--r--   0 runner    (1001) docker     (127)     4169 2024-04-18 17:45:39.000000 pulumi_okta-4.9.0a1713462165/pulumi_okta/get_app_signon_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)     3368 2024-04-18 17:45:39.000000 pulumi_okta-4.9.0a1713462165/pulumi_okta/get_app_user_assignments.py
--rw-r--r--   0 runner    (1001) docker     (127)     7367 2024-04-18 17:45:39.000000 pulumi_okta-4.9.0a1713462165/pulumi_okta/get_auth_server_claim.py
--rw-r--r--   0 runner    (1001) docker     (127)     3887 2024-04-18 17:45:39.000000 pulumi_okta-4.9.0a1713462165/pulumi_okta/get_auth_server_claims.py
--rw-r--r--   0 runner    (1001) docker     (127)     9487 2024-04-18 17:45:39.000000 pulumi_okta-4.9.0a1713462165/pulumi_okta/get_authenticator.py
--rw-r--r--   0 runner    (1001) docker     (127)     4238 2024-04-18 17:45:39.000000 pulumi_okta-4.9.0a1713462165/pulumi_okta/get_behaviour.py
--rw-r--r--   0 runner    (1001) docker     (127)     3425 2024-04-18 17:45:39.000000 pulumi_okta-4.9.0a1713462165/pulumi_okta/get_behaviours.py
--rw-r--r--   0 runner    (1001) docker     (127)     4989 2024-04-18 17:45:39.000000 pulumi_okta-4.9.0a1713462165/pulumi_okta/get_brand.py
--rw-r--r--   0 runner    (1001) docker     (127)     2786 2024-04-18 17:45:39.000000 pulumi_okta-4.9.0a1713462165/pulumi_okta/get_brands.py
--rw-r--r--   0 runner    (1001) docker     (127)     6857 2024-04-18 17:45:39.000000 pulumi_okta-4.9.0a1713462165/pulumi_okta/get_email_customization.py
--rw-r--r--   0 runner    (1001) docker     (127)     4600 2024-04-18 17:45:39.000000 pulumi_okta-4.9.0a1713462165/pulumi_okta/get_email_customizations.py
--rw-r--r--   0 runner    (1001) docker     (127)     5529 2024-04-18 17:45:39.000000 pulumi_okta-4.9.0a1713462165/pulumi_okta/get_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     7227 2024-04-18 17:45:39.000000 pulumi_okta-4.9.0a1713462165/pulumi_okta/get_network_zone.py
--rw-r--r--   0 runner    (1001) docker     (127)     5839 2024-04-18 17:45:39.000000 pulumi_okta-4.9.0a1713462165/pulumi_okta/get_role_subscription.py
--rw-r--r--   0 runner    (1001) docker     (127)     3783 2024-04-18 17:45:39.000000 pulumi_okta-4.9.0a1713462165/pulumi_okta/get_template.py
--rw-r--r--   0 runner    (1001) docker     (127)     3406 2024-04-18 17:45:39.000000 pulumi_okta-4.9.0a1713462165/pulumi_okta/get_templates.py
--rw-r--r--   0 runner    (1001) docker     (127)    11335 2024-04-18 17:45:39.000000 pulumi_okta-4.9.0a1713462165/pulumi_okta/get_theme.py
--rw-r--r--   0 runner    (1001) docker     (127)     3190 2024-04-18 17:45:39.000000 pulumi_okta-4.9.0a1713462165/pulumi_okta/get_themes.py
--rw-r--r--   0 runner    (1001) docker     (127)     3995 2024-04-18 17:45:39.000000 pulumi_okta-4.9.0a1713462165/pulumi_okta/get_trusted_origins.py
--rw-r--r--   0 runner    (1001) docker     (127)     4245 2024-04-18 17:45:39.000000 pulumi_okta-4.9.0a1713462165/pulumi_okta/get_user_security_questions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 17:45:45.549199 pulumi_okta-4.9.0a1713462165/pulumi_okta/group/
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-04-18 17:45:39.000000 pulumi_okta-4.9.0a1713462165/pulumi_okta/group/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3951 2024-04-18 17:45:39.000000 pulumi_okta-4.9.0a1713462165/pulumi_okta/group/get_everyone_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     7349 2024-04-18 17:45:39.000000 pulumi_okta-4.9.0a1713462165/pulumi_okta/group/get_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     6192 2024-04-18 17:45:39.000000 pulumi_okta-4.9.0a1713462165/pulumi_okta/group/get_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)    15435 2024-04-18 17:45:39.000000 pulumi_okta-4.9.0a1713462165/pulumi_okta/group/group.py
--rw-r--r--   0 runner    (1001) docker     (127)    24255 2024-04-18 17:45:39.000000 pulumi_okta-4.9.0a1713462165/pulumi_okta/group/role.py
--rw-r--r--   0 runner    (1001) docker     (127)    21005 2024-04-18 17:45:39.000000 pulumi_okta-4.9.0a1713462165/pulumi_okta/group/rule.py
--rw-r--r--   0 runner    (1001) docker     (127)    13869 2024-04-18 17:45:39.000000 pulumi_okta-4.9.0a1713462165/pulumi_okta/group_memberships.py
--rw-r--r--   0 runner    (1001) docker     (127)    47368 2024-04-18 17:45:39.000000 pulumi_okta-4.9.0a1713462165/pulumi_okta/group_schema_property.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 17:45:45.553199 pulumi_okta-4.9.0a1713462165/pulumi_okta/idp/
--rw-r--r--   0 runner    (1001) docker     (127)      462 2024-04-18 17:45:39.000000 pulumi_okta-4.9.0a1713462165/pulumi_okta/idp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7898 2024-04-18 17:45:39.000000 pulumi_okta-4.9.0a1713462165/pulumi_okta/idp/get_metadata_saml.py
--rw-r--r--   0 runner    (1001) docker     (127)    11858 2024-04-18 17:45:39.000000 pulumi_okta-4.9.0a1713462165/pulumi_okta/idp/get_oidc.py
--rw-r--r--   0 runner    (1001) docker     (127)     9186 2024-04-18 17:45:39.000000 pulumi_okta-4.9.0a1713462165/pulumi_okta/idp/get_saml.py
--rw-r--r--   0 runner    (1001) docker     (127)    18055 2024-04-18 17:45:39.000000 pulumi_okta-4.9.0a1713462165/pulumi_okta/idp/get_social.py
--rw-r--r--   0 runner    (1001) docker     (127)    87549 2024-04-18 17:45:39.000000 pulumi_okta-4.9.0a1713462165/pulumi_okta/idp/oidc.py
--rw-r--r--   0 runner    (1001) docker     (127)    83562 2024-04-18 17:45:39.000000 pulumi_okta-4.9.0a1713462165/pulumi_okta/idp/saml.py
--rw-r--r--   0 runner    (1001) docker     (127)    15186 2024-04-18 17:45:39.000000 pulumi_okta-4.9.0a1713462165/pulumi_okta/idp/saml_key.py
--rw-r--r--   0 runner    (1001) docker     (127)    73088 2024-04-18 17:45:39.000000 pulumi_okta-4.9.0a1713462165/pulumi_okta/idp/social.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 17:45:45.553199 pulumi_okta-4.9.0a1713462165/pulumi_okta/index/
--rw-r--r--   0 runner    (1001) docker     (127)      609 2024-04-18 17:45:39.000000 pulumi_okta-4.9.0a1713462165/pulumi_okta/index/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    50207 2024-04-18 17:45:39.000000 pulumi_okta-4.9.0a1713462165/pulumi_okta/index/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    19077 2024-04-18 17:45:39.000000 pulumi_okta-4.9.0a1713462165/pulumi_okta/index/customized_signin_page.py
--rw-r--r--   0 runner    (1001) docker     (127)    15331 2024-04-18 17:45:39.000000 pulumi_okta-4.9.0a1713462165/pulumi_okta/index/email_domain.py
--rw-r--r--   0 runner    (1001) docker     (127)     7149 2024-04-18 17:45:39.000000 pulumi_okta-4.9.0a1713462165/pulumi_okta/index/email_domain_verification.py
--rw-r--r--   0 runner    (1001) docker     (127)     6074 2024-04-18 17:45:39.000000 pulumi_okta-4.9.0a1713462165/pulumi_okta/index/get_default_signin_page.py
--rw-r--r--   0 runner    (1001) docker     (127)     6742 2024-04-18 17:45:39.000000 pulumi_okta-4.9.0a1713462165/pulumi_okta/index/get_domain.py
--rw-r--r--   0 runner    (1001) docker     (127)     5199 2024-04-18 17:45:39.000000 pulumi_okta-4.9.0a1713462165/pulumi_okta/index/get_log_stream.py
--rw-r--r--   0 runner    (1001) docker     (127)     5502 2024-04-18 17:45:39.000000 pulumi_okta-4.9.0a1713462165/pulumi_okta/index/get_org_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)    12124 2024-04-18 17:45:39.000000 pulumi_okta-4.9.0a1713462165/pulumi_okta/index/log_stream.py
--rw-r--r--   0 runner    (1001) docker     (127)    43669 2024-04-18 17:45:39.000000 pulumi_okta-4.9.0a1713462165/pulumi_okta/index/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    18617 2024-04-18 17:45:39.000000 pulumi_okta-4.9.0a1713462165/pulumi_okta/index/preview_signin_page.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 17:45:45.557199 pulumi_okta-4.9.0a1713462165/pulumi_okta/inline/
--rw-r--r--   0 runner    (1001) docker     (127)      334 2024-04-18 17:45:39.000000 pulumi_okta-4.9.0a1713462165/pulumi_okta/inline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1590 2024-04-18 17:45:39.000000 pulumi_okta-4.9.0a1713462165/pulumi_okta/inline/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    19300 2024-04-18 17:45:39.000000 pulumi_okta-4.9.0a1713462165/pulumi_okta/inline/hook.py
--rw-r--r--   0 runner    (1001) docker     (127)     1277 2024-04-18 17:45:39.000000 pulumi_okta-4.9.0a1713462165/pulumi_okta/inline/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    18947 2024-04-18 17:45:39.000000 pulumi_okta-4.9.0a1713462165/pulumi_okta/link_definition.py
--rw-r--r--   0 runner    (1001) docker     (127)    14827 2024-04-18 17:45:39.000000 pulumi_okta-4.9.0a1713462165/pulumi_okta/link_value.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 17:45:45.557199 pulumi_okta-4.9.0a1713462165/pulumi_okta/network/
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-04-18 17:45:39.000000 pulumi_okta-4.9.0a1713462165/pulumi_okta/network/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    26599 2024-04-18 17:45:39.000000 pulumi_okta-4.9.0a1713462165/pulumi_okta/network/zone.py
--rw-r--r--   0 runner    (1001) docker     (127)    36906 2024-04-18 17:45:39.000000 pulumi_okta-4.9.0a1713462165/pulumi_okta/org_configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     8808 2024-04-18 17:45:39.000000 pulumi_okta-4.9.0a1713462165/pulumi_okta/org_support.py
--rw-r--r--   0 runner    (1001) docker     (127)    37606 2024-04-18 17:45:39.000000 pulumi_okta-4.9.0a1713462165/pulumi_okta/outputs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 17:45:45.561199 pulumi_okta-4.9.0a1713462165/pulumi_okta/policy/
--rw-r--r--   0 runner    (1001) docker     (127)      748 2024-04-18 17:45:39.000000 pulumi_okta-4.9.0a1713462165/pulumi_okta/policy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15416 2024-04-18 17:45:39.000000 pulumi_okta-4.9.0a1713462165/pulumi_okta/policy/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    22720 2024-04-18 17:45:39.000000 pulumi_okta-4.9.0a1713462165/pulumi_okta/policy/device_assurance_android.py
--rw-r--r--   0 runner    (1001) docker     (127)    48372 2024-04-18 17:45:39.000000 pulumi_okta-4.9.0a1713462165/pulumi_okta/policy/device_assurance_chromeos.py
--rw-r--r--   0 runner    (1001) docker     (127)    17935 2024-04-18 17:45:39.000000 pulumi_okta-4.9.0a1713462165/pulumi_okta/policy/device_assurance_ios.py
--rw-r--r--   0 runner    (1001) docker     (127)    56471 2024-04-18 17:45:39.000000 pulumi_okta-4.9.0a1713462165/pulumi_okta/policy/device_assurance_macos.py
--rw-r--r--   0 runner    (1001) docker     (127)    71871 2024-04-18 17:45:39.000000 pulumi_okta-4.9.0a1713462165/pulumi_okta/policy/device_assurance_windows.py
--rw-r--r--   0 runner    (1001) docker     (127)     3811 2024-04-18 17:45:39.000000 pulumi_okta-4.9.0a1713462165/pulumi_okta/policy/get_default_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)     4211 2024-04-18 17:45:39.000000 pulumi_okta-4.9.0a1713462165/pulumi_okta/policy/get_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)    69364 2024-04-18 17:45:39.000000 pulumi_okta-4.9.0a1713462165/pulumi_okta/policy/mfa.py
--rw-r--r--   0 runner    (1001) docker     (127)    14488 2024-04-18 17:45:39.000000 pulumi_okta-4.9.0a1713462165/pulumi_okta/policy/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    79753 2024-04-18 17:45:39.000000 pulumi_okta-4.9.0a1713462165/pulumi_okta/policy/password.py
--rw-r--r--   0 runner    (1001) docker     (127)    50878 2024-04-18 17:45:39.000000 pulumi_okta-4.9.0a1713462165/pulumi_okta/policy/rule_idp_discovery.py
--rw-r--r--   0 runner    (1001) docker     (127)    34098 2024-04-18 17:45:39.000000 pulumi_okta-4.9.0a1713462165/pulumi_okta/policy/rule_mfa.py
--rw-r--r--   0 runner    (1001) docker     (127)    30687 2024-04-18 17:45:39.000000 pulumi_okta-4.9.0a1713462165/pulumi_okta/policy/rule_password.py
--rw-r--r--   0 runner    (1001) docker     (127)    69874 2024-04-18 17:45:39.000000 pulumi_okta-4.9.0a1713462165/pulumi_okta/policy/rule_signon.py
--rw-r--r--   0 runner    (1001) docker     (127)    13857 2024-04-18 17:45:39.000000 pulumi_okta-4.9.0a1713462165/pulumi_okta/policy/signon.py
--rw-r--r--   0 runner    (1001) docker     (127)    65477 2024-04-18 17:45:39.000000 pulumi_okta-4.9.0a1713462165/pulumi_okta/policy_mfa_default.py
--rw-r--r--   0 runner    (1001) docker     (127)    71555 2024-04-18 17:45:39.000000 pulumi_okta-4.9.0a1713462165/pulumi_okta/policy_password_default.py
--rw-r--r--   0 runner    (1001) docker     (127)     8421 2024-04-18 17:45:39.000000 pulumi_okta-4.9.0a1713462165/pulumi_okta/policy_profile_enrollment.py
--rw-r--r--   0 runner    (1001) docker     (127)    11812 2024-04-18 17:45:39.000000 pulumi_okta-4.9.0a1713462165/pulumi_okta/policy_profile_enrollment_apps.py
--rw-r--r--   0 runner    (1001) docker     (127)    34999 2024-04-18 17:45:39.000000 pulumi_okta-4.9.0a1713462165/pulumi_okta/policy_rule_profile_enrollment.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 17:45:45.561199 pulumi_okta-4.9.0a1713462165/pulumi_okta/profile/
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-04-18 17:45:39.000000 pulumi_okta-4.9.0a1713462165/pulumi_okta/profile/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2166 2024-04-18 17:45:39.000000 pulumi_okta-4.9.0a1713462165/pulumi_okta/profile/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    23956 2024-04-18 17:45:39.000000 pulumi_okta-4.9.0a1713462165/pulumi_okta/profile/mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)     2246 2024-04-18 17:45:39.000000 pulumi_okta-4.9.0a1713462165/pulumi_okta/profile/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    23808 2024-04-18 17:45:39.000000 pulumi_okta-4.9.0a1713462165/pulumi_okta/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-18 17:45:39.000000 pulumi_okta-4.9.0a1713462165/pulumi_okta/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 17:45:39.000000 pulumi_okta-4.9.0a1713462165/pulumi_okta/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    14054 2024-04-18 17:45:39.000000 pulumi_okta-4.9.0a1713462165/pulumi_okta/rate_limiting.py
--rw-r--r--   0 runner    (1001) docker     (127)    11745 2024-04-18 17:45:39.000000 pulumi_okta-4.9.0a1713462165/pulumi_okta/resource_set.py
--rw-r--r--   0 runner    (1001) docker     (127)    21342 2024-04-18 17:45:39.000000 pulumi_okta-4.9.0a1713462165/pulumi_okta/role_subscription.py
--rw-r--r--   0 runner    (1001) docker     (127)    21992 2024-04-18 17:45:39.000000 pulumi_okta-4.9.0a1713462165/pulumi_okta/security_notification_emails.py
--rw-r--r--   0 runner    (1001) docker     (127)    11664 2024-04-18 17:45:39.000000 pulumi_okta-4.9.0a1713462165/pulumi_okta/template_sms.py
--rw-r--r--   0 runner    (1001) docker     (127)    42952 2024-04-18 17:45:39.000000 pulumi_okta-4.9.0a1713462165/pulumi_okta/theme.py
--rw-r--r--   0 runner    (1001) docker     (127)    15010 2024-04-18 17:45:39.000000 pulumi_okta-4.9.0a1713462165/pulumi_okta/threat_insight_settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 17:45:45.561199 pulumi_okta-4.9.0a1713462165/pulumi_okta/trustedorigin/
--rw-r--r--   0 runner    (1001) docker     (127)      291 2024-04-18 17:45:39.000000 pulumi_okta-4.9.0a1713462165/pulumi_okta/trustedorigin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12718 2024-04-18 17:45:39.000000 pulumi_okta-4.9.0a1713462165/pulumi_okta/trustedorigin/origin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 17:45:45.561199 pulumi_okta-4.9.0a1713462165/pulumi_okta/user/
--rw-r--r--   0 runner    (1001) docker     (127)      484 2024-04-18 17:45:39.000000 pulumi_okta-4.9.0a1713462165/pulumi_okta/user/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9846 2024-04-18 17:45:39.000000 pulumi_okta-4.9.0a1713462165/pulumi_okta/user/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    25124 2024-04-18 17:45:39.000000 pulumi_okta-4.9.0a1713462165/pulumi_okta/user/get_user.py
--rw-r--r--   0 runner    (1001) docker     (127)     3675 2024-04-18 17:45:39.000000 pulumi_okta-4.9.0a1713462165/pulumi_okta/user/get_user_profile_mapping_source.py
--rw-r--r--   0 runner    (1001) docker     (127)     3965 2024-04-18 17:45:39.000000 pulumi_okta-4.9.0a1713462165/pulumi_okta/user/get_user_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     9173 2024-04-18 17:45:39.000000 pulumi_okta-4.9.0a1713462165/pulumi_okta/user/get_users.py
--rw-r--r--   0 runner    (1001) docker     (127)    22357 2024-04-18 17:45:39.000000 pulumi_okta-4.9.0a1713462165/pulumi_okta/user/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)   100207 2024-04-18 17:45:39.000000 pulumi_okta-4.9.0a1713462165/pulumi_okta/user/user.py
--rw-r--r--   0 runner    (1001) docker     (127)    10123 2024-04-18 17:45:39.000000 pulumi_okta-4.9.0a1713462165/pulumi_okta/user/user_type.py
--rw-r--r--   0 runner    (1001) docker     (127)    13809 2024-04-18 17:45:39.000000 pulumi_okta-4.9.0a1713462165/pulumi_okta/user_admin_roles.py
--rw-r--r--   0 runner    (1001) docker     (127)    23053 2024-04-18 17:45:39.000000 pulumi_okta-4.9.0a1713462165/pulumi_okta/user_base_schema_property.py
--rw-r--r--   0 runner    (1001) docker     (127)    14110 2024-04-18 17:45:39.000000 pulumi_okta-4.9.0a1713462165/pulumi_okta/user_factor_question.py
--rw-r--r--   0 runner    (1001) docker     (127)     9000 2024-04-18 17:45:39.000000 pulumi_okta-4.9.0a1713462165/pulumi_okta/user_group_memberships.py
--rw-r--r--   0 runner    (1001) docker     (127)    51832 2024-04-18 17:45:39.000000 pulumi_okta-4.9.0a1713462165/pulumi_okta/user_schema_property.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 17:45:45.561199 pulumi_okta-4.9.0a1713462165/pulumi_okta.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3351 2024-04-18 17:45:45.000000 pulumi_okta-4.9.0a1713462165/pulumi_okta.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6157 2024-04-18 17:45:45.000000 pulumi_okta-4.9.0a1713462165/pulumi_okta.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 17:45:45.000000 pulumi_okta-4.9.0a1713462165/pulumi_okta.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-18 17:45:45.000000 pulumi_okta-4.9.0a1713462165/pulumi_okta.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-18 17:45:45.000000 pulumi_okta-4.9.0a1713462165/pulumi_okta.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      663 2024-04-18 17:45:39.000000 pulumi_okta-4.9.0a1713462165/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 17:45:45.565199 pulumi_okta-4.9.0a1713462165/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 20:09:12.958008 pulumi_okta-4.9.0a1713902092/
+-rw-r--r--   0 runner    (1001) docker     (127)     3351 2024-04-23 20:09:12.958008 pulumi_okta-4.9.0a1713902092/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2913 2024-04-23 20:09:06.000000 pulumi_okta-4.9.0a1713902092/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 20:09:12.938009 pulumi_okta-4.9.0a1713902092/pulumi_okta/
+-rw-r--r--   0 runner    (1001) docker     (127)    21302 2024-04-23 20:09:06.000000 pulumi_okta-4.9.0a1713902092/pulumi_okta/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20463 2024-04-23 20:09:06.000000 pulumi_okta-4.9.0a1713902092/pulumi_okta/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-04-23 20:09:06.000000 pulumi_okta-4.9.0a1713902092/pulumi_okta/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21362 2024-04-23 20:09:06.000000 pulumi_okta-4.9.0a1713902092/pulumi_okta/admin_role_custom.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11759 2024-04-23 20:09:06.000000 pulumi_okta-4.9.0a1713902092/pulumi_okta/admin_role_custom_assignments.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15332 2024-04-23 20:09:06.000000 pulumi_okta-4.9.0a1713902092/pulumi_okta/admin_role_targets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 20:09:12.942009 pulumi_okta-4.9.0a1713902092/pulumi_okta/app/
+-rw-r--r--   0 runner    (1001) docker     (127)      831 2024-04-23 20:09:06.000000 pulumi_okta-4.9.0a1713902092/pulumi_okta/app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15781 2024-04-23 20:09:06.000000 pulumi_okta-4.9.0a1713902092/pulumi_okta/app/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9829 2024-04-23 20:09:06.000000 pulumi_okta-4.9.0a1713902092/pulumi_okta/app/access_policy_assignment.py
+-rw-r--r--   0 runner    (1001) docker     (127)    63791 2024-04-23 20:09:06.000000 pulumi_okta-4.9.0a1713902092/pulumi_okta/app/auto_login.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36995 2024-04-23 20:09:06.000000 pulumi_okta-4.9.0a1713902092/pulumi_okta/app/basic_auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40308 2024-04-23 20:09:06.000000 pulumi_okta-4.9.0a1713902092/pulumi_okta/app/bookmark.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10314 2024-04-23 20:09:06.000000 pulumi_okta-4.9.0a1713902092/pulumi_okta/app/get_app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7161 2024-04-23 20:09:06.000000 pulumi_okta-4.9.0a1713902092/pulumi_okta/app/get_metadata_saml.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18000 2024-04-23 20:09:06.000000 pulumi_okta-4.9.0a1713902092/pulumi_okta/app/get_oauth.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32266 2024-04-23 20:09:06.000000 pulumi_okta-4.9.0a1713902092/pulumi_okta/app/get_saml.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14663 2024-04-23 20:09:06.000000 pulumi_okta-4.9.0a1713902092/pulumi_okta/app/group_assignment.py
+-rw-r--r--   0 runner    (1001) docker     (127)   146700 2024-04-23 20:09:06.000000 pulumi_okta-4.9.0a1713902092/pulumi_okta/app/o_auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10037 2024-04-23 20:09:06.000000 pulumi_okta-4.9.0a1713902092/pulumi_okta/app/o_auth_post_logout_redirect_uri.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9431 2024-04-23 20:09:06.000000 pulumi_okta-4.9.0a1713902092/pulumi_okta/app/o_auth_redirect_uri.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16081 2024-04-23 20:09:06.000000 pulumi_okta-4.9.0a1713902092/pulumi_okta/app/oauth_role_assignment.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15419 2024-04-23 20:09:06.000000 pulumi_okta-4.9.0a1713902092/pulumi_okta/app/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)   137735 2024-04-23 20:09:06.000000 pulumi_okta-4.9.0a1713902092/pulumi_okta/app/saml.py
+-rw-r--r--   0 runner    (1001) docker     (127)    72763 2024-04-23 20:09:06.000000 pulumi_okta-4.9.0a1713902092/pulumi_okta/app/secure_password_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)    59398 2024-04-23 20:09:06.000000 pulumi_okta-4.9.0a1713902092/pulumi_okta/app/swa.py
+-rw-r--r--   0 runner    (1001) docker     (127)    67402 2024-04-23 20:09:06.000000 pulumi_okta-4.9.0a1713902092/pulumi_okta/app/three_field.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18032 2024-04-23 20:09:06.000000 pulumi_okta-4.9.0a1713902092/pulumi_okta/app/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10202 2024-04-23 20:09:06.000000 pulumi_okta-4.9.0a1713902092/pulumi_okta/app_group_assignments.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10856 2024-04-23 20:09:06.000000 pulumi_okta-4.9.0a1713902092/pulumi_okta/app_oauth_api_scope.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10001 2024-04-23 20:09:06.000000 pulumi_okta-4.9.0a1713902092/pulumi_okta/app_saml_app_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)    66043 2024-04-23 20:09:06.000000 pulumi_okta-4.9.0a1713902092/pulumi_okta/app_shared_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9792 2024-04-23 20:09:06.000000 pulumi_okta-4.9.0a1713902092/pulumi_okta/app_signon_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    91374 2024-04-23 20:09:06.000000 pulumi_okta-4.9.0a1713902092/pulumi_okta/app_signon_policy_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23559 2024-04-23 20:09:06.000000 pulumi_okta-4.9.0a1713902092/pulumi_okta/app_user_base_schema_property.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51344 2024-04-23 20:09:06.000000 pulumi_okta-4.9.0a1713902092/pulumi_okta/app_user_schema_property.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 20:09:12.946009 pulumi_okta-4.9.0a1713902092/pulumi_okta/auth/
+-rw-r--r--   0 runner    (1001) docker     (127)      559 2024-04-23 20:09:06.000000 pulumi_okta-4.9.0a1713902092/pulumi_okta/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7689 2024-04-23 20:09:06.000000 pulumi_okta-4.9.0a1713902092/pulumi_okta/auth/get_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5396 2024-04-23 20:09:06.000000 pulumi_okta-4.9.0a1713902092/pulumi_okta/auth/get_server_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3656 2024-04-23 20:09:06.000000 pulumi_okta-4.9.0a1713902092/pulumi_okta/auth/get_server_scopes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3495 2024-04-23 20:09:06.000000 pulumi_okta-4.9.0a1713902092/pulumi_okta/auth/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23481 2024-04-23 20:09:06.000000 pulumi_okta-4.9.0a1713902092/pulumi_okta/auth/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24634 2024-04-23 20:09:06.000000 pulumi_okta-4.9.0a1713902092/pulumi_okta/auth/server_claim.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17596 2024-04-23 20:09:06.000000 pulumi_okta-4.9.0a1713902092/pulumi_okta/auth/server_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47855 2024-04-23 20:09:06.000000 pulumi_okta-4.9.0a1713902092/pulumi_okta/auth/server_policy_claim.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47497 2024-04-23 20:09:06.000000 pulumi_okta-4.9.0a1713902092/pulumi_okta/auth/server_policy_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22472 2024-04-23 20:09:06.000000 pulumi_okta-4.9.0a1713902092/pulumi_okta/auth/server_scope.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20026 2024-04-23 20:09:06.000000 pulumi_okta-4.9.0a1713902092/pulumi_okta/auth_server_claim_default.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23943 2024-04-23 20:09:06.000000 pulumi_okta-4.9.0a1713902092/pulumi_okta/auth_server_default.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47422 2024-04-23 20:09:06.000000 pulumi_okta-4.9.0a1713902092/pulumi_okta/authenticator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24328 2024-04-23 20:09:06.000000 pulumi_okta-4.9.0a1713902092/pulumi_okta/behaviour.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30565 2024-04-23 20:09:06.000000 pulumi_okta-4.9.0a1713902092/pulumi_okta/brand.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12900 2024-04-23 20:09:06.000000 pulumi_okta-4.9.0a1713902092/pulumi_okta/captcha.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11100 2024-04-23 20:09:06.000000 pulumi_okta-4.9.0a1713902092/pulumi_okta/captcha_org_wide_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 20:09:12.946009 pulumi_okta-4.9.0a1713902092/pulumi_okta/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-23 20:09:06.000000 pulumi_okta-4.9.0a1713902092/pulumi_okta/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2358 2024-04-23 20:09:06.000000 pulumi_okta-4.9.0a1713902092/pulumi_okta/config/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4218 2024-04-23 20:09:06.000000 pulumi_okta-4.9.0a1713902092/pulumi_okta/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14162 2024-04-23 20:09:06.000000 pulumi_okta-4.9.0a1713902092/pulumi_okta/domain.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17334 2024-04-23 20:09:06.000000 pulumi_okta-4.9.0a1713902092/pulumi_okta/domain_certificate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6727 2024-04-23 20:09:06.000000 pulumi_okta-4.9.0a1713902092/pulumi_okta/domain_verification.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39467 2024-04-23 20:09:06.000000 pulumi_okta-4.9.0a1713902092/pulumi_okta/email_customization.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12865 2024-04-23 20:09:06.000000 pulumi_okta-4.9.0a1713902092/pulumi_okta/email_sender.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6859 2024-04-23 20:09:06.000000 pulumi_okta-4.9.0a1713902092/pulumi_okta/email_sender_verification.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18426 2024-04-23 20:09:06.000000 pulumi_okta-4.9.0a1713902092/pulumi_okta/event_hook.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7836 2024-04-23 20:09:06.000000 pulumi_okta-4.9.0a1713902092/pulumi_okta/event_hook_verification.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 20:09:12.946009 pulumi_okta-4.9.0a1713902092/pulumi_okta/factor/
+-rw-r--r--   0 runner    (1001) docker     (127)      291 2024-04-23 20:09:06.000000 pulumi_okta-4.9.0a1713902092/pulumi_okta/factor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9782 2024-04-23 20:09:06.000000 pulumi_okta-4.9.0a1713902092/pulumi_okta/factor/factor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19431 2024-04-23 20:09:06.000000 pulumi_okta-4.9.0a1713902092/pulumi_okta/factor_totp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3266 2024-04-23 20:09:06.000000 pulumi_okta-4.9.0a1713902092/pulumi_okta/get_app_group_assignments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4029 2024-04-23 20:09:06.000000 pulumi_okta-4.9.0a1713902092/pulumi_okta/get_app_signon_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3228 2024-04-23 20:09:06.000000 pulumi_okta-4.9.0a1713902092/pulumi_okta/get_app_user_assignments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7227 2024-04-23 20:09:06.000000 pulumi_okta-4.9.0a1713902092/pulumi_okta/get_auth_server_claim.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3747 2024-04-23 20:09:06.000000 pulumi_okta-4.9.0a1713902092/pulumi_okta/get_auth_server_claims.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9207 2024-04-23 20:09:06.000000 pulumi_okta-4.9.0a1713902092/pulumi_okta/get_authenticator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4238 2024-04-23 20:09:06.000000 pulumi_okta-4.9.0a1713902092/pulumi_okta/get_behaviour.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3285 2024-04-23 20:09:06.000000 pulumi_okta-4.9.0a1713902092/pulumi_okta/get_behaviours.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4989 2024-04-23 20:09:06.000000 pulumi_okta-4.9.0a1713902092/pulumi_okta/get_brand.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2646 2024-04-23 20:09:06.000000 pulumi_okta-4.9.0a1713902092/pulumi_okta/get_brands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6857 2024-04-23 20:09:06.000000 pulumi_okta-4.9.0a1713902092/pulumi_okta/get_email_customization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4600 2024-04-23 20:09:06.000000 pulumi_okta-4.9.0a1713902092/pulumi_okta/get_email_customizations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5389 2024-04-23 20:09:06.000000 pulumi_okta-4.9.0a1713902092/pulumi_okta/get_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7087 2024-04-23 20:09:06.000000 pulumi_okta-4.9.0a1713902092/pulumi_okta/get_network_zone.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5699 2024-04-23 20:09:06.000000 pulumi_okta-4.9.0a1713902092/pulumi_okta/get_role_subscription.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3783 2024-04-23 20:09:06.000000 pulumi_okta-4.9.0a1713902092/pulumi_okta/get_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3406 2024-04-23 20:09:06.000000 pulumi_okta-4.9.0a1713902092/pulumi_okta/get_templates.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11335 2024-04-23 20:09:06.000000 pulumi_okta-4.9.0a1713902092/pulumi_okta/get_theme.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3190 2024-04-23 20:09:06.000000 pulumi_okta-4.9.0a1713902092/pulumi_okta/get_themes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3855 2024-04-23 20:09:06.000000 pulumi_okta-4.9.0a1713902092/pulumi_okta/get_trusted_origins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4105 2024-04-23 20:09:06.000000 pulumi_okta-4.9.0a1713902092/pulumi_okta/get_user_security_questions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 20:09:12.946009 pulumi_okta-4.9.0a1713902092/pulumi_okta/group/
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-04-23 20:09:06.000000 pulumi_okta-4.9.0a1713902092/pulumi_okta/group/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3811 2024-04-23 20:09:06.000000 pulumi_okta-4.9.0a1713902092/pulumi_okta/group/get_everyone_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7209 2024-04-23 20:09:06.000000 pulumi_okta-4.9.0a1713902092/pulumi_okta/group/get_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6052 2024-04-23 20:09:06.000000 pulumi_okta-4.9.0a1713902092/pulumi_okta/group/get_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15123 2024-04-23 20:09:06.000000 pulumi_okta-4.9.0a1713902092/pulumi_okta/group/group.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24099 2024-04-23 20:09:06.000000 pulumi_okta-4.9.0a1713902092/pulumi_okta/group/role.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20849 2024-04-23 20:09:06.000000 pulumi_okta-4.9.0a1713902092/pulumi_okta/group/rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13713 2024-04-23 20:09:06.000000 pulumi_okta-4.9.0a1713902092/pulumi_okta/group_memberships.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47772 2024-04-23 20:09:06.000000 pulumi_okta-4.9.0a1713902092/pulumi_okta/group_schema_property.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 20:09:12.946009 pulumi_okta-4.9.0a1713902092/pulumi_okta/idp/
+-rw-r--r--   0 runner    (1001) docker     (127)      462 2024-04-23 20:09:06.000000 pulumi_okta-4.9.0a1713902092/pulumi_okta/idp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7758 2024-04-23 20:09:06.000000 pulumi_okta-4.9.0a1713902092/pulumi_okta/idp/get_metadata_saml.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11718 2024-04-23 20:09:06.000000 pulumi_okta-4.9.0a1713902092/pulumi_okta/idp/get_oidc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9046 2024-04-23 20:09:06.000000 pulumi_okta-4.9.0a1713902092/pulumi_okta/idp/get_saml.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17915 2024-04-23 20:09:06.000000 pulumi_okta-4.9.0a1713902092/pulumi_okta/idp/get_social.py
+-rw-r--r--   0 runner    (1001) docker     (127)    87393 2024-04-23 20:09:06.000000 pulumi_okta-4.9.0a1713902092/pulumi_okta/idp/oidc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    83406 2024-04-23 20:09:06.000000 pulumi_okta-4.9.0a1713902092/pulumi_okta/idp/saml.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15030 2024-04-23 20:09:06.000000 pulumi_okta-4.9.0a1713902092/pulumi_okta/idp/saml_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)    72932 2024-04-23 20:09:06.000000 pulumi_okta-4.9.0a1713902092/pulumi_okta/idp/social.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 20:09:12.950008 pulumi_okta-4.9.0a1713902092/pulumi_okta/index/
+-rw-r--r--   0 runner    (1001) docker     (127)      609 2024-04-23 20:09:06.000000 pulumi_okta-4.9.0a1713902092/pulumi_okta/index/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50207 2024-04-23 20:09:06.000000 pulumi_okta-4.9.0a1713902092/pulumi_okta/index/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19077 2024-04-23 20:09:06.000000 pulumi_okta-4.9.0a1713902092/pulumi_okta/index/customized_signin_page.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15175 2024-04-23 20:09:06.000000 pulumi_okta-4.9.0a1713902092/pulumi_okta/index/email_domain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6993 2024-04-23 20:09:06.000000 pulumi_okta-4.9.0a1713902092/pulumi_okta/index/email_domain_verification.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6074 2024-04-23 20:09:06.000000 pulumi_okta-4.9.0a1713902092/pulumi_okta/index/get_default_signin_page.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6602 2024-04-23 20:09:06.000000 pulumi_okta-4.9.0a1713902092/pulumi_okta/index/get_domain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5059 2024-04-23 20:09:06.000000 pulumi_okta-4.9.0a1713902092/pulumi_okta/index/get_log_stream.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5362 2024-04-23 20:09:06.000000 pulumi_okta-4.9.0a1713902092/pulumi_okta/index/get_org_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12124 2024-04-23 20:09:06.000000 pulumi_okta-4.9.0a1713902092/pulumi_okta/index/log_stream.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43669 2024-04-23 20:09:06.000000 pulumi_okta-4.9.0a1713902092/pulumi_okta/index/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18617 2024-04-23 20:09:06.000000 pulumi_okta-4.9.0a1713902092/pulumi_okta/index/preview_signin_page.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 20:09:12.950008 pulumi_okta-4.9.0a1713902092/pulumi_okta/inline/
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-04-23 20:09:06.000000 pulumi_okta-4.9.0a1713902092/pulumi_okta/inline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-04-23 20:09:06.000000 pulumi_okta-4.9.0a1713902092/pulumi_okta/inline/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19655 2024-04-23 20:09:06.000000 pulumi_okta-4.9.0a1713902092/pulumi_okta/inline/hook.py
+-rw-r--r--   0 runner    (1001) docker     (127)      919 2024-04-23 20:09:06.000000 pulumi_okta-4.9.0a1713902092/pulumi_okta/inline/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18791 2024-04-23 20:09:06.000000 pulumi_okta-4.9.0a1713902092/pulumi_okta/link_definition.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14671 2024-04-23 20:09:06.000000 pulumi_okta-4.9.0a1713902092/pulumi_okta/link_value.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 20:09:12.950008 pulumi_okta-4.9.0a1713902092/pulumi_okta/network/
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-04-23 20:09:06.000000 pulumi_okta-4.9.0a1713902092/pulumi_okta/network/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26287 2024-04-23 20:09:06.000000 pulumi_okta-4.9.0a1713902092/pulumi_okta/network/zone.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36750 2024-04-23 20:09:06.000000 pulumi_okta-4.9.0a1713902092/pulumi_okta/org_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8652 2024-04-23 20:09:06.000000 pulumi_okta-4.9.0a1713902092/pulumi_okta/org_support.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37142 2024-04-23 20:09:06.000000 pulumi_okta-4.9.0a1713902092/pulumi_okta/outputs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 20:09:12.954008 pulumi_okta-4.9.0a1713902092/pulumi_okta/policy/
+-rw-r--r--   0 runner    (1001) docker     (127)      748 2024-04-23 20:09:06.000000 pulumi_okta-4.9.0a1713902092/pulumi_okta/policy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14142 2024-04-23 20:09:06.000000 pulumi_okta-4.9.0a1713902092/pulumi_okta/policy/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22720 2024-04-23 20:09:06.000000 pulumi_okta-4.9.0a1713902092/pulumi_okta/policy/device_assurance_android.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48216 2024-04-23 20:09:06.000000 pulumi_okta-4.9.0a1713902092/pulumi_okta/policy/device_assurance_chromeos.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17935 2024-04-23 20:09:06.000000 pulumi_okta-4.9.0a1713902092/pulumi_okta/policy/device_assurance_ios.py
+-rw-r--r--   0 runner    (1001) docker     (127)    56471 2024-04-23 20:09:06.000000 pulumi_okta-4.9.0a1713902092/pulumi_okta/policy/device_assurance_macos.py
+-rw-r--r--   0 runner    (1001) docker     (127)    71871 2024-04-23 20:09:06.000000 pulumi_okta-4.9.0a1713902092/pulumi_okta/policy/device_assurance_windows.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3671 2024-04-23 20:09:06.000000 pulumi_okta-4.9.0a1713902092/pulumi_okta/policy/get_default_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4071 2024-04-23 20:09:06.000000 pulumi_okta-4.9.0a1713902092/pulumi_okta/policy/get_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    69208 2024-04-23 20:09:06.000000 pulumi_okta-4.9.0a1713902092/pulumi_okta/policy/mfa.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13242 2024-04-23 20:09:06.000000 pulumi_okta-4.9.0a1713902092/pulumi_okta/policy/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    79597 2024-04-23 20:09:06.000000 pulumi_okta-4.9.0a1713902092/pulumi_okta/policy/password.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49623 2024-04-23 20:09:06.000000 pulumi_okta-4.9.0a1713902092/pulumi_okta/policy/rule_idp_discovery.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32999 2024-04-23 20:09:06.000000 pulumi_okta-4.9.0a1713902092/pulumi_okta/policy/rule_mfa.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30687 2024-04-23 20:09:06.000000 pulumi_okta-4.9.0a1713902092/pulumi_okta/policy/rule_password.py
+-rw-r--r--   0 runner    (1001) docker     (127)    69718 2024-04-23 20:09:06.000000 pulumi_okta-4.9.0a1713902092/pulumi_okta/policy/rule_signon.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13701 2024-04-23 20:09:06.000000 pulumi_okta-4.9.0a1713902092/pulumi_okta/policy/signon.py
+-rw-r--r--   0 runner    (1001) docker     (127)    65321 2024-04-23 20:09:06.000000 pulumi_okta-4.9.0a1713902092/pulumi_okta/policy_mfa_default.py
+-rw-r--r--   0 runner    (1001) docker     (127)    71399 2024-04-23 20:09:06.000000 pulumi_okta-4.9.0a1713902092/pulumi_okta/policy_password_default.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8265 2024-04-23 20:09:06.000000 pulumi_okta-4.9.0a1713902092/pulumi_okta/policy_profile_enrollment.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11656 2024-04-23 20:09:06.000000 pulumi_okta-4.9.0a1713902092/pulumi_okta/policy_profile_enrollment_apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34771 2024-04-23 20:09:06.000000 pulumi_okta-4.9.0a1713902092/pulumi_okta/policy_rule_profile_enrollment.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 20:09:12.954008 pulumi_okta-4.9.0a1713902092/pulumi_okta/profile/
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-04-23 20:09:06.000000 pulumi_okta-4.9.0a1713902092/pulumi_okta/profile/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2166 2024-04-23 20:09:06.000000 pulumi_okta-4.9.0a1713902092/pulumi_okta/profile/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23800 2024-04-23 20:09:06.000000 pulumi_okta-4.9.0a1713902092/pulumi_okta/profile/mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2246 2024-04-23 20:09:06.000000 pulumi_okta-4.9.0a1713902092/pulumi_okta/profile/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23808 2024-04-23 20:09:06.000000 pulumi_okta-4.9.0a1713902092/pulumi_okta/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-23 20:09:06.000000 pulumi_okta-4.9.0a1713902092/pulumi_okta/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 20:09:06.000000 pulumi_okta-4.9.0a1713902092/pulumi_okta/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    13898 2024-04-23 20:09:06.000000 pulumi_okta-4.9.0a1713902092/pulumi_okta/rate_limiting.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11745 2024-04-23 20:09:06.000000 pulumi_okta-4.9.0a1713902092/pulumi_okta/resource_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21186 2024-04-23 20:09:06.000000 pulumi_okta-4.9.0a1713902092/pulumi_okta/role_subscription.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21836 2024-04-23 20:09:06.000000 pulumi_okta-4.9.0a1713902092/pulumi_okta/security_notification_emails.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11529 2024-04-23 20:09:06.000000 pulumi_okta-4.9.0a1713902092/pulumi_okta/template_sms.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42952 2024-04-23 20:09:06.000000 pulumi_okta-4.9.0a1713902092/pulumi_okta/theme.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14854 2024-04-23 20:09:06.000000 pulumi_okta-4.9.0a1713902092/pulumi_okta/threat_insight_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 20:09:12.954008 pulumi_okta-4.9.0a1713902092/pulumi_okta/trustedorigin/
+-rw-r--r--   0 runner    (1001) docker     (127)      291 2024-04-23 20:09:06.000000 pulumi_okta-4.9.0a1713902092/pulumi_okta/trustedorigin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12562 2024-04-23 20:09:06.000000 pulumi_okta-4.9.0a1713902092/pulumi_okta/trustedorigin/origin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 20:09:12.958008 pulumi_okta-4.9.0a1713902092/pulumi_okta/user/
+-rw-r--r--   0 runner    (1001) docker     (127)      484 2024-04-23 20:09:06.000000 pulumi_okta-4.9.0a1713902092/pulumi_okta/user/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9196 2024-04-23 20:09:06.000000 pulumi_okta-4.9.0a1713902092/pulumi_okta/user/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25124 2024-04-23 20:09:06.000000 pulumi_okta-4.9.0a1713902092/pulumi_okta/user/get_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3535 2024-04-23 20:09:06.000000 pulumi_okta-4.9.0a1713902092/pulumi_okta/user/get_user_profile_mapping_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3825 2024-04-23 20:09:06.000000 pulumi_okta-4.9.0a1713902092/pulumi_okta/user/get_user_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9033 2024-04-23 20:09:06.000000 pulumi_okta-4.9.0a1713902092/pulumi_okta/user/get_users.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21707 2024-04-23 20:09:06.000000 pulumi_okta-4.9.0a1713902092/pulumi_okta/user/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    99895 2024-04-23 20:09:06.000000 pulumi_okta-4.9.0a1713902092/pulumi_okta/user/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9967 2024-04-23 20:09:06.000000 pulumi_okta-4.9.0a1713902092/pulumi_okta/user/user_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13653 2024-04-23 20:09:06.000000 pulumi_okta-4.9.0a1713902092/pulumi_okta/user_admin_roles.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22897 2024-04-23 20:09:06.000000 pulumi_okta-4.9.0a1713902092/pulumi_okta/user_base_schema_property.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13954 2024-04-23 20:09:06.000000 pulumi_okta-4.9.0a1713902092/pulumi_okta/user_factor_question.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8844 2024-04-23 20:09:06.000000 pulumi_okta-4.9.0a1713902092/pulumi_okta/user_group_memberships.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52236 2024-04-23 20:09:06.000000 pulumi_okta-4.9.0a1713902092/pulumi_okta/user_schema_property.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 20:09:12.958008 pulumi_okta-4.9.0a1713902092/pulumi_okta.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3351 2024-04-23 20:09:12.000000 pulumi_okta-4.9.0a1713902092/pulumi_okta.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6157 2024-04-23 20:09:12.000000 pulumi_okta-4.9.0a1713902092/pulumi_okta.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 20:09:12.000000 pulumi_okta-4.9.0a1713902092/pulumi_okta.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-23 20:09:12.000000 pulumi_okta-4.9.0a1713902092/pulumi_okta.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-23 20:09:12.000000 pulumi_okta-4.9.0a1713902092/pulumi_okta.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-04-23 20:09:06.000000 pulumi_okta-4.9.0a1713902092/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 20:09:12.958008 pulumi_okta-4.9.0a1713902092/setup.cfg
```

### Comparing `pulumi_okta-4.9.0a1713462165/PKG-INFO` & `pulumi_okta-4.9.0a1713902092/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_okta
-Version: 4.9.0a1713462165
+Version: 4.9.0a1713902092
 Summary: A Pulumi package for creating and managing okta resources.
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.io
 Project-URL: Repository, https://github.com/pulumi/pulumi-okta
 Keywords: pulumi,okta
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_okta-4.9.0a1713462165/README.md` & `pulumi_okta-4.9.0a1713902092/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713462165/pulumi_okta/__init__.py` & `pulumi_okta-4.9.0a1713902092/pulumi_okta/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713462165/pulumi_okta/_inputs.py` & `pulumi_okta-4.9.0a1713902092/pulumi_okta/_inputs.py`

 * *Files 1% similar despite different names*

```diff
@@ -85,15 +85,15 @@
     def __init__(__self__, *,
                  os_expression: Optional[pulumi.Input[str]] = None,
                  os_type: Optional[pulumi.Input[str]] = None,
                  type: Optional[pulumi.Input[str]] = None):
         """
         :param pulumi.Input[str] os_expression: Only available and required when using `os_type = "OTHER"`
         :param pulumi.Input[str] os_type: One of: `"ANY"`, `"IOS"`, `"WINDOWS"`, `"ANDROID"`, `"OTHER"`, `"OSX"`, `"MACOS"`, `"CHROMEOS"`
-        :param pulumi.Input[str] type: The Verification Method type. It can be set to `"ASSURANCE"`. Default is `"ASSURANCE"`.
+        :param pulumi.Input[str] type: One of: `"ANY"`, `"MOBILE"`, `"DESKTOP"`
         """
         if os_expression is not None:
             pulumi.set(__self__, "os_expression", os_expression)
         if os_type is not None:
             pulumi.set(__self__, "os_type", os_type)
         if type is not None:
             pulumi.set(__self__, "type", type)
@@ -122,15 +122,15 @@
     def os_type(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "os_type", value)
 
     @property
     @pulumi.getter
     def type(self) -> Optional[pulumi.Input[str]]:
         """
-        The Verification Method type. It can be set to `"ASSURANCE"`. Default is `"ASSURANCE"`.
+        One of: `"ANY"`, `"MOBILE"`, `"DESKTOP"`
         """
         return pulumi.get(self, "type")
 
     @type.setter
     def type(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "type", value)
 
@@ -174,25 +174,25 @@
 
 @pulumi.input_type
 class AppUserSchemaPropertyOneOfArgs:
     def __init__(__self__, *,
                  const: pulumi.Input[str],
                  title: pulumi.Input[str]):
         """
-        :param pulumi.Input[str] const: value mapping to member of `array_enum`.
+        :param pulumi.Input[str] const: value mapping to member of `enum`.
         :param pulumi.Input[str] title: display name for the enum value.
         """
         pulumi.set(__self__, "const", const)
         pulumi.set(__self__, "title", title)
 
     @property
     @pulumi.getter
     def const(self) -> pulumi.Input[str]:
         """
-        value mapping to member of `array_enum`.
+        value mapping to member of `enum`.
         """
         return pulumi.get(self, "const")
 
     @const.setter
     def const(self, value: pulumi.Input[str]):
         pulumi.set(self, "const", value)
 
@@ -336,41 +336,31 @@
 
 
 @pulumi.input_type
 class EventHookHeaderArgs:
     def __init__(__self__, *,
                  key: Optional[pulumi.Input[str]] = None,
                  value: Optional[pulumi.Input[str]] = None):
-        """
-        :param pulumi.Input[str] key: Key to use for authentication, usually the header name, for example `"Authorization"`.
-        :param pulumi.Input[str] value: Authentication secret.
-        """
         if key is not None:
             pulumi.set(__self__, "key", key)
         if value is not None:
             pulumi.set(__self__, "value", value)
 
     @property
     @pulumi.getter
     def key(self) -> Optional[pulumi.Input[str]]:
-        """
-        Key to use for authentication, usually the header name, for example `"Authorization"`.
-        """
         return pulumi.get(self, "key")
 
     @key.setter
     def key(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "key", value)
 
     @property
     @pulumi.getter
     def value(self) -> Optional[pulumi.Input[str]]:
-        """
-        Authentication secret.
-        """
         return pulumi.get(self, "value")
 
     @value.setter
     def value(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "value", value)
```

### Comparing `pulumi_okta-4.9.0a1713462165/pulumi_okta/_utilities.py` & `pulumi_okta-4.9.0a1713902092/pulumi_okta/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713462165/pulumi_okta/admin_role_custom.py` & `pulumi_okta-4.9.0a1713902092/pulumi_okta/admin_role_custom.py`

 * *Files 2% similar despite different names*

```diff
@@ -261,25 +261,23 @@
         """
         These operations allow the creation and manipulation of custom roles as custom collections of permissions.
 
         > **NOTE:** This an `Early Access` feature.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_okta as okta
 
         example = okta.AdminRoleCustom("example",
             label="AppAssignmentManager",
             description="This role allows app assignment management",
             permissions=["okta.apps.assignment.manage"])
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Okta Custom Admin Role can be imported via the Okta ID.
 
         ```sh
         $ pulumi import okta:index/adminRoleCustom:AdminRoleCustom example &#60;custom role id&#62;
@@ -332,25 +330,23 @@
         """
         These operations allow the creation and manipulation of custom roles as custom collections of permissions.
 
         > **NOTE:** This an `Early Access` feature.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_okta as okta
 
         example = okta.AdminRoleCustom("example",
             label="AppAssignmentManager",
             description="This role allows app assignment management",
             permissions=["okta.apps.assignment.manage"])
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Okta Custom Admin Role can be imported via the Okta ID.
 
         ```sh
         $ pulumi import okta:index/adminRoleCustom:AdminRoleCustom example &#60;custom role id&#62;
```

### Comparing `pulumi_okta-4.9.0a1713462165/pulumi_okta/admin_role_custom_assignments.py` & `pulumi_okta-4.9.0a1713902092/pulumi_okta/admin_role_custom_assignments.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713462165/pulumi_okta/admin_role_targets.py` & `pulumi_okta-4.9.0a1713902092/pulumi_okta/admin_role_targets.py`

 * *Files 3% similar despite different names*

```diff
@@ -183,28 +183,26 @@
         Manages targets for administrator roles.
 
         This resource allows you to define permissions for admin roles into a smaller subset of Groups or Apps within your org.
         You can define admin roles to target Groups, Applications, and Application Instances.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_okta as okta
 
         example = okta.AdminRoleTargets("example",
             user_id="<user_id>",
             role_type="APP_ADMIN",
             apps=[
                 "oidc_client.<app_id>",
                 "facebook",
             ])
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Okta Admin Role Targets can be imported via the Okta ID.
 
         ```sh
         $ pulumi import okta:index/adminRoleTargets:AdminRoleTargets example &#60;user id&#62;/&#60;role type&#62;
@@ -227,28 +225,26 @@
         Manages targets for administrator roles.
 
         This resource allows you to define permissions for admin roles into a smaller subset of Groups or Apps within your org.
         You can define admin roles to target Groups, Applications, and Application Instances.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_okta as okta
 
         example = okta.AdminRoleTargets("example",
             user_id="<user_id>",
             role_type="APP_ADMIN",
             apps=[
                 "oidc_client.<app_id>",
                 "facebook",
             ])
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Okta Admin Role Targets can be imported via the Okta ID.
 
         ```sh
         $ pulumi import okta:index/adminRoleTargets:AdminRoleTargets example &#60;user id&#62;/&#60;role type&#62;
```

### Comparing `pulumi_okta-4.9.0a1713462165/pulumi_okta/app/__init__.py` & `pulumi_okta-4.9.0a1713902092/pulumi_okta/app/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713462165/pulumi_okta/app/_inputs.py` & `pulumi_okta-4.9.0a1713902092/pulumi_okta/app/_inputs.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,19 +22,18 @@
                  name: pulumi.Input[str],
                  type: pulumi.Input[str],
                  value: pulumi.Input[str],
                  filter_type: Optional[pulumi.Input[str]] = None,
                  issuer_mode: Optional[pulumi.Input[str]] = None):
         """
         :param pulumi.Input[str] name: Name of the claim that will be used in the token.
-        :param pulumi.Input[str] type: The type of OAuth application. Valid values: `"web"`, `"native"`, `"browser"`, `"service"`. For SPA apps use `browser`.
+        :param pulumi.Input[str] type: Groups claim type. Valid values: `"FILTER"`, `"EXPRESSION"`.
         :param pulumi.Input[str] value: Value of the claim. Can be an Okta Expression Language statement that evaluates at the time the token is minted.
         :param pulumi.Input[str] filter_type: Groups claim filter. Can only be set if type is `"FILTER"`. Valid values: `"EQUALS"`, `"STARTS_WITH"`, `"CONTAINS"`, `"REGEX"`.
-        :param pulumi.Input[str] issuer_mode: Indicates whether the Okta Authorization Server uses the original Okta org domain URL or a custom domain URL as the issuer of ID token for this client.
-               Valid values: `"CUSTOM_URL"`,`"ORG_URL"` or `"DYNAMIC"`. Default is `"ORG_URL"`.
+        :param pulumi.Input[str] issuer_mode: Issuer Mode is inherited from the Issuer Mode on the OAuth app itself.
         """
         pulumi.set(__self__, "name", name)
         pulumi.set(__self__, "type", type)
         pulumi.set(__self__, "value", value)
         if filter_type is not None:
             pulumi.set(__self__, "filter_type", filter_type)
         if issuer_mode is not None:
@@ -52,15 +51,15 @@
     def name(self, value: pulumi.Input[str]):
         pulumi.set(self, "name", value)
 
     @property
     @pulumi.getter
     def type(self) -> pulumi.Input[str]:
         """
-        The type of OAuth application. Valid values: `"web"`, `"native"`, `"browser"`, `"service"`. For SPA apps use `browser`.
+        Groups claim type. Valid values: `"FILTER"`, `"EXPRESSION"`.
         """
         return pulumi.get(self, "type")
 
     @type.setter
     def type(self, value: pulumi.Input[str]):
         pulumi.set(self, "type", value)
 
@@ -88,16 +87,15 @@
     def filter_type(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "filter_type", value)
 
     @property
     @pulumi.getter(name="issuerMode")
     def issuer_mode(self) -> Optional[pulumi.Input[str]]:
         """
-        Indicates whether the Okta Authorization Server uses the original Okta org domain URL or a custom domain URL as the issuer of ID token for this client.
-        Valid values: `"CUSTOM_URL"`,`"ORG_URL"` or `"DYNAMIC"`. Default is `"ORG_URL"`.
+        Issuer Mode is inherited from the Issuer Mode on the OAuth app itself.
         """
         return pulumi.get(self, "issuer_mode")
 
     @issuer_mode.setter
     def issuer_mode(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "issuer_mode", value)
```

### Comparing `pulumi_okta-4.9.0a1713462165/pulumi_okta/app/access_policy_assignment.py` & `pulumi_okta-4.9.0a1713902092/pulumi_okta/app/access_policy_assignment.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713462165/pulumi_okta/app/auto_login.py` & `pulumi_okta-4.9.0a1713902092/pulumi_okta/app/auto_login.py`

 * *Files 0% similar despite different names*

```diff
@@ -877,45 +877,41 @@
 
         > During an apply if there is change in `status` the app will first be
         activated or deactivated in accordance with the `status` change. Then, all
         other arguments that changed will be applied.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_okta as okta
 
         example = okta.app.AutoLogin("example",
             label="Example App",
             sign_on_url="https://example.com/login.html",
             sign_on_redirect_url="https://example.com",
             reveal_password=True,
             credentials_scheme="EDIT_USERNAME_AND_PASSWORD")
         ```
-        <!--End PulumiCodeChooser -->
 
         ### Pre-configured application
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_okta as okta
 
         example = okta.app.AutoLogin("example",
             label="Google Example App",
             status="ACTIVE",
             preconfigured_app="google",
             app_settings_json=\"\"\"{
             "domain": "okta",
             "afwOnly": false
         }
         \"\"\")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Okta Auto Login App can be imported via the Okta ID.
 
         ```sh
         $ pulumi import okta:app/autoLogin:AutoLogin example &#60;app id&#62;
@@ -959,45 +955,41 @@
 
         > During an apply if there is change in `status` the app will first be
         activated or deactivated in accordance with the `status` change. Then, all
         other arguments that changed will be applied.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_okta as okta
 
         example = okta.app.AutoLogin("example",
             label="Example App",
             sign_on_url="https://example.com/login.html",
             sign_on_redirect_url="https://example.com",
             reveal_password=True,
             credentials_scheme="EDIT_USERNAME_AND_PASSWORD")
         ```
-        <!--End PulumiCodeChooser -->
 
         ### Pre-configured application
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_okta as okta
 
         example = okta.app.AutoLogin("example",
             label="Google Example App",
             status="ACTIVE",
             preconfigured_app="google",
             app_settings_json=\"\"\"{
             "domain": "okta",
             "afwOnly": false
         }
         \"\"\")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Okta Auto Login App can be imported via the Okta ID.
 
         ```sh
         $ pulumi import okta:app/autoLogin:AutoLogin example &#60;app id&#62;
```

### Comparing `pulumi_okta-4.9.0a1713462165/pulumi_okta/app/basic_auth.py` & `pulumi_okta-4.9.0a1713902092/pulumi_okta/app/basic_auth.py`

 * *Files 1% similar despite different names*

```diff
@@ -545,25 +545,23 @@
 
         > During an apply if there is change in `status` the app will first be
         activated or deactivated in accordance with the `status` change. Then, all
         other arguments that changed will be applied.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_okta as okta
 
         example = okta.app.BasicAuth("example",
             label="Example",
             url="https://example.com/login.html",
             auth_url="https://example.com/auth.html")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         A Basic Auth App can be imported via the Okta ID.
 
         ```sh
         $ pulumi import okta:app/basicAuth:BasicAuth example &#60;app id&#62;
@@ -597,25 +595,23 @@
 
         > During an apply if there is change in `status` the app will first be
         activated or deactivated in accordance with the `status` change. Then, all
         other arguments that changed will be applied.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_okta as okta
 
         example = okta.app.BasicAuth("example",
             label="Example",
             url="https://example.com/login.html",
             auth_url="https://example.com/auth.html")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         A Basic Auth App can be imported via the Okta ID.
 
         ```sh
         $ pulumi import okta:app/basicAuth:BasicAuth example &#60;app id&#62;
```

### Comparing `pulumi_okta-4.9.0a1713462165/pulumi_okta/app/bookmark.py` & `pulumi_okta-4.9.0a1713902092/pulumi_okta/app/bookmark.py`

 * *Files 0% similar despite different names*

```diff
@@ -579,24 +579,22 @@
 
         > During an apply if there is change in `status` the app will first be
         activated or deactivated in accordance with the `status` change. Then, all
         other arguments that changed will be applied.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_okta as okta
 
         example = okta.app.Bookmark("example",
             label="Example",
             url="https://example.com")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         A Bookmark App can be imported via the Okta ID.
 
         ```sh
         $ pulumi import okta:app/bookmark:Bookmark example &#60;app id&#62;
@@ -631,24 +629,22 @@
 
         > During an apply if there is change in `status` the app will first be
         activated or deactivated in accordance with the `status` change. Then, all
         other arguments that changed will be applied.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_okta as okta
 
         example = okta.app.Bookmark("example",
             label="Example",
             url="https://example.com")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         A Bookmark App can be imported via the Okta ID.
 
         ```sh
         $ pulumi import okta:app/bookmark:Bookmark example &#60;app id&#62;
```

### Comparing `pulumi_okta-4.9.0a1713462165/pulumi_okta/app/get_app.py` & `pulumi_okta-4.9.0a1713902092/pulumi_okta/app/get_app.py`

 * *Files 2% similar despite different names*

```diff
@@ -166,22 +166,20 @@
             skip_users: Optional[bool] = None,
             opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetAppResult:
     """
     Use this data source to retrieve an application from Okta.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_okta as okta
 
     example = okta.app.get_app(label="Example App")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param bool active_only: tells the provider to query for only `ACTIVE` applications.
     :param str id: `id` of application to retrieve, conflicts with `label` and `label_prefix`.
     :param str label: The label of the app to retrieve, conflicts with `label_prefix` and `id`. Label uses
            the `?q=<label>` query parameter exposed by Okta's API. It should be noted that at this time the API searches both `name`
            and `label` with a [starts with query](https://developer.okta.com/docs/reference/api/apps/#list-applications) which
@@ -223,22 +221,20 @@
                    skip_users: Optional[pulumi.Input[Optional[bool]]] = None,
                    opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetAppResult]:
     """
     Use this data source to retrieve an application from Okta.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_okta as okta
 
     example = okta.app.get_app(label="Example App")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param bool active_only: tells the provider to query for only `ACTIVE` applications.
     :param str id: `id` of application to retrieve, conflicts with `label` and `label_prefix`.
     :param str label: The label of the app to retrieve, conflicts with `label_prefix` and `id`. Label uses
            the `?q=<label>` query parameter exposed by Okta's API. It should be noted that at this time the API searches both `name`
            and `label` with a [starts with query](https://developer.okta.com/docs/reference/api/apps/#list-applications) which
```

### Comparing `pulumi_okta-4.9.0a1713462165/pulumi_okta/app/get_metadata_saml.py` & `pulumi_okta-4.9.0a1713902092/pulumi_okta/app/get_metadata_saml.py`

 * *Files 2% similar despite different names*

```diff
@@ -138,23 +138,21 @@
                       key_id: Optional[str] = None,
                       opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetMetadataSamlResult:
     """
     Use this data source to retrieve the metadata for SAML application from Okta.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_okta as okta
 
     example = okta.app.get_metadata_saml(app_id="<app id>",
         key_id="<cert key id>")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str app_id: The application ID.
     :param str key_id: Certificate Key ID.
     """
     __args__ = dict()
     __args__['appId'] = app_id
@@ -179,22 +177,20 @@
                              key_id: Optional[pulumi.Input[Optional[str]]] = None,
                              opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetMetadataSamlResult]:
     """
     Use this data source to retrieve the metadata for SAML application from Okta.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_okta as okta
 
     example = okta.app.get_metadata_saml(app_id="<app id>",
         key_id="<cert key id>")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str app_id: The application ID.
     :param str key_id: Certificate Key ID.
     """
     ...
```

### Comparing `pulumi_okta-4.9.0a1713462165/pulumi_okta/app/get_oauth.py` & `pulumi_okta-4.9.0a1713902092/pulumi_okta/app/get_oauth.py`

 * *Files 1% similar despite different names*

```diff
@@ -343,22 +343,20 @@
               skip_users: Optional[bool] = None,
               opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetOauthResult:
     """
     Use this data source to retrieve an OIDC application from Okta.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_okta as okta
 
     test = okta.app.get_oauth(label="Example App")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param bool active_only: tells the provider to query for only `ACTIVE` applications.
     :param str id: `id` of application to retrieve, conflicts with `label` and `label_prefix`.
     :param str label: The label of the app to retrieve, conflicts with
            `label_prefix` and `id`. Label uses the `?q=<label>` query parameter exposed by
            Okta's List Apps API. The API will search both `name` and `label` using that
@@ -417,22 +415,20 @@
                      skip_users: Optional[pulumi.Input[Optional[bool]]] = None,
                      opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetOauthResult]:
     """
     Use this data source to retrieve an OIDC application from Okta.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_okta as okta
 
     test = okta.app.get_oauth(label="Example App")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param bool active_only: tells the provider to query for only `ACTIVE` applications.
     :param str id: `id` of application to retrieve, conflicts with `label` and `label_prefix`.
     :param str label: The label of the app to retrieve, conflicts with
            `label_prefix` and `id`. Label uses the `?q=<label>` query parameter exposed by
            Okta's List Apps API. The API will search both `name` and `label` using that
```

### Comparing `pulumi_okta-4.9.0a1713462165/pulumi_okta/app/get_saml.py` & `pulumi_okta-4.9.0a1713902092/pulumi_okta/app/get_saml.py`

 * *Files 1% similar despite different names*

```diff
@@ -603,22 +603,20 @@
              skip_users: Optional[bool] = None,
              opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetSamlResult:
     """
     Use this data source to retrieve an SAML application from Okta.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_okta as okta
 
     example = okta.app.get_saml(label="Example App")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param bool active_only: tells the provider to query for only `ACTIVE` applications.
     :param str id: `id` of application to retrieve, conflicts with `label` and `label_prefix`.
     :param str label: The label of the app to retrieve, conflicts with `label_prefix` and `id`. Label uses
            the `?q=<label>` query parameter exposed by Okta's API. It should be noted that at this time this searches both `name`
            and `label`. This is used to avoid paginating through all applications.
@@ -697,22 +695,20 @@
                     skip_users: Optional[pulumi.Input[Optional[bool]]] = None,
                     opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetSamlResult]:
     """
     Use this data source to retrieve an SAML application from Okta.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_okta as okta
 
     example = okta.app.get_saml(label="Example App")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param bool active_only: tells the provider to query for only `ACTIVE` applications.
     :param str id: `id` of application to retrieve, conflicts with `label` and `label_prefix`.
     :param str label: The label of the app to retrieve, conflicts with `label_prefix` and `id`. Label uses
            the `?q=<label>` query parameter exposed by Okta's API. It should be noted that at this time this searches both `name`
            and `label`. This is used to avoid paginating through all applications.
```

### Comparing `pulumi_okta-4.9.0a1713462165/pulumi_okta/app/group_assignment.py` & `pulumi_okta-4.9.0a1713902092/pulumi_okta/app/group_assignment.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713462165/pulumi_okta/app/o_auth.py` & `pulumi_okta-4.9.0a1713902092/pulumi_okta/app/o_auth.py`

 * *Files 1% similar despite different names*

```diff
@@ -902,15 +902,15 @@
         :param pulumi.Input[str] label: The Application's display name.
         :param pulumi.Input[str] login_mode: The type of Idp-Initiated login that the client supports, if any. Valid values: `"DISABLED"`, `"SPEC"`, `"OKTA"`. Default is `"DISABLED"`.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] login_scopes: List of scopes to use for the request. Valid values: `"openid"`, `"profile"`, `"email"`, `"address"`, `"phone"`. Required when `login_mode` is NOT `DISABLED`.
         :param pulumi.Input[str] login_uri: URI that initiates login. Required when `login_mode` is NOT `DISABLED`.
         :param pulumi.Input[str] logo: Local file path to the logo. The file must be in PNG, JPG, or GIF format, and less than 1 MB in size.
         :param pulumi.Input[str] logo_uri: URI that references a logo for the client.
         :param pulumi.Input[str] logo_url: Direct link of application logo.
-        :param pulumi.Input[str] name: Name of the claim that will be used in the token.
+        :param pulumi.Input[str] name: Name assigned to the application by Okta.
         :param pulumi.Input[bool] omit_secret: This tells the provider not manage the `client_secret` value in state. When this is false (the default), it will cause the auto-generated `client_secret` to be persisted in the `client_secret` attribute in state. This also means that every time an update to this app is run, this value is also set on the API. If this changes from false => true, the `client_secret` is dropped from state and the secret at the time of the apply is what remains. If this is ever changes from true => false your app will be recreated, due to the need to regenerate a secret we can store in state.
         :param pulumi.Input[bool] pkce_required: Require Proof Key for Code Exchange (PKCE) for
                additional verification.  If `pkce_required` isn't specified when adding a new
                application, Okta sets it to `true` by default for `"browser"` and `"native"`
                application types.
                See https://developer.okta.com/docs/reference/api/apps/#oauth-credential-object
         :param pulumi.Input[str] policy_uri: URI to web page providing client policy document.
@@ -1417,15 +1417,15 @@
     def logo_url(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "logo_url", value)
 
     @property
     @pulumi.getter
     def name(self) -> Optional[pulumi.Input[str]]:
         """
-        Name of the claim that will be used in the token.
+        Name assigned to the application by Okta.
         """
         return pulumi.get(self, "name")
 
     @name.setter
     def name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "name", value)
 
@@ -1736,33 +1736,30 @@
 
         > During an apply if there is change in `status` the app will first be
         activated or deactivated in accordance with the `status` change. Then, all
         other arguments that changed will be applied.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_okta as okta
 
         example = okta.app.OAuth("example",
             label="example",
             type="web",
             grant_types=["authorization_code"],
             redirect_uris=["https://example.com/"],
             response_types=["code"])
         ```
-        <!--End PulumiCodeChooser -->
 
         ### With JWKS value
 
         See also Advanced PEM secrets and JWKS example.
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_okta as okta
 
         example = okta.app.OAuth("example",
             label="example",
             type="service",
@@ -1780,15 +1777,14 @@
                     kty="EC",
                     kid="SIGNING_KEY_EC",
                     x="K37X78mXJHHldZYMzrwipjKR-YZUS2SMye0KindHp6I",
                     y="8IfvsvXWzbFWOZoVOMwgF5p46mUj3kbOVf9Fk0vVVHo",
                 ),
             ])
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Etc.
 
         ### Resetting client secret
 
         If the client secret needs to be reset run an apply with `omit_secret` set to
         true in the resource. This causes `client_secret` to be set to blank. Remove
@@ -1902,33 +1898,30 @@
 
         > During an apply if there is change in `status` the app will first be
         activated or deactivated in accordance with the `status` change. Then, all
         other arguments that changed will be applied.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_okta as okta
 
         example = okta.app.OAuth("example",
             label="example",
             type="web",
             grant_types=["authorization_code"],
             redirect_uris=["https://example.com/"],
             response_types=["code"])
         ```
-        <!--End PulumiCodeChooser -->
 
         ### With JWKS value
 
         See also Advanced PEM secrets and JWKS example.
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_okta as okta
 
         example = okta.app.OAuth("example",
             label="example",
             type="service",
@@ -1946,15 +1939,14 @@
                     kty="EC",
                     kid="SIGNING_KEY_EC",
                     x="K37X78mXJHHldZYMzrwipjKR-YZUS2SMye0KindHp6I",
                     y="8IfvsvXWzbFWOZoVOMwgF5p46mUj3kbOVf9Fk0vVVHo",
                 ),
             ])
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Etc.
 
         ### Resetting client secret
 
         If the client secret needs to be reset run an apply with `omit_secret` set to
         true in the resource. This causes `client_secret` to be set to blank. Remove
@@ -2206,15 +2198,15 @@
         :param pulumi.Input[str] label: The Application's display name.
         :param pulumi.Input[str] login_mode: The type of Idp-Initiated login that the client supports, if any. Valid values: `"DISABLED"`, `"SPEC"`, `"OKTA"`. Default is `"DISABLED"`.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] login_scopes: List of scopes to use for the request. Valid values: `"openid"`, `"profile"`, `"email"`, `"address"`, `"phone"`. Required when `login_mode` is NOT `DISABLED`.
         :param pulumi.Input[str] login_uri: URI that initiates login. Required when `login_mode` is NOT `DISABLED`.
         :param pulumi.Input[str] logo: Local file path to the logo. The file must be in PNG, JPG, or GIF format, and less than 1 MB in size.
         :param pulumi.Input[str] logo_uri: URI that references a logo for the client.
         :param pulumi.Input[str] logo_url: Direct link of application logo.
-        :param pulumi.Input[str] name: Name of the claim that will be used in the token.
+        :param pulumi.Input[str] name: Name assigned to the application by Okta.
         :param pulumi.Input[bool] omit_secret: This tells the provider not manage the `client_secret` value in state. When this is false (the default), it will cause the auto-generated `client_secret` to be persisted in the `client_secret` attribute in state. This also means that every time an update to this app is run, this value is also set on the API. If this changes from false => true, the `client_secret` is dropped from state and the secret at the time of the apply is what remains. If this is ever changes from true => false your app will be recreated, due to the need to regenerate a secret we can store in state.
         :param pulumi.Input[bool] pkce_required: Require Proof Key for Code Exchange (PKCE) for
                additional verification.  If `pkce_required` isn't specified when adding a new
                application, Okta sets it to `true` by default for `"browser"` and `"native"`
                application types.
                See https://developer.okta.com/docs/reference/api/apps/#oauth-credential-object
         :param pulumi.Input[str] policy_uri: URI to web page providing client policy document.
@@ -2556,15 +2548,15 @@
         """
         return pulumi.get(self, "logo_url")
 
     @property
     @pulumi.getter
     def name(self) -> pulumi.Output[str]:
         """
-        Name of the claim that will be used in the token.
+        Name assigned to the application by Okta.
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter(name="omitSecret")
     def omit_secret(self) -> pulumi.Output[Optional[bool]]:
         """
```

### Comparing `pulumi_okta-4.9.0a1713462165/pulumi_okta/app/o_auth_post_logout_redirect_uri.py` & `pulumi_okta-4.9.0a1713902092/pulumi_okta/app/o_auth_post_logout_redirect_uri.py`

 * *Files 3% similar despite different names*

```diff
@@ -102,15 +102,14 @@
 
         > `app.OAuthPostLogoutRedirectUri` has been marked deprecated and will
         be removed in the v5 release of the provider. Operators should manage the post
         logout redirect URIs for an oauth app directly on that resource.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_okta as okta
 
         test = okta.app.OAuth("test",
             label="testAcc_replace_with_uuid",
             type="web",
@@ -118,15 +117,14 @@
             response_types=["code"],
             redirect_uris=["myapp://callback"],
             post_logout_redirect_uris=["https://www.example.com"])
         test_o_auth_post_logout_redirect_uri = okta.app.OAuthPostLogoutRedirectUri("test",
             app_id=test.id,
             uri="https://www.example.com")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         A post logout redirect URI can be imported via the Okta ID.
 
         ```sh
         $ pulumi import okta:app/oAuthPostLogoutRedirectUri:OAuthPostLogoutRedirectUri example &#60;app id&#62;/&#60;uri&#62;
@@ -148,15 +146,14 @@
 
         > `app.OAuthPostLogoutRedirectUri` has been marked deprecated and will
         be removed in the v5 release of the provider. Operators should manage the post
         logout redirect URIs for an oauth app directly on that resource.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_okta as okta
 
         test = okta.app.OAuth("test",
             label="testAcc_replace_with_uuid",
             type="web",
@@ -164,15 +161,14 @@
             response_types=["code"],
             redirect_uris=["myapp://callback"],
             post_logout_redirect_uris=["https://www.example.com"])
         test_o_auth_post_logout_redirect_uri = okta.app.OAuthPostLogoutRedirectUri("test",
             app_id=test.id,
             uri="https://www.example.com")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         A post logout redirect URI can be imported via the Okta ID.
 
         ```sh
         $ pulumi import okta:app/oAuthPostLogoutRedirectUri:OAuthPostLogoutRedirectUri example &#60;app id&#62;/&#60;uri&#62;
```

### Comparing `pulumi_okta-4.9.0a1713462165/pulumi_okta/app/o_auth_redirect_uri.py` & `pulumi_okta-4.9.0a1713902092/pulumi_okta/app/o_auth_redirect_uri.py`

 * *Files 5% similar despite different names*

```diff
@@ -102,30 +102,28 @@
 
         > `app.OAuthRedirectUri` has been marked deprecated and will be removed
         in the v5 release of the provider. Operators should manage the redirect URIs for
         an oauth app directly on that resource.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_okta as okta
 
         test = okta.app.OAuth("test",
             label="testAcc_replace_with_uuid",
             type="web",
             grant_types=["authorization_code"],
             response_types=["code"],
             redirect_uris=["myapp://callback"])
         test_o_auth_redirect_uri = okta.app.OAuthRedirectUri("test",
             app_id=test.id,
             uri="http://google.com")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         A redirect URI can be imported via the Okta ID.
 
         ```sh
         $ pulumi import okta:app/oAuthRedirectUri:OAuthRedirectUri example &#60;app id&#62;/&#60;uri&#62;
@@ -147,30 +145,28 @@
 
         > `app.OAuthRedirectUri` has been marked deprecated and will be removed
         in the v5 release of the provider. Operators should manage the redirect URIs for
         an oauth app directly on that resource.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_okta as okta
 
         test = okta.app.OAuth("test",
             label="testAcc_replace_with_uuid",
             type="web",
             grant_types=["authorization_code"],
             response_types=["code"],
             redirect_uris=["myapp://callback"])
         test_o_auth_redirect_uri = okta.app.OAuthRedirectUri("test",
             app_id=test.id,
             uri="http://google.com")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         A redirect URI can be imported via the Okta ID.
 
         ```sh
         $ pulumi import okta:app/oAuthRedirectUri:OAuthRedirectUri example &#60;app id&#62;/&#60;uri&#62;
```

### Comparing `pulumi_okta-4.9.0a1713462165/pulumi_okta/app/oauth_role_assignment.py` & `pulumi_okta-4.9.0a1713902092/pulumi_okta/app/oauth_role_assignment.py`

 * *Files 2% similar despite different names*

```diff
@@ -200,30 +200,28 @@
 
         This resource allows you to assign an Okta admin role to a OAuth service application. This requires the Okta tenant feature flag for this function to be enabled.
 
         ## Example Usage
 
         Standard Role:
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_okta as okta
 
         test = okta.app.OAuth("test",
             label="test",
             type="service",
             response_types=["token"],
             grant_types=["client_credentials"],
             jwks_uri="https://example.com")
         test_oauth_role_assignment = okta.app.OauthRoleAssignment("test",
             client_id=test.client_id,
             type="HELP_DESK_ADMIN")
         ```
-        <!--End PulumiCodeChooser -->
 
         Custom Role:
 
         ## Import
 
         OAuth Role assignment can be imported by passing the Client ID and Role Assignment ID for the specific client role.
 
@@ -249,30 +247,28 @@
 
         This resource allows you to assign an Okta admin role to a OAuth service application. This requires the Okta tenant feature flag for this function to be enabled.
 
         ## Example Usage
 
         Standard Role:
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_okta as okta
 
         test = okta.app.OAuth("test",
             label="test",
             type="service",
             response_types=["token"],
             grant_types=["client_credentials"],
             jwks_uri="https://example.com")
         test_oauth_role_assignment = okta.app.OauthRoleAssignment("test",
             client_id=test.client_id,
             type="HELP_DESK_ADMIN")
         ```
-        <!--End PulumiCodeChooser -->
 
         Custom Role:
 
         ## Import
 
         OAuth Role assignment can be imported by passing the Client ID and Role Assignment ID for the specific client role.
```

### Comparing `pulumi_okta-4.9.0a1713462165/pulumi_okta/app/outputs.py` & `pulumi_okta-4.9.0a1713902092/pulumi_okta/app/outputs.py`

 * *Files 8% similar despite different names*

```diff
@@ -42,19 +42,18 @@
                  name: str,
                  type: str,
                  value: str,
                  filter_type: Optional[str] = None,
                  issuer_mode: Optional[str] = None):
         """
         :param str name: Name of the claim that will be used in the token.
-        :param str type: The type of OAuth application. Valid values: `"web"`, `"native"`, `"browser"`, `"service"`. For SPA apps use `browser`.
+        :param str type: Groups claim type. Valid values: `"FILTER"`, `"EXPRESSION"`.
         :param str value: Value of the claim. Can be an Okta Expression Language statement that evaluates at the time the token is minted.
         :param str filter_type: Groups claim filter. Can only be set if type is `"FILTER"`. Valid values: `"EQUALS"`, `"STARTS_WITH"`, `"CONTAINS"`, `"REGEX"`.
-        :param str issuer_mode: Indicates whether the Okta Authorization Server uses the original Okta org domain URL or a custom domain URL as the issuer of ID token for this client.
-               Valid values: `"CUSTOM_URL"`,`"ORG_URL"` or `"DYNAMIC"`. Default is `"ORG_URL"`.
+        :param str issuer_mode: Issuer Mode is inherited from the Issuer Mode on the OAuth app itself.
         """
         pulumi.set(__self__, "name", name)
         pulumi.set(__self__, "type", type)
         pulumi.set(__self__, "value", value)
         if filter_type is not None:
             pulumi.set(__self__, "filter_type", filter_type)
         if issuer_mode is not None:
@@ -68,15 +67,15 @@
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter
     def type(self) -> str:
         """
-        The type of OAuth application. Valid values: `"web"`, `"native"`, `"browser"`, `"service"`. For SPA apps use `browser`.
+        Groups claim type. Valid values: `"FILTER"`, `"EXPRESSION"`.
         """
         return pulumi.get(self, "type")
 
     @property
     @pulumi.getter
     def value(self) -> str:
         """
@@ -92,16 +91,15 @@
         """
         return pulumi.get(self, "filter_type")
 
     @property
     @pulumi.getter(name="issuerMode")
     def issuer_mode(self) -> Optional[str]:
         """
-        Indicates whether the Okta Authorization Server uses the original Okta org domain URL or a custom domain URL as the issuer of ID token for this client.
-        Valid values: `"CUSTOM_URL"`,`"ORG_URL"` or `"DYNAMIC"`. Default is `"ORG_URL"`.
+        Issuer Mode is inherited from the Issuer Mode on the OAuth app itself.
         """
         return pulumi.get(self, "issuer_mode")
 
 
 @pulumi.output_type
 class OAuthJwk(dict):
     def __init__(__self__, *,
```

### Comparing `pulumi_okta-4.9.0a1713462165/pulumi_okta/app/saml.py` & `pulumi_okta-4.9.0a1713902092/pulumi_okta/app/saml.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,21 +70,21 @@
         :param pulumi.Input[bool] accessibility_self_service: Enable self-service. Default is: `false`.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] acs_endpoints: An array of ACS endpoints. You can configure a maximum of 100 endpoints.
         :param pulumi.Input[str] admin_note: Application notes for admins.
         :param pulumi.Input[str] app_links_json: Displays specific appLinks for the app. The value for each application link should be boolean.
         :param pulumi.Input[str] app_settings_json: Application settings in JSON format.
         :param pulumi.Input[bool] assertion_signed: Determines whether the SAML assertion is digitally signed.
         :param pulumi.Input[Sequence[pulumi.Input['SamlAttributeStatementArgs']]] attribute_statements: List of SAML Attribute statements.
-        :param pulumi.Input[str] audience: Audience Restriction
+        :param pulumi.Input[str] audience: Audience restriction.
         :param pulumi.Input[str] authentication_policy: The ID of the associated `app_signon_policy`. If this property is removed from the application the `default` sign-on-policy will be associated with this application.
-        :param pulumi.Input[str] authn_context_class_ref: Identifies the SAML authentication context class for the assertion’s authentication statement
+        :param pulumi.Input[str] authn_context_class_ref: Identifies the SAML authentication context class for the assertion’s authentication statement.
         :param pulumi.Input[bool] auto_submit_toolbar: Display auto submit toolbar. Default is: `false`
         :param pulumi.Input[str] default_relay_state: Identifies a specific application resource in an IDP initiated SSO scenario.
-        :param pulumi.Input[str] destination: Identifies the location where the SAML response is intended to be sent inside of the SAML assertion
-        :param pulumi.Input[str] digest_algorithm: Determines the digest algorithm used to digitally sign the SAML assertion and response
+        :param pulumi.Input[str] destination: Identifies the location where the SAML response is intended to be sent inside the SAML assertion.
+        :param pulumi.Input[str] digest_algorithm: Determines the digest algorithm used to digitally sign the SAML assertion and response.
         :param pulumi.Input[str] enduser_note: Application notes for end users.
         :param pulumi.Input[bool] hide_ios: Do not display application icon on mobile app. Default is: `false`
         :param pulumi.Input[bool] hide_web: Do not display application icon to users. Default is: `false`
         :param pulumi.Input[bool] honor_force_authn: Prompt user to re-authenticate if SP asks for it. Default is: `false`
         :param pulumi.Input[str] idp_issuer: SAML issuer ID.
         :param pulumi.Input[bool] implicit_assignment: _Early Access Property_. Enables [Federation Broker Mode](https://help.okta.com/en/prod/Content/Topics/Apps/apps-fbm-enable.htm).
         :param pulumi.Input[str] inline_hook_id: Saml Inline Hook associated with the application.
@@ -323,15 +323,15 @@
     def attribute_statements(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['SamlAttributeStatementArgs']]]]):
         pulumi.set(self, "attribute_statements", value)
 
     @property
     @pulumi.getter
     def audience(self) -> Optional[pulumi.Input[str]]:
         """
-        Audience Restriction
+        Audience restriction.
         """
         return pulumi.get(self, "audience")
 
     @audience.setter
     def audience(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "audience", value)
 
@@ -347,15 +347,15 @@
     def authentication_policy(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "authentication_policy", value)
 
     @property
     @pulumi.getter(name="authnContextClassRef")
     def authn_context_class_ref(self) -> Optional[pulumi.Input[str]]:
         """
-        Identifies the SAML authentication context class for the assertion’s authentication statement
+        Identifies the SAML authentication context class for the assertion’s authentication statement.
         """
         return pulumi.get(self, "authn_context_class_ref")
 
     @authn_context_class_ref.setter
     def authn_context_class_ref(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "authn_context_class_ref", value)
 
@@ -383,27 +383,27 @@
     def default_relay_state(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "default_relay_state", value)
 
     @property
     @pulumi.getter
     def destination(self) -> Optional[pulumi.Input[str]]:
         """
-        Identifies the location where the SAML response is intended to be sent inside of the SAML assertion
+        Identifies the location where the SAML response is intended to be sent inside the SAML assertion.
         """
         return pulumi.get(self, "destination")
 
     @destination.setter
     def destination(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "destination", value)
 
     @property
     @pulumi.getter(name="digestAlgorithm")
     def digest_algorithm(self) -> Optional[pulumi.Input[str]]:
         """
-        Determines the digest algorithm used to digitally sign the SAML assertion and response
+        Determines the digest algorithm used to digitally sign the SAML assertion and response.
         """
         return pulumi.get(self, "digest_algorithm")
 
     @digest_algorithm.setter
     def digest_algorithm(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "digest_algorithm", value)
 
@@ -826,22 +826,22 @@
         :param pulumi.Input[bool] accessibility_self_service: Enable self-service. Default is: `false`.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] acs_endpoints: An array of ACS endpoints. You can configure a maximum of 100 endpoints.
         :param pulumi.Input[str] admin_note: Application notes for admins.
         :param pulumi.Input[str] app_links_json: Displays specific appLinks for the app. The value for each application link should be boolean.
         :param pulumi.Input[str] app_settings_json: Application settings in JSON format.
         :param pulumi.Input[bool] assertion_signed: Determines whether the SAML assertion is digitally signed.
         :param pulumi.Input[Sequence[pulumi.Input['SamlAttributeStatementArgs']]] attribute_statements: List of SAML Attribute statements.
-        :param pulumi.Input[str] audience: Audience Restriction
+        :param pulumi.Input[str] audience: Audience restriction.
         :param pulumi.Input[str] authentication_policy: The ID of the associated `app_signon_policy`. If this property is removed from the application the `default` sign-on-policy will be associated with this application.
-        :param pulumi.Input[str] authn_context_class_ref: Identifies the SAML authentication context class for the assertion’s authentication statement
+        :param pulumi.Input[str] authn_context_class_ref: Identifies the SAML authentication context class for the assertion’s authentication statement.
         :param pulumi.Input[bool] auto_submit_toolbar: Display auto submit toolbar. Default is: `false`
         :param pulumi.Input[str] certificate: The raw signing certificate.
         :param pulumi.Input[str] default_relay_state: Identifies a specific application resource in an IDP initiated SSO scenario.
-        :param pulumi.Input[str] destination: Identifies the location where the SAML response is intended to be sent inside of the SAML assertion
-        :param pulumi.Input[str] digest_algorithm: Determines the digest algorithm used to digitally sign the SAML assertion and response
+        :param pulumi.Input[str] destination: Identifies the location where the SAML response is intended to be sent inside the SAML assertion.
+        :param pulumi.Input[str] digest_algorithm: Determines the digest algorithm used to digitally sign the SAML assertion and response.
         :param pulumi.Input[str] embed_url: Url that can be used to embed this application into another portal.
         :param pulumi.Input[str] enduser_note: Application notes for end users.
         :param pulumi.Input[str] entity_key: Entity ID, the ID portion of the `entity_url`.
         :param pulumi.Input[str] entity_url: Entity URL for instance [http://www.okta.com/exk1fcia6d6EMsf331d8](http://www.okta.com/exk1fcia6d6EMsf331d8).
         :param pulumi.Input[Sequence[pulumi.Input[str]]] features: features enabled. Notice: you can't currently configure provisioning features via the API.
         :param pulumi.Input[bool] hide_ios: Do not display application icon on mobile app. Default is: `false`
         :param pulumi.Input[bool] hide_web: Do not display application icon to users. Default is: `false`
@@ -856,15 +856,15 @@
         :param pulumi.Input[int] key_years_valid: Number of years the certificate is valid (2 - 10 years).
         :param pulumi.Input[Sequence[pulumi.Input['SamlKeyArgs']]] keys: An array of all key credentials for the application. Format of each entry is as follows:
         :param pulumi.Input[str] label: label of application.
         :param pulumi.Input[str] logo: Local file path to the logo. The file must be in PNG, JPG, or GIF format, and less than 1 MB in size.
         :param pulumi.Input[str] logo_url: Direct link of application logo.
         :param pulumi.Input[str] metadata: The raw SAML metadata in XML.
         :param pulumi.Input[str] metadata_url: SAML xml metadata URL.
-        :param pulumi.Input[str] name: The name of the attribute statement.
+        :param pulumi.Input[str] name: Name assigned to the application by Okta.
         :param pulumi.Input[str] preconfigured_app: name of application from the Okta Integration Network, if not included a custom app will be created.  If not provided the following arguments are required:
         :param pulumi.Input[str] recipient: The location where the app may present the SAML assertion.
         :param pulumi.Input[bool] request_compressed: Denotes whether the request is compressed or not.
         :param pulumi.Input[bool] response_signed: Determines whether the SAML auth response message is digitally signed.
         :param pulumi.Input[bool] saml_signed_request_enabled: SAML Signed Request enabled
         :param pulumi.Input[str] saml_version: SAML version for the app's sign-on mode. Valid values are: `"2.0"` or `"1.1"`. Default is `"2.0"`.
         :param pulumi.Input[str] sign_on_mode: Sign-on mode of application.
@@ -1111,15 +1111,15 @@
     def attribute_statements(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['SamlAttributeStatementArgs']]]]):
         pulumi.set(self, "attribute_statements", value)
 
     @property
     @pulumi.getter
     def audience(self) -> Optional[pulumi.Input[str]]:
         """
-        Audience Restriction
+        Audience restriction.
         """
         return pulumi.get(self, "audience")
 
     @audience.setter
     def audience(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "audience", value)
 
@@ -1135,15 +1135,15 @@
     def authentication_policy(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "authentication_policy", value)
 
     @property
     @pulumi.getter(name="authnContextClassRef")
     def authn_context_class_ref(self) -> Optional[pulumi.Input[str]]:
         """
-        Identifies the SAML authentication context class for the assertion’s authentication statement
+        Identifies the SAML authentication context class for the assertion’s authentication statement.
         """
         return pulumi.get(self, "authn_context_class_ref")
 
     @authn_context_class_ref.setter
     def authn_context_class_ref(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "authn_context_class_ref", value)
 
@@ -1183,27 +1183,27 @@
     def default_relay_state(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "default_relay_state", value)
 
     @property
     @pulumi.getter
     def destination(self) -> Optional[pulumi.Input[str]]:
         """
-        Identifies the location where the SAML response is intended to be sent inside of the SAML assertion
+        Identifies the location where the SAML response is intended to be sent inside the SAML assertion.
         """
         return pulumi.get(self, "destination")
 
     @destination.setter
     def destination(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "destination", value)
 
     @property
     @pulumi.getter(name="digestAlgorithm")
     def digest_algorithm(self) -> Optional[pulumi.Input[str]]:
         """
-        Determines the digest algorithm used to digitally sign the SAML assertion and response
+        Determines the digest algorithm used to digitally sign the SAML assertion and response.
         """
         return pulumi.get(self, "digest_algorithm")
 
     @digest_algorithm.setter
     def digest_algorithm(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "digest_algorithm", value)
 
@@ -1471,15 +1471,15 @@
     def metadata_url(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "metadata_url", value)
 
     @property
     @pulumi.getter
     def name(self) -> Optional[pulumi.Input[str]]:
         """
-        The name of the attribute statement.
+        Name assigned to the application by Okta.
         """
         return pulumi.get(self, "name")
 
     @name.setter
     def name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "name", value)
 
@@ -1785,15 +1785,14 @@
 
         > If you receive the error `You do not have permission to access the feature
         you are requesting` contact support and
         request feature flag `ADVANCED_SSO` be applied to your org.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_okta as okta
 
         example = okta.app.Saml("example",
             label="example",
             sso_url="https://example.com",
@@ -1810,19 +1809,17 @@
             attribute_statements=[okta.app.SamlAttributeStatementArgs(
                 type="GROUP",
                 name="groups",
                 filter_type="REGEX",
                 filter_value=".*",
             )])
         ```
-        <!--End PulumiCodeChooser -->
 
         ### With inline hook
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_okta as okta
 
         test = okta.inline.Hook("test",
             name="testAcc_replace_with_uuid",
             status="ACTIVE",
@@ -1857,19 +1854,17 @@
                 type="GROUP",
                 name="groups",
                 filter_type="REGEX",
                 filter_value=".*",
             )],
             opts=pulumi.ResourceOptions(depends_on=[test]))
         ```
-        <!--End PulumiCodeChooser -->
 
         ### Pre-configured app with SAML 1.1 sign-on mode
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_okta as okta
 
         test = okta.app.Saml("test",
             app_settings_json=\"\"\"{
             "groupFilter": "app1.*",
@@ -1879,19 +1874,17 @@
             label="SharePoint (On-Premise)",
             preconfigured_app="sharepoint_onpremise",
             saml_version="1.1",
             status="ACTIVE",
             user_name_template="${source.login}",
             user_name_template_type="BUILT_IN")
         ```
-        <!--End PulumiCodeChooser -->
 
         ### Pre-configured app with SAML 1.1 sign-on mode, `app_settings_json` and `app_links_json`
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_okta as okta
 
         office365 = okta.app.Saml("office365",
             preconfigured_app="office365",
             label="Microsoft Office 365",
@@ -1926,15 +1919,14 @@
               "video": false,
               "word": false,
               "yammer": false,
               "login": true
           }
         \"\"\")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         A SAML App can be imported via the Okta ID.
 
         ```sh
         $ pulumi import okta:app/saml:Saml example &#60;app id&#62;
@@ -1947,21 +1939,21 @@
         :param pulumi.Input[bool] accessibility_self_service: Enable self-service. Default is: `false`.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] acs_endpoints: An array of ACS endpoints. You can configure a maximum of 100 endpoints.
         :param pulumi.Input[str] admin_note: Application notes for admins.
         :param pulumi.Input[str] app_links_json: Displays specific appLinks for the app. The value for each application link should be boolean.
         :param pulumi.Input[str] app_settings_json: Application settings in JSON format.
         :param pulumi.Input[bool] assertion_signed: Determines whether the SAML assertion is digitally signed.
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['SamlAttributeStatementArgs']]]] attribute_statements: List of SAML Attribute statements.
-        :param pulumi.Input[str] audience: Audience Restriction
+        :param pulumi.Input[str] audience: Audience restriction.
         :param pulumi.Input[str] authentication_policy: The ID of the associated `app_signon_policy`. If this property is removed from the application the `default` sign-on-policy will be associated with this application.
-        :param pulumi.Input[str] authn_context_class_ref: Identifies the SAML authentication context class for the assertion’s authentication statement
+        :param pulumi.Input[str] authn_context_class_ref: Identifies the SAML authentication context class for the assertion’s authentication statement.
         :param pulumi.Input[bool] auto_submit_toolbar: Display auto submit toolbar. Default is: `false`
         :param pulumi.Input[str] default_relay_state: Identifies a specific application resource in an IDP initiated SSO scenario.
-        :param pulumi.Input[str] destination: Identifies the location where the SAML response is intended to be sent inside of the SAML assertion
-        :param pulumi.Input[str] digest_algorithm: Determines the digest algorithm used to digitally sign the SAML assertion and response
+        :param pulumi.Input[str] destination: Identifies the location where the SAML response is intended to be sent inside the SAML assertion.
+        :param pulumi.Input[str] digest_algorithm: Determines the digest algorithm used to digitally sign the SAML assertion and response.
         :param pulumi.Input[str] enduser_note: Application notes for end users.
         :param pulumi.Input[bool] hide_ios: Do not display application icon on mobile app. Default is: `false`
         :param pulumi.Input[bool] hide_web: Do not display application icon to users. Default is: `false`
         :param pulumi.Input[bool] honor_force_authn: Prompt user to re-authenticate if SP asks for it. Default is: `false`
         :param pulumi.Input[str] idp_issuer: SAML issuer ID.
         :param pulumi.Input[bool] implicit_assignment: _Early Access Property_. Enables [Federation Broker Mode](https://help.okta.com/en/prod/Content/Topics/Apps/apps-fbm-enable.htm).
         :param pulumi.Input[str] inline_hook_id: Saml Inline Hook associated with the application.
@@ -2004,15 +1996,14 @@
 
         > If you receive the error `You do not have permission to access the feature
         you are requesting` contact support and
         request feature flag `ADVANCED_SSO` be applied to your org.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_okta as okta
 
         example = okta.app.Saml("example",
             label="example",
             sso_url="https://example.com",
@@ -2029,19 +2020,17 @@
             attribute_statements=[okta.app.SamlAttributeStatementArgs(
                 type="GROUP",
                 name="groups",
                 filter_type="REGEX",
                 filter_value=".*",
             )])
         ```
-        <!--End PulumiCodeChooser -->
 
         ### With inline hook
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_okta as okta
 
         test = okta.inline.Hook("test",
             name="testAcc_replace_with_uuid",
             status="ACTIVE",
@@ -2076,19 +2065,17 @@
                 type="GROUP",
                 name="groups",
                 filter_type="REGEX",
                 filter_value=".*",
             )],
             opts=pulumi.ResourceOptions(depends_on=[test]))
         ```
-        <!--End PulumiCodeChooser -->
 
         ### Pre-configured app with SAML 1.1 sign-on mode
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_okta as okta
 
         test = okta.app.Saml("test",
             app_settings_json=\"\"\"{
             "groupFilter": "app1.*",
@@ -2098,19 +2085,17 @@
             label="SharePoint (On-Premise)",
             preconfigured_app="sharepoint_onpremise",
             saml_version="1.1",
             status="ACTIVE",
             user_name_template="${source.login}",
             user_name_template_type="BUILT_IN")
         ```
-        <!--End PulumiCodeChooser -->
 
         ### Pre-configured app with SAML 1.1 sign-on mode, `app_settings_json` and `app_links_json`
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_okta as okta
 
         office365 = okta.app.Saml("office365",
             preconfigured_app="office365",
             label="Microsoft Office 365",
@@ -2145,15 +2130,14 @@
               "video": false,
               "word": false,
               "yammer": false,
               "login": true
           }
         \"\"\")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         A SAML App can be imported via the Okta ID.
 
         ```sh
         $ pulumi import okta:app/saml:Saml example &#60;app id&#62;
@@ -2373,22 +2357,22 @@
         :param pulumi.Input[bool] accessibility_self_service: Enable self-service. Default is: `false`.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] acs_endpoints: An array of ACS endpoints. You can configure a maximum of 100 endpoints.
         :param pulumi.Input[str] admin_note: Application notes for admins.
         :param pulumi.Input[str] app_links_json: Displays specific appLinks for the app. The value for each application link should be boolean.
         :param pulumi.Input[str] app_settings_json: Application settings in JSON format.
         :param pulumi.Input[bool] assertion_signed: Determines whether the SAML assertion is digitally signed.
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['SamlAttributeStatementArgs']]]] attribute_statements: List of SAML Attribute statements.
-        :param pulumi.Input[str] audience: Audience Restriction
+        :param pulumi.Input[str] audience: Audience restriction.
         :param pulumi.Input[str] authentication_policy: The ID of the associated `app_signon_policy`. If this property is removed from the application the `default` sign-on-policy will be associated with this application.
-        :param pulumi.Input[str] authn_context_class_ref: Identifies the SAML authentication context class for the assertion’s authentication statement
+        :param pulumi.Input[str] authn_context_class_ref: Identifies the SAML authentication context class for the assertion’s authentication statement.
         :param pulumi.Input[bool] auto_submit_toolbar: Display auto submit toolbar. Default is: `false`
         :param pulumi.Input[str] certificate: The raw signing certificate.
         :param pulumi.Input[str] default_relay_state: Identifies a specific application resource in an IDP initiated SSO scenario.
-        :param pulumi.Input[str] destination: Identifies the location where the SAML response is intended to be sent inside of the SAML assertion
-        :param pulumi.Input[str] digest_algorithm: Determines the digest algorithm used to digitally sign the SAML assertion and response
+        :param pulumi.Input[str] destination: Identifies the location where the SAML response is intended to be sent inside the SAML assertion.
+        :param pulumi.Input[str] digest_algorithm: Determines the digest algorithm used to digitally sign the SAML assertion and response.
         :param pulumi.Input[str] embed_url: Url that can be used to embed this application into another portal.
         :param pulumi.Input[str] enduser_note: Application notes for end users.
         :param pulumi.Input[str] entity_key: Entity ID, the ID portion of the `entity_url`.
         :param pulumi.Input[str] entity_url: Entity URL for instance [http://www.okta.com/exk1fcia6d6EMsf331d8](http://www.okta.com/exk1fcia6d6EMsf331d8).
         :param pulumi.Input[Sequence[pulumi.Input[str]]] features: features enabled. Notice: you can't currently configure provisioning features via the API.
         :param pulumi.Input[bool] hide_ios: Do not display application icon on mobile app. Default is: `false`
         :param pulumi.Input[bool] hide_web: Do not display application icon to users. Default is: `false`
@@ -2403,15 +2387,15 @@
         :param pulumi.Input[int] key_years_valid: Number of years the certificate is valid (2 - 10 years).
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['SamlKeyArgs']]]] keys: An array of all key credentials for the application. Format of each entry is as follows:
         :param pulumi.Input[str] label: label of application.
         :param pulumi.Input[str] logo: Local file path to the logo. The file must be in PNG, JPG, or GIF format, and less than 1 MB in size.
         :param pulumi.Input[str] logo_url: Direct link of application logo.
         :param pulumi.Input[str] metadata: The raw SAML metadata in XML.
         :param pulumi.Input[str] metadata_url: SAML xml metadata URL.
-        :param pulumi.Input[str] name: The name of the attribute statement.
+        :param pulumi.Input[str] name: Name assigned to the application by Okta.
         :param pulumi.Input[str] preconfigured_app: name of application from the Okta Integration Network, if not included a custom app will be created.  If not provided the following arguments are required:
         :param pulumi.Input[str] recipient: The location where the app may present the SAML assertion.
         :param pulumi.Input[bool] request_compressed: Denotes whether the request is compressed or not.
         :param pulumi.Input[bool] response_signed: Determines whether the SAML auth response message is digitally signed.
         :param pulumi.Input[bool] saml_signed_request_enabled: SAML Signed Request enabled
         :param pulumi.Input[str] saml_version: SAML version for the app's sign-on mode. Valid values are: `"2.0"` or `"1.1"`. Default is `"2.0"`.
         :param pulumi.Input[str] sign_on_mode: Sign-on mode of application.
@@ -2567,15 +2551,15 @@
         """
         return pulumi.get(self, "attribute_statements")
 
     @property
     @pulumi.getter
     def audience(self) -> pulumi.Output[Optional[str]]:
         """
-        Audience Restriction
+        Audience restriction.
         """
         return pulumi.get(self, "audience")
 
     @property
     @pulumi.getter(name="authenticationPolicy")
     def authentication_policy(self) -> pulumi.Output[Optional[str]]:
         """
@@ -2583,15 +2567,15 @@
         """
         return pulumi.get(self, "authentication_policy")
 
     @property
     @pulumi.getter(name="authnContextClassRef")
     def authn_context_class_ref(self) -> pulumi.Output[Optional[str]]:
         """
-        Identifies the SAML authentication context class for the assertion’s authentication statement
+        Identifies the SAML authentication context class for the assertion’s authentication statement.
         """
         return pulumi.get(self, "authn_context_class_ref")
 
     @property
     @pulumi.getter(name="autoSubmitToolbar")
     def auto_submit_toolbar(self) -> pulumi.Output[Optional[bool]]:
         """
@@ -2615,23 +2599,23 @@
         """
         return pulumi.get(self, "default_relay_state")
 
     @property
     @pulumi.getter
     def destination(self) -> pulumi.Output[Optional[str]]:
         """
-        Identifies the location where the SAML response is intended to be sent inside of the SAML assertion
+        Identifies the location where the SAML response is intended to be sent inside the SAML assertion.
         """
         return pulumi.get(self, "destination")
 
     @property
     @pulumi.getter(name="digestAlgorithm")
     def digest_algorithm(self) -> pulumi.Output[Optional[str]]:
         """
-        Determines the digest algorithm used to digitally sign the SAML assertion and response
+        Determines the digest algorithm used to digitally sign the SAML assertion and response.
         """
         return pulumi.get(self, "digest_algorithm")
 
     @property
     @pulumi.getter(name="embedUrl")
     def embed_url(self) -> pulumi.Output[str]:
         """
@@ -2807,15 +2791,15 @@
         """
         return pulumi.get(self, "metadata_url")
 
     @property
     @pulumi.getter
     def name(self) -> pulumi.Output[str]:
         """
-        The name of the attribute statement.
+        Name assigned to the application by Okta.
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter(name="preconfiguredApp")
     def preconfigured_app(self) -> pulumi.Output[Optional[str]]:
         """
```

### Comparing `pulumi_okta-4.9.0a1713462165/pulumi_okta/app/secure_password_store.py` & `pulumi_okta-4.9.0a1713902092/pulumi_okta/app/secure_password_store.py`

 * *Files 1% similar despite different names*

```diff
@@ -1039,27 +1039,25 @@
 
         > During an apply if there is change in `status` the app will first be
         activated or deactivated in accordance with the `status` change. Then, all
         other arguments that changed will be applied.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_okta as okta
 
         example = okta.app.SecurePasswordStore("example",
             label="example",
             username_field="user",
             password_field="pass",
             url="https://test.com",
             credentials_scheme="ADMIN_SETS_CREDENTIALS")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Secure Password Store Application can be imported via the Okta ID.
 
         ```sh
         $ pulumi import okta:app/securePasswordStore:SecurePasswordStore example &#60;app id&#62;
@@ -1108,27 +1106,25 @@
 
         > During an apply if there is change in `status` the app will first be
         activated or deactivated in accordance with the `status` change. Then, all
         other arguments that changed will be applied.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_okta as okta
 
         example = okta.app.SecurePasswordStore("example",
             label="example",
             username_field="user",
             password_field="pass",
             url="https://test.com",
             credentials_scheme="ADMIN_SETS_CREDENTIALS")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Secure Password Store Application can be imported via the Okta ID.
 
         ```sh
         $ pulumi import okta:app/securePasswordStore:SecurePasswordStore example &#60;app id&#62;
```

### Comparing `pulumi_okta-4.9.0a1713462165/pulumi_okta/app/swa.py` & `pulumi_okta-4.9.0a1713902092/pulumi_okta/app/swa.py`

 * *Files 0% similar despite different names*

```diff
@@ -877,27 +877,25 @@
 
         > During an apply if there is change in `status` the app will first be
         activated or deactivated in accordance with the `status` change. Then, all
         other arguments that changed will be applied.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_okta as okta
 
         example = okta.app.Swa("example",
             label="example",
             button_field="btn-login",
             password_field="txtbox-password",
             username_field="txtbox-username",
             url="https://example.com/login.html")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Okta SWA App can be imported via the Okta ID.
 
         ```sh
         $ pulumi import okta:app/swa:Swa example &#60;app id&#62;
@@ -941,27 +939,25 @@
 
         > During an apply if there is change in `status` the app will first be
         activated or deactivated in accordance with the `status` change. Then, all
         other arguments that changed will be applied.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_okta as okta
 
         example = okta.app.Swa("example",
             label="example",
             button_field="btn-login",
             password_field="txtbox-password",
             username_field="txtbox-username",
             url="https://example.com/login.html")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Okta SWA App can be imported via the Okta ID.
 
         ```sh
         $ pulumi import okta:app/swa:Swa example &#60;app id&#62;
```

### Comparing `pulumi_okta-4.9.0a1713462165/pulumi_okta/app/three_field.py` & `pulumi_okta-4.9.0a1713902092/pulumi_okta/app/three_field.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713462165/pulumi_okta/app/user.py` & `pulumi_okta-4.9.0a1713902092/pulumi_okta/app/user.py`

 * *Files 2% similar despite different names*

```diff
@@ -244,25 +244,23 @@
                  retain_assignment: Optional[pulumi.Input[bool]] = None,
                  user_id: Optional[pulumi.Input[str]] = None,
                  username: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_okta as okta
 
         example = okta.app.User("example",
             app_id="<app_id>",
             user_id="<user id>",
             username="example")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         An Application User can be imported via the Okta ID.
 
         ```sh
         $ pulumi import okta:app/user:User example &#60;app id&#62;/&#60;user id&#62;
@@ -283,25 +281,23 @@
     def __init__(__self__,
                  resource_name: str,
                  args: UserArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_okta as okta
 
         example = okta.app.User("example",
             app_id="<app_id>",
             user_id="<user id>",
             username="example")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         An Application User can be imported via the Okta ID.
 
         ```sh
         $ pulumi import okta:app/user:User example &#60;app id&#62;/&#60;user id&#62;
```

### Comparing `pulumi_okta-4.9.0a1713462165/pulumi_okta/app_group_assignments.py` & `pulumi_okta-4.9.0a1713902092/pulumi_okta/app_group_assignments.py`

 * *Files 2% similar despite different names*

```diff
@@ -102,15 +102,14 @@
         """
         Assigns groups to an application.
 
         This resource allows you to create multiple App Group assignments.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import json
         import pulumi_okta as okta
 
         example = okta.AppGroupAssignments("example",
             app_id="<app id>",
@@ -124,15 +123,14 @@
                     priority=2,
                     profile=json.dumps({
                         "application profile field": "application profile value",
                     }),
                 ),
             ])
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         An application's group assignments can be imported via `app_id`.
 
         ```sh
         $ pulumi import okta:index/appGroupAssignments:AppGroupAssignments example &#60;app_id&#62;
@@ -152,15 +150,14 @@
         """
         Assigns groups to an application.
 
         This resource allows you to create multiple App Group assignments.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import json
         import pulumi_okta as okta
 
         example = okta.AppGroupAssignments("example",
             app_id="<app id>",
@@ -174,15 +171,14 @@
                     priority=2,
                     profile=json.dumps({
                         "application profile field": "application profile value",
                     }),
                 ),
             ])
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         An application's group assignments can be imported via `app_id`.
 
         ```sh
         $ pulumi import okta:index/appGroupAssignments:AppGroupAssignments example &#60;app_id&#62;
```

### Comparing `pulumi_okta-4.9.0a1713462165/pulumi_okta/app_oauth_api_scope.py` & `pulumi_okta-4.9.0a1713902092/pulumi_okta/app_oauth_api_scope.py`

 * *Files 2% similar despite different names*

```diff
@@ -132,28 +132,26 @@
         """
         Manages API scopes for OAuth applications.
 
         This resource allows you to grant or revoke API scopes for OAuth2 applications within your organization.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_okta as okta
 
         example = okta.AppOauthApiScope("example",
             app_id="<application_id>",
             issuer="<your org domain>",
             scopes=[
                 "okta.users.read",
                 "okta.users.manage",
             ])
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         OAuth API scopes can be imported via the Okta Application ID.
 
         ```sh
         $ pulumi import okta:index/appOauthApiScope:AppOauthApiScope example &#60;app id&#62;
@@ -174,28 +172,26 @@
         """
         Manages API scopes for OAuth applications.
 
         This resource allows you to grant or revoke API scopes for OAuth2 applications within your organization.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_okta as okta
 
         example = okta.AppOauthApiScope("example",
             app_id="<application_id>",
             issuer="<your org domain>",
             scopes=[
                 "okta.users.read",
                 "okta.users.manage",
             ])
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         OAuth API scopes can be imported via the Okta Application ID.
 
         ```sh
         $ pulumi import okta:index/appOauthApiScope:AppOauthApiScope example &#60;app id&#62;
```

### Comparing `pulumi_okta-4.9.0a1713462165/pulumi_okta/app_saml_app_settings.py` & `pulumi_okta-4.9.0a1713902092/pulumi_okta/app_saml_app_settings.py`

 * *Files 5% similar despite different names*

```diff
@@ -99,15 +99,14 @@
                  __props__=None):
         """
         This resource allows you to manage app settings of the SAML Application . It's basically the same as
         `app_settings_json` field in `app.Saml` resource and can be used in cases where settings require to be managed separately.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import json
         import pulumi_okta as okta
 
         test = okta.app.Saml("test",
             preconfigured_app="amazon_aws",
@@ -122,15 +121,14 @@
                 "joinAllRoles": False,
                 "loginURL": "https://console.aws.amazon.com/ec2/home",
                 "roleValuePattern": "arn:aws:iam::${accountid}:saml-provider/OKTA,arn:aws:iam::${accountid}:role/${role}",
                 "sessionDuration": 3200,
                 "useGroupMapping": False,
             }))
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         A settings for the SAML App can be imported via the Okta ID.
 
         ```sh
         $ pulumi import okta:index/appSamlAppSettings:AppSamlAppSettings example &#60;app id&#62;
@@ -149,15 +147,14 @@
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         This resource allows you to manage app settings of the SAML Application . It's basically the same as
         `app_settings_json` field in `app.Saml` resource and can be used in cases where settings require to be managed separately.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import json
         import pulumi_okta as okta
 
         test = okta.app.Saml("test",
             preconfigured_app="amazon_aws",
@@ -172,15 +169,14 @@
                 "joinAllRoles": False,
                 "loginURL": "https://console.aws.amazon.com/ec2/home",
                 "roleValuePattern": "arn:aws:iam::${accountid}:saml-provider/OKTA,arn:aws:iam::${accountid}:role/${role}",
                 "sessionDuration": 3200,
                 "useGroupMapping": False,
             }))
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         A settings for the SAML App can be imported via the Okta ID.
 
         ```sh
         $ pulumi import okta:index/appSamlAppSettings:AppSamlAppSettings example &#60;app id&#62;
```

### Comparing `pulumi_okta-4.9.0a1713462165/pulumi_okta/app_shared_credentials.py` & `pulumi_okta-4.9.0a1713902092/pulumi_okta/app_shared_credentials.py`

 * *Files 1% similar despite different names*

```diff
@@ -943,15 +943,14 @@
 
         > During an apply if there is change in `status` the app will first be
         activated or deactivated in accordance with the `status` change. Then, all
         other arguments that changed will be applied.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_okta as okta
 
         example = okta.AppSharedCredentials("example",
             label="Example App",
             status="ACTIVE",
@@ -968,15 +967,14 @@
             shared_username="sharedusername",
             accessibility_self_service=True,
             accessibility_error_redirect_url="https://example.com/redirect_url_1",
             accessibility_login_redirect_url="https://example.com/redirect_url_2",
             auto_submit_toolbar=True,
             hide_ios=True)
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Okta SWA Shared Credentials App can be imported via the Okta ID.
 
         ```sh
         $ pulumi import okta:index/appSharedCredentials:AppSharedCredentials example &#60;app id&#62;
@@ -1022,15 +1020,14 @@
 
         > During an apply if there is change in `status` the app will first be
         activated or deactivated in accordance with the `status` change. Then, all
         other arguments that changed will be applied.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_okta as okta
 
         example = okta.AppSharedCredentials("example",
             label="Example App",
             status="ACTIVE",
@@ -1047,15 +1044,14 @@
             shared_username="sharedusername",
             accessibility_self_service=True,
             accessibility_error_redirect_url="https://example.com/redirect_url_1",
             accessibility_login_redirect_url="https://example.com/redirect_url_2",
             auto_submit_toolbar=True,
             hide_ios=True)
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Okta SWA Shared Credentials App can be imported via the Okta ID.
 
         ```sh
         $ pulumi import okta:index/appSharedCredentials:AppSharedCredentials example &#60;app id&#62;
```

### Comparing `pulumi_okta-4.9.0a1713462165/pulumi_okta/app_signon_policy.py` & `pulumi_okta-4.9.0a1713902092/pulumi_okta/app_signon_policy.py`

 * *Files 4% similar despite different names*

```diff
@@ -97,15 +97,14 @@
                  opts: Optional[pulumi.ResourceOptions] = None,
                  description: Optional[pulumi.Input[str]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_okta as okta
 
         my_app_policy = okta.AppSignonPolicy("my_app_policy",
             name="My App Sign-On Policy",
             description="Authentication Policy to be used on my app.")
@@ -114,19 +113,17 @@
             type="web",
             grant_types=["authorization_code"],
             redirect_uris=["http://localhost:3000"],
             post_logout_redirect_uris=["http://localhost:3000"],
             response_types=["code"],
             authentication_policy=my_app_policy.id)
         ```
-        <!--End PulumiCodeChooser -->
 
         The created policy can be extended using `app_signon_policy_rules`.
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import json
         import pulumi_okta as okta
 
         my_app_policy = okta.AppSignonPolicy("my_app_policy",
             name="My App Sign-On Policy",
@@ -138,15 +135,14 @@
             re_authentication_frequency="PT43800H",
             constraints=[json.dumps({
                 "knowledge": {
                     "types": ["password"],
                 },
             })])
         ```
-        <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] description: Description of the policy.
         :param pulumi.Input[str] name: Name of the policy.
         """
         ...
@@ -154,15 +150,14 @@
     def __init__(__self__,
                  resource_name: str,
                  args: AppSignonPolicyArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_okta as okta
 
         my_app_policy = okta.AppSignonPolicy("my_app_policy",
             name="My App Sign-On Policy",
             description="Authentication Policy to be used on my app.")
@@ -171,19 +166,17 @@
             type="web",
             grant_types=["authorization_code"],
             redirect_uris=["http://localhost:3000"],
             post_logout_redirect_uris=["http://localhost:3000"],
             response_types=["code"],
             authentication_policy=my_app_policy.id)
         ```
-        <!--End PulumiCodeChooser -->
 
         The created policy can be extended using `app_signon_policy_rules`.
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import json
         import pulumi_okta as okta
 
         my_app_policy = okta.AppSignonPolicy("my_app_policy",
             name="My App Sign-On Policy",
@@ -195,15 +188,14 @@
             re_authentication_frequency="PT43800H",
             constraints=[json.dumps({
                 "knowledge": {
                     "types": ["password"],
                 },
             })])
         ```
-        <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param AppSignonPolicyArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
```

### Comparing `pulumi_okta-4.9.0a1713462165/pulumi_okta/app_signon_policy_rule.py` & `pulumi_okta-4.9.0a1713902092/pulumi_okta/app_signon_policy_rule.py`

 * *Files 3% similar despite different names*

```diff
@@ -893,15 +893,14 @@
         `network_includes`, `platform_include`, `custom_expression`, `device_is_registered`, `device_is_managed`, `users_excluded`,
         `users_included`, `groups_excluded`, `groups_included`, `user_types_excluded` and `user_types_included`.
 
         ## Example Usage
 
         ### Simple usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_okta as okta
 
         test_saml = okta.app.Saml("test",
             label="My App",
             sso_url="https://google.com",
@@ -917,44 +916,40 @@
             honor_force_authn=False,
             authn_context_class_ref="urn:oasis:names:tc:SAML:2.0:ac:classes:PasswordProtectedTransport")
         test = okta.get_app_signon_policy_output(app_id=test_saml.id)
         test_app_signon_policy_rule = okta.AppSignonPolicyRule("test",
             policy_id=test.id,
             name="testAcc_replace_with_uuid")
         ```
-        <!--End PulumiCodeChooser -->
 
         This will create an app sign-on policy rule with the following `THEN` block:
 
         ### Rule with Constraints
 
         ### Example 1:
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import json
         import pulumi_okta as okta
 
         test = okta.AppSignonPolicyRule("test",
             policy_id=test_okta_app_signon_policy["id"],
             name="testAcc_replace_with_uuid",
             constraints=[json.dumps({
                 "knowledge": {
                     "types": ["password"],
                 },
             })])
         ```
-        <!--End PulumiCodeChooser -->
 
         This will create an app sign-on policy rule with the following `THEN` block:
 
         ### Example 2:
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import json
         import pulumi_okta as okta
 
         test = okta.AppSignonPolicyRule("test",
             policy_id=test_okta_app_signon_policy["id"],
@@ -966,24 +961,22 @@
                 },
                 "possession": {
                     "deviceBound": "REQUIRED",
                     "hardwareProtection": "REQUIRED",
                 },
             })])
         ```
-        <!--End PulumiCodeChooser -->
 
         This will create an app sign-on policy rule with the following `THEN` block:
 
         More examples can be
         found [here](https://developer.okta.com/docs/reference/api/policy/#verification-method-json-examples).
 
         ### Complex example
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import json
         import pulumi_okta as okta
 
         test_saml = okta.app.Saml("test",
             label="testAcc_replace_with_uuid",
@@ -996,40 +989,40 @@
             response_signed=True,
             signature_algorithm="RSA_SHA256",
             digest_algorithm="SHA256",
             honor_force_authn=False,
             authn_context_class_ref="urn:oasis:names:tc:SAML:2.0:ac:classes:PasswordProtectedTransport",
             single_logout_issuer="https://dunshire.okta.com",
             single_logout_url="https://dunshire.okta.com/logout",
-            single_logout_certificate=\"\"\"MIIFnDCCA4QCCQDBSLbiON2T1zANBgkqhkiG9w0BAQsFADCBjzELMAkGA1UEBhMCVVMxDjAMBgNV
-        BAgMBU1haW5lMRAwDgYDVQQHDAdDYXJpYm91MRcwFQYDVQQKDA5Tbm93bWFrZXJzIEluYzEUMBIG
-        A1UECwwLRW5naW5lZXJpbmcxDTALBgNVBAMMBFNub3cxIDAeBgkqhkiG9w0BCQEWEWVtYWlsQGV4
-        YW1wbGUuY29tMB4XDTIwMTIwMzIyNDY0M1oXDTMwMTIwMTIyNDY0M1owgY8xCzAJBgNVBAYTAlVT
-        MQ4wDAYDVQQIDAVNYWluZTEQMA4GA1UEBwwHQ2FyaWJvdTEXMBUGA1UECgwOU25vd21ha2VycyBJ
-        bmMxFDASBgNVBAsMC0VuZ2luZWVyaW5nMQ0wCwYDVQQDDARTbm93MSAwHgYJKoZIhvcNAQkBFhFl
-        bWFpbEBleGFtcGxlLmNvbTCCAiIwDQYJKoZIhvcNAQEBBQADggIPADCCAgoCggIBANMmWDjXPdoa
-        PyzIENqeY9njLan2FqCbQPSestWUUcb6NhDsJVGSQ7XR+ozQA5TaJzbP7cAJUj8vCcbqMZsgOQAu
-        O/pzYyQEKptLmrGvPn7xkJ1A1xLkp2NY18cpDTeUPueJUoidZ9EJwEuyUZIktzxNNU1pA1lGijiu
-        2XNxs9d9JR/hm3tCu9Im8qLVB4JtX80YUa6QtlRjWR/H8a373AYCOASdoB3c57fIPD8ATDNy2w/c
-        fCVGiyKDMFB+GA/WTsZpOP3iohRp8ltAncSuzypcztb2iE+jijtTsiC9kUA2abAJqqpoCJubNShi
-        Vff4822czpziS44MV2guC9wANi8u3Uyl5MKsU95j01jzadKRP5S+2f0K+n8n4UoV9fnqZFyuGAKd
-        CJi9K6NlSAP+TgPe/JP9FOSuxQOHWJfmdLHdJD+evoKi9E55sr5lRFK0xU1Fj5Ld7zjC0pXPhtJf
-        sgjEZzD433AsHnRzvRT1KSNCPkLYomznZo5n9rWYgCQ8HcytlQDTesmKE+s05E/VSWNtH84XdDrt
-        ieXwfwhHfaABSu+WjZYxi9CXdFCSvXhsgufUcK4FbYAHl/ga/cJxZc52yFC7Pcq0u9O2BSCjYPdQ
-        DAHs9dhT1RhwVLM8RmoAzgxyyzau0gxnAlgSBD9FMW6dXqIHIp8yAAg9cRXhYRTNAgMBAAEwDQYJ
-        KoZIhvcNAQELBQADggIBADofEC1SvG8qa7pmKCjB/E9Sxhk3mvUO9Gq43xzwVb721Ng3VYf4vGU3
-        wLUwJeLt0wggnj26NJweN5T3q9T8UMxZhHSWvttEU3+S1nArRB0beti716HSlOCDx4wTmBu/D1MG
-        t/kZYFJw+zuzvAcbYct2pK69AQhD8xAIbQvqADJI7cCK3yRry+aWtppc58P81KYabUlCfFXfhJ9E
-        P72ffN4jVHpX3lxxYh7FKAdiKbY2FYzjsc7RdgKI1R3iAAZUCGBTvezNzaetGzTUjjl/g1tcVYij
-        ltH9ZOQBPlUMI88lxUxqgRTerpPmAJH00CACx4JFiZrweLM1trZyy06wNDQgLrqHr3EOagBF/O2h
-        hfTehNdVr6iq3YhKWBo4/+RL0RCzHMh4u86VbDDnDn4Y6HzLuyIAtBFoikoKM6UHTOa0Pqv2bBr5
-        wbkRkVUxl9yJJw/HmTCdfnsM9dTOJUKzEglnGF2184Gg+qJDZB6fSf0EAO1F6sTqiSswl+uHQZiy
-        DaZzyU7Gg5seKOZ20zTRaX3Ihj9Zij/ORnrARE7eM/usKMECp+7syUwAUKxDCZkGiUdskmOhhBGL
-        JtbyK3F2UvoJoLsm3pIcvMak9KwMjSTGJB47ABUP1+w+zGcNk0D5Co3IJ6QekiLfWJyQ+kKsWLKt
-        zOYQQatrnBagM7MI2/T4
+            single_logout_certificate=\"\"\"MIIFnDCCA4QCCQDBSLbiON2T1zANBgkqhkiG9w0BAQsFADCBjzELMAkGA1UEBhMCVVMxDjAMBgNV\\x0d
+        BAgMBU1haW5lMRAwDgYDVQQHDAdDYXJpYm91MRcwFQYDVQQKDA5Tbm93bWFrZXJzIEluYzEUMBIG\\x0d
+        A1UECwwLRW5naW5lZXJpbmcxDTALBgNVBAMMBFNub3cxIDAeBgkqhkiG9w0BCQEWEWVtYWlsQGV4\\x0d
+        YW1wbGUuY29tMB4XDTIwMTIwMzIyNDY0M1oXDTMwMTIwMTIyNDY0M1owgY8xCzAJBgNVBAYTAlVT\\x0d
+        MQ4wDAYDVQQIDAVNYWluZTEQMA4GA1UEBwwHQ2FyaWJvdTEXMBUGA1UECgwOU25vd21ha2VycyBJ\\x0d
+        bmMxFDASBgNVBAsMC0VuZ2luZWVyaW5nMQ0wCwYDVQQDDARTbm93MSAwHgYJKoZIhvcNAQkBFhFl\\x0d
+        bWFpbEBleGFtcGxlLmNvbTCCAiIwDQYJKoZIhvcNAQEBBQADggIPADCCAgoCggIBANMmWDjXPdoa\\x0d
+        PyzIENqeY9njLan2FqCbQPSestWUUcb6NhDsJVGSQ7XR+ozQA5TaJzbP7cAJUj8vCcbqMZsgOQAu\\x0d
+        O/pzYyQEKptLmrGvPn7xkJ1A1xLkp2NY18cpDTeUPueJUoidZ9EJwEuyUZIktzxNNU1pA1lGijiu\\x0d
+        2XNxs9d9JR/hm3tCu9Im8qLVB4JtX80YUa6QtlRjWR/H8a373AYCOASdoB3c57fIPD8ATDNy2w/c\\x0d
+        fCVGiyKDMFB+GA/WTsZpOP3iohRp8ltAncSuzypcztb2iE+jijtTsiC9kUA2abAJqqpoCJubNShi\\x0d
+        Vff4822czpziS44MV2guC9wANi8u3Uyl5MKsU95j01jzadKRP5S+2f0K+n8n4UoV9fnqZFyuGAKd\\x0d
+        CJi9K6NlSAP+TgPe/JP9FOSuxQOHWJfmdLHdJD+evoKi9E55sr5lRFK0xU1Fj5Ld7zjC0pXPhtJf\\x0d
+        sgjEZzD433AsHnRzvRT1KSNCPkLYomznZo5n9rWYgCQ8HcytlQDTesmKE+s05E/VSWNtH84XdDrt\\x0d
+        ieXwfwhHfaABSu+WjZYxi9CXdFCSvXhsgufUcK4FbYAHl/ga/cJxZc52yFC7Pcq0u9O2BSCjYPdQ\\x0d
+        DAHs9dhT1RhwVLM8RmoAzgxyyzau0gxnAlgSBD9FMW6dXqIHIp8yAAg9cRXhYRTNAgMBAAEwDQYJ\\x0d
+        KoZIhvcNAQELBQADggIBADofEC1SvG8qa7pmKCjB/E9Sxhk3mvUO9Gq43xzwVb721Ng3VYf4vGU3\\x0d
+        wLUwJeLt0wggnj26NJweN5T3q9T8UMxZhHSWvttEU3+S1nArRB0beti716HSlOCDx4wTmBu/D1MG\\x0d
+        t/kZYFJw+zuzvAcbYct2pK69AQhD8xAIbQvqADJI7cCK3yRry+aWtppc58P81KYabUlCfFXfhJ9E\\x0d
+        P72ffN4jVHpX3lxxYh7FKAdiKbY2FYzjsc7RdgKI1R3iAAZUCGBTvezNzaetGzTUjjl/g1tcVYij\\x0d
+        ltH9ZOQBPlUMI88lxUxqgRTerpPmAJH00CACx4JFiZrweLM1trZyy06wNDQgLrqHr3EOagBF/O2h\\x0d
+        hfTehNdVr6iq3YhKWBo4/+RL0RCzHMh4u86VbDDnDn4Y6HzLuyIAtBFoikoKM6UHTOa0Pqv2bBr5\\x0d
+        wbkRkVUxl9yJJw/HmTCdfnsM9dTOJUKzEglnGF2184Gg+qJDZB6fSf0EAO1F6sTqiSswl+uHQZiy\\x0d
+        DaZzyU7Gg5seKOZ20zTRaX3Ihj9Zij/ORnrARE7eM/usKMECp+7syUwAUKxDCZkGiUdskmOhhBGL\\x0d
+        JtbyK3F2UvoJoLsm3pIcvMak9KwMjSTGJB47ABUP1+w+zGcNk0D5Co3IJ6QekiLfWJyQ+kKsWLKt\\x0d
+        zOYQQatrnBagM7MI2/T4\\x0d
         \"\"\",
             attribute_statements=[okta.app.SamlAttributeStatementArgs(
                 type="GROUP",
                 name="groups",
                 filter_type="REGEX",
                 filter_value=".*",
             )])
@@ -1145,15 +1138,14 @@
                         "deviceBound": "REQUIRED",
                         "hardwareProtection": "REQUIRED",
                         "userPresence": "OPTIONAL",
                     },
                 }),
             ])
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Okta app sign-on policy rule can be imported via the Okta ID.
 
         ```sh
         $ pulumi import okta:index/appSignonPolicyRule:AppSignonPolicyRule example &#60;policy_id&#62;/&#60;rule_id&#62;
@@ -1205,15 +1197,14 @@
         `network_includes`, `platform_include`, `custom_expression`, `device_is_registered`, `device_is_managed`, `users_excluded`,
         `users_included`, `groups_excluded`, `groups_included`, `user_types_excluded` and `user_types_included`.
 
         ## Example Usage
 
         ### Simple usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_okta as okta
 
         test_saml = okta.app.Saml("test",
             label="My App",
             sso_url="https://google.com",
@@ -1229,44 +1220,40 @@
             honor_force_authn=False,
             authn_context_class_ref="urn:oasis:names:tc:SAML:2.0:ac:classes:PasswordProtectedTransport")
         test = okta.get_app_signon_policy_output(app_id=test_saml.id)
         test_app_signon_policy_rule = okta.AppSignonPolicyRule("test",
             policy_id=test.id,
             name="testAcc_replace_with_uuid")
         ```
-        <!--End PulumiCodeChooser -->
 
         This will create an app sign-on policy rule with the following `THEN` block:
 
         ### Rule with Constraints
 
         ### Example 1:
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import json
         import pulumi_okta as okta
 
         test = okta.AppSignonPolicyRule("test",
             policy_id=test_okta_app_signon_policy["id"],
             name="testAcc_replace_with_uuid",
             constraints=[json.dumps({
                 "knowledge": {
                     "types": ["password"],
                 },
             })])
         ```
-        <!--End PulumiCodeChooser -->
 
         This will create an app sign-on policy rule with the following `THEN` block:
 
         ### Example 2:
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import json
         import pulumi_okta as okta
 
         test = okta.AppSignonPolicyRule("test",
             policy_id=test_okta_app_signon_policy["id"],
@@ -1278,24 +1265,22 @@
                 },
                 "possession": {
                     "deviceBound": "REQUIRED",
                     "hardwareProtection": "REQUIRED",
                 },
             })])
         ```
-        <!--End PulumiCodeChooser -->
 
         This will create an app sign-on policy rule with the following `THEN` block:
 
         More examples can be
         found [here](https://developer.okta.com/docs/reference/api/policy/#verification-method-json-examples).
 
         ### Complex example
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import json
         import pulumi_okta as okta
 
         test_saml = okta.app.Saml("test",
             label="testAcc_replace_with_uuid",
@@ -1308,40 +1293,40 @@
             response_signed=True,
             signature_algorithm="RSA_SHA256",
             digest_algorithm="SHA256",
             honor_force_authn=False,
             authn_context_class_ref="urn:oasis:names:tc:SAML:2.0:ac:classes:PasswordProtectedTransport",
             single_logout_issuer="https://dunshire.okta.com",
             single_logout_url="https://dunshire.okta.com/logout",
-            single_logout_certificate=\"\"\"MIIFnDCCA4QCCQDBSLbiON2T1zANBgkqhkiG9w0BAQsFADCBjzELMAkGA1UEBhMCVVMxDjAMBgNV
-        BAgMBU1haW5lMRAwDgYDVQQHDAdDYXJpYm91MRcwFQYDVQQKDA5Tbm93bWFrZXJzIEluYzEUMBIG
-        A1UECwwLRW5naW5lZXJpbmcxDTALBgNVBAMMBFNub3cxIDAeBgkqhkiG9w0BCQEWEWVtYWlsQGV4
-        YW1wbGUuY29tMB4XDTIwMTIwMzIyNDY0M1oXDTMwMTIwMTIyNDY0M1owgY8xCzAJBgNVBAYTAlVT
-        MQ4wDAYDVQQIDAVNYWluZTEQMA4GA1UEBwwHQ2FyaWJvdTEXMBUGA1UECgwOU25vd21ha2VycyBJ
-        bmMxFDASBgNVBAsMC0VuZ2luZWVyaW5nMQ0wCwYDVQQDDARTbm93MSAwHgYJKoZIhvcNAQkBFhFl
-        bWFpbEBleGFtcGxlLmNvbTCCAiIwDQYJKoZIhvcNAQEBBQADggIPADCCAgoCggIBANMmWDjXPdoa
-        PyzIENqeY9njLan2FqCbQPSestWUUcb6NhDsJVGSQ7XR+ozQA5TaJzbP7cAJUj8vCcbqMZsgOQAu
-        O/pzYyQEKptLmrGvPn7xkJ1A1xLkp2NY18cpDTeUPueJUoidZ9EJwEuyUZIktzxNNU1pA1lGijiu
-        2XNxs9d9JR/hm3tCu9Im8qLVB4JtX80YUa6QtlRjWR/H8a373AYCOASdoB3c57fIPD8ATDNy2w/c
-        fCVGiyKDMFB+GA/WTsZpOP3iohRp8ltAncSuzypcztb2iE+jijtTsiC9kUA2abAJqqpoCJubNShi
-        Vff4822czpziS44MV2guC9wANi8u3Uyl5MKsU95j01jzadKRP5S+2f0K+n8n4UoV9fnqZFyuGAKd
-        CJi9K6NlSAP+TgPe/JP9FOSuxQOHWJfmdLHdJD+evoKi9E55sr5lRFK0xU1Fj5Ld7zjC0pXPhtJf
-        sgjEZzD433AsHnRzvRT1KSNCPkLYomznZo5n9rWYgCQ8HcytlQDTesmKE+s05E/VSWNtH84XdDrt
-        ieXwfwhHfaABSu+WjZYxi9CXdFCSvXhsgufUcK4FbYAHl/ga/cJxZc52yFC7Pcq0u9O2BSCjYPdQ
-        DAHs9dhT1RhwVLM8RmoAzgxyyzau0gxnAlgSBD9FMW6dXqIHIp8yAAg9cRXhYRTNAgMBAAEwDQYJ
-        KoZIhvcNAQELBQADggIBADofEC1SvG8qa7pmKCjB/E9Sxhk3mvUO9Gq43xzwVb721Ng3VYf4vGU3
-        wLUwJeLt0wggnj26NJweN5T3q9T8UMxZhHSWvttEU3+S1nArRB0beti716HSlOCDx4wTmBu/D1MG
-        t/kZYFJw+zuzvAcbYct2pK69AQhD8xAIbQvqADJI7cCK3yRry+aWtppc58P81KYabUlCfFXfhJ9E
-        P72ffN4jVHpX3lxxYh7FKAdiKbY2FYzjsc7RdgKI1R3iAAZUCGBTvezNzaetGzTUjjl/g1tcVYij
-        ltH9ZOQBPlUMI88lxUxqgRTerpPmAJH00CACx4JFiZrweLM1trZyy06wNDQgLrqHr3EOagBF/O2h
-        hfTehNdVr6iq3YhKWBo4/+RL0RCzHMh4u86VbDDnDn4Y6HzLuyIAtBFoikoKM6UHTOa0Pqv2bBr5
-        wbkRkVUxl9yJJw/HmTCdfnsM9dTOJUKzEglnGF2184Gg+qJDZB6fSf0EAO1F6sTqiSswl+uHQZiy
-        DaZzyU7Gg5seKOZ20zTRaX3Ihj9Zij/ORnrARE7eM/usKMECp+7syUwAUKxDCZkGiUdskmOhhBGL
-        JtbyK3F2UvoJoLsm3pIcvMak9KwMjSTGJB47ABUP1+w+zGcNk0D5Co3IJ6QekiLfWJyQ+kKsWLKt
-        zOYQQatrnBagM7MI2/T4
+            single_logout_certificate=\"\"\"MIIFnDCCA4QCCQDBSLbiON2T1zANBgkqhkiG9w0BAQsFADCBjzELMAkGA1UEBhMCVVMxDjAMBgNV\\x0d
+        BAgMBU1haW5lMRAwDgYDVQQHDAdDYXJpYm91MRcwFQYDVQQKDA5Tbm93bWFrZXJzIEluYzEUMBIG\\x0d
+        A1UECwwLRW5naW5lZXJpbmcxDTALBgNVBAMMBFNub3cxIDAeBgkqhkiG9w0BCQEWEWVtYWlsQGV4\\x0d
+        YW1wbGUuY29tMB4XDTIwMTIwMzIyNDY0M1oXDTMwMTIwMTIyNDY0M1owgY8xCzAJBgNVBAYTAlVT\\x0d
+        MQ4wDAYDVQQIDAVNYWluZTEQMA4GA1UEBwwHQ2FyaWJvdTEXMBUGA1UECgwOU25vd21ha2VycyBJ\\x0d
+        bmMxFDASBgNVBAsMC0VuZ2luZWVyaW5nMQ0wCwYDVQQDDARTbm93MSAwHgYJKoZIhvcNAQkBFhFl\\x0d
+        bWFpbEBleGFtcGxlLmNvbTCCAiIwDQYJKoZIhvcNAQEBBQADggIPADCCAgoCggIBANMmWDjXPdoa\\x0d
+        PyzIENqeY9njLan2FqCbQPSestWUUcb6NhDsJVGSQ7XR+ozQA5TaJzbP7cAJUj8vCcbqMZsgOQAu\\x0d
+        O/pzYyQEKptLmrGvPn7xkJ1A1xLkp2NY18cpDTeUPueJUoidZ9EJwEuyUZIktzxNNU1pA1lGijiu\\x0d
+        2XNxs9d9JR/hm3tCu9Im8qLVB4JtX80YUa6QtlRjWR/H8a373AYCOASdoB3c57fIPD8ATDNy2w/c\\x0d
+        fCVGiyKDMFB+GA/WTsZpOP3iohRp8ltAncSuzypcztb2iE+jijtTsiC9kUA2abAJqqpoCJubNShi\\x0d
+        Vff4822czpziS44MV2guC9wANi8u3Uyl5MKsU95j01jzadKRP5S+2f0K+n8n4UoV9fnqZFyuGAKd\\x0d
+        CJi9K6NlSAP+TgPe/JP9FOSuxQOHWJfmdLHdJD+evoKi9E55sr5lRFK0xU1Fj5Ld7zjC0pXPhtJf\\x0d
+        sgjEZzD433AsHnRzvRT1KSNCPkLYomznZo5n9rWYgCQ8HcytlQDTesmKE+s05E/VSWNtH84XdDrt\\x0d
+        ieXwfwhHfaABSu+WjZYxi9CXdFCSvXhsgufUcK4FbYAHl/ga/cJxZc52yFC7Pcq0u9O2BSCjYPdQ\\x0d
+        DAHs9dhT1RhwVLM8RmoAzgxyyzau0gxnAlgSBD9FMW6dXqIHIp8yAAg9cRXhYRTNAgMBAAEwDQYJ\\x0d
+        KoZIhvcNAQELBQADggIBADofEC1SvG8qa7pmKCjB/E9Sxhk3mvUO9Gq43xzwVb721Ng3VYf4vGU3\\x0d
+        wLUwJeLt0wggnj26NJweN5T3q9T8UMxZhHSWvttEU3+S1nArRB0beti716HSlOCDx4wTmBu/D1MG\\x0d
+        t/kZYFJw+zuzvAcbYct2pK69AQhD8xAIbQvqADJI7cCK3yRry+aWtppc58P81KYabUlCfFXfhJ9E\\x0d
+        P72ffN4jVHpX3lxxYh7FKAdiKbY2FYzjsc7RdgKI1R3iAAZUCGBTvezNzaetGzTUjjl/g1tcVYij\\x0d
+        ltH9ZOQBPlUMI88lxUxqgRTerpPmAJH00CACx4JFiZrweLM1trZyy06wNDQgLrqHr3EOagBF/O2h\\x0d
+        hfTehNdVr6iq3YhKWBo4/+RL0RCzHMh4u86VbDDnDn4Y6HzLuyIAtBFoikoKM6UHTOa0Pqv2bBr5\\x0d
+        wbkRkVUxl9yJJw/HmTCdfnsM9dTOJUKzEglnGF2184Gg+qJDZB6fSf0EAO1F6sTqiSswl+uHQZiy\\x0d
+        DaZzyU7Gg5seKOZ20zTRaX3Ihj9Zij/ORnrARE7eM/usKMECp+7syUwAUKxDCZkGiUdskmOhhBGL\\x0d
+        JtbyK3F2UvoJoLsm3pIcvMak9KwMjSTGJB47ABUP1+w+zGcNk0D5Co3IJ6QekiLfWJyQ+kKsWLKt\\x0d
+        zOYQQatrnBagM7MI2/T4\\x0d
         \"\"\",
             attribute_statements=[okta.app.SamlAttributeStatementArgs(
                 type="GROUP",
                 name="groups",
                 filter_type="REGEX",
                 filter_value=".*",
             )])
@@ -1457,15 +1442,14 @@
                         "deviceBound": "REQUIRED",
                         "hardwareProtection": "REQUIRED",
                         "userPresence": "OPTIONAL",
                     },
                 }),
             ])
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Okta app sign-on policy rule can be imported via the Okta ID.
 
         ```sh
         $ pulumi import okta:index/appSignonPolicyRule:AppSignonPolicyRule example &#60;policy_id&#62;/&#60;rule_id&#62;
```

### Comparing `pulumi_okta-4.9.0a1713462165/pulumi_okta/app_user_base_schema_property.py` & `pulumi_okta-4.9.0a1713902092/pulumi_okta/app_user_base_schema_property.py`

 * *Files 2% similar despite different names*

```diff
@@ -329,27 +329,25 @@
         """
         Manages an Application User Base Schema property.
 
         This resource allows you to configure a base app user schema property.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_okta as okta
 
         example = okta.AppUserBaseSchemaProperty("example",
             app_id="<app id>",
             index="customPropertyName",
             title="customPropertyName",
             type="string",
             master="OKTA")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         App user base schema property can be imported via the property index and app id.
 
         ```sh
         $ pulumi import okta:index/appUserBaseSchemaProperty:AppUserBaseSchemaProperty example &#60;app id&#62;/&#60;property name&#62;
@@ -376,27 +374,25 @@
         """
         Manages an Application User Base Schema property.
 
         This resource allows you to configure a base app user schema property.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_okta as okta
 
         example = okta.AppUserBaseSchemaProperty("example",
             app_id="<app id>",
             index="customPropertyName",
             title="customPropertyName",
             type="string",
             master="OKTA")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         App user base schema property can be imported via the property index and app id.
 
         ```sh
         $ pulumi import okta:index/appUserBaseSchemaProperty:AppUserBaseSchemaProperty example &#60;app id&#62;/&#60;property name&#62;
```

### Comparing `pulumi_okta-4.9.0a1713462165/pulumi_okta/app_user_schema_property.py` & `pulumi_okta-4.9.0a1713902092/pulumi_okta/app_user_schema_property.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,15 @@
                  union: Optional[pulumi.Input[bool]] = None,
                  unique: Optional[pulumi.Input[str]] = None,
                  user_type: Optional[pulumi.Input[str]] = None):
         """
         The set of arguments for constructing a AppUserSchemaProperty resource.
         :param pulumi.Input[str] app_id: The Application's ID the user custom schema property should be assigned to.
         :param pulumi.Input[str] index: The property name.
-        :param pulumi.Input[str] title: display name for the enum value.
+        :param pulumi.Input[str] title: The display name.
         :param pulumi.Input[str] type: The type of the schema property. It can be `"string"`, `"boolean"`, `"number"`, `"integer"`, `"array"`, or `"object"`.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] array_enums: Array of values that an array property's items can be set to.
         :param pulumi.Input[Sequence[pulumi.Input['AppUserSchemaPropertyArrayOneOfArgs']]] array_one_ofs: Display name and value an enum array can be set to.
         :param pulumi.Input[str] array_type: The type of the array elements if `type` is set to `"array"`.
         :param pulumi.Input[str] description: The description of the user schema property.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] enums: Array of values a primitive property can be set to. See `array_enum` for arrays.
         :param pulumi.Input[str] external_name: External name of the user schema property.
@@ -124,15 +124,15 @@
     def index(self, value: pulumi.Input[str]):
         pulumi.set(self, "index", value)
 
     @property
     @pulumi.getter
     def title(self) -> pulumi.Input[str]:
         """
-        display name for the enum value.
+        The display name.
         """
         return pulumi.get(self, "title")
 
     @title.setter
     def title(self, value: pulumi.Input[str]):
         pulumi.set(self, "title", value)
 
@@ -391,15 +391,15 @@
         :param pulumi.Input[str] master: Master priority for the user schema property. It can be set to `"PROFILE_MASTER"` or `"OKTA"`.
         :param pulumi.Input[int] max_length: The maximum length of the user property value. Only applies to type `"string"`.
         :param pulumi.Input[int] min_length: The minimum length of the user property value. Only applies to type `"string"`.
         :param pulumi.Input[Sequence[pulumi.Input['AppUserSchemaPropertyOneOfArgs']]] one_ofs: Array of maps containing a mapping for display name to enum value.
         :param pulumi.Input[str] permissions: Access control permissions for the property. It can be set to `"READ_WRITE"`, `"READ_ONLY"`, `"HIDE"`.
         :param pulumi.Input[bool] required: Whether the property is required for this application's users.
         :param pulumi.Input[str] scope: determines whether an app user attribute can be set at the Personal `"SELF"` or Group `"NONE"` level. Default value is `"NONE"`.
-        :param pulumi.Input[str] title: display name for the enum value.
+        :param pulumi.Input[str] title: The display name.
         :param pulumi.Input[str] type: The type of the schema property. It can be `"string"`, `"boolean"`, `"number"`, `"integer"`, `"array"`, or `"object"`.
         :param pulumi.Input[bool] union: If `type` is set to `"array"`, used to set whether attribute value is determined by group priority `false`, or combine values across groups `true`. Can not be set to `true` if `scope` is set to `"SELF"`.
         :param pulumi.Input[str] unique: Whether the property should be unique. It can be set to `UNIQUE_VALIDATED` or `NOT_UNIQUE`.
         :param pulumi.Input[str] user_type: User type ID. By default, it is `default`
         """
         if app_id is not None:
             pulumi.set(__self__, "app_id", app_id)
@@ -636,15 +636,15 @@
     def scope(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "scope", value)
 
     @property
     @pulumi.getter
     def title(self) -> Optional[pulumi.Input[str]]:
         """
-        display name for the enum value.
+        The display name.
         """
         return pulumi.get(self, "title")
 
     @title.setter
     def title(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "title", value)
 
@@ -723,29 +723,27 @@
                  union: Optional[pulumi.Input[bool]] = None,
                  unique: Optional[pulumi.Input[str]] = None,
                  user_type: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_okta as okta
 
         example = okta.AppUserSchemaProperty("example",
             app_id="<app id>",
             index="customPropertyName",
             title="customPropertyName",
             type="string",
             description="My custom property name",
             master="OKTA",
             scope="SELF")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         App user schema property can be imported via the property index and app id.
 
         ```sh
         $ pulumi import okta:index/appUserSchemaProperty:AppUserSchemaProperty example &#60;app id&#62;/&#60;property name&#62;
@@ -765,44 +763,42 @@
         :param pulumi.Input[str] master: Master priority for the user schema property. It can be set to `"PROFILE_MASTER"` or `"OKTA"`.
         :param pulumi.Input[int] max_length: The maximum length of the user property value. Only applies to type `"string"`.
         :param pulumi.Input[int] min_length: The minimum length of the user property value. Only applies to type `"string"`.
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['AppUserSchemaPropertyOneOfArgs']]]] one_ofs: Array of maps containing a mapping for display name to enum value.
         :param pulumi.Input[str] permissions: Access control permissions for the property. It can be set to `"READ_WRITE"`, `"READ_ONLY"`, `"HIDE"`.
         :param pulumi.Input[bool] required: Whether the property is required for this application's users.
         :param pulumi.Input[str] scope: determines whether an app user attribute can be set at the Personal `"SELF"` or Group `"NONE"` level. Default value is `"NONE"`.
-        :param pulumi.Input[str] title: display name for the enum value.
+        :param pulumi.Input[str] title: The display name.
         :param pulumi.Input[str] type: The type of the schema property. It can be `"string"`, `"boolean"`, `"number"`, `"integer"`, `"array"`, or `"object"`.
         :param pulumi.Input[bool] union: If `type` is set to `"array"`, used to set whether attribute value is determined by group priority `false`, or combine values across groups `true`. Can not be set to `true` if `scope` is set to `"SELF"`.
         :param pulumi.Input[str] unique: Whether the property should be unique. It can be set to `UNIQUE_VALIDATED` or `NOT_UNIQUE`.
         :param pulumi.Input[str] user_type: User type ID. By default, it is `default`
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: AppUserSchemaPropertyArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_okta as okta
 
         example = okta.AppUserSchemaProperty("example",
             app_id="<app id>",
             index="customPropertyName",
             title="customPropertyName",
             type="string",
             description="My custom property name",
             master="OKTA",
             scope="SELF")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         App user schema property can be imported via the property index and app id.
 
         ```sh
         $ pulumi import okta:index/appUserSchemaProperty:AppUserSchemaProperty example &#60;app id&#62;/&#60;property name&#62;
@@ -932,15 +928,15 @@
         :param pulumi.Input[str] master: Master priority for the user schema property. It can be set to `"PROFILE_MASTER"` or `"OKTA"`.
         :param pulumi.Input[int] max_length: The maximum length of the user property value. Only applies to type `"string"`.
         :param pulumi.Input[int] min_length: The minimum length of the user property value. Only applies to type `"string"`.
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['AppUserSchemaPropertyOneOfArgs']]]] one_ofs: Array of maps containing a mapping for display name to enum value.
         :param pulumi.Input[str] permissions: Access control permissions for the property. It can be set to `"READ_WRITE"`, `"READ_ONLY"`, `"HIDE"`.
         :param pulumi.Input[bool] required: Whether the property is required for this application's users.
         :param pulumi.Input[str] scope: determines whether an app user attribute can be set at the Personal `"SELF"` or Group `"NONE"` level. Default value is `"NONE"`.
-        :param pulumi.Input[str] title: display name for the enum value.
+        :param pulumi.Input[str] title: The display name.
         :param pulumi.Input[str] type: The type of the schema property. It can be `"string"`, `"boolean"`, `"number"`, `"integer"`, `"array"`, or `"object"`.
         :param pulumi.Input[bool] union: If `type` is set to `"array"`, used to set whether attribute value is determined by group priority `false`, or combine values across groups `true`. Can not be set to `true` if `scope` is set to `"SELF"`.
         :param pulumi.Input[str] unique: Whether the property should be unique. It can be set to `UNIQUE_VALIDATED` or `NOT_UNIQUE`.
         :param pulumi.Input[str] user_type: User type ID. By default, it is `default`
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
@@ -1097,15 +1093,15 @@
         """
         return pulumi.get(self, "scope")
 
     @property
     @pulumi.getter
     def title(self) -> pulumi.Output[str]:
         """
-        display name for the enum value.
+        The display name.
         """
         return pulumi.get(self, "title")
 
     @property
     @pulumi.getter
     def type(self) -> pulumi.Output[str]:
         """
```

### Comparing `pulumi_okta-4.9.0a1713462165/pulumi_okta/auth/__init__.py` & `pulumi_okta-4.9.0a1713902092/pulumi_okta/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713462165/pulumi_okta/auth/get_server.py` & `pulumi_okta-4.9.0a1713902092/pulumi_okta/auth/get_server.py`

 * *Files 2% similar despite different names*

```diff
@@ -167,22 +167,20 @@
 def get_server(name: Optional[str] = None,
                opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetServerResult:
     """
     Use this data source to retrieve an auth server from Okta.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_okta as okta
 
     example = okta.auth.get_server(name="Example Auth")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str name: The name of the auth server to retrieve.
     """
     __args__ = dict()
     __args__['name'] = name
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
@@ -206,20 +204,18 @@
 def get_server_output(name: Optional[pulumi.Input[str]] = None,
                       opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetServerResult]:
     """
     Use this data source to retrieve an auth server from Okta.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_okta as okta
 
     example = okta.auth.get_server(name="Example Auth")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str name: The name of the auth server to retrieve.
     """
     ...
```

### Comparing `pulumi_okta-4.9.0a1713462165/pulumi_okta/auth/get_server_policy.py` & `pulumi_okta-4.9.0a1713902092/pulumi_okta/auth/get_server_policy.py`

 * *Files 8% similar despite different names*

```diff
@@ -102,23 +102,21 @@
                       name: Optional[str] = None,
                       opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetServerPolicyResult:
     """
     Use this data source to retrieve an authorization server policy from Okta.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_okta as okta
 
     example = okta.auth.get_server_policy(auth_server_id="<auth server id>",
         name="staff")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str auth_server_id: The ID of the Auth Server.
     :param str name: Name of policy to retrieve.
     """
     __args__ = dict()
     __args__['authServerId'] = auth_server_id
@@ -140,22 +138,20 @@
                              name: Optional[pulumi.Input[str]] = None,
                              opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetServerPolicyResult]:
     """
     Use this data source to retrieve an authorization server policy from Okta.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_okta as okta
 
     example = okta.auth.get_server_policy(auth_server_id="<auth server id>",
         name="staff")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str auth_server_id: The ID of the Auth Server.
     :param str name: Name of policy to retrieve.
     """
     ...
```

### Comparing `pulumi_okta-4.9.0a1713462165/pulumi_okta/auth/get_server_scopes.py` & `pulumi_okta-4.9.0a1713902092/pulumi_okta/auth/get_server_scopes.py`

 * *Files 4% similar despite different names*

```diff
@@ -69,22 +69,20 @@
 def get_server_scopes(auth_server_id: Optional[str] = None,
                       opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetServerScopesResult:
     """
     Use this data source to retrieve a list of authorization server scopes from Okta.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_okta as okta
 
     test = okta.auth.get_server_scopes(auth_server_id="default")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str auth_server_id: Auth server ID.
     """
     __args__ = dict()
     __args__['authServerId'] = auth_server_id
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
@@ -100,20 +98,18 @@
 def get_server_scopes_output(auth_server_id: Optional[pulumi.Input[str]] = None,
                              opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetServerScopesResult]:
     """
     Use this data source to retrieve a list of authorization server scopes from Okta.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_okta as okta
 
     test = okta.auth.get_server_scopes(auth_server_id="default")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str auth_server_id: Auth server ID.
     """
     ...
```

### Comparing `pulumi_okta-4.9.0a1713462165/pulumi_okta/auth/outputs.py` & `pulumi_okta-4.9.0a1713902092/pulumi_okta/auth/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713462165/pulumi_okta/auth/server.py` & `pulumi_okta-4.9.0a1713902092/pulumi_okta/auth/server.py`

 * *Files 0% similar despite different names*

```diff
@@ -297,27 +297,25 @@
         """
         Creates an Authorization Server.
 
         This resource allows you to create and configure an Authorization Server.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_okta as okta
 
         example = okta.auth.Server("example",
             audiences=["api://example"],
             description="My Example Auth Server",
             name="example",
             issuer_mode="CUSTOM_URL",
             status="ACTIVE")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Authorization Server can be imported via the Okta ID.
 
         ```sh
         $ pulumi import okta:auth/server:Server example &#60;auth server id&#62;
@@ -341,27 +339,25 @@
         """
         Creates an Authorization Server.
 
         This resource allows you to create and configure an Authorization Server.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_okta as okta
 
         example = okta.auth.Server("example",
             audiences=["api://example"],
             description="My Example Auth Server",
             name="example",
             issuer_mode="CUSTOM_URL",
             status="ACTIVE")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Authorization Server can be imported via the Okta ID.
 
         ```sh
         $ pulumi import okta:auth/server:Server example &#60;auth server id&#62;
```

### Comparing `pulumi_okta-4.9.0a1713462165/pulumi_okta/auth/server_claim.py` & `pulumi_okta-4.9.0a1713902092/pulumi_okta/auth/server_claim.py`

 * *Files 0% similar despite different names*

```diff
@@ -330,27 +330,25 @@
         """
         Creates an Authorization Server Claim.
 
         This resource allows you to create and configure an Authorization Server Claim.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_okta as okta
 
         example = okta.auth.ServerClaim("example",
             auth_server_id="<auth server id>",
             name="staff",
             value="String.substringAfter(user.email, \\"@\\") == \\"example.com\\"",
             scopes=[example_okta_auth_server_scope["name"]],
             claim_type="IDENTITY")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Authorization Server Claim can be imported via the Auth Server ID and Claim ID.
 
         ```sh
         $ pulumi import okta:auth/serverClaim:ServerClaim example &#60;auth server id&#62;/&#60;claim id&#62;
@@ -377,27 +375,25 @@
         """
         Creates an Authorization Server Claim.
 
         This resource allows you to create and configure an Authorization Server Claim.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_okta as okta
 
         example = okta.auth.ServerClaim("example",
             auth_server_id="<auth server id>",
             name="staff",
             value="String.substringAfter(user.email, \\"@\\") == \\"example.com\\"",
             scopes=[example_okta_auth_server_scope["name"]],
             claim_type="IDENTITY")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Authorization Server Claim can be imported via the Auth Server ID and Claim ID.
 
         ```sh
         $ pulumi import okta:auth/serverClaim:ServerClaim example &#60;auth server id&#62;/&#60;claim id&#62;
```

### Comparing `pulumi_okta-4.9.0a1713462165/pulumi_okta/auth/server_policy.py` & `pulumi_okta-4.9.0a1713902092/pulumi_okta/auth/server_policy.py`

 * *Files 4% similar despite different names*

```diff
@@ -230,28 +230,26 @@
         """
         Creates an Authorization Server Policy.
 
         This resource allows you to create and configure an Authorization Server Policy.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_okta as okta
 
         example = okta.auth.ServerPolicy("example",
             auth_server_id="<auth server id>",
             status="ACTIVE",
             name="example",
             description="example",
             priority=1,
             client_whitelists=["ALL_CLIENTS"])
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Authorization Server Policy can be imported via the Auth Server ID and Policy ID.
 
         ```sh
         $ pulumi import okta:auth/serverPolicy:ServerPolicy example &#60;auth server id&#62;/&#60;policy id&#62;
@@ -275,28 +273,26 @@
         """
         Creates an Authorization Server Policy.
 
         This resource allows you to create and configure an Authorization Server Policy.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_okta as okta
 
         example = okta.auth.ServerPolicy("example",
             auth_server_id="<auth server id>",
             status="ACTIVE",
             name="example",
             description="example",
             priority=1,
             client_whitelists=["ALL_CLIENTS"])
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Authorization Server Policy can be imported via the Auth Server ID and Policy ID.
 
         ```sh
         $ pulumi import okta:auth/serverPolicy:ServerPolicy example &#60;auth server id&#62;/&#60;policy id&#62;
```

### Comparing `pulumi_okta-4.9.0a1713462165/pulumi_okta/auth/server_policy_claim.py` & `pulumi_okta-4.9.0a1713902092/pulumi_okta/auth/server_policy_claim.py`

 * *Files 0% similar despite different names*

```diff
@@ -589,29 +589,27 @@
                  type: Optional[pulumi.Input[str]] = None,
                  user_blacklists: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  user_whitelists: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  __props__=None):
         """
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_okta as okta
 
         example = okta.auth.ServerPolicyRule("example",
             auth_server_id="<auth server id>",
             policy_id="<auth server policy id>",
             status="ACTIVE",
             name="example",
             priority=1,
             group_whitelists=["<group ids>"],
             grant_type_whitelists=["implicit"])
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Authorization Server Policy Rule can be imported via the Auth Server ID, Policy ID, and Policy Rule ID.
 
         ```sh
         $ pulumi import okta:auth/serverPolicyClaim:ServerPolicyClaim example &#60;auth server id&#62;/&#60;policy id&#62;/&#60;policy rule id&#62;
@@ -644,29 +642,27 @@
     def __init__(__self__,
                  resource_name: str,
                  args: ServerPolicyClaimArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_okta as okta
 
         example = okta.auth.ServerPolicyRule("example",
             auth_server_id="<auth server id>",
             policy_id="<auth server policy id>",
             status="ACTIVE",
             name="example",
             priority=1,
             group_whitelists=["<group ids>"],
             grant_type_whitelists=["implicit"])
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Authorization Server Policy Rule can be imported via the Auth Server ID, Policy ID, and Policy Rule ID.
 
         ```sh
         $ pulumi import okta:auth/serverPolicyClaim:ServerPolicyClaim example &#60;auth server id&#62;/&#60;policy id&#62;/&#60;policy rule id&#62;
```

### Comparing `pulumi_okta-4.9.0a1713462165/pulumi_okta/auth/server_policy_rule.py` & `pulumi_okta-4.9.0a1713902092/pulumi_okta/auth/server_policy_rule.py`

 * *Files 1% similar despite different names*

```diff
@@ -584,29 +584,27 @@
                  type: Optional[pulumi.Input[str]] = None,
                  user_blacklists: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  user_whitelists: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  __props__=None):
         """
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_okta as okta
 
         example = okta.auth.ServerPolicyRule("example",
             auth_server_id="<auth server id>",
             policy_id="<auth server policy id>",
             status="ACTIVE",
             name="example",
             priority=1,
             group_whitelists=["<group ids>"],
             grant_type_whitelists=["implicit"])
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Authorization Server Policy Rule can be imported via the Auth Server ID, Policy ID, and Policy Rule ID.
 
         ```sh
         $ pulumi import okta:auth/serverPolicyRule:ServerPolicyRule example &#60;auth server id&#62;/&#60;policy id&#62;/&#60;policy rule id&#62;
@@ -639,29 +637,27 @@
     def __init__(__self__,
                  resource_name: str,
                  args: ServerPolicyRuleArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_okta as okta
 
         example = okta.auth.ServerPolicyRule("example",
             auth_server_id="<auth server id>",
             policy_id="<auth server policy id>",
             status="ACTIVE",
             name="example",
             priority=1,
             group_whitelists=["<group ids>"],
             grant_type_whitelists=["implicit"])
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Authorization Server Policy Rule can be imported via the Auth Server ID, Policy ID, and Policy Rule ID.
 
         ```sh
         $ pulumi import okta:auth/serverPolicyRule:ServerPolicyRule example &#60;auth server id&#62;/&#60;policy id&#62;/&#60;policy rule id&#62;
```

### Comparing `pulumi_okta-4.9.0a1713462165/pulumi_okta/auth/server_scope.py` & `pulumi_okta-4.9.0a1713902092/pulumi_okta/auth/server_scope.py`

 * *Files 2% similar despite different names*

```diff
@@ -315,26 +315,24 @@
         """
         Creates an Authorization Server Scope.
 
         This resource allows you to create and configure an Authorization Server Scope.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_okta as okta
 
         example = okta.auth.ServerScope("example",
             auth_server_id="<auth server id>",
             metadata_publish="NO_CLIENTS",
             name="example",
             consent="IMPLICIT")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Okta Auth Server Scope can be imported via the Auth Server ID and Scope ID.
 
         ```sh
         $ pulumi import okta:auth/serverScope:ServerScope example &#60;auth server id&#62;/&#60;scope id&#62;
@@ -360,26 +358,24 @@
         """
         Creates an Authorization Server Scope.
 
         This resource allows you to create and configure an Authorization Server Scope.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_okta as okta
 
         example = okta.auth.ServerScope("example",
             auth_server_id="<auth server id>",
             metadata_publish="NO_CLIENTS",
             name="example",
             consent="IMPLICIT")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Okta Auth Server Scope can be imported via the Auth Server ID and Scope ID.
 
         ```sh
         $ pulumi import okta:auth/serverScope:ServerScope example &#60;auth server id&#62;/&#60;scope id&#62;
```

### Comparing `pulumi_okta-4.9.0a1713462165/pulumi_okta/auth_server_claim_default.py` & `pulumi_okta-4.9.0a1713902092/pulumi_okta/auth_server_claim_default.py`

 * *Files 2% similar despite different names*

```diff
@@ -239,25 +239,23 @@
         """
         Configures Default Authorization Server Claim.
 
         This resource allows you to configure Default Authorization Server Claims.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_okta as okta
 
         example = okta.AuthServerClaimDefault("example",
             auth_server_id="<auth server id>",
             name="sub",
             value="(appuser != null) ? appuser.userName : app.clientId")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Authorization Server Claim can be imported via the Auth Server ID and Claim ID or Claim Name.
 
         ```sh
         $ pulumi import okta:index/authServerClaimDefault:AuthServerClaimDefault example &#60;auth server id&#62;/&#60;claim id&#62;
@@ -287,25 +285,23 @@
         """
         Configures Default Authorization Server Claim.
 
         This resource allows you to configure Default Authorization Server Claims.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_okta as okta
 
         example = okta.AuthServerClaimDefault("example",
             auth_server_id="<auth server id>",
             name="sub",
             value="(appuser != null) ? appuser.userName : app.clientId")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Authorization Server Claim can be imported via the Auth Server ID and Claim ID or Claim Name.
 
         ```sh
         $ pulumi import okta:index/authServerClaimDefault:AuthServerClaimDefault example &#60;auth server id&#62;/&#60;claim id&#62;
```

### Comparing `pulumi_okta-4.9.0a1713462165/pulumi_okta/auth_server_default.py` & `pulumi_okta-4.9.0a1713902092/pulumi_okta/auth_server_default.py`

 * *Files 0% similar despite different names*

```diff
@@ -298,24 +298,22 @@
         """
         Configures Default Authorization Server.
 
         This resource allows you to configure Default Authorization Server.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_okta as okta
 
         example = okta.AuthServerDefault("example",
             audiences=["api://default"],
             description="Default Authorization Server for your Applications")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Authorization Server can be imported via the Okta ID.
 
         ```sh
         $ pulumi import okta:index/authServerDefault:AuthServerDefault example &#60;default&#62;
@@ -339,24 +337,22 @@
         """
         Configures Default Authorization Server.
 
         This resource allows you to configure Default Authorization Server.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_okta as okta
 
         example = okta.AuthServerDefault("example",
             audiences=["api://default"],
             description="Default Authorization Server for your Applications")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Authorization Server can be imported via the Okta ID.
 
         ```sh
         $ pulumi import okta:index/authServerDefault:AuthServerDefault example &#60;default&#62;
```

### Comparing `pulumi_okta-4.9.0a1713462165/pulumi_okta/authenticator.py` & `pulumi_okta-4.9.0a1713902092/pulumi_okta/authenticator.py`

 * *Files 1% similar despite different names*

```diff
@@ -514,30 +514,27 @@
 
         > **Delete:** Authenticators can not be truly deleted therefore delete is soft.
         Delete will attempt to deativate the authenticator. An authenticator can only be
         deactivated if it's not in use by any other policy.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import json
         import pulumi_okta as okta
 
         test = okta.Authenticator("test",
             name="Security Question",
             key="security_question",
             settings=json.dumps({
                 "allowedFor": "recovery",
             }))
         ```
-        <!--End PulumiCodeChooser -->
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import json
         import pulumi_okta as okta
 
         test = okta.Authenticator("test",
             name="Custom OTP",
@@ -548,15 +545,14 @@
                 "acceptableAdjacentIntervals": 3,
                 "timeIntervalInSeconds": 30,
                 "encoding": "base32",
                 "algorithm": "HMacSHA256",
                 "passCodeLength": 6,
             }))
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Okta authenticator can be imported via the Okta ID.
 
         ```sh
         $ pulumi import okta:index/authenticator:Authenticator example &#60;authenticator_id&#62;
@@ -603,30 +599,27 @@
 
         > **Delete:** Authenticators can not be truly deleted therefore delete is soft.
         Delete will attempt to deativate the authenticator. An authenticator can only be
         deactivated if it's not in use by any other policy.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import json
         import pulumi_okta as okta
 
         test = okta.Authenticator("test",
             name="Security Question",
             key="security_question",
             settings=json.dumps({
                 "allowedFor": "recovery",
             }))
         ```
-        <!--End PulumiCodeChooser -->
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import json
         import pulumi_okta as okta
 
         test = okta.Authenticator("test",
             name="Custom OTP",
@@ -637,15 +630,14 @@
                 "acceptableAdjacentIntervals": 3,
                 "timeIntervalInSeconds": 30,
                 "encoding": "base32",
                 "algorithm": "HMacSHA256",
                 "passCodeLength": 6,
             }))
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Okta authenticator can be imported via the Okta ID.
 
         ```sh
         $ pulumi import okta:index/authenticator:Authenticator example &#60;authenticator_id&#62;
```

### Comparing `pulumi_okta-4.9.0a1713462165/pulumi_okta/behaviour.py` & `pulumi_okta-4.9.0a1713902092/pulumi_okta/behaviour.py`

 * *Files 1% similar despite different names*

```diff
@@ -288,15 +288,14 @@
                  velocity: Optional[pulumi.Input[int]] = None,
                  __props__=None):
         """
         This resource allows you to create and configure a behavior.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_okta as okta
 
         my_location = okta.Behaviour("my_location",
             name="My Location",
             type="ANOMALOUS_LOCATION",
@@ -317,15 +316,14 @@
             type="ANOMALOUS_IP",
             number_of_authentications=50)
         my_velocity = okta.Behaviour("my_velocity",
             name="My Velocity",
             type="VELOCITY",
             velocity=25)
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Behavior can be imported via the Okta ID.
 
         ```sh
         $ pulumi import okta:index/behaviour:Behaviour example &#60;behavior id&#62;
@@ -354,15 +352,14 @@
                  args: BehaviourArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         This resource allows you to create and configure a behavior.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_okta as okta
 
         my_location = okta.Behaviour("my_location",
             name="My Location",
             type="ANOMALOUS_LOCATION",
@@ -383,15 +380,14 @@
             type="ANOMALOUS_IP",
             number_of_authentications=50)
         my_velocity = okta.Behaviour("my_velocity",
             name="My Velocity",
             type="VELOCITY",
             velocity=25)
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Behavior can be imported via the Okta ID.
 
         ```sh
         $ pulumi import okta:index/behaviour:Behaviour example &#60;behavior id&#62;
```

### Comparing `pulumi_okta-4.9.0a1713462165/pulumi_okta/brand.py` & `pulumi_okta-4.9.0a1713902092/pulumi_okta/brand.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713462165/pulumi_okta/captcha.py` & `pulumi_okta-4.9.0a1713902092/pulumi_okta/captcha.py`

 * *Files 2% similar despite different names*

```diff
@@ -165,26 +165,24 @@
         """
         > **WARNING:** This feature is only available as a part of the Identity Engine. Contact support for further information.
 
         This resource allows you to create and configure a CAPTCHA.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_okta as okta
 
         example = okta.Captcha("example",
             name="My CAPTCHA",
             type="HCAPTCHA",
             site_key="some_key",
             secret_key="some_secret_key")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Behavior can be imported via the Okta ID.
 
         ```sh
         $ pulumi import okta:index/captcha:Captcha example &#60;captcha id&#62;
@@ -206,26 +204,24 @@
         """
         > **WARNING:** This feature is only available as a part of the Identity Engine. Contact support for further information.
 
         This resource allows you to create and configure a CAPTCHA.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_okta as okta
 
         example = okta.Captcha("example",
             name="My CAPTCHA",
             type="HCAPTCHA",
             site_key="some_key",
             secret_key="some_secret_key")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Behavior can be imported via the Okta ID.
 
         ```sh
         $ pulumi import okta:index/captcha:Captcha example &#60;captcha id&#62;
```

### Comparing `pulumi_okta-4.9.0a1713462165/pulumi_okta/captcha_org_wide_settings.py` & `pulumi_okta-4.9.0a1713902092/pulumi_okta/captcha_org_wide_settings.py`

 * *Files 9% similar despite different names*

```diff
@@ -103,45 +103,41 @@
         > **WARNING:** This feature is only available as a part of the Identity Engine. Contact support for further information.
 
         This resource allows you to configure which parts of the authentication flow requires users to pass the CAPTCHA logic.
         CAPTCHA org-wide settings can be disabled by unsetting `captcha_id` and `enabled_for`.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_okta as okta
 
         example = okta.Captcha("example",
             name="My CAPTCHA",
             type="HCAPTCHA",
             site_key="some_key",
             secret_key="some_secret_key")
         example_captcha_org_wide_settings = okta.CaptchaOrgWideSettings("example",
             captcha_id=test["id"],
             enabled_fors=["SSR"])
         ```
-        <!--End PulumiCodeChooser -->
 
         The following example disables org-wide CAPTCHA.
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_okta as okta
 
         example = okta.Captcha("example",
             name="My CAPTCHA",
             type="HCAPTCHA",
             site_key="some_key",
             secret_key="some_secret_key")
         example_captcha_org_wide_settings = okta.CaptchaOrgWideSettings("example")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Org-Wide CAPTCHA settings can be imported without any parameters.
 
         ```sh
         $ pulumi import okta:index/captchaOrgWideSettings:CaptchaOrgWideSettings example _
@@ -162,45 +158,41 @@
         > **WARNING:** This feature is only available as a part of the Identity Engine. Contact support for further information.
 
         This resource allows you to configure which parts of the authentication flow requires users to pass the CAPTCHA logic.
         CAPTCHA org-wide settings can be disabled by unsetting `captcha_id` and `enabled_for`.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_okta as okta
 
         example = okta.Captcha("example",
             name="My CAPTCHA",
             type="HCAPTCHA",
             site_key="some_key",
             secret_key="some_secret_key")
         example_captcha_org_wide_settings = okta.CaptchaOrgWideSettings("example",
             captcha_id=test["id"],
             enabled_fors=["SSR"])
         ```
-        <!--End PulumiCodeChooser -->
 
         The following example disables org-wide CAPTCHA.
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_okta as okta
 
         example = okta.Captcha("example",
             name="My CAPTCHA",
             type="HCAPTCHA",
             site_key="some_key",
             secret_key="some_secret_key")
         example_captcha_org_wide_settings = okta.CaptchaOrgWideSettings("example")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Org-Wide CAPTCHA settings can be imported without any parameters.
 
         ```sh
         $ pulumi import okta:index/captchaOrgWideSettings:CaptchaOrgWideSettings example _
```

### Comparing `pulumi_okta-4.9.0a1713462165/pulumi_okta/config/__init__.pyi` & `pulumi_okta-4.9.0a1713902092/pulumi_okta/config/__init__.pyi`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713462165/pulumi_okta/config/vars.py` & `pulumi_okta-4.9.0a1713902092/pulumi_okta/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713462165/pulumi_okta/domain.py` & `pulumi_okta-4.9.0a1713902092/pulumi_okta/domain.py`

 * *Files 2% similar despite different names*

```diff
@@ -175,22 +175,20 @@
                  name: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         Manages custom domain for your organization.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_okta as okta
 
         example = okta.Domain("example", name="www.example.com")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Okta Admin Role Targets can be imported via the Okta ID.
 
         ```sh
         $ pulumi import okta:index/domain:Domain example &#60;domain_id&#62;
@@ -211,22 +209,20 @@
                  args: Optional[DomainArgs] = None,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         Manages custom domain for your organization.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_okta as okta
 
         example = okta.Domain("example", name="www.example.com")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Okta Admin Role Targets can be imported via the Okta ID.
 
         ```sh
         $ pulumi import okta:index/domain:Domain example &#60;domain_id&#62;
```

### Comparing `pulumi_okta-4.9.0a1713462165/pulumi_okta/domain_certificate.py` & `pulumi_okta-4.9.0a1713902092/pulumi_okta/domain_certificate.py`

 * *Files 4% similar despite different names*

```diff
@@ -204,15 +204,14 @@
 
         See Let's Encrypt Certbot notes at the end of this
         documentation for notes on how to generate a domain certificate with Let's
         Encrypt Certbot
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_okta as okta
 
         example = okta.Domain("example", name="www.example.com")
         test = okta.DomainCertificate("test",
             domain_id=test_okta_domain["id"],
@@ -232,15 +231,14 @@
             private_key=\"\"\"-----BEGIN PRIVATE KEY-----
         MIIEvgIBADANBgkqhkiG9w0BAQEFAASCBKgwggSkAgEAAoIBAQC5cyk6x63iBJSW
         ...
         nUFLNE8pXSnsqb0eOL74f3uQ
         -----END PRIVATE KEY-----
         \"\"\")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Let's Encrypt Certbot
 
         This example demonstrates generatoring a domain certificate with letsencrypt
         certbot https://letsencrypt.org/getting-started/
 
         Use letsencrypt's certbot to generate domain certificates in RSA output mode.
@@ -282,15 +280,14 @@
 
         See Let's Encrypt Certbot notes at the end of this
         documentation for notes on how to generate a domain certificate with Let's
         Encrypt Certbot
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_okta as okta
 
         example = okta.Domain("example", name="www.example.com")
         test = okta.DomainCertificate("test",
             domain_id=test_okta_domain["id"],
@@ -310,15 +307,14 @@
             private_key=\"\"\"-----BEGIN PRIVATE KEY-----
         MIIEvgIBADANBgkqhkiG9w0BAQEFAASCBKgwggSkAgEAAoIBAQC5cyk6x63iBJSW
         ...
         nUFLNE8pXSnsqb0eOL74f3uQ
         -----END PRIVATE KEY-----
         \"\"\")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Let's Encrypt Certbot
 
         This example demonstrates generatoring a domain certificate with letsencrypt
         certbot https://letsencrypt.org/getting-started/
 
         Use letsencrypt's certbot to generate domain certificates in RSA output mode.
```

### Comparing `pulumi_okta-4.9.0a1713462165/pulumi_okta/domain_verification.py` & `pulumi_okta-4.9.0a1713902092/pulumi_okta/domain_verification.py`

 * *Files 7% similar despite different names*

```diff
@@ -68,23 +68,21 @@
         """
         Verifies the Domain. This is replacement for the `verify` field from the `Domain` resource. The resource won't be
         created if the domain could not be verified. The provider will make several requests to verify the domain until
         the API returns `VERIFIED` verification status.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_okta as okta
 
         example = okta.Domain("example", name="www.example.com")
         example_domain_verification = okta.DomainVerification("example", domain_id=test["id"])
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         This resource does not support importing.
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
@@ -99,23 +97,21 @@
         """
         Verifies the Domain. This is replacement for the `verify` field from the `Domain` resource. The resource won't be
         created if the domain could not be verified. The provider will make several requests to verify the domain until
         the API returns `VERIFIED` verification status.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_okta as okta
 
         example = okta.Domain("example", name="www.example.com")
         example_domain_verification = okta.DomainVerification("example", domain_id=test["id"])
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         This resource does not support importing.
 
         :param str resource_name: The name of the resource.
         :param DomainVerificationArgs args: The arguments to use to populate this resource's properties.
```

### Comparing `pulumi_okta-4.9.0a1713462165/pulumi_okta/email_customization.py` & `pulumi_okta-4.9.0a1713902092/pulumi_okta/email_customization.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713462165/pulumi_okta/email_sender.py` & `pulumi_okta-4.9.0a1713902092/pulumi_okta/email_sender.py`

 * *Files 5% similar despite different names*

```diff
@@ -166,25 +166,23 @@
         """
         > **DEPRECATED** use `Index.EmailDomain` instead.
 
         This resource allows you to create and configure a custom email sender.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_okta as okta
 
         example = okta.EmailSender("example",
             from_name="Paul Atreides",
             from_address="no-reply@caladan.planet",
             subdomain="mail")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Custom email sender can be imported via the Okta ID.
 
         ```sh
         $ pulumi import okta:index/emailSender:EmailSender example &#60;sender id&#62;
@@ -205,25 +203,23 @@
         """
         > **DEPRECATED** use `Index.EmailDomain` instead.
 
         This resource allows you to create and configure a custom email sender.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_okta as okta
 
         example = okta.EmailSender("example",
             from_name="Paul Atreides",
             from_address="no-reply@caladan.planet",
             subdomain="mail")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Custom email sender can be imported via the Okta ID.
 
         ```sh
         $ pulumi import okta:index/emailSender:EmailSender example &#60;sender id&#62;
```

### Comparing `pulumi_okta-4.9.0a1713462165/pulumi_okta/email_sender_verification.py` & `pulumi_okta-4.9.0a1713902092/pulumi_okta/email_sender_verification.py`

 * *Files 6% similar despite different names*

```diff
@@ -68,26 +68,24 @@
         """
         > **DEPRECATED** use `Index.EmailDomainVerification` instead.
 
         Verifies the email sender. The resource won't be created if the email sender could not be verified.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_okta as okta
 
         example = okta.EmailSender("example",
             from_name="Paul Atreides",
             from_address="no-reply@caladan.planet",
             subdomain="mail")
         example_email_sender_verification = okta.EmailSenderVerification("example", sender_id=valid["id"])
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         This resource does not support importing.
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
@@ -102,26 +100,24 @@
         """
         > **DEPRECATED** use `Index.EmailDomainVerification` instead.
 
         Verifies the email sender. The resource won't be created if the email sender could not be verified.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_okta as okta
 
         example = okta.EmailSender("example",
             from_name="Paul Atreides",
             from_address="no-reply@caladan.planet",
             subdomain="mail")
         example_email_sender_verification = okta.EmailSenderVerification("example", sender_id=valid["id"])
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         This resource does not support importing.
 
         :param str resource_name: The name of the resource.
         :param EmailSenderVerificationArgs args: The arguments to use to populate this resource's properties.
```

### Comparing `pulumi_okta-4.9.0a1713462165/pulumi_okta/event_hook.py` & `pulumi_okta-4.9.0a1713902092/pulumi_okta/event_hook.py`

 * *Files 2% similar despite different names*

```diff
@@ -234,15 +234,14 @@
         """
         Creates an event hook.
 
         This resource allows you to create and configure an event hook.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_okta as okta
 
         example = okta.EventHook("example",
             name="example",
             events=[
@@ -256,15 +255,14 @@
             },
             auth={
                 "type": "HEADER",
                 "key": "Authorization",
                 "value": "123",
             })
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         An event hook can be imported via the Okta ID.
 
         ```sh
         $ pulumi import okta:index/eventHook:EventHook example &#60;hook id&#62;
@@ -288,15 +286,14 @@
         """
         Creates an event hook.
 
         This resource allows you to create and configure an event hook.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_okta as okta
 
         example = okta.EventHook("example",
             name="example",
             events=[
@@ -310,15 +307,14 @@
             },
             auth={
                 "type": "HEADER",
                 "key": "Authorization",
                 "value": "123",
             })
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         An event hook can be imported via the Okta ID.
 
         ```sh
         $ pulumi import okta:index/eventHook:EventHook example &#60;hook id&#62;
```

### Comparing `pulumi_okta-4.9.0a1713462165/pulumi_okta/event_hook_verification.py` & `pulumi_okta-4.9.0a1713902092/pulumi_okta/event_hook_verification.py`

 * *Files 8% similar despite different names*

```diff
@@ -68,15 +68,14 @@
         """
         Verifies the Event Hook. The resource won't be created unless the URI provided in the event hook returns a valid
         JSON object with verification. See [Event Hooks](https://developer.okta.com/docs/concepts/event-hooks/#one-time-verification-request)
         documentation for details.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_okta as okta
 
         example = okta.EventHook("example",
             name="example",
             events=[
@@ -91,15 +90,14 @@
             auth={
                 "type": "HEADER",
                 "key": "Authorization",
                 "value": "123",
             })
         example_event_hook_verification = okta.EventHookVerification("example", event_hook_id=example.id)
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         This resource does not support importing.
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
@@ -114,15 +112,14 @@
         """
         Verifies the Event Hook. The resource won't be created unless the URI provided in the event hook returns a valid
         JSON object with verification. See [Event Hooks](https://developer.okta.com/docs/concepts/event-hooks/#one-time-verification-request)
         documentation for details.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_okta as okta
 
         example = okta.EventHook("example",
             name="example",
             events=[
@@ -137,15 +134,14 @@
             auth={
                 "type": "HEADER",
                 "key": "Authorization",
                 "value": "123",
             })
         example_event_hook_verification = okta.EventHookVerification("example", event_hook_id=example.id)
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         This resource does not support importing.
 
         :param str resource_name: The name of the resource.
         :param EventHookVerificationArgs args: The arguments to use to populate this resource's properties.
```

### Comparing `pulumi_okta-4.9.0a1713462165/pulumi_okta/factor/factor.py` & `pulumi_okta-4.9.0a1713902092/pulumi_okta/factor/factor.py`

 * *Files 2% similar despite different names*

```diff
@@ -105,22 +105,20 @@
         """
         Allows you to manage the activation of Okta MFA methods.
 
         This resource allows you to manage Okta MFA methods.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_okta as okta
 
         example = okta.factor.Factor("example", provider_id="google_otp")
         ```
-        <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[bool] active: Whether to activate the provider, by default, it is set to `true`.
         :param pulumi.Input[str] provider_id: The MFA provider name.
                Allowed values are `"duo"`, `"fido_u2f"`, `"fido_webauthn"`, `"google_otp"`, `"okta_call"`, `"okta_otp"`, `"okta_password"`, `"okta_push"`, `"okta_question"`, `"okta_sms"`, `"okta_email"`, `"rsa_token"`, `"symantec_vip"`, `"yubikey_token"`, or `"hotp"`.
         """
@@ -133,22 +131,20 @@
         """
         Allows you to manage the activation of Okta MFA methods.
 
         This resource allows you to manage Okta MFA methods.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_okta as okta
 
         example = okta.factor.Factor("example", provider_id="google_otp")
         ```
-        <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param FactorArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
```

### Comparing `pulumi_okta-4.9.0a1713462165/pulumi_okta/factor_totp.py` & `pulumi_okta-4.9.0a1713902092/pulumi_okta/factor_totp.py`

 * *Files 1% similar despite different names*

```diff
@@ -249,28 +249,26 @@
         mobile app authenticators.
 
         Once saved, the settings cannot be changed (except for the `name` field). Any other change would force resource
         recreation.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_okta as okta
 
         example = okta.FactorTotp("example",
             name="example",
             otp_length=10,
             hmac_algorithm="HMacSHA256",
             time_step=30,
             clock_drift_interval=10,
             shared_secret_encoding="hexadecimal")
         ```
-        <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[int] clock_drift_interval: Clock drift interval. This setting allows you to build in tolerance for any
                drift between the token's current time and the server's current time. Valid values: `3`, `5`, `10`. Default is `3`.
         :param pulumi.Input[str] hmac_algorithm: HMAC Algorithm. Valid values: `"HMacSHA1"`, `"HMacSHA256"`, `"HMacSHA512"`. Default
                is `"HMacSHA512"`.
@@ -292,28 +290,26 @@
         mobile app authenticators.
 
         Once saved, the settings cannot be changed (except for the `name` field). Any other change would force resource
         recreation.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_okta as okta
 
         example = okta.FactorTotp("example",
             name="example",
             otp_length=10,
             hmac_algorithm="HMacSHA256",
             time_step=30,
             clock_drift_interval=10,
             shared_secret_encoding="hexadecimal")
         ```
-        <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param FactorTotpArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
```

### Comparing `pulumi_okta-4.9.0a1713462165/pulumi_okta/get_app_group_assignments.py` & `pulumi_okta-4.9.0a1713902092/pulumi_okta/get_app_group_assignments.py`

 * *Files 4% similar despite different names*

```diff
@@ -59,22 +59,20 @@
 def get_app_group_assignments(id: Optional[str] = None,
                               opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetAppGroupAssignmentsResult:
     """
     Use this data source to retrieve the list of groups assigned to the given Okta application (by ID).
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_okta as okta
 
     test = okta.get_app_group_assignments(id=test_okta_app_oauth["id"])
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str id: The ID of the Okta application you want to retrieve the groups for.
     """
     __args__ = dict()
     __args__['id'] = id
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
@@ -89,20 +87,18 @@
 def get_app_group_assignments_output(id: Optional[pulumi.Input[str]] = None,
                                      opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetAppGroupAssignmentsResult]:
     """
     Use this data source to retrieve the list of groups assigned to the given Okta application (by ID).
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_okta as okta
 
     test = okta.get_app_group_assignments(id=test_okta_app_oauth["id"])
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str id: The ID of the Okta application you want to retrieve the groups for.
     """
     ...
```

### Comparing `pulumi_okta-4.9.0a1713462165/pulumi_okta/get_app_signon_policy.py` & `pulumi_okta-4.9.0a1713902092/pulumi_okta/get_app_signon_policy.py`

 * *Files 6% similar despite different names*

```diff
@@ -71,22 +71,20 @@
 
     > Inside the product a sign-on policy is referenced as an _authentication
     policy_, in the public API the policy is of type
     [`ACCESS_POLICY`](https://developer.okta.com/docs/reference/api/policy/#policy-object).
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_okta as okta
 
     example = okta.get_app_signon_policy(app_id="app_id")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str app_id: The application ID.
     """
     __args__ = dict()
     __args__['appId'] = app_id
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
@@ -108,20 +106,18 @@
 
     > Inside the product a sign-on policy is referenced as an _authentication
     policy_, in the public API the policy is of type
     [`ACCESS_POLICY`](https://developer.okta.com/docs/reference/api/policy/#policy-object).
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_okta as okta
 
     example = okta.get_app_signon_policy(app_id="app_id")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str app_id: The application ID.
     """
     ...
```

### Comparing `pulumi_okta-4.9.0a1713462165/pulumi_okta/get_app_user_assignments.py` & `pulumi_okta-4.9.0a1713902092/pulumi_okta/get_app_user_assignments.py`

 * *Files 6% similar despite different names*

```diff
@@ -59,22 +59,20 @@
 def get_app_user_assignments(id: Optional[str] = None,
                              opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetAppUserAssignmentsResult:
     """
     Use this data source to retrieve the list of users assigned to the given Okta application (by ID).
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_okta as okta
 
     test = okta.get_app_user_assignments(id=test_okta_app_oauth["id"])
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str id: The ID of the Okta application you want to retrieve the groups for.
     """
     __args__ = dict()
     __args__['id'] = id
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
@@ -89,20 +87,18 @@
 def get_app_user_assignments_output(id: Optional[pulumi.Input[str]] = None,
                                     opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetAppUserAssignmentsResult]:
     """
     Use this data source to retrieve the list of users assigned to the given Okta application (by ID).
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_okta as okta
 
     test = okta.get_app_user_assignments(id=test_okta_app_oauth["id"])
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str id: The ID of the Okta application you want to retrieve the groups for.
     """
     ...
```

### Comparing `pulumi_okta-4.9.0a1713462165/pulumi_okta/get_auth_server_claim.py` & `pulumi_okta-4.9.0a1713902092/pulumi_okta/get_auth_server_claim.py`

 * *Files 1% similar despite different names*

```diff
@@ -142,23 +142,21 @@
                           name: Optional[str] = None,
                           opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetAuthServerClaimResult:
     """
     Use this data source to retrieve authorization server claim from Okta.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_okta as okta
 
     test = okta.get_auth_server_claim(auth_server_id="default",
         name="birthdate")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str auth_server_id: Auth server ID.
     :param str id: ID of the claim. Conflicts with `name`.
     :param str name: Name of the claim. Conflicts with `id`.
     """
     __args__ = dict()
@@ -186,23 +184,21 @@
                                  name: Optional[pulumi.Input[Optional[str]]] = None,
                                  opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetAuthServerClaimResult]:
     """
     Use this data source to retrieve authorization server claim from Okta.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_okta as okta
 
     test = okta.get_auth_server_claim(auth_server_id="default",
         name="birthdate")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str auth_server_id: Auth server ID.
     :param str id: ID of the claim. Conflicts with `name`.
     :param str name: Name of the claim. Conflicts with `id`.
     """
     ...
```

### Comparing `pulumi_okta-4.9.0a1713462165/pulumi_okta/get_auth_server_claims.py` & `pulumi_okta-4.9.0a1713902092/pulumi_okta/get_auth_server_claims.py`

 * *Files 3% similar despite different names*

```diff
@@ -69,22 +69,20 @@
 def get_auth_server_claims(auth_server_id: Optional[str] = None,
                            opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetAuthServerClaimsResult:
     """
     Use this data source to retrieve a list of authorization server claims from Okta.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_okta as okta
 
     test = okta.get_auth_server_claims(auth_server_id="default")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str auth_server_id: Auth server ID.
     """
     __args__ = dict()
     __args__['authServerId'] = auth_server_id
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
@@ -100,20 +98,18 @@
 def get_auth_server_claims_output(auth_server_id: Optional[pulumi.Input[str]] = None,
                                   opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetAuthServerClaimsResult]:
     """
     Use this data source to retrieve a list of authorization server claims from Okta.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_okta as okta
 
     test = okta.get_auth_server_claims(auth_server_id="default")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str auth_server_id: Auth server ID.
     """
     ...
```

### Comparing `pulumi_okta-4.9.0a1713462165/pulumi_okta/get_authenticator.py` & `pulumi_okta-4.9.0a1713902092/pulumi_okta/get_authenticator.py`

 * *Files 8% similar despite different names*

```diff
@@ -177,31 +177,27 @@
     """
     > **WARNING:** This feature is only available as a part of the Identity Engine. Contact support for further information.
 
     Use this data source to retrieve an authenticator.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_okta as okta
 
     test = okta.get_authenticator(name="Security Question")
     ```
-    <!--End PulumiCodeChooser -->
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_okta as okta
 
     test = okta.get_authenticator(key="okta_email")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str id: ID of the authenticator.
     :param str key: A human-readable string that identifies the authenticator.
     :param str name: Name of the authenticator.
     """
     __args__ = dict()
@@ -234,31 +230,27 @@
     """
     > **WARNING:** This feature is only available as a part of the Identity Engine. Contact support for further information.
 
     Use this data source to retrieve an authenticator.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_okta as okta
 
     test = okta.get_authenticator(name="Security Question")
     ```
-    <!--End PulumiCodeChooser -->
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_okta as okta
 
     test = okta.get_authenticator(key="okta_email")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str id: ID of the authenticator.
     :param str key: A human-readable string that identifies the authenticator.
     :param str name: Name of the authenticator.
     """
     ...
```

### Comparing `pulumi_okta-4.9.0a1713462165/pulumi_okta/get_behaviour.py` & `pulumi_okta-4.9.0a1713902092/pulumi_okta/get_behaviour.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713462165/pulumi_okta/get_behaviours.py` & `pulumi_okta-4.9.0a1713902092/pulumi_okta/get_behaviours.py`

 * *Files 6% similar despite different names*

```diff
@@ -69,22 +69,20 @@
 def get_behaviours(q: Optional[str] = None,
                    opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetBehavioursResult:
     """
     Use this data source to retrieve a behaviors from Okta.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_okta as okta
 
     example = okta.get_behaviours(q="New")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str q: Searches query to look up behaviors.
     """
     __args__ = dict()
     __args__['q'] = q
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
@@ -100,20 +98,18 @@
 def get_behaviours_output(q: Optional[pulumi.Input[Optional[str]]] = None,
                           opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetBehavioursResult]:
     """
     Use this data source to retrieve a behaviors from Okta.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_okta as okta
 
     example = okta.get_behaviours(q="New")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str q: Searches query to look up behaviors.
     """
     ...
```

### Comparing `pulumi_okta-4.9.0a1713462165/pulumi_okta/get_brand.py` & `pulumi_okta-4.9.0a1713902092/pulumi_okta/get_brand.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713462165/pulumi_okta/get_brands.py` & `pulumi_okta-4.9.0a1713902092/pulumi_okta/get_brands.py`

 * *Files 4% similar despite different names*

```diff
@@ -59,22 +59,20 @@
 
 def get_brands(opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetBrandsResult:
     """
     Use this data source to retrieve the brands belonging to an Okta organization.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_okta as okta
 
     test = okta.get_brands()
     ```
-    <!--End PulumiCodeChooser -->
     """
     __args__ = dict()
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('okta:index/getBrands:getBrands', __args__, opts=opts, typ=GetBrandsResult).value
 
     return AwaitableGetBrandsResult(
         brands=pulumi.get(__ret__, 'brands'),
@@ -84,17 +82,15 @@
 @_utilities.lift_output_func(get_brands)
 def get_brands_output(opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetBrandsResult]:
     """
     Use this data source to retrieve the brands belonging to an Okta organization.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_okta as okta
 
     test = okta.get_brands()
     ```
-    <!--End PulumiCodeChooser -->
     """
     ...
```

### Comparing `pulumi_okta-4.9.0a1713462165/pulumi_okta/get_email_customization.py` & `pulumi_okta-4.9.0a1713902092/pulumi_okta/get_email_customization.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713462165/pulumi_okta/get_email_customizations.py` & `pulumi_okta-4.9.0a1713902092/pulumi_okta/get_email_customizations.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713462165/pulumi_okta/get_groups.py` & `pulumi_okta-4.9.0a1713902092/pulumi_okta/get_groups.py`

 * *Files 3% similar despite different names*

```diff
@@ -92,22 +92,20 @@
                type: Optional[str] = None,
                opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetGroupsResult:
     """
     Use this data source to retrieve a list of groups from Okta.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_okta as okta
 
     example = okta.get_groups(q="Engineering - ")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str q: Searches the name property of groups for matching value.
     :param str search: Searches for groups with a
            supported [filtering](https://developer.okta.com/docs/reference/api-overview/#filtering) expression for
            all [attributes](https://developer.okta.com/docs/reference/api/groups/#group-attributes)
            except for `"_embedded"`, `"_links"`, and `"objectClass"`
@@ -135,22 +133,20 @@
                       type: Optional[pulumi.Input[Optional[str]]] = None,
                       opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetGroupsResult]:
     """
     Use this data source to retrieve a list of groups from Okta.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_okta as okta
 
     example = okta.get_groups(q="Engineering - ")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str q: Searches the name property of groups for matching value.
     :param str search: Searches for groups with a
            supported [filtering](https://developer.okta.com/docs/reference/api-overview/#filtering) expression for
            all [attributes](https://developer.okta.com/docs/reference/api/groups/#group-attributes)
            except for `"_embedded"`, `"_links"`, and `"objectClass"`
```

### Comparing `pulumi_okta-4.9.0a1713462165/pulumi_okta/get_network_zone.py` & `pulumi_okta-4.9.0a1713902092/pulumi_okta/get_network_zone.py`

 * *Files 2% similar despite different names*

```diff
@@ -156,22 +156,20 @@
                      name: Optional[str] = None,
                      opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetNetworkZoneResult:
     """
     Use this data source to retrieve a network zone from Okta.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_okta as okta
 
     example = okta.get_network_zone(name="Block Antarctica")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str id: ID of the network zone to retrieve, conflicts with `name`.
     :param str name: Name of the network zone to retrieve, conflicts with `id`.
     """
     __args__ = dict()
     __args__['id'] = id
@@ -197,21 +195,19 @@
                             name: Optional[pulumi.Input[Optional[str]]] = None,
                             opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetNetworkZoneResult]:
     """
     Use this data source to retrieve a network zone from Okta.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_okta as okta
 
     example = okta.get_network_zone(name="Block Antarctica")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str id: ID of the network zone to retrieve, conflicts with `name`.
     :param str name: Name of the network zone to retrieve, conflicts with `id`.
     """
     ...
```

### Comparing `pulumi_okta-4.9.0a1713462165/pulumi_okta/get_role_subscription.py` & `pulumi_okta-4.9.0a1713902092/pulumi_okta/get_role_subscription.py`

 * *Files 3% similar despite different names*

```diff
@@ -78,23 +78,21 @@
                           role_type: Optional[str] = None,
                           opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetRoleSubscriptionResult:
     """
     Use this data source to retrieve role subscription with a specific type.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_okta as okta
 
     example = okta.get_role_subscription(notification_type="APP_IMPORT",
         role_type="SUPER_ADMIN")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str notification_type: Type of the notification. Valid values: `"CONNECTOR_AGENT"`, `"USER_LOCKED_OUT"`, 
            `"APP_IMPORT"`, `"LDAP_AGENT"`, `"AD_AGENT"`, `"OKTA_ANNOUNCEMENT"`, `"OKTA_ISSUE"`, `"OKTA_UPDATE"`, `"IWA_AGENT"`,
            `"USER_DEPROVISION"`, `"REPORT_SUSPICIOUS_ACTIVITY"`, `"RATELIMIT_NOTIFICATION"`.
     :param str role_type: Type of the role. Valid values:
            `"API_ACCESS_MANAGEMENT_ADMIN"`,
@@ -128,23 +126,21 @@
                                  role_type: Optional[pulumi.Input[str]] = None,
                                  opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetRoleSubscriptionResult]:
     """
     Use this data source to retrieve role subscription with a specific type.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_okta as okta
 
     example = okta.get_role_subscription(notification_type="APP_IMPORT",
         role_type="SUPER_ADMIN")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str notification_type: Type of the notification. Valid values: `"CONNECTOR_AGENT"`, `"USER_LOCKED_OUT"`, 
            `"APP_IMPORT"`, `"LDAP_AGENT"`, `"AD_AGENT"`, `"OKTA_ANNOUNCEMENT"`, `"OKTA_ISSUE"`, `"OKTA_UPDATE"`, `"IWA_AGENT"`,
            `"USER_DEPROVISION"`, `"REPORT_SUSPICIOUS_ACTIVITY"`, `"RATELIMIT_NOTIFICATION"`.
     :param str role_type: Type of the role. Valid values:
            `"API_ACCESS_MANAGEMENT_ADMIN"`,
```

### Comparing `pulumi_okta-4.9.0a1713462165/pulumi_okta/get_template.py` & `pulumi_okta-4.9.0a1713902092/pulumi_okta/get_template.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713462165/pulumi_okta/get_templates.py` & `pulumi_okta-4.9.0a1713902092/pulumi_okta/get_templates.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713462165/pulumi_okta/get_theme.py` & `pulumi_okta-4.9.0a1713902092/pulumi_okta/get_theme.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713462165/pulumi_okta/get_themes.py` & `pulumi_okta-4.9.0a1713902092/pulumi_okta/get_themes.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713462165/pulumi_okta/get_trusted_origins.py` & `pulumi_okta-4.9.0a1713902092/pulumi_okta/get_trusted_origins.py`

 * *Files 12% similar despite different names*

```diff
@@ -66,22 +66,20 @@
 def get_trusted_origins(filter: Optional[str] = None,
                         opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetTrustedOriginsResult:
     """
     This resource allows you to retrieve a list of trusted origins from Okta.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_okta as okta
 
     all = okta.get_trusted_origins()
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str filter: Filter criteria (will be URL-encoded by the provider). See [Filtering](https://developer.okta.com/docs/reference/core-okta-api/#filter) for more information on the expressions used in filtering.
     """
     __args__ = dict()
     __args__['filter'] = filter
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
@@ -97,20 +95,18 @@
 def get_trusted_origins_output(filter: Optional[pulumi.Input[Optional[str]]] = None,
                                opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetTrustedOriginsResult]:
     """
     This resource allows you to retrieve a list of trusted origins from Okta.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_okta as okta
 
     all = okta.get_trusted_origins()
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str filter: Filter criteria (will be URL-encoded by the provider). See [Filtering](https://developer.okta.com/docs/reference/core-okta-api/#filter) for more information on the expressions used in filtering.
     """
     ...
```

### Comparing `pulumi_okta-4.9.0a1713462165/pulumi_okta/get_user_security_questions.py` & `pulumi_okta-4.9.0a1713902092/pulumi_okta/get_user_security_questions.py`

 * *Files 12% similar despite different names*

```diff
@@ -69,27 +69,25 @@
 def get_user_security_questions(user_id: Optional[str] = None,
                                 opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetUserSecurityQuestionsResult:
     """
     Use this data source to retrieve a list of user's security questions.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_okta as okta
 
     example_user = okta.user.User("example",
         first_name="John",
         last_name="Smith",
         login="john.smith@example.com",
         email="john.smith@example.com")
     example = okta.get_user_security_questions_output(user_id=example_user.id)
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str user_id: User ID.
     """
     __args__ = dict()
     __args__['userId'] = user_id
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
@@ -105,25 +103,23 @@
 def get_user_security_questions_output(user_id: Optional[pulumi.Input[str]] = None,
                                        opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetUserSecurityQuestionsResult]:
     """
     Use this data source to retrieve a list of user's security questions.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_okta as okta
 
     example_user = okta.user.User("example",
         first_name="John",
         last_name="Smith",
         login="john.smith@example.com",
         email="john.smith@example.com")
     example = okta.get_user_security_questions_output(user_id=example_user.id)
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str user_id: User ID.
     """
     ...
```

### Comparing `pulumi_okta-4.9.0a1713462165/pulumi_okta/group/get_everyone_group.py` & `pulumi_okta-4.9.0a1713902092/pulumi_okta/group/get_everyone_group.py`

 * *Files 7% similar despite different names*

```diff
@@ -69,22 +69,20 @@
                        opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetEveryoneGroupResult:
     """
     Use this data source to retrieve the `Everyone` group from Okta. The same can be achieved with the `group.Group` data
     source with `name = "Everyone"`. This is simply a shortcut.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_okta as okta
 
     example = okta.group.get_everyone_group()
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param bool include_users: whether to retrieve all member ids.
     """
     __args__ = dict()
     __args__['includeUsers'] = include_users
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
@@ -101,20 +99,18 @@
                               opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetEveryoneGroupResult]:
     """
     Use this data source to retrieve the `Everyone` group from Okta. The same can be achieved with the `group.Group` data
     source with `name = "Everyone"`. This is simply a shortcut.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_okta as okta
 
     example = okta.group.get_everyone_group()
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param bool include_users: whether to retrieve all member ids.
     """
     ...
```

### Comparing `pulumi_okta-4.9.0a1713462165/pulumi_okta/group/get_group.py` & `pulumi_okta-4.9.0a1713902092/pulumi_okta/group/get_group.py`

 * *Files 2% similar despite different names*

```diff
@@ -117,22 +117,20 @@
               type: Optional[str] = None,
               opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetGroupResult:
     """
     Use this data source to retrieve a group from Okta.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_okta as okta
 
     example = okta.group.get_group(name="Example App")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str delay_read_seconds: Force delay of the group read by N seconds. Useful when eventual consistency of group information needs to be allowed for; for instance, when group rules are known to have been applied.
     :param str id: ID of the group. Conflicts with `"name"` and `"type"`.
     :param bool include_users: whether to retrieve all member ids.
     :param str name: name of group to retrieve. 
            
@@ -167,22 +165,20 @@
                      type: Optional[pulumi.Input[Optional[str]]] = None,
                      opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetGroupResult]:
     """
     Use this data source to retrieve a group from Okta.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_okta as okta
 
     example = okta.group.get_group(name="Example App")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str delay_read_seconds: Force delay of the group read by N seconds. Useful when eventual consistency of group information needs to be allowed for; for instance, when group rules are known to have been applied.
     :param str id: ID of the group. Conflicts with `"name"` and `"type"`.
     :param bool include_users: whether to retrieve all member ids.
     :param str name: name of group to retrieve.
```

### Comparing `pulumi_okta-4.9.0a1713462165/pulumi_okta/group/get_rule.py` & `pulumi_okta-4.9.0a1713902092/pulumi_okta/group/get_rule.py`

 * *Files 5% similar despite different names*

```diff
@@ -121,22 +121,20 @@
              status: Optional[str] = None,
              opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetRuleResult:
     """
     Use this data source to retrieve a group rule from Okta.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_okta as okta
 
     test = okta.group.get_rule(id=example["id"])
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str id: The ID of the group rule to retrieve.
     :param str name: The name of the Group Rule to retrieve.
     :param str status: The status of the group rule.
     """
     __args__ = dict()
@@ -162,22 +160,20 @@
                     status: Optional[pulumi.Input[Optional[str]]] = None,
                     opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetRuleResult]:
     """
     Use this data source to retrieve a group rule from Okta.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_okta as okta
 
     test = okta.group.get_rule(id=example["id"])
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str id: The ID of the group rule to retrieve.
     :param str name: The name of the Group Rule to retrieve.
     :param str status: The status of the group rule.
     """
     ...
```

### Comparing `pulumi_okta-4.9.0a1713462165/pulumi_okta/group/group.py` & `pulumi_okta-4.9.0a1713902092/pulumi_okta/group/group.py`

 * *Files 2% similar despite different names*

```diff
@@ -180,42 +180,38 @@
         """
         Creates an Okta Group.
 
         This resource allows you to create and configure an Okta Group.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_okta as okta
 
         example = okta.group.Group("example",
             name="Example",
             description="My Example Group")
         ```
-        <!--End PulumiCodeChooser -->
 
         Custom profile attributes
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import json
         import pulumi_okta as okta
 
         example = okta.group.Group("example",
             name="Example",
             description="My Example Group",
             custom_profile_attributes=json.dumps({
                 "example1": "testing1234",
                 "example2": True,
                 "example3": 54321,
             }))
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         An Okta Group can be imported via the Okta ID.
 
         ```sh
         $ pulumi import okta:group/group:Group example &#60;group id&#62;
@@ -237,42 +233,38 @@
         """
         Creates an Okta Group.
 
         This resource allows you to create and configure an Okta Group.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_okta as okta
 
         example = okta.group.Group("example",
             name="Example",
             description="My Example Group")
         ```
-        <!--End PulumiCodeChooser -->
 
         Custom profile attributes
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import json
         import pulumi_okta as okta
 
         example = okta.group.Group("example",
             name="Example",
             description="My Example Group",
             custom_profile_attributes=json.dumps({
                 "example1": "testing1234",
                 "example2": True,
                 "example3": 54321,
             }))
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         An Okta Group can be imported via the Okta ID.
 
         ```sh
         $ pulumi import okta:group/group:Group example &#60;group id&#62;
```

### Comparing `pulumi_okta-4.9.0a1713462165/pulumi_okta/group/role.py` & `pulumi_okta-4.9.0a1713902092/pulumi_okta/group/role.py`

 * *Files 2% similar despite different names*

```diff
@@ -280,24 +280,22 @@
         Assigns Admin roles to Okta Groups.
 
         This resource allows you to assign Okta administrator roles to Okta Groups. This resource provides a one-to-one
         interface between the Okta group and the admin role.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_okta as okta
 
         example = okta.group.Role("example",
             group_id="<group id>",
             role_type="READ_ONLY_ADMIN")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Individual admin role assignment can be imported by passing the group and role assignment IDs as follows:
 
         ```sh
         $ pulumi import okta:group/role:Role example &#60;group id&#62;/&#60;role id&#62;
@@ -341,24 +339,22 @@
         Assigns Admin roles to Okta Groups.
 
         This resource allows you to assign Okta administrator roles to Okta Groups. This resource provides a one-to-one
         interface between the Okta group and the admin role.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_okta as okta
 
         example = okta.group.Role("example",
             group_id="<group id>",
             role_type="READ_ONLY_ADMIN")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Individual admin role assignment can be imported by passing the group and role assignment IDs as follows:
 
         ```sh
         $ pulumi import okta:group/role:Role example &#60;group id&#62;/&#60;role id&#62;
```

### Comparing `pulumi_okta-4.9.0a1713462165/pulumi_okta/group/rule.py` & `pulumi_okta-4.9.0a1713902092/pulumi_okta/group/rule.py`

 * *Files 1% similar despite different names*

```diff
@@ -269,27 +269,25 @@
                  remove_assigned_users: Optional[pulumi.Input[bool]] = None,
                  status: Optional[pulumi.Input[str]] = None,
                  users_excludeds: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  __props__=None):
         """
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_okta as okta
 
         example = okta.group.Rule("example",
             name="example",
             status="ACTIVE",
             group_assignments=["<group id>"],
             expression_type="urn:okta:expression:1.0",
             expression_value="String.startsWith(user.firstName,\\"andy\\")")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         An Okta Group Rule can be imported via the Okta ID.
 
         ```sh
         $ pulumi import okta:group/rule:Rule example &#60;group rule id&#62;
@@ -312,27 +310,25 @@
     def __init__(__self__,
                  resource_name: str,
                  args: RuleArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_okta as okta
 
         example = okta.group.Rule("example",
             name="example",
             status="ACTIVE",
             group_assignments=["<group id>"],
             expression_type="urn:okta:expression:1.0",
             expression_value="String.startsWith(user.firstName,\\"andy\\")")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         An Okta Group Rule can be imported via the Okta ID.
 
         ```sh
         $ pulumi import okta:group/rule:Rule example &#60;group rule id&#62;
```

### Comparing `pulumi_okta-4.9.0a1713462165/pulumi_okta/group_memberships.py` & `pulumi_okta-4.9.0a1713902092/pulumi_okta/group_memberships.py`

 * *Files 1% similar despite different names*

```diff
@@ -142,30 +142,28 @@
         state of user ids that are assigned it. This behavior will signal drift only if
         those users stop being part of the group. If the desired behavior is track all
         users that are added/removed from the group make use of the `track_all_users`
         argument with this resource.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_okta as okta
 
         test = okta.group.Group("test",
             name="testAcc_replace_with_uuid",
             description="testing, testing")
         test_group_memberships = okta.GroupMemberships("test",
             group_id=test.id,
             users=[
                 test1["id"],
                 test2["id"],
             ])
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         an Okta Group's memberships can be imported via the Okta group ID.
 
         ```sh
         $ pulumi import okta:index/groupMemberships:GroupMemberships test &#60;group id&#62;
@@ -201,30 +199,28 @@
         state of user ids that are assigned it. This behavior will signal drift only if
         those users stop being part of the group. If the desired behavior is track all
         users that are added/removed from the group make use of the `track_all_users`
         argument with this resource.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_okta as okta
 
         test = okta.group.Group("test",
             name="testAcc_replace_with_uuid",
             description="testing, testing")
         test_group_memberships = okta.GroupMemberships("test",
             group_id=test.id,
             users=[
                 test1["id"],
                 test2["id"],
             ])
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         an Okta Group's memberships can be imported via the Okta group ID.
 
         ```sh
         $ pulumi import okta:index/groupMemberships:GroupMemberships test &#60;group id&#62;
```

### Comparing `pulumi_okta-4.9.0a1713462165/pulumi_okta/group_schema_property.py` & `pulumi_okta-4.9.0a1713902092/pulumi_okta/group_schema_property.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,16 +34,16 @@
                  permissions: Optional[pulumi.Input[str]] = None,
                  required: Optional[pulumi.Input[bool]] = None,
                  scope: Optional[pulumi.Input[str]] = None,
                  unique: Optional[pulumi.Input[str]] = None):
         """
         The set of arguments for constructing a GroupSchemaProperty resource.
         :param pulumi.Input[str] index: The property name.
-        :param pulumi.Input[str] title: display name for the enum value.
-        :param pulumi.Input[str] type: Type of profile source.
+        :param pulumi.Input[str] title: The display name.
+        :param pulumi.Input[str] type: The type of the schema property. It can be `"string"`, `"boolean"`, `"number"`, `"integer"`, `"array"`, or `"object"`.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] array_enums: Array of values that an array property's items can be set to.
         :param pulumi.Input[Sequence[pulumi.Input['GroupSchemaPropertyArrayOneOfArgs']]] array_one_ofs: Display name and value an enum array can be set to.
         :param pulumi.Input[str] array_type: The type of the array elements if `type` is set to `"array"`.
         :param pulumi.Input[str] description: The description of the group schema property.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] enums: Array of values a primitive property can be set to. See `array_enum` for arrays.
         :param pulumi.Input[str] external_name: External name of the group schema property.
         :param pulumi.Input[str] external_namespace: External name of the group schema property.
@@ -105,27 +105,27 @@
     def index(self, value: pulumi.Input[str]):
         pulumi.set(self, "index", value)
 
     @property
     @pulumi.getter
     def title(self) -> pulumi.Input[str]:
         """
-        display name for the enum value.
+        The display name.
         """
         return pulumi.get(self, "title")
 
     @title.setter
     def title(self, value: pulumi.Input[str]):
         pulumi.set(self, "title", value)
 
     @property
     @pulumi.getter
     def type(self) -> pulumi.Input[str]:
         """
-        Type of profile source.
+        The type of the schema property. It can be `"string"`, `"boolean"`, `"number"`, `"integer"`, `"array"`, or `"object"`.
         """
         return pulumi.get(self, "type")
 
     @type.setter
     def type(self, value: pulumi.Input[str]):
         pulumi.set(self, "type", value)
 
@@ -358,16 +358,16 @@
         :param pulumi.Input[Sequence[pulumi.Input['GroupSchemaPropertyMasterOverridePriorityArgs']]] master_override_priorities: Prioritized list of profile sources (required when `master` is `"OVERRIDE"`).
         :param pulumi.Input[int] max_length: The maximum length of the group property value. Only applies to type `"string"`.
         :param pulumi.Input[int] min_length: The minimum length of the group property value. Only applies to type `"string"`.
         :param pulumi.Input[Sequence[pulumi.Input['GroupSchemaPropertyOneOfArgs']]] one_ofs: Array of maps containing a mapping for display name to enum value.
         :param pulumi.Input[str] permissions: Access control permissions for the property. It can be set to `"READ_WRITE"`, `"READ_ONLY"`, `"HIDE"`.
         :param pulumi.Input[bool] required: Whether the property is required for this group.
         :param pulumi.Input[str] scope: determines whether an app user attribute can be set at the Individual or Group Level.
-        :param pulumi.Input[str] title: display name for the enum value.
-        :param pulumi.Input[str] type: Type of profile source.
+        :param pulumi.Input[str] title: The display name.
+        :param pulumi.Input[str] type: The type of the schema property. It can be `"string"`, `"boolean"`, `"number"`, `"integer"`, `"array"`, or `"object"`.
         :param pulumi.Input[str] unique: Whether the property should be unique. It can be set to `"UNIQUE_VALIDATED"` or `"NOT_UNIQUE"`.
         """
         if array_enums is not None:
             pulumi.set(__self__, "array_enums", array_enums)
         if array_one_ofs is not None:
             pulumi.set(__self__, "array_one_ofs", array_one_ofs)
         if array_type is not None:
@@ -597,27 +597,27 @@
     def scope(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "scope", value)
 
     @property
     @pulumi.getter
     def title(self) -> Optional[pulumi.Input[str]]:
         """
-        display name for the enum value.
+        The display name.
         """
         return pulumi.get(self, "title")
 
     @title.setter
     def title(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "title", value)
 
     @property
     @pulumi.getter
     def type(self) -> Optional[pulumi.Input[str]]:
         """
-        Type of profile source.
+        The type of the schema property. It can be `"string"`, `"boolean"`, `"number"`, `"integer"`, `"array"`, or `"object"`.
         """
         return pulumi.get(self, "type")
 
     @type.setter
     def type(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "type", value)
 
@@ -658,28 +658,26 @@
                  title: Optional[pulumi.Input[str]] = None,
                  type: Optional[pulumi.Input[str]] = None,
                  unique: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_okta as okta
 
         example = okta.GroupSchemaProperty("example",
             index="customPropertyName",
             title="customPropertyName",
             type="string",
             description="My custom property name",
             master="OKTA",
             scope="SELF")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Group schema property can be imported via the property index.
 
         ```sh
         $ pulumi import okta:index/groupSchemaProperty:GroupSchemaProperty example &#60;index&#62;
@@ -699,41 +697,39 @@
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['GroupSchemaPropertyMasterOverridePriorityArgs']]]] master_override_priorities: Prioritized list of profile sources (required when `master` is `"OVERRIDE"`).
         :param pulumi.Input[int] max_length: The maximum length of the group property value. Only applies to type `"string"`.
         :param pulumi.Input[int] min_length: The minimum length of the group property value. Only applies to type `"string"`.
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['GroupSchemaPropertyOneOfArgs']]]] one_ofs: Array of maps containing a mapping for display name to enum value.
         :param pulumi.Input[str] permissions: Access control permissions for the property. It can be set to `"READ_WRITE"`, `"READ_ONLY"`, `"HIDE"`.
         :param pulumi.Input[bool] required: Whether the property is required for this group.
         :param pulumi.Input[str] scope: determines whether an app user attribute can be set at the Individual or Group Level.
-        :param pulumi.Input[str] title: display name for the enum value.
-        :param pulumi.Input[str] type: Type of profile source.
+        :param pulumi.Input[str] title: The display name.
+        :param pulumi.Input[str] type: The type of the schema property. It can be `"string"`, `"boolean"`, `"number"`, `"integer"`, `"array"`, or `"object"`.
         :param pulumi.Input[str] unique: Whether the property should be unique. It can be set to `"UNIQUE_VALIDATED"` or `"NOT_UNIQUE"`.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: GroupSchemaPropertyArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_okta as okta
 
         example = okta.GroupSchemaProperty("example",
             index="customPropertyName",
             title="customPropertyName",
             type="string",
             description="My custom property name",
             master="OKTA",
             scope="SELF")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Group schema property can be imported via the property index.
 
         ```sh
         $ pulumi import okta:index/groupSchemaProperty:GroupSchemaProperty example &#60;index&#62;
@@ -855,16 +851,16 @@
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['GroupSchemaPropertyMasterOverridePriorityArgs']]]] master_override_priorities: Prioritized list of profile sources (required when `master` is `"OVERRIDE"`).
         :param pulumi.Input[int] max_length: The maximum length of the group property value. Only applies to type `"string"`.
         :param pulumi.Input[int] min_length: The minimum length of the group property value. Only applies to type `"string"`.
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['GroupSchemaPropertyOneOfArgs']]]] one_ofs: Array of maps containing a mapping for display name to enum value.
         :param pulumi.Input[str] permissions: Access control permissions for the property. It can be set to `"READ_WRITE"`, `"READ_ONLY"`, `"HIDE"`.
         :param pulumi.Input[bool] required: Whether the property is required for this group.
         :param pulumi.Input[str] scope: determines whether an app user attribute can be set at the Individual or Group Level.
-        :param pulumi.Input[str] title: display name for the enum value.
-        :param pulumi.Input[str] type: Type of profile source.
+        :param pulumi.Input[str] title: The display name.
+        :param pulumi.Input[str] type: The type of the schema property. It can be `"string"`, `"boolean"`, `"number"`, `"integer"`, `"array"`, or `"object"`.
         :param pulumi.Input[str] unique: Whether the property should be unique. It can be set to `"UNIQUE_VALIDATED"` or `"NOT_UNIQUE"`.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _GroupSchemaPropertyState.__new__(_GroupSchemaPropertyState)
 
         __props__.__dict__["array_enums"] = array_enums
@@ -1016,23 +1012,23 @@
         """
         return pulumi.get(self, "scope")
 
     @property
     @pulumi.getter
     def title(self) -> pulumi.Output[str]:
         """
-        display name for the enum value.
+        The display name.
         """
         return pulumi.get(self, "title")
 
     @property
     @pulumi.getter
     def type(self) -> pulumi.Output[str]:
         """
-        Type of profile source.
+        The type of the schema property. It can be `"string"`, `"boolean"`, `"number"`, `"integer"`, `"array"`, or `"object"`.
         """
         return pulumi.get(self, "type")
 
     @property
     @pulumi.getter
     def unique(self) -> pulumi.Output[Optional[str]]:
         """
```

### Comparing `pulumi_okta-4.9.0a1713462165/pulumi_okta/idp/get_metadata_saml.py` & `pulumi_okta-4.9.0a1713902092/pulumi_okta/idp/get_metadata_saml.py`

 * *Files 5% similar despite different names*

```diff
@@ -152,22 +152,20 @@
 def get_metadata_saml(idp_id: Optional[str] = None,
                       opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetMetadataSamlResult:
     """
     Use this data source to retrieve SAML IdP metadata from Okta.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_okta as okta
 
     example = okta.idp.get_metadata_saml(idp_id="<idp id>")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str idp_id: The id of the IdP to retrieve metadata for.
     """
     __args__ = dict()
     __args__['idpId'] = idp_id
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
@@ -190,20 +188,18 @@
 def get_metadata_saml_output(idp_id: Optional[pulumi.Input[Optional[str]]] = None,
                              opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetMetadataSamlResult]:
     """
     Use this data source to retrieve SAML IdP metadata from Okta.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_okta as okta
 
     example = okta.idp.get_metadata_saml(idp_id="<idp id>")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str idp_id: The id of the IdP to retrieve metadata for.
     """
     ...
```

### Comparing `pulumi_okta-4.9.0a1713462165/pulumi_okta/idp/get_oidc.py` & `pulumi_okta-4.9.0a1713902092/pulumi_okta/idp/get_oidc.py`

 * *Files 6% similar despite different names*

```diff
@@ -252,22 +252,20 @@
              name: Optional[str] = None,
              opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetOidcResult:
     """
     Use this data source to retrieve a OIDC IdP from Okta.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_okta as okta
 
     example = okta.idp.get_oidc(name="Example Provider")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str id: The id of the idp to retrieve, conflicts with `name`.
     :param str name: The name of the idp to retrieve, conflicts with `id`.
     """
     __args__ = dict()
     __args__['id'] = id
@@ -301,21 +299,19 @@
                     name: Optional[pulumi.Input[Optional[str]]] = None,
                     opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetOidcResult]:
     """
     Use this data source to retrieve a OIDC IdP from Okta.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_okta as okta
 
     example = okta.idp.get_oidc(name="Example Provider")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str id: The id of the idp to retrieve, conflicts with `name`.
     :param str name: The name of the idp to retrieve, conflicts with `id`.
     """
     ...
```

### Comparing `pulumi_okta-4.9.0a1713462165/pulumi_okta/idp/get_saml.py` & `pulumi_okta-4.9.0a1713902092/pulumi_okta/idp/get_saml.py`

 * *Files 1% similar despite different names*

```diff
@@ -201,22 +201,20 @@
              name: Optional[str] = None,
              opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetSamlResult:
     """
     Use this data source to retrieve a SAML IdP from Okta.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_okta as okta
 
     example = okta.idp.get_saml(name="Example App")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str id: The id of the idp to retrieve, conflicts with `name`.
     :param str name: The name of the idp to retrieve, conflicts with `id`.
     """
     __args__ = dict()
     __args__['id'] = id
@@ -246,21 +244,19 @@
                     name: Optional[pulumi.Input[Optional[str]]] = None,
                     opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetSamlResult]:
     """
     Use this data source to retrieve a SAML IdP from Okta.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_okta as okta
 
     example = okta.idp.get_saml(name="Example App")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str id: The id of the idp to retrieve, conflicts with `name`.
     :param str name: The name of the idp to retrieve, conflicts with `id`.
     """
     ...
```

### Comparing `pulumi_okta-4.9.0a1713462165/pulumi_okta/idp/get_social.py` & `pulumi_okta-4.9.0a1713902092/pulumi_okta/idp/get_social.py`

 * *Files 1% similar despite different names*

```diff
@@ -354,22 +354,20 @@
                name: Optional[str] = None,
                opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetSocialResult:
     """
     Use this data source to retrieve a social IdP from Okta, namely `APPLE`, `FACEBOOK`, `LINKEDIN`, `MICROSOFT`, or  `GOOGLE`.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_okta as okta
 
     example = okta.idp.get_social(name="My Facebook IdP")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str id: The id of the social idp to retrieve, conflicts with `name`.
     :param str name: The name of the social idp to retrieve, conflicts with `id`.
     """
     __args__ = dict()
     __args__['id'] = id
@@ -412,21 +410,19 @@
                       name: Optional[pulumi.Input[Optional[str]]] = None,
                       opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetSocialResult]:
     """
     Use this data source to retrieve a social IdP from Okta, namely `APPLE`, `FACEBOOK`, `LINKEDIN`, `MICROSOFT`, or  `GOOGLE`.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_okta as okta
 
     example = okta.idp.get_social(name="My Facebook IdP")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str id: The id of the social idp to retrieve, conflicts with `name`.
     :param str name: The name of the social idp to retrieve, conflicts with `id`.
     """
     ...
```

### Comparing `pulumi_okta-4.9.0a1713462165/pulumi_okta/idp/oidc.py` & `pulumi_okta-4.9.0a1713902092/pulumi_okta/idp/oidc.py`

 * *Files 0% similar despite different names*

```diff
@@ -1106,15 +1106,14 @@
         """
         Creates an OIDC Identity Provider.
 
         This resource allows you to create and configure an OIDC Identity Provider.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_okta as okta
 
         example = okta.idp.Oidc("example",
             name="example",
             authorization_url="https://idp.example.com/authorize",
@@ -1127,15 +1126,14 @@
             jwks_binding="HTTP-REDIRECT",
             scopes=["openid"],
             client_id="efg456",
             client_secret="efg456",
             issuer_url="https://id.example.com",
             username_template="idpuser.email")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         An OIDC IdP can be imported via the Okta ID.
 
         ```sh
         $ pulumi import okta:idp/oidc:Oidc example &#60;idp id&#62;
@@ -1184,15 +1182,14 @@
         """
         Creates an OIDC Identity Provider.
 
         This resource allows you to create and configure an OIDC Identity Provider.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_okta as okta
 
         example = okta.idp.Oidc("example",
             name="example",
             authorization_url="https://idp.example.com/authorize",
@@ -1205,15 +1202,14 @@
             jwks_binding="HTTP-REDIRECT",
             scopes=["openid"],
             client_id="efg456",
             client_secret="efg456",
             issuer_url="https://id.example.com",
             username_template="idpuser.email")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         An OIDC IdP can be imported via the Okta ID.
 
         ```sh
         $ pulumi import okta:idp/oidc:Oidc example &#60;idp id&#62;
```

### Comparing `pulumi_okta-4.9.0a1713462165/pulumi_okta/idp/saml.py` & `pulumi_okta-4.9.0a1713902092/pulumi_okta/idp/saml.py`

 * *Files 1% similar despite different names*

```diff
@@ -1083,15 +1083,14 @@
         """
         Creates a SAML Identity Provider.
 
         This resource allows you to create and configure a SAML Identity Provider.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_okta as okta
 
         example = okta.idp.Saml("example",
             name="testAcc_replace_with_uuid",
             acs_type="INSTANCE",
@@ -1100,15 +1099,14 @@
             sso_binding="HTTP-POST",
             username_template="idpuser.email",
             kid=test["id"],
             issuer="https://idp.example.com",
             request_signature_scope="REQUEST",
             response_signature_scope="ANY")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         An SAML IdP can be imported via the Okta ID.
 
         ```sh
         $ pulumi import okta:idp/saml:Saml example &#60;idp id&#62;
@@ -1156,15 +1154,14 @@
         """
         Creates a SAML Identity Provider.
 
         This resource allows you to create and configure a SAML Identity Provider.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_okta as okta
 
         example = okta.idp.Saml("example",
             name="testAcc_replace_with_uuid",
             acs_type="INSTANCE",
@@ -1173,15 +1170,14 @@
             sso_binding="HTTP-POST",
             username_template="idpuser.email",
             kid=test["id"],
             issuer="https://idp.example.com",
             request_signature_scope="REQUEST",
             response_signature_scope="ANY")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         An SAML IdP can be imported via the Okta ID.
 
         ```sh
         $ pulumi import okta:idp/saml:Saml example &#60;idp id&#62;
```

### Comparing `pulumi_okta-4.9.0a1713462165/pulumi_okta/idp/saml_key.py` & `pulumi_okta-4.9.0a1713902092/pulumi_okta/idp/saml_key.py`

 * *Files 2% similar despite different names*

```diff
@@ -160,15 +160,14 @@
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  x5cs: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  __props__=None):
         """
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_okta as okta
 
         example1 = okta.idp.SamlKey("example_1", x5cs=[example["certificate"]])
         example2 = okta.idp.SamlKey("example_2", x5cs=[\"\"\"MIIDnjCCAoagAwIBAgIGAVG3MN+PMA0GCSqGSIb3DQEBBQUAMIGPMQswCQYDVQQGEwJVUzETMBEGA1UECAwKQ2FsaWZvcm5p
         YTEWMBQGA1UEBwwNU2FuIEZyYW5jaXNjbzENMAsGA1UECgwET2t0YTEUMBIGA1UECwwLU1NPUHJvdmlkZXIxEDAOBgNVBAMM
@@ -180,15 +179,14 @@
         wWeVH8g5d1n3KyR2TVajVJpCrPhLFmq1Il4G/IUnPe4MvjXqB6CpKkog1+ThWsItPRJPAM+RweFHXq7KfChXsYE7Mmfuly8s
         DQlvBmQyxZnFHVuiPfCvGHJjpvHy11YlHdOjfgqHRvZbmo30+y0X/oY/yV4YEJ00LL6eJWU4wi7ViY3HP6/VCdRjHoRdr5L/
         DwIDAQABMA0GCSqGSIb3DQEBBQUAA4IBAQCzzhOFkvyYLNFj2WDcq1YqD4sBy1iCia9QpRH3rjQvMKDwQDYWbi6EdOX0TQ/I
         YR7UWGj+2pXd6v0t33lYtoKocp/4lUvT3tfBnWZ5KnObi+J2uY2teUqoYkASN7F+GRPVOuMVoVgm05ss8tuMb2dLc9vsx93s
         Dt+XlMTv/2qi5VPwaDtqduKkzwW9lUfn4xIMkTiVvCpe0X2HneD2Bpuao3/U8Rk0uiPfq6TooWaoW3kjsmErhEAs9bA7xuqo
         1KKY9CdHcFhkSsMhoeaZylZHtzbnoipUlQKSLMdJQiiYZQ0bYL83/Ta9fulr1EERICMFt3GUmtYaZZKHpWSfdJp9\"\"\"])
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         A SAML IdP Signing Key can be imported via the key id.
 
         ```sh
         $ pulumi import okta:idp/samlKey:SamlKey example &#60;key id&#62;
@@ -203,15 +201,14 @@
     def __init__(__self__,
                  resource_name: str,
                  args: SamlKeyArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_okta as okta
 
         example1 = okta.idp.SamlKey("example_1", x5cs=[example["certificate"]])
         example2 = okta.idp.SamlKey("example_2", x5cs=[\"\"\"MIIDnjCCAoagAwIBAgIGAVG3MN+PMA0GCSqGSIb3DQEBBQUAMIGPMQswCQYDVQQGEwJVUzETMBEGA1UECAwKQ2FsaWZvcm5p
         YTEWMBQGA1UEBwwNU2FuIEZyYW5jaXNjbzENMAsGA1UECgwET2t0YTEUMBIGA1UECwwLU1NPUHJvdmlkZXIxEDAOBgNVBAMM
@@ -223,15 +220,14 @@
         wWeVH8g5d1n3KyR2TVajVJpCrPhLFmq1Il4G/IUnPe4MvjXqB6CpKkog1+ThWsItPRJPAM+RweFHXq7KfChXsYE7Mmfuly8s
         DQlvBmQyxZnFHVuiPfCvGHJjpvHy11YlHdOjfgqHRvZbmo30+y0X/oY/yV4YEJ00LL6eJWU4wi7ViY3HP6/VCdRjHoRdr5L/
         DwIDAQABMA0GCSqGSIb3DQEBBQUAA4IBAQCzzhOFkvyYLNFj2WDcq1YqD4sBy1iCia9QpRH3rjQvMKDwQDYWbi6EdOX0TQ/I
         YR7UWGj+2pXd6v0t33lYtoKocp/4lUvT3tfBnWZ5KnObi+J2uY2teUqoYkASN7F+GRPVOuMVoVgm05ss8tuMb2dLc9vsx93s
         Dt+XlMTv/2qi5VPwaDtqduKkzwW9lUfn4xIMkTiVvCpe0X2HneD2Bpuao3/U8Rk0uiPfq6TooWaoW3kjsmErhEAs9bA7xuqo
         1KKY9CdHcFhkSsMhoeaZylZHtzbnoipUlQKSLMdJQiiYZQ0bYL83/Ta9fulr1EERICMFt3GUmtYaZZKHpWSfdJp9\"\"\"])
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         A SAML IdP Signing Key can be imported via the key id.
 
         ```sh
         $ pulumi import okta:idp/samlKey:SamlKey example &#60;key id&#62;
```

### Comparing `pulumi_okta-4.9.0a1713462165/pulumi_okta/idp/social.py` & `pulumi_okta-4.9.0a1713902092/pulumi_okta/idp/social.py`

 * *Files 0% similar despite different names*

```diff
@@ -931,15 +931,14 @@
         """
         Creates a Social Identity Provider.
 
         This resource allows you to create and configure a Social Identity Provider.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_okta as okta
 
         example = okta.idp.Social("example",
             type="FACEBOOK",
             protocol_type="OAUTH2",
@@ -948,15 +947,14 @@
                 "public_profile",
                 "email",
             ],
             client_id="abcd123",
             client_secret="abcd123",
             username_template="idpuser.email")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         A Social IdP can be imported via the Okta ID.
 
         ```sh
         $ pulumi import okta:idp/social:Social example &#60;idp id&#62;
@@ -1001,15 +999,14 @@
         """
         Creates a Social Identity Provider.
 
         This resource allows you to create and configure a Social Identity Provider.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_okta as okta
 
         example = okta.idp.Social("example",
             type="FACEBOOK",
             protocol_type="OAUTH2",
@@ -1018,15 +1015,14 @@
                 "public_profile",
                 "email",
             ],
             client_id="abcd123",
             client_secret="abcd123",
             username_template="idpuser.email")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         A Social IdP can be imported via the Okta ID.
 
         ```sh
         $ pulumi import okta:idp/social:Social example &#60;idp id&#62;
```

### Comparing `pulumi_okta-4.9.0a1713462165/pulumi_okta/index/__init__.py` & `pulumi_okta-4.9.0a1713902092/pulumi_okta/index/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713462165/pulumi_okta/index/_inputs.py` & `pulumi_okta-4.9.0a1713902092/pulumi_okta/index/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713462165/pulumi_okta/index/customized_signin_page.py` & `pulumi_okta-4.9.0a1713902092/pulumi_okta/index/customized_signin_page.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713462165/pulumi_okta/index/email_domain.py` & `pulumi_okta-4.9.0a1713902092/pulumi_okta/index/email_domain.py`

 * *Files 1% similar despite different names*

```diff
@@ -196,26 +196,24 @@
                  user_name: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         This resource allows you to create and configure an email domain.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_okta as okta
 
         example = okta.index.EmailDomain("example",
             brand_id="abc123",
             domain="example.com",
             display_name="test",
             user_name="paul_atreides")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Custom email domain can be imported via the Okta ID.
 
         ```sh
         $ pulumi import okta:Index/emailDomain:EmailDomain example &#60;domain id&#62;
@@ -235,26 +233,24 @@
                  args: EmailDomainArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         This resource allows you to create and configure an email domain.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_okta as okta
 
         example = okta.index.EmailDomain("example",
             brand_id="abc123",
             domain="example.com",
             display_name="test",
             user_name="paul_atreides")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Custom email domain can be imported via the Okta ID.
 
         ```sh
         $ pulumi import okta:Index/emailDomain:EmailDomain example &#60;domain id&#62;
```

### Comparing `pulumi_okta-4.9.0a1713462165/pulumi_okta/index/email_domain_verification.py` & `pulumi_okta-4.9.0a1713902092/pulumi_okta/index/email_domain_verification.py`

 * *Files 5% similar despite different names*

```diff
@@ -66,27 +66,25 @@
                  email_domain_id: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         Verifies the email domain. The resource won't be created if the email domain could not be verified.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_okta as okta
 
         example = okta.index.EmailDomain("example",
             brand_id="abc123",
             domain="example.com",
             display_name="test",
             user_name="paul_atreides")
         example_email_domain_verification = okta.index.EmailDomainVerification("example", email_domain_id=valid["id"])
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         This resource does not support importing.
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
@@ -99,27 +97,25 @@
                  args: EmailDomainVerificationArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         Verifies the email domain. The resource won't be created if the email domain could not be verified.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_okta as okta
 
         example = okta.index.EmailDomain("example",
             brand_id="abc123",
             domain="example.com",
             display_name="test",
             user_name="paul_atreides")
         example_email_domain_verification = okta.index.EmailDomainVerification("example", email_domain_id=valid["id"])
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         This resource does not support importing.
 
         :param str resource_name: The name of the resource.
         :param EmailDomainVerificationArgs args: The arguments to use to populate this resource's properties.
```

### Comparing `pulumi_okta-4.9.0a1713462165/pulumi_okta/index/get_default_signin_page.py` & `pulumi_okta-4.9.0a1713902092/pulumi_okta/index/get_default_signin_page.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713462165/pulumi_okta/index/get_domain.py` & `pulumi_okta-4.9.0a1713902092/pulumi_okta/index/get_domain.py`

 * *Files 3% similar despite different names*

```diff
@@ -120,24 +120,22 @@
     Use this data source to retrieve a domain from Okta.
 
     - https://developer.okta.com/docs/reference/api/domains/#get-domain
     - https://developer.okta.com/docs/reference/api/domains/#domainresponse-object
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_okta as okta
 
     example = okta.Domain("example", name="www.example.com")
     by_name = okta.Index.get_domain(domain_id_or_name="www.example.com")
     by_id = okta.Index.get_domain_output(domain_id_or_name=example.id)
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str domain_id_or_name: The Okta ID of the domain or the domain name itself.
     """
     __args__ = dict()
     __args__['domainIdOrName'] = domain_id_or_name
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
@@ -160,22 +158,20 @@
     Use this data source to retrieve a domain from Okta.
 
     - https://developer.okta.com/docs/reference/api/domains/#get-domain
     - https://developer.okta.com/docs/reference/api/domains/#domainresponse-object
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_okta as okta
 
     example = okta.Domain("example", name="www.example.com")
     by_name = okta.Index.get_domain(domain_id_or_name="www.example.com")
     by_id = okta.Index.get_domain_output(domain_id_or_name=example.id)
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str domain_id_or_name: The Okta ID of the domain or the domain name itself.
     """
     ...
```

### Comparing `pulumi_okta-4.9.0a1713462165/pulumi_okta/index/get_log_stream.py` & `pulumi_okta-4.9.0a1713902092/pulumi_okta/index/get_log_stream.py`

 * *Files 4% similar despite different names*

```diff
@@ -99,22 +99,20 @@
                    settings: Optional[pulumi.InputType['GetLogStreamSettingsArgs']] = None,
                    opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetLogStreamResult:
     """
     Use this data source to retrieve a log stream from Okta.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_okta as okta
 
     example = okta.Index.get_log_stream(name="Example Stream")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str id: ID of the log stream to retrieve, conflicts with `name`.
     :param str name: Name of the log stream to retrieve, conflicts with `id`.
     :param pulumi.InputType['GetLogStreamSettingsArgs'] settings: Provider specific configuration.
     """
     __args__ = dict()
@@ -138,22 +136,20 @@
                           settings: Optional[pulumi.Input[Optional[pulumi.InputType['GetLogStreamSettingsArgs']]]] = None,
                           opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetLogStreamResult]:
     """
     Use this data source to retrieve a log stream from Okta.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_okta as okta
 
     example = okta.Index.get_log_stream(name="Example Stream")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str id: ID of the log stream to retrieve, conflicts with `name`.
     :param str name: Name of the log stream to retrieve, conflicts with `id`.
     :param pulumi.InputType['GetLogStreamSettingsArgs'] settings: Provider specific configuration.
     """
     ...
```

### Comparing `pulumi_okta-4.9.0a1713462165/pulumi_okta/index/get_org_metadata.py` & `pulumi_okta-4.9.0a1713902092/pulumi_okta/index/get_org_metadata.py`

 * *Files 3% similar despite different names*

```diff
@@ -88,22 +88,20 @@
     """
     Retrieves the well-known org metadata, which includes the id, configured custom domains, authentication pipeline, and various other org settings.
 
     - [Org Well Known Metadata Reference](https://developer.okta.com/docs/api/openapi/okta-management/management/tag/OrgSetting/#tag/OrgSetting/operation/getWellknownOrgMetadata)
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_okta as okta
 
     test = okta.Index.get_org_metadata()
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param pulumi.InputType['GetOrgMetadataDomainsArgs'] domains: The URIs for the org's configured domains.
     :param pulumi.InputType['GetOrgMetadataSettingsArgs'] settings: The wellknown org settings (safe for public consumption).
     """
     __args__ = dict()
     __args__['domains'] = domains
@@ -125,21 +123,19 @@
     """
     Retrieves the well-known org metadata, which includes the id, configured custom domains, authentication pipeline, and various other org settings.
 
     - [Org Well Known Metadata Reference](https://developer.okta.com/docs/api/openapi/okta-management/management/tag/OrgSetting/#tag/OrgSetting/operation/getWellknownOrgMetadata)
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_okta as okta
 
     test = okta.Index.get_org_metadata()
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param pulumi.InputType['GetOrgMetadataDomainsArgs'] domains: The URIs for the org's configured domains.
     :param pulumi.InputType['GetOrgMetadataSettingsArgs'] settings: The wellknown org settings (safe for public consumption).
     """
     ...
```

### Comparing `pulumi_okta-4.9.0a1713462165/pulumi_okta/index/log_stream.py` & `pulumi_okta-4.9.0a1713902092/pulumi_okta/index/log_stream.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713462165/pulumi_okta/index/outputs.py` & `pulumi_okta-4.9.0a1713902092/pulumi_okta/index/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713462165/pulumi_okta/index/preview_signin_page.py` & `pulumi_okta-4.9.0a1713902092/pulumi_okta/index/preview_signin_page.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713462165/pulumi_okta/inline/_inputs.py` & `pulumi_okta-4.9.0a1713902092/pulumi_okta/inline/outputs.py`

 * *Files 21% similar despite different names*

```diff
@@ -6,49 +6,31 @@
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 
 __all__ = [
-    'HookHeaderArgs',
+    'HookHeader',
 ]
 
-@pulumi.input_type
-class HookHeaderArgs:
+@pulumi.output_type
+class HookHeader(dict):
     def __init__(__self__, *,
-                 key: Optional[pulumi.Input[str]] = None,
-                 value: Optional[pulumi.Input[str]] = None):
-        """
-        :param pulumi.Input[str] key: Key to use for authentication, usually the header name, for example `"Authorization"`.
-        :param pulumi.Input[str] value: Authentication secret.
-        """
+                 key: Optional[str] = None,
+                 value: Optional[str] = None):
         if key is not None:
             pulumi.set(__self__, "key", key)
         if value is not None:
             pulumi.set(__self__, "value", value)
 
     @property
     @pulumi.getter
-    def key(self) -> Optional[pulumi.Input[str]]:
-        """
-        Key to use for authentication, usually the header name, for example `"Authorization"`.
-        """
+    def key(self) -> Optional[str]:
         return pulumi.get(self, "key")
 
-    @key.setter
-    def key(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "key", value)
-
     @property
     @pulumi.getter
-    def value(self) -> Optional[pulumi.Input[str]]:
-        """
-        Authentication secret.
-        """
+    def value(self) -> Optional[str]:
         return pulumi.get(self, "value")
 
-    @value.setter
-    def value(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "value", value)
-
```

### Comparing `pulumi_okta-4.9.0a1713462165/pulumi_okta/inline/hook.py` & `pulumi_okta-4.9.0a1713902092/pulumi_okta/inline/hook.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,16 +22,16 @@
                  auth: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  headers: Optional[pulumi.Input[Sequence[pulumi.Input['HookHeaderArgs']]]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  status: Optional[pulumi.Input[str]] = None):
         """
         The set of arguments for constructing a Hook resource.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] channel: Details of the endpoint the inline hook will hit.
-        :param pulumi.Input[str] type: The type of hook to trigger. Currently, the only supported type is `"HTTP"`.
-        :param pulumi.Input[str] version: Version of the channel. The currently-supported version is `"1.0.0"`.
+        :param pulumi.Input[str] type: The type of hook to create. [See here for supported types](https://developer.okta.com/docs/reference/api/inline-hooks/#supported-inline-hook-types).
+        :param pulumi.Input[str] version: The version of the hook. The currently-supported version is `"1.0.0"`.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] auth: Authentication required for inline hook request.
         :param pulumi.Input[Sequence[pulumi.Input['HookHeaderArgs']]] headers: Map of headers to send along in inline hook request.
         :param pulumi.Input[str] name: The inline hook display name.
         :param pulumi.Input[str] status: Default to `ACTIVE`
         """
         pulumi.set(__self__, "channel", channel)
         pulumi.set(__self__, "type", type)
@@ -57,27 +57,27 @@
     def channel(self, value: pulumi.Input[Mapping[str, pulumi.Input[str]]]):
         pulumi.set(self, "channel", value)
 
     @property
     @pulumi.getter
     def type(self) -> pulumi.Input[str]:
         """
-        The type of hook to trigger. Currently, the only supported type is `"HTTP"`.
+        The type of hook to create. [See here for supported types](https://developer.okta.com/docs/reference/api/inline-hooks/#supported-inline-hook-types).
         """
         return pulumi.get(self, "type")
 
     @type.setter
     def type(self, value: pulumi.Input[str]):
         pulumi.set(self, "type", value)
 
     @property
     @pulumi.getter
     def version(self) -> pulumi.Input[str]:
         """
-        Version of the channel. The currently-supported version is `"1.0.0"`.
+        The version of the hook. The currently-supported version is `"1.0.0"`.
         """
         return pulumi.get(self, "version")
 
     @version.setter
     def version(self, value: pulumi.Input[str]):
         pulumi.set(self, "version", value)
 
@@ -143,16 +143,16 @@
         """
         Input properties used for looking up and filtering Hook resources.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] auth: Authentication required for inline hook request.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] channel: Details of the endpoint the inline hook will hit.
         :param pulumi.Input[Sequence[pulumi.Input['HookHeaderArgs']]] headers: Map of headers to send along in inline hook request.
         :param pulumi.Input[str] name: The inline hook display name.
         :param pulumi.Input[str] status: Default to `ACTIVE`
-        :param pulumi.Input[str] type: The type of hook to trigger. Currently, the only supported type is `"HTTP"`.
-        :param pulumi.Input[str] version: Version of the channel. The currently-supported version is `"1.0.0"`.
+        :param pulumi.Input[str] type: The type of hook to create. [See here for supported types](https://developer.okta.com/docs/reference/api/inline-hooks/#supported-inline-hook-types).
+        :param pulumi.Input[str] version: The version of the hook. The currently-supported version is `"1.0.0"`.
         """
         if auth is not None:
             pulumi.set(__self__, "auth", auth)
         if channel is not None:
             pulumi.set(__self__, "channel", channel)
         if headers is not None:
             pulumi.set(__self__, "headers", headers)
@@ -225,27 +225,27 @@
     def status(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "status", value)
 
     @property
     @pulumi.getter
     def type(self) -> Optional[pulumi.Input[str]]:
         """
-        The type of hook to trigger. Currently, the only supported type is `"HTTP"`.
+        The type of hook to create. [See here for supported types](https://developer.okta.com/docs/reference/api/inline-hooks/#supported-inline-hook-types).
         """
         return pulumi.get(self, "type")
 
     @type.setter
     def type(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "type", value)
 
     @property
     @pulumi.getter
     def version(self) -> Optional[pulumi.Input[str]]:
         """
-        Version of the channel. The currently-supported version is `"1.0.0"`.
+        The version of the hook. The currently-supported version is `"1.0.0"`.
         """
         return pulumi.get(self, "version")
 
     @version.setter
     def version(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "version", value)
 
@@ -266,15 +266,14 @@
         """
         Creates an inline hook.
 
         This resource allows you to create and configure an inline hook.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_okta as okta
 
         example = okta.inline.Hook("example",
             name="example",
             version="1.0.0",
@@ -286,15 +285,14 @@
             },
             auth={
                 "key": "Authorization",
                 "type": "HEADER",
                 "value": "secret",
             })
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         An inline hook can be imported via the Okta ID.
 
         ```sh
         $ pulumi import okta:inline/hook:Hook example &#60;hook id&#62;
@@ -303,31 +301,30 @@
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] auth: Authentication required for inline hook request.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] channel: Details of the endpoint the inline hook will hit.
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['HookHeaderArgs']]]] headers: Map of headers to send along in inline hook request.
         :param pulumi.Input[str] name: The inline hook display name.
         :param pulumi.Input[str] status: Default to `ACTIVE`
-        :param pulumi.Input[str] type: The type of hook to trigger. Currently, the only supported type is `"HTTP"`.
-        :param pulumi.Input[str] version: Version of the channel. The currently-supported version is `"1.0.0"`.
+        :param pulumi.Input[str] type: The type of hook to create. [See here for supported types](https://developer.okta.com/docs/reference/api/inline-hooks/#supported-inline-hook-types).
+        :param pulumi.Input[str] version: The version of the hook. The currently-supported version is `"1.0.0"`.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: HookArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         Creates an inline hook.
 
         This resource allows you to create and configure an inline hook.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_okta as okta
 
         example = okta.inline.Hook("example",
             name="example",
             version="1.0.0",
@@ -339,15 +336,14 @@
             },
             auth={
                 "key": "Authorization",
                 "type": "HEADER",
                 "value": "secret",
             })
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         An inline hook can be imported via the Okta ID.
 
         ```sh
         $ pulumi import okta:inline/hook:Hook example &#60;hook id&#62;
@@ -422,16 +418,16 @@
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] auth: Authentication required for inline hook request.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] channel: Details of the endpoint the inline hook will hit.
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['HookHeaderArgs']]]] headers: Map of headers to send along in inline hook request.
         :param pulumi.Input[str] name: The inline hook display name.
         :param pulumi.Input[str] status: Default to `ACTIVE`
-        :param pulumi.Input[str] type: The type of hook to trigger. Currently, the only supported type is `"HTTP"`.
-        :param pulumi.Input[str] version: Version of the channel. The currently-supported version is `"1.0.0"`.
+        :param pulumi.Input[str] type: The type of hook to create. [See here for supported types](https://developer.okta.com/docs/reference/api/inline-hooks/#supported-inline-hook-types).
+        :param pulumi.Input[str] version: The version of the hook. The currently-supported version is `"1.0.0"`.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _HookState.__new__(_HookState)
 
         __props__.__dict__["auth"] = auth
         __props__.__dict__["channel"] = channel
@@ -482,19 +478,19 @@
         """
         return pulumi.get(self, "status")
 
     @property
     @pulumi.getter
     def type(self) -> pulumi.Output[str]:
         """
-        The type of hook to trigger. Currently, the only supported type is `"HTTP"`.
+        The type of hook to create. [See here for supported types](https://developer.okta.com/docs/reference/api/inline-hooks/#supported-inline-hook-types).
         """
         return pulumi.get(self, "type")
 
     @property
     @pulumi.getter
     def version(self) -> pulumi.Output[str]:
         """
-        Version of the channel. The currently-supported version is `"1.0.0"`.
+        The version of the hook. The currently-supported version is `"1.0.0"`.
         """
         return pulumi.get(self, "version")
```

### Comparing `pulumi_okta-4.9.0a1713462165/pulumi_okta/link_definition.py` & `pulumi_okta-4.9.0a1713902092/pulumi_okta/link_definition.py`

 * *Files 0% similar despite different names*

```diff
@@ -229,28 +229,26 @@
         Link definition operations allow you to manage the creation and removal of the link definitions. If you remove a link
         definition, links based on that definition are unavailable. Note that this resource is immutable, thus can not be modified.
 
         > **NOTE:** Links reappear if you recreate the definition. However, Okta is likely to change this behavior so that links don't reappear. Don't rely on this behavior in production environments.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_okta as okta
 
         example = okta.LinkDefinition("example",
             primary_name="emperor",
             primary_title="Emperor",
             primary_description="Hereditary ruler of the Imperium and the Known Universe",
             associated_name="sardaukar",
             associated_title="Sardaukar",
             associated_description="Elite military force member")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Okta Link Definition can be imported via the Okta Primary Link Name.
 
         ```sh
         $ pulumi import okta:index/linkDefinition:LinkDefinition example &#60;primary_name&#62;
@@ -275,28 +273,26 @@
         Link definition operations allow you to manage the creation and removal of the link definitions. If you remove a link
         definition, links based on that definition are unavailable. Note that this resource is immutable, thus can not be modified.
 
         > **NOTE:** Links reappear if you recreate the definition. However, Okta is likely to change this behavior so that links don't reappear. Don't rely on this behavior in production environments.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_okta as okta
 
         example = okta.LinkDefinition("example",
             primary_name="emperor",
             primary_title="Emperor",
             primary_description="Hereditary ruler of the Imperium and the Known Universe",
             associated_name="sardaukar",
             associated_title="Sardaukar",
             associated_description="Elite military force member")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Okta Link Definition can be imported via the Okta Primary Link Name.
 
         ```sh
         $ pulumi import okta:index/linkDefinition:LinkDefinition example &#60;primary_name&#62;
```

### Comparing `pulumi_okta-4.9.0a1713462165/pulumi_okta/link_value.py` & `pulumi_okta-4.9.0a1713902092/pulumi_okta/link_value.py`

 * *Files 2% similar despite different names*

```diff
@@ -131,15 +131,14 @@
                  primary_user_id: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         Link value operations allow you to create relationships between primary and associated users.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_okta as okta
 
         padishah = okta.LinkDefinition("padishah",
             primary_name="emperor",
             primary_title="Emperor",
@@ -166,15 +165,14 @@
                 sardaukars[0].id,
                 sardaukars[1].id,
                 sardaukars[2].id,
                 sardaukars[3].id,
                 sardaukars[4].id,
             ])
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Okta Link Value can be imported via Primary Name and Primary User ID.
 
         ```sh
         $ pulumi import okta:index/linkValue:LinkValue example &#60;primary_name&#62;/&#60;primary_user_id&#62;
@@ -193,15 +191,14 @@
                  args: LinkValueArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         Link value operations allow you to create relationships between primary and associated users.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_okta as okta
 
         padishah = okta.LinkDefinition("padishah",
             primary_name="emperor",
             primary_title="Emperor",
@@ -228,15 +225,14 @@
                 sardaukars[0].id,
                 sardaukars[1].id,
                 sardaukars[2].id,
                 sardaukars[3].id,
                 sardaukars[4].id,
             ])
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Okta Link Value can be imported via Primary Name and Primary User ID.
 
         ```sh
         $ pulumi import okta:index/linkValue:LinkValue example &#60;primary_name&#62;/&#60;primary_user_id&#62;
```

### Comparing `pulumi_okta-4.9.0a1713462165/pulumi_okta/network/zone.py` & `pulumi_okta-4.9.0a1713902092/pulumi_okta/network/zone.py`

 * *Files 1% similar despite different names*

```diff
@@ -336,15 +336,14 @@
         """
         Creates an Okta Network Zone.
 
         This resource allows you to create and configure an Okta Network Zone.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_okta as okta
 
         example = okta.network.Zone("example",
             name="example",
             type="IP",
@@ -353,30 +352,27 @@
                 "2.3.4.5-2.3.4.15",
             ],
             proxies=[
                 "2.2.3.4/24",
                 "3.3.4.5-3.3.4.15",
             ])
         ```
-        <!--End PulumiCodeChooser -->
 
         ### Dynamic Tor Blocker
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_okta as okta
 
         example = okta.network.Zone("example",
             name="TOR Blocker",
             type="DYNAMIC",
             usage="BLOCKLIST",
             dynamic_proxy_type="TorAnonymizer")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Okta Network Zone can be imported via the Okta ID.
 
         ```sh
         $ pulumi import okta:network/zone:Zone example &#60;zone id&#62;
@@ -404,15 +400,14 @@
         """
         Creates an Okta Network Zone.
 
         This resource allows you to create and configure an Okta Network Zone.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_okta as okta
 
         example = okta.network.Zone("example",
             name="example",
             type="IP",
@@ -421,30 +416,27 @@
                 "2.3.4.5-2.3.4.15",
             ],
             proxies=[
                 "2.2.3.4/24",
                 "3.3.4.5-3.3.4.15",
             ])
         ```
-        <!--End PulumiCodeChooser -->
 
         ### Dynamic Tor Blocker
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_okta as okta
 
         example = okta.network.Zone("example",
             name="TOR Blocker",
             type="DYNAMIC",
             usage="BLOCKLIST",
             dynamic_proxy_type="TorAnonymizer")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Okta Network Zone can be imported via the Okta ID.
 
         ```sh
         $ pulumi import okta:network/zone:Zone example &#60;zone id&#62;
```

### Comparing `pulumi_okta-4.9.0a1713462165/pulumi_okta/org_configuration.py` & `pulumi_okta-4.9.0a1713902092/pulumi_okta/org_configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -566,24 +566,22 @@
         """
         This resource allows you manage org settings, logo, support and communication options.
 
         > **IMPORTANT:** You must specify all Org Setting properties when you update an org's profile. Any property not specified in the script will be deleted.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_okta as okta
 
         example = okta.OrgConfiguration("example",
             company_name="Umbrella Corporation",
             website="https://terraform.io")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Okta Org Configuration can be imported even without specifying the Org ID.
 
         ```sh
         $ pulumi import okta:index/orgConfiguration:OrgConfiguration example _
@@ -617,24 +615,22 @@
         """
         This resource allows you manage org settings, logo, support and communication options.
 
         > **IMPORTANT:** You must specify all Org Setting properties when you update an org's profile. Any property not specified in the script will be deleted.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_okta as okta
 
         example = okta.OrgConfiguration("example",
             company_name="Umbrella Corporation",
             website="https://terraform.io")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Okta Org Configuration can be imported even without specifying the Org ID.
 
         ```sh
         $ pulumi import okta:index/orgConfiguration:OrgConfiguration example _
```

### Comparing `pulumi_okta-4.9.0a1713462165/pulumi_okta/org_support.py` & `pulumi_okta-4.9.0a1713902092/pulumi_okta/org_support.py`

 * *Files 2% similar despite different names*

```diff
@@ -100,22 +100,20 @@
                  __props__=None):
         """
         This resource allows you to temporarily allow Okta Support to access your org as an administrator. By default,
         access will be granted for eight hours. Removing this resource will revoke Okta Support access to your org.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_okta as okta
 
         example = okta.OrgSupport("example", extend_by=1)
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         This resource does not support importing.
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
@@ -129,22 +127,20 @@
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         This resource allows you to temporarily allow Okta Support to access your org as an administrator. By default,
         access will be granted for eight hours. Removing this resource will revoke Okta Support access to your org.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_okta as okta
 
         example = okta.OrgSupport("example", extend_by=1)
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         This resource does not support importing.
 
         :param str resource_name: The name of the resource.
         :param OrgSupportArgs args: The arguments to use to populate this resource's properties.
```

### Comparing `pulumi_okta-4.9.0a1713462165/pulumi_okta/outputs.py` & `pulumi_okta-4.9.0a1713902092/pulumi_okta/outputs.py`

 * *Files 1% similar despite different names*

```diff
@@ -101,15 +101,15 @@
     def __init__(__self__, *,
                  os_expression: Optional[str] = None,
                  os_type: Optional[str] = None,
                  type: Optional[str] = None):
         """
         :param str os_expression: Only available and required when using `os_type = "OTHER"`
         :param str os_type: One of: `"ANY"`, `"IOS"`, `"WINDOWS"`, `"ANDROID"`, `"OTHER"`, `"OSX"`, `"MACOS"`, `"CHROMEOS"`
-        :param str type: The Verification Method type. It can be set to `"ASSURANCE"`. Default is `"ASSURANCE"`.
+        :param str type: One of: `"ANY"`, `"MOBILE"`, `"DESKTOP"`
         """
         if os_expression is not None:
             pulumi.set(__self__, "os_expression", os_expression)
         if os_type is not None:
             pulumi.set(__self__, "os_type", os_type)
         if type is not None:
             pulumi.set(__self__, "type", type)
@@ -130,15 +130,15 @@
         """
         return pulumi.get(self, "os_type")
 
     @property
     @pulumi.getter
     def type(self) -> Optional[str]:
         """
-        The Verification Method type. It can be set to `"ASSURANCE"`. Default is `"ASSURANCE"`.
+        One of: `"ANY"`, `"MOBILE"`, `"DESKTOP"`
         """
         return pulumi.get(self, "type")
 
 
 @pulumi.output_type
 class AppUserSchemaPropertyArrayOneOf(dict):
     def __init__(__self__, *,
@@ -170,25 +170,25 @@
 
 @pulumi.output_type
 class AppUserSchemaPropertyOneOf(dict):
     def __init__(__self__, *,
                  const: str,
                  title: str):
         """
-        :param str const: value mapping to member of `array_enum`.
+        :param str const: value mapping to member of `enum`.
         :param str title: display name for the enum value.
         """
         pulumi.set(__self__, "const", const)
         pulumi.set(__self__, "title", title)
 
     @property
     @pulumi.getter
     def const(self) -> str:
         """
-        value mapping to member of `array_enum`.
+        value mapping to member of `enum`.
         """
         return pulumi.get(self, "const")
 
     @property
     @pulumi.getter
     def title(self) -> str:
         """
@@ -330,37 +330,27 @@
 
 
 @pulumi.output_type
 class EventHookHeader(dict):
     def __init__(__self__, *,
                  key: Optional[str] = None,
                  value: Optional[str] = None):
-        """
-        :param str key: Key to use for authentication, usually the header name, for example `"Authorization"`.
-        :param str value: Authentication secret.
-        """
         if key is not None:
             pulumi.set(__self__, "key", key)
         if value is not None:
             pulumi.set(__self__, "value", value)
 
     @property
     @pulumi.getter
     def key(self) -> Optional[str]:
-        """
-        Key to use for authentication, usually the header name, for example `"Authorization"`.
-        """
         return pulumi.get(self, "key")
 
     @property
     @pulumi.getter
     def value(self) -> Optional[str]:
-        """
-        Authentication secret.
-        """
         return pulumi.get(self, "value")
 
 
 @pulumi.output_type
 class GroupSchemaPropertyArrayOneOf(dict):
     def __init__(__self__, *,
                  const: str,
```

### Comparing `pulumi_okta-4.9.0a1713462165/pulumi_okta/policy/__init__.py` & `pulumi_okta-4.9.0a1713902092/pulumi_okta/policy/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713462165/pulumi_okta/policy/_inputs.py` & `pulumi_okta-4.9.0a1713902092/pulumi_okta/policy/_inputs.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,53 +23,49 @@
 @pulumi.input_type
 class RuleIdpDiscoveryAppExcludeArgs:
     def __init__(__self__, *,
                  type: pulumi.Input[str],
                  id: Optional[pulumi.Input[str]] = None,
                  name: Optional[pulumi.Input[str]] = None):
         """
-        :param pulumi.Input[str] type: One of: `"ANY"`, `"MOBILE"`, `"DESKTOP"`
-        :param pulumi.Input[str] id: Use if `type` is `"APP"` to indicate the application id to include.
-        :param pulumi.Input[str] name: Use if the `type` is `"APP_TYPE"` to indicate the type of application(s) to include in instances where an entire group (i.e. `yahoo_mail`) of applications should be included.
+        :param pulumi.Input[str] id: ID of the Rule.
+        :param pulumi.Input[str] name: Policy rule name.
         """
         pulumi.set(__self__, "type", type)
         if id is not None:
             pulumi.set(__self__, "id", id)
         if name is not None:
             pulumi.set(__self__, "name", name)
 
     @property
     @pulumi.getter
     def type(self) -> pulumi.Input[str]:
-        """
-        One of: `"ANY"`, `"MOBILE"`, `"DESKTOP"`
-        """
         return pulumi.get(self, "type")
 
     @type.setter
     def type(self, value: pulumi.Input[str]):
         pulumi.set(self, "type", value)
 
     @property
     @pulumi.getter
     def id(self) -> Optional[pulumi.Input[str]]:
         """
-        Use if `type` is `"APP"` to indicate the application id to include.
+        ID of the Rule.
         """
         return pulumi.get(self, "id")
 
     @id.setter
     def id(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "id", value)
 
     @property
     @pulumi.getter
     def name(self) -> Optional[pulumi.Input[str]]:
         """
-        Use if the `type` is `"APP_TYPE"` to indicate the type of application(s) to include in instances where an entire group (i.e. `yahoo_mail`) of applications should be included.
+        Policy rule name.
         """
         return pulumi.get(self, "name")
 
     @name.setter
     def name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "name", value)
 
@@ -77,29 +73,29 @@
 @pulumi.input_type
 class RuleIdpDiscoveryAppIncludeArgs:
     def __init__(__self__, *,
                  type: pulumi.Input[str],
                  id: Optional[pulumi.Input[str]] = None,
                  name: Optional[pulumi.Input[str]] = None):
         """
-        :param pulumi.Input[str] type: One of: `"ANY"`, `"MOBILE"`, `"DESKTOP"`
+        :param pulumi.Input[str] type: One of: `"APP"`, `"APP_TYPE"`
         :param pulumi.Input[str] id: Use if `type` is `"APP"` to indicate the application id to include.
         :param pulumi.Input[str] name: Use if the `type` is `"APP_TYPE"` to indicate the type of application(s) to include in instances where an entire group (i.e. `yahoo_mail`) of applications should be included.
         """
         pulumi.set(__self__, "type", type)
         if id is not None:
             pulumi.set(__self__, "id", id)
         if name is not None:
             pulumi.set(__self__, "name", name)
 
     @property
     @pulumi.getter
     def type(self) -> pulumi.Input[str]:
         """
-        One of: `"ANY"`, `"MOBILE"`, `"DESKTOP"`
+        One of: `"APP"`, `"APP_TYPE"`
         """
         return pulumi.get(self, "type")
 
     @type.setter
     def type(self, value: pulumi.Input[str]):
         pulumi.set(self, "type", value)
 
@@ -225,53 +221,49 @@
 @pulumi.input_type
 class RuleMfaAppExcludeArgs:
     def __init__(__self__, *,
                  type: pulumi.Input[str],
                  id: Optional[pulumi.Input[str]] = None,
                  name: Optional[pulumi.Input[str]] = None):
         """
-        :param pulumi.Input[str] type: One of: `"APP"`, `"APP_TYPE"`
-        :param pulumi.Input[str] id: Use if `type` is `"APP"` to indicate the application id to include.
-        :param pulumi.Input[str] name: Use if the `type` is `"APP_TYPE"` to indicate the type of application(s) to include in instances where an entire group (i.e. `yahoo_mail`) of applications should be included.
+        :param pulumi.Input[str] id: ID of the Rule.
+        :param pulumi.Input[str] name: Policy Rule Name.
         """
         pulumi.set(__self__, "type", type)
         if id is not None:
             pulumi.set(__self__, "id", id)
         if name is not None:
             pulumi.set(__self__, "name", name)
 
     @property
     @pulumi.getter
     def type(self) -> pulumi.Input[str]:
-        """
-        One of: `"APP"`, `"APP_TYPE"`
-        """
         return pulumi.get(self, "type")
 
     @type.setter
     def type(self, value: pulumi.Input[str]):
         pulumi.set(self, "type", value)
 
     @property
     @pulumi.getter
     def id(self) -> Optional[pulumi.Input[str]]:
         """
-        Use if `type` is `"APP"` to indicate the application id to include.
+        ID of the Rule.
         """
         return pulumi.get(self, "id")
 
     @id.setter
     def id(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "id", value)
 
     @property
     @pulumi.getter
     def name(self) -> Optional[pulumi.Input[str]]:
         """
-        Use if the `type` is `"APP_TYPE"` to indicate the type of application(s) to include in instances where an entire group (i.e. `yahoo_mail`) of applications should be included.
+        Policy Rule Name.
         """
         return pulumi.get(self, "name")
 
     @name.setter
     def name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "name", value)
 
@@ -385,37 +377,37 @@
 
 @pulumi.input_type
 class RuleSignonFactorSequenceSecondaryCriteriaArgs:
     def __init__(__self__, *,
                  factor_type: pulumi.Input[str],
                  provider: pulumi.Input[str]):
         """
-        :param pulumi.Input[str] factor_type: Factor type of the additional authentication step.
-        :param pulumi.Input[str] provider: Provider of the additional authentication step.
+        :param pulumi.Input[str] factor_type: Type of a Factor
+        :param pulumi.Input[str] provider: Factor provider
         """
         pulumi.set(__self__, "factor_type", factor_type)
         pulumi.set(__self__, "provider", provider)
 
     @property
     @pulumi.getter(name="factorType")
     def factor_type(self) -> pulumi.Input[str]:
         """
-        Factor type of the additional authentication step.
+        Type of a Factor
         """
         return pulumi.get(self, "factor_type")
 
     @factor_type.setter
     def factor_type(self, value: pulumi.Input[str]):
         pulumi.set(self, "factor_type", value)
 
     @property
     @pulumi.getter
     def provider(self) -> pulumi.Input[str]:
         """
-        Provider of the additional authentication step.
+        Factor provider
         """
         return pulumi.get(self, "provider")
 
     @provider.setter
     def provider(self, value: pulumi.Input[str]):
         pulumi.set(self, "provider", value)
```

### Comparing `pulumi_okta-4.9.0a1713462165/pulumi_okta/policy/device_assurance_android.py` & `pulumi_okta-4.9.0a1713902092/pulumi_okta/policy/device_assurance_android.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713462165/pulumi_okta/policy/device_assurance_chromeos.py` & `pulumi_okta-4.9.0a1713902092/pulumi_okta/policy/device_assurance_chromeos.py`

 * *Files 0% similar despite different names*

```diff
@@ -609,15 +609,14 @@
                  tpsp_site_isolation_enabled: Optional[pulumi.Input[bool]] = None,
                  __props__=None):
         """
         Manages a device assurance policy for chromeos.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_okta as okta
 
         example = okta.policy.DeviceAssuranceChromeos("example",
             name="example",
             tpsp_allow_screen_lock=True,
@@ -631,15 +630,14 @@
             tpsp_os_version="10.0.19041.1110",
             tpsp_password_proctection_warning_trigger="PASSWORD_PROTECTION_OFF",
             tpsp_realtime_url_check_mode=True,
             tpsp_safe_browsing_protection_level="ENHANCED_PROTECTION",
             tpsp_screen_lock_secured=True,
             tpsp_site_isolation_enabled=True)
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         ```sh
         $ pulumi import okta:policy/deviceAssuranceChromeos:DeviceAssuranceChromeos example &#60;device assurance id&#62;
         ```
 
@@ -668,15 +666,14 @@
                  args: Optional[DeviceAssuranceChromeosArgs] = None,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         Manages a device assurance policy for chromeos.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_okta as okta
 
         example = okta.policy.DeviceAssuranceChromeos("example",
             name="example",
             tpsp_allow_screen_lock=True,
@@ -690,15 +687,14 @@
             tpsp_os_version="10.0.19041.1110",
             tpsp_password_proctection_warning_trigger="PASSWORD_PROTECTION_OFF",
             tpsp_realtime_url_check_mode=True,
             tpsp_safe_browsing_protection_level="ENHANCED_PROTECTION",
             tpsp_screen_lock_secured=True,
             tpsp_site_isolation_enabled=True)
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         ```sh
         $ pulumi import okta:policy/deviceAssuranceChromeos:DeviceAssuranceChromeos example &#60;device assurance id&#62;
         ```
```

### Comparing `pulumi_okta-4.9.0a1713462165/pulumi_okta/policy/device_assurance_ios.py` & `pulumi_okta-4.9.0a1713902092/pulumi_okta/policy/device_assurance_ios.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713462165/pulumi_okta/policy/device_assurance_macos.py` & `pulumi_okta-4.9.0a1713902092/pulumi_okta/policy/device_assurance_macos.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713462165/pulumi_okta/policy/device_assurance_windows.py` & `pulumi_okta-4.9.0a1713902092/pulumi_okta/policy/device_assurance_windows.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713462165/pulumi_okta/policy/get_default_policy.py` & `pulumi_okta-4.9.0a1713902092/pulumi_okta/policy/get_default_policy.py`

 * *Files 8% similar despite different names*

```diff
@@ -59,22 +59,20 @@
 def get_default_policy(type: Optional[str] = None,
                        opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetDefaultPolicyResult:
     """
     Use this data source to retrieve a default policy from Okta. This same thing can be achieved using the `policy_get_policy` with default names, this is simply a shortcut.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_okta as okta
 
     example = okta.policy.get_default_policy(type="PASSWORD")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str type: Type of policy to retrieve.  Valid values: `OKTA_SIGN_ON`, `PASSWORD`, `MFA_ENROLL`, `IDP_DISCOVERY`
            `"IDP_DISCOVERY"`, `"ACCESS_POLICY"` (**only available as a part of the Identity Engine**), `"PROFILE_ENROLLMENT"` (**only available as a part of the Identity Engine**)
     """
     __args__ = dict()
     __args__['type'] = type
@@ -90,21 +88,19 @@
 def get_default_policy_output(type: Optional[pulumi.Input[str]] = None,
                               opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetDefaultPolicyResult]:
     """
     Use this data source to retrieve a default policy from Okta. This same thing can be achieved using the `policy_get_policy` with default names, this is simply a shortcut.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_okta as okta
 
     example = okta.policy.get_default_policy(type="PASSWORD")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str type: Type of policy to retrieve.  Valid values: `OKTA_SIGN_ON`, `PASSWORD`, `MFA_ENROLL`, `IDP_DISCOVERY`
            `"IDP_DISCOVERY"`, `"ACCESS_POLICY"` (**only available as a part of the Identity Engine**), `"PROFILE_ENROLLMENT"` (**only available as a part of the Identity Engine**)
     """
     ...
```

### Comparing `pulumi_okta-4.9.0a1713462165/pulumi_okta/policy/get_policy.py` & `pulumi_okta-4.9.0a1713902092/pulumi_okta/policy/get_policy.py`

 * *Files 7% similar despite different names*

```diff
@@ -81,23 +81,21 @@
                type: Optional[str] = None,
                opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetPolicyResult:
     """
     Use this data source to retrieve a policy from Okta.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_okta as okta
 
     example = okta.policy.get_policy(name="Password Policy Example",
         type="PASSWORD")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str name: Name of policy to retrieve.
     :param str type: Type of policy to retrieve. See https://developer.okta.com/docs/reference/api/policy/#policy-object for valid values. Currently:
            - All:
     """
     __args__ = dict()
@@ -118,23 +116,21 @@
                       type: Optional[pulumi.Input[str]] = None,
                       opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetPolicyResult]:
     """
     Use this data source to retrieve a policy from Okta.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_okta as okta
 
     example = okta.policy.get_policy(name="Password Policy Example",
         type="PASSWORD")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str name: Name of policy to retrieve.
     :param str type: Type of policy to retrieve. See https://developer.okta.com/docs/reference/api/policy/#policy-object for valid values. Currently:
            - All:
     """
     ...
```

### Comparing `pulumi_okta-4.9.0a1713462165/pulumi_okta/policy/mfa.py` & `pulumi_okta-4.9.0a1713902092/pulumi_okta/policy/mfa.py`

 * *Files 0% similar despite different names*

```diff
@@ -935,15 +935,14 @@
 
         > Requires Org Feature Flag `OKTA_MFA_POLICY`. Contact support to have this feature flag ***enabled***.
 
         > Unless Org Feature Flag `ENG_ENABLE_OPTIONAL_PASSWORD_ENROLLMENT` is ***disabled*** `okta_password` or `okta_email` must be present and its `enroll` value set to `REQUIRED`. Contact support to have this feature flag ***disabled***.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_okta as okta
 
         classic_example = okta.policy.Mfa("classic_example",
             name="MFA Policy Classic",
             status="ACTIVE",
@@ -965,15 +964,14 @@
                 "enroll": "REQUIRED",
             },
             okta_verify={
                 "enroll": "REQUIRED",
             },
             groups_includeds=[everyone["id"]])
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         An MFA Policy can be imported via the Okta ID.
 
         ```sh
         $ pulumi import okta:policy/mfa:Mfa example &#60;policy id&#62;
@@ -1023,15 +1021,14 @@
 
         > Requires Org Feature Flag `OKTA_MFA_POLICY`. Contact support to have this feature flag ***enabled***.
 
         > Unless Org Feature Flag `ENG_ENABLE_OPTIONAL_PASSWORD_ENROLLMENT` is ***disabled*** `okta_password` or `okta_email` must be present and its `enroll` value set to `REQUIRED`. Contact support to have this feature flag ***disabled***.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_okta as okta
 
         classic_example = okta.policy.Mfa("classic_example",
             name="MFA Policy Classic",
             status="ACTIVE",
@@ -1053,15 +1050,14 @@
                 "enroll": "REQUIRED",
             },
             okta_verify={
                 "enroll": "REQUIRED",
             },
             groups_includeds=[everyone["id"]])
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         An MFA Policy can be imported via the Okta ID.
 
         ```sh
         $ pulumi import okta:policy/mfa:Mfa example &#60;policy id&#62;
```

### Comparing `pulumi_okta-4.9.0a1713462165/pulumi_okta/policy/outputs.py` & `pulumi_okta-4.9.0a1713902092/pulumi_okta/policy/outputs.py`

 * *Files 9% similar despite different names*

```diff
@@ -24,71 +24,67 @@
 @pulumi.output_type
 class RuleIdpDiscoveryAppExclude(dict):
     def __init__(__self__, *,
                  type: str,
                  id: Optional[str] = None,
                  name: Optional[str] = None):
         """
-        :param str type: One of: `"ANY"`, `"MOBILE"`, `"DESKTOP"`
-        :param str id: Use if `type` is `"APP"` to indicate the application id to include.
-        :param str name: Use if the `type` is `"APP_TYPE"` to indicate the type of application(s) to include in instances where an entire group (i.e. `yahoo_mail`) of applications should be included.
+        :param str id: ID of the Rule.
+        :param str name: Policy rule name.
         """
         pulumi.set(__self__, "type", type)
         if id is not None:
             pulumi.set(__self__, "id", id)
         if name is not None:
             pulumi.set(__self__, "name", name)
 
     @property
     @pulumi.getter
     def type(self) -> str:
-        """
-        One of: `"ANY"`, `"MOBILE"`, `"DESKTOP"`
-        """
         return pulumi.get(self, "type")
 
     @property
     @pulumi.getter
     def id(self) -> Optional[str]:
         """
-        Use if `type` is `"APP"` to indicate the application id to include.
+        ID of the Rule.
         """
         return pulumi.get(self, "id")
 
     @property
     @pulumi.getter
     def name(self) -> Optional[str]:
         """
-        Use if the `type` is `"APP_TYPE"` to indicate the type of application(s) to include in instances where an entire group (i.e. `yahoo_mail`) of applications should be included.
+        Policy rule name.
         """
         return pulumi.get(self, "name")
 
 
 @pulumi.output_type
 class RuleIdpDiscoveryAppInclude(dict):
     def __init__(__self__, *,
                  type: str,
                  id: Optional[str] = None,
                  name: Optional[str] = None):
         """
-        :param str type: One of: `"ANY"`, `"MOBILE"`, `"DESKTOP"`
+        :param str type: One of: `"APP"`, `"APP_TYPE"`
         :param str id: Use if `type` is `"APP"` to indicate the application id to include.
         :param str name: Use if the `type` is `"APP_TYPE"` to indicate the type of application(s) to include in instances where an entire group (i.e. `yahoo_mail`) of applications should be included.
         """
         pulumi.set(__self__, "type", type)
         if id is not None:
             pulumi.set(__self__, "id", id)
         if name is not None:
             pulumi.set(__self__, "name", name)
 
     @property
     @pulumi.getter
     def type(self) -> str:
         """
-        One of: `"ANY"`, `"MOBILE"`, `"DESKTOP"`
+        One of: `"APP"`, `"APP_TYPE"`
         """
         return pulumi.get(self, "type")
 
     @property
     @pulumi.getter
     def id(self) -> Optional[str]:
         """
@@ -218,45 +214,41 @@
 @pulumi.output_type
 class RuleMfaAppExclude(dict):
     def __init__(__self__, *,
                  type: str,
                  id: Optional[str] = None,
                  name: Optional[str] = None):
         """
-        :param str type: One of: `"APP"`, `"APP_TYPE"`
-        :param str id: Use if `type` is `"APP"` to indicate the application id to include.
-        :param str name: Use if the `type` is `"APP_TYPE"` to indicate the type of application(s) to include in instances where an entire group (i.e. `yahoo_mail`) of applications should be included.
+        :param str id: ID of the Rule.
+        :param str name: Policy Rule Name.
         """
         pulumi.set(__self__, "type", type)
         if id is not None:
             pulumi.set(__self__, "id", id)
         if name is not None:
             pulumi.set(__self__, "name", name)
 
     @property
     @pulumi.getter
     def type(self) -> str:
-        """
-        One of: `"APP"`, `"APP_TYPE"`
-        """
         return pulumi.get(self, "type")
 
     @property
     @pulumi.getter
     def id(self) -> Optional[str]:
         """
-        Use if `type` is `"APP"` to indicate the application id to include.
+        ID of the Rule.
         """
         return pulumi.get(self, "id")
 
     @property
     @pulumi.getter
     def name(self) -> Optional[str]:
         """
-        Use if the `type` is `"APP_TYPE"` to indicate the type of application(s) to include in instances where an entire group (i.e. `yahoo_mail`) of applications should be included.
+        Policy Rule Name.
         """
         return pulumi.get(self, "name")
 
 
 @pulumi.output_type
 class RuleMfaAppInclude(dict):
     def __init__(__self__, *,
@@ -380,30 +372,30 @@
         RuleSignonFactorSequenceSecondaryCriteria.__key_warning(key)
         return super().get(key, default)
 
     def __init__(__self__, *,
                  factor_type: str,
                  provider: str):
         """
-        :param str factor_type: Factor type of the additional authentication step.
-        :param str provider: Provider of the additional authentication step.
+        :param str factor_type: Type of a Factor
+        :param str provider: Factor provider
         """
         pulumi.set(__self__, "factor_type", factor_type)
         pulumi.set(__self__, "provider", provider)
 
     @property
     @pulumi.getter(name="factorType")
     def factor_type(self) -> str:
         """
-        Factor type of the additional authentication step.
+        Type of a Factor
         """
         return pulumi.get(self, "factor_type")
 
     @property
     @pulumi.getter
     def provider(self) -> str:
         """
-        Provider of the additional authentication step.
+        Factor provider
         """
         return pulumi.get(self, "provider")
```

### Comparing `pulumi_okta-4.9.0a1713462165/pulumi_okta/policy/password.py` & `pulumi_okta-4.9.0a1713902092/pulumi_okta/policy/password.py`

 * *Files 1% similar despite different names*

```diff
@@ -1026,27 +1026,25 @@
         """
         Creates a Password Policy.
 
         This resource allows you to create and configure a Password Policy.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_okta as okta
 
         example = okta.policy.Password("example",
             name="example",
             status="ACTIVE",
             description="Example",
             password_history_count=4,
             groups_includeds=[everyone["id"]])
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         A Password Policy can be imported via the Okta ID.
 
         ```sh
         $ pulumi import okta:policy/password:Password example &#60;policy id&#62;
@@ -1094,27 +1092,25 @@
         """
         Creates a Password Policy.
 
         This resource allows you to create and configure a Password Policy.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_okta as okta
 
         example = okta.policy.Password("example",
             name="example",
             status="ACTIVE",
             description="Example",
             password_history_count=4,
             groups_includeds=[everyone["id"]])
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         A Password Policy can be imported via the Okta ID.
 
         ```sh
         $ pulumi import okta:policy/password:Password example &#60;policy id&#62;
```

### Comparing `pulumi_okta-4.9.0a1713462165/pulumi_okta/policy/rule_idp_discovery.py` & `pulumi_okta-4.9.0a1713902092/pulumi_okta/policy/rule_idp_discovery.py`

 * *Files 3% similar despite different names*

```diff
@@ -33,15 +33,15 @@
                  user_identifier_type: Optional[pulumi.Input[str]] = None):
         """
         The set of arguments for constructing a RuleIdpDiscovery resource.
         :param pulumi.Input[Sequence[pulumi.Input['RuleIdpDiscoveryAppExcludeArgs']]] app_excludes: Applications to exclude in discovery. See `app_include` for details.
         :param pulumi.Input[Sequence[pulumi.Input['RuleIdpDiscoveryAppIncludeArgs']]] app_includes: Applications to include in discovery rule.
         :param pulumi.Input[str] idp_id: The identifier for the Idp the rule should route to if all conditions are met.
         :param pulumi.Input[str] idp_type: Type of Idp. One of: `"SAML2"`, `"IWA"`, `"AgentlessDSSO"`, `"X509"`, `"FACEBOOK"`, `"GOOGLE"`, `"LINKEDIN"`, `"MICROSOFT"`, `"OIDC"`
-        :param pulumi.Input[str] name: Use if the `type` is `"APP_TYPE"` to indicate the type of application(s) to include in instances where an entire group (i.e. `yahoo_mail`) of applications should be included.
+        :param pulumi.Input[str] name: Policy rule name.
         :param pulumi.Input[str] network_connection: The network selection mode. One of `"ANYWEHRE"` or `"ZONE"`.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] network_excludes: Required if `network_connection` = `"ZONE"`. Indicates the network zones to exclude.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] network_includes: Required if `network_connection` = `"ZONE"`. Indicates the network zones to include.
         :param pulumi.Input[Sequence[pulumi.Input['RuleIdpDiscoveryPlatformIncludeArgs']]] platform_includes: Platform to include in discovery rule. - 'type' - (Optional) One of: 'ANY', 'MOBILE', 'DESKTOP' - 'os_expression -
                (Optional) Only available when using os_type = 'OTHER' - 'os_type' - (Optional) One of: 'ANY', 'IOS', 'WINDOWS',
                'ANDROID', 'OTHER', 'OSX'
         :param pulumi.Input[str] policy_id: Policy ID.
@@ -130,15 +130,15 @@
     def idp_type(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "idp_type", value)
 
     @property
     @pulumi.getter
     def name(self) -> Optional[pulumi.Input[str]]:
         """
-        Use if the `type` is `"APP_TYPE"` to indicate the type of application(s) to include in instances where an entire group (i.e. `yahoo_mail`) of applications should be included.
+        Policy rule name.
         """
         return pulumi.get(self, "name")
 
     @name.setter
     def name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "name", value)
 
@@ -285,15 +285,15 @@
                  user_identifier_type: Optional[pulumi.Input[str]] = None):
         """
         Input properties used for looking up and filtering RuleIdpDiscovery resources.
         :param pulumi.Input[Sequence[pulumi.Input['RuleIdpDiscoveryAppExcludeArgs']]] app_excludes: Applications to exclude in discovery. See `app_include` for details.
         :param pulumi.Input[Sequence[pulumi.Input['RuleIdpDiscoveryAppIncludeArgs']]] app_includes: Applications to include in discovery rule.
         :param pulumi.Input[str] idp_id: The identifier for the Idp the rule should route to if all conditions are met.
         :param pulumi.Input[str] idp_type: Type of Idp. One of: `"SAML2"`, `"IWA"`, `"AgentlessDSSO"`, `"X509"`, `"FACEBOOK"`, `"GOOGLE"`, `"LINKEDIN"`, `"MICROSOFT"`, `"OIDC"`
-        :param pulumi.Input[str] name: Use if the `type` is `"APP_TYPE"` to indicate the type of application(s) to include in instances where an entire group (i.e. `yahoo_mail`) of applications should be included.
+        :param pulumi.Input[str] name: Policy rule name.
         :param pulumi.Input[str] network_connection: The network selection mode. One of `"ANYWEHRE"` or `"ZONE"`.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] network_excludes: Required if `network_connection` = `"ZONE"`. Indicates the network zones to exclude.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] network_includes: Required if `network_connection` = `"ZONE"`. Indicates the network zones to include.
         :param pulumi.Input[Sequence[pulumi.Input['RuleIdpDiscoveryPlatformIncludeArgs']]] platform_includes: Platform to include in discovery rule. - 'type' - (Optional) One of: 'ANY', 'MOBILE', 'DESKTOP' - 'os_expression -
                (Optional) Only available when using os_type = 'OTHER' - 'os_type' - (Optional) One of: 'ANY', 'IOS', 'WINDOWS',
                'ANDROID', 'OTHER', 'OSX'
         :param pulumi.Input[str] policy_id: Policy ID.
@@ -382,15 +382,15 @@
     def idp_type(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "idp_type", value)
 
     @property
     @pulumi.getter
     def name(self) -> Optional[pulumi.Input[str]]:
         """
-        Use if the `type` is `"APP_TYPE"` to indicate the type of application(s) to include in instances where an entire group (i.e. `yahoo_mail`) of applications should be included.
+        Policy rule name.
         """
         return pulumi.get(self, "name")
 
     @name.setter
     def name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "name", value)
 
@@ -543,15 +543,14 @@
 
         > If you receive the error `You do not have permission to access the feature
         you are requesting` contact support and
         request feature flag `ADVANCED_SSO` be applied to your org.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_okta as okta
 
         # All Okta orgs contain only one IdP Discovery Policy
         idp_discovery_policy = okta.policy.get_policy(name="Idp Discovery Policy",
             type="IDP_DISCOVERY")
@@ -590,15 +589,14 @@
                 os_type="OSX",
             )],
             user_identifier_patterns=[okta.policy.RuleIdpDiscoveryUserIdentifierPatternArgs(
                 match_type="EQUALS",
                 value="Articulate",
             )])
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         A Policy Rule can be imported via the Policy and Rule ID.
 
         ```sh
         $ pulumi import okta:policy/ruleIdpDiscovery:RuleIdpDiscovery example &#60;policy id&#62;/&#60;rule id&#62;
@@ -606,15 +604,15 @@
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['RuleIdpDiscoveryAppExcludeArgs']]]] app_excludes: Applications to exclude in discovery. See `app_include` for details.
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['RuleIdpDiscoveryAppIncludeArgs']]]] app_includes: Applications to include in discovery rule.
         :param pulumi.Input[str] idp_id: The identifier for the Idp the rule should route to if all conditions are met.
         :param pulumi.Input[str] idp_type: Type of Idp. One of: `"SAML2"`, `"IWA"`, `"AgentlessDSSO"`, `"X509"`, `"FACEBOOK"`, `"GOOGLE"`, `"LINKEDIN"`, `"MICROSOFT"`, `"OIDC"`
-        :param pulumi.Input[str] name: Use if the `type` is `"APP_TYPE"` to indicate the type of application(s) to include in instances where an entire group (i.e. `yahoo_mail`) of applications should be included.
+        :param pulumi.Input[str] name: Policy rule name.
         :param pulumi.Input[str] network_connection: The network selection mode. One of `"ANYWEHRE"` or `"ZONE"`.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] network_excludes: Required if `network_connection` = `"ZONE"`. Indicates the network zones to exclude.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] network_includes: Required if `network_connection` = `"ZONE"`. Indicates the network zones to include.
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['RuleIdpDiscoveryPlatformIncludeArgs']]]] platform_includes: Platform to include in discovery rule. - 'type' - (Optional) One of: 'ANY', 'MOBILE', 'DESKTOP' - 'os_expression -
                (Optional) Only available when using os_type = 'OTHER' - 'os_type' - (Optional) One of: 'ANY', 'IOS', 'WINDOWS',
                'ANDROID', 'OTHER', 'OSX'
         :param pulumi.Input[str] policy_id: Policy ID.
@@ -635,15 +633,14 @@
 
         > If you receive the error `You do not have permission to access the feature
         you are requesting` contact support and
         request feature flag `ADVANCED_SSO` be applied to your org.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_okta as okta
 
         # All Okta orgs contain only one IdP Discovery Policy
         idp_discovery_policy = okta.policy.get_policy(name="Idp Discovery Policy",
             type="IDP_DISCOVERY")
@@ -682,15 +679,14 @@
                 os_type="OSX",
             )],
             user_identifier_patterns=[okta.policy.RuleIdpDiscoveryUserIdentifierPatternArgs(
                 match_type="EQUALS",
                 value="Articulate",
             )])
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         A Policy Rule can be imported via the Policy and Rule ID.
 
         ```sh
         $ pulumi import okta:policy/ruleIdpDiscovery:RuleIdpDiscovery example &#60;policy id&#62;/&#60;rule id&#62;
@@ -782,15 +778,15 @@
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['RuleIdpDiscoveryAppExcludeArgs']]]] app_excludes: Applications to exclude in discovery. See `app_include` for details.
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['RuleIdpDiscoveryAppIncludeArgs']]]] app_includes: Applications to include in discovery rule.
         :param pulumi.Input[str] idp_id: The identifier for the Idp the rule should route to if all conditions are met.
         :param pulumi.Input[str] idp_type: Type of Idp. One of: `"SAML2"`, `"IWA"`, `"AgentlessDSSO"`, `"X509"`, `"FACEBOOK"`, `"GOOGLE"`, `"LINKEDIN"`, `"MICROSOFT"`, `"OIDC"`
-        :param pulumi.Input[str] name: Use if the `type` is `"APP_TYPE"` to indicate the type of application(s) to include in instances where an entire group (i.e. `yahoo_mail`) of applications should be included.
+        :param pulumi.Input[str] name: Policy rule name.
         :param pulumi.Input[str] network_connection: The network selection mode. One of `"ANYWEHRE"` or `"ZONE"`.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] network_excludes: Required if `network_connection` = `"ZONE"`. Indicates the network zones to exclude.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] network_includes: Required if `network_connection` = `"ZONE"`. Indicates the network zones to include.
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['RuleIdpDiscoveryPlatformIncludeArgs']]]] platform_includes: Platform to include in discovery rule. - 'type' - (Optional) One of: 'ANY', 'MOBILE', 'DESKTOP' - 'os_expression -
                (Optional) Only available when using os_type = 'OTHER' - 'os_type' - (Optional) One of: 'ANY', 'IOS', 'WINDOWS',
                'ANDROID', 'OTHER', 'OSX'
         :param pulumi.Input[str] policy_id: Policy ID.
@@ -853,15 +849,15 @@
         """
         return pulumi.get(self, "idp_type")
 
     @property
     @pulumi.getter
     def name(self) -> pulumi.Output[str]:
         """
-        Use if the `type` is `"APP_TYPE"` to indicate the type of application(s) to include in instances where an entire group (i.e. `yahoo_mail`) of applications should be included.
+        Policy rule name.
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter(name="networkConnection")
     def network_connection(self) -> pulumi.Output[Optional[str]]:
         """
```

### Comparing `pulumi_okta-4.9.0a1713462165/pulumi_okta/policy/rule_mfa.py` & `pulumi_okta-4.9.0a1713902092/pulumi_okta/policy/rule_mfa.py`

 * *Files 5% similar despite different names*

```diff
@@ -31,15 +31,15 @@
         The set of arguments for constructing a RuleMfa resource.
         :param pulumi.Input[Sequence[pulumi.Input['RuleMfaAppExcludeArgs']]] app_excludes: Applications to exclude in discovery rule. **IMPORTANT**: this field is only available in Classic Organizations. - 'id'
                - (Optional) Use if 'type' is 'APP' to indicate the application id to include. - 'name' - (Optional) Use if the 'type'
                is 'APP_TYPE' to indicate the type of application(s) to include in instances where an entire group (i.e. 'yahoo_mail')
                of applications should be included. - 'type' - (Required) One of: 'APP', 'APP_TYPE'
         :param pulumi.Input[Sequence[pulumi.Input['RuleMfaAppIncludeArgs']]] app_includes: Applications to include in discovery rule. **IMPORTANT**: this field is only available in Classic Organizations.
         :param pulumi.Input[str] enroll: When a user should be prompted for MFA. It can be `"CHALLENGE"`, `"LOGIN"`, or `"NEVER"`.
-        :param pulumi.Input[str] name: Use if the `type` is `"APP_TYPE"` to indicate the type of application(s) to include in instances where an entire group (i.e. `yahoo_mail`) of applications should be included.
+        :param pulumi.Input[str] name: Policy Rule Name.
         :param pulumi.Input[str] network_connection: Network selection mode: `"ANYWHERE"`, `"ZONE"`, `"ON_NETWORK"`, or `"OFF_NETWORK"`.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] network_excludes: The network zones to exclude. Conflicts with `network_includes`.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] network_includes: The network zones to include. Conflicts with `network_excludes`.
         :param pulumi.Input[str] policy_id: Policy ID.
         :param pulumi.Input[int] priority: Policy Rule Priority, this attribute can be set to a valid priority. To avoid endless diff situation we error if an invalid priority is provided. API defaults it to the last (lowest) if not there.
         :param pulumi.Input[str] status: Policy Rule Status: `"ACTIVE"` or `"INACTIVE"`.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] users_excludeds: Set of User IDs to Exclude
@@ -106,15 +106,15 @@
     def enroll(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "enroll", value)
 
     @property
     @pulumi.getter
     def name(self) -> Optional[pulumi.Input[str]]:
         """
-        Use if the `type` is `"APP_TYPE"` to indicate the type of application(s) to include in instances where an entire group (i.e. `yahoo_mail`) of applications should be included.
+        Policy Rule Name.
         """
         return pulumi.get(self, "name")
 
     @name.setter
     def name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "name", value)
 
@@ -221,15 +221,15 @@
         Input properties used for looking up and filtering RuleMfa resources.
         :param pulumi.Input[Sequence[pulumi.Input['RuleMfaAppExcludeArgs']]] app_excludes: Applications to exclude in discovery rule. **IMPORTANT**: this field is only available in Classic Organizations. - 'id'
                - (Optional) Use if 'type' is 'APP' to indicate the application id to include. - 'name' - (Optional) Use if the 'type'
                is 'APP_TYPE' to indicate the type of application(s) to include in instances where an entire group (i.e. 'yahoo_mail')
                of applications should be included. - 'type' - (Required) One of: 'APP', 'APP_TYPE'
         :param pulumi.Input[Sequence[pulumi.Input['RuleMfaAppIncludeArgs']]] app_includes: Applications to include in discovery rule. **IMPORTANT**: this field is only available in Classic Organizations.
         :param pulumi.Input[str] enroll: When a user should be prompted for MFA. It can be `"CHALLENGE"`, `"LOGIN"`, or `"NEVER"`.
-        :param pulumi.Input[str] name: Use if the `type` is `"APP_TYPE"` to indicate the type of application(s) to include in instances where an entire group (i.e. `yahoo_mail`) of applications should be included.
+        :param pulumi.Input[str] name: Policy Rule Name.
         :param pulumi.Input[str] network_connection: Network selection mode: `"ANYWHERE"`, `"ZONE"`, `"ON_NETWORK"`, or `"OFF_NETWORK"`.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] network_excludes: The network zones to exclude. Conflicts with `network_includes`.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] network_includes: The network zones to include. Conflicts with `network_excludes`.
         :param pulumi.Input[str] policy_id: Policy ID.
         :param pulumi.Input[int] priority: Policy Rule Priority, this attribute can be set to a valid priority. To avoid endless diff situation we error if an invalid priority is provided. API defaults it to the last (lowest) if not there.
         :param pulumi.Input[str] status: Policy Rule Status: `"ACTIVE"` or `"INACTIVE"`.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] users_excludeds: Set of User IDs to Exclude
@@ -296,15 +296,15 @@
     def enroll(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "enroll", value)
 
     @property
     @pulumi.getter
     def name(self) -> Optional[pulumi.Input[str]]:
         """
-        Use if the `type` is `"APP_TYPE"` to indicate the type of application(s) to include in instances where an entire group (i.e. `yahoo_mail`) of applications should be included.
+        Policy Rule Name.
         """
         return pulumi.get(self, "name")
 
     @name.setter
     def name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "name", value)
 
@@ -425,15 +425,15 @@
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['RuleMfaAppExcludeArgs']]]] app_excludes: Applications to exclude in discovery rule. **IMPORTANT**: this field is only available in Classic Organizations. - 'id'
                - (Optional) Use if 'type' is 'APP' to indicate the application id to include. - 'name' - (Optional) Use if the 'type'
                is 'APP_TYPE' to indicate the type of application(s) to include in instances where an entire group (i.e. 'yahoo_mail')
                of applications should be included. - 'type' - (Required) One of: 'APP', 'APP_TYPE'
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['RuleMfaAppIncludeArgs']]]] app_includes: Applications to include in discovery rule. **IMPORTANT**: this field is only available in Classic Organizations.
         :param pulumi.Input[str] enroll: When a user should be prompted for MFA. It can be `"CHALLENGE"`, `"LOGIN"`, or `"NEVER"`.
-        :param pulumi.Input[str] name: Use if the `type` is `"APP_TYPE"` to indicate the type of application(s) to include in instances where an entire group (i.e. `yahoo_mail`) of applications should be included.
+        :param pulumi.Input[str] name: Policy Rule Name.
         :param pulumi.Input[str] network_connection: Network selection mode: `"ANYWHERE"`, `"ZONE"`, `"ON_NETWORK"`, or `"OFF_NETWORK"`.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] network_excludes: The network zones to exclude. Conflicts with `network_includes`.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] network_includes: The network zones to include. Conflicts with `network_excludes`.
         :param pulumi.Input[str] policy_id: Policy ID.
         :param pulumi.Input[int] priority: Policy Rule Priority, this attribute can be set to a valid priority. To avoid endless diff situation we error if an invalid priority is provided. API defaults it to the last (lowest) if not there.
         :param pulumi.Input[str] status: Policy Rule Status: `"ACTIVE"` or `"INACTIVE"`.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] users_excludeds: Set of User IDs to Exclude
@@ -531,15 +531,15 @@
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['RuleMfaAppExcludeArgs']]]] app_excludes: Applications to exclude in discovery rule. **IMPORTANT**: this field is only available in Classic Organizations. - 'id'
                - (Optional) Use if 'type' is 'APP' to indicate the application id to include. - 'name' - (Optional) Use if the 'type'
                is 'APP_TYPE' to indicate the type of application(s) to include in instances where an entire group (i.e. 'yahoo_mail')
                of applications should be included. - 'type' - (Required) One of: 'APP', 'APP_TYPE'
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['RuleMfaAppIncludeArgs']]]] app_includes: Applications to include in discovery rule. **IMPORTANT**: this field is only available in Classic Organizations.
         :param pulumi.Input[str] enroll: When a user should be prompted for MFA. It can be `"CHALLENGE"`, `"LOGIN"`, or `"NEVER"`.
-        :param pulumi.Input[str] name: Use if the `type` is `"APP_TYPE"` to indicate the type of application(s) to include in instances where an entire group (i.e. `yahoo_mail`) of applications should be included.
+        :param pulumi.Input[str] name: Policy Rule Name.
         :param pulumi.Input[str] network_connection: Network selection mode: `"ANYWHERE"`, `"ZONE"`, `"ON_NETWORK"`, or `"OFF_NETWORK"`.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] network_excludes: The network zones to exclude. Conflicts with `network_includes`.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] network_includes: The network zones to include. Conflicts with `network_excludes`.
         :param pulumi.Input[str] policy_id: Policy ID.
         :param pulumi.Input[int] priority: Policy Rule Priority, this attribute can be set to a valid priority. To avoid endless diff situation we error if an invalid priority is provided. API defaults it to the last (lowest) if not there.
         :param pulumi.Input[str] status: Policy Rule Status: `"ACTIVE"` or `"INACTIVE"`.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] users_excludeds: Set of User IDs to Exclude
@@ -588,15 +588,15 @@
         """
         return pulumi.get(self, "enroll")
 
     @property
     @pulumi.getter
     def name(self) -> pulumi.Output[str]:
         """
-        Use if the `type` is `"APP_TYPE"` to indicate the type of application(s) to include in instances where an entire group (i.e. `yahoo_mail`) of applications should be included.
+        Policy Rule Name.
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter(name="networkConnection")
     def network_connection(self) -> pulumi.Output[Optional[str]]:
         """
```

### Comparing `pulumi_okta-4.9.0a1713462165/pulumi_okta/policy/rule_password.py` & `pulumi_okta-4.9.0a1713902092/pulumi_okta/policy/rule_password.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713462165/pulumi_okta/policy/rule_signon.py` & `pulumi_okta-4.9.0a1713902092/pulumi_okta/policy/rule_signon.py`

 * *Files 0% similar despite different names*

```diff
@@ -857,15 +857,14 @@
                  __props__=None):
         """
         Creates a Sign On Policy Rule. In case `Invalid condition type specified: riskScore.` error is thrown, set `risc_level`
         to an empty string, since this feature is not enabled.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_okta as okta
 
         test = okta.policy.Signon("test",
             name="Example Policy",
             status="ACTIVE",
@@ -933,15 +932,14 @@
                 ),
                 okta.policy.RuleSignonFactorSequenceArgs(
                     primary_criteria_factor_type="token:software:totp",
                     primary_criteria_provider="OKTA",
                 ),
             ])
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         A Policy Rule can be imported via the Policy and Rule ID.
 
         ```sh
         $ pulumi import okta:policy/ruleSignon:RuleSignon example &#60;policy id&#62;/&#60;rule id&#62;
@@ -986,15 +984,14 @@
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         Creates a Sign On Policy Rule. In case `Invalid condition type specified: riskScore.` error is thrown, set `risc_level`
         to an empty string, since this feature is not enabled.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_okta as okta
 
         test = okta.policy.Signon("test",
             name="Example Policy",
             status="ACTIVE",
@@ -1062,15 +1059,14 @@
                 ),
                 okta.policy.RuleSignonFactorSequenceArgs(
                     primary_criteria_factor_type="token:software:totp",
                     primary_criteria_provider="OKTA",
                 ),
             ])
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         A Policy Rule can be imported via the Policy and Rule ID.
 
         ```sh
         $ pulumi import okta:policy/ruleSignon:RuleSignon example &#60;policy id&#62;/&#60;rule id&#62;
```

### Comparing `pulumi_okta-4.9.0a1713462165/pulumi_okta/policy/signon.py` & `pulumi_okta-4.9.0a1713902092/pulumi_okta/policy/signon.py`

 * *Files 2% similar despite different names*

```diff
@@ -201,26 +201,24 @@
         """
         Creates a Sign On Policy.
 
         This resource allows you to create and configure a Sign On Policy.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_okta as okta
 
         example = okta.policy.Signon("example",
             name="example",
             status="ACTIVE",
             description="Example",
             groups_includeds=[everyone["id"]])
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         A Sign On Policy can be imported via the Okta ID.
 
         ```sh
         $ pulumi import okta:policy/signon:Signon example &#60;policy id&#62;
@@ -243,26 +241,24 @@
         """
         Creates a Sign On Policy.
 
         This resource allows you to create and configure a Sign On Policy.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_okta as okta
 
         example = okta.policy.Signon("example",
             name="example",
             status="ACTIVE",
             description="Example",
             groups_includeds=[everyone["id"]])
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         A Sign On Policy can be imported via the Okta ID.
 
         ```sh
         $ pulumi import okta:policy/signon:Signon example &#60;policy id&#62;
```

### Comparing `pulumi_okta-4.9.0a1713462165/pulumi_okta/policy_mfa_default.py` & `pulumi_okta-4.9.0a1713902092/pulumi_okta/policy_mfa_default.py`

 * *Files 0% similar despite different names*

```diff
@@ -850,15 +850,14 @@
 
         > Requires Org Feature Flag `OKTA_MFA_POLICY`. Contact support to have this feature flag ***enabled***.
 
         > Unless Org Feature Flag `ENG_ENABLE_OPTIONAL_PASSWORD_ENROLLMENT` is ***disabled*** `okta_password` or `okta_email` must be present and its `enroll` value set to `REQUIRED`. Contact support to have this feature flag ***disabled***.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_okta as okta
 
         classic_example = okta.PolicyMfaDefault("classic_example",
             is_oie=False,
             okta_password={
@@ -872,15 +871,14 @@
             okta_password={
                 "enroll": "REQUIRED",
             },
             okta_verify={
                 "enroll": "REQUIRED",
             })
         ```
-        <!--End PulumiCodeChooser -->
 
         > If the `PolicyMfaDefault` is used in conjunction with `policy.Mfa` resources, ensure to use a `depends_on` attribute for the default policy to ensure that all other policies are created/updated first such that the `priority` field can be appropriately computed on the first plan/apply.
 
         ## Import
 
         Default MFA Policy can be imported without providing Okta ID.
 
@@ -927,15 +925,14 @@
 
         > Requires Org Feature Flag `OKTA_MFA_POLICY`. Contact support to have this feature flag ***enabled***.
 
         > Unless Org Feature Flag `ENG_ENABLE_OPTIONAL_PASSWORD_ENROLLMENT` is ***disabled*** `okta_password` or `okta_email` must be present and its `enroll` value set to `REQUIRED`. Contact support to have this feature flag ***disabled***.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_okta as okta
 
         classic_example = okta.PolicyMfaDefault("classic_example",
             is_oie=False,
             okta_password={
@@ -949,15 +946,14 @@
             okta_password={
                 "enroll": "REQUIRED",
             },
             okta_verify={
                 "enroll": "REQUIRED",
             })
         ```
-        <!--End PulumiCodeChooser -->
 
         > If the `PolicyMfaDefault` is used in conjunction with `policy.Mfa` resources, ensure to use a `depends_on` attribute for the default policy to ensure that all other policies are created/updated first such that the `priority` field can be appropriately computed on the first plan/apply.
 
         ## Import
 
         Default MFA Policy can be imported without providing Okta ID.
```

### Comparing `pulumi_okta-4.9.0a1713462165/pulumi_okta/policy_password_default.py` & `pulumi_okta-4.9.0a1713902092/pulumi_okta/policy_password_default.py`

 * *Files 1% similar despite different names*

```diff
@@ -940,22 +940,20 @@
         """
         Configures default password policy.
 
         This resource allows you to configure default password policy.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_okta as okta
 
         default = okta.PolicyPasswordDefault("default")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Default Password Policy can be imported without providing Okta ID.
 
         ```sh
         $ pulumi import okta:index/policyPasswordDefault:PolicyPasswordDefault example .
@@ -1001,22 +999,20 @@
         """
         Configures default password policy.
 
         This resource allows you to configure default password policy.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_okta as okta
 
         default = okta.PolicyPasswordDefault("default")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Default Password Policy can be imported without providing Okta ID.
 
         ```sh
         $ pulumi import okta:index/policyPasswordDefault:PolicyPasswordDefault example .
```

### Comparing `pulumi_okta-4.9.0a1713462165/pulumi_okta/policy_profile_enrollment.py` & `pulumi_okta-4.9.0a1713902092/pulumi_okta/policy_profile_enrollment.py`

 * *Files 8% similar despite different names*

```diff
@@ -102,24 +102,22 @@
         """
         > **WARNING:** This feature is only available as a part of the Identity Engine. Contact support for further information.
 
         This resource allows you to create and configure a Profile Enrollment Policy.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_okta as okta
 
         example = okta.PolicyProfileEnrollment("example",
             name="example",
             status="ACTIVE")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         A Profile Enrollment Policy can be imported via the Okta ID.
 
         ```sh
         $ pulumi import okta:index/policyProfileEnrollment:PolicyProfileEnrollment example &#60;policy id&#62;
@@ -139,24 +137,22 @@
         """
         > **WARNING:** This feature is only available as a part of the Identity Engine. Contact support for further information.
 
         This resource allows you to create and configure a Profile Enrollment Policy.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_okta as okta
 
         example = okta.PolicyProfileEnrollment("example",
             name="example",
             status="ACTIVE")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         A Profile Enrollment Policy can be imported via the Okta ID.
 
         ```sh
         $ pulumi import okta:index/policyProfileEnrollment:PolicyProfileEnrollment example &#60;policy id&#62;
```

### Comparing `pulumi_okta-4.9.0a1713462165/pulumi_okta/policy_profile_enrollment_apps.py` & `pulumi_okta-4.9.0a1713902092/pulumi_okta/policy_profile_enrollment_apps.py`

 * *Files 2% similar despite different names*

```diff
@@ -122,27 +122,25 @@
         **Important Notes:**
          - Default Enrollment Policy can not be used in this resource since it is used as a policy to re-assign apps to when they are unassigned from this one.
          - When re-assigning the app to another policy, please use `depends_on` in the policy to which the app will be assigned. This is necessary to avoid
              unexpected behavior, since if the app is unassigned from the policy it is just assigned to the `Default` one.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_okta as okta
 
         example = okta.policy.get_policy(name="My Policy",
             type="PROFILE_ENROLLMENT")
         test = okta.app.get_app(label="My App")
         example_policy_profile_enrollment_apps = okta.PolicyProfileEnrollmentApps("example",
             policy_id=example_okta_policy["id"],
             apps=[id])
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         A Profile Enrollment Policy Apps can be imported via the Okta ID.
 
         ```sh
         $ pulumi import okta:index/policyProfileEnrollmentApps:PolicyProfileEnrollmentApps example &#60;policy id&#62;
@@ -167,27 +165,25 @@
         **Important Notes:**
          - Default Enrollment Policy can not be used in this resource since it is used as a policy to re-assign apps to when they are unassigned from this one.
          - When re-assigning the app to another policy, please use `depends_on` in the policy to which the app will be assigned. This is necessary to avoid
              unexpected behavior, since if the app is unassigned from the policy it is just assigned to the `Default` one.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_okta as okta
 
         example = okta.policy.get_policy(name="My Policy",
             type="PROFILE_ENROLLMENT")
         test = okta.app.get_app(label="My App")
         example_policy_profile_enrollment_apps = okta.PolicyProfileEnrollmentApps("example",
             policy_id=example_okta_policy["id"],
             apps=[id])
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         A Profile Enrollment Policy Apps can be imported via the Okta ID.
 
         ```sh
         $ pulumi import okta:index/policyProfileEnrollmentApps:PolicyProfileEnrollmentApps example &#60;policy id&#62;
```

### Comparing `pulumi_okta-4.9.0a1713462165/pulumi_okta/policy_rule_profile_enrollment.py` & `pulumi_okta-4.9.0a1713902092/pulumi_okta/policy_rule_profile_enrollment.py`

 * *Files 0% similar despite different names*

```diff
@@ -178,15 +178,15 @@
                  ui_schema_id: Optional[pulumi.Input[str]] = None,
                  unknown_user_action: Optional[pulumi.Input[str]] = None):
         """
         Input properties used for looking up and filtering PolicyRuleProfileEnrollment resources.
         :param pulumi.Input[str] access: Allow or deny access based on the rule conditions. Valid values are: `"ALLOW"`, `"DENY"`. Default is `"ALLOW"`.
         :param pulumi.Input[bool] email_verification: Indicates whether email verification should occur before access is granted. Default is `true`.
         :param pulumi.Input[str] inline_hook_id: ID of a Registration Inline Hook.
-        :param pulumi.Input[str] name: The name of a User Profile property
+        :param pulumi.Input[str] name: Name of the Rule.
         :param pulumi.Input[str] policy_id: Policy ID.
         :param pulumi.Input[Sequence[pulumi.Input['PolicyRuleProfileEnrollmentProfileAttributeArgs']]] profile_attributes: A list of attributes to prompt the user during registration or progressive profiling. Where defined on the User schema, these attributes are persisted in the User profile. Non-schema attributes may also be added, which aren't persisted to the User's profile, but are included in requests to the registration inline hook. A maximum of 10 Profile properties is supported.
         :param pulumi.Input[str] progressive_profiling_action: Enabled or disabled progressive profiling action rule conditions. Valid values are: `"ENABLED"`, `"DISABLED"`. Default is `"DISABLED"`.
         :param pulumi.Input[str] status: Status of the Rule.
         :param pulumi.Input[str] target_group_id: The ID of a Group that this User should be added to.
         :param pulumi.Input[str] ui_schema_id: Value created by the backend. If present all policy updates must include this attribute/value.
         :param pulumi.Input[str] unknown_user_action: Which action should be taken if this User is new. Valid values are: `"DENY"`, `"REGISTER"`.
@@ -250,15 +250,15 @@
     def inline_hook_id(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "inline_hook_id", value)
 
     @property
     @pulumi.getter
     def name(self) -> Optional[pulumi.Input[str]]:
         """
-        The name of a User Profile property
+        Name of the Rule.
         """
         return pulumi.get(self, "name")
 
     @name.setter
     def name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "name", value)
 
@@ -368,15 +368,14 @@
         A [profile enrollment
         policy](https://developer.okta.com/docs/reference/api/policy/#profile-enrollment-policy)
         is limited to one default rule. This resource does not create a rule for an
         enrollment policy, it allows the default policy rule to be updated.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_okta as okta
 
         example = okta.PolicyProfileEnrollment("example", name="My Enrollment Policy")
         example_hook = okta.inline.Hook("example",
             name="My Inline Hook",
@@ -413,15 +412,14 @@
                 okta.PolicyRuleProfileEnrollmentProfileAttributeArgs(
                     name="t-shirt",
                     label="T-Shirt Size",
                     required=False,
                 ),
             ])
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         A Policy Rule can be imported via the Policy and Rule ID.
 
         ```sh
         $ pulumi import okta:index/policyRuleProfileEnrollment:PolicyRuleProfileEnrollment example &#60;policy id&#62;/&#60;rule id&#62;
@@ -451,15 +449,14 @@
         A [profile enrollment
         policy](https://developer.okta.com/docs/reference/api/policy/#profile-enrollment-policy)
         is limited to one default rule. This resource does not create a rule for an
         enrollment policy, it allows the default policy rule to be updated.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_okta as okta
 
         example = okta.PolicyProfileEnrollment("example", name="My Enrollment Policy")
         example_hook = okta.inline.Hook("example",
             name="My Inline Hook",
@@ -496,15 +493,14 @@
                 okta.PolicyRuleProfileEnrollmentProfileAttributeArgs(
                     name="t-shirt",
                     label="T-Shirt Size",
                     required=False,
                 ),
             ])
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         A Policy Rule can be imported via the Policy and Rule ID.
 
         ```sh
         $ pulumi import okta:index/policyRuleProfileEnrollment:PolicyRuleProfileEnrollment example &#60;policy id&#62;/&#60;rule id&#62;
@@ -585,15 +581,15 @@
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] access: Allow or deny access based on the rule conditions. Valid values are: `"ALLOW"`, `"DENY"`. Default is `"ALLOW"`.
         :param pulumi.Input[bool] email_verification: Indicates whether email verification should occur before access is granted. Default is `true`.
         :param pulumi.Input[str] inline_hook_id: ID of a Registration Inline Hook.
-        :param pulumi.Input[str] name: The name of a User Profile property
+        :param pulumi.Input[str] name: Name of the Rule.
         :param pulumi.Input[str] policy_id: Policy ID.
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['PolicyRuleProfileEnrollmentProfileAttributeArgs']]]] profile_attributes: A list of attributes to prompt the user during registration or progressive profiling. Where defined on the User schema, these attributes are persisted in the User profile. Non-schema attributes may also be added, which aren't persisted to the User's profile, but are included in requests to the registration inline hook. A maximum of 10 Profile properties is supported.
         :param pulumi.Input[str] progressive_profiling_action: Enabled or disabled progressive profiling action rule conditions. Valid values are: `"ENABLED"`, `"DISABLED"`. Default is `"DISABLED"`.
         :param pulumi.Input[str] status: Status of the Rule.
         :param pulumi.Input[str] target_group_id: The ID of a Group that this User should be added to.
         :param pulumi.Input[str] ui_schema_id: Value created by the backend. If present all policy updates must include this attribute/value.
         :param pulumi.Input[str] unknown_user_action: Which action should be taken if this User is new. Valid values are: `"DENY"`, `"REGISTER"`.
@@ -639,15 +635,15 @@
         """
         return pulumi.get(self, "inline_hook_id")
 
     @property
     @pulumi.getter
     def name(self) -> pulumi.Output[str]:
         """
-        The name of a User Profile property
+        Name of the Rule.
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter(name="policyId")
     def policy_id(self) -> pulumi.Output[str]:
         """
```

### Comparing `pulumi_okta-4.9.0a1713462165/pulumi_okta/profile/_inputs.py` & `pulumi_okta-4.9.0a1713902092/pulumi_okta/profile/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713462165/pulumi_okta/profile/mapping.py` & `pulumi_okta-4.9.0a1713902092/pulumi_okta/profile/mapping.py`

 * *Files 1% similar despite different names*

```diff
@@ -281,15 +281,14 @@
         """
         This resource allows you to manage a profile mapping by source and target IDs.
 
         > **NOTE:** If using this resource with OAuth2 scopes, this resource requires `okta.profileMappings.manage` scope.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_okta as okta
 
         user = okta.user.get_user_profile_mapping_source()
         example = okta.profile.Mapping("example",
             source_id="<source id>",
@@ -310,15 +309,14 @@
                 ),
                 okta.profile.MappingMappingArgs(
                     id="login",
                     expression="appuser.email",
                 ),
             ])
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         There is no reason to import this resource. You can simply create the resource config and point it to a source ID. Mind here, once the source is deleted this resources will no longer exist.
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
@@ -341,15 +339,14 @@
         """
         This resource allows you to manage a profile mapping by source and target IDs.
 
         > **NOTE:** If using this resource with OAuth2 scopes, this resource requires `okta.profileMappings.manage` scope.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_okta as okta
 
         user = okta.user.get_user_profile_mapping_source()
         example = okta.profile.Mapping("example",
             source_id="<source id>",
@@ -370,15 +367,14 @@
                 ),
                 okta.profile.MappingMappingArgs(
                     id="login",
                     expression="appuser.email",
                 ),
             ])
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         There is no reason to import this resource. You can simply create the resource config and point it to a source ID. Mind here, once the source is deleted this resources will no longer exist.
 
         :param str resource_name: The name of the resource.
         :param MappingArgs args: The arguments to use to populate this resource's properties.
```

### Comparing `pulumi_okta-4.9.0a1713462165/pulumi_okta/profile/outputs.py` & `pulumi_okta-4.9.0a1713902092/pulumi_okta/profile/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713462165/pulumi_okta/provider.py` & `pulumi_okta-4.9.0a1713902092/pulumi_okta/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713462165/pulumi_okta/rate_limiting.py` & `pulumi_okta-4.9.0a1713902092/pulumi_okta/rate_limiting.py`

 * *Files 1% similar despite different names*

```diff
@@ -143,25 +143,23 @@
 
         > **WARNING:** This resource is available only when using a SSWS API token in the provider config, it is incompatible with OAuth 2.0 authentication.
 
         > **WARNING:** This resource makes use of an internal/private Okta API endpoint that could change without notice rendering this resource inoperable.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_okta as okta
 
         example = okta.RateLimiting("example",
             login="ENFORCE",
             authorize="ENFORCE",
             communications_enabled=True)
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Rate limit settings can be imported without any parameters.
 
         ```sh
         $ pulumi import okta:index/rateLimiting:RateLimiting example .
@@ -186,25 +184,23 @@
 
         > **WARNING:** This resource is available only when using a SSWS API token in the provider config, it is incompatible with OAuth 2.0 authentication.
 
         > **WARNING:** This resource makes use of an internal/private Okta API endpoint that could change without notice rendering this resource inoperable.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_okta as okta
 
         example = okta.RateLimiting("example",
             login="ENFORCE",
             authorize="ENFORCE",
             communications_enabled=True)
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Rate limit settings can be imported without any parameters.
 
         ```sh
         $ pulumi import okta:index/rateLimiting:RateLimiting example .
```

### Comparing `pulumi_okta-4.9.0a1713462165/pulumi_okta/resource_set.py` & `pulumi_okta-4.9.0a1713902092/pulumi_okta/resource_set.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713462165/pulumi_okta/role_subscription.py` & `pulumi_okta-4.9.0a1713902092/pulumi_okta/role_subscription.py`

 * *Files 2% similar despite different names*

```diff
@@ -233,25 +233,23 @@
         """
         This resource allows you to configure subscriptions of a Role with a specific type.
         Check [configure email notifications](https://help.okta.com/oie/en-us/Content/Topics/Security/custom-admin-role/administrator-email-settings.htm)
         page regarding what notifications are available for specific admin roles.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_okta as okta
 
         test = okta.RoleSubscription("test",
             role_type="SUPER_ADMIN",
             notification_type="APP_IMPORT",
             status="unsubscribed")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         A role subscription can be imported via the Okta ID.
 
         ```sh
         $ pulumi import okta:index/roleSubscription:RoleSubscription example &#60;role_type&#62;/&#60;notification_type&#62;
@@ -297,25 +295,23 @@
         """
         This resource allows you to configure subscriptions of a Role with a specific type.
         Check [configure email notifications](https://help.okta.com/oie/en-us/Content/Topics/Security/custom-admin-role/administrator-email-settings.htm)
         page regarding what notifications are available for specific admin roles.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_okta as okta
 
         test = okta.RoleSubscription("test",
             role_type="SUPER_ADMIN",
             notification_type="APP_IMPORT",
             status="unsubscribed")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         A role subscription can be imported via the Okta ID.
 
         ```sh
         $ pulumi import okta:index/roleSubscription:RoleSubscription example &#60;role_type&#62;/&#60;notification_type&#62;
```

### Comparing `pulumi_okta-4.9.0a1713462165/pulumi_okta/security_notification_emails.py` & `pulumi_okta-4.9.0a1713902092/pulumi_okta/security_notification_emails.py`

 * *Files 2% similar despite different names*

```diff
@@ -203,27 +203,25 @@
 
         > **WARNING:** This resource is available only when using a SSWS API token in the provider config, it is incompatible with OAuth 2.0 authentication.
 
         > **WARNING:** This resource makes use of an internal/private Okta API endpoint that could change without notice rendering this resource inoperable.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_okta as okta
 
         example = okta.SecurityNotificationEmails("example",
             report_suspicious_activity_enabled=True,
             send_email_for_factor_enrollment_enabled=True,
             send_email_for_factor_reset_enabled=True,
             send_email_for_new_device_enabled=True,
             send_email_for_password_changed_enabled=True)
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Security Notification Emails can be imported without any parameters.
 
         ```sh
         $ pulumi import okta:index/securityNotificationEmails:SecurityNotificationEmails example _
@@ -248,27 +246,25 @@
 
         > **WARNING:** This resource is available only when using a SSWS API token in the provider config, it is incompatible with OAuth 2.0 authentication.
 
         > **WARNING:** This resource makes use of an internal/private Okta API endpoint that could change without notice rendering this resource inoperable.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_okta as okta
 
         example = okta.SecurityNotificationEmails("example",
             report_suspicious_activity_enabled=True,
             send_email_for_factor_enrollment_enabled=True,
             send_email_for_factor_reset_enabled=True,
             send_email_for_new_device_enabled=True,
             send_email_for_password_changed_enabled=True)
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Security Notification Emails can be imported without any parameters.
 
         ```sh
         $ pulumi import okta:index/securityNotificationEmails:SecurityNotificationEmails example _
```

### Comparing `pulumi_okta-4.9.0a1713462165/pulumi_okta/template_sms.py` & `pulumi_okta-4.9.0a1713902092/pulumi_okta/template_sms.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,28 +17,28 @@
 class TemplateSmsArgs:
     def __init__(__self__, *,
                  template: pulumi.Input[str],
                  type: pulumi.Input[str],
                  translations: Optional[pulumi.Input[Sequence[pulumi.Input['TemplateSmsTranslationArgs']]]] = None):
         """
         The set of arguments for constructing a TemplateSms resource.
-        :param pulumi.Input[str] template: The SMS message.
+        :param pulumi.Input[str] template: Default SMS message
         :param pulumi.Input[str] type: SMS template type
         :param pulumi.Input[Sequence[pulumi.Input['TemplateSmsTranslationArgs']]] translations: Set of translations for a particular template.
         """
         pulumi.set(__self__, "template", template)
         pulumi.set(__self__, "type", type)
         if translations is not None:
             pulumi.set(__self__, "translations", translations)
 
     @property
     @pulumi.getter
     def template(self) -> pulumi.Input[str]:
         """
-        The SMS message.
+        Default SMS message
         """
         return pulumi.get(self, "template")
 
     @template.setter
     def template(self, value: pulumi.Input[str]):
         pulumi.set(self, "template", value)
 
@@ -71,30 +71,30 @@
 class _TemplateSmsState:
     def __init__(__self__, *,
                  template: Optional[pulumi.Input[str]] = None,
                  translations: Optional[pulumi.Input[Sequence[pulumi.Input['TemplateSmsTranslationArgs']]]] = None,
                  type: Optional[pulumi.Input[str]] = None):
         """
         Input properties used for looking up and filtering TemplateSms resources.
-        :param pulumi.Input[str] template: The SMS message.
+        :param pulumi.Input[str] template: Default SMS message
         :param pulumi.Input[Sequence[pulumi.Input['TemplateSmsTranslationArgs']]] translations: Set of translations for a particular template.
         :param pulumi.Input[str] type: SMS template type
         """
         if template is not None:
             pulumi.set(__self__, "template", template)
         if translations is not None:
             pulumi.set(__self__, "translations", translations)
         if type is not None:
             pulumi.set(__self__, "type", type)
 
     @property
     @pulumi.getter
     def template(self) -> Optional[pulumi.Input[str]]:
         """
-        The SMS message.
+        Default SMS message
         """
         return pulumi.get(self, "template")
 
     @template.setter
     def template(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "template", value)
 
@@ -135,15 +135,14 @@
         """
         Creates an Okta SMS Template.
 
         This resource allows you to create and configure an Okta SMS Template.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_okta as okta
 
         example = okta.TemplateSms("example",
             type="SMS_VERIFY_CODE",
             template="Your ${org.name} code is: ${code}",
@@ -154,27 +153,26 @@
                 ),
                 okta.TemplateSmsTranslationArgs(
                     language="es",
                     template="Tu código de ${org.name} es: ${code}.",
                 ),
             ])
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         An Okta SMS Template can be imported via the template type.
 
         ```sh
         $ pulumi import okta:index/templateSms:TemplateSms example &#60;template type&#62;
         ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[str] template: The SMS message.
+        :param pulumi.Input[str] template: Default SMS message
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['TemplateSmsTranslationArgs']]]] translations: Set of translations for a particular template.
         :param pulumi.Input[str] type: SMS template type
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
@@ -183,15 +181,14 @@
         """
         Creates an Okta SMS Template.
 
         This resource allows you to create and configure an Okta SMS Template.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_okta as okta
 
         example = okta.TemplateSms("example",
             type="SMS_VERIFY_CODE",
             template="Your ${org.name} code is: ${code}",
@@ -202,15 +199,14 @@
                 ),
                 okta.TemplateSmsTranslationArgs(
                     language="es",
                     template="Tu código de ${org.name} es: ${code}.",
                 ),
             ])
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         An Okta SMS Template can be imported via the template type.
 
         ```sh
         $ pulumi import okta:index/templateSms:TemplateSms example &#60;template type&#62;
@@ -266,15 +262,15 @@
         """
         Get an existing TemplateSms resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[str] template: The SMS message.
+        :param pulumi.Input[str] template: Default SMS message
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['TemplateSmsTranslationArgs']]]] translations: Set of translations for a particular template.
         :param pulumi.Input[str] type: SMS template type
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _TemplateSmsState.__new__(_TemplateSmsState)
 
@@ -283,15 +279,15 @@
         __props__.__dict__["type"] = type
         return TemplateSms(resource_name, opts=opts, __props__=__props__)
 
     @property
     @pulumi.getter
     def template(self) -> pulumi.Output[str]:
         """
-        The SMS message.
+        Default SMS message
         """
         return pulumi.get(self, "template")
 
     @property
     @pulumi.getter
     def translations(self) -> pulumi.Output[Optional[Sequence['outputs.TemplateSmsTranslation']]]:
         """
```

### Comparing `pulumi_okta-4.9.0a1713462165/pulumi_okta/theme.py` & `pulumi_okta-4.9.0a1713902092/pulumi_okta/theme.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713462165/pulumi_okta/threat_insight_settings.py` & `pulumi_okta-4.9.0a1713902092/pulumi_okta/threat_insight_settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -123,15 +123,14 @@
                  network_excludes: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  __props__=None):
         """
         This resource allows you to configure Threat Insight Settings.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_okta as okta
 
         ip_network_zone_example = okta.network.Zone("ip_network_zone_example",
             name="example",
             type="IP",
@@ -143,15 +142,14 @@
                 "2.2.3.4/24",
                 "3.3.4.5-3.3.4.15",
             ])
         example = okta.ThreatInsightSettings("example",
             action="block",
             network_excludes=[ip_network_zone_example.id])
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Threat Insight Settings can be imported without any parameters.
 
         ```sh
         $ pulumi import okta:index/threatInsightSettings:ThreatInsightSettings example _
@@ -175,15 +173,14 @@
                  args: ThreatInsightSettingsArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         This resource allows you to configure Threat Insight Settings.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_okta as okta
 
         ip_network_zone_example = okta.network.Zone("ip_network_zone_example",
             name="example",
             type="IP",
@@ -195,15 +192,14 @@
                 "2.2.3.4/24",
                 "3.3.4.5-3.3.4.15",
             ])
         example = okta.ThreatInsightSettings("example",
             action="block",
             network_excludes=[ip_network_zone_example.id])
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Threat Insight Settings can be imported without any parameters.
 
         ```sh
         $ pulumi import okta:index/threatInsightSettings:ThreatInsightSettings example _
```

### Comparing `pulumi_okta-4.9.0a1713462165/pulumi_okta/trustedorigin/origin.py` & `pulumi_okta-4.9.0a1713902092/pulumi_okta/trustedorigin/origin.py`

 * *Files 2% similar despite different names*

```diff
@@ -166,25 +166,23 @@
         """
         Creates a Trusted Origin.
 
         This resource allows you to create and configure a Trusted Origin.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_okta as okta
 
         example = okta.trustedorigin.Origin("example",
             name="example",
             origin="https://example.com",
             scopes=["CORS"])
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         A Trusted Origin can be imported via the Okta ID.
 
         ```sh
         $ pulumi import okta:trustedorigin/origin:Origin example &#60;trusted origin id&#62;
@@ -206,25 +204,23 @@
         """
         Creates a Trusted Origin.
 
         This resource allows you to create and configure a Trusted Origin.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_okta as okta
 
         example = okta.trustedorigin.Origin("example",
             name="example",
             origin="https://example.com",
             scopes=["CORS"])
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         A Trusted Origin can be imported via the Okta ID.
 
         ```sh
         $ pulumi import okta:trustedorigin/origin:Origin example &#60;trusted origin id&#62;
```

### Comparing `pulumi_okta-4.9.0a1713462165/pulumi_okta/user/_inputs.py` & `pulumi_okta-4.9.0a1713902092/pulumi_okta/user/_inputs.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,22 +21,18 @@
                  algorithm: pulumi.Input[str],
                  value: pulumi.Input[str],
                  salt: Optional[pulumi.Input[str]] = None,
                  salt_order: Optional[pulumi.Input[str]] = None,
                  work_factor: Optional[pulumi.Input[int]] = None):
         """
         :param pulumi.Input[str] algorithm: The algorithm used to generate the hash using the password
-        :param pulumi.Input[str] value: For SHA-512, SHA-256, SHA-1, MD5, this is the actual base64-encoded hash of the password (and salt, if used).
-               This is the Base64 encoded value of the SHA-512/SHA-256/SHA-1/MD5 digest that was computed by either pre-fixing or post-fixing
-               the salt to the password, depending on the saltOrder. If a salt was not used in the source system, then this should just be
-               the Base64 encoded value of the password's SHA-512/SHA-256/SHA-1/MD5 digest. For BCRYPT, This is the actual radix64-encoded hashed password.
-        :param pulumi.Input[str] salt: Only required for salted hashes. For BCRYPT, this specifies the radix64-encoded salt used to generate
-               the hash, which must be 22 characters long. For other salted hashes, this specifies the base64-encoded salt used to generate the hash.
-        :param pulumi.Input[str] salt_order: Specifies whether salt was pre- or postfixed to the password before hashing. Only required for salted algorithms.
-        :param pulumi.Input[int] work_factor: Governs the strength of the hash and the time required to compute it. Only required for BCRYPT algorithm. Minimum value is 1, and maximum is 20.
+        :param pulumi.Input[str] value: For SHA-512, SHA-256, SHA-1, MD5, This is the actual base64-encoded hash of the password (and salt, if used). This is the Base64 encoded value of the SHA-512/SHA-256/SHA-1/MD5 digest that was computed by either pre-fixing or post-fixing the salt to the password, depending on the saltOrder. If a salt was not used in the source system, then this should just be the the Base64 encoded value of the password's SHA-512/SHA-256/SHA-1/MD5 digest. For BCRYPT, This is the actual radix64-encoded hashed password.
+        :param pulumi.Input[str] salt: Only required for salted hashes
+        :param pulumi.Input[str] salt_order: Specifies whether salt was pre- or postfixed to the password before hashing
+        :param pulumi.Input[int] work_factor: Governs the strength of the hash and the time required to compute it. Only required for BCRYPT algorithm
         """
         pulumi.set(__self__, "algorithm", algorithm)
         pulumi.set(__self__, "value", value)
         if salt is not None:
             pulumi.set(__self__, "salt", salt)
         if salt_order is not None:
             pulumi.set(__self__, "salt_order", salt_order)
@@ -55,55 +51,51 @@
     def algorithm(self, value: pulumi.Input[str]):
         pulumi.set(self, "algorithm", value)
 
     @property
     @pulumi.getter
     def value(self) -> pulumi.Input[str]:
         """
-        For SHA-512, SHA-256, SHA-1, MD5, this is the actual base64-encoded hash of the password (and salt, if used).
-        This is the Base64 encoded value of the SHA-512/SHA-256/SHA-1/MD5 digest that was computed by either pre-fixing or post-fixing
-        the salt to the password, depending on the saltOrder. If a salt was not used in the source system, then this should just be
-        the Base64 encoded value of the password's SHA-512/SHA-256/SHA-1/MD5 digest. For BCRYPT, This is the actual radix64-encoded hashed password.
+        For SHA-512, SHA-256, SHA-1, MD5, This is the actual base64-encoded hash of the password (and salt, if used). This is the Base64 encoded value of the SHA-512/SHA-256/SHA-1/MD5 digest that was computed by either pre-fixing or post-fixing the salt to the password, depending on the saltOrder. If a salt was not used in the source system, then this should just be the the Base64 encoded value of the password's SHA-512/SHA-256/SHA-1/MD5 digest. For BCRYPT, This is the actual radix64-encoded hashed password.
         """
         return pulumi.get(self, "value")
 
     @value.setter
     def value(self, value: pulumi.Input[str]):
         pulumi.set(self, "value", value)
 
     @property
     @pulumi.getter
     def salt(self) -> Optional[pulumi.Input[str]]:
         """
-        Only required for salted hashes. For BCRYPT, this specifies the radix64-encoded salt used to generate
-        the hash, which must be 22 characters long. For other salted hashes, this specifies the base64-encoded salt used to generate the hash.
+        Only required for salted hashes
         """
         return pulumi.get(self, "salt")
 
     @salt.setter
     def salt(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "salt", value)
 
     @property
     @pulumi.getter(name="saltOrder")
     def salt_order(self) -> Optional[pulumi.Input[str]]:
         """
-        Specifies whether salt was pre- or postfixed to the password before hashing. Only required for salted algorithms.
+        Specifies whether salt was pre- or postfixed to the password before hashing
         """
         return pulumi.get(self, "salt_order")
 
     @salt_order.setter
     def salt_order(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "salt_order", value)
 
     @property
     @pulumi.getter(name="workFactor")
     def work_factor(self) -> Optional[pulumi.Input[int]]:
         """
-        Governs the strength of the hash and the time required to compute it. Only required for BCRYPT algorithm. Minimum value is 1, and maximum is 20.
+        Governs the strength of the hash and the time required to compute it. Only required for BCRYPT algorithm
         """
         return pulumi.get(self, "work_factor")
 
     @work_factor.setter
     def work_factor(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "work_factor", value)
```

### Comparing `pulumi_okta-4.9.0a1713462165/pulumi_okta/user/get_user.py` & `pulumi_okta-4.9.0a1713902092/pulumi_okta/user/get_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713462165/pulumi_okta/user/get_user_profile_mapping_source.py` & `pulumi_okta-4.9.0a1713902092/pulumi_okta/user/get_user_profile_mapping_source.py`

 * *Files 6% similar despite different names*

```diff
@@ -72,22 +72,20 @@
     """
     Use this data source to retrieve the base user Profile Mapping source or target from Okta.
 
     > **NOTE:** If using this resource with OAuth2 scopes, this resource requires `okta.profileMappings.read` scope.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_okta as okta
 
     example = okta.user.get_user_profile_mapping_source()
     ```
-    <!--End PulumiCodeChooser -->
     """
     __args__ = dict()
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('okta:user/getUserProfileMappingSource:getUserProfileMappingSource', __args__, opts=opts, typ=GetUserProfileMappingSourceResult).value
 
     return AwaitableGetUserProfileMappingSourceResult(
         id=pulumi.get(__ret__, 'id'),
@@ -100,17 +98,15 @@
     """
     Use this data source to retrieve the base user Profile Mapping source or target from Okta.
 
     > **NOTE:** If using this resource with OAuth2 scopes, this resource requires `okta.profileMappings.read` scope.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_okta as okta
 
     example = okta.user.get_user_profile_mapping_source()
     ```
-    <!--End PulumiCodeChooser -->
     """
     ...
```

### Comparing `pulumi_okta-4.9.0a1713462165/pulumi_okta/user/get_user_type.py` & `pulumi_okta-4.9.0a1713902092/pulumi_okta/user/get_user_type.py`

 * *Files 7% similar despite different names*

```diff
@@ -83,22 +83,20 @@
 def get_user_type(name: Optional[str] = None,
                   opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetUserTypeResult:
     """
     Use this data source to retrieve a user type from Okta.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_okta as okta
 
     example = okta.user.get_user_type(name="example")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str name: name of user type to retrieve.
     """
     __args__ = dict()
     __args__['name'] = name
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
@@ -115,20 +113,18 @@
 def get_user_type_output(name: Optional[pulumi.Input[str]] = None,
                          opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetUserTypeResult]:
     """
     Use this data source to retrieve a user type from Okta.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_okta as okta
 
     example = okta.user.get_user_type(name="example")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str name: name of user type to retrieve.
     """
     ...
```

### Comparing `pulumi_okta-4.9.0a1713462165/pulumi_okta/user/get_users.py` & `pulumi_okta-4.9.0a1713902092/pulumi_okta/user/get_users.py`

 * *Files 2% similar despite different names*

```diff
@@ -121,25 +121,23 @@
               opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetUsersResult:
     """
     Use this data source to retrieve a list of users from Okta.
 
     ## Example Usage
 
     ### Lookup Users by Group Membership
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_okta as okta
 
     example_group = okta.group.Group("example", name="example-group")
     example = okta.user.get_users_output(group_id=example_group.id,
         include_groups=True,
         include_roles=True)
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str compound_search_operator: Given multiple search elements they will be compounded together with the op. Default is `and`, `or` is also valid.
     :param str delay_read_seconds: Force delay of the users read by N seconds. Useful when eventual consistency of users information needs to be allowed for; for instance, when administrator roles are known to have been applied.
     :param str group_id: Id of group used to find users based on membership.
     :param bool include_groups: Fetch each user's group memberships. Defaults to `false`, in which case the `group_memberships` user attribute will be empty.
     :param bool include_roles: Fetch each user's administrator roles. Defaults to `false`, in which case the `admin_roles` user attribute will be empty.
@@ -176,25 +174,23 @@
                      opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetUsersResult]:
     """
     Use this data source to retrieve a list of users from Okta.
 
     ## Example Usage
 
     ### Lookup Users by Group Membership
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_okta as okta
 
     example_group = okta.group.Group("example", name="example-group")
     example = okta.user.get_users_output(group_id=example_group.id,
         include_groups=True,
         include_roles=True)
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str compound_search_operator: Given multiple search elements they will be compounded together with the op. Default is `and`, `or` is also valid.
     :param str delay_read_seconds: Force delay of the users read by N seconds. Useful when eventual consistency of users information needs to be allowed for; for instance, when administrator roles are known to have been applied.
     :param str group_id: Id of group used to find users based on membership.
     :param bool include_groups: Fetch each user's group memberships. Defaults to `false`, in which case the `group_memberships` user attribute will be empty.
     :param bool include_roles: Fetch each user's administrator roles. Defaults to `false`, in which case the `admin_roles` user attribute will be empty.
```

### Comparing `pulumi_okta-4.9.0a1713462165/pulumi_okta/user/outputs.py` & `pulumi_okta-4.9.0a1713902092/pulumi_okta/user/outputs.py`

 * *Files 4% similar despite different names*

```diff
@@ -41,22 +41,18 @@
                  algorithm: str,
                  value: str,
                  salt: Optional[str] = None,
                  salt_order: Optional[str] = None,
                  work_factor: Optional[int] = None):
         """
         :param str algorithm: The algorithm used to generate the hash using the password
-        :param str value: For SHA-512, SHA-256, SHA-1, MD5, this is the actual base64-encoded hash of the password (and salt, if used).
-               This is the Base64 encoded value of the SHA-512/SHA-256/SHA-1/MD5 digest that was computed by either pre-fixing or post-fixing
-               the salt to the password, depending on the saltOrder. If a salt was not used in the source system, then this should just be
-               the Base64 encoded value of the password's SHA-512/SHA-256/SHA-1/MD5 digest. For BCRYPT, This is the actual radix64-encoded hashed password.
-        :param str salt: Only required for salted hashes. For BCRYPT, this specifies the radix64-encoded salt used to generate
-               the hash, which must be 22 characters long. For other salted hashes, this specifies the base64-encoded salt used to generate the hash.
-        :param str salt_order: Specifies whether salt was pre- or postfixed to the password before hashing. Only required for salted algorithms.
-        :param int work_factor: Governs the strength of the hash and the time required to compute it. Only required for BCRYPT algorithm. Minimum value is 1, and maximum is 20.
+        :param str value: For SHA-512, SHA-256, SHA-1, MD5, This is the actual base64-encoded hash of the password (and salt, if used). This is the Base64 encoded value of the SHA-512/SHA-256/SHA-1/MD5 digest that was computed by either pre-fixing or post-fixing the salt to the password, depending on the saltOrder. If a salt was not used in the source system, then this should just be the the Base64 encoded value of the password's SHA-512/SHA-256/SHA-1/MD5 digest. For BCRYPT, This is the actual radix64-encoded hashed password.
+        :param str salt: Only required for salted hashes
+        :param str salt_order: Specifies whether salt was pre- or postfixed to the password before hashing
+        :param int work_factor: Governs the strength of the hash and the time required to compute it. Only required for BCRYPT algorithm
         """
         pulumi.set(__self__, "algorithm", algorithm)
         pulumi.set(__self__, "value", value)
         if salt is not None:
             pulumi.set(__self__, "salt", salt)
         if salt_order is not None:
             pulumi.set(__self__, "salt_order", salt_order)
@@ -71,43 +67,39 @@
         """
         return pulumi.get(self, "algorithm")
 
     @property
     @pulumi.getter
     def value(self) -> str:
         """
-        For SHA-512, SHA-256, SHA-1, MD5, this is the actual base64-encoded hash of the password (and salt, if used).
-        This is the Base64 encoded value of the SHA-512/SHA-256/SHA-1/MD5 digest that was computed by either pre-fixing or post-fixing
-        the salt to the password, depending on the saltOrder. If a salt was not used in the source system, then this should just be
-        the Base64 encoded value of the password's SHA-512/SHA-256/SHA-1/MD5 digest. For BCRYPT, This is the actual radix64-encoded hashed password.
+        For SHA-512, SHA-256, SHA-1, MD5, This is the actual base64-encoded hash of the password (and salt, if used). This is the Base64 encoded value of the SHA-512/SHA-256/SHA-1/MD5 digest that was computed by either pre-fixing or post-fixing the salt to the password, depending on the saltOrder. If a salt was not used in the source system, then this should just be the the Base64 encoded value of the password's SHA-512/SHA-256/SHA-1/MD5 digest. For BCRYPT, This is the actual radix64-encoded hashed password.
         """
         return pulumi.get(self, "value")
 
     @property
     @pulumi.getter
     def salt(self) -> Optional[str]:
         """
-        Only required for salted hashes. For BCRYPT, this specifies the radix64-encoded salt used to generate
-        the hash, which must be 22 characters long. For other salted hashes, this specifies the base64-encoded salt used to generate the hash.
+        Only required for salted hashes
         """
         return pulumi.get(self, "salt")
 
     @property
     @pulumi.getter(name="saltOrder")
     def salt_order(self) -> Optional[str]:
         """
-        Specifies whether salt was pre- or postfixed to the password before hashing. Only required for salted algorithms.
+        Specifies whether salt was pre- or postfixed to the password before hashing
         """
         return pulumi.get(self, "salt_order")
 
     @property
     @pulumi.getter(name="workFactor")
     def work_factor(self) -> Optional[int]:
         """
-        Governs the strength of the hash and the time required to compute it. Only required for BCRYPT algorithm. Minimum value is 1, and maximum is 20.
+        Governs the strength of the hash and the time required to compute it. Only required for BCRYPT algorithm
         """
         return pulumi.get(self, "work_factor")
 
 
 @pulumi.output_type
 class GetUserSearchResult(dict):
     def __init__(__self__, *,
```

### Comparing `pulumi_okta-4.9.0a1713462165/pulumi_okta/user/user.py` & `pulumi_okta-4.9.0a1713902092/pulumi_okta/user/user.py`

 * *Files 1% similar despite different names*

```diff
@@ -1490,15 +1490,14 @@
 
         This resource allows you to create and configure an Okta User.
 
         ## Example Usage
 
         Full profile:
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_okta as okta
 
         example = okta.user.User("example",
             first_name="John",
             last_name="Smith",
@@ -1528,31 +1527,28 @@
             state="NY",
             street_address="5678 Testing Ave.",
             timezone="America/New_York",
             title="Director",
             user_type="Employee",
             zip_code="11111")
         ```
-        <!--End PulumiCodeChooser -->
 
         With Password Inline Hook:
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_okta as okta
 
         test2 = okta.user.User("test2",
             first_name="John",
             last_name="Smith",
             login="example@example.com",
             email="example@example.com",
             password_inline_hook="default")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         An Okta User can be imported via the ID.
 
         ```sh
         $ pulumi import okta:user/user:User example &#60;user id&#62;
@@ -1624,15 +1620,14 @@
 
         This resource allows you to create and configure an Okta User.
 
         ## Example Usage
 
         Full profile:
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_okta as okta
 
         example = okta.user.User("example",
             first_name="John",
             last_name="Smith",
@@ -1662,31 +1657,28 @@
             state="NY",
             street_address="5678 Testing Ave.",
             timezone="America/New_York",
             title="Director",
             user_type="Employee",
             zip_code="11111")
         ```
-        <!--End PulumiCodeChooser -->
 
         With Password Inline Hook:
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_okta as okta
 
         test2 = okta.user.User("test2",
             first_name="John",
             last_name="Smith",
             login="example@example.com",
             email="example@example.com",
             password_inline_hook="default")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         An Okta User can be imported via the ID.
 
         ```sh
         $ pulumi import okta:user/user:User example &#60;user id&#62;
```

### Comparing `pulumi_okta-4.9.0a1713462165/pulumi_okta/user/user_type.py` & `pulumi_okta-4.9.0a1713902092/pulumi_okta/user/user_type.py`

 * *Files 2% similar despite different names*

```diff
@@ -133,25 +133,23 @@
         """
         Creates a User type.
 
         This resource allows you to create and configure a User Type.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_okta as okta
 
         example = okta.user.UserType("example",
             name="example",
             display_name="example",
             description="example")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         A User Type can be imported via the Okta ID.
 
         ```sh
         $ pulumi import okta:user/userType:UserType example &#60;user type id&#62;
@@ -172,25 +170,23 @@
         """
         Creates a User type.
 
         This resource allows you to create and configure a User Type.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_okta as okta
 
         example = okta.user.UserType("example",
             name="example",
             display_name="example",
             description="example")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         A User Type can be imported via the Okta ID.
 
         ```sh
         $ pulumi import okta:user/userType:UserType example &#60;user type id&#62;
```

### Comparing `pulumi_okta-4.9.0a1713462165/pulumi_okta/user_admin_roles.py` & `pulumi_okta-4.9.0a1713902092/pulumi_okta/user_admin_roles.py`

 * *Files 1% similar despite different names*

```diff
@@ -137,29 +137,27 @@
         """
         Resource to manage a set of admin roles for a specific user.
 
         This resource allows you to manage admin roles for a single user, independent of the user schema itself.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_okta as okta
 
         test = okta.user.User("test",
             first_name="TestAcc",
             last_name="Smith",
             login="testAcc-replace_with_uuid@example.com",
             email="testAcc-replace_with_uuid@example.com")
         test_user_admin_roles = okta.UserAdminRoles("test",
             user_id=test.id,
             admin_roles=["APP_ADMIN"])
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Existing user admin roles can be imported via the Okta User ID.
 
         ```sh
         $ pulumi import okta:index/userAdminRoles:UserAdminRoles example &#60;user id&#62;
@@ -181,29 +179,27 @@
         """
         Resource to manage a set of admin roles for a specific user.
 
         This resource allows you to manage admin roles for a single user, independent of the user schema itself.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_okta as okta
 
         test = okta.user.User("test",
             first_name="TestAcc",
             last_name="Smith",
             login="testAcc-replace_with_uuid@example.com",
             email="testAcc-replace_with_uuid@example.com")
         test_user_admin_roles = okta.UserAdminRoles("test",
             user_id=test.id,
             admin_roles=["APP_ADMIN"])
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Existing user admin roles can be imported via the Okta User ID.
 
         ```sh
         $ pulumi import okta:index/userAdminRoles:UserAdminRoles example &#60;user id&#62;
```

### Comparing `pulumi_okta-4.9.0a1713462165/pulumi_okta/user_base_schema_property.py` & `pulumi_okta-4.9.0a1713902092/pulumi_okta/user_base_schema_property.py`

 * *Files 1% similar despite different names*

```diff
@@ -305,28 +305,26 @@
         base properties can not be modified, except to update permissions, to change the nullability of `firstName` and
         `lastName` (`required` property) or to specify a `pattern` for `login`. Currently, `title` and `type` are required, so
         they should be set to the current values of the base property. This will be fixed in the future releases, as this is
         a breaking change.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_okta as okta
 
         example = okta.UserBaseSchemaProperty("example",
             index="firstName",
             title="First name",
             type="string",
             required=True,
             master="OKTA",
             user_type=example_okta_user_type["id"])
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         User schema property of default user type can be imported via the property index.
 
         ```sh
         $ pulumi import okta:index/userBaseSchemaProperty:UserBaseSchemaProperty example &#60;property name&#62;
@@ -366,28 +364,26 @@
         base properties can not be modified, except to update permissions, to change the nullability of `firstName` and
         `lastName` (`required` property) or to specify a `pattern` for `login`. Currently, `title` and `type` are required, so
         they should be set to the current values of the base property. This will be fixed in the future releases, as this is
         a breaking change.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_okta as okta
 
         example = okta.UserBaseSchemaProperty("example",
             index="firstName",
             title="First name",
             type="string",
             required=True,
             master="OKTA",
             user_type=example_okta_user_type["id"])
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         User schema property of default user type can be imported via the property index.
 
         ```sh
         $ pulumi import okta:index/userBaseSchemaProperty:UserBaseSchemaProperty example &#60;property name&#62;
```

### Comparing `pulumi_okta-4.9.0a1713462165/pulumi_okta/user_factor_question.py` & `pulumi_okta-4.9.0a1713902092/pulumi_okta/user_factor_question.py`

 * *Files 7% similar despite different names*

```diff
@@ -164,15 +164,14 @@
         """
         Creates security question factor for a user.
 
         This resource allows you to create and configure security question factor for a user.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_okta as okta
 
         example_user = okta.user.User("example",
             first_name="John",
             last_name="Smith",
@@ -184,15 +183,14 @@
             active=True)
         example_user_factor_question = okta.UserFactorQuestion("example",
             user_id=example_user.id,
             key=example.questions[0].key,
             answer="meatball",
             opts=pulumi.ResourceOptions(depends_on=[example_factor]))
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Security question factor for a user can be imported via the `user_id` and the `factor_id`.
 
         ```sh
         $ pulumi import okta:index/userFactorQuestion:UserFactorQuestion example &#60;user id&#62;/&#60;question factor id&#62;
@@ -213,15 +211,14 @@
         """
         Creates security question factor for a user.
 
         This resource allows you to create and configure security question factor for a user.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_okta as okta
 
         example_user = okta.user.User("example",
             first_name="John",
             last_name="Smith",
@@ -233,15 +230,14 @@
             active=True)
         example_user_factor_question = okta.UserFactorQuestion("example",
             user_id=example_user.id,
             key=example.questions[0].key,
             answer="meatball",
             opts=pulumi.ResourceOptions(depends_on=[example_factor]))
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Security question factor for a user can be imported via the `user_id` and the `factor_id`.
 
         ```sh
         $ pulumi import okta:index/userFactorQuestion:UserFactorQuestion example &#60;user id&#62;/&#60;question factor id&#62;
```

### Comparing `pulumi_okta-4.9.0a1713462165/pulumi_okta/user_group_memberships.py` & `pulumi_okta-4.9.0a1713902092/pulumi_okta/user_group_memberships.py`

 * *Files 2% similar despite different names*

```diff
@@ -96,15 +96,14 @@
                  opts: Optional[pulumi.ResourceOptions] = None,
                  groups: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  user_id: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_okta as okta
 
         test = okta.user.User("test",
             first_name="TestAcc",
             last_name="Smith",
@@ -113,15 +112,14 @@
         test_user_group_memberships = okta.UserGroupMemberships("test",
             user_id=test.id,
             groups=[
                 test1["id"],
                 test2["id"],
             ])
         ```
-        <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] groups: The list of Okta group IDs which the user should have membership managed for.
         :param pulumi.Input[str] user_id: Okta user ID.
         """
         ...
@@ -129,15 +127,14 @@
     def __init__(__self__,
                  resource_name: str,
                  args: UserGroupMembershipsArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_okta as okta
 
         test = okta.user.User("test",
             first_name="TestAcc",
             last_name="Smith",
@@ -146,15 +143,14 @@
         test_user_group_memberships = okta.UserGroupMemberships("test",
             user_id=test.id,
             groups=[
                 test1["id"],
                 test2["id"],
             ])
         ```
-        <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param UserGroupMembershipsArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
```

### Comparing `pulumi_okta-4.9.0a1713462165/pulumi_okta/user_schema_property.py` & `pulumi_okta-4.9.0a1713902092/pulumi_okta/user_schema_property.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,16 +36,16 @@
                  required: Optional[pulumi.Input[bool]] = None,
                  scope: Optional[pulumi.Input[str]] = None,
                  unique: Optional[pulumi.Input[str]] = None,
                  user_type: Optional[pulumi.Input[str]] = None):
         """
         The set of arguments for constructing a UserSchemaProperty resource.
         :param pulumi.Input[str] index: The property name.
-        :param pulumi.Input[str] title: display name for the enum value.
-        :param pulumi.Input[str] type: Type of profile source.
+        :param pulumi.Input[str] title: The display name.
+        :param pulumi.Input[str] type: The type of the schema property. It can be `"string"`, `"boolean"`, `"number"`, `"integer"`, `"array"`, or `"object"`.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] array_enums: Array of values that an array property's items can be set to.
         :param pulumi.Input[Sequence[pulumi.Input['UserSchemaPropertyArrayOneOfArgs']]] array_one_ofs: Display name and value an enum array can be set to.
         :param pulumi.Input[str] array_type: The type of the array elements if `type` is set to `"array"`.
         :param pulumi.Input[str] description: The description of the user schema property.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] enums: Array of values a primitive property can be set to. See `array_enum` for arrays.
         :param pulumi.Input[str] external_name: External name of the user schema property.
         :param pulumi.Input[str] external_namespace: External name of the user schema property.
@@ -113,27 +113,27 @@
     def index(self, value: pulumi.Input[str]):
         pulumi.set(self, "index", value)
 
     @property
     @pulumi.getter
     def title(self) -> pulumi.Input[str]:
         """
-        display name for the enum value.
+        The display name.
         """
         return pulumi.get(self, "title")
 
     @title.setter
     def title(self, value: pulumi.Input[str]):
         pulumi.set(self, "title", value)
 
     @property
     @pulumi.getter
     def type(self) -> pulumi.Input[str]:
         """
-        Type of profile source.
+        The type of the schema property. It can be `"string"`, `"boolean"`, `"number"`, `"integer"`, `"array"`, or `"object"`.
         """
         return pulumi.get(self, "type")
 
     @type.setter
     def type(self, value: pulumi.Input[str]):
         pulumi.set(self, "type", value)
 
@@ -393,16 +393,16 @@
         :param pulumi.Input[int] max_length: The maximum length of the user property value. Only applies to type `"string"`.
         :param pulumi.Input[int] min_length: The minimum length of the user property value. Only applies to type `"string"`.
         :param pulumi.Input[Sequence[pulumi.Input['UserSchemaPropertyOneOfArgs']]] one_ofs: Array of maps containing a mapping for display name to enum value.
         :param pulumi.Input[str] pattern: The validation pattern to use for the subschema. Must be in form of '.+', or '[<pattern>]+' if present.'
         :param pulumi.Input[str] permissions: Access control permissions for the property. It can be set to `"READ_WRITE"`, `"READ_ONLY"`, `"HIDE"`.
         :param pulumi.Input[bool] required: Whether the property is required for these users.
         :param pulumi.Input[str] scope: determines whether an app user attribute can be set at the Individual or Group Level.
-        :param pulumi.Input[str] title: display name for the enum value.
-        :param pulumi.Input[str] type: Type of profile source.
+        :param pulumi.Input[str] title: The display name.
+        :param pulumi.Input[str] type: The type of the schema property. It can be `"string"`, `"boolean"`, `"number"`, `"integer"`, `"array"`, or `"object"`.
         :param pulumi.Input[str] unique: Whether the property should be unique. It can be set to `"UNIQUE_VALIDATED"` or `"NOT_UNIQUE"`.
         :param pulumi.Input[str] user_type: User type ID
         """
         if array_enums is not None:
             pulumi.set(__self__, "array_enums", array_enums)
         if array_one_ofs is not None:
             pulumi.set(__self__, "array_one_ofs", array_one_ofs)
@@ -649,27 +649,27 @@
     def scope(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "scope", value)
 
     @property
     @pulumi.getter
     def title(self) -> Optional[pulumi.Input[str]]:
         """
-        display name for the enum value.
+        The display name.
         """
         return pulumi.get(self, "title")
 
     @title.setter
     def title(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "title", value)
 
     @property
     @pulumi.getter
     def type(self) -> Optional[pulumi.Input[str]]:
         """
-        Type of profile source.
+        The type of the schema property. It can be `"string"`, `"boolean"`, `"number"`, `"integer"`, `"array"`, or `"object"`.
         """
         return pulumi.get(self, "type")
 
     @type.setter
     def type(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "type", value)
 
@@ -724,29 +724,27 @@
                  type: Optional[pulumi.Input[str]] = None,
                  unique: Optional[pulumi.Input[str]] = None,
                  user_type: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_okta as okta
 
         example = okta.UserSchemaProperty("example",
             index="customPropertyName",
             title="customPropertyName",
             type="string",
             description="My custom property name",
             master="OKTA",
             scope="SELF",
             user_type=example_okta_user_type["id"])
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         User schema property of default user type can be imported via the property variableName.
 
         ```sh
         $ pulumi import okta:index/userSchemaProperty:UserSchemaProperty example &#60;variableName&#62;
@@ -773,43 +771,41 @@
         :param pulumi.Input[int] max_length: The maximum length of the user property value. Only applies to type `"string"`.
         :param pulumi.Input[int] min_length: The minimum length of the user property value. Only applies to type `"string"`.
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['UserSchemaPropertyOneOfArgs']]]] one_ofs: Array of maps containing a mapping for display name to enum value.
         :param pulumi.Input[str] pattern: The validation pattern to use for the subschema. Must be in form of '.+', or '[<pattern>]+' if present.'
         :param pulumi.Input[str] permissions: Access control permissions for the property. It can be set to `"READ_WRITE"`, `"READ_ONLY"`, `"HIDE"`.
         :param pulumi.Input[bool] required: Whether the property is required for these users.
         :param pulumi.Input[str] scope: determines whether an app user attribute can be set at the Individual or Group Level.
-        :param pulumi.Input[str] title: display name for the enum value.
-        :param pulumi.Input[str] type: Type of profile source.
+        :param pulumi.Input[str] title: The display name.
+        :param pulumi.Input[str] type: The type of the schema property. It can be `"string"`, `"boolean"`, `"number"`, `"integer"`, `"array"`, or `"object"`.
         :param pulumi.Input[str] unique: Whether the property should be unique. It can be set to `"UNIQUE_VALIDATED"` or `"NOT_UNIQUE"`.
         :param pulumi.Input[str] user_type: User type ID
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: UserSchemaPropertyArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_okta as okta
 
         example = okta.UserSchemaProperty("example",
             index="customPropertyName",
             title="customPropertyName",
             type="string",
             description="My custom property name",
             master="OKTA",
             scope="SELF",
             user_type=example_okta_user_type["id"])
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         User schema property of default user type can be imported via the property variableName.
 
         ```sh
         $ pulumi import okta:index/userSchemaProperty:UserSchemaProperty example &#60;variableName&#62;
@@ -944,16 +940,16 @@
         :param pulumi.Input[int] max_length: The maximum length of the user property value. Only applies to type `"string"`.
         :param pulumi.Input[int] min_length: The minimum length of the user property value. Only applies to type `"string"`.
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['UserSchemaPropertyOneOfArgs']]]] one_ofs: Array of maps containing a mapping for display name to enum value.
         :param pulumi.Input[str] pattern: The validation pattern to use for the subschema. Must be in form of '.+', or '[<pattern>]+' if present.'
         :param pulumi.Input[str] permissions: Access control permissions for the property. It can be set to `"READ_WRITE"`, `"READ_ONLY"`, `"HIDE"`.
         :param pulumi.Input[bool] required: Whether the property is required for these users.
         :param pulumi.Input[str] scope: determines whether an app user attribute can be set at the Individual or Group Level.
-        :param pulumi.Input[str] title: display name for the enum value.
-        :param pulumi.Input[str] type: Type of profile source.
+        :param pulumi.Input[str] title: The display name.
+        :param pulumi.Input[str] type: The type of the schema property. It can be `"string"`, `"boolean"`, `"number"`, `"integer"`, `"array"`, or `"object"`.
         :param pulumi.Input[str] unique: Whether the property should be unique. It can be set to `"UNIQUE_VALIDATED"` or `"NOT_UNIQUE"`.
         :param pulumi.Input[str] user_type: User type ID
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _UserSchemaPropertyState.__new__(_UserSchemaPropertyState)
 
@@ -1116,23 +1112,23 @@
         """
         return pulumi.get(self, "scope")
 
     @property
     @pulumi.getter
     def title(self) -> pulumi.Output[str]:
         """
-        display name for the enum value.
+        The display name.
         """
         return pulumi.get(self, "title")
 
     @property
     @pulumi.getter
     def type(self) -> pulumi.Output[str]:
         """
-        Type of profile source.
+        The type of the schema property. It can be `"string"`, `"boolean"`, `"number"`, `"integer"`, `"array"`, or `"object"`.
         """
         return pulumi.get(self, "type")
 
     @property
     @pulumi.getter
     def unique(self) -> pulumi.Output[Optional[str]]:
         """
```

### Comparing `pulumi_okta-4.9.0a1713462165/pulumi_okta.egg-info/PKG-INFO` & `pulumi_okta-4.9.0a1713902092/pulumi_okta.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_okta
-Version: 4.9.0a1713462165
+Version: 4.9.0a1713902092
 Summary: A Pulumi package for creating and managing okta resources.
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.io
 Project-URL: Repository, https://github.com/pulumi/pulumi-okta
 Keywords: pulumi,okta
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_okta-4.9.0a1713462165/pulumi_okta.egg-info/SOURCES.txt` & `pulumi_okta-4.9.0a1713902092/pulumi_okta.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1713462165/pyproject.toml` & `pulumi_okta-4.9.0a1713902092/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [project]
   name = "pulumi_okta"
   description = "A Pulumi package for creating and managing okta resources."
   dependencies = ["parver>=0.2.1", "pulumi>=3.0.0,<4.0.0", "semver>=2.8.1"]
   keywords = ["pulumi", "okta"]
   readme = "README.md"
   requires-python = ">=3.8"
-  version = "4.9.0a1713462165"
+  version = "4.9.0a1713902092"
   [project.license]
     text = "Apache-2.0"
   [project.urls]
     Homepage = "https://pulumi.io"
     Repository = "https://github.com/pulumi/pulumi-okta"
 
 [build-system]
```

