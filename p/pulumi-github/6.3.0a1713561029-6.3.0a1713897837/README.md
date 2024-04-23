# Comparing `tmp/pulumi_github-6.3.0a1713561029.tar.gz` & `tmp/pulumi_github-6.3.0a1713897837.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_github-6.3.0a1713561029.tar", last modified: Fri Apr 19 21:15:48 2024, max compression
+gzip compressed data, was "pulumi_github-6.3.0a1713897837.tar", last modified: Tue Apr 23 19:19:35 2024, max compression
```

## Comparing `pulumi_github-6.3.0a1713561029.tar` & `pulumi_github-6.3.0a1713897837.tar`

### file list

```diff
@@ -1,155 +1,155 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:15:48.705532 pulumi_github-6.3.0a1713561029/
--rw-r--r--   0 runner    (1001) docker     (127)     2842 2024-04-19 21:15:48.705532 pulumi_github-6.3.0a1713561029/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2390 2024-04-19 21:15:40.000000 pulumi_github-6.3.0a1713561029/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:15:48.701532 pulumi_github-6.3.0a1713561029/pulumi_github/
--rw-r--r--   0 runner    (1001) docker     (127)    19736 2024-04-19 21:15:40.000000 pulumi_github-6.3.0a1713561029/pulumi_github/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   171750 2024-04-19 21:15:40.000000 pulumi_github-6.3.0a1713561029/pulumi_github/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-04-19 21:15:40.000000 pulumi_github-6.3.0a1713561029/pulumi_github/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)    16264 2024-04-19 21:15:40.000000 pulumi_github-6.3.0a1713561029/pulumi_github/actions_environment_secret.py
--rw-r--r--   0 runner    (1001) docker     (127)    16331 2024-04-19 21:15:40.000000 pulumi_github-6.3.0a1713561029/pulumi_github/actions_environment_variable.py
--rw-r--r--   0 runner    (1001) docker     (127)     9307 2024-04-19 21:15:40.000000 pulumi_github-6.3.0a1713561029/pulumi_github/actions_organization_oidc_subject_claim_customization_template.py
--rw-r--r--   0 runner    (1001) docker     (127)    20945 2024-04-19 21:15:40.000000 pulumi_github-6.3.0a1713561029/pulumi_github/actions_organization_permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)    19290 2024-04-19 21:15:40.000000 pulumi_github-6.3.0a1713561029/pulumi_github/actions_organization_secret.py
--rw-r--r--   0 runner    (1001) docker     (127)    11058 2024-04-19 21:15:40.000000 pulumi_github-6.3.0a1713561029/pulumi_github/actions_organization_secret_repositories.py
--rw-r--r--   0 runner    (1001) docker     (127)    18054 2024-04-19 21:15:40.000000 pulumi_github-6.3.0a1713561029/pulumi_github/actions_organization_variable.py
--rw-r--r--   0 runner    (1001) docker     (127)    10221 2024-04-19 21:15:40.000000 pulumi_github-6.3.0a1713561029/pulumi_github/actions_repository_access_level.py
--rw-r--r--   0 runner    (1001) docker     (127)    15013 2024-04-19 21:15:40.000000 pulumi_github-6.3.0a1713561029/pulumi_github/actions_repository_oidc_subject_claim_customization_template.py
--rw-r--r--   0 runner    (1001) docker     (127)    16470 2024-04-19 21:15:40.000000 pulumi_github-6.3.0a1713561029/pulumi_github/actions_repository_permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)    27443 2024-04-19 21:15:40.000000 pulumi_github-6.3.0a1713561029/pulumi_github/actions_runner_group.py
--rw-r--r--   0 runner    (1001) docker     (127)    15026 2024-04-19 21:15:40.000000 pulumi_github-6.3.0a1713561029/pulumi_github/actions_secret.py
--rw-r--r--   0 runner    (1001) docker     (127)    12752 2024-04-19 21:15:40.000000 pulumi_github-6.3.0a1713561029/pulumi_github/actions_variable.py
--rw-r--r--   0 runner    (1001) docker     (127)    12985 2024-04-19 21:15:40.000000 pulumi_github-6.3.0a1713561029/pulumi_github/app_installation_repositories.py
--rw-r--r--   0 runner    (1001) docker     (127)    11381 2024-04-19 21:15:40.000000 pulumi_github-6.3.0a1713561029/pulumi_github/app_installation_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    17023 2024-04-19 21:15:40.000000 pulumi_github-6.3.0a1713561029/pulumi_github/branch.py
--rw-r--r--   0 runner    (1001) docker     (127)    13169 2024-04-19 21:15:40.000000 pulumi_github-6.3.0a1713561029/pulumi_github/branch_default.py
--rw-r--r--   0 runner    (1001) docker     (127)    46196 2024-04-19 21:15:40.000000 pulumi_github-6.3.0a1713561029/pulumi_github/branch_protection.py
--rw-r--r--   0 runner    (1001) docker     (127)    28640 2024-04-19 21:15:40.000000 pulumi_github-6.3.0a1713561029/pulumi_github/branch_protection_v3.py
--rw-r--r--   0 runner    (1001) docker     (127)    19390 2024-04-19 21:15:40.000000 pulumi_github-6.3.0a1713561029/pulumi_github/codespaces_organization_secret.py
--rw-r--r--   0 runner    (1001) docker     (127)    11150 2024-04-19 21:15:40.000000 pulumi_github-6.3.0a1713561029/pulumi_github/codespaces_organization_secret_repositories.py
--rw-r--r--   0 runner    (1001) docker     (127)    15154 2024-04-19 21:15:40.000000 pulumi_github-6.3.0a1713561029/pulumi_github/codespaces_secret.py
--rw-r--r--   0 runner    (1001) docker     (127)    16200 2024-04-19 21:15:40.000000 pulumi_github-6.3.0a1713561029/pulumi_github/codespaces_user_secret.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:15:48.701532 pulumi_github-6.3.0a1713561029/pulumi_github/config/
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-19 21:15:40.000000 pulumi_github-6.3.0a1713561029/pulumi_github/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2316 2024-04-19 21:15:40.000000 pulumi_github-6.3.0a1713561029/pulumi_github/config/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1465 2024-04-19 21:15:40.000000 pulumi_github-6.3.0a1713561029/pulumi_github/config/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     3787 2024-04-19 21:15:40.000000 pulumi_github-6.3.0a1713561029/pulumi_github/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (127)    19390 2024-04-19 21:15:40.000000 pulumi_github-6.3.0a1713561029/pulumi_github/dependabot_organization_secret.py
--rw-r--r--   0 runner    (1001) docker     (127)    11574 2024-04-19 21:15:40.000000 pulumi_github-6.3.0a1713561029/pulumi_github/dependabot_organization_secret_repositories.py
--rw-r--r--   0 runner    (1001) docker     (127)    15144 2024-04-19 21:15:40.000000 pulumi_github-6.3.0a1713561029/pulumi_github/dependabot_secret.py
--rw-r--r--   0 runner    (1001) docker     (127)    10188 2024-04-19 21:15:40.000000 pulumi_github-6.3.0a1713561029/pulumi_github/emu_group_mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)    23051 2024-04-19 21:15:40.000000 pulumi_github-6.3.0a1713561029/pulumi_github/enterprise_actions_permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)    29238 2024-04-19 21:15:40.000000 pulumi_github-6.3.0a1713561029/pulumi_github/enterprise_actions_runner_group.py
--rw-r--r--   0 runner    (1001) docker     (127)    18391 2024-04-19 21:15:40.000000 pulumi_github-6.3.0a1713561029/pulumi_github/enterprise_organization.py
--rw-r--r--   0 runner    (1001) docker     (127)     5266 2024-04-19 21:15:40.000000 pulumi_github-6.3.0a1713561029/pulumi_github/get_actions_environment_secrets.py
--rw-r--r--   0 runner    (1001) docker     (127)     5358 2024-04-19 21:15:40.000000 pulumi_github-6.3.0a1713561029/pulumi_github/get_actions_environment_variables.py
--rw-r--r--   0 runner    (1001) docker     (127)     4021 2024-04-19 21:15:40.000000 pulumi_github-6.3.0a1713561029/pulumi_github/get_actions_organization_oidc_subject_claim_customization_template.py
--rw-r--r--   0 runner    (1001) docker     (127)     4009 2024-04-19 21:15:40.000000 pulumi_github-6.3.0a1713561029/pulumi_github/get_actions_organization_public_key.py
--rw-r--r--   0 runner    (1001) docker     (127)     3964 2024-04-19 21:15:40.000000 pulumi_github-6.3.0a1713561029/pulumi_github/get_actions_organization_registration_token.py
--rw-r--r--   0 runner    (1001) docker     (127)     3232 2024-04-19 21:15:40.000000 pulumi_github-6.3.0a1713561029/pulumi_github/get_actions_organization_secrets.py
--rw-r--r--   0 runner    (1001) docker     (127)     3306 2024-04-19 21:15:40.000000 pulumi_github-6.3.0a1713561029/pulumi_github/get_actions_organization_variables.py
--rw-r--r--   0 runner    (1001) docker     (127)     4527 2024-04-19 21:15:40.000000 pulumi_github-6.3.0a1713561029/pulumi_github/get_actions_public_key.py
--rw-r--r--   0 runner    (1001) docker     (127)     4574 2024-04-19 21:15:40.000000 pulumi_github-6.3.0a1713561029/pulumi_github/get_actions_registration_token.py
--rw-r--r--   0 runner    (1001) docker     (127)     5364 2024-04-19 21:15:40.000000 pulumi_github-6.3.0a1713561029/pulumi_github/get_actions_repository_oidc_subject_claim_customization_template.py
--rw-r--r--   0 runner    (1001) docker     (127)     4413 2024-04-19 21:15:40.000000 pulumi_github-6.3.0a1713561029/pulumi_github/get_actions_secrets.py
--rw-r--r--   0 runner    (1001) docker     (127)     4504 2024-04-19 21:15:40.000000 pulumi_github-6.3.0a1713561029/pulumi_github/get_actions_variables.py
--rw-r--r--   0 runner    (1001) docker     (127)     5455 2024-04-19 21:15:40.000000 pulumi_github-6.3.0a1713561029/pulumi_github/get_app_token.py
--rw-r--r--   0 runner    (1001) docker     (127)     4972 2024-04-19 21:15:40.000000 pulumi_github-6.3.0a1713561029/pulumi_github/get_branch.py
--rw-r--r--   0 runner    (1001) docker     (127)     3928 2024-04-19 21:15:40.000000 pulumi_github-6.3.0a1713561029/pulumi_github/get_branch_protection_rules.py
--rw-r--r--   0 runner    (1001) docker     (127)     4083 2024-04-19 21:15:40.000000 pulumi_github-6.3.0a1713561029/pulumi_github/get_codespaces_organization_public_key.py
--rw-r--r--   0 runner    (1001) docker     (127)     3317 2024-04-19 21:15:40.000000 pulumi_github-6.3.0a1713561029/pulumi_github/get_codespaces_organization_secrets.py
--rw-r--r--   0 runner    (1001) docker     (127)     4607 2024-04-19 21:15:40.000000 pulumi_github-6.3.0a1713561029/pulumi_github/get_codespaces_public_key.py
--rw-r--r--   0 runner    (1001) docker     (127)     4705 2024-04-19 21:15:40.000000 pulumi_github-6.3.0a1713561029/pulumi_github/get_codespaces_secrets.py
--rw-r--r--   0 runner    (1001) docker     (127)     3891 2024-04-19 21:15:40.000000 pulumi_github-6.3.0a1713561029/pulumi_github/get_codespaces_user_public_key.py
--rw-r--r--   0 runner    (1001) docker     (127)     3133 2024-04-19 21:15:40.000000 pulumi_github-6.3.0a1713561029/pulumi_github/get_codespaces_user_secrets.py
--rw-r--r--   0 runner    (1001) docker     (127)     5451 2024-04-19 21:15:40.000000 pulumi_github-6.3.0a1713561029/pulumi_github/get_collaborators.py
--rw-r--r--   0 runner    (1001) docker     (127)     4083 2024-04-19 21:15:40.000000 pulumi_github-6.3.0a1713561029/pulumi_github/get_dependabot_organization_public_key.py
--rw-r--r--   0 runner    (1001) docker     (127)     3317 2024-04-19 21:15:40.000000 pulumi_github-6.3.0a1713561029/pulumi_github/get_dependabot_organization_secrets.py
--rw-r--r--   0 runner    (1001) docker     (127)     4607 2024-04-19 21:15:40.000000 pulumi_github-6.3.0a1713561029/pulumi_github/get_dependabot_public_key.py
--rw-r--r--   0 runner    (1001) docker     (127)     4521 2024-04-19 21:15:40.000000 pulumi_github-6.3.0a1713561029/pulumi_github/get_dependabot_secrets.py
--rw-r--r--   0 runner    (1001) docker     (127)     5387 2024-04-19 21:15:40.000000 pulumi_github-6.3.0a1713561029/pulumi_github/get_enterprise.py
--rw-r--r--   0 runner    (1001) docker     (127)     3387 2024-04-19 21:15:40.000000 pulumi_github-6.3.0a1713561029/pulumi_github/get_external_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     4286 2024-04-19 21:15:40.000000 pulumi_github-6.3.0a1713561029/pulumi_github/get_github_app.py
--rw-r--r--   0 runner    (1001) docker     (127)    17171 2024-04-19 21:15:40.000000 pulumi_github-6.3.0a1713561029/pulumi_github/get_ip_ranges.py
--rw-r--r--   0 runner    (1001) docker     (127)     3222 2024-04-19 21:15:40.000000 pulumi_github-6.3.0a1713561029/pulumi_github/get_issue_labels.py
--rw-r--r--   0 runner    (1001) docker     (127)     5787 2024-04-19 21:15:40.000000 pulumi_github-6.3.0a1713561029/pulumi_github/get_membership.py
--rw-r--r--   0 runner    (1001) docker     (127)    24830 2024-04-19 21:15:40.000000 pulumi_github-6.3.0a1713561029/pulumi_github/get_organization.py
--rw-r--r--   0 runner    (1001) docker     (127)     4994 2024-04-19 21:15:40.000000 pulumi_github-6.3.0a1713561029/pulumi_github/get_organization_custom_role.py
--rw-r--r--   0 runner    (1001) docker     (127)     3395 2024-04-19 21:15:40.000000 pulumi_github-6.3.0a1713561029/pulumi_github/get_organization_external_identities.py
--rw-r--r--   0 runner    (1001) docker     (127)     3637 2024-04-19 21:15:40.000000 pulumi_github-6.3.0a1713561029/pulumi_github/get_organization_ip_allow_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     3321 2024-04-19 21:15:40.000000 pulumi_github-6.3.0a1713561029/pulumi_github/get_organization_team_sync_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     7296 2024-04-19 21:15:40.000000 pulumi_github-6.3.0a1713561029/pulumi_github/get_organization_teams.py
--rw-r--r--   0 runner    (1001) docker     (127)     3265 2024-04-19 21:15:40.000000 pulumi_github-6.3.0a1713561029/pulumi_github/get_organization_webhooks.py
--rw-r--r--   0 runner    (1001) docker     (127)     5183 2024-04-19 21:15:40.000000 pulumi_github-6.3.0a1713561029/pulumi_github/get_ref.py
--rw-r--r--   0 runner    (1001) docker     (127)    14248 2024-04-19 21:15:40.000000 pulumi_github-6.3.0a1713561029/pulumi_github/get_release.py
--rw-r--r--   0 runner    (1001) docker     (127)     7850 2024-04-19 21:15:40.000000 pulumi_github-6.3.0a1713561029/pulumi_github/get_repositories.py
--rw-r--r--   0 runner    (1001) docker     (127)    22722 2024-04-19 21:15:40.000000 pulumi_github-6.3.0a1713561029/pulumi_github/get_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)     4403 2024-04-19 21:15:40.000000 pulumi_github-6.3.0a1713561029/pulumi_github/get_repository_autolink_references.py
--rw-r--r--   0 runner    (1001) docker     (127)     6336 2024-04-19 21:15:40.000000 pulumi_github-6.3.0a1713561029/pulumi_github/get_repository_branches.py
--rw-r--r--   0 runner    (1001) docker     (127)     3943 2024-04-19 21:15:40.000000 pulumi_github-6.3.0a1713561029/pulumi_github/get_repository_deploy_keys.py
--rw-r--r--   0 runner    (1001) docker     (127)     5760 2024-04-19 21:15:40.000000 pulumi_github-6.3.0a1713561029/pulumi_github/get_repository_deployment_branch_policies.py
--rw-r--r--   0 runner    (1001) docker     (127)     4133 2024-04-19 21:15:40.000000 pulumi_github-6.3.0a1713561029/pulumi_github/get_repository_environments.py
--rw-r--r--   0 runner    (1001) docker     (127)     8518 2024-04-19 21:15:40.000000 pulumi_github-6.3.0a1713561029/pulumi_github/get_repository_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     6579 2024-04-19 21:15:40.000000 pulumi_github-6.3.0a1713561029/pulumi_github/get_repository_milestone.py
--rw-r--r--   0 runner    (1001) docker     (127)    12391 2024-04-19 21:15:40.000000 pulumi_github-6.3.0a1713561029/pulumi_github/get_repository_pull_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    10070 2024-04-19 21:15:40.000000 pulumi_github-6.3.0a1713561029/pulumi_github/get_repository_pull_requests.py
--rw-r--r--   0 runner    (1001) docker     (127)     4455 2024-04-19 21:15:40.000000 pulumi_github-6.3.0a1713561029/pulumi_github/get_repository_teams.py
--rw-r--r--   0 runner    (1001) docker     (127)     3832 2024-04-19 21:15:40.000000 pulumi_github-6.3.0a1713561029/pulumi_github/get_repository_webhooks.py
--rw-r--r--   0 runner    (1001) docker     (127)     4814 2024-04-19 21:15:40.000000 pulumi_github-6.3.0a1713561029/pulumi_github/get_rest_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2728 2024-04-19 21:15:40.000000 pulumi_github-6.3.0a1713561029/pulumi_github/get_ssh_keys.py
--rw-r--r--   0 runner    (1001) docker     (127)     9850 2024-04-19 21:15:40.000000 pulumi_github-6.3.0a1713561029/pulumi_github/get_team.py
--rw-r--r--   0 runner    (1001) docker     (127)     5559 2024-04-19 21:15:40.000000 pulumi_github-6.3.0a1713561029/pulumi_github/get_tree.py
--rw-r--r--   0 runner    (1001) docker     (127)    12671 2024-04-19 21:15:40.000000 pulumi_github-6.3.0a1713561029/pulumi_github/get_user.py
--rw-r--r--   0 runner    (1001) docker     (127)     5172 2024-04-19 21:15:40.000000 pulumi_github-6.3.0a1713561029/pulumi_github/get_user_external_identity.py
--rw-r--r--   0 runner    (1001) docker     (127)     5499 2024-04-19 21:15:40.000000 pulumi_github-6.3.0a1713561029/pulumi_github/get_users.py
--rw-r--r--   0 runner    (1001) docker     (127)    21240 2024-04-19 21:15:40.000000 pulumi_github-6.3.0a1713561029/pulumi_github/issue.py
--rw-r--r--   0 runner    (1001) docker     (127)    13487 2024-04-19 21:15:40.000000 pulumi_github-6.3.0a1713561029/pulumi_github/issue_label.py
--rw-r--r--   0 runner    (1001) docker     (127)    10857 2024-04-19 21:15:40.000000 pulumi_github-6.3.0a1713561029/pulumi_github/issue_labels.py
--rw-r--r--   0 runner    (1001) docker     (127)    14110 2024-04-19 21:15:40.000000 pulumi_github-6.3.0a1713561029/pulumi_github/membership.py
--rw-r--r--   0 runner    (1001) docker     (127)     7250 2024-04-19 21:15:40.000000 pulumi_github-6.3.0a1713561029/pulumi_github/organization_block.py
--rw-r--r--   0 runner    (1001) docker     (127)    17937 2024-04-19 21:15:40.000000 pulumi_github-6.3.0a1713561029/pulumi_github/organization_custom_role.py
--rw-r--r--   0 runner    (1001) docker     (127)     9221 2024-04-19 21:15:40.000000 pulumi_github-6.3.0a1713561029/pulumi_github/organization_project.py
--rw-r--r--   0 runner    (1001) docker     (127)    25596 2024-04-19 21:15:40.000000 pulumi_github-6.3.0a1713561029/pulumi_github/organization_ruleset.py
--rw-r--r--   0 runner    (1001) docker     (127)     7116 2024-04-19 21:15:40.000000 pulumi_github-6.3.0a1713561029/pulumi_github/organization_security_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    80038 2024-04-19 21:15:40.000000 pulumi_github-6.3.0a1713561029/pulumi_github/organization_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)    14218 2024-04-19 21:15:40.000000 pulumi_github-6.3.0a1713561029/pulumi_github/organization_webhook.py
--rw-r--r--   0 runner    (1001) docker     (127)   222686 2024-04-19 21:15:40.000000 pulumi_github-6.3.0a1713561029/pulumi_github/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    17547 2024-04-19 21:15:40.000000 pulumi_github-6.3.0a1713561029/pulumi_github/project_card.py
--rw-r--r--   0 runner    (1001) docker     (127)    10008 2024-04-19 21:15:40.000000 pulumi_github-6.3.0a1713561029/pulumi_github/project_column.py
--rw-r--r--   0 runner    (1001) docker     (127)    21016 2024-04-19 21:15:40.000000 pulumi_github-6.3.0a1713561029/pulumi_github/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-19 21:15:40.000000 pulumi_github-6.3.0a1713561029/pulumi_github/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 21:15:40.000000 pulumi_github-6.3.0a1713561029/pulumi_github/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    29057 2024-04-19 21:15:40.000000 pulumi_github-6.3.0a1713561029/pulumi_github/release.py
--rw-r--r--   0 runner    (1001) docker     (127)   115438 2024-04-19 21:15:40.000000 pulumi_github-6.3.0a1713561029/pulumi_github/repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    16601 2024-04-19 21:15:40.000000 pulumi_github-6.3.0a1713561029/pulumi_github/repository_autolink_reference.py
--rw-r--r--   0 runner    (1001) docker     (127)    23106 2024-04-19 21:15:40.000000 pulumi_github-6.3.0a1713561029/pulumi_github/repository_collaborator.py
--rw-r--r--   0 runner    (1001) docker     (127)    17694 2024-04-19 21:15:40.000000 pulumi_github-6.3.0a1713561029/pulumi_github/repository_collaborators.py
--rw-r--r--   0 runner    (1001) docker     (127)     9790 2024-04-19 21:15:40.000000 pulumi_github-6.3.0a1713561029/pulumi_github/repository_dependabot_security_updates.py
--rw-r--r--   0 runner    (1001) docker     (127)    14988 2024-04-19 21:15:40.000000 pulumi_github-6.3.0a1713561029/pulumi_github/repository_deploy_key.py
--rw-r--r--   0 runner    (1001) docker     (127)    13651 2024-04-19 21:15:40.000000 pulumi_github-6.3.0a1713561029/pulumi_github/repository_deployment_branch_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)    23225 2024-04-19 21:15:40.000000 pulumi_github-6.3.0a1713561029/pulumi_github/repository_environment.py
--rw-r--r--   0 runner    (1001) docker     (127)    13412 2024-04-19 21:15:40.000000 pulumi_github-6.3.0a1713561029/pulumi_github/repository_environment_deployment_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)    28647 2024-04-19 21:15:40.000000 pulumi_github-6.3.0a1713561029/pulumi_github/repository_file.py
--rw-r--r--   0 runner    (1001) docker     (127)    17263 2024-04-19 21:15:40.000000 pulumi_github-6.3.0a1713561029/pulumi_github/repository_milestone.py
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-19 21:15:40.000000 pulumi_github-6.3.0a1713561029/pulumi_github/repository_project.py
--rw-r--r--   0 runner    (1001) docker     (127)    28838 2024-04-19 21:15:40.000000 pulumi_github-6.3.0a1713561029/pulumi_github/repository_pull_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    27106 2024-04-19 21:15:40.000000 pulumi_github-6.3.0a1713561029/pulumi_github/repository_ruleset.py
--rw-r--r--   0 runner    (1001) docker     (127)    10864 2024-04-19 21:15:40.000000 pulumi_github-6.3.0a1713561029/pulumi_github/repository_tag_protection.py
--rw-r--r--   0 runner    (1001) docker     (127)     8905 2024-04-19 21:15:40.000000 pulumi_github-6.3.0a1713561029/pulumi_github/repository_topics.py
--rw-r--r--   0 runner    (1001) docker     (127)    17426 2024-04-19 21:15:40.000000 pulumi_github-6.3.0a1713561029/pulumi_github/repository_webhook.py
--rw-r--r--   0 runner    (1001) docker     (127)    27101 2024-04-19 21:15:40.000000 pulumi_github-6.3.0a1713561029/pulumi_github/team.py
--rw-r--r--   0 runner    (1001) docker     (127)    13140 2024-04-19 21:15:40.000000 pulumi_github-6.3.0a1713561029/pulumi_github/team_members.py
--rw-r--r--   0 runner    (1001) docker     (127)    13689 2024-04-19 21:15:40.000000 pulumi_github-6.3.0a1713561029/pulumi_github/team_membership.py
--rw-r--r--   0 runner    (1001) docker     (127)    15777 2024-04-19 21:15:40.000000 pulumi_github-6.3.0a1713561029/pulumi_github/team_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    16849 2024-04-19 21:15:40.000000 pulumi_github-6.3.0a1713561029/pulumi_github/team_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)    12602 2024-04-19 21:15:40.000000 pulumi_github-6.3.0a1713561029/pulumi_github/team_sync_group_mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)     9917 2024-04-19 21:15:40.000000 pulumi_github-6.3.0a1713561029/pulumi_github/user_gpg_key.py
--rw-r--r--   0 runner    (1001) docker     (127)    11668 2024-04-19 21:15:40.000000 pulumi_github-6.3.0a1713561029/pulumi_github/user_invitation_accepter.py
--rw-r--r--   0 runner    (1001) docker     (127)    10052 2024-04-19 21:15:40.000000 pulumi_github-6.3.0a1713561029/pulumi_github/user_ssh_key.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:15:48.701532 pulumi_github-6.3.0a1713561029/pulumi_github.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2842 2024-04-19 21:15:48.000000 pulumi_github-6.3.0a1713561029/pulumi_github.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5957 2024-04-19 21:15:48.000000 pulumi_github-6.3.0a1713561029/pulumi_github.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 21:15:48.000000 pulumi_github-6.3.0a1713561029/pulumi_github.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-19 21:15:48.000000 pulumi_github-6.3.0a1713561029/pulumi_github.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-19 21:15:48.000000 pulumi_github-6.3.0a1713561029/pulumi_github.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      679 2024-04-19 21:15:40.000000 pulumi_github-6.3.0a1713561029/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 21:15:48.705532 pulumi_github-6.3.0a1713561029/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:19:35.743580 pulumi_github-6.3.0a1713897837/
+-rw-r--r--   0 runner    (1001) docker     (127)     2842 2024-04-23 19:19:35.743580 pulumi_github-6.3.0a1713897837/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2390 2024-04-23 19:19:29.000000 pulumi_github-6.3.0a1713897837/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:19:35.743580 pulumi_github-6.3.0a1713897837/pulumi_github/
+-rw-r--r--   0 runner    (1001) docker     (127)    19736 2024-04-23 19:19:29.000000 pulumi_github-6.3.0a1713897837/pulumi_github/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   169844 2024-04-23 19:19:29.000000 pulumi_github-6.3.0a1713897837/pulumi_github/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-04-23 19:19:29.000000 pulumi_github-6.3.0a1713897837/pulumi_github/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16264 2024-04-23 19:19:29.000000 pulumi_github-6.3.0a1713897837/pulumi_github/actions_environment_secret.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16019 2024-04-23 19:19:29.000000 pulumi_github-6.3.0a1713897837/pulumi_github/actions_environment_variable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9151 2024-04-23 19:19:29.000000 pulumi_github-6.3.0a1713897837/pulumi_github/actions_organization_oidc_subject_claim_customization_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20789 2024-04-23 19:19:29.000000 pulumi_github-6.3.0a1713897837/pulumi_github/actions_organization_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19290 2024-04-23 19:19:29.000000 pulumi_github-6.3.0a1713897837/pulumi_github/actions_organization_secret.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10902 2024-04-23 19:19:29.000000 pulumi_github-6.3.0a1713897837/pulumi_github/actions_organization_secret_repositories.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17742 2024-04-23 19:19:29.000000 pulumi_github-6.3.0a1713897837/pulumi_github/actions_organization_variable.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10065 2024-04-23 19:19:29.000000 pulumi_github-6.3.0a1713897837/pulumi_github/actions_repository_access_level.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14857 2024-04-23 19:19:29.000000 pulumi_github-6.3.0a1713897837/pulumi_github/actions_repository_oidc_subject_claim_customization_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16314 2024-04-23 19:19:29.000000 pulumi_github-6.3.0a1713897837/pulumi_github/actions_repository_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27287 2024-04-23 19:19:29.000000 pulumi_github-6.3.0a1713897837/pulumi_github/actions_runner_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15026 2024-04-23 19:19:29.000000 pulumi_github-6.3.0a1713897837/pulumi_github/actions_secret.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12596 2024-04-23 19:19:29.000000 pulumi_github-6.3.0a1713897837/pulumi_github/actions_variable.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12985 2024-04-23 19:19:29.000000 pulumi_github-6.3.0a1713897837/pulumi_github/app_installation_repositories.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11225 2024-04-23 19:19:29.000000 pulumi_github-6.3.0a1713897837/pulumi_github/app_installation_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16867 2024-04-23 19:19:29.000000 pulumi_github-6.3.0a1713897837/pulumi_github/branch.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12857 2024-04-23 19:19:29.000000 pulumi_github-6.3.0a1713897837/pulumi_github/branch_default.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46040 2024-04-23 19:19:29.000000 pulumi_github-6.3.0a1713897837/pulumi_github/branch_protection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28484 2024-04-23 19:19:29.000000 pulumi_github-6.3.0a1713897837/pulumi_github/branch_protection_v3.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19390 2024-04-23 19:19:29.000000 pulumi_github-6.3.0a1713897837/pulumi_github/codespaces_organization_secret.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10994 2024-04-23 19:19:29.000000 pulumi_github-6.3.0a1713897837/pulumi_github/codespaces_organization_secret_repositories.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15154 2024-04-23 19:19:29.000000 pulumi_github-6.3.0a1713897837/pulumi_github/codespaces_secret.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16200 2024-04-23 19:19:29.000000 pulumi_github-6.3.0a1713897837/pulumi_github/codespaces_user_secret.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:19:35.743580 pulumi_github-6.3.0a1713897837/pulumi_github/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-23 19:19:29.000000 pulumi_github-6.3.0a1713897837/pulumi_github/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2316 2024-04-23 19:19:29.000000 pulumi_github-6.3.0a1713897837/pulumi_github/config/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1465 2024-04-23 19:19:29.000000 pulumi_github-6.3.0a1713897837/pulumi_github/config/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3787 2024-04-23 19:19:29.000000 pulumi_github-6.3.0a1713897837/pulumi_github/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19390 2024-04-23 19:19:29.000000 pulumi_github-6.3.0a1713897837/pulumi_github/dependabot_organization_secret.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11418 2024-04-23 19:19:29.000000 pulumi_github-6.3.0a1713897837/pulumi_github/dependabot_organization_secret_repositories.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15144 2024-04-23 19:19:29.000000 pulumi_github-6.3.0a1713897837/pulumi_github/dependabot_secret.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10032 2024-04-23 19:19:29.000000 pulumi_github-6.3.0a1713897837/pulumi_github/emu_group_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22895 2024-04-23 19:19:29.000000 pulumi_github-6.3.0a1713897837/pulumi_github/enterprise_actions_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29082 2024-04-23 19:19:29.000000 pulumi_github-6.3.0a1713897837/pulumi_github/enterprise_actions_runner_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18235 2024-04-23 19:19:29.000000 pulumi_github-6.3.0a1713897837/pulumi_github/enterprise_organization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5126 2024-04-23 19:19:29.000000 pulumi_github-6.3.0a1713897837/pulumi_github/get_actions_environment_secrets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5218 2024-04-23 19:19:29.000000 pulumi_github-6.3.0a1713897837/pulumi_github/get_actions_environment_variables.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3881 2024-04-23 19:19:29.000000 pulumi_github-6.3.0a1713897837/pulumi_github/get_actions_organization_oidc_subject_claim_customization_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3869 2024-04-23 19:19:29.000000 pulumi_github-6.3.0a1713897837/pulumi_github/get_actions_organization_public_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3824 2024-04-23 19:19:29.000000 pulumi_github-6.3.0a1713897837/pulumi_github/get_actions_organization_registration_token.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3092 2024-04-23 19:19:29.000000 pulumi_github-6.3.0a1713897837/pulumi_github/get_actions_organization_secrets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3166 2024-04-23 19:19:29.000000 pulumi_github-6.3.0a1713897837/pulumi_github/get_actions_organization_variables.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4387 2024-04-23 19:19:29.000000 pulumi_github-6.3.0a1713897837/pulumi_github/get_actions_public_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4434 2024-04-23 19:19:29.000000 pulumi_github-6.3.0a1713897837/pulumi_github/get_actions_registration_token.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5224 2024-04-23 19:19:29.000000 pulumi_github-6.3.0a1713897837/pulumi_github/get_actions_repository_oidc_subject_claim_customization_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4273 2024-04-23 19:19:29.000000 pulumi_github-6.3.0a1713897837/pulumi_github/get_actions_secrets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4364 2024-04-23 19:19:29.000000 pulumi_github-6.3.0a1713897837/pulumi_github/get_actions_variables.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5315 2024-04-23 19:19:29.000000 pulumi_github-6.3.0a1713897837/pulumi_github/get_app_token.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4832 2024-04-23 19:19:29.000000 pulumi_github-6.3.0a1713897837/pulumi_github/get_branch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3788 2024-04-23 19:19:29.000000 pulumi_github-6.3.0a1713897837/pulumi_github/get_branch_protection_rules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3943 2024-04-23 19:19:29.000000 pulumi_github-6.3.0a1713897837/pulumi_github/get_codespaces_organization_public_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3177 2024-04-23 19:19:29.000000 pulumi_github-6.3.0a1713897837/pulumi_github/get_codespaces_organization_secrets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4467 2024-04-23 19:19:29.000000 pulumi_github-6.3.0a1713897837/pulumi_github/get_codespaces_public_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4565 2024-04-23 19:19:29.000000 pulumi_github-6.3.0a1713897837/pulumi_github/get_codespaces_secrets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3751 2024-04-23 19:19:29.000000 pulumi_github-6.3.0a1713897837/pulumi_github/get_codespaces_user_public_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2993 2024-04-23 19:19:29.000000 pulumi_github-6.3.0a1713897837/pulumi_github/get_codespaces_user_secrets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5311 2024-04-23 19:19:29.000000 pulumi_github-6.3.0a1713897837/pulumi_github/get_collaborators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3943 2024-04-23 19:19:29.000000 pulumi_github-6.3.0a1713897837/pulumi_github/get_dependabot_organization_public_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3177 2024-04-23 19:19:29.000000 pulumi_github-6.3.0a1713897837/pulumi_github/get_dependabot_organization_secrets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4467 2024-04-23 19:19:29.000000 pulumi_github-6.3.0a1713897837/pulumi_github/get_dependabot_public_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4381 2024-04-23 19:19:29.000000 pulumi_github-6.3.0a1713897837/pulumi_github/get_dependabot_secrets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5247 2024-04-23 19:19:29.000000 pulumi_github-6.3.0a1713897837/pulumi_github/get_enterprise.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3247 2024-04-23 19:19:29.000000 pulumi_github-6.3.0a1713897837/pulumi_github/get_external_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4146 2024-04-23 19:19:29.000000 pulumi_github-6.3.0a1713897837/pulumi_github/get_github_app.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17031 2024-04-23 19:19:29.000000 pulumi_github-6.3.0a1713897837/pulumi_github/get_ip_ranges.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3222 2024-04-23 19:19:29.000000 pulumi_github-6.3.0a1713897837/pulumi_github/get_issue_labels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5647 2024-04-23 19:19:29.000000 pulumi_github-6.3.0a1713897837/pulumi_github/get_membership.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24690 2024-04-23 19:19:29.000000 pulumi_github-6.3.0a1713897837/pulumi_github/get_organization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4854 2024-04-23 19:19:29.000000 pulumi_github-6.3.0a1713897837/pulumi_github/get_organization_custom_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3255 2024-04-23 19:19:29.000000 pulumi_github-6.3.0a1713897837/pulumi_github/get_organization_external_identities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3497 2024-04-23 19:19:29.000000 pulumi_github-6.3.0a1713897837/pulumi_github/get_organization_ip_allow_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3181 2024-04-23 19:19:29.000000 pulumi_github-6.3.0a1713897837/pulumi_github/get_organization_team_sync_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7016 2024-04-23 19:19:29.000000 pulumi_github-6.3.0a1713897837/pulumi_github/get_organization_teams.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3125 2024-04-23 19:19:29.000000 pulumi_github-6.3.0a1713897837/pulumi_github/get_organization_webhooks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5043 2024-04-23 19:19:29.000000 pulumi_github-6.3.0a1713897837/pulumi_github/get_ref.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14108 2024-04-23 19:19:29.000000 pulumi_github-6.3.0a1713897837/pulumi_github/get_release.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7710 2024-04-23 19:19:29.000000 pulumi_github-6.3.0a1713897837/pulumi_github/get_repositories.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22582 2024-04-23 19:19:29.000000 pulumi_github-6.3.0a1713897837/pulumi_github/get_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4263 2024-04-23 19:19:29.000000 pulumi_github-6.3.0a1713897837/pulumi_github/get_repository_autolink_references.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6196 2024-04-23 19:19:29.000000 pulumi_github-6.3.0a1713897837/pulumi_github/get_repository_branches.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3803 2024-04-23 19:19:29.000000 pulumi_github-6.3.0a1713897837/pulumi_github/get_repository_deploy_keys.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5620 2024-04-23 19:19:29.000000 pulumi_github-6.3.0a1713897837/pulumi_github/get_repository_deployment_branch_policies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3993 2024-04-23 19:19:29.000000 pulumi_github-6.3.0a1713897837/pulumi_github/get_repository_environments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8378 2024-04-23 19:19:29.000000 pulumi_github-6.3.0a1713897837/pulumi_github/get_repository_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6439 2024-04-23 19:19:29.000000 pulumi_github-6.3.0a1713897837/pulumi_github/get_repository_milestone.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12251 2024-04-23 19:19:29.000000 pulumi_github-6.3.0a1713897837/pulumi_github/get_repository_pull_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9930 2024-04-23 19:19:29.000000 pulumi_github-6.3.0a1713897837/pulumi_github/get_repository_pull_requests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4315 2024-04-23 19:19:29.000000 pulumi_github-6.3.0a1713897837/pulumi_github/get_repository_teams.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3692 2024-04-23 19:19:29.000000 pulumi_github-6.3.0a1713897837/pulumi_github/get_repository_webhooks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4674 2024-04-23 19:19:29.000000 pulumi_github-6.3.0a1713897837/pulumi_github/get_rest_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2588 2024-04-23 19:19:29.000000 pulumi_github-6.3.0a1713897837/pulumi_github/get_ssh_keys.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9710 2024-04-23 19:19:29.000000 pulumi_github-6.3.0a1713897837/pulumi_github/get_team.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5419 2024-04-23 19:19:29.000000 pulumi_github-6.3.0a1713897837/pulumi_github/get_tree.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12531 2024-04-23 19:19:29.000000 pulumi_github-6.3.0a1713897837/pulumi_github/get_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5032 2024-04-23 19:19:29.000000 pulumi_github-6.3.0a1713897837/pulumi_github/get_user_external_identity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5359 2024-04-23 19:19:29.000000 pulumi_github-6.3.0a1713897837/pulumi_github/get_users.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20928 2024-04-23 19:19:29.000000 pulumi_github-6.3.0a1713897837/pulumi_github/issue.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13331 2024-04-23 19:19:29.000000 pulumi_github-6.3.0a1713897837/pulumi_github/issue_label.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10701 2024-04-23 19:19:29.000000 pulumi_github-6.3.0a1713897837/pulumi_github/issue_labels.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13954 2024-04-23 19:19:29.000000 pulumi_github-6.3.0a1713897837/pulumi_github/membership.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7094 2024-04-23 19:19:29.000000 pulumi_github-6.3.0a1713897837/pulumi_github/organization_block.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17781 2024-04-23 19:19:29.000000 pulumi_github-6.3.0a1713897837/pulumi_github/organization_custom_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9065 2024-04-23 19:19:29.000000 pulumi_github-6.3.0a1713897837/pulumi_github/organization_project.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25440 2024-04-23 19:19:29.000000 pulumi_github-6.3.0a1713897837/pulumi_github/organization_ruleset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6960 2024-04-23 19:19:29.000000 pulumi_github-6.3.0a1713897837/pulumi_github/organization_security_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    79882 2024-04-23 19:19:29.000000 pulumi_github-6.3.0a1713897837/pulumi_github/organization_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14218 2024-04-23 19:19:29.000000 pulumi_github-6.3.0a1713897837/pulumi_github/organization_webhook.py
+-rw-r--r--   0 runner    (1001) docker     (127)   220780 2024-04-23 19:19:29.000000 pulumi_github-6.3.0a1713897837/pulumi_github/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17235 2024-04-23 19:19:29.000000 pulumi_github-6.3.0a1713897837/pulumi_github/project_card.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9852 2024-04-23 19:19:29.000000 pulumi_github-6.3.0a1713897837/pulumi_github/project_column.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21016 2024-04-23 19:19:29.000000 pulumi_github-6.3.0a1713897837/pulumi_github/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-23 19:19:29.000000 pulumi_github-6.3.0a1713897837/pulumi_github/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 19:19:29.000000 pulumi_github-6.3.0a1713897837/pulumi_github/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    28745 2024-04-23 19:19:29.000000 pulumi_github-6.3.0a1713897837/pulumi_github/release.py
+-rw-r--r--   0 runner    (1001) docker     (127)   115126 2024-04-23 19:19:29.000000 pulumi_github-6.3.0a1713897837/pulumi_github/repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16445 2024-04-23 19:19:29.000000 pulumi_github-6.3.0a1713897837/pulumi_github/repository_autolink_reference.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22950 2024-04-23 19:19:29.000000 pulumi_github-6.3.0a1713897837/pulumi_github/repository_collaborator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17538 2024-04-23 19:19:29.000000 pulumi_github-6.3.0a1713897837/pulumi_github/repository_collaborators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9634 2024-04-23 19:19:29.000000 pulumi_github-6.3.0a1713897837/pulumi_github/repository_dependabot_security_updates.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14832 2024-04-23 19:19:29.000000 pulumi_github-6.3.0a1713897837/pulumi_github/repository_deploy_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13495 2024-04-23 19:19:29.000000 pulumi_github-6.3.0a1713897837/pulumi_github/repository_deployment_branch_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23069 2024-04-23 19:19:29.000000 pulumi_github-6.3.0a1713897837/pulumi_github/repository_environment.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13256 2024-04-23 19:19:29.000000 pulumi_github-6.3.0a1713897837/pulumi_github/repository_environment_deployment_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28491 2024-04-23 19:19:29.000000 pulumi_github-6.3.0a1713897837/pulumi_github/repository_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17107 2024-04-23 19:19:29.000000 pulumi_github-6.3.0a1713897837/pulumi_github/repository_milestone.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11201 2024-04-23 19:19:29.000000 pulumi_github-6.3.0a1713897837/pulumi_github/repository_project.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28682 2024-04-23 19:19:29.000000 pulumi_github-6.3.0a1713897837/pulumi_github/repository_pull_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26950 2024-04-23 19:19:29.000000 pulumi_github-6.3.0a1713897837/pulumi_github/repository_ruleset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10708 2024-04-23 19:19:29.000000 pulumi_github-6.3.0a1713897837/pulumi_github/repository_tag_protection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8749 2024-04-23 19:19:29.000000 pulumi_github-6.3.0a1713897837/pulumi_github/repository_topics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17566 2024-04-23 19:19:29.000000 pulumi_github-6.3.0a1713897837/pulumi_github/repository_webhook.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26945 2024-04-23 19:19:29.000000 pulumi_github-6.3.0a1713897837/pulumi_github/team.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12984 2024-04-23 19:19:29.000000 pulumi_github-6.3.0a1713897837/pulumi_github/team_members.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13533 2024-04-23 19:19:29.000000 pulumi_github-6.3.0a1713897837/pulumi_github/team_membership.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15621 2024-04-23 19:19:29.000000 pulumi_github-6.3.0a1713897837/pulumi_github/team_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16693 2024-04-23 19:19:29.000000 pulumi_github-6.3.0a1713897837/pulumi_github/team_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12446 2024-04-23 19:19:29.000000 pulumi_github-6.3.0a1713897837/pulumi_github/team_sync_group_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9761 2024-04-23 19:19:29.000000 pulumi_github-6.3.0a1713897837/pulumi_github/user_gpg_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11512 2024-04-23 19:19:29.000000 pulumi_github-6.3.0a1713897837/pulumi_github/user_invitation_accepter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9896 2024-04-23 19:19:29.000000 pulumi_github-6.3.0a1713897837/pulumi_github/user_ssh_key.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:19:35.743580 pulumi_github-6.3.0a1713897837/pulumi_github.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2842 2024-04-23 19:19:35.000000 pulumi_github-6.3.0a1713897837/pulumi_github.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5957 2024-04-23 19:19:35.000000 pulumi_github-6.3.0a1713897837/pulumi_github.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 19:19:35.000000 pulumi_github-6.3.0a1713897837/pulumi_github.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-23 19:19:35.000000 pulumi_github-6.3.0a1713897837/pulumi_github.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-23 19:19:35.000000 pulumi_github-6.3.0a1713897837/pulumi_github.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      679 2024-04-23 19:19:29.000000 pulumi_github-6.3.0a1713897837/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 19:19:35.743580 pulumi_github-6.3.0a1713897837/setup.cfg
```

### Comparing `pulumi_github-6.3.0a1713561029/PKG-INFO` & `pulumi_github-6.3.0a1713897837/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_github
-Version: 6.3.0a1713561029
+Version: 6.3.0a1713897837
 Summary: A Pulumi package for creating and managing github cloud resources.
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.io
 Project-URL: Repository, https://github.com/pulumi/pulumi-github
 Keywords: pulumi,github
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_github-6.3.0a1713561029/README.md` & `pulumi_github-6.3.0a1713897837/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_github-6.3.0a1713561029/pulumi_github/__init__.py` & `pulumi_github-6.3.0a1713897837/pulumi_github/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-6.3.0a1713561029/pulumi_github/_inputs.py` & `pulumi_github-6.3.0a1713897837/pulumi_github/_inputs.py`

 * *Files 2% similar despite different names*

```diff
@@ -1030,37 +1030,37 @@
 
 @pulumi.input_type
 class OrganizationRulesetConditionsRefNameArgs:
     def __init__(__self__, *,
                  excludes: pulumi.Input[Sequence[pulumi.Input[str]]],
                  includes: pulumi.Input[Sequence[pulumi.Input[str]]]):
         """
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] excludes: (List of String) Array of repository names or patterns to exclude. The condition will not pass if any of these patterns match.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] includes: (List of String) Array of repository names or patterns to include. One of these patterns must match for the condition to pass. Also accepts `~ALL` to include all repositories.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] excludes: Array of ref names or patterns to exclude. The condition will not pass if any of these patterns match.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] includes: Array of ref names or patterns to include. One of these patterns must match for the condition to pass. Also accepts `~DEFAULT_BRANCH` to include the default branch or `~ALL` to include all branches.
         """
         pulumi.set(__self__, "excludes", excludes)
         pulumi.set(__self__, "includes", includes)
 
     @property
     @pulumi.getter
     def excludes(self) -> pulumi.Input[Sequence[pulumi.Input[str]]]:
         """
-        (List of String) Array of repository names or patterns to exclude. The condition will not pass if any of these patterns match.
+        Array of ref names or patterns to exclude. The condition will not pass if any of these patterns match.
         """
         return pulumi.get(self, "excludes")
 
     @excludes.setter
     def excludes(self, value: pulumi.Input[Sequence[pulumi.Input[str]]]):
         pulumi.set(self, "excludes", value)
 
     @property
     @pulumi.getter
     def includes(self) -> pulumi.Input[Sequence[pulumi.Input[str]]]:
         """
-        (List of String) Array of repository names or patterns to include. One of these patterns must match for the condition to pass. Also accepts `~ALL` to include all repositories.
+        Array of ref names or patterns to include. One of these patterns must match for the condition to pass. Also accepts `~DEFAULT_BRANCH` to include the default branch or `~ALL` to include all branches.
         """
         return pulumi.get(self, "includes")
 
     @includes.setter
     def includes(self, value: pulumi.Input[Sequence[pulumi.Input[str]]]):
         pulumi.set(self, "includes", value)
 
@@ -1068,40 +1068,40 @@
 @pulumi.input_type
 class OrganizationRulesetConditionsRepositoryNameArgs:
     def __init__(__self__, *,
                  excludes: pulumi.Input[Sequence[pulumi.Input[str]]],
                  includes: pulumi.Input[Sequence[pulumi.Input[str]]],
                  protected: Optional[pulumi.Input[bool]] = None):
         """
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] excludes: (List of String) Array of repository names or patterns to exclude. The condition will not pass if any of these patterns match.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] includes: (List of String) Array of repository names or patterns to include. One of these patterns must match for the condition to pass. Also accepts `~ALL` to include all repositories.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] excludes: Array of repository names or patterns to exclude. The condition will not pass if any of these patterns match.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] includes: Array of repository names or patterns to include. One of these patterns must match for the condition to pass. Also accepts `~ALL` to include all repositories.
         :param pulumi.Input[bool] protected: Whether renaming of target repositories is prevented.
         """
         pulumi.set(__self__, "excludes", excludes)
         pulumi.set(__self__, "includes", includes)
         if protected is not None:
             pulumi.set(__self__, "protected", protected)
 
     @property
     @pulumi.getter
     def excludes(self) -> pulumi.Input[Sequence[pulumi.Input[str]]]:
         """
-        (List of String) Array of repository names or patterns to exclude. The condition will not pass if any of these patterns match.
+        Array of repository names or patterns to exclude. The condition will not pass if any of these patterns match.
         """
         return pulumi.get(self, "excludes")
 
     @excludes.setter
     def excludes(self, value: pulumi.Input[Sequence[pulumi.Input[str]]]):
         pulumi.set(self, "excludes", value)
 
     @property
     @pulumi.getter
     def includes(self) -> pulumi.Input[Sequence[pulumi.Input[str]]]:
         """
-        (List of String) Array of repository names or patterns to include. One of these patterns must match for the condition to pass. Also accepts `~ALL` to include all repositories.
+        Array of repository names or patterns to include. One of these patterns must match for the condition to pass. Also accepts `~ALL` to include all repositories.
         """
         return pulumi.get(self, "includes")
 
     @includes.setter
     def includes(self, value: pulumi.Input[Sequence[pulumi.Input[str]]]):
         pulumi.set(self, "includes", value)
 
@@ -1353,43 +1353,43 @@
 class OrganizationRulesetRulesBranchNamePatternArgs:
     def __init__(__self__, *,
                  operator: pulumi.Input[str],
                  pattern: pulumi.Input[str],
                  name: Optional[pulumi.Input[str]] = None,
                  negate: Optional[pulumi.Input[bool]] = None):
         """
-        :param pulumi.Input[str] operator: (String) The operator to use for matching. Can be one of: `starts_with`, `ends_with`, `contains`, `regex`.
-        :param pulumi.Input[str] pattern: (String) The pattern to match with.
+        :param pulumi.Input[str] operator: The operator to use for matching. Can be one of: `starts_with`, `ends_with`, `contains`, `regex`.
+        :param pulumi.Input[str] pattern: The pattern to match with.
         :param pulumi.Input[str] name: (String) The name of the ruleset.
-        :param pulumi.Input[bool] negate: (Boolean) If true, the rule will fail if the pattern matches.
+        :param pulumi.Input[bool] negate: If true, the rule will fail if the pattern matches.
         """
         pulumi.set(__self__, "operator", operator)
         pulumi.set(__self__, "pattern", pattern)
         if name is not None:
             pulumi.set(__self__, "name", name)
         if negate is not None:
             pulumi.set(__self__, "negate", negate)
 
     @property
     @pulumi.getter
     def operator(self) -> pulumi.Input[str]:
         """
-        (String) The operator to use for matching. Can be one of: `starts_with`, `ends_with`, `contains`, `regex`.
+        The operator to use for matching. Can be one of: `starts_with`, `ends_with`, `contains`, `regex`.
         """
         return pulumi.get(self, "operator")
 
     @operator.setter
     def operator(self, value: pulumi.Input[str]):
         pulumi.set(self, "operator", value)
 
     @property
     @pulumi.getter
     def pattern(self) -> pulumi.Input[str]:
         """
-        (String) The pattern to match with.
+        The pattern to match with.
         """
         return pulumi.get(self, "pattern")
 
     @pattern.setter
     def pattern(self, value: pulumi.Input[str]):
         pulumi.set(self, "pattern", value)
 
@@ -1405,15 +1405,15 @@
     def name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "name", value)
 
     @property
     @pulumi.getter
     def negate(self) -> Optional[pulumi.Input[bool]]:
         """
-        (Boolean) If true, the rule will fail if the pattern matches.
+        If true, the rule will fail if the pattern matches.
         """
         return pulumi.get(self, "negate")
 
     @negate.setter
     def negate(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "negate", value)
 
@@ -1422,43 +1422,43 @@
 class OrganizationRulesetRulesCommitAuthorEmailPatternArgs:
     def __init__(__self__, *,
                  operator: pulumi.Input[str],
                  pattern: pulumi.Input[str],
                  name: Optional[pulumi.Input[str]] = None,
                  negate: Optional[pulumi.Input[bool]] = None):
         """
-        :param pulumi.Input[str] operator: (String) The operator to use for matching. Can be one of: `starts_with`, `ends_with`, `contains`, `regex`.
-        :param pulumi.Input[str] pattern: (String) The pattern to match with.
+        :param pulumi.Input[str] operator: The operator to use for matching. Can be one of: `starts_with`, `ends_with`, `contains`, `regex`.
+        :param pulumi.Input[str] pattern: The pattern to match with.
         :param pulumi.Input[str] name: (String) The name of the ruleset.
-        :param pulumi.Input[bool] negate: (Boolean) If true, the rule will fail if the pattern matches.
+        :param pulumi.Input[bool] negate: If true, the rule will fail if the pattern matches.
         """
         pulumi.set(__self__, "operator", operator)
         pulumi.set(__self__, "pattern", pattern)
         if name is not None:
             pulumi.set(__self__, "name", name)
         if negate is not None:
             pulumi.set(__self__, "negate", negate)
 
     @property
     @pulumi.getter
     def operator(self) -> pulumi.Input[str]:
         """
-        (String) The operator to use for matching. Can be one of: `starts_with`, `ends_with`, `contains`, `regex`.
+        The operator to use for matching. Can be one of: `starts_with`, `ends_with`, `contains`, `regex`.
         """
         return pulumi.get(self, "operator")
 
     @operator.setter
     def operator(self, value: pulumi.Input[str]):
         pulumi.set(self, "operator", value)
 
     @property
     @pulumi.getter
     def pattern(self) -> pulumi.Input[str]:
         """
-        (String) The pattern to match with.
+        The pattern to match with.
         """
         return pulumi.get(self, "pattern")
 
     @pattern.setter
     def pattern(self, value: pulumi.Input[str]):
         pulumi.set(self, "pattern", value)
 
@@ -1474,15 +1474,15 @@
     def name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "name", value)
 
     @property
     @pulumi.getter
     def negate(self) -> Optional[pulumi.Input[bool]]:
         """
-        (Boolean) If true, the rule will fail if the pattern matches.
+        If true, the rule will fail if the pattern matches.
         """
         return pulumi.get(self, "negate")
 
     @negate.setter
     def negate(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "negate", value)
 
@@ -1491,43 +1491,43 @@
 class OrganizationRulesetRulesCommitMessagePatternArgs:
     def __init__(__self__, *,
                  operator: pulumi.Input[str],
                  pattern: pulumi.Input[str],
                  name: Optional[pulumi.Input[str]] = None,
                  negate: Optional[pulumi.Input[bool]] = None):
         """
-        :param pulumi.Input[str] operator: (String) The operator to use for matching. Can be one of: `starts_with`, `ends_with`, `contains`, `regex`.
-        :param pulumi.Input[str] pattern: (String) The pattern to match with.
+        :param pulumi.Input[str] operator: The operator to use for matching. Can be one of: `starts_with`, `ends_with`, `contains`, `regex`.
+        :param pulumi.Input[str] pattern: The pattern to match with.
         :param pulumi.Input[str] name: (String) The name of the ruleset.
-        :param pulumi.Input[bool] negate: (Boolean) If true, the rule will fail if the pattern matches.
+        :param pulumi.Input[bool] negate: If true, the rule will fail if the pattern matches.
         """
         pulumi.set(__self__, "operator", operator)
         pulumi.set(__self__, "pattern", pattern)
         if name is not None:
             pulumi.set(__self__, "name", name)
         if negate is not None:
             pulumi.set(__self__, "negate", negate)
 
     @property
     @pulumi.getter
     def operator(self) -> pulumi.Input[str]:
         """
-        (String) The operator to use for matching. Can be one of: `starts_with`, `ends_with`, `contains`, `regex`.
+        The operator to use for matching. Can be one of: `starts_with`, `ends_with`, `contains`, `regex`.
         """
         return pulumi.get(self, "operator")
 
     @operator.setter
     def operator(self, value: pulumi.Input[str]):
         pulumi.set(self, "operator", value)
 
     @property
     @pulumi.getter
     def pattern(self) -> pulumi.Input[str]:
         """
-        (String) The pattern to match with.
+        The pattern to match with.
         """
         return pulumi.get(self, "pattern")
 
     @pattern.setter
     def pattern(self, value: pulumi.Input[str]):
         pulumi.set(self, "pattern", value)
 
@@ -1543,15 +1543,15 @@
     def name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "name", value)
 
     @property
     @pulumi.getter
     def negate(self) -> Optional[pulumi.Input[bool]]:
         """
-        (Boolean) If true, the rule will fail if the pattern matches.
+        If true, the rule will fail if the pattern matches.
         """
         return pulumi.get(self, "negate")
 
     @negate.setter
     def negate(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "negate", value)
 
@@ -1560,43 +1560,43 @@
 class OrganizationRulesetRulesCommitterEmailPatternArgs:
     def __init__(__self__, *,
                  operator: pulumi.Input[str],
                  pattern: pulumi.Input[str],
                  name: Optional[pulumi.Input[str]] = None,
                  negate: Optional[pulumi.Input[bool]] = None):
         """
-        :param pulumi.Input[str] operator: (String) The operator to use for matching. Can be one of: `starts_with`, `ends_with`, `contains`, `regex`.
-        :param pulumi.Input[str] pattern: (String) The pattern to match with.
+        :param pulumi.Input[str] operator: The operator to use for matching. Can be one of: `starts_with`, `ends_with`, `contains`, `regex`.
+        :param pulumi.Input[str] pattern: The pattern to match with.
         :param pulumi.Input[str] name: (String) The name of the ruleset.
-        :param pulumi.Input[bool] negate: (Boolean) If true, the rule will fail if the pattern matches.
+        :param pulumi.Input[bool] negate: If true, the rule will fail if the pattern matches.
         """
         pulumi.set(__self__, "operator", operator)
         pulumi.set(__self__, "pattern", pattern)
         if name is not None:
             pulumi.set(__self__, "name", name)
         if negate is not None:
             pulumi.set(__self__, "negate", negate)
 
     @property
     @pulumi.getter
     def operator(self) -> pulumi.Input[str]:
         """
-        (String) The operator to use for matching. Can be one of: `starts_with`, `ends_with`, `contains`, `regex`.
+        The operator to use for matching. Can be one of: `starts_with`, `ends_with`, `contains`, `regex`.
         """
         return pulumi.get(self, "operator")
 
     @operator.setter
     def operator(self, value: pulumi.Input[str]):
         pulumi.set(self, "operator", value)
 
     @property
     @pulumi.getter
     def pattern(self) -> pulumi.Input[str]:
         """
-        (String) The pattern to match with.
+        The pattern to match with.
         """
         return pulumi.get(self, "pattern")
 
     @pattern.setter
     def pattern(self, value: pulumi.Input[str]):
         pulumi.set(self, "pattern", value)
 
@@ -1612,15 +1612,15 @@
     def name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "name", value)
 
     @property
     @pulumi.getter
     def negate(self) -> Optional[pulumi.Input[bool]]:
         """
-        (Boolean) If true, the rule will fail if the pattern matches.
+        If true, the rule will fail if the pattern matches.
         """
         return pulumi.get(self, "negate")
 
     @negate.setter
     def negate(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "negate", value)
 
@@ -1630,19 +1630,19 @@
     def __init__(__self__, *,
                  dismiss_stale_reviews_on_push: Optional[pulumi.Input[bool]] = None,
                  require_code_owner_review: Optional[pulumi.Input[bool]] = None,
                  require_last_push_approval: Optional[pulumi.Input[bool]] = None,
                  required_approving_review_count: Optional[pulumi.Input[int]] = None,
                  required_review_thread_resolution: Optional[pulumi.Input[bool]] = None):
         """
-        :param pulumi.Input[bool] dismiss_stale_reviews_on_push: (Boolean) New, reviewable commits pushed will dismiss previous pull request review approvals. Defaults to `false`.
-        :param pulumi.Input[bool] require_code_owner_review: (Boolean) Require an approving review in pull requests that modify files that have a designated code owner. Defaults to `false`.
-        :param pulumi.Input[bool] require_last_push_approval: (Boolean) Whether the most recent reviewable push must be approved by someone other than the person who pushed it. Defaults to `false`.
-        :param pulumi.Input[int] required_approving_review_count: (Number) The number of approving reviews that are required before a pull request can be merged. Defaults to `0`.
-        :param pulumi.Input[bool] required_review_thread_resolution: (Boolean) All conversations on code must be resolved before a pull request can be merged. Defaults to `false`.
+        :param pulumi.Input[bool] dismiss_stale_reviews_on_push: New, reviewable commits pushed will dismiss previous pull request review approvals. Defaults to `false`.
+        :param pulumi.Input[bool] require_code_owner_review: Require an approving review in pull requests that modify files that have a designated code owner. Defaults to `false`.
+        :param pulumi.Input[bool] require_last_push_approval: Whether the most recent reviewable push must be approved by someone other than the person who pushed it. Defaults to `false`.
+        :param pulumi.Input[int] required_approving_review_count: The number of approving reviews that are required before a pull request can be merged. Defaults to `0`.
+        :param pulumi.Input[bool] required_review_thread_resolution: All conversations on code must be resolved before a pull request can be merged. Defaults to `false`.
         """
         if dismiss_stale_reviews_on_push is not None:
             pulumi.set(__self__, "dismiss_stale_reviews_on_push", dismiss_stale_reviews_on_push)
         if require_code_owner_review is not None:
             pulumi.set(__self__, "require_code_owner_review", require_code_owner_review)
         if require_last_push_approval is not None:
             pulumi.set(__self__, "require_last_push_approval", require_last_push_approval)
@@ -1651,161 +1651,161 @@
         if required_review_thread_resolution is not None:
             pulumi.set(__self__, "required_review_thread_resolution", required_review_thread_resolution)
 
     @property
     @pulumi.getter(name="dismissStaleReviewsOnPush")
     def dismiss_stale_reviews_on_push(self) -> Optional[pulumi.Input[bool]]:
         """
-        (Boolean) New, reviewable commits pushed will dismiss previous pull request review approvals. Defaults to `false`.
+        New, reviewable commits pushed will dismiss previous pull request review approvals. Defaults to `false`.
         """
         return pulumi.get(self, "dismiss_stale_reviews_on_push")
 
     @dismiss_stale_reviews_on_push.setter
     def dismiss_stale_reviews_on_push(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "dismiss_stale_reviews_on_push", value)
 
     @property
     @pulumi.getter(name="requireCodeOwnerReview")
     def require_code_owner_review(self) -> Optional[pulumi.Input[bool]]:
         """
-        (Boolean) Require an approving review in pull requests that modify files that have a designated code owner. Defaults to `false`.
+        Require an approving review in pull requests that modify files that have a designated code owner. Defaults to `false`.
         """
         return pulumi.get(self, "require_code_owner_review")
 
     @require_code_owner_review.setter
     def require_code_owner_review(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "require_code_owner_review", value)
 
     @property
     @pulumi.getter(name="requireLastPushApproval")
     def require_last_push_approval(self) -> Optional[pulumi.Input[bool]]:
         """
-        (Boolean) Whether the most recent reviewable push must be approved by someone other than the person who pushed it. Defaults to `false`.
+        Whether the most recent reviewable push must be approved by someone other than the person who pushed it. Defaults to `false`.
         """
         return pulumi.get(self, "require_last_push_approval")
 
     @require_last_push_approval.setter
     def require_last_push_approval(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "require_last_push_approval", value)
 
     @property
     @pulumi.getter(name="requiredApprovingReviewCount")
     def required_approving_review_count(self) -> Optional[pulumi.Input[int]]:
         """
-        (Number) The number of approving reviews that are required before a pull request can be merged. Defaults to `0`.
+        The number of approving reviews that are required before a pull request can be merged. Defaults to `0`.
         """
         return pulumi.get(self, "required_approving_review_count")
 
     @required_approving_review_count.setter
     def required_approving_review_count(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "required_approving_review_count", value)
 
     @property
     @pulumi.getter(name="requiredReviewThreadResolution")
     def required_review_thread_resolution(self) -> Optional[pulumi.Input[bool]]:
         """
-        (Boolean) All conversations on code must be resolved before a pull request can be merged. Defaults to `false`.
+        All conversations on code must be resolved before a pull request can be merged. Defaults to `false`.
         """
         return pulumi.get(self, "required_review_thread_resolution")
 
     @required_review_thread_resolution.setter
     def required_review_thread_resolution(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "required_review_thread_resolution", value)
 
 
 @pulumi.input_type
 class OrganizationRulesetRulesRequiredStatusChecksArgs:
     def __init__(__self__, *,
                  required_checks: pulumi.Input[Sequence[pulumi.Input['OrganizationRulesetRulesRequiredStatusChecksRequiredCheckArgs']]],
                  strict_required_status_checks_policy: Optional[pulumi.Input[bool]] = None):
         """
-        :param pulumi.Input[Sequence[pulumi.Input['OrganizationRulesetRulesRequiredStatusChecksRequiredCheckArgs']]] required_checks: (Block Set, Min: 1) Status checks that are required. Several can be defined. (see below for nested schema)
-        :param pulumi.Input[bool] strict_required_status_checks_policy: (Boolean) Whether pull requests targeting a matching branch must be tested with the latest code. This setting will not take effect unless at least one status check is enabled. Defaults to `false`.
+        :param pulumi.Input[Sequence[pulumi.Input['OrganizationRulesetRulesRequiredStatusChecksRequiredCheckArgs']]] required_checks: Status checks that are required. Several can be defined.
+        :param pulumi.Input[bool] strict_required_status_checks_policy: Whether pull requests targeting a matching branch must be tested with the latest code. This setting will not take effect unless at least one status check is enabled. Defaults to `false`.
         """
         pulumi.set(__self__, "required_checks", required_checks)
         if strict_required_status_checks_policy is not None:
             pulumi.set(__self__, "strict_required_status_checks_policy", strict_required_status_checks_policy)
 
     @property
     @pulumi.getter(name="requiredChecks")
     def required_checks(self) -> pulumi.Input[Sequence[pulumi.Input['OrganizationRulesetRulesRequiredStatusChecksRequiredCheckArgs']]]:
         """
-        (Block Set, Min: 1) Status checks that are required. Several can be defined. (see below for nested schema)
+        Status checks that are required. Several can be defined.
         """
         return pulumi.get(self, "required_checks")
 
     @required_checks.setter
     def required_checks(self, value: pulumi.Input[Sequence[pulumi.Input['OrganizationRulesetRulesRequiredStatusChecksRequiredCheckArgs']]]):
         pulumi.set(self, "required_checks", value)
 
     @property
     @pulumi.getter(name="strictRequiredStatusChecksPolicy")
     def strict_required_status_checks_policy(self) -> Optional[pulumi.Input[bool]]:
         """
-        (Boolean) Whether pull requests targeting a matching branch must be tested with the latest code. This setting will not take effect unless at least one status check is enabled. Defaults to `false`.
+        Whether pull requests targeting a matching branch must be tested with the latest code. This setting will not take effect unless at least one status check is enabled. Defaults to `false`.
         """
         return pulumi.get(self, "strict_required_status_checks_policy")
 
     @strict_required_status_checks_policy.setter
     def strict_required_status_checks_policy(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "strict_required_status_checks_policy", value)
 
 
 @pulumi.input_type
 class OrganizationRulesetRulesRequiredStatusChecksRequiredCheckArgs:
     def __init__(__self__, *,
                  context: pulumi.Input[str],
                  integration_id: Optional[pulumi.Input[int]] = None):
         """
-        :param pulumi.Input[str] context: (String) The status check context name that must be present on the commit.
-        :param pulumi.Input[int] integration_id: (Number) The optional integration ID that this status check must originate from.
+        :param pulumi.Input[str] context: The status check context name that must be present on the commit.
+        :param pulumi.Input[int] integration_id: The optional integration ID that this status check must originate from.
         """
         pulumi.set(__self__, "context", context)
         if integration_id is not None:
             pulumi.set(__self__, "integration_id", integration_id)
 
     @property
     @pulumi.getter
     def context(self) -> pulumi.Input[str]:
         """
-        (String) The status check context name that must be present on the commit.
+        The status check context name that must be present on the commit.
         """
         return pulumi.get(self, "context")
 
     @context.setter
     def context(self, value: pulumi.Input[str]):
         pulumi.set(self, "context", value)
 
     @property
     @pulumi.getter(name="integrationId")
     def integration_id(self) -> Optional[pulumi.Input[int]]:
         """
-        (Number) The optional integration ID that this status check must originate from.
+        The optional integration ID that this status check must originate from.
         """
         return pulumi.get(self, "integration_id")
 
     @integration_id.setter
     def integration_id(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "integration_id", value)
 
 
 @pulumi.input_type
 class OrganizationRulesetRulesRequiredWorkflowsArgs:
     def __init__(__self__, *,
                  required_workflows: pulumi.Input[Sequence[pulumi.Input['OrganizationRulesetRulesRequiredWorkflowsRequiredWorkflowArgs']]]):
         """
-        :param pulumi.Input[Sequence[pulumi.Input['OrganizationRulesetRulesRequiredWorkflowsRequiredWorkflowArgs']]] required_workflows: (Block Set, Min: 1) Actions workflows that are required. Multiple can be defined. (see below for nested schema)
+        :param pulumi.Input[Sequence[pulumi.Input['OrganizationRulesetRulesRequiredWorkflowsRequiredWorkflowArgs']]] required_workflows: Actions workflows that are required. Several can be defined.
         """
         pulumi.set(__self__, "required_workflows", required_workflows)
 
     @property
     @pulumi.getter(name="requiredWorkflows")
     def required_workflows(self) -> pulumi.Input[Sequence[pulumi.Input['OrganizationRulesetRulesRequiredWorkflowsRequiredWorkflowArgs']]]:
         """
-        (Block Set, Min: 1) Actions workflows that are required. Multiple can be defined. (see below for nested schema)
+        Actions workflows that are required. Several can be defined.
         """
         return pulumi.get(self, "required_workflows")
 
     @required_workflows.setter
     def required_workflows(self, value: pulumi.Input[Sequence[pulumi.Input['OrganizationRulesetRulesRequiredWorkflowsRequiredWorkflowArgs']]]):
         pulumi.set(self, "required_workflows", value)
 
@@ -1813,52 +1813,52 @@
 @pulumi.input_type
 class OrganizationRulesetRulesRequiredWorkflowsRequiredWorkflowArgs:
     def __init__(__self__, *,
                  path: pulumi.Input[str],
                  repository_id: pulumi.Input[int],
                  ref: Optional[pulumi.Input[str]] = None):
         """
-        :param pulumi.Input[str] path: (String) The path to the YAML definition file of the workflow.
-        :param pulumi.Input[int] repository_id: The repository IDs that the ruleset applies to. One of these IDs must match for the condition to pass. Conflicts with `repository_name`.
-        :param pulumi.Input[str] ref: (String) The optional ref from which to fetch the workflow. Defaults to `master`.
+        :param pulumi.Input[str] path: The path to the workflow YAML definition file.
+        :param pulumi.Input[int] repository_id: The repository in which the workflow is defined.
+        :param pulumi.Input[str] ref: The ref (branch or tag) of the workflow file to use.
         """
         pulumi.set(__self__, "path", path)
         pulumi.set(__self__, "repository_id", repository_id)
         if ref is not None:
             pulumi.set(__self__, "ref", ref)
 
     @property
     @pulumi.getter
     def path(self) -> pulumi.Input[str]:
         """
-        (String) The path to the YAML definition file of the workflow.
+        The path to the workflow YAML definition file.
         """
         return pulumi.get(self, "path")
 
     @path.setter
     def path(self, value: pulumi.Input[str]):
         pulumi.set(self, "path", value)
 
     @property
     @pulumi.getter(name="repositoryId")
     def repository_id(self) -> pulumi.Input[int]:
         """
-        The repository IDs that the ruleset applies to. One of these IDs must match for the condition to pass. Conflicts with `repository_name`.
+        The repository in which the workflow is defined.
         """
         return pulumi.get(self, "repository_id")
 
     @repository_id.setter
     def repository_id(self, value: pulumi.Input[int]):
         pulumi.set(self, "repository_id", value)
 
     @property
     @pulumi.getter
     def ref(self) -> Optional[pulumi.Input[str]]:
         """
-        (String) The optional ref from which to fetch the workflow. Defaults to `master`.
+        The ref (branch or tag) of the workflow file to use.
         """
         return pulumi.get(self, "ref")
 
     @ref.setter
     def ref(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "ref", value)
 
@@ -1867,43 +1867,43 @@
 class OrganizationRulesetRulesTagNamePatternArgs:
     def __init__(__self__, *,
                  operator: pulumi.Input[str],
                  pattern: pulumi.Input[str],
                  name: Optional[pulumi.Input[str]] = None,
                  negate: Optional[pulumi.Input[bool]] = None):
         """
-        :param pulumi.Input[str] operator: (String) The operator to use for matching. Can be one of: `starts_with`, `ends_with`, `contains`, `regex`.
-        :param pulumi.Input[str] pattern: (String) The pattern to match with.
+        :param pulumi.Input[str] operator: The operator to use for matching. Can be one of: `starts_with`, `ends_with`, `contains`, `regex`.
+        :param pulumi.Input[str] pattern: The pattern to match with.
         :param pulumi.Input[str] name: (String) The name of the ruleset.
-        :param pulumi.Input[bool] negate: (Boolean) If true, the rule will fail if the pattern matches.
+        :param pulumi.Input[bool] negate: If true, the rule will fail if the pattern matches.
         """
         pulumi.set(__self__, "operator", operator)
         pulumi.set(__self__, "pattern", pattern)
         if name is not None:
             pulumi.set(__self__, "name", name)
         if negate is not None:
             pulumi.set(__self__, "negate", negate)
 
     @property
     @pulumi.getter
     def operator(self) -> pulumi.Input[str]:
         """
-        (String) The operator to use for matching. Can be one of: `starts_with`, `ends_with`, `contains`, `regex`.
+        The operator to use for matching. Can be one of: `starts_with`, `ends_with`, `contains`, `regex`.
         """
         return pulumi.get(self, "operator")
 
     @operator.setter
     def operator(self, value: pulumi.Input[str]):
         pulumi.set(self, "operator", value)
 
     @property
     @pulumi.getter
     def pattern(self) -> pulumi.Input[str]:
         """
-        (String) The pattern to match with.
+        The pattern to match with.
         """
         return pulumi.get(self, "pattern")
 
     @pattern.setter
     def pattern(self, value: pulumi.Input[str]):
         pulumi.set(self, "pattern", value)
 
@@ -1919,15 +1919,15 @@
     def name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "name", value)
 
     @property
     @pulumi.getter
     def negate(self) -> Optional[pulumi.Input[bool]]:
         """
-        (Boolean) If true, the rule will fail if the pattern matches.
+        If true, the rule will fail if the pattern matches.
         """
         return pulumi.get(self, "negate")
 
     @negate.setter
     def negate(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "negate", value)
 
@@ -2226,15 +2226,15 @@
                  url: Optional[pulumi.Input[str]] = None):
         """
         :param pulumi.Input[str] build_type: The type of GitHub Pages site to build. Can be `legacy` or `workflow`. If you use `legacy` as build type you need to set the option `source`.
         :param pulumi.Input[str] cname: The custom domain for the repository. This can only be set after the repository has been created.
         :param pulumi.Input[bool] custom404: Whether the rendered GitHub Pages site has a custom 404 page.
         :param pulumi.Input[str] html_url: The absolute URL (including scheme) of the rendered GitHub Pages site e.g. `https://username.github.io`.
         :param pulumi.Input['RepositoryPagesSourceArgs'] source: The source branch and directory for the rendered Pages site. See GitHub Pages Source below for details.
-        :param pulumi.Input[str] status: Set to `enabled` to enable advanced security features on the repository. Can be `enabled` or `disabled`.
+        :param pulumi.Input[str] status: The GitHub Pages site's build status e.g. `building` or `built`.
         """
         if build_type is not None:
             pulumi.set(__self__, "build_type", build_type)
         if cname is not None:
             pulumi.set(__self__, "cname", cname)
         if custom404 is not None:
             pulumi.set(__self__, "custom404", custom404)
@@ -2307,15 +2307,15 @@
     def source(self, value: Optional[pulumi.Input['RepositoryPagesSourceArgs']]):
         pulumi.set(self, "source", value)
 
     @property
     @pulumi.getter
     def status(self) -> Optional[pulumi.Input[str]]:
         """
-        Set to `enabled` to enable advanced security features on the repository. Can be `enabled` or `disabled`.
+        The GitHub Pages site's build status e.g. `building` or `built`.
         """
         return pulumi.get(self, "status")
 
     @status.setter
     def status(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "status", value)
 
@@ -2447,37 +2447,37 @@
 
 @pulumi.input_type
 class RepositoryRulesetConditionsRefNameArgs:
     def __init__(__self__, *,
                  excludes: pulumi.Input[Sequence[pulumi.Input[str]]],
                  includes: pulumi.Input[Sequence[pulumi.Input[str]]]):
         """
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] excludes: (List of String) Array of ref names or patterns to exclude. The condition will not pass if any of these patterns match.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] includes: (List of String) Array of ref names or patterns to include. One of these patterns must match for the condition to pass. Also accepts `~DEFAULT_BRANCH` to include the default branch or `~ALL` to include all branches.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] excludes: Array of ref names or patterns to exclude. The condition will not pass if any of these patterns match.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] includes: Array of ref names or patterns to include. One of these patterns must match for the condition to pass. Also accepts `~DEFAULT_BRANCH` to include the default branch or `~ALL` to include all branches.
         """
         pulumi.set(__self__, "excludes", excludes)
         pulumi.set(__self__, "includes", includes)
 
     @property
     @pulumi.getter
     def excludes(self) -> pulumi.Input[Sequence[pulumi.Input[str]]]:
         """
-        (List of String) Array of ref names or patterns to exclude. The condition will not pass if any of these patterns match.
+        Array of ref names or patterns to exclude. The condition will not pass if any of these patterns match.
         """
         return pulumi.get(self, "excludes")
 
     @excludes.setter
     def excludes(self, value: pulumi.Input[Sequence[pulumi.Input[str]]]):
         pulumi.set(self, "excludes", value)
 
     @property
     @pulumi.getter
     def includes(self) -> pulumi.Input[Sequence[pulumi.Input[str]]]:
         """
-        (List of String) Array of ref names or patterns to include. One of these patterns must match for the condition to pass. Also accepts `~DEFAULT_BRANCH` to include the default branch or `~ALL` to include all branches.
+        Array of ref names or patterns to include. One of these patterns must match for the condition to pass. Also accepts `~DEFAULT_BRANCH` to include the default branch or `~ALL` to include all branches.
         """
         return pulumi.get(self, "includes")
 
     @includes.setter
     def includes(self, value: pulumi.Input[Sequence[pulumi.Input[str]]]):
         pulumi.set(self, "includes", value)
 
@@ -2733,43 +2733,43 @@
 class RepositoryRulesetRulesBranchNamePatternArgs:
     def __init__(__self__, *,
                  operator: pulumi.Input[str],
                  pattern: pulumi.Input[str],
                  name: Optional[pulumi.Input[str]] = None,
                  negate: Optional[pulumi.Input[bool]] = None):
         """
-        :param pulumi.Input[str] operator: (String) The operator to use for matching. Can be one of: `starts_with`, `ends_with`, `contains`, `regex`.
-        :param pulumi.Input[str] pattern: (String) The pattern to match with.
+        :param pulumi.Input[str] operator: The operator to use for matching. Can be one of: `starts_with`, `ends_with`, `contains`, `regex`.
+        :param pulumi.Input[str] pattern: The pattern to match with.
         :param pulumi.Input[str] name: (String) The name of the ruleset.
-        :param pulumi.Input[bool] negate: (Boolean) If true, the rule will fail if the pattern matches.
+        :param pulumi.Input[bool] negate: If true, the rule will fail if the pattern matches.
         """
         pulumi.set(__self__, "operator", operator)
         pulumi.set(__self__, "pattern", pattern)
         if name is not None:
             pulumi.set(__self__, "name", name)
         if negate is not None:
             pulumi.set(__self__, "negate", negate)
 
     @property
     @pulumi.getter
     def operator(self) -> pulumi.Input[str]:
         """
-        (String) The operator to use for matching. Can be one of: `starts_with`, `ends_with`, `contains`, `regex`.
+        The operator to use for matching. Can be one of: `starts_with`, `ends_with`, `contains`, `regex`.
         """
         return pulumi.get(self, "operator")
 
     @operator.setter
     def operator(self, value: pulumi.Input[str]):
         pulumi.set(self, "operator", value)
 
     @property
     @pulumi.getter
     def pattern(self) -> pulumi.Input[str]:
         """
-        (String) The pattern to match with.
+        The pattern to match with.
         """
         return pulumi.get(self, "pattern")
 
     @pattern.setter
     def pattern(self, value: pulumi.Input[str]):
         pulumi.set(self, "pattern", value)
 
@@ -2785,15 +2785,15 @@
     def name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "name", value)
 
     @property
     @pulumi.getter
     def negate(self) -> Optional[pulumi.Input[bool]]:
         """
-        (Boolean) If true, the rule will fail if the pattern matches.
+        If true, the rule will fail if the pattern matches.
         """
         return pulumi.get(self, "negate")
 
     @negate.setter
     def negate(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "negate", value)
 
@@ -2802,43 +2802,43 @@
 class RepositoryRulesetRulesCommitAuthorEmailPatternArgs:
     def __init__(__self__, *,
                  operator: pulumi.Input[str],
                  pattern: pulumi.Input[str],
                  name: Optional[pulumi.Input[str]] = None,
                  negate: Optional[pulumi.Input[bool]] = None):
         """
-        :param pulumi.Input[str] operator: (String) The operator to use for matching. Can be one of: `starts_with`, `ends_with`, `contains`, `regex`.
-        :param pulumi.Input[str] pattern: (String) The pattern to match with.
+        :param pulumi.Input[str] operator: The operator to use for matching. Can be one of: `starts_with`, `ends_with`, `contains`, `regex`.
+        :param pulumi.Input[str] pattern: The pattern to match with.
         :param pulumi.Input[str] name: (String) The name of the ruleset.
-        :param pulumi.Input[bool] negate: (Boolean) If true, the rule will fail if the pattern matches.
+        :param pulumi.Input[bool] negate: If true, the rule will fail if the pattern matches.
         """
         pulumi.set(__self__, "operator", operator)
         pulumi.set(__self__, "pattern", pattern)
         if name is not None:
             pulumi.set(__self__, "name", name)
         if negate is not None:
             pulumi.set(__self__, "negate", negate)
 
     @property
     @pulumi.getter
     def operator(self) -> pulumi.Input[str]:
         """
-        (String) The operator to use for matching. Can be one of: `starts_with`, `ends_with`, `contains`, `regex`.
+        The operator to use for matching. Can be one of: `starts_with`, `ends_with`, `contains`, `regex`.
         """
         return pulumi.get(self, "operator")
 
     @operator.setter
     def operator(self, value: pulumi.Input[str]):
         pulumi.set(self, "operator", value)
 
     @property
     @pulumi.getter
     def pattern(self) -> pulumi.Input[str]:
         """
-        (String) The pattern to match with.
+        The pattern to match with.
         """
         return pulumi.get(self, "pattern")
 
     @pattern.setter
     def pattern(self, value: pulumi.Input[str]):
         pulumi.set(self, "pattern", value)
 
@@ -2854,15 +2854,15 @@
     def name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "name", value)
 
     @property
     @pulumi.getter
     def negate(self) -> Optional[pulumi.Input[bool]]:
         """
-        (Boolean) If true, the rule will fail if the pattern matches.
+        If true, the rule will fail if the pattern matches.
         """
         return pulumi.get(self, "negate")
 
     @negate.setter
     def negate(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "negate", value)
 
@@ -2871,43 +2871,43 @@
 class RepositoryRulesetRulesCommitMessagePatternArgs:
     def __init__(__self__, *,
                  operator: pulumi.Input[str],
                  pattern: pulumi.Input[str],
                  name: Optional[pulumi.Input[str]] = None,
                  negate: Optional[pulumi.Input[bool]] = None):
         """
-        :param pulumi.Input[str] operator: (String) The operator to use for matching. Can be one of: `starts_with`, `ends_with`, `contains`, `regex`.
-        :param pulumi.Input[str] pattern: (String) The pattern to match with.
+        :param pulumi.Input[str] operator: The operator to use for matching. Can be one of: `starts_with`, `ends_with`, `contains`, `regex`.
+        :param pulumi.Input[str] pattern: The pattern to match with.
         :param pulumi.Input[str] name: (String) The name of the ruleset.
-        :param pulumi.Input[bool] negate: (Boolean) If true, the rule will fail if the pattern matches.
+        :param pulumi.Input[bool] negate: If true, the rule will fail if the pattern matches.
         """
         pulumi.set(__self__, "operator", operator)
         pulumi.set(__self__, "pattern", pattern)
         if name is not None:
             pulumi.set(__self__, "name", name)
         if negate is not None:
             pulumi.set(__self__, "negate", negate)
 
     @property
     @pulumi.getter
     def operator(self) -> pulumi.Input[str]:
         """
-        (String) The operator to use for matching. Can be one of: `starts_with`, `ends_with`, `contains`, `regex`.
+        The operator to use for matching. Can be one of: `starts_with`, `ends_with`, `contains`, `regex`.
         """
         return pulumi.get(self, "operator")
 
     @operator.setter
     def operator(self, value: pulumi.Input[str]):
         pulumi.set(self, "operator", value)
 
     @property
     @pulumi.getter
     def pattern(self) -> pulumi.Input[str]:
         """
-        (String) The pattern to match with.
+        The pattern to match with.
         """
         return pulumi.get(self, "pattern")
 
     @pattern.setter
     def pattern(self, value: pulumi.Input[str]):
         pulumi.set(self, "pattern", value)
 
@@ -2923,15 +2923,15 @@
     def name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "name", value)
 
     @property
     @pulumi.getter
     def negate(self) -> Optional[pulumi.Input[bool]]:
         """
-        (Boolean) If true, the rule will fail if the pattern matches.
+        If true, the rule will fail if the pattern matches.
         """
         return pulumi.get(self, "negate")
 
     @negate.setter
     def negate(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "negate", value)
 
@@ -2940,43 +2940,43 @@
 class RepositoryRulesetRulesCommitterEmailPatternArgs:
     def __init__(__self__, *,
                  operator: pulumi.Input[str],
                  pattern: pulumi.Input[str],
                  name: Optional[pulumi.Input[str]] = None,
                  negate: Optional[pulumi.Input[bool]] = None):
         """
-        :param pulumi.Input[str] operator: (String) The operator to use for matching. Can be one of: `starts_with`, `ends_with`, `contains`, `regex`.
-        :param pulumi.Input[str] pattern: (String) The pattern to match with.
+        :param pulumi.Input[str] operator: The operator to use for matching. Can be one of: `starts_with`, `ends_with`, `contains`, `regex`.
+        :param pulumi.Input[str] pattern: The pattern to match with.
         :param pulumi.Input[str] name: (String) The name of the ruleset.
-        :param pulumi.Input[bool] negate: (Boolean) If true, the rule will fail if the pattern matches.
+        :param pulumi.Input[bool] negate: If true, the rule will fail if the pattern matches.
         """
         pulumi.set(__self__, "operator", operator)
         pulumi.set(__self__, "pattern", pattern)
         if name is not None:
             pulumi.set(__self__, "name", name)
         if negate is not None:
             pulumi.set(__self__, "negate", negate)
 
     @property
     @pulumi.getter
     def operator(self) -> pulumi.Input[str]:
         """
-        (String) The operator to use for matching. Can be one of: `starts_with`, `ends_with`, `contains`, `regex`.
+        The operator to use for matching. Can be one of: `starts_with`, `ends_with`, `contains`, `regex`.
         """
         return pulumi.get(self, "operator")
 
     @operator.setter
     def operator(self, value: pulumi.Input[str]):
         pulumi.set(self, "operator", value)
 
     @property
     @pulumi.getter
     def pattern(self) -> pulumi.Input[str]:
         """
-        (String) The pattern to match with.
+        The pattern to match with.
         """
         return pulumi.get(self, "pattern")
 
     @pattern.setter
     def pattern(self, value: pulumi.Input[str]):
         pulumi.set(self, "pattern", value)
 
@@ -2992,15 +2992,15 @@
     def name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "name", value)
 
     @property
     @pulumi.getter
     def negate(self) -> Optional[pulumi.Input[bool]]:
         """
-        (Boolean) If true, the rule will fail if the pattern matches.
+        If true, the rule will fail if the pattern matches.
         """
         return pulumi.get(self, "negate")
 
     @negate.setter
     def negate(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "negate", value)
 
@@ -3010,19 +3010,19 @@
     def __init__(__self__, *,
                  dismiss_stale_reviews_on_push: Optional[pulumi.Input[bool]] = None,
                  require_code_owner_review: Optional[pulumi.Input[bool]] = None,
                  require_last_push_approval: Optional[pulumi.Input[bool]] = None,
                  required_approving_review_count: Optional[pulumi.Input[int]] = None,
                  required_review_thread_resolution: Optional[pulumi.Input[bool]] = None):
         """
-        :param pulumi.Input[bool] dismiss_stale_reviews_on_push: (Boolean) New, reviewable commits pushed will dismiss previous pull request review approvals. Defaults to `false`.
-        :param pulumi.Input[bool] require_code_owner_review: (Boolean) Require an approving review in pull requests that modify files that have a designated code owner. Defaults to `false`.
-        :param pulumi.Input[bool] require_last_push_approval: (Boolean) Whether the most recent reviewable push must be approved by someone other than the person who pushed it. Defaults to `false`.
-        :param pulumi.Input[int] required_approving_review_count: (Number) The number of approving reviews that are required before a pull request can be merged. Defaults to `0`.
-        :param pulumi.Input[bool] required_review_thread_resolution: (Boolean) All conversations on code must be resolved before a pull request can be merged. Defaults to `false`.
+        :param pulumi.Input[bool] dismiss_stale_reviews_on_push: New, reviewable commits pushed will dismiss previous pull request review approvals. Defaults to `false`.
+        :param pulumi.Input[bool] require_code_owner_review: Require an approving review in pull requests that modify files that have a designated code owner. Defaults to `false`.
+        :param pulumi.Input[bool] require_last_push_approval: Whether the most recent reviewable push must be approved by someone other than the person who pushed it. Defaults to `false`.
+        :param pulumi.Input[int] required_approving_review_count: The number of approving reviews that are required before a pull request can be merged. Defaults to `0`.
+        :param pulumi.Input[bool] required_review_thread_resolution: All conversations on code must be resolved before a pull request can be merged. Defaults to `false`.
         """
         if dismiss_stale_reviews_on_push is not None:
             pulumi.set(__self__, "dismiss_stale_reviews_on_push", dismiss_stale_reviews_on_push)
         if require_code_owner_review is not None:
             pulumi.set(__self__, "require_code_owner_review", require_code_owner_review)
         if require_last_push_approval is not None:
             pulumi.set(__self__, "require_last_push_approval", require_last_push_approval)
@@ -3031,161 +3031,161 @@
         if required_review_thread_resolution is not None:
             pulumi.set(__self__, "required_review_thread_resolution", required_review_thread_resolution)
 
     @property
     @pulumi.getter(name="dismissStaleReviewsOnPush")
     def dismiss_stale_reviews_on_push(self) -> Optional[pulumi.Input[bool]]:
         """
-        (Boolean) New, reviewable commits pushed will dismiss previous pull request review approvals. Defaults to `false`.
+        New, reviewable commits pushed will dismiss previous pull request review approvals. Defaults to `false`.
         """
         return pulumi.get(self, "dismiss_stale_reviews_on_push")
 
     @dismiss_stale_reviews_on_push.setter
     def dismiss_stale_reviews_on_push(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "dismiss_stale_reviews_on_push", value)
 
     @property
     @pulumi.getter(name="requireCodeOwnerReview")
     def require_code_owner_review(self) -> Optional[pulumi.Input[bool]]:
         """
-        (Boolean) Require an approving review in pull requests that modify files that have a designated code owner. Defaults to `false`.
+        Require an approving review in pull requests that modify files that have a designated code owner. Defaults to `false`.
         """
         return pulumi.get(self, "require_code_owner_review")
 
     @require_code_owner_review.setter
     def require_code_owner_review(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "require_code_owner_review", value)
 
     @property
     @pulumi.getter(name="requireLastPushApproval")
     def require_last_push_approval(self) -> Optional[pulumi.Input[bool]]:
         """
-        (Boolean) Whether the most recent reviewable push must be approved by someone other than the person who pushed it. Defaults to `false`.
+        Whether the most recent reviewable push must be approved by someone other than the person who pushed it. Defaults to `false`.
         """
         return pulumi.get(self, "require_last_push_approval")
 
     @require_last_push_approval.setter
     def require_last_push_approval(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "require_last_push_approval", value)
 
     @property
     @pulumi.getter(name="requiredApprovingReviewCount")
     def required_approving_review_count(self) -> Optional[pulumi.Input[int]]:
         """
-        (Number) The number of approving reviews that are required before a pull request can be merged. Defaults to `0`.
+        The number of approving reviews that are required before a pull request can be merged. Defaults to `0`.
         """
         return pulumi.get(self, "required_approving_review_count")
 
     @required_approving_review_count.setter
     def required_approving_review_count(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "required_approving_review_count", value)
 
     @property
     @pulumi.getter(name="requiredReviewThreadResolution")
     def required_review_thread_resolution(self) -> Optional[pulumi.Input[bool]]:
         """
-        (Boolean) All conversations on code must be resolved before a pull request can be merged. Defaults to `false`.
+        All conversations on code must be resolved before a pull request can be merged. Defaults to `false`.
         """
         return pulumi.get(self, "required_review_thread_resolution")
 
     @required_review_thread_resolution.setter
     def required_review_thread_resolution(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "required_review_thread_resolution", value)
 
 
 @pulumi.input_type
 class RepositoryRulesetRulesRequiredDeploymentsArgs:
     def __init__(__self__, *,
                  required_deployment_environments: pulumi.Input[Sequence[pulumi.Input[str]]]):
         """
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] required_deployment_environments: (List of String) The environments that must be successfully deployed to before branches can be merged.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] required_deployment_environments: The environments that must be successfully deployed to before branches can be merged.
         """
         pulumi.set(__self__, "required_deployment_environments", required_deployment_environments)
 
     @property
     @pulumi.getter(name="requiredDeploymentEnvironments")
     def required_deployment_environments(self) -> pulumi.Input[Sequence[pulumi.Input[str]]]:
         """
-        (List of String) The environments that must be successfully deployed to before branches can be merged.
+        The environments that must be successfully deployed to before branches can be merged.
         """
         return pulumi.get(self, "required_deployment_environments")
 
     @required_deployment_environments.setter
     def required_deployment_environments(self, value: pulumi.Input[Sequence[pulumi.Input[str]]]):
         pulumi.set(self, "required_deployment_environments", value)
 
 
 @pulumi.input_type
 class RepositoryRulesetRulesRequiredStatusChecksArgs:
     def __init__(__self__, *,
                  required_checks: pulumi.Input[Sequence[pulumi.Input['RepositoryRulesetRulesRequiredStatusChecksRequiredCheckArgs']]],
                  strict_required_status_checks_policy: Optional[pulumi.Input[bool]] = None):
         """
-        :param pulumi.Input[Sequence[pulumi.Input['RepositoryRulesetRulesRequiredStatusChecksRequiredCheckArgs']]] required_checks: (Block Set, Min: 1) Status checks that are required. Several can be defined. (see below for nested schema)
-        :param pulumi.Input[bool] strict_required_status_checks_policy: (Boolean) Whether pull requests targeting a matching branch must be tested with the latest code. This setting will not take effect unless at least one status check is enabled. Defaults to `false`.
+        :param pulumi.Input[Sequence[pulumi.Input['RepositoryRulesetRulesRequiredStatusChecksRequiredCheckArgs']]] required_checks: Status checks that are required. Several can be defined.
+        :param pulumi.Input[bool] strict_required_status_checks_policy: Whether pull requests targeting a matching branch must be tested with the latest code. This setting will not take effect unless at least one status check is enabled. Defaults to `false`.
         """
         pulumi.set(__self__, "required_checks", required_checks)
         if strict_required_status_checks_policy is not None:
             pulumi.set(__self__, "strict_required_status_checks_policy", strict_required_status_checks_policy)
 
     @property
     @pulumi.getter(name="requiredChecks")
     def required_checks(self) -> pulumi.Input[Sequence[pulumi.Input['RepositoryRulesetRulesRequiredStatusChecksRequiredCheckArgs']]]:
         """
-        (Block Set, Min: 1) Status checks that are required. Several can be defined. (see below for nested schema)
+        Status checks that are required. Several can be defined.
         """
         return pulumi.get(self, "required_checks")
 
     @required_checks.setter
     def required_checks(self, value: pulumi.Input[Sequence[pulumi.Input['RepositoryRulesetRulesRequiredStatusChecksRequiredCheckArgs']]]):
         pulumi.set(self, "required_checks", value)
 
     @property
     @pulumi.getter(name="strictRequiredStatusChecksPolicy")
     def strict_required_status_checks_policy(self) -> Optional[pulumi.Input[bool]]:
         """
-        (Boolean) Whether pull requests targeting a matching branch must be tested with the latest code. This setting will not take effect unless at least one status check is enabled. Defaults to `false`.
+        Whether pull requests targeting a matching branch must be tested with the latest code. This setting will not take effect unless at least one status check is enabled. Defaults to `false`.
         """
         return pulumi.get(self, "strict_required_status_checks_policy")
 
     @strict_required_status_checks_policy.setter
     def strict_required_status_checks_policy(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "strict_required_status_checks_policy", value)
 
 
 @pulumi.input_type
 class RepositoryRulesetRulesRequiredStatusChecksRequiredCheckArgs:
     def __init__(__self__, *,
                  context: pulumi.Input[str],
                  integration_id: Optional[pulumi.Input[int]] = None):
         """
-        :param pulumi.Input[str] context: (String) The status check context name that must be present on the commit.
-        :param pulumi.Input[int] integration_id: (Number) The optional integration ID that this status check must originate from.
+        :param pulumi.Input[str] context: The status check context name that must be present on the commit.
+        :param pulumi.Input[int] integration_id: The optional integration ID that this status check must originate from.
         """
         pulumi.set(__self__, "context", context)
         if integration_id is not None:
             pulumi.set(__self__, "integration_id", integration_id)
 
     @property
     @pulumi.getter
     def context(self) -> pulumi.Input[str]:
         """
-        (String) The status check context name that must be present on the commit.
+        The status check context name that must be present on the commit.
         """
         return pulumi.get(self, "context")
 
     @context.setter
     def context(self, value: pulumi.Input[str]):
         pulumi.set(self, "context", value)
 
     @property
     @pulumi.getter(name="integrationId")
     def integration_id(self) -> Optional[pulumi.Input[int]]:
         """
-        (Number) The optional integration ID that this status check must originate from.
+        The optional integration ID that this status check must originate from.
         """
         return pulumi.get(self, "integration_id")
 
     @integration_id.setter
     def integration_id(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "integration_id", value)
 
@@ -3194,43 +3194,43 @@
 class RepositoryRulesetRulesTagNamePatternArgs:
     def __init__(__self__, *,
                  operator: pulumi.Input[str],
                  pattern: pulumi.Input[str],
                  name: Optional[pulumi.Input[str]] = None,
                  negate: Optional[pulumi.Input[bool]] = None):
         """
-        :param pulumi.Input[str] operator: (String) The operator to use for matching. Can be one of: `starts_with`, `ends_with`, `contains`, `regex`.
-        :param pulumi.Input[str] pattern: (String) The pattern to match with.
+        :param pulumi.Input[str] operator: The operator to use for matching. Can be one of: `starts_with`, `ends_with`, `contains`, `regex`.
+        :param pulumi.Input[str] pattern: The pattern to match with.
         :param pulumi.Input[str] name: (String) The name of the ruleset.
-        :param pulumi.Input[bool] negate: (Boolean) If true, the rule will fail if the pattern matches.
+        :param pulumi.Input[bool] negate: If true, the rule will fail if the pattern matches.
         """
         pulumi.set(__self__, "operator", operator)
         pulumi.set(__self__, "pattern", pattern)
         if name is not None:
             pulumi.set(__self__, "name", name)
         if negate is not None:
             pulumi.set(__self__, "negate", negate)
 
     @property
     @pulumi.getter
     def operator(self) -> pulumi.Input[str]:
         """
-        (String) The operator to use for matching. Can be one of: `starts_with`, `ends_with`, `contains`, `regex`.
+        The operator to use for matching. Can be one of: `starts_with`, `ends_with`, `contains`, `regex`.
         """
         return pulumi.get(self, "operator")
 
     @operator.setter
     def operator(self, value: pulumi.Input[str]):
         pulumi.set(self, "operator", value)
 
     @property
     @pulumi.getter
     def pattern(self) -> pulumi.Input[str]:
         """
-        (String) The pattern to match with.
+        The pattern to match with.
         """
         return pulumi.get(self, "pattern")
 
     @pattern.setter
     def pattern(self, value: pulumi.Input[str]):
         pulumi.set(self, "pattern", value)
 
@@ -3246,15 +3246,15 @@
     def name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "name", value)
 
     @property
     @pulumi.getter
     def negate(self) -> Optional[pulumi.Input[bool]]:
         """
-        (Boolean) If true, the rule will fail if the pattern matches.
+        If true, the rule will fail if the pattern matches.
         """
         return pulumi.get(self, "negate")
 
     @negate.setter
     def negate(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "negate", value)
 
@@ -3337,45 +3337,45 @@
 
 
 @pulumi.input_type
 class RepositorySecurityAndAnalysisSecretScanningArgs:
     def __init__(__self__, *,
                  status: pulumi.Input[str]):
         """
-        :param pulumi.Input[str] status: Set to `enabled` to enable advanced security features on the repository. Can be `enabled` or `disabled`.
+        :param pulumi.Input[str] status: The GitHub Pages site's build status e.g. `building` or `built`.
         """
         pulumi.set(__self__, "status", status)
 
     @property
     @pulumi.getter
     def status(self) -> pulumi.Input[str]:
         """
-        Set to `enabled` to enable advanced security features on the repository. Can be `enabled` or `disabled`.
+        The GitHub Pages site's build status e.g. `building` or `built`.
         """
         return pulumi.get(self, "status")
 
     @status.setter
     def status(self, value: pulumi.Input[str]):
         pulumi.set(self, "status", value)
 
 
 @pulumi.input_type
 class RepositorySecurityAndAnalysisSecretScanningPushProtectionArgs:
     def __init__(__self__, *,
                  status: pulumi.Input[str]):
         """
-        :param pulumi.Input[str] status: Set to `enabled` to enable advanced security features on the repository. Can be `enabled` or `disabled`.
+        :param pulumi.Input[str] status: The GitHub Pages site's build status e.g. `building` or `built`.
         """
         pulumi.set(__self__, "status", status)
 
     @property
     @pulumi.getter
     def status(self) -> pulumi.Input[str]:
         """
-        Set to `enabled` to enable advanced security features on the repository. Can be `enabled` or `disabled`.
+        The GitHub Pages site's build status e.g. `building` or `built`.
         """
         return pulumi.get(self, "status")
 
     @status.setter
     def status(self, value: pulumi.Input[str]):
         pulumi.set(self, "status", value)
 
@@ -3546,54 +3546,54 @@
 @pulumi.input_type
 class TeamSettingsReviewRequestDelegationArgs:
     def __init__(__self__, *,
                  algorithm: Optional[pulumi.Input[str]] = None,
                  member_count: Optional[pulumi.Input[int]] = None,
                  notify: Optional[pulumi.Input[bool]] = None):
         """
-        :param pulumi.Input[str] algorithm: The algorithm to use when assigning pull requests to team members. Supported values are `ROUND_ROBIN` and `LOAD_BALANCE`. Default value is `ROUND_ROBIN`
-        :param pulumi.Input[int] member_count: The number of team members to assign to a pull request
-        :param pulumi.Input[bool] notify: whether to notify the entire team when at least one member is also assigned to the pull request
+        :param pulumi.Input[str] algorithm: The algorithm to use when assigning pull requests to team members. Supported values are 'ROUND_ROBIN' and 'LOAD_BALANCE'.
+        :param pulumi.Input[int] member_count: The number of team members to assign to a pull request.
+        :param pulumi.Input[bool] notify: whether to notify the entire team when at least one member is also assigned to the pull request.
         """
         if algorithm is not None:
             pulumi.set(__self__, "algorithm", algorithm)
         if member_count is not None:
             pulumi.set(__self__, "member_count", member_count)
         if notify is not None:
             pulumi.set(__self__, "notify", notify)
 
     @property
     @pulumi.getter
     def algorithm(self) -> Optional[pulumi.Input[str]]:
         """
-        The algorithm to use when assigning pull requests to team members. Supported values are `ROUND_ROBIN` and `LOAD_BALANCE`. Default value is `ROUND_ROBIN`
+        The algorithm to use when assigning pull requests to team members. Supported values are 'ROUND_ROBIN' and 'LOAD_BALANCE'.
         """
         return pulumi.get(self, "algorithm")
 
     @algorithm.setter
     def algorithm(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "algorithm", value)
 
     @property
     @pulumi.getter(name="memberCount")
     def member_count(self) -> Optional[pulumi.Input[int]]:
         """
-        The number of team members to assign to a pull request
+        The number of team members to assign to a pull request.
         """
         return pulumi.get(self, "member_count")
 
     @member_count.setter
     def member_count(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "member_count", value)
 
     @property
     @pulumi.getter
     def notify(self) -> Optional[pulumi.Input[bool]]:
         """
-        whether to notify the entire team when at least one member is also assigned to the pull request
+        whether to notify the entire team when at least one member is also assigned to the pull request.
         """
         return pulumi.get(self, "notify")
 
     @notify.setter
     def notify(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "notify", value)
```

### Comparing `pulumi_github-6.3.0a1713561029/pulumi_github/_utilities.py` & `pulumi_github-6.3.0a1713897837/pulumi_github/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-6.3.0a1713561029/pulumi_github/actions_environment_secret.py` & `pulumi_github-6.3.0a1713897837/pulumi_github/actions_environment_secret.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-6.3.0a1713561029/pulumi_github/actions_environment_variable.py` & `pulumi_github-6.3.0a1713897837/pulumi_github/actions_environment_variable.py`

 * *Files 3% similar despite different names*

```diff
@@ -195,42 +195,38 @@
                  __props__=None):
         """
         This resource allows you to create and manage GitHub Actions variables within your GitHub repository environments.
         You must have write access to a repository to use this resource.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_github as github
 
         example_variable = github.ActionsEnvironmentVariable("example_variable",
             environment="example_environment",
             variable_name="example_variable_name",
             value="example_variable_value")
         ```
-        <!--End PulumiCodeChooser -->
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_github as github
 
         repo = github.get_repository(full_name="my-org/repo")
         repo_environment = github.RepositoryEnvironment("repo_environment",
             repository=repo.name,
             environment="example_environment")
         example_variable = github.ActionsEnvironmentVariable("example_variable",
             repository=repo.name,
             environment=repo_environment.environment,
             variable_name="example_variable_name",
             value="example_variable_value")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         This resource can be imported using an ID made up of the repository name, environment name, and variable name:
 
         ```sh
         $ pulumi import github:index/actionsEnvironmentVariable:ActionsEnvironmentVariable test_variable myrepo:myenv:myvariable
@@ -251,42 +247,38 @@
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         This resource allows you to create and manage GitHub Actions variables within your GitHub repository environments.
         You must have write access to a repository to use this resource.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_github as github
 
         example_variable = github.ActionsEnvironmentVariable("example_variable",
             environment="example_environment",
             variable_name="example_variable_name",
             value="example_variable_value")
         ```
-        <!--End PulumiCodeChooser -->
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_github as github
 
         repo = github.get_repository(full_name="my-org/repo")
         repo_environment = github.RepositoryEnvironment("repo_environment",
             repository=repo.name,
             environment="example_environment")
         example_variable = github.ActionsEnvironmentVariable("example_variable",
             repository=repo.name,
             environment=repo_environment.environment,
             variable_name="example_variable_name",
             value="example_variable_value")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         This resource can be imported using an ID made up of the repository name, environment name, and variable name:
 
         ```sh
         $ pulumi import github:index/actionsEnvironmentVariable:ActionsEnvironmentVariable test_variable myrepo:myenv:myvariable
```

### Comparing `pulumi_github-6.3.0a1713561029/pulumi_github/actions_organization_oidc_subject_claim_customization_template.py` & `pulumi_github-6.3.0a1713897837/pulumi_github/actions_organization_oidc_subject_claim_customization_template.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,26 +70,24 @@
         organization.
 
         More information on integrating GitHub with cloud providers using OpenID Connect and a list of available claims is
         available in the [Actions documentation](https://docs.github.com/en/actions/deployment/security-hardening-your-deployments/about-security-hardening-with-openid-connect).
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_github as github
 
         example_template = github.ActionsOrganizationOidcSubjectClaimCustomizationTemplate("example_template", include_claim_keys=[
             "actor",
             "context",
             "repository_owner",
         ])
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         This resource can be imported using the organization's name.
 
         ```sh
         $ pulumi import github:index/actionsOrganizationOidcSubjectClaimCustomizationTemplate:ActionsOrganizationOidcSubjectClaimCustomizationTemplate test example_organization
@@ -110,26 +108,24 @@
         organization.
 
         More information on integrating GitHub with cloud providers using OpenID Connect and a list of available claims is
         available in the [Actions documentation](https://docs.github.com/en/actions/deployment/security-hardening-your-deployments/about-security-hardening-with-openid-connect).
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_github as github
 
         example_template = github.ActionsOrganizationOidcSubjectClaimCustomizationTemplate("example_template", include_claim_keys=[
             "actor",
             "context",
             "repository_owner",
         ])
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         This resource can be imported using the organization's name.
 
         ```sh
         $ pulumi import github:index/actionsOrganizationOidcSubjectClaimCustomizationTemplate:ActionsOrganizationOidcSubjectClaimCustomizationTemplate test example_organization
```

### Comparing `pulumi_github-6.3.0a1713561029/pulumi_github/actions_organization_permissions.py` & `pulumi_github-6.3.0a1713897837/pulumi_github/actions_organization_permissions.py`

 * *Files 1% similar despite different names*

```diff
@@ -168,15 +168,14 @@
                  __props__=None):
         """
         This resource allows you to create and manage GitHub Actions permissions within your GitHub enterprise organizations.
         You must have admin access to an organization to use this resource.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_github as github
 
         example = github.Repository("example", name="my-repository")
         test = github.ActionsOrganizationPermissions("test",
             allowed_actions="selected",
@@ -189,15 +188,14 @@
                 ],
                 verified_allowed=True,
             ),
             enabled_repositories_config=github.ActionsOrganizationPermissionsEnabledRepositoriesConfigArgs(
                 repository_ids=[example.repo_id],
             ))
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         This resource can be imported using the name of the GitHub organization:
 
         ```sh
         $ pulumi import github:index/actionsOrganizationPermissions:ActionsOrganizationPermissions test github_organization_name
@@ -218,15 +216,14 @@
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         This resource allows you to create and manage GitHub Actions permissions within your GitHub enterprise organizations.
         You must have admin access to an organization to use this resource.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_github as github
 
         example = github.Repository("example", name="my-repository")
         test = github.ActionsOrganizationPermissions("test",
             allowed_actions="selected",
@@ -239,15 +236,14 @@
                 ],
                 verified_allowed=True,
             ),
             enabled_repositories_config=github.ActionsOrganizationPermissionsEnabledRepositoriesConfigArgs(
                 repository_ids=[example.repo_id],
             ))
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         This resource can be imported using the name of the GitHub organization:
 
         ```sh
         $ pulumi import github:index/actionsOrganizationPermissions:ActionsOrganizationPermissions test github_organization_name
```

### Comparing `pulumi_github-6.3.0a1713561029/pulumi_github/actions_organization_secret.py` & `pulumi_github-6.3.0a1713897837/pulumi_github/actions_organization_secret.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-6.3.0a1713561029/pulumi_github/actions_organization_secret_repositories.py` & `pulumi_github-6.3.0a1713897837/pulumi_github/actions_organization_secret_repositories.py`

 * *Files 2% similar despite different names*

```diff
@@ -101,25 +101,23 @@
         This resource allows you to manage repository allow list for existing GitHub Actions secrets within your GitHub organization.
         You must have write access to an organization secret to use this resource.
 
         This resource is only applicable when `visibility` of the existing organization secret has been set to `selected`.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_github as github
 
         repo = github.get_repository(full_name="my-org/repo")
         org_secret_repos = github.ActionsOrganizationSecretRepositories("org_secret_repos",
             secret_name="existing_secret_name",
             selected_repository_ids=[repo.repo_id])
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         This resource can be imported using an ID made up of the secret name:
 
         ```sh
         $ pulumi import github:index/actionsOrganizationSecretRepositories:ActionsOrganizationSecretRepositories test_secret_repos test_secret_name
@@ -140,25 +138,23 @@
         This resource allows you to manage repository allow list for existing GitHub Actions secrets within your GitHub organization.
         You must have write access to an organization secret to use this resource.
 
         This resource is only applicable when `visibility` of the existing organization secret has been set to `selected`.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_github as github
 
         repo = github.get_repository(full_name="my-org/repo")
         org_secret_repos = github.ActionsOrganizationSecretRepositories("org_secret_repos",
             secret_name="existing_secret_name",
             selected_repository_ids=[repo.repo_id])
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         This resource can be imported using an ID made up of the secret name:
 
         ```sh
         $ pulumi import github:index/actionsOrganizationSecretRepositories:ActionsOrganizationSecretRepositories test_secret_repos test_secret_name
```

### Comparing `pulumi_github-6.3.0a1713561029/pulumi_github/actions_organization_variable.py` & `pulumi_github-6.3.0a1713897837/pulumi_github/actions_organization_variable.py`

 * *Files 2% similar despite different names*

```diff
@@ -200,39 +200,35 @@
                  __props__=None):
         """
         This resource allows you to create and manage GitHub Actions variables within your GitHub organization.
         You must have write access to a repository to use this resource.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_github as github
 
         example_variable = github.ActionsOrganizationVariable("example_variable",
             variable_name="example_variable_name",
             visibility="private",
             value="example_variable_value")
         ```
-        <!--End PulumiCodeChooser -->
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_github as github
 
         repo = github.get_repository(full_name="my-org/repo")
         example_variable = github.ActionsOrganizationVariable("example_variable",
             variable_name="example_variable_name",
             visibility="selected",
             value="example_variable_value",
             selected_repository_ids=[repo.repo_id])
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         This resource can be imported using an ID made up of the variable name:
 
         ```sh
         $ pulumi import github:index/actionsOrganizationVariable:ActionsOrganizationVariable test_variable test_variable_name
@@ -254,39 +250,35 @@
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         This resource allows you to create and manage GitHub Actions variables within your GitHub organization.
         You must have write access to a repository to use this resource.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_github as github
 
         example_variable = github.ActionsOrganizationVariable("example_variable",
             variable_name="example_variable_name",
             visibility="private",
             value="example_variable_value")
         ```
-        <!--End PulumiCodeChooser -->
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_github as github
 
         repo = github.get_repository(full_name="my-org/repo")
         example_variable = github.ActionsOrganizationVariable("example_variable",
             variable_name="example_variable_name",
             visibility="selected",
             value="example_variable_value",
             selected_repository_ids=[repo.repo_id])
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         This resource can be imported using an ID made up of the variable name:
 
         ```sh
         $ pulumi import github:index/actionsOrganizationVariable:ActionsOrganizationVariable test_variable test_variable_name
```

### Comparing `pulumi_github-6.3.0a1713561029/pulumi_github/actions_repository_access_level.py` & `pulumi_github-6.3.0a1713897837/pulumi_github/actions_repository_access_level.py`

 * *Files 4% similar despite different names*

```diff
@@ -99,27 +99,25 @@
                  __props__=None):
         """
         This resource allows you to set the access level of a non-public repositories actions and reusable workflows for use in other repositories.
         You must have admin access to a repository to use this resource.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_github as github
 
         example = github.Repository("example",
             name="my-repository",
             visibility="private")
         test = github.ActionsRepositoryAccessLevel("test",
             access_level="user",
             repository=example.name)
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         This resource can be imported using the name of the GitHub repository:
 
         ```sh
         $ pulumi import github:index/actionsRepositoryAccessLevel:ActionsRepositoryAccessLevel test my-repository
@@ -138,27 +136,25 @@
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         This resource allows you to set the access level of a non-public repositories actions and reusable workflows for use in other repositories.
         You must have admin access to a repository to use this resource.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_github as github
 
         example = github.Repository("example",
             name="my-repository",
             visibility="private")
         test = github.ActionsRepositoryAccessLevel("test",
             access_level="user",
             repository=example.name)
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         This resource can be imported using the name of the GitHub repository:
 
         ```sh
         $ pulumi import github:index/actionsRepositoryAccessLevel:ActionsRepositoryAccessLevel test my-repository
```

### Comparing `pulumi_github-6.3.0a1713561029/pulumi_github/actions_repository_oidc_subject_claim_customization_template.py` & `pulumi_github-6.3.0a1713897837/pulumi_github/actions_repository_oidc_subject_claim_customization_template.py`

 * *Files 1% similar despite different names*

```diff
@@ -147,30 +147,28 @@
         |---------------|----------------------|-----------------------------------------------------------|
         | `true`        | Unset                | GitHub's default                                          |
         | `false`       | Set                  | `include_claim_keys`                                      |
         | `false`       | Unset                | Organization's default if set, otherwise GitHub's default |
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_github as github
 
         example = github.Repository("example", name="example-repository")
         example_template = github.ActionsRepositoryOidcSubjectClaimCustomizationTemplate("example_template",
             repository=example.name,
             use_default=False,
             include_claim_keys=[
                 "actor",
                 "context",
                 "repository_owner",
             ])
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         This resource can be imported using the repository's name.
 
         ```sh
         $ pulumi import github:index/actionsRepositoryOidcSubjectClaimCustomizationTemplate:ActionsRepositoryOidcSubjectClaimCustomizationTemplate test example_repository
@@ -202,30 +200,28 @@
         |---------------|----------------------|-----------------------------------------------------------|
         | `true`        | Unset                | GitHub's default                                          |
         | `false`       | Set                  | `include_claim_keys`                                      |
         | `false`       | Unset                | Organization's default if set, otherwise GitHub's default |
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_github as github
 
         example = github.Repository("example", name="example-repository")
         example_template = github.ActionsRepositoryOidcSubjectClaimCustomizationTemplate("example_template",
             repository=example.name,
             use_default=False,
             include_claim_keys=[
                 "actor",
                 "context",
                 "repository_owner",
             ])
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         This resource can be imported using the repository's name.
 
         ```sh
         $ pulumi import github:index/actionsRepositoryOidcSubjectClaimCustomizationTemplate:ActionsRepositoryOidcSubjectClaimCustomizationTemplate test example_repository
```

### Comparing `pulumi_github-6.3.0a1713561029/pulumi_github/actions_repository_permissions.py` & `pulumi_github-6.3.0a1713897837/pulumi_github/actions_repository_permissions.py`

 * *Files 1% similar despite different names*

```diff
@@ -168,15 +168,14 @@
                  __props__=None):
         """
         This resource allows you to enable and manage GitHub Actions permissions for a given repository.
         You must have admin access to an repository to use this resource.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_github as github
 
         example = github.Repository("example", name="my-repository")
         test = github.ActionsRepositoryPermissions("test",
             allowed_actions="selected",
@@ -186,15 +185,14 @@
                     "actions/cache@*",
                     "actions/checkout@*",
                 ],
                 verified_allowed=True,
             ),
             repository=example.name)
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         This resource can be imported using the name of the GitHub repository:
 
         ```sh
         $ pulumi import github:index/actionsRepositoryPermissions:ActionsRepositoryPermissions test my-repository
@@ -215,15 +213,14 @@
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         This resource allows you to enable and manage GitHub Actions permissions for a given repository.
         You must have admin access to an repository to use this resource.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_github as github
 
         example = github.Repository("example", name="my-repository")
         test = github.ActionsRepositoryPermissions("test",
             allowed_actions="selected",
@@ -233,15 +230,14 @@
                     "actions/cache@*",
                     "actions/checkout@*",
                 ],
                 verified_allowed=True,
             ),
             repository=example.name)
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         This resource can be imported using the name of the GitHub repository:
 
         ```sh
         $ pulumi import github:index/actionsRepositoryPermissions:ActionsRepositoryPermissions test my-repository
```

### Comparing `pulumi_github-6.3.0a1713561029/pulumi_github/actions_runner_group.py` & `pulumi_github-6.3.0a1713897837/pulumi_github/actions_runner_group.py`

 * *Files 1% similar despite different names*

```diff
@@ -312,26 +312,24 @@
                  __props__=None):
         """
         This resource allows you to create and manage GitHub Actions runner groups within your GitHub enterprise organizations.
         You must have admin access to an organization to use this resource.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_github as github
 
         example = github.Repository("example", name="my-repository")
         example_actions_runner_group = github.ActionsRunnerGroup("example",
             name=example.name,
             visibility="selected",
             selected_repository_ids=[example.repo_id])
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         This resource can be imported using the ID of the runner group:
 
         ```sh
         $ pulumi import github:index/actionsRunnerGroup:ActionsRunnerGroup test 7
@@ -354,26 +352,24 @@
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         This resource allows you to create and manage GitHub Actions runner groups within your GitHub enterprise organizations.
         You must have admin access to an organization to use this resource.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_github as github
 
         example = github.Repository("example", name="my-repository")
         example_actions_runner_group = github.ActionsRunnerGroup("example",
             name=example.name,
             visibility="selected",
             selected_repository_ids=[example.repo_id])
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         This resource can be imported using the ID of the runner group:
 
         ```sh
         $ pulumi import github:index/actionsRunnerGroup:ActionsRunnerGroup test 7
```

### Comparing `pulumi_github-6.3.0a1713561029/pulumi_github/actions_secret.py` & `pulumi_github-6.3.0a1713897837/pulumi_github/actions_secret.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-6.3.0a1713561029/pulumi_github/actions_variable.py` & `pulumi_github-6.3.0a1713897837/pulumi_github/actions_variable.py`

 * *Files 2% similar despite different names*

```diff
@@ -163,25 +163,23 @@
                  __props__=None):
         """
         This resource allows you to create and manage GitHub Actions variables within your GitHub repositories.
         You must have write access to a repository to use this resource.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_github as github
 
         example_variable = github.ActionsVariable("example_variable",
             repository="example_repository",
             variable_name="example_variable_name",
             value="example_variable_value")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         GitHub Actions variables can be imported using an ID made up of `repository:variable_name`, e.g.
 
         ```sh
         $ pulumi import github:index/actionsVariable:ActionsVariable myvariable myrepo:myvariable
@@ -201,25 +199,23 @@
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         This resource allows you to create and manage GitHub Actions variables within your GitHub repositories.
         You must have write access to a repository to use this resource.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_github as github
 
         example_variable = github.ActionsVariable("example_variable",
             repository="example_repository",
             variable_name="example_variable_name",
             value="example_variable_value")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         GitHub Actions variables can be imported using an ID made up of `repository:variable_name`, e.g.
 
         ```sh
         $ pulumi import github:index/actionsVariable:ActionsVariable myvariable myrepo:myvariable
```

### Comparing `pulumi_github-6.3.0a1713561029/pulumi_github/app_installation_repositories.py` & `pulumi_github-6.3.0a1713897837/pulumi_github/app_installation_repositories.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-6.3.0a1713561029/pulumi_github/app_installation_repository.py` & `pulumi_github-6.3.0a1713897837/pulumi_github/app_installation_repository.py`

 * *Files 5% similar despite different names*

```diff
@@ -120,26 +120,24 @@
         The app installation and the repository must both belong to the same
         organization on GitHub. Note: you can review your organization's installations
         by the following the instructions at this
         [link](https://docs.github.com/en/github/setting-up-and-managing-organizations-and-teams/reviewing-your-organizations-installed-integrations).
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_github as github
 
         # Create a repository.
         some_repo = github.Repository("some_repo", name="some-repo")
         some_app_repo = github.AppInstallationRepository("some_app_repo",
             installation_id="1234567",
             repository=some_repo.name)
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         GitHub App Installation Repository can be imported
         using an ID made up of `installation_id:repository`, e.g.
 
         ```sh
@@ -168,26 +166,24 @@
         The app installation and the repository must both belong to the same
         organization on GitHub. Note: you can review your organization's installations
         by the following the instructions at this
         [link](https://docs.github.com/en/github/setting-up-and-managing-organizations-and-teams/reviewing-your-organizations-installed-integrations).
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_github as github
 
         # Create a repository.
         some_repo = github.Repository("some_repo", name="some-repo")
         some_app_repo = github.AppInstallationRepository("some_app_repo",
             installation_id="1234567",
             repository=some_repo.name)
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         GitHub App Installation Repository can be imported
         using an ID made up of `installation_id:repository`, e.g.
 
         ```sh
```

### Comparing `pulumi_github-6.3.0a1713561029/pulumi_github/branch.py` & `pulumi_github-6.3.0a1713897837/pulumi_github/branch.py`

 * *Files 2% similar despite different names*

```diff
@@ -215,24 +215,22 @@
         This resource allows you to create and manage branches within your repository.
 
         Additional constraints can be applied to ensure your branch is created from
         another branch or commit.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_github as github
 
         development = github.Branch("development",
             repository="example",
             branch="development")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         GitHub Branch can be imported using an ID made up of `repository:branch`, e.g.
 
         ```sh
         $ pulumi import github:index/branch:Branch terraform terraform:main
@@ -266,24 +264,22 @@
         This resource allows you to create and manage branches within your repository.
 
         Additional constraints can be applied to ensure your branch is created from
         another branch or commit.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_github as github
 
         development = github.Branch("development",
             repository="example",
             branch="development")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         GitHub Branch can be imported using an ID made up of `repository:branch`, e.g.
 
         ```sh
         $ pulumi import github:index/branch:Branch terraform terraform:main
```

### Comparing `pulumi_github-6.3.0a1713561029/pulumi_github/branch_default.py` & `pulumi_github-6.3.0a1713897837/pulumi_github/branch_default.py`

 * *Files 8% similar despite different names*

```diff
@@ -149,15 +149,14 @@
 
         Note that use of this resource is incompatible with the `default_branch` option of the `Repository` resource.  Using both will result in plans always showing a diff.
 
         ## Example Usage
 
         Basic usage:
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_github as github
 
         example = github.Repository("example",
             name="example",
             description="My awesome codebase",
@@ -165,33 +164,30 @@
         development = github.Branch("development",
             repository=example.name,
             branch="development")
         default = github.BranchDefault("default",
             repository=example.name,
             branch=development.branch)
         ```
-        <!--End PulumiCodeChooser -->
 
         Renaming to a branch that doesn't exist:
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_github as github
 
         example = github.Repository("example",
             name="example",
             description="My awesome codebase",
             auto_init=True)
         default = github.BranchDefault("default",
             repository=example.name,
             branch="development",
             rename=True)
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         GitHub Branch Defaults can be imported using an ID made up of `repository`, e.g.
 
         ```sh
         $ pulumi import github:index/branchDefault:BranchDefault branch_default my-repo
@@ -216,15 +212,14 @@
 
         Note that use of this resource is incompatible with the `default_branch` option of the `Repository` resource.  Using both will result in plans always showing a diff.
 
         ## Example Usage
 
         Basic usage:
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_github as github
 
         example = github.Repository("example",
             name="example",
             description="My awesome codebase",
@@ -232,33 +227,30 @@
         development = github.Branch("development",
             repository=example.name,
             branch="development")
         default = github.BranchDefault("default",
             repository=example.name,
             branch=development.branch)
         ```
-        <!--End PulumiCodeChooser -->
 
         Renaming to a branch that doesn't exist:
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_github as github
 
         example = github.Repository("example",
             name="example",
             description="My awesome codebase",
             auto_init=True)
         default = github.BranchDefault("default",
             repository=example.name,
             branch="development",
             rename=True)
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         GitHub Branch Defaults can be imported using an ID made up of `repository`, e.g.
 
         ```sh
         $ pulumi import github:index/branchDefault:BranchDefault branch_default my-repo
```

### Comparing `pulumi_github-6.3.0a1713561029/pulumi_github/branch_protection.py` & `pulumi_github-6.3.0a1713897837/pulumi_github/branch_protection.py`

 * *Files 1% similar despite different names*

```diff
@@ -461,15 +461,14 @@
                  required_pull_request_reviews: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['BranchProtectionRequiredPullRequestReviewArgs']]]]] = None,
                  required_status_checks: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['BranchProtectionRequiredStatusCheckArgs']]]]] = None,
                  restrict_pushes: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['BranchProtectionRestrictPushArgs']]]]] = None,
                  __props__=None):
         """
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_github as github
 
         example_repository = github.Repository("example", name="test")
         example = github.get_user(username="example")
         example_team = github.Team("example", name="Example Name")
@@ -508,15 +507,14 @@
                 "exampleorganization/exampleteam",
             ])
         example_team_repository = github.TeamRepository("example",
             team_id=example_team.id,
             repository=example_repository.name,
             permission="pull")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         GitHub Branch Protection can be imported using an ID made up of `repository:pattern`, e.g.
 
         ```sh
         $ pulumi import github:index/branchProtection:BranchProtection terraform terraform:main
@@ -543,15 +541,14 @@
     def __init__(__self__,
                  resource_name: str,
                  args: BranchProtectionArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_github as github
 
         example_repository = github.Repository("example", name="test")
         example = github.get_user(username="example")
         example_team = github.Team("example", name="Example Name")
@@ -590,15 +587,14 @@
                 "exampleorganization/exampleteam",
             ])
         example_team_repository = github.TeamRepository("example",
             team_id=example_team.id,
             repository=example_repository.name,
             permission="pull")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         GitHub Branch Protection can be imported using an ID made up of `repository:pattern`, e.g.
 
         ```sh
         $ pulumi import github:index/branchProtection:BranchProtection terraform terraform:main
```

### Comparing `pulumi_github-6.3.0a1713561029/pulumi_github/branch_protection_v3.py` & `pulumi_github-6.3.0a1713897837/pulumi_github/branch_protection_v3.py`

 * *Files 1% similar despite different names*

```diff
@@ -314,28 +314,26 @@
 
         The `BranchProtection` resource has moved to the GraphQL API, while this resource will continue to leverage the REST API.
 
         This resource allows you to configure branch protection for repositories in your organization. When applied, the branch will be protected from forced pushes and deletion. Additional constraints, such as required status checks or restrictions on users, teams, and apps, can also be configured.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_github as github
 
         # Protect the main branch of the foo repository. Only allow a specific user to merge to the branch.
         example = github.BranchProtectionV3("example",
             repository=example_github_repository["name"],
             branch="main",
             restrictions=github.BranchProtectionV3RestrictionsArgs(
                 users=["foo-user"],
             ))
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         GitHub Branch Protection can be imported using an ID made up of `repository:branch`, e.g.
 
         ```sh
         $ pulumi import github:index/branchProtectionV3:BranchProtectionV3 terraform terraform:main
@@ -363,28 +361,26 @@
 
         The `BranchProtection` resource has moved to the GraphQL API, while this resource will continue to leverage the REST API.
 
         This resource allows you to configure branch protection for repositories in your organization. When applied, the branch will be protected from forced pushes and deletion. Additional constraints, such as required status checks or restrictions on users, teams, and apps, can also be configured.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_github as github
 
         # Protect the main branch of the foo repository. Only allow a specific user to merge to the branch.
         example = github.BranchProtectionV3("example",
             repository=example_github_repository["name"],
             branch="main",
             restrictions=github.BranchProtectionV3RestrictionsArgs(
                 users=["foo-user"],
             ))
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         GitHub Branch Protection can be imported using an ID made up of `repository:branch`, e.g.
 
         ```sh
         $ pulumi import github:index/branchProtectionV3:BranchProtectionV3 terraform terraform:main
```

### Comparing `pulumi_github-6.3.0a1713561029/pulumi_github/codespaces_organization_secret.py` & `pulumi_github-6.3.0a1713897837/pulumi_github/codespaces_organization_secret.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-6.3.0a1713561029/pulumi_github/codespaces_organization_secret_repositories.py` & `pulumi_github-6.3.0a1713897837/pulumi_github/codespaces_organization_secret_repositories.py`

 * *Files 5% similar despite different names*

```diff
@@ -102,25 +102,23 @@
 
         You must have write access to an organization secret to use this resource.
 
         This resource is only applicable when `visibility` of the existing organization secret has been set to `selected`.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_github as github
 
         repo = github.get_repository(full_name="my-org/repo")
         org_secret_repos = github.CodespacesOrganizationSecretRepositories("org_secret_repos",
             secret_name="existing_secret_name",
             selected_repository_ids=[repo.repo_id])
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         This resource can be imported using an ID made up of the secret name:
 
         ```sh
         $ pulumi import github:index/codespacesOrganizationSecretRepositories:CodespacesOrganizationSecretRepositories org_secret_repos existing_secret_name
@@ -142,25 +140,23 @@
 
         You must have write access to an organization secret to use this resource.
 
         This resource is only applicable when `visibility` of the existing organization secret has been set to `selected`.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_github as github
 
         repo = github.get_repository(full_name="my-org/repo")
         org_secret_repos = github.CodespacesOrganizationSecretRepositories("org_secret_repos",
             secret_name="existing_secret_name",
             selected_repository_ids=[repo.repo_id])
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         This resource can be imported using an ID made up of the secret name:
 
         ```sh
         $ pulumi import github:index/codespacesOrganizationSecretRepositories:CodespacesOrganizationSecretRepositories org_secret_repos existing_secret_name
```

### Comparing `pulumi_github-6.3.0a1713561029/pulumi_github/codespaces_secret.py` & `pulumi_github-6.3.0a1713897837/pulumi_github/codespaces_secret.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-6.3.0a1713561029/pulumi_github/codespaces_user_secret.py` & `pulumi_github-6.3.0a1713897837/pulumi_github/codespaces_user_secret.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-6.3.0a1713561029/pulumi_github/config/__init__.pyi` & `pulumi_github-6.3.0a1713897837/pulumi_github/config/__init__.pyi`

 * *Files identical despite different names*

### Comparing `pulumi_github-6.3.0a1713561029/pulumi_github/config/outputs.py` & `pulumi_github-6.3.0a1713897837/pulumi_github/config/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-6.3.0a1713561029/pulumi_github/config/vars.py` & `pulumi_github-6.3.0a1713897837/pulumi_github/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-6.3.0a1713561029/pulumi_github/dependabot_organization_secret.py` & `pulumi_github-6.3.0a1713897837/pulumi_github/dependabot_organization_secret.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-6.3.0a1713561029/pulumi_github/dependabot_organization_secret_repositories.py` & `pulumi_github-6.3.0a1713897837/pulumi_github/dependabot_organization_secret_repositories.py`

 * *Files 2% similar despite different names*

```diff
@@ -101,29 +101,27 @@
         This resource allows you to manage the repository allow list for existing GitHub Dependabot secrets within your GitHub organization.
         You must have write access to an organization secret to use this resource.
 
         This resource is only applicable when `visibility` of the existing organization secret has been set to `selected`.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_github as github
 
         repo = github.get_repository(full_name="my-org/repo")
         example_secret = github.DependabotOrganizationSecret("example_secret",
             secret_name="example_secret_name",
             visibility="private",
             plaintext_value=some_secret_string)
         org_secret_repos = github.DependabotOrganizationSecretRepositories("org_secret_repos",
             secret_name=example_secret.secret_name,
             selected_repository_ids=[repo.repo_id])
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         This resource can be imported using an ID made up of the secret name:
 
         ```sh
         $ pulumi import github:index/dependabotOrganizationSecretRepositories:DependabotOrganizationSecretRepositories test_secret_repos test_secret_name
@@ -144,29 +142,27 @@
         This resource allows you to manage the repository allow list for existing GitHub Dependabot secrets within your GitHub organization.
         You must have write access to an organization secret to use this resource.
 
         This resource is only applicable when `visibility` of the existing organization secret has been set to `selected`.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_github as github
 
         repo = github.get_repository(full_name="my-org/repo")
         example_secret = github.DependabotOrganizationSecret("example_secret",
             secret_name="example_secret_name",
             visibility="private",
             plaintext_value=some_secret_string)
         org_secret_repos = github.DependabotOrganizationSecretRepositories("org_secret_repos",
             secret_name=example_secret.secret_name,
             selected_repository_ids=[repo.repo_id])
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         This resource can be imported using an ID made up of the secret name:
 
         ```sh
         $ pulumi import github:index/dependabotOrganizationSecretRepositories:DependabotOrganizationSecretRepositories test_secret_repos test_secret_name
```

### Comparing `pulumi_github-6.3.0a1713561029/pulumi_github/dependabot_secret.py` & `pulumi_github-6.3.0a1713897837/pulumi_github/dependabot_secret.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-6.3.0a1713561029/pulumi_github/emu_group_mapping.py` & `pulumi_github-6.3.0a1713897837/pulumi_github/emu_group_mapping.py`

 * *Files 5% similar despite different names*

```diff
@@ -110,24 +110,22 @@
                  team_slug: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         This resource manages mappings between external groups for enterprise managed users and GitHub teams. It wraps the API detailed [here](https://docs.github.com/en/rest/reference/teams#external-groups). Note that this is a distinct resource from `TeamSyncGroupMapping`. `EmuGroupMapping` is special to the Enterprise Managed User (EMU) external group feature, whereas `TeamSyncGroupMapping` is specific to Identity Provider Groups.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_github as github
 
         example_emu_group_mapping = github.EmuGroupMapping("example_emu_group_mapping",
             team_slug="emu-test-team",
             group_id=28836)
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         GitHub EMU External Group Mappings can be imported using the external `group_id`, e.g.
 
         ```sh
         $ pulumi import github:index/emuGroupMapping:EmuGroupMapping example_emu_group_mapping 28836
@@ -145,24 +143,22 @@
                  args: EmuGroupMappingArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         This resource manages mappings between external groups for enterprise managed users and GitHub teams. It wraps the API detailed [here](https://docs.github.com/en/rest/reference/teams#external-groups). Note that this is a distinct resource from `TeamSyncGroupMapping`. `EmuGroupMapping` is special to the Enterprise Managed User (EMU) external group feature, whereas `TeamSyncGroupMapping` is specific to Identity Provider Groups.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_github as github
 
         example_emu_group_mapping = github.EmuGroupMapping("example_emu_group_mapping",
             team_slug="emu-test-team",
             group_id=28836)
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         GitHub EMU External Group Mappings can be imported using the external `group_id`, e.g.
 
         ```sh
         $ pulumi import github:index/emuGroupMapping:EmuGroupMapping example_emu_group_mapping 28836
```

### Comparing `pulumi_github-6.3.0a1713561029/pulumi_github/enterprise_actions_permissions.py` & `pulumi_github-6.3.0a1713897837/pulumi_github/enterprise_actions_permissions.py`

 * *Files 2% similar despite different names*

```diff
@@ -200,15 +200,14 @@
                  __props__=None):
         """
         This resource allows you to create and manage GitHub Actions permissions within your GitHub enterprise.
         You must have admin access to an enterprise to use this resource.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_github as github
 
         example_enterprise = github.get_enterprise(slug="my-enterprise")
         example_org = github.get_organization(name="my-org")
         test = github.EnterpriseActionsPermissions("test",
@@ -223,15 +222,14 @@
                 ],
                 verified_allowed=True,
             ),
             enabled_organizations_config=github.EnterpriseActionsPermissionsEnabledOrganizationsConfigArgs(
                 organization_ids=[example_org.id],
             ))
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         This resource can be imported using the name of the GitHub enterprise:
 
         ```sh
         $ pulumi import github:index/enterpriseActionsPermissions:EnterpriseActionsPermissions test github_enterprise_name
@@ -253,15 +251,14 @@
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         This resource allows you to create and manage GitHub Actions permissions within your GitHub enterprise.
         You must have admin access to an enterprise to use this resource.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_github as github
 
         example_enterprise = github.get_enterprise(slug="my-enterprise")
         example_org = github.get_organization(name="my-org")
         test = github.EnterpriseActionsPermissions("test",
@@ -276,15 +273,14 @@
                 ],
                 verified_allowed=True,
             ),
             enabled_organizations_config=github.EnterpriseActionsPermissionsEnabledOrganizationsConfigArgs(
                 organization_ids=[example_org.id],
             ))
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         This resource can be imported using the name of the GitHub enterprise:
 
         ```sh
         $ pulumi import github:index/enterpriseActionsPermissions:EnterpriseActionsPermissions test github_enterprise_name
```

### Comparing `pulumi_github-6.3.0a1713561029/pulumi_github/enterprise_actions_runner_group.py` & `pulumi_github-6.3.0a1713897837/pulumi_github/enterprise_actions_runner_group.py`

 * *Files 0% similar despite different names*

```diff
@@ -328,15 +328,14 @@
                  __props__=None):
         """
         This resource allows you to create and manage GitHub Actions runner groups within your GitHub enterprise.
         You must have admin access to an enterprise to use this resource.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_github as github
 
         enterprise = github.get_enterprise(slug="my-enterprise")
         enterprise_organization = github.EnterpriseOrganization("enterprise_organization",
             enterprise_id=enterprise.id,
@@ -348,15 +347,14 @@
             enterprise_slug=enterprise.slug,
             allows_public_repositories=True,
             visibility="selected",
             selected_organization_ids=[enterprise_organization.database_id],
             restricted_to_workflows=True,
             selected_workflows=["my-organization/my-repo/.github/workflows/cool-workflow.yaml@refs/tags/v1"])
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         This resource can be imported using the enterprise slug and the ID of the runner group:
 
         ```sh
         $ pulumi import github:index/enterpriseActionsRunnerGroup:EnterpriseActionsRunnerGroup test enterprise-slug/42
@@ -380,15 +378,14 @@
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         This resource allows you to create and manage GitHub Actions runner groups within your GitHub enterprise.
         You must have admin access to an enterprise to use this resource.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_github as github
 
         enterprise = github.get_enterprise(slug="my-enterprise")
         enterprise_organization = github.EnterpriseOrganization("enterprise_organization",
             enterprise_id=enterprise.id,
@@ -400,15 +397,14 @@
             enterprise_slug=enterprise.slug,
             allows_public_repositories=True,
             visibility="selected",
             selected_organization_ids=[enterprise_organization.database_id],
             restricted_to_workflows=True,
             selected_workflows=["my-organization/my-repo/.github/workflows/cool-workflow.yaml@refs/tags/v1"])
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         This resource can be imported using the enterprise slug and the ID of the runner group:
 
         ```sh
         $ pulumi import github:index/enterpriseActionsRunnerGroup:EnterpriseActionsRunnerGroup test enterprise-slug/42
```

### Comparing `pulumi_github-6.3.0a1713561029/pulumi_github/enterprise_organization.py` & `pulumi_github-6.3.0a1713897837/pulumi_github/enterprise_organization.py`

 * *Files 1% similar despite different names*

```diff
@@ -245,28 +245,26 @@
                  name: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         This resource allows you to create and manage a GitHub enterprise organization.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_github as github
 
         org = github.EnterpriseOrganization("org",
             enterprise_id=enterprise["id"],
             name="some-awesome-org",
             display_name="Some Awesome Org",
             description="Organization created with terraform",
             billing_email="jon@winteriscoming.com",
             admin_logins=["jon-snow"])
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         GitHub Enterprise Organization can be imported using the `slug` of the enterprise, combined with the `orgname` of the organization, separated by a `/` character.
 
         ```sh
         $ pulumi import github:index/enterpriseOrganization:EnterpriseOrganization org enterp/some-awesome-org
@@ -288,28 +286,26 @@
                  args: EnterpriseOrganizationArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         This resource allows you to create and manage a GitHub enterprise organization.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_github as github
 
         org = github.EnterpriseOrganization("org",
             enterprise_id=enterprise["id"],
             name="some-awesome-org",
             display_name="Some Awesome Org",
             description="Organization created with terraform",
             billing_email="jon@winteriscoming.com",
             admin_logins=["jon-snow"])
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         GitHub Enterprise Organization can be imported using the `slug` of the enterprise, combined with the `orgname` of the organization, separated by a `/` character.
 
         ```sh
         $ pulumi import github:index/enterpriseOrganization:EnterpriseOrganization org enterp/some-awesome-org
```

### Comparing `pulumi_github-6.3.0a1713561029/pulumi_github/get_actions_environment_secrets.py` & `pulumi_github-6.3.0a1713897837/pulumi_github/get_actions_environment_secrets.py`

 * *Files 2% similar despite different names*

```diff
@@ -92,23 +92,21 @@
                                     name: Optional[str] = None,
                                     opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetActionsEnvironmentSecretsResult:
     """
     Use this data source to retrieve the list of secrets of the repository environment.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_github as github
 
     example = github.get_actions_environment_secrets(name="exampleRepo",
         environment="exampleEnvironment")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str name: Name of the secret
     """
     __args__ = dict()
     __args__['environment'] = environment
     __args__['fullName'] = full_name
@@ -130,21 +128,19 @@
                                            name: Optional[pulumi.Input[Optional[str]]] = None,
                                            opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetActionsEnvironmentSecretsResult]:
     """
     Use this data source to retrieve the list of secrets of the repository environment.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_github as github
 
     example = github.get_actions_environment_secrets(name="exampleRepo",
         environment="exampleEnvironment")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str name: Name of the secret
     """
     ...
```

### Comparing `pulumi_github-6.3.0a1713561029/pulumi_github/get_actions_environment_variables.py` & `pulumi_github-6.3.0a1713897837/pulumi_github/get_actions_environment_variables.py`

 * *Files 6% similar despite different names*

```diff
@@ -92,23 +92,21 @@
                                       name: Optional[str] = None,
                                       opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetActionsEnvironmentVariablesResult:
     """
     Use this data source to retrieve the list of variables of the repository environment.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_github as github
 
     example = github.get_actions_environment_variables(name="exampleRepo",
         environment="exampleEnvironment")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str name: Name of the variable
     """
     __args__ = dict()
     __args__['environment'] = environment
     __args__['fullName'] = full_name
@@ -130,21 +128,19 @@
                                              name: Optional[pulumi.Input[Optional[str]]] = None,
                                              opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetActionsEnvironmentVariablesResult]:
     """
     Use this data source to retrieve the list of variables of the repository environment.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_github as github
 
     example = github.get_actions_environment_variables(name="exampleRepo",
         environment="exampleEnvironment")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str name: Name of the variable
     """
     ...
```

### Comparing `pulumi_github-6.3.0a1713561029/pulumi_github/get_actions_organization_oidc_subject_claim_customization_template.py` & `pulumi_github-6.3.0a1713897837/pulumi_github/get_actions_organization_oidc_subject_claim_customization_template.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,22 +58,20 @@
 
 def get_actions_organization_oidc_subject_claim_customization_template(opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetActionsOrganizationOidcSubjectClaimCustomizationTemplateResult:
     """
     Use this data source to retrieve the OpenID Connect subject claim customization template for an organization
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_github as github
 
     example = github.get_actions_organization_oidc_subject_claim_customization_template()
     ```
-    <!--End PulumiCodeChooser -->
     """
     __args__ = dict()
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('github:index/getActionsOrganizationOidcSubjectClaimCustomizationTemplate:getActionsOrganizationOidcSubjectClaimCustomizationTemplate', __args__, opts=opts, typ=GetActionsOrganizationOidcSubjectClaimCustomizationTemplateResult).value
 
     return AwaitableGetActionsOrganizationOidcSubjectClaimCustomizationTemplateResult(
         id=pulumi.get(__ret__, 'id'),
@@ -83,17 +81,15 @@
 @_utilities.lift_output_func(get_actions_organization_oidc_subject_claim_customization_template)
 def get_actions_organization_oidc_subject_claim_customization_template_output(opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetActionsOrganizationOidcSubjectClaimCustomizationTemplateResult]:
     """
     Use this data source to retrieve the OpenID Connect subject claim customization template for an organization
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_github as github
 
     example = github.get_actions_organization_oidc_subject_claim_customization_template()
     ```
-    <!--End PulumiCodeChooser -->
     """
     ...
```

### Comparing `pulumi_github-6.3.0a1713561029/pulumi_github/get_actions_organization_public_key.py` & `pulumi_github-6.3.0a1713897837/pulumi_github/get_actions_organization_public_key.py`

 * *Files 3% similar despite different names*

```diff
@@ -71,22 +71,20 @@
 def get_actions_organization_public_key(opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetActionsOrganizationPublicKeyResult:
     """
     Use this data source to retrieve information about a GitHub Actions Organization public key. This data source is required to be used with other GitHub secrets interactions.
     Note that the provider `token` must have admin rights to an organization to retrieve it's action public key.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_github as github
 
     example = github.get_actions_organization_public_key()
     ```
-    <!--End PulumiCodeChooser -->
     """
     __args__ = dict()
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('github:index/getActionsOrganizationPublicKey:getActionsOrganizationPublicKey', __args__, opts=opts, typ=GetActionsOrganizationPublicKeyResult).value
 
     return AwaitableGetActionsOrganizationPublicKeyResult(
         id=pulumi.get(__ret__, 'id'),
@@ -98,17 +96,15 @@
 def get_actions_organization_public_key_output(opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetActionsOrganizationPublicKeyResult]:
     """
     Use this data source to retrieve information about a GitHub Actions Organization public key. This data source is required to be used with other GitHub secrets interactions.
     Note that the provider `token` must have admin rights to an organization to retrieve it's action public key.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_github as github
 
     example = github.get_actions_organization_public_key()
     ```
-    <!--End PulumiCodeChooser -->
     """
     ...
```

### Comparing `pulumi_github-6.3.0a1713561029/pulumi_github/get_actions_organization_registration_token.py` & `pulumi_github-6.3.0a1713897837/pulumi_github/get_actions_organization_registration_token.py`

 * *Files 3% similar despite different names*

```diff
@@ -70,22 +70,20 @@
 
 def get_actions_organization_registration_token(opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetActionsOrganizationRegistrationTokenResult:
     """
     Use this data source to retrieve a GitHub Actions organization registration token. This token can then be used to register a self-hosted runner.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_github as github
 
     example = github.get_actions_organization_registration_token()
     ```
-    <!--End PulumiCodeChooser -->
     """
     __args__ = dict()
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('github:index/getActionsOrganizationRegistrationToken:getActionsOrganizationRegistrationToken', __args__, opts=opts, typ=GetActionsOrganizationRegistrationTokenResult).value
 
     return AwaitableGetActionsOrganizationRegistrationTokenResult(
         expires_at=pulumi.get(__ret__, 'expires_at'),
@@ -96,17 +94,15 @@
 @_utilities.lift_output_func(get_actions_organization_registration_token)
 def get_actions_organization_registration_token_output(opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetActionsOrganizationRegistrationTokenResult]:
     """
     Use this data source to retrieve a GitHub Actions organization registration token. This token can then be used to register a self-hosted runner.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_github as github
 
     example = github.get_actions_organization_registration_token()
     ```
-    <!--End PulumiCodeChooser -->
     """
     ...
```

### Comparing `pulumi_github-6.3.0a1713561029/pulumi_github/get_actions_organization_secrets.py` & `pulumi_github-6.3.0a1713897837/pulumi_github/get_actions_organization_secrets.py`

 * *Files 12% similar despite different names*

```diff
@@ -59,22 +59,20 @@
 
 def get_actions_organization_secrets(opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetActionsOrganizationSecretsResult:
     """
     Use this data source to retrieve the list of secrets of the organization.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_github as github
 
     example = github.get_actions_organization_secrets()
     ```
-    <!--End PulumiCodeChooser -->
     """
     __args__ = dict()
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('github:index/getActionsOrganizationSecrets:getActionsOrganizationSecrets', __args__, opts=opts, typ=GetActionsOrganizationSecretsResult).value
 
     return AwaitableGetActionsOrganizationSecretsResult(
         id=pulumi.get(__ret__, 'id'),
@@ -84,17 +82,15 @@
 @_utilities.lift_output_func(get_actions_organization_secrets)
 def get_actions_organization_secrets_output(opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetActionsOrganizationSecretsResult]:
     """
     Use this data source to retrieve the list of secrets of the organization.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_github as github
 
     example = github.get_actions_organization_secrets()
     ```
-    <!--End PulumiCodeChooser -->
     """
     ...
```

### Comparing `pulumi_github-6.3.0a1713561029/pulumi_github/get_actions_organization_variables.py` & `pulumi_github-6.3.0a1713897837/pulumi_github/get_actions_organization_variables.py`

 * *Files 10% similar despite different names*

```diff
@@ -59,22 +59,20 @@
 
 def get_actions_organization_variables(opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetActionsOrganizationVariablesResult:
     """
     Use this data source to retrieve the list of variables of the organization.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_github as github
 
     example = github.get_actions_organization_variables()
     ```
-    <!--End PulumiCodeChooser -->
     """
     __args__ = dict()
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('github:index/getActionsOrganizationVariables:getActionsOrganizationVariables', __args__, opts=opts, typ=GetActionsOrganizationVariablesResult).value
 
     return AwaitableGetActionsOrganizationVariablesResult(
         id=pulumi.get(__ret__, 'id'),
@@ -84,17 +82,15 @@
 @_utilities.lift_output_func(get_actions_organization_variables)
 def get_actions_organization_variables_output(opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetActionsOrganizationVariablesResult]:
     """
     Use this data source to retrieve the list of variables of the organization.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_github as github
 
     example = github.get_actions_organization_variables()
     ```
-    <!--End PulumiCodeChooser -->
     """
     ...
```

### Comparing `pulumi_github-6.3.0a1713561029/pulumi_github/get_actions_public_key.py` & `pulumi_github-6.3.0a1713897837/pulumi_github/get_actions_public_key.py`

 * *Files 4% similar despite different names*

```diff
@@ -81,22 +81,20 @@
                            opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetActionsPublicKeyResult:
     """
     Use this data source to retrieve information about a GitHub Actions public key. This data source is required to be used with other GitHub secrets interactions.
     Note that the provider `token` must have admin rights to a repository to retrieve it's action public key.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_github as github
 
     example = github.get_actions_public_key(repository="example_repo")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str repository: Name of the repository to get public key from.
     """
     __args__ = dict()
     __args__['repository'] = repository
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
@@ -114,20 +112,18 @@
                                   opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetActionsPublicKeyResult]:
     """
     Use this data source to retrieve information about a GitHub Actions public key. This data source is required to be used with other GitHub secrets interactions.
     Note that the provider `token` must have admin rights to a repository to retrieve it's action public key.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_github as github
 
     example = github.get_actions_public_key(repository="example_repo")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str repository: Name of the repository to get public key from.
     """
     ...
```

### Comparing `pulumi_github-6.3.0a1713561029/pulumi_github/get_actions_registration_token.py` & `pulumi_github-6.3.0a1713897837/pulumi_github/get_actions_registration_token.py`

 * *Files 8% similar despite different names*

```diff
@@ -80,22 +80,20 @@
 def get_actions_registration_token(repository: Optional[str] = None,
                                    opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetActionsRegistrationTokenResult:
     """
     Use this data source to retrieve a GitHub Actions repository registration token. This token can then be used to register a self-hosted runner.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_github as github
 
     example = github.get_actions_registration_token(repository="example_repo")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str repository: Name of the repository to get a GitHub Actions registration token for.
     """
     __args__ = dict()
     __args__['repository'] = repository
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
@@ -112,20 +110,18 @@
 def get_actions_registration_token_output(repository: Optional[pulumi.Input[str]] = None,
                                           opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetActionsRegistrationTokenResult]:
     """
     Use this data source to retrieve a GitHub Actions repository registration token. This token can then be used to register a self-hosted runner.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_github as github
 
     example = github.get_actions_registration_token(repository="example_repo")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str repository: Name of the repository to get a GitHub Actions registration token for.
     """
     ...
```

### Comparing `pulumi_github-6.3.0a1713561029/pulumi_github/get_actions_repository_oidc_subject_claim_customization_template.py` & `pulumi_github-6.3.0a1713897837/pulumi_github/get_actions_repository_oidc_subject_claim_customization_template.py`

 * *Files 5% similar despite different names*

```diff
@@ -80,22 +80,20 @@
 def get_actions_repository_oidc_subject_claim_customization_template(name: Optional[str] = None,
                                                                      opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetActionsRepositoryOidcSubjectClaimCustomizationTemplateResult:
     """
     Use this data source to retrieve the OpenID Connect subject claim customization template for a repository
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_github as github
 
     example = github.get_actions_repository_oidc_subject_claim_customization_template(name="example_repository")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str name: Name of the repository to get the OpenID Connect subject claim customization template for.
     """
     __args__ = dict()
     __args__['name'] = name
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
@@ -112,20 +110,18 @@
 def get_actions_repository_oidc_subject_claim_customization_template_output(name: Optional[pulumi.Input[str]] = None,
                                                                             opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetActionsRepositoryOidcSubjectClaimCustomizationTemplateResult]:
     """
     Use this data source to retrieve the OpenID Connect subject claim customization template for a repository
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_github as github
 
     example = github.get_actions_repository_oidc_subject_claim_customization_template(name="example_repository")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str name: Name of the repository to get the OpenID Connect subject claim customization template for.
     """
     ...
```

### Comparing `pulumi_github-6.3.0a1713561029/pulumi_github/get_actions_secrets.py` & `pulumi_github-6.3.0a1713897837/pulumi_github/get_actions_secrets.py`

 * *Files 4% similar despite different names*

```diff
@@ -82,22 +82,20 @@
                         name: Optional[str] = None,
                         opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetActionsSecretsResult:
     """
     Use this data source to retrieve the list of secrets for a GitHub repository.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_github as github
 
     example = github.get_actions_secrets(name="example")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str full_name: Full name of the repository (in `org/name` format).
     :param str name: The name of the repository.
     """
     __args__ = dict()
     __args__['fullName'] = full_name
@@ -117,21 +115,19 @@
                                name: Optional[pulumi.Input[Optional[str]]] = None,
                                opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetActionsSecretsResult]:
     """
     Use this data source to retrieve the list of secrets for a GitHub repository.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_github as github
 
     example = github.get_actions_secrets(name="example")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str full_name: Full name of the repository (in `org/name` format).
     :param str name: The name of the repository.
     """
     ...
```

### Comparing `pulumi_github-6.3.0a1713561029/pulumi_github/get_actions_variables.py` & `pulumi_github-6.3.0a1713897837/pulumi_github/get_actions_variables.py`

 * *Files 4% similar despite different names*

```diff
@@ -82,22 +82,20 @@
                           name: Optional[str] = None,
                           opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetActionsVariablesResult:
     """
     Use this data source to retrieve the list of variables for a GitHub repository.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_github as github
 
     example = github.get_actions_variables(name="example")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str full_name: Full name of the repository (in `org/name` format).
     :param str name: The name of the repository.
     """
     __args__ = dict()
     __args__['fullName'] = full_name
@@ -117,21 +115,19 @@
                                  name: Optional[pulumi.Input[Optional[str]]] = None,
                                  opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetActionsVariablesResult]:
     """
     Use this data source to retrieve the list of variables for a GitHub repository.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_github as github
 
     example = github.get_actions_variables(name="example")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str full_name: Full name of the repository (in `org/name` format).
     :param str name: The name of the repository.
     """
     ...
```

### Comparing `pulumi_github-6.3.0a1713561029/pulumi_github/get_app_token.py` & `pulumi_github-6.3.0a1713897837/pulumi_github/get_app_token.py`

 * *Files 2% similar despite different names*

```diff
@@ -88,25 +88,23 @@
                   pem_file: Optional[str] = None,
                   opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetAppTokenResult:
     """
     Use this data source to generate a [GitHub App JWT](https://docs.github.com/en/apps/creating-github-apps/authenticating-with-a-github-app/generating-a-json-web-token-jwt-for-a-github-app).
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_github as github
     import pulumi_std as std
 
     this = github.get_app_token(app_id="123456",
         installation_id="78910",
         pem_file=std.file(input="foo/bar.pem").result)
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str app_id: This is the ID of the GitHub App.
     :param str installation_id: This is the ID of the GitHub App installation.
     :param str pem_file: This is the contents of the GitHub App private key PEM file.
     """
     __args__ = dict()
@@ -130,25 +128,23 @@
                          pem_file: Optional[pulumi.Input[str]] = None,
                          opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetAppTokenResult]:
     """
     Use this data source to generate a [GitHub App JWT](https://docs.github.com/en/apps/creating-github-apps/authenticating-with-a-github-app/generating-a-json-web-token-jwt-for-a-github-app).
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_github as github
     import pulumi_std as std
 
     this = github.get_app_token(app_id="123456",
         installation_id="78910",
         pem_file=std.file(input="foo/bar.pem").result)
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str app_id: This is the ID of the GitHub App.
     :param str installation_id: This is the ID of the GitHub App installation.
     :param str pem_file: This is the contents of the GitHub App private key PEM file.
     """
     ...
```

### Comparing `pulumi_github-6.3.0a1713561029/pulumi_github/get_branch.py` & `pulumi_github-6.3.0a1713897837/pulumi_github/get_branch.py`

 * *Files 7% similar despite different names*

```diff
@@ -102,23 +102,21 @@
                repository: Optional[str] = None,
                opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetBranchResult:
     """
     Use this data source to retrieve information about a repository branch.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_github as github
 
     development = github.get_branch(repository="example",
         branch="development")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str branch: The repository branch to retrieve.
     :param str repository: The GitHub repository name.
     """
     __args__ = dict()
     __args__['branch'] = branch
@@ -140,22 +138,20 @@
                       repository: Optional[pulumi.Input[str]] = None,
                       opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetBranchResult]:
     """
     Use this data source to retrieve information about a repository branch.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_github as github
 
     development = github.get_branch(repository="example",
         branch="development")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str branch: The repository branch to retrieve.
     :param str repository: The GitHub repository name.
     """
     ...
```

### Comparing `pulumi_github-6.3.0a1713561029/pulumi_github/get_branch_protection_rules.py` & `pulumi_github-6.3.0a1713897837/pulumi_github/get_branch_protection_rules.py`

 * *Files 4% similar despite different names*

```diff
@@ -69,22 +69,20 @@
 def get_branch_protection_rules(repository: Optional[str] = None,
                                 opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetBranchProtectionRulesResult:
     """
     Use this data source to retrieve a list of repository branch protection rules.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_github as github
 
     example = github.get_branch_protection_rules(repository="example")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str repository: The GitHub repository name.
     """
     __args__ = dict()
     __args__['repository'] = repository
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
@@ -100,20 +98,18 @@
 def get_branch_protection_rules_output(repository: Optional[pulumi.Input[str]] = None,
                                        opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetBranchProtectionRulesResult]:
     """
     Use this data source to retrieve a list of repository branch protection rules.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_github as github
 
     example = github.get_branch_protection_rules(repository="example")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str repository: The GitHub repository name.
     """
     ...
```

### Comparing `pulumi_github-6.3.0a1713561029/pulumi_github/get_codespaces_organization_public_key.py` & `pulumi_github-6.3.0a1713897837/pulumi_github/get_codespaces_organization_public_key.py`

 * *Files 12% similar despite different names*

```diff
@@ -71,22 +71,20 @@
 def get_codespaces_organization_public_key(opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetCodespacesOrganizationPublicKeyResult:
     """
     Use this data source to retrieve information about a GitHub Codespaces Organization public key. This data source is required to be used with other GitHub secrets interactions.
     Note that the provider `token` must have admin rights to an organization to retrieve it's Codespaces public key.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_github as github
 
     example = github.get_codespaces_organization_public_key()
     ```
-    <!--End PulumiCodeChooser -->
     """
     __args__ = dict()
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('github:index/getCodespacesOrganizationPublicKey:getCodespacesOrganizationPublicKey', __args__, opts=opts, typ=GetCodespacesOrganizationPublicKeyResult).value
 
     return AwaitableGetCodespacesOrganizationPublicKeyResult(
         id=pulumi.get(__ret__, 'id'),
@@ -98,17 +96,15 @@
 def get_codespaces_organization_public_key_output(opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetCodespacesOrganizationPublicKeyResult]:
     """
     Use this data source to retrieve information about a GitHub Codespaces Organization public key. This data source is required to be used with other GitHub secrets interactions.
     Note that the provider `token` must have admin rights to an organization to retrieve it's Codespaces public key.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_github as github
 
     example = github.get_codespaces_organization_public_key()
     ```
-    <!--End PulumiCodeChooser -->
     """
     ...
```

### Comparing `pulumi_github-6.3.0a1713561029/pulumi_github/get_codespaces_organization_secrets.py` & `pulumi_github-6.3.0a1713897837/pulumi_github/get_codespaces_organization_secrets.py`

 * *Files 16% similar despite different names*

```diff
@@ -59,22 +59,20 @@
 
 def get_codespaces_organization_secrets(opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetCodespacesOrganizationSecretsResult:
     """
     Use this data source to retrieve the list of codespaces secrets of the organization.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_github as github
 
     example = github.get_codespaces_organization_secrets()
     ```
-    <!--End PulumiCodeChooser -->
     """
     __args__ = dict()
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('github:index/getCodespacesOrganizationSecrets:getCodespacesOrganizationSecrets', __args__, opts=opts, typ=GetCodespacesOrganizationSecretsResult).value
 
     return AwaitableGetCodespacesOrganizationSecretsResult(
         id=pulumi.get(__ret__, 'id'),
@@ -84,17 +82,15 @@
 @_utilities.lift_output_func(get_codespaces_organization_secrets)
 def get_codespaces_organization_secrets_output(opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetCodespacesOrganizationSecretsResult]:
     """
     Use this data source to retrieve the list of codespaces secrets of the organization.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_github as github
 
     example = github.get_codespaces_organization_secrets()
     ```
-    <!--End PulumiCodeChooser -->
     """
     ...
```

### Comparing `pulumi_github-6.3.0a1713561029/pulumi_github/get_codespaces_public_key.py` & `pulumi_github-6.3.0a1713897837/pulumi_github/get_codespaces_public_key.py`

 * *Files 3% similar despite different names*

```diff
@@ -81,22 +81,20 @@
                               opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetCodespacesPublicKeyResult:
     """
     Use this data source to retrieve information about a GitHub Codespaces public key. This data source is required to be used with other GitHub secrets interactions.
     Note that the provider `token` must have admin rights to a repository to retrieve it's Codespaces public key.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_github as github
 
     example = github.get_codespaces_public_key(repository="example_repo")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str repository: Name of the repository to get public key from.
     """
     __args__ = dict()
     __args__['repository'] = repository
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
@@ -114,20 +112,18 @@
                                      opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetCodespacesPublicKeyResult]:
     """
     Use this data source to retrieve information about a GitHub Codespaces public key. This data source is required to be used with other GitHub secrets interactions.
     Note that the provider `token` must have admin rights to a repository to retrieve it's Codespaces public key.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_github as github
 
     example = github.get_codespaces_public_key(repository="example_repo")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str repository: Name of the repository to get public key from.
     """
     ...
```

### Comparing `pulumi_github-6.3.0a1713561029/pulumi_github/get_codespaces_secrets.py` & `pulumi_github-6.3.0a1713897837/pulumi_github/get_codespaces_secrets.py`

 * *Files 8% similar despite different names*

```diff
@@ -82,23 +82,21 @@
                            name: Optional[str] = None,
                            opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetCodespacesSecretsResult:
     """
     Use this data source to retrieve the list of codespaces secrets for a GitHub repository.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_github as github
 
     example = github.get_codespaces_secrets(name="example_repository")
     example2 = github.get_codespaces_secrets(full_name="org/example_repository")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str full_name: Full name of the repository (in `org/name` format).
     :param str name: The name of the repository.
     """
     __args__ = dict()
     __args__['fullName'] = full_name
@@ -118,22 +116,20 @@
                                   name: Optional[pulumi.Input[Optional[str]]] = None,
                                   opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetCodespacesSecretsResult]:
     """
     Use this data source to retrieve the list of codespaces secrets for a GitHub repository.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_github as github
 
     example = github.get_codespaces_secrets(name="example_repository")
     example2 = github.get_codespaces_secrets(full_name="org/example_repository")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str full_name: Full name of the repository (in `org/name` format).
     :param str name: The name of the repository.
     """
     ...
```

### Comparing `pulumi_github-6.3.0a1713561029/pulumi_github/get_codespaces_user_public_key.py` & `pulumi_github-6.3.0a1713897837/pulumi_github/get_codespaces_user_public_key.py`

 * *Files 4% similar despite different names*

```diff
@@ -71,22 +71,20 @@
 def get_codespaces_user_public_key(opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetCodespacesUserPublicKeyResult:
     """
     Use this data source to retrieve information about a GitHub Codespaces User public key. This data source is required to be used with other GitHub secrets interactions.
     Note that the provider `token` must have admin rights to an user to retrieve it's Codespaces public key.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_github as github
 
     example = github.get_codespaces_user_public_key()
     ```
-    <!--End PulumiCodeChooser -->
     """
     __args__ = dict()
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('github:index/getCodespacesUserPublicKey:getCodespacesUserPublicKey', __args__, opts=opts, typ=GetCodespacesUserPublicKeyResult).value
 
     return AwaitableGetCodespacesUserPublicKeyResult(
         id=pulumi.get(__ret__, 'id'),
@@ -98,17 +96,15 @@
 def get_codespaces_user_public_key_output(opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetCodespacesUserPublicKeyResult]:
     """
     Use this data source to retrieve information about a GitHub Codespaces User public key. This data source is required to be used with other GitHub secrets interactions.
     Note that the provider `token` must have admin rights to an user to retrieve it's Codespaces public key.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_github as github
 
     example = github.get_codespaces_user_public_key()
     ```
-    <!--End PulumiCodeChooser -->
     """
     ...
```

### Comparing `pulumi_github-6.3.0a1713561029/pulumi_github/get_codespaces_user_secrets.py` & `pulumi_github-6.3.0a1713897837/pulumi_github/get_codespaces_user_secrets.py`

 * *Files 4% similar despite different names*

```diff
@@ -59,22 +59,20 @@
 
 def get_codespaces_user_secrets(opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetCodespacesUserSecretsResult:
     """
     Use this data source to retrieve the list of codespaces secrets of the user.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_github as github
 
     example = github.get_codespaces_user_secrets()
     ```
-    <!--End PulumiCodeChooser -->
     """
     __args__ = dict()
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('github:index/getCodespacesUserSecrets:getCodespacesUserSecrets', __args__, opts=opts, typ=GetCodespacesUserSecretsResult).value
 
     return AwaitableGetCodespacesUserSecretsResult(
         id=pulumi.get(__ret__, 'id'),
@@ -84,17 +82,15 @@
 @_utilities.lift_output_func(get_codespaces_user_secrets)
 def get_codespaces_user_secrets_output(opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetCodespacesUserSecretsResult]:
     """
     Use this data source to retrieve the list of codespaces secrets of the user.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_github as github
 
     example = github.get_codespaces_user_secrets()
     ```
-    <!--End PulumiCodeChooser -->
     """
     ...
```

### Comparing `pulumi_github-6.3.0a1713561029/pulumi_github/get_collaborators.py` & `pulumi_github-6.3.0a1713897837/pulumi_github/get_collaborators.py`

 * *Files 4% similar despite different names*

```diff
@@ -89,23 +89,21 @@
                       repository: Optional[str] = None,
                       opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetCollaboratorsResult:
     """
     Use this data source to retrieve the collaborators for a given repository.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_github as github
 
     test = github.get_collaborators(owner="example_owner",
         repository="example_repository")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str affiliation: Filter collaborators returned by their affiliation. Can be one of: `outside`, `direct`, `all`.  Defaults to `all`.
     :param str owner: The organization that owns the repository.
     :param str repository: The name of the repository.
     """
     __args__ = dict()
@@ -129,23 +127,21 @@
                              repository: Optional[pulumi.Input[str]] = None,
                              opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetCollaboratorsResult]:
     """
     Use this data source to retrieve the collaborators for a given repository.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_github as github
 
     test = github.get_collaborators(owner="example_owner",
         repository="example_repository")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str affiliation: Filter collaborators returned by their affiliation. Can be one of: `outside`, `direct`, `all`.  Defaults to `all`.
     :param str owner: The organization that owns the repository.
     :param str repository: The name of the repository.
     """
     ...
```

### Comparing `pulumi_github-6.3.0a1713561029/pulumi_github/get_dependabot_organization_public_key.py` & `pulumi_github-6.3.0a1713897837/pulumi_github/get_dependabot_organization_public_key.py`

 * *Files 5% similar despite different names*

```diff
@@ -71,22 +71,20 @@
 def get_dependabot_organization_public_key(opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetDependabotOrganizationPublicKeyResult:
     """
     Use this data source to retrieve information about a GitHub Dependabot Organization public key. This data source is required to be used with other GitHub secrets interactions.
     Note that the provider `token` must have admin rights to an organization to retrieve it's Dependabot public key.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_github as github
 
     example = github.get_dependabot_organization_public_key()
     ```
-    <!--End PulumiCodeChooser -->
     """
     __args__ = dict()
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('github:index/getDependabotOrganizationPublicKey:getDependabotOrganizationPublicKey', __args__, opts=opts, typ=GetDependabotOrganizationPublicKeyResult).value
 
     return AwaitableGetDependabotOrganizationPublicKeyResult(
         id=pulumi.get(__ret__, 'id'),
@@ -98,17 +96,15 @@
 def get_dependabot_organization_public_key_output(opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetDependabotOrganizationPublicKeyResult]:
     """
     Use this data source to retrieve information about a GitHub Dependabot Organization public key. This data source is required to be used with other GitHub secrets interactions.
     Note that the provider `token` must have admin rights to an organization to retrieve it's Dependabot public key.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_github as github
 
     example = github.get_dependabot_organization_public_key()
     ```
-    <!--End PulumiCodeChooser -->
     """
     ...
```

### Comparing `pulumi_github-6.3.0a1713561029/pulumi_github/get_dependabot_organization_secrets.py` & `pulumi_github-6.3.0a1713897837/pulumi_github/get_dependabot_organization_secrets.py`

 * *Files 5% similar despite different names*

```diff
@@ -59,22 +59,20 @@
 
 def get_dependabot_organization_secrets(opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetDependabotOrganizationSecretsResult:
     """
     Use this data source to retrieve the list of dependabot secrets of the organization.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_github as github
 
     example = github.get_dependabot_organization_secrets()
     ```
-    <!--End PulumiCodeChooser -->
     """
     __args__ = dict()
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('github:index/getDependabotOrganizationSecrets:getDependabotOrganizationSecrets', __args__, opts=opts, typ=GetDependabotOrganizationSecretsResult).value
 
     return AwaitableGetDependabotOrganizationSecretsResult(
         id=pulumi.get(__ret__, 'id'),
@@ -84,17 +82,15 @@
 @_utilities.lift_output_func(get_dependabot_organization_secrets)
 def get_dependabot_organization_secrets_output(opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetDependabotOrganizationSecretsResult]:
     """
     Use this data source to retrieve the list of dependabot secrets of the organization.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_github as github
 
     example = github.get_dependabot_organization_secrets()
     ```
-    <!--End PulumiCodeChooser -->
     """
     ...
```

### Comparing `pulumi_github-6.3.0a1713561029/pulumi_github/get_dependabot_public_key.py` & `pulumi_github-6.3.0a1713897837/pulumi_github/get_dependabot_public_key.py`

 * *Files 3% similar despite different names*

```diff
@@ -81,22 +81,20 @@
                               opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetDependabotPublicKeyResult:
     """
     Use this data source to retrieve information about a GitHub Dependabot public key. This data source is required to be used with other GitHub secrets interactions.
     Note that the provider `token` must have admin rights to a repository to retrieve it's Dependabot public key.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_github as github
 
     example = github.get_dependabot_public_key(repository="example_repo")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str repository: Name of the repository to get public key from.
     """
     __args__ = dict()
     __args__['repository'] = repository
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
@@ -114,20 +112,18 @@
                                      opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetDependabotPublicKeyResult]:
     """
     Use this data source to retrieve information about a GitHub Dependabot public key. This data source is required to be used with other GitHub secrets interactions.
     Note that the provider `token` must have admin rights to a repository to retrieve it's Dependabot public key.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_github as github
 
     example = github.get_dependabot_public_key(repository="example_repo")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str repository: Name of the repository to get public key from.
     """
     ...
```

### Comparing `pulumi_github-6.3.0a1713561029/pulumi_github/get_dependabot_secrets.py` & `pulumi_github-6.3.0a1713897837/pulumi_github/get_dependabot_secrets.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,22 +82,20 @@
                            name: Optional[str] = None,
                            opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetDependabotSecretsResult:
     """
     Use this data source to retrieve the list of dependabot secrets for a GitHub repository.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_github as github
 
     example = github.get_dependabot_secrets(name="example")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str full_name: Full name of the repository (in `org/name` format).
     :param str name: The name of the repository.
     """
     __args__ = dict()
     __args__['fullName'] = full_name
@@ -117,21 +115,19 @@
                                   name: Optional[pulumi.Input[Optional[str]]] = None,
                                   opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetDependabotSecretsResult]:
     """
     Use this data source to retrieve the list of dependabot secrets for a GitHub repository.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_github as github
 
     example = github.get_dependabot_secrets(name="example")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str full_name: Full name of the repository (in `org/name` format).
     :param str name: The name of the repository.
     """
     ...
```

### Comparing `pulumi_github-6.3.0a1713561029/pulumi_github/get_enterprise.py` & `pulumi_github-6.3.0a1713897837/pulumi_github/get_enterprise.py`

 * *Files 3% similar despite different names*

```diff
@@ -119,22 +119,20 @@
 def get_enterprise(slug: Optional[str] = None,
                    opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetEnterpriseResult:
     """
     Use this data source to retrieve basic information about a GitHub enterprise.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_github as github
 
     example = github.get_enterprise(slug="example-co")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str slug: The URL slug identifying the enterprise.
     """
     __args__ = dict()
     __args__['slug'] = slug
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
@@ -154,20 +152,18 @@
 def get_enterprise_output(slug: Optional[pulumi.Input[str]] = None,
                           opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetEnterpriseResult]:
     """
     Use this data source to retrieve basic information about a GitHub enterprise.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_github as github
 
     example = github.get_enterprise(slug="example-co")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str slug: The URL slug identifying the enterprise.
     """
     ...
```

### Comparing `pulumi_github-6.3.0a1713561029/pulumi_github/get_external_groups.py` & `pulumi_github-6.3.0a1713897837/pulumi_github/get_external_groups.py`

 * *Files 7% similar despite different names*

```diff
@@ -59,24 +59,22 @@
 
 def get_external_groups(opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetExternalGroupsResult:
     """
     Use this data source to retrieve external groups belonging to an organization.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_github as github
 
     example_external_groups = github.get_external_groups()
     local_groups = example_external_groups
     pulumi.export("groups", local_groups)
     ```
-    <!--End PulumiCodeChooser -->
     """
     __args__ = dict()
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('github:index/getExternalGroups:getExternalGroups', __args__, opts=opts, typ=GetExternalGroupsResult).value
 
     return AwaitableGetExternalGroupsResult(
         external_groups=pulumi.get(__ret__, 'external_groups'),
@@ -86,19 +84,17 @@
 @_utilities.lift_output_func(get_external_groups)
 def get_external_groups_output(opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetExternalGroupsResult]:
     """
     Use this data source to retrieve external groups belonging to an organization.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_github as github
 
     example_external_groups = github.get_external_groups()
     local_groups = example_external_groups
     pulumi.export("groups", local_groups)
     ```
-    <!--End PulumiCodeChooser -->
     """
     ...
```

### Comparing `pulumi_github-6.3.0a1713561029/pulumi_github/get_github_app.py` & `pulumi_github-6.3.0a1713897837/pulumi_github/get_github_app.py`

 * *Files 4% similar despite different names*

```diff
@@ -92,22 +92,20 @@
 def get_github_app(slug: Optional[str] = None,
                    opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetGithubAppResult:
     """
     Use this data source to retrieve information about an app.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_github as github
 
     foobar = github.get_github_app(slug="foobar")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str slug: The URL-friendly name of your GitHub App.
     """
     __args__ = dict()
     __args__['slug'] = slug
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
@@ -125,20 +123,18 @@
 def get_github_app_output(slug: Optional[pulumi.Input[str]] = None,
                           opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetGithubAppResult]:
     """
     Use this data source to retrieve information about an app.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_github as github
 
     foobar = github.get_github_app(slug="foobar")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str slug: The URL-friendly name of your GitHub App.
     """
     ...
```

### Comparing `pulumi_github-6.3.0a1713561029/pulumi_github/get_ip_ranges.py` & `pulumi_github-6.3.0a1713897837/pulumi_github/get_ip_ranges.py`

 * *Files 2% similar despite different names*

```diff
@@ -370,22 +370,20 @@
 
 def get_ip_ranges(opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetIpRangesResult:
     """
     Use this data source to retrieve information about GitHub's IP addresses.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_github as github
 
     test = github.get_ip_ranges()
     ```
-    <!--End PulumiCodeChooser -->
     """
     __args__ = dict()
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('github:index/getIpRanges:getIpRanges', __args__, opts=opts, typ=GetIpRangesResult).value
 
     return AwaitableGetIpRangesResult(
         actions=pulumi.get(__ret__, 'actions'),
@@ -421,17 +419,15 @@
 @_utilities.lift_output_func(get_ip_ranges)
 def get_ip_ranges_output(opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetIpRangesResult]:
     """
     Use this data source to retrieve information about GitHub's IP addresses.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_github as github
 
     test = github.get_ip_ranges()
     ```
-    <!--End PulumiCodeChooser -->
     """
     ...
```

### Comparing `pulumi_github-6.3.0a1713561029/pulumi_github/get_issue_labels.py` & `pulumi_github-6.3.0a1713897837/pulumi_github/get_issue_labels.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-6.3.0a1713561029/pulumi_github/get_membership.py` & `pulumi_github-6.3.0a1713897837/pulumi_github/get_membership.py`

 * *Files 6% similar despite different names*

```diff
@@ -108,22 +108,20 @@
     Use this data source to find out if a user is a member of your organization, as well
     as what role they have within it.
     If the user's membership in the organization is pending their acceptance of an invite,
     the role they would have once they accept will be returned.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_github as github
 
     membership_for_some_user = github.get_membership(username="SomeUser")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str organization: The organization to check for the above username.
     :param str username: The username to lookup in the organization.
     """
     __args__ = dict()
     __args__['organization'] = organization
@@ -148,21 +146,19 @@
     Use this data source to find out if a user is a member of your organization, as well
     as what role they have within it.
     If the user's membership in the organization is pending their acceptance of an invite,
     the role they would have once they accept will be returned.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_github as github
 
     membership_for_some_user = github.get_membership(username="SomeUser")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str organization: The organization to check for the above username.
     :param str username: The username to lookup in the organization.
     """
     ...
```

### Comparing `pulumi_github-6.3.0a1713561029/pulumi_github/get_organization.py` & `pulumi_github-6.3.0a1713897837/pulumi_github/get_organization.py`

 * *Files 0% similar despite different names*

```diff
@@ -384,22 +384,20 @@
                      name: Optional[str] = None,
                      opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetOrganizationResult:
     """
     Use this data source to retrieve basic information about a GitHub Organization.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_github as github
 
     example = github.get_organization(name="github")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param bool ignore_archived_repos: Whether or not to include archived repos in the `repositories` list
     :param str name: The organization's public profile name
     """
     __args__ = dict()
     __args__['ignoreArchivedRepos'] = ignore_archived_repos
@@ -444,21 +442,19 @@
                             name: Optional[pulumi.Input[str]] = None,
                             opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetOrganizationResult]:
     """
     Use this data source to retrieve basic information about a GitHub Organization.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_github as github
 
     example = github.get_organization(name="github")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param bool ignore_archived_repos: Whether or not to include archived repos in the `repositories` list
     :param str name: The organization's public profile name
     """
     ...
```

### Comparing `pulumi_github-6.3.0a1713561029/pulumi_github/get_organization_custom_role.py` & `pulumi_github-6.3.0a1713897837/pulumi_github/get_organization_custom_role.py`

 * *Files 4% similar despite different names*

```diff
@@ -94,22 +94,20 @@
     """
     Use this data source to retrieve information about a custom role in a GitHub Organization.
 
     > Note: Custom roles are currently only available in GitHub Enterprise Cloud.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_github as github
 
     example = github.get_organization_custom_role(name="example")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str name: The name of the custom role.
     """
     __args__ = dict()
     __args__['name'] = name
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
@@ -129,20 +127,18 @@
     """
     Use this data source to retrieve information about a custom role in a GitHub Organization.
 
     > Note: Custom roles are currently only available in GitHub Enterprise Cloud.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_github as github
 
     example = github.get_organization_custom_role(name="example")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str name: The name of the custom role.
     """
     ...
```

### Comparing `pulumi_github-6.3.0a1713561029/pulumi_github/get_organization_external_identities.py` & `pulumi_github-6.3.0a1713897837/pulumi_github/get_organization_external_identities.py`

 * *Files 10% similar despite different names*

```diff
@@ -60,22 +60,20 @@
 def get_organization_external_identities(opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetOrganizationExternalIdentitiesResult:
     """
     Use this data source to retrieve each organization member's SAML or SCIM user
     attributes.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_github as github
 
     all = github.get_organization_external_identities()
     ```
-    <!--End PulumiCodeChooser -->
     """
     __args__ = dict()
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('github:index/getOrganizationExternalIdentities:getOrganizationExternalIdentities', __args__, opts=opts, typ=GetOrganizationExternalIdentitiesResult).value
 
     return AwaitableGetOrganizationExternalIdentitiesResult(
         id=pulumi.get(__ret__, 'id'),
@@ -86,17 +84,15 @@
 def get_organization_external_identities_output(opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetOrganizationExternalIdentitiesResult]:
     """
     Use this data source to retrieve each organization member's SAML or SCIM user
     attributes.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_github as github
 
     all = github.get_organization_external_identities()
     ```
-    <!--End PulumiCodeChooser -->
     """
     ...
```

### Comparing `pulumi_github-6.3.0a1713561029/pulumi_github/get_organization_ip_allow_list.py` & `pulumi_github-6.3.0a1713897837/pulumi_github/get_organization_ip_allow_list.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,22 +62,20 @@
     """
     Use this data source to retrieve information about the IP allow list of an organization.
     The allow list for IP addresses will block access to private resources via the web, API,
     and Git from any IP addresses that are not on the allow list.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_github as github
 
     all = github.get_organization_ip_allow_list()
     ```
-    <!--End PulumiCodeChooser -->
     """
     __args__ = dict()
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('github:index/getOrganizationIpAllowList:getOrganizationIpAllowList', __args__, opts=opts, typ=GetOrganizationIpAllowListResult).value
 
     return AwaitableGetOrganizationIpAllowListResult(
         id=pulumi.get(__ret__, 'id'),
@@ -89,17 +87,15 @@
     """
     Use this data source to retrieve information about the IP allow list of an organization.
     The allow list for IP addresses will block access to private resources via the web, API,
     and Git from any IP addresses that are not on the allow list.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_github as github
 
     all = github.get_organization_ip_allow_list()
     ```
-    <!--End PulumiCodeChooser -->
     """
     ...
```

### Comparing `pulumi_github-6.3.0a1713561029/pulumi_github/get_organization_team_sync_groups.py` & `pulumi_github-6.3.0a1713897837/pulumi_github/get_organization_team_sync_groups.py`

 * *Files 8% similar despite different names*

```diff
@@ -59,22 +59,20 @@
 
 def get_organization_team_sync_groups(opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetOrganizationTeamSyncGroupsResult:
     """
     Use this data source to retrieve the identity provider (IdP) groups for an organization.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_github as github
 
     test = github.get_organization_team_sync_groups()
     ```
-    <!--End PulumiCodeChooser -->
     """
     __args__ = dict()
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('github:index/getOrganizationTeamSyncGroups:getOrganizationTeamSyncGroups', __args__, opts=opts, typ=GetOrganizationTeamSyncGroupsResult).value
 
     return AwaitableGetOrganizationTeamSyncGroupsResult(
         groups=pulumi.get(__ret__, 'groups'),
@@ -84,17 +82,15 @@
 @_utilities.lift_output_func(get_organization_team_sync_groups)
 def get_organization_team_sync_groups_output(opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetOrganizationTeamSyncGroupsResult]:
     """
     Use this data source to retrieve the identity provider (IdP) groups for an organization.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_github as github
 
     test = github.get_organization_team_sync_groups()
     ```
-    <!--End PulumiCodeChooser -->
     """
     ...
```

### Comparing `pulumi_github-6.3.0a1713561029/pulumi_github/get_organization_teams.py` & `pulumi_github-6.3.0a1713897837/pulumi_github/get_organization_teams.py`

 * *Files 5% similar despite different names*

```diff
@@ -100,33 +100,29 @@
     """
     Use this data source to retrieve information about all GitHub teams in an organization.
 
     ## Example Usage
 
     To retrieve *all* teams of the organization:
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_github as github
 
     all = github.get_organization_teams()
     ```
-    <!--End PulumiCodeChooser -->
 
     To retrieve only the team's at the root of the organization:
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_github as github
 
     root_teams = github.get_organization_teams(root_teams_only=True)
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param int results_per_page: (Optional) Set the number of results per graphql query. Reducing this number can alleviate timeout errors. Accepts a value between 0 - 100. Defaults to `100`.
     :param bool root_teams_only: (Optional) Only return teams that are at the organization's root, i.e. no nested teams. Defaults to `false`.
     :param bool summary_only: (Optional) Exclude the members and repositories of the team from the returned result. Defaults to `false`.
     """
     __args__ = dict()
@@ -152,33 +148,29 @@
     """
     Use this data source to retrieve information about all GitHub teams in an organization.
 
     ## Example Usage
 
     To retrieve *all* teams of the organization:
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_github as github
 
     all = github.get_organization_teams()
     ```
-    <!--End PulumiCodeChooser -->
 
     To retrieve only the team's at the root of the organization:
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_github as github
 
     root_teams = github.get_organization_teams(root_teams_only=True)
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param int results_per_page: (Optional) Set the number of results per graphql query. Reducing this number can alleviate timeout errors. Accepts a value between 0 - 100. Defaults to `100`.
     :param bool root_teams_only: (Optional) Only return teams that are at the organization's root, i.e. no nested teams. Defaults to `false`.
     :param bool summary_only: (Optional) Exclude the members and repositories of the team from the returned result. Defaults to `false`.
     """
     ...
```

### Comparing `pulumi_github-6.3.0a1713561029/pulumi_github/get_organization_webhooks.py` & `pulumi_github-6.3.0a1713897837/pulumi_github/get_organization_webhooks.py`

 * *Files 17% similar despite different names*

```diff
@@ -62,22 +62,20 @@
     """
     Use this data source to retrieve all webhooks of the organization.
 
     ## Example Usage
 
     To retrieve *all* webhooks of the organization:
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_github as github
 
     all = github.get_organization_webhooks()
     ```
-    <!--End PulumiCodeChooser -->
     """
     __args__ = dict()
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('github:index/getOrganizationWebhooks:getOrganizationWebhooks', __args__, opts=opts, typ=GetOrganizationWebhooksResult).value
 
     return AwaitableGetOrganizationWebhooksResult(
         id=pulumi.get(__ret__, 'id'),
@@ -89,17 +87,15 @@
     """
     Use this data source to retrieve all webhooks of the organization.
 
     ## Example Usage
 
     To retrieve *all* webhooks of the organization:
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_github as github
 
     all = github.get_organization_webhooks()
     ```
-    <!--End PulumiCodeChooser -->
     """
     ...
```

### Comparing `pulumi_github-6.3.0a1713561029/pulumi_github/get_ref.py` & `pulumi_github-6.3.0a1713897837/pulumi_github/get_ref.py`

 * *Files 2% similar despite different names*

```diff
@@ -100,24 +100,22 @@
             repository: Optional[str] = None,
             opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetRefResult:
     """
     Use this data source to retrieve information about a repository ref.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_github as github
 
     development = github.get_ref(owner="example",
         repository="example",
         ref="heads/development")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str owner: Owner of the repository.
     :param str ref: The repository ref to look up. Must be formatted `heads/<ref>` for branches, and `tags/<ref>` for tags.
     :param str repository: The GitHub repository name.
     """
     __args__ = dict()
@@ -142,24 +140,22 @@
                    repository: Optional[pulumi.Input[str]] = None,
                    opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetRefResult]:
     """
     Use this data source to retrieve information about a repository ref.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_github as github
 
     development = github.get_ref(owner="example",
         repository="example",
         ref="heads/development")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str owner: Owner of the repository.
     :param str ref: The repository ref to look up. Must be formatted `heads/<ref>` for branches, and `tags/<ref>` for tags.
     :param str repository: The GitHub repository name.
     """
     ...
```

### Comparing `pulumi_github-6.3.0a1713561029/pulumi_github/get_release.py` & `pulumi_github-6.3.0a1713897837/pulumi_github/get_release.py`

 * *Files 1% similar despite different names*

```diff
@@ -288,24 +288,22 @@
     """
     Use this data source to retrieve information about a GitHub release in a specific repository.
 
     ## Example Usage
 
     To retrieve the latest release that is present in a repository:
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_github as github
 
     example = github.get_release(repository="example-repository",
         owner="example-owner",
         retrieve_by="latest")
     ```
-    <!--End PulumiCodeChooser -->
 
     To retrieve a specific release from a repository based on it's ID:
 
 
     :param str owner: Owner of the repository.
     :param int release_id: ID of the release to retrieve. Must be specified when `retrieve_by` = `id`.
     :param str release_tag: Tag of the release to retrieve. Must be specified when `retrieve_by` = `tag`.
@@ -355,24 +353,22 @@
     """
     Use this data source to retrieve information about a GitHub release in a specific repository.
 
     ## Example Usage
 
     To retrieve the latest release that is present in a repository:
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_github as github
 
     example = github.get_release(repository="example-repository",
         owner="example-owner",
         retrieve_by="latest")
     ```
-    <!--End PulumiCodeChooser -->
 
     To retrieve a specific release from a repository based on it's ID:
 
 
     :param str owner: Owner of the repository.
     :param int release_id: ID of the release to retrieve. Must be specified when `retrieve_by` = `id`.
     :param str release_tag: Tag of the release to retrieve. Must be specified when `retrieve_by` = `tag`.
```

### Comparing `pulumi_github-6.3.0a1713561029/pulumi_github/get_repositories.py` & `pulumi_github-6.3.0a1713897837/pulumi_github/get_repositories.py`

 * *Files 14% similar despite different names*

```diff
@@ -119,23 +119,21 @@
     > **Note:** The data source will return a maximum of `1000` repositories
     	[as documented in official API docs](https://developer.github.com/v3/search/#about-the-search-api).
 
     Use this data source to retrieve a list of GitHub repositories using a search query.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_github as github
 
     example = github.get_repositories(query="org:hashicorp language:Go",
         include_repo_id=True)
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param bool include_repo_id: Returns a list of found repository IDs
     :param str query: Search query. See [documentation for the search syntax](https://help.github.com/articles/understanding-the-search-syntax/).
     :param int results_per_page: Set the number of repositories requested per API call. Can be useful to decrease if requests are timing out or to increase to reduce the number of API calls. Defaults to 100.
     :param str sort: Sorts the repositories returned by the specified attribute. Valid values include `stars`, `fork`, and `updated`. Defaults to `updated`.
     """
@@ -168,23 +166,21 @@
     > **Note:** The data source will return a maximum of `1000` repositories
     	[as documented in official API docs](https://developer.github.com/v3/search/#about-the-search-api).
 
     Use this data source to retrieve a list of GitHub repositories using a search query.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_github as github
 
     example = github.get_repositories(query="org:hashicorp language:Go",
         include_repo_id=True)
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param bool include_repo_id: Returns a list of found repository IDs
     :param str query: Search query. See [documentation for the search syntax](https://help.github.com/articles/understanding-the-search-syntax/).
     :param int results_per_page: Set the number of repositories requested per API call. Can be useful to decrease if requests are timing out or to increase to reduce the number of API calls. Defaults to 100.
     :param str sort: Sorts the repositories returned by the specified attribute. Valid values include `stars`, `fork`, and `updated`. Defaults to `updated`.
     """
```

### Comparing `pulumi_github-6.3.0a1713561029/pulumi_github/get_repository.py` & `pulumi_github-6.3.0a1713897837/pulumi_github/get_repository.py`

 * *Files 1% similar despite different names*

```diff
@@ -468,22 +468,20 @@
                    name: Optional[str] = None,
                    opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetRepositoryResult:
     """
     Use this data source to retrieve information about a GitHub repository.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_github as github
 
     example = github.get_repository(full_name="hashicorp/terraform")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str description: A description of the license.
     :param str full_name: Full name of the repository (in `org/name` format).
     :param str homepage_url: URL of a page describing the project.
     :param str name: The name of the repository.
     """
@@ -541,22 +539,20 @@
                           name: Optional[pulumi.Input[Optional[str]]] = None,
                           opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetRepositoryResult]:
     """
     Use this data source to retrieve information about a GitHub repository.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_github as github
 
     example = github.get_repository(full_name="hashicorp/terraform")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str description: A description of the license.
     :param str full_name: Full name of the repository (in `org/name` format).
     :param str homepage_url: URL of a page describing the project.
     :param str name: The name of the repository.
     """
```

### Comparing `pulumi_github-6.3.0a1713561029/pulumi_github/get_repository_autolink_references.py` & `pulumi_github-6.3.0a1713897837/pulumi_github/get_repository_autolink_references.py`

 * *Files 10% similar despite different names*

```diff
@@ -69,22 +69,20 @@
 def get_repository_autolink_references(repository: Optional[str] = None,
                                        opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetRepositoryAutolinkReferencesResult:
     """
     Use this data source to retrieve autolink references for a repository.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_github as github
 
     example = github.get_repository_autolink_references(repository="example-repository")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str repository: Name of the repository to retrieve the autolink references from.
     """
     __args__ = dict()
     __args__['repository'] = repository
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
@@ -100,20 +98,18 @@
 def get_repository_autolink_references_output(repository: Optional[pulumi.Input[str]] = None,
                                               opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetRepositoryAutolinkReferencesResult]:
     """
     Use this data source to retrieve autolink references for a repository.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_github as github
 
     example = github.get_repository_autolink_references(repository="example-repository")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str repository: Name of the repository to retrieve the autolink references from.
     """
     ...
```

### Comparing `pulumi_github-6.3.0a1713561029/pulumi_github/get_repository_branches.py` & `pulumi_github-6.3.0a1713897837/pulumi_github/get_repository_branches.py`

 * *Files 2% similar despite different names*

```diff
@@ -89,22 +89,20 @@
                             repository: Optional[str] = None,
                             opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetRepositoryBranchesResult:
     """
     Use this data source to retrieve information about branches in a repository.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_github as github
 
     example = github.get_repository_branches(repository="example-repository")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param bool only_non_protected_branches: . If true, the `branches` attributes will be populated only with non protected branches. Default: `false`.
     :param bool only_protected_branches: . If true, the `branches` attributes will be populated only with protected branches. Default: `false`.
     :param str repository: Name of the repository to retrieve the branches from.
     """
     __args__ = dict()
@@ -128,22 +126,20 @@
                                    repository: Optional[pulumi.Input[str]] = None,
                                    opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetRepositoryBranchesResult]:
     """
     Use this data source to retrieve information about branches in a repository.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_github as github
 
     example = github.get_repository_branches(repository="example-repository")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param bool only_non_protected_branches: . If true, the `branches` attributes will be populated only with non protected branches. Default: `false`.
     :param bool only_protected_branches: . If true, the `branches` attributes will be populated only with protected branches. Default: `false`.
     :param str repository: Name of the repository to retrieve the branches from.
     """
     ...
```

### Comparing `pulumi_github-6.3.0a1713561029/pulumi_github/get_repository_deploy_keys.py` & `pulumi_github-6.3.0a1713897837/pulumi_github/get_repository_deploy_keys.py`

 * *Files 5% similar despite different names*

```diff
@@ -69,22 +69,20 @@
 def get_repository_deploy_keys(repository: Optional[str] = None,
                                opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetRepositoryDeployKeysResult:
     """
     Use this data source to retrieve all deploy keys of a repository.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_github as github
 
     example = github.get_repository_deploy_keys(repository="example-repository")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str repository: Name of the repository to retrieve the branches from.
     """
     __args__ = dict()
     __args__['repository'] = repository
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
@@ -100,20 +98,18 @@
 def get_repository_deploy_keys_output(repository: Optional[pulumi.Input[str]] = None,
                                       opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetRepositoryDeployKeysResult]:
     """
     Use this data source to retrieve all deploy keys of a repository.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_github as github
 
     example = github.get_repository_deploy_keys(repository="example-repository")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str repository: Name of the repository to retrieve the branches from.
     """
     ...
```

### Comparing `pulumi_github-6.3.0a1713561029/pulumi_github/get_repository_deployment_branch_policies.py` & `pulumi_github-6.3.0a1713897837/pulumi_github/get_repository_deployment_branch_policies.py`

 * *Files 5% similar despite different names*

```diff
@@ -79,23 +79,21 @@
                                               repository: Optional[str] = None,
                                               opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetRepositoryDeploymentBranchPoliciesResult:
     """
     Use this data source to retrieve deployment branch policies for a repository / environment.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_github as github
 
     example = github.get_repository_deployment_branch_policies(repository="example-repository",
         environment_name="env_name")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str environment_name: Name of the environment to retrieve the deployment branch policies  from.
     :param str repository: Name of the repository to retrieve the deployment branch policies from.
     """
     __args__ = dict()
     __args__['environmentName'] = environment_name
@@ -115,22 +113,20 @@
                                                      repository: Optional[pulumi.Input[str]] = None,
                                                      opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetRepositoryDeploymentBranchPoliciesResult]:
     """
     Use this data source to retrieve deployment branch policies for a repository / environment.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_github as github
 
     example = github.get_repository_deployment_branch_policies(repository="example-repository",
         environment_name="env_name")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str environment_name: Name of the environment to retrieve the deployment branch policies  from.
     :param str repository: Name of the repository to retrieve the deployment branch policies from.
     """
     ...
```

### Comparing `pulumi_github-6.3.0a1713561029/pulumi_github/get_repository_environments.py` & `pulumi_github-6.3.0a1713897837/pulumi_github/get_repository_environments.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,22 +69,20 @@
 def get_repository_environments(repository: Optional[str] = None,
                                 opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetRepositoryEnvironmentsResult:
     """
     Use this data source to retrieve information about environments for a repository.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_github as github
 
     example = github.get_repository_environments(repository="example-repository")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str repository: Name of the repository to retrieve the environments from.
     """
     __args__ = dict()
     __args__['repository'] = repository
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
@@ -100,20 +98,18 @@
 def get_repository_environments_output(repository: Optional[pulumi.Input[str]] = None,
                                        opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetRepositoryEnvironmentsResult]:
     """
     Use this data source to retrieve information about environments for a repository.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_github as github
 
     example = github.get_repository_environments(repository="example-repository")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str repository: Name of the repository to retrieve the environments from.
     """
     ...
```

### Comparing `pulumi_github-6.3.0a1713561029/pulumi_github/get_repository_file.py` & `pulumi_github-6.3.0a1713897837/pulumi_github/get_repository_file.py`

 * *Files 2% similar despite different names*

```diff
@@ -161,24 +161,22 @@
                         opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetRepositoryFileResult:
     """
     This data source allows you to read files within a
     GitHub repository.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_github as github
 
     foo = github.get_repository_file(repository=foo_github_repository["name"],
         branch="main",
         file=".gitignore")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str branch: Git branch. Defaults to the repository's default branch.
     :param str file: The path of the file to read.
     :param str repository: The repository to read the file from. If an unqualified repo name (without an owner) is passed, the owner will be inferred from the owner of the token used to execute the plan. If a name of the type "owner/repo" (with a slash in the middle) is passed, the owner will be as specified and not the owner of the token.
     """
     __args__ = dict()
@@ -209,24 +207,22 @@
                                opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetRepositoryFileResult]:
     """
     This data source allows you to read files within a
     GitHub repository.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_github as github
 
     foo = github.get_repository_file(repository=foo_github_repository["name"],
         branch="main",
         file=".gitignore")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str branch: Git branch. Defaults to the repository's default branch.
     :param str file: The path of the file to read.
     :param str repository: The repository to read the file from. If an unqualified repo name (without an owner) is passed, the owner will be inferred from the owner of the token used to execute the plan. If a name of the type "owner/repo" (with a slash in the middle) is passed, the owner will be as specified and not the owner of the token.
     """
     ...
```

### Comparing `pulumi_github-6.3.0a1713561029/pulumi_github/get_repository_milestone.py` & `pulumi_github-6.3.0a1713897837/pulumi_github/get_repository_milestone.py`

 * *Files 2% similar despite different names*

```diff
@@ -124,24 +124,22 @@
                              repository: Optional[str] = None,
                              opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetRepositoryMilestoneResult:
     """
     Use this data source to retrieve information about a specific GitHub milestone in a repository.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_github as github
 
     example = github.get_repository_milestone(owner="example-owner",
         repository="example-repository",
         number=1)
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param int number: The number of the milestone.
     :param str owner: Owner of the repository.
     :param str repository: Name of the repository to retrieve the milestone from.
     """
     __args__ = dict()
@@ -168,24 +166,22 @@
                                     repository: Optional[pulumi.Input[str]] = None,
                                     opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetRepositoryMilestoneResult]:
     """
     Use this data source to retrieve information about a specific GitHub milestone in a repository.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_github as github
 
     example = github.get_repository_milestone(owner="example-owner",
         repository="example-repository",
         number=1)
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param int number: The number of the milestone.
     :param str owner: Owner of the repository.
     :param str repository: Name of the repository to retrieve the milestone from.
     """
     ...
```

### Comparing `pulumi_github-6.3.0a1713561029/pulumi_github/get_repository_pull_request.py` & `pulumi_github-6.3.0a1713897837/pulumi_github/get_repository_pull_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -253,23 +253,21 @@
                                 owner: Optional[str] = None,
                                 opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetRepositoryPullRequestResult:
     """
     Use this data source to retrieve information about a specific GitHub Pull Request in a repository.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_github as github
 
     example = github.get_repository_pull_request(base_repository="example_repository",
         number=1)
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str base_repository: Name of the base repository to retrieve the Pull Request from.
     :param int number: The number of the Pull Request within the repository.
     :param str owner: Owner of the repository. If not provided, the provider's default owner is used.
     """
     __args__ = dict()
@@ -307,23 +305,21 @@
                                        owner: Optional[pulumi.Input[Optional[str]]] = None,
                                        opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetRepositoryPullRequestResult]:
     """
     Use this data source to retrieve information about a specific GitHub Pull Request in a repository.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_github as github
 
     example = github.get_repository_pull_request(base_repository="example_repository",
         number=1)
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str base_repository: Name of the base repository to retrieve the Pull Request from.
     :param int number: The number of the Pull Request within the repository.
     :param str owner: Owner of the repository. If not provided, the provider's default owner is used.
     """
     ...
```

### Comparing `pulumi_github-6.3.0a1713561029/pulumi_github/get_repository_pull_requests.py` & `pulumi_github-6.3.0a1713897837/pulumi_github/get_repository_pull_requests.py`

 * *Files 2% similar despite different names*

```diff
@@ -138,26 +138,24 @@
                                  state: Optional[str] = None,
                                  opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetRepositoryPullRequestsResult:
     """
     Use this data source to retrieve information about multiple GitHub Pull Requests in a repository.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_github as github
 
     example = github.get_repository_pull_requests(base_repository="example-repository",
         base_ref="main",
         sort_by="updated",
         sort_direction="desc",
         state="open")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str base_ref: If set, filters Pull Requests by base branch name.
     :param str base_repository: Name of the base repository to retrieve the Pull Requests from.
     :param str head_ref: If set, filters Pull Requests by head user or head organization and branch name in the format of "user:ref-name" or "organization:ref-name". For example: "github:new-script-format" or "octocat:test-branch".
     :param str owner: Owner of the repository. If not provided, the provider's default owner is used.
     :param str sort_by: If set, indicates what to sort results by. Can be either "created", "updated", "popularity" (comment count) or "long-running" (age, filtering by pulls updated in the last month). Default: "created".
@@ -197,26 +195,24 @@
                                         state: Optional[pulumi.Input[Optional[str]]] = None,
                                         opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetRepositoryPullRequestsResult]:
     """
     Use this data source to retrieve information about multiple GitHub Pull Requests in a repository.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_github as github
 
     example = github.get_repository_pull_requests(base_repository="example-repository",
         base_ref="main",
         sort_by="updated",
         sort_direction="desc",
         state="open")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str base_ref: If set, filters Pull Requests by base branch name.
     :param str base_repository: Name of the base repository to retrieve the Pull Requests from.
     :param str head_ref: If set, filters Pull Requests by head user or head organization and branch name in the format of "user:ref-name" or "organization:ref-name". For example: "github:new-script-format" or "octocat:test-branch".
     :param str owner: Owner of the repository. If not provided, the provider's default owner is used.
     :param str sort_by: If set, indicates what to sort results by. Can be either "created", "updated", "popularity" (comment count) or "long-running" (age, filtering by pulls updated in the last month). Default: "created".
```

### Comparing `pulumi_github-6.3.0a1713561029/pulumi_github/get_repository_teams.py` & `pulumi_github-6.3.0a1713897837/pulumi_github/get_repository_teams.py`

 * *Files 4% similar despite different names*

```diff
@@ -82,22 +82,20 @@
                          name: Optional[str] = None,
                          opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetRepositoryTeamsResult:
     """
     Use this data source to retrieve the list of teams which have access to a GitHub repository.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_github as github
 
     example = github.get_repository_teams(name="example")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str full_name: Full name of the repository (in `org/name` format).
     :param str name: The name of the repository.
     """
     __args__ = dict()
     __args__['fullName'] = full_name
@@ -117,21 +115,19 @@
                                 name: Optional[pulumi.Input[Optional[str]]] = None,
                                 opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetRepositoryTeamsResult]:
     """
     Use this data source to retrieve the list of teams which have access to a GitHub repository.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_github as github
 
     example = github.get_repository_teams(name="example")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str full_name: Full name of the repository (in `org/name` format).
     :param str name: The name of the repository.
     """
     ...
```

### Comparing `pulumi_github-6.3.0a1713561029/pulumi_github/get_repository_webhooks.py` & `pulumi_github-6.3.0a1713897837/pulumi_github/get_repository_webhooks.py`

 * *Files 4% similar despite different names*

```diff
@@ -72,22 +72,20 @@
     """
     Use this data source to retrieve webhooks for a given repository.
 
     ## Example Usage
 
     To retrieve webhooks of a repository:
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_github as github
 
     repo = github.get_repository_webhooks(repository="foo")
     ```
-    <!--End PulumiCodeChooser -->
     """
     __args__ = dict()
     __args__['repository'] = repository
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('github:index/getRepositoryWebhooks:getRepositoryWebhooks', __args__, opts=opts, typ=GetRepositoryWebhooksResult).value
 
     return AwaitableGetRepositoryWebhooksResult(
@@ -102,17 +100,15 @@
     """
     Use this data source to retrieve webhooks for a given repository.
 
     ## Example Usage
 
     To retrieve webhooks of a repository:
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_github as github
 
     repo = github.get_repository_webhooks(repository="foo")
     ```
-    <!--End PulumiCodeChooser -->
     """
     ...
```

### Comparing `pulumi_github-6.3.0a1713561029/pulumi_github/get_rest_api.py` & `pulumi_github-6.3.0a1713897837/pulumi_github/get_rest_api.py`

 * *Files 6% similar despite different names*

```diff
@@ -104,22 +104,20 @@
 def get_rest_api(endpoint: Optional[str] = None,
                  opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetRestApiResult:
     """
     Use this data source to retrieve information about a GitHub resource through REST API.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_github as github
 
     example = github.get_rest_api(endpoint="repos/example_repo/git/refs/heads/main")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str endpoint: REST API endpoint to send the GET request to.
     """
     __args__ = dict()
     __args__['endpoint'] = endpoint
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
@@ -138,20 +136,18 @@
 def get_rest_api_output(endpoint: Optional[pulumi.Input[str]] = None,
                         opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetRestApiResult]:
     """
     Use this data source to retrieve information about a GitHub resource through REST API.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_github as github
 
     example = github.get_rest_api(endpoint="repos/example_repo/git/refs/heads/main")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str endpoint: REST API endpoint to send the GET request to.
     """
     ...
```

### Comparing `pulumi_github-6.3.0a1713561029/pulumi_github/get_ssh_keys.py` & `pulumi_github-6.3.0a1713897837/pulumi_github/get_ssh_keys.py`

 * *Files 8% similar despite different names*

```diff
@@ -58,22 +58,20 @@
 
 def get_ssh_keys(opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetSshKeysResult:
     """
     Use this data source to retrieve information about GitHub's SSH keys.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_github as github
 
     test = github.get_ssh_keys()
     ```
-    <!--End PulumiCodeChooser -->
     """
     __args__ = dict()
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('github:index/getSshKeys:getSshKeys', __args__, opts=opts, typ=GetSshKeysResult).value
 
     return AwaitableGetSshKeysResult(
         id=pulumi.get(__ret__, 'id'),
@@ -83,17 +81,15 @@
 @_utilities.lift_output_func(get_ssh_keys)
 def get_ssh_keys_output(opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetSshKeysResult]:
     """
     Use this data source to retrieve information about GitHub's SSH keys.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_github as github
 
     test = github.get_ssh_keys()
     ```
-    <!--End PulumiCodeChooser -->
     """
     ...
```

### Comparing `pulumi_github-6.3.0a1713561029/pulumi_github/get_team.py` & `pulumi_github-6.3.0a1713897837/pulumi_github/get_team.py`

 * *Files 2% similar despite different names*

```diff
@@ -183,22 +183,20 @@
              summary_only: Optional[bool] = None,
              opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetTeamResult:
     """
     Use this data source to retrieve information about a GitHub team.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_github as github
 
     example = github.get_team(slug="example")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str membership_type: Type of membership to be requested to fill the list of members. Can be either "all" or "immediate". Default: "all"
     :param int results_per_page: Set the number of results per graphql query. Reducing this number can alleviate timeout errors. Accepts a value between 0 - 100. Defaults to `100`.
     :param str slug: The team slug.
     :param bool summary_only: Exclude the members and repositories of the team from the returned result. Defaults to `false`.
     """
@@ -233,22 +231,20 @@
                     summary_only: Optional[pulumi.Input[Optional[bool]]] = None,
                     opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetTeamResult]:
     """
     Use this data source to retrieve information about a GitHub team.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_github as github
 
     example = github.get_team(slug="example")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str membership_type: Type of membership to be requested to fill the list of members. Can be either "all" or "immediate". Default: "all"
     :param int results_per_page: Set the number of results per graphql query. Reducing this number can alleviate timeout errors. Accepts a value between 0 - 100. Defaults to `100`.
     :param str slug: The team slug.
     :param bool summary_only: Exclude the members and repositories of the team from the returned result. Defaults to `false`.
     """
```

### Comparing `pulumi_github-6.3.0a1713561029/pulumi_github/get_tree.py` & `pulumi_github-6.3.0a1713897837/pulumi_github/get_tree.py`

 * *Files 1% similar despite different names*

```diff
@@ -89,28 +89,26 @@
              tree_sha: Optional[str] = None,
              opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetTreeResult:
     """
     Use this data source to retrieve information about a single tree.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_github as github
 
     this = github.get_repository(name="example")
     this_get_branch = github.get_branch(branch=this.default_branch,
         repository=this.name)
     this_get_tree = github.get_tree(recursive=False,
         repository=this.name,
         tree_sha=this_get_branch.sha)
     pulumi.export("entries", this_get_tree.entries)
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param bool recursive: Setting this parameter to `true` returns the objects or subtrees referenced by the tree specified in `tree_sha`.
     :param str repository: The name of the repository.
     :param str tree_sha: The SHA1 value for the tree.
     """
     __args__ = dict()
@@ -134,28 +132,26 @@
                     tree_sha: Optional[pulumi.Input[str]] = None,
                     opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetTreeResult]:
     """
     Use this data source to retrieve information about a single tree.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_github as github
 
     this = github.get_repository(name="example")
     this_get_branch = github.get_branch(branch=this.default_branch,
         repository=this.name)
     this_get_tree = github.get_tree(recursive=False,
         repository=this.name,
         tree_sha=this_get_branch.sha)
     pulumi.export("entries", this_get_tree.entries)
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param bool recursive: Setting this parameter to `true` returns the objects or subtrees referenced by the tree specified in `tree_sha`.
     :param str repository: The name of the repository.
     :param str tree_sha: The SHA1 value for the tree.
     """
     ...
```

### Comparing `pulumi_github-6.3.0a1713561029/pulumi_github/get_user.py` & `pulumi_github-6.3.0a1713897837/pulumi_github/get_user.py`

 * *Files 1% similar despite different names*

```diff
@@ -296,26 +296,24 @@
 def get_user(username: Optional[str] = None,
              opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetUserResult:
     """
     Use this data source to retrieve information about a GitHub user.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_github as github
 
     # Retrieve information about a GitHub user.
     example = github.get_user(username="example")
     # Retrieve information about the currently authenticated user.
     current = github.get_user(username="")
     pulumi.export("currentGithubLogin", current.login)
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str username: The username. Use an empty string `""` to retrieve information about the currently authenticated user.
     """
     __args__ = dict()
     __args__['username'] = username
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
@@ -350,24 +348,22 @@
 def get_user_output(username: Optional[pulumi.Input[str]] = None,
                     opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetUserResult]:
     """
     Use this data source to retrieve information about a GitHub user.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_github as github
 
     # Retrieve information about a GitHub user.
     example = github.get_user(username="example")
     # Retrieve information about the currently authenticated user.
     current = github.get_user(username="")
     pulumi.export("currentGithubLogin", current.login)
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str username: The username. Use an empty string `""` to retrieve information about the currently authenticated user.
     """
     ...
```

### Comparing `pulumi_github-6.3.0a1713561029/pulumi_github/get_user_external_identity.py` & `pulumi_github-6.3.0a1713897837/pulumi_github/get_user_external_identity.py`

 * *Files 10% similar despite different names*

```diff
@@ -98,22 +98,20 @@
                                opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetUserExternalIdentityResult:
     """
     Use this data source to retrieve a specific organization member's SAML or SCIM user
     attributes.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_github as github
 
     example_user = github.get_user_external_identity(username="example-user")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str username: The username of the member to fetch external identity for.
     """
     __args__ = dict()
     __args__['username'] = username
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
@@ -132,20 +130,18 @@
                                       opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetUserExternalIdentityResult]:
     """
     Use this data source to retrieve a specific organization member's SAML or SCIM user
     attributes.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_github as github
 
     example_user = github.get_user_external_identity(username="example-user")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str username: The username of the member to fetch external identity for.
     """
     ...
```

### Comparing `pulumi_github-6.3.0a1713561029/pulumi_github/get_users.py` & `pulumi_github-6.3.0a1713897837/pulumi_github/get_users.py`

 * *Files 4% similar despite different names*

```diff
@@ -104,29 +104,27 @@
 def get_users(usernames: Optional[Sequence[str]] = None,
               opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetUsersResult:
     """
     Use this data source to retrieve information about multiple GitHub users at once.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_github as github
 
     # Retrieve information about multiple GitHub users.
     example = github.get_users(usernames=[
         "example1",
         "example2",
         "example3",
     ])
     pulumi.export("validUsers", example.logins)
     pulumi.export("invalidUsers", example.unknown_logins)
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param Sequence[str] usernames: List of usernames.
     """
     __args__ = dict()
     __args__['usernames'] = usernames
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
@@ -145,27 +143,25 @@
 def get_users_output(usernames: Optional[pulumi.Input[Sequence[str]]] = None,
                      opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetUsersResult]:
     """
     Use this data source to retrieve information about multiple GitHub users at once.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_github as github
 
     # Retrieve information about multiple GitHub users.
     example = github.get_users(usernames=[
         "example1",
         "example2",
         "example3",
     ])
     pulumi.export("validUsers", example.logins)
     pulumi.export("invalidUsers", example.unknown_logins)
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param Sequence[str] usernames: List of usernames.
     """
     ...
```

### Comparing `pulumi_github-6.3.0a1713561029/pulumi_github/issue.py` & `pulumi_github-6.3.0a1713897837/pulumi_github/issue.py`

 * *Files 2% similar despite different names*

```diff
@@ -277,34 +277,31 @@
         Provides a GitHub issue resource.
 
         This resource allows you to create and manage issue within your
         GitHub repository.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_github as github
 
         # Create a simple issue
         test = github.Repository("test",
             name="tf-acc-test-%s",
             auto_init=True,
             has_issues=True)
         test_issue = github.Issue("test",
             repository=test.name,
             title="My issue title",
             body="The body of my issue")
         ```
-        <!--End PulumiCodeChooser -->
 
         ### With Milestone And Project Assignment
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_github as github
         import pulumi_std as std
 
         # Create an issue with milestone and project assignment
         test = github.Repository("test",
@@ -326,15 +323,14 @@
             labels=[
                 "bug",
                 "documentation",
             ],
             assignees=["bob-github"],
             milestone_number=test_repository_milestone.number)
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         GitHub Issues can be imported using an ID made up of `repository:number`, e.g.
 
         ```sh
         $ pulumi import github:index/issue:Issue issue_15 myrepo:15
@@ -359,34 +355,31 @@
         Provides a GitHub issue resource.
 
         This resource allows you to create and manage issue within your
         GitHub repository.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_github as github
 
         # Create a simple issue
         test = github.Repository("test",
             name="tf-acc-test-%s",
             auto_init=True,
             has_issues=True)
         test_issue = github.Issue("test",
             repository=test.name,
             title="My issue title",
             body="The body of my issue")
         ```
-        <!--End PulumiCodeChooser -->
 
         ### With Milestone And Project Assignment
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_github as github
         import pulumi_std as std
 
         # Create an issue with milestone and project assignment
         test = github.Repository("test",
@@ -408,15 +401,14 @@
             labels=[
                 "bug",
                 "documentation",
             ],
             assignees=["bob-github"],
             milestone_number=test_repository_milestone.number)
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         GitHub Issues can be imported using an ID made up of `repository:number`, e.g.
 
         ```sh
         $ pulumi import github:index/issue:Issue issue_15 myrepo:15
```

### Comparing `pulumi_github-6.3.0a1713561029/pulumi_github/issue_label.py` & `pulumi_github-6.3.0a1713897837/pulumi_github/issue_label.py`

 * *Files 2% similar despite different names*

```diff
@@ -190,26 +190,24 @@
                  description: Optional[pulumi.Input[str]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  repository: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_github as github
 
         # Create a new, red colored label
         test_repo = github.IssueLabel("test_repo",
             repository="test-repo",
             name="Urgent",
             color="FF0000")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         GitHub Issue Labels can be imported using an ID made up of `repository:name`, e.g.
 
         ```sh
         $ pulumi import github:index/issueLabel:IssueLabel panic_label terraform:panic
@@ -227,26 +225,24 @@
     def __init__(__self__,
                  resource_name: str,
                  args: IssueLabelArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_github as github
 
         # Create a new, red colored label
         test_repo = github.IssueLabel("test_repo",
             repository="test-repo",
             name="Urgent",
             color="FF0000")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         GitHub Issue Labels can be imported using an ID made up of `repository:name`, e.g.
 
         ```sh
         $ pulumi import github:index/issueLabel:IssueLabel panic_label terraform:panic
```

### Comparing `pulumi_github-6.3.0a1713561029/pulumi_github/issue_labels.py` & `pulumi_github-6.3.0a1713897837/pulumi_github/issue_labels.py`

 * *Files 2% similar despite different names*

```diff
@@ -110,15 +110,14 @@
 
         This resource is authoritative. For adding a label to a repo in a non-authoritative manner, use IssueLabel instead.
 
         If you change the case of a label's name, its' color, or description, this resource will edit the existing label to match the new values. However, if you change the name of a label, this resource will create a new label with the new name and delete the old label. Beware that this will remove the label from any issues it was previously attached to.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_github as github
 
         # Create a new, red colored label
         test_repo = github.IssueLabels("test_repo",
             repository="test-repo",
@@ -129,15 +128,14 @@
                 ),
                 github.IssueLabelsLabelArgs(
                     name="Critical",
                     color="FF0000",
                 ),
             ])
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         GitHub Issue Labels can be imported using the repository `name`, e.g.
 
         ```sh
         $ pulumi import github:index/issueLabels:IssueLabels test_repo test_repo
@@ -164,15 +162,14 @@
 
         This resource is authoritative. For adding a label to a repo in a non-authoritative manner, use IssueLabel instead.
 
         If you change the case of a label's name, its' color, or description, this resource will edit the existing label to match the new values. However, if you change the name of a label, this resource will create a new label with the new name and delete the old label. Beware that this will remove the label from any issues it was previously attached to.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_github as github
 
         # Create a new, red colored label
         test_repo = github.IssueLabels("test_repo",
             repository="test-repo",
@@ -183,15 +180,14 @@
                 ),
                 github.IssueLabelsLabelArgs(
                     name="Critical",
                     color="FF0000",
                 ),
             ])
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         GitHub Issue Labels can be imported using the repository `name`, e.g.
 
         ```sh
         $ pulumi import github:index/issueLabels:IssueLabels test_repo test_repo
```

### Comparing `pulumi_github-6.3.0a1713561029/pulumi_github/membership.py` & `pulumi_github-6.3.0a1713897837/pulumi_github/membership.py`

 * *Files 2% similar despite different names*

```diff
@@ -168,25 +168,23 @@
 
         This resource allows you to add/remove users from your organization. When applied,
         an invitation will be sent to the user to become part of the organization. When
         destroyed, either the invitation will be cancelled or the user will be removed.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_github as github
 
         # Add a user to the organization
         membership_for_some_user = github.Membership("membership_for_some_user",
             username="SomeUser",
             role="member")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         GitHub Membership can be imported using an ID made up of `organization:username`, e.g.
 
         ```sh
         $ pulumi import github:index/membership:Membership member hashicorp:someuser
@@ -214,25 +212,23 @@
 
         This resource allows you to add/remove users from your organization. When applied,
         an invitation will be sent to the user to become part of the organization. When
         destroyed, either the invitation will be cancelled or the user will be removed.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_github as github
 
         # Add a user to the organization
         membership_for_some_user = github.Membership("membership_for_some_user",
             username="SomeUser",
             role="member")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         GitHub Membership can be imported using an ID made up of `organization:username`, e.g.
 
         ```sh
         $ pulumi import github:index/membership:Membership member hashicorp:someuser
```

### Comparing `pulumi_github-6.3.0a1713561029/pulumi_github/organization_block.py` & `pulumi_github-6.3.0a1713897837/pulumi_github/organization_block.py`

 * *Files 10% similar despite different names*

```diff
@@ -78,22 +78,20 @@
                  username: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         This resource allows you to create and manage blocks for GitHub organizations.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_github as github
 
         example = github.OrganizationBlock("example", username="paultyng")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         GitHub organization block can be imported using a username, e.g.
 
         ```sh
         $ pulumi import github:index/organizationBlock:OrganizationBlock example someuser
@@ -110,22 +108,20 @@
                  args: OrganizationBlockArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         This resource allows you to create and manage blocks for GitHub organizations.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_github as github
 
         example = github.OrganizationBlock("example", username="paultyng")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         GitHub organization block can be imported using a username, e.g.
 
         ```sh
         $ pulumi import github:index/organizationBlock:OrganizationBlock example someuser
```

### Comparing `pulumi_github-6.3.0a1713561029/pulumi_github/organization_custom_role.py` & `pulumi_github-6.3.0a1713897837/pulumi_github/organization_custom_role.py`

 * *Files 2% similar despite different names*

```diff
@@ -166,15 +166,14 @@
         """
         This resource allows you to create and manage custom roles in a GitHub Organization for use in repositories.
 
         > Note: Custom roles are currently only available in GitHub Enterprise Cloud.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_github as github
 
         example = github.OrganizationCustomRole("example",
             name="example",
             description="Example custom role that uses the read role as its base",
@@ -197,15 +196,14 @@
                 "request_pr_review",
                 "resolve_dependabot_alerts",
                 "resolve_secret_scanning_alerts",
                 "view_secret_scanning_alerts",
                 "write_code_scanning",
             ])
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Custom roles can be imported using the `id` of the role.
         The `id` of the custom role can be found using the [list custom roles in an organization](https://docs.github.com/en/enterprise-cloud@latest/rest/orgs/custom-roles#list-custom-repository-roles-in-an-organization) API.
 
         ```sh
@@ -228,15 +226,14 @@
         """
         This resource allows you to create and manage custom roles in a GitHub Organization for use in repositories.
 
         > Note: Custom roles are currently only available in GitHub Enterprise Cloud.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_github as github
 
         example = github.OrganizationCustomRole("example",
             name="example",
             description="Example custom role that uses the read role as its base",
@@ -259,15 +256,14 @@
                 "request_pr_review",
                 "resolve_dependabot_alerts",
                 "resolve_secret_scanning_alerts",
                 "view_secret_scanning_alerts",
                 "write_code_scanning",
             ])
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Custom roles can be imported using the `id` of the role.
         The `id` of the custom role can be found using the [list custom roles in an organization](https://docs.github.com/en/enterprise-cloud@latest/rest/orgs/custom-roles#list-custom-repository-roles-in-an-organization) API.
 
         ```sh
```

### Comparing `pulumi_github-6.3.0a1713561029/pulumi_github/organization_project.py` & `pulumi_github-6.3.0a1713897837/pulumi_github/organization_project.py`

 * *Files 3% similar despite different names*

```diff
@@ -128,24 +128,22 @@
                  name: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         This resource allows you to create and manage projects for GitHub organization.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_github as github
 
         project = github.OrganizationProject("project",
             name="A Organization Project",
             body="This is a organization project.")
         ```
-        <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] body: The body of the project.
         :param pulumi.Input[str] name: The name of the project.
         """
         ...
@@ -155,24 +153,22 @@
                  args: Optional[OrganizationProjectArgs] = None,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         This resource allows you to create and manage projects for GitHub organization.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_github as github
 
         project = github.OrganizationProject("project",
             name="A Organization Project",
             body="This is a organization project.")
         ```
-        <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param OrganizationProjectArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
```

### Comparing `pulumi_github-6.3.0a1713561029/pulumi_github/organization_ruleset.py` & `pulumi_github-6.3.0a1713897837/pulumi_github/organization_ruleset.py`

 * *Files 1% similar despite different names*

```diff
@@ -281,15 +281,14 @@
         """
         Creates a GitHub organization ruleset.
 
         This resource allows you to create and manage rulesets on the organization level. When applied, a new ruleset will be created. When destroyed, that ruleset will be removed.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_github as github
 
         example = github.OrganizationRuleset("example",
             name="example",
             target="branch",
@@ -315,15 +314,14 @@
                     name="example",
                     negate=False,
                     operator="starts_with",
                     pattern="ex",
                 ),
             ))
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         GitHub Organization Rulesets can be imported using the GitHub ruleset ID e.g.
 
         ```sh
         $ pulumi import github:index/organizationRuleset:OrganizationRuleset example 12345`
@@ -347,15 +345,14 @@
         """
         Creates a GitHub organization ruleset.
 
         This resource allows you to create and manage rulesets on the organization level. When applied, a new ruleset will be created. When destroyed, that ruleset will be removed.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_github as github
 
         example = github.OrganizationRuleset("example",
             name="example",
             target="branch",
@@ -381,15 +378,14 @@
                     name="example",
                     negate=False,
                     operator="starts_with",
                     pattern="ex",
                 ),
             ))
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         GitHub Organization Rulesets can be imported using the GitHub ruleset ID e.g.
 
         ```sh
         $ pulumi import github:index/organizationRuleset:OrganizationRuleset example 12345`
```

### Comparing `pulumi_github-6.3.0a1713561029/pulumi_github/organization_security_manager.py` & `pulumi_github-6.3.0a1713897837/pulumi_github/organization_security_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,25 +64,23 @@
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  team_slug: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_github as github
 
         some_team = github.Team("some_team",
             name="SomeTeam",
             description="Some cool team")
         some_team_organization_security_manager = github.OrganizationSecurityManager("some_team", team_slug=some_team.slug)
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         GitHub Security Manager Teams can be imported using the GitHub team ID e.g.
 
         ```sh
         $ pulumi import github:index/organizationSecurityManager:OrganizationSecurityManager core 1234567
@@ -97,25 +95,23 @@
     def __init__(__self__,
                  resource_name: str,
                  args: OrganizationSecurityManagerArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_github as github
 
         some_team = github.Team("some_team",
             name="SomeTeam",
             description="Some cool team")
         some_team_organization_security_manager = github.OrganizationSecurityManager("some_team", team_slug=some_team.slug)
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         GitHub Security Manager Teams can be imported using the GitHub team ID e.g.
 
         ```sh
         $ pulumi import github:index/organizationSecurityManager:OrganizationSecurityManager core 1234567
```

### Comparing `pulumi_github-6.3.0a1713561029/pulumi_github/organization_settings.py` & `pulumi_github-6.3.0a1713897837/pulumi_github/organization_settings.py`

 * *Files 0% similar despite different names*

```diff
@@ -891,15 +891,14 @@
                  web_commit_signoff_required: Optional[pulumi.Input[bool]] = None,
                  __props__=None):
         """
         This resource allows you to create and manage settings for a GitHub Organization.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_github as github
 
         test = github.OrganizationSettings("test",
             billing_email="test@example.com",
             company="Test Company",
@@ -924,15 +923,14 @@
             advanced_security_enabled_for_new_repositories=False,
             dependabot_alerts_enabled_for_new_repositories=False,
             dependabot_security_updates_enabled_for_new_repositories=False,
             dependency_graph_enabled_for_new_repositories=False,
             secret_scanning_enabled_for_new_repositories=False,
             secret_scanning_push_protection_enabled_for_new_repositories=False)
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Organization settings can be imported using the `id` of the organization.
         The `id` of the organization can be found using the [get an organization](https://docs.github.com/en/rest/orgs/orgs#get-an-organization) API.
 
         ```sh
@@ -975,15 +973,14 @@
                  args: OrganizationSettingsArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         This resource allows you to create and manage settings for a GitHub Organization.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_github as github
 
         test = github.OrganizationSettings("test",
             billing_email="test@example.com",
             company="Test Company",
@@ -1008,15 +1005,14 @@
             advanced_security_enabled_for_new_repositories=False,
             dependabot_alerts_enabled_for_new_repositories=False,
             dependabot_security_updates_enabled_for_new_repositories=False,
             dependency_graph_enabled_for_new_repositories=False,
             secret_scanning_enabled_for_new_repositories=False,
             secret_scanning_push_protection_enabled_for_new_repositories=False)
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Organization settings can be imported using the `id` of the organization.
         The `id` of the organization can be found using the [get an organization](https://docs.github.com/en/rest/orgs/orgs#get-an-organization) API.
 
         ```sh
```

### Comparing `pulumi_github-6.3.0a1713561029/pulumi_github/organization_webhook.py` & `pulumi_github-6.3.0a1713897837/pulumi_github/organization_webhook.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-6.3.0a1713561029/pulumi_github/outputs.py` & `pulumi_github-6.3.0a1713897837/pulumi_github/outputs.py`

 * *Files 2% similar despite different names*

```diff
@@ -1090,66 +1090,66 @@
 
 @pulumi.output_type
 class OrganizationRulesetConditionsRefName(dict):
     def __init__(__self__, *,
                  excludes: Sequence[str],
                  includes: Sequence[str]):
         """
-        :param Sequence[str] excludes: (List of String) Array of repository names or patterns to exclude. The condition will not pass if any of these patterns match.
-        :param Sequence[str] includes: (List of String) Array of repository names or patterns to include. One of these patterns must match for the condition to pass. Also accepts `~ALL` to include all repositories.
+        :param Sequence[str] excludes: Array of ref names or patterns to exclude. The condition will not pass if any of these patterns match.
+        :param Sequence[str] includes: Array of ref names or patterns to include. One of these patterns must match for the condition to pass. Also accepts `~DEFAULT_BRANCH` to include the default branch or `~ALL` to include all branches.
         """
         pulumi.set(__self__, "excludes", excludes)
         pulumi.set(__self__, "includes", includes)
 
     @property
     @pulumi.getter
     def excludes(self) -> Sequence[str]:
         """
-        (List of String) Array of repository names or patterns to exclude. The condition will not pass if any of these patterns match.
+        Array of ref names or patterns to exclude. The condition will not pass if any of these patterns match.
         """
         return pulumi.get(self, "excludes")
 
     @property
     @pulumi.getter
     def includes(self) -> Sequence[str]:
         """
-        (List of String) Array of repository names or patterns to include. One of these patterns must match for the condition to pass. Also accepts `~ALL` to include all repositories.
+        Array of ref names or patterns to include. One of these patterns must match for the condition to pass. Also accepts `~DEFAULT_BRANCH` to include the default branch or `~ALL` to include all branches.
         """
         return pulumi.get(self, "includes")
 
 
 @pulumi.output_type
 class OrganizationRulesetConditionsRepositoryName(dict):
     def __init__(__self__, *,
                  excludes: Sequence[str],
                  includes: Sequence[str],
                  protected: Optional[bool] = None):
         """
-        :param Sequence[str] excludes: (List of String) Array of repository names or patterns to exclude. The condition will not pass if any of these patterns match.
-        :param Sequence[str] includes: (List of String) Array of repository names or patterns to include. One of these patterns must match for the condition to pass. Also accepts `~ALL` to include all repositories.
+        :param Sequence[str] excludes: Array of repository names or patterns to exclude. The condition will not pass if any of these patterns match.
+        :param Sequence[str] includes: Array of repository names or patterns to include. One of these patterns must match for the condition to pass. Also accepts `~ALL` to include all repositories.
         :param bool protected: Whether renaming of target repositories is prevented.
         """
         pulumi.set(__self__, "excludes", excludes)
         pulumi.set(__self__, "includes", includes)
         if protected is not None:
             pulumi.set(__self__, "protected", protected)
 
     @property
     @pulumi.getter
     def excludes(self) -> Sequence[str]:
         """
-        (List of String) Array of repository names or patterns to exclude. The condition will not pass if any of these patterns match.
+        Array of repository names or patterns to exclude. The condition will not pass if any of these patterns match.
         """
         return pulumi.get(self, "excludes")
 
     @property
     @pulumi.getter
     def includes(self) -> Sequence[str]:
         """
-        (List of String) Array of repository names or patterns to include. One of these patterns must match for the condition to pass. Also accepts `~ALL` to include all repositories.
+        Array of repository names or patterns to include. One of these patterns must match for the condition to pass. Also accepts `~ALL` to include all repositories.
         """
         return pulumi.get(self, "includes")
 
     @property
     @pulumi.getter
     def protected(self) -> Optional[bool]:
         """
@@ -1374,39 +1374,39 @@
 class OrganizationRulesetRulesBranchNamePattern(dict):
     def __init__(__self__, *,
                  operator: str,
                  pattern: str,
                  name: Optional[str] = None,
                  negate: Optional[bool] = None):
         """
-        :param str operator: (String) The operator to use for matching. Can be one of: `starts_with`, `ends_with`, `contains`, `regex`.
-        :param str pattern: (String) The pattern to match with.
+        :param str operator: The operator to use for matching. Can be one of: `starts_with`, `ends_with`, `contains`, `regex`.
+        :param str pattern: The pattern to match with.
         :param str name: (String) The name of the ruleset.
-        :param bool negate: (Boolean) If true, the rule will fail if the pattern matches.
+        :param bool negate: If true, the rule will fail if the pattern matches.
         """
         pulumi.set(__self__, "operator", operator)
         pulumi.set(__self__, "pattern", pattern)
         if name is not None:
             pulumi.set(__self__, "name", name)
         if negate is not None:
             pulumi.set(__self__, "negate", negate)
 
     @property
     @pulumi.getter
     def operator(self) -> str:
         """
-        (String) The operator to use for matching. Can be one of: `starts_with`, `ends_with`, `contains`, `regex`.
+        The operator to use for matching. Can be one of: `starts_with`, `ends_with`, `contains`, `regex`.
         """
         return pulumi.get(self, "operator")
 
     @property
     @pulumi.getter
     def pattern(self) -> str:
         """
-        (String) The pattern to match with.
+        The pattern to match with.
         """
         return pulumi.get(self, "pattern")
 
     @property
     @pulumi.getter
     def name(self) -> Optional[str]:
         """
@@ -1414,52 +1414,52 @@
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter
     def negate(self) -> Optional[bool]:
         """
-        (Boolean) If true, the rule will fail if the pattern matches.
+        If true, the rule will fail if the pattern matches.
         """
         return pulumi.get(self, "negate")
 
 
 @pulumi.output_type
 class OrganizationRulesetRulesCommitAuthorEmailPattern(dict):
     def __init__(__self__, *,
                  operator: str,
                  pattern: str,
                  name: Optional[str] = None,
                  negate: Optional[bool] = None):
         """
-        :param str operator: (String) The operator to use for matching. Can be one of: `starts_with`, `ends_with`, `contains`, `regex`.
-        :param str pattern: (String) The pattern to match with.
+        :param str operator: The operator to use for matching. Can be one of: `starts_with`, `ends_with`, `contains`, `regex`.
+        :param str pattern: The pattern to match with.
         :param str name: (String) The name of the ruleset.
-        :param bool negate: (Boolean) If true, the rule will fail if the pattern matches.
+        :param bool negate: If true, the rule will fail if the pattern matches.
         """
         pulumi.set(__self__, "operator", operator)
         pulumi.set(__self__, "pattern", pattern)
         if name is not None:
             pulumi.set(__self__, "name", name)
         if negate is not None:
             pulumi.set(__self__, "negate", negate)
 
     @property
     @pulumi.getter
     def operator(self) -> str:
         """
-        (String) The operator to use for matching. Can be one of: `starts_with`, `ends_with`, `contains`, `regex`.
+        The operator to use for matching. Can be one of: `starts_with`, `ends_with`, `contains`, `regex`.
         """
         return pulumi.get(self, "operator")
 
     @property
     @pulumi.getter
     def pattern(self) -> str:
         """
-        (String) The pattern to match with.
+        The pattern to match with.
         """
         return pulumi.get(self, "pattern")
 
     @property
     @pulumi.getter
     def name(self) -> Optional[str]:
         """
@@ -1467,52 +1467,52 @@
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter
     def negate(self) -> Optional[bool]:
         """
-        (Boolean) If true, the rule will fail if the pattern matches.
+        If true, the rule will fail if the pattern matches.
         """
         return pulumi.get(self, "negate")
 
 
 @pulumi.output_type
 class OrganizationRulesetRulesCommitMessagePattern(dict):
     def __init__(__self__, *,
                  operator: str,
                  pattern: str,
                  name: Optional[str] = None,
                  negate: Optional[bool] = None):
         """
-        :param str operator: (String) The operator to use for matching. Can be one of: `starts_with`, `ends_with`, `contains`, `regex`.
-        :param str pattern: (String) The pattern to match with.
+        :param str operator: The operator to use for matching. Can be one of: `starts_with`, `ends_with`, `contains`, `regex`.
+        :param str pattern: The pattern to match with.
         :param str name: (String) The name of the ruleset.
-        :param bool negate: (Boolean) If true, the rule will fail if the pattern matches.
+        :param bool negate: If true, the rule will fail if the pattern matches.
         """
         pulumi.set(__self__, "operator", operator)
         pulumi.set(__self__, "pattern", pattern)
         if name is not None:
             pulumi.set(__self__, "name", name)
         if negate is not None:
             pulumi.set(__self__, "negate", negate)
 
     @property
     @pulumi.getter
     def operator(self) -> str:
         """
-        (String) The operator to use for matching. Can be one of: `starts_with`, `ends_with`, `contains`, `regex`.
+        The operator to use for matching. Can be one of: `starts_with`, `ends_with`, `contains`, `regex`.
         """
         return pulumi.get(self, "operator")
 
     @property
     @pulumi.getter
     def pattern(self) -> str:
         """
-        (String) The pattern to match with.
+        The pattern to match with.
         """
         return pulumi.get(self, "pattern")
 
     @property
     @pulumi.getter
     def name(self) -> Optional[str]:
         """
@@ -1520,52 +1520,52 @@
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter
     def negate(self) -> Optional[bool]:
         """
-        (Boolean) If true, the rule will fail if the pattern matches.
+        If true, the rule will fail if the pattern matches.
         """
         return pulumi.get(self, "negate")
 
 
 @pulumi.output_type
 class OrganizationRulesetRulesCommitterEmailPattern(dict):
     def __init__(__self__, *,
                  operator: str,
                  pattern: str,
                  name: Optional[str] = None,
                  negate: Optional[bool] = None):
         """
-        :param str operator: (String) The operator to use for matching. Can be one of: `starts_with`, `ends_with`, `contains`, `regex`.
-        :param str pattern: (String) The pattern to match with.
+        :param str operator: The operator to use for matching. Can be one of: `starts_with`, `ends_with`, `contains`, `regex`.
+        :param str pattern: The pattern to match with.
         :param str name: (String) The name of the ruleset.
-        :param bool negate: (Boolean) If true, the rule will fail if the pattern matches.
+        :param bool negate: If true, the rule will fail if the pattern matches.
         """
         pulumi.set(__self__, "operator", operator)
         pulumi.set(__self__, "pattern", pattern)
         if name is not None:
             pulumi.set(__self__, "name", name)
         if negate is not None:
             pulumi.set(__self__, "negate", negate)
 
     @property
     @pulumi.getter
     def operator(self) -> str:
         """
-        (String) The operator to use for matching. Can be one of: `starts_with`, `ends_with`, `contains`, `regex`.
+        The operator to use for matching. Can be one of: `starts_with`, `ends_with`, `contains`, `regex`.
         """
         return pulumi.get(self, "operator")
 
     @property
     @pulumi.getter
     def pattern(self) -> str:
         """
-        (String) The pattern to match with.
+        The pattern to match with.
         """
         return pulumi.get(self, "pattern")
 
     @property
     @pulumi.getter
     def name(self) -> Optional[str]:
         """
@@ -1573,15 +1573,15 @@
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter
     def negate(self) -> Optional[bool]:
         """
-        (Boolean) If true, the rule will fail if the pattern matches.
+        If true, the rule will fail if the pattern matches.
         """
         return pulumi.get(self, "negate")
 
 
 @pulumi.output_type
 class OrganizationRulesetRulesPullRequest(dict):
     @staticmethod
@@ -1612,19 +1612,19 @@
     def __init__(__self__, *,
                  dismiss_stale_reviews_on_push: Optional[bool] = None,
                  require_code_owner_review: Optional[bool] = None,
                  require_last_push_approval: Optional[bool] = None,
                  required_approving_review_count: Optional[int] = None,
                  required_review_thread_resolution: Optional[bool] = None):
         """
-        :param bool dismiss_stale_reviews_on_push: (Boolean) New, reviewable commits pushed will dismiss previous pull request review approvals. Defaults to `false`.
-        :param bool require_code_owner_review: (Boolean) Require an approving review in pull requests that modify files that have a designated code owner. Defaults to `false`.
-        :param bool require_last_push_approval: (Boolean) Whether the most recent reviewable push must be approved by someone other than the person who pushed it. Defaults to `false`.
-        :param int required_approving_review_count: (Number) The number of approving reviews that are required before a pull request can be merged. Defaults to `0`.
-        :param bool required_review_thread_resolution: (Boolean) All conversations on code must be resolved before a pull request can be merged. Defaults to `false`.
+        :param bool dismiss_stale_reviews_on_push: New, reviewable commits pushed will dismiss previous pull request review approvals. Defaults to `false`.
+        :param bool require_code_owner_review: Require an approving review in pull requests that modify files that have a designated code owner. Defaults to `false`.
+        :param bool require_last_push_approval: Whether the most recent reviewable push must be approved by someone other than the person who pushed it. Defaults to `false`.
+        :param int required_approving_review_count: The number of approving reviews that are required before a pull request can be merged. Defaults to `0`.
+        :param bool required_review_thread_resolution: All conversations on code must be resolved before a pull request can be merged. Defaults to `false`.
         """
         if dismiss_stale_reviews_on_push is not None:
             pulumi.set(__self__, "dismiss_stale_reviews_on_push", dismiss_stale_reviews_on_push)
         if require_code_owner_review is not None:
             pulumi.set(__self__, "require_code_owner_review", require_code_owner_review)
         if require_last_push_approval is not None:
             pulumi.set(__self__, "require_last_push_approval", require_last_push_approval)
@@ -1633,47 +1633,47 @@
         if required_review_thread_resolution is not None:
             pulumi.set(__self__, "required_review_thread_resolution", required_review_thread_resolution)
 
     @property
     @pulumi.getter(name="dismissStaleReviewsOnPush")
     def dismiss_stale_reviews_on_push(self) -> Optional[bool]:
         """
-        (Boolean) New, reviewable commits pushed will dismiss previous pull request review approvals. Defaults to `false`.
+        New, reviewable commits pushed will dismiss previous pull request review approvals. Defaults to `false`.
         """
         return pulumi.get(self, "dismiss_stale_reviews_on_push")
 
     @property
     @pulumi.getter(name="requireCodeOwnerReview")
     def require_code_owner_review(self) -> Optional[bool]:
         """
-        (Boolean) Require an approving review in pull requests that modify files that have a designated code owner. Defaults to `false`.
+        Require an approving review in pull requests that modify files that have a designated code owner. Defaults to `false`.
         """
         return pulumi.get(self, "require_code_owner_review")
 
     @property
     @pulumi.getter(name="requireLastPushApproval")
     def require_last_push_approval(self) -> Optional[bool]:
         """
-        (Boolean) Whether the most recent reviewable push must be approved by someone other than the person who pushed it. Defaults to `false`.
+        Whether the most recent reviewable push must be approved by someone other than the person who pushed it. Defaults to `false`.
         """
         return pulumi.get(self, "require_last_push_approval")
 
     @property
     @pulumi.getter(name="requiredApprovingReviewCount")
     def required_approving_review_count(self) -> Optional[int]:
         """
-        (Number) The number of approving reviews that are required before a pull request can be merged. Defaults to `0`.
+        The number of approving reviews that are required before a pull request can be merged. Defaults to `0`.
         """
         return pulumi.get(self, "required_approving_review_count")
 
     @property
     @pulumi.getter(name="requiredReviewThreadResolution")
     def required_review_thread_resolution(self) -> Optional[bool]:
         """
-        (Boolean) All conversations on code must be resolved before a pull request can be merged. Defaults to `false`.
+        All conversations on code must be resolved before a pull request can be merged. Defaults to `false`.
         """
         return pulumi.get(self, "required_review_thread_resolution")
 
 
 @pulumi.output_type
 class OrganizationRulesetRulesRequiredStatusChecks(dict):
     @staticmethod
@@ -1695,34 +1695,34 @@
         OrganizationRulesetRulesRequiredStatusChecks.__key_warning(key)
         return super().get(key, default)
 
     def __init__(__self__, *,
                  required_checks: Sequence['outputs.OrganizationRulesetRulesRequiredStatusChecksRequiredCheck'],
                  strict_required_status_checks_policy: Optional[bool] = None):
         """
-        :param Sequence['OrganizationRulesetRulesRequiredStatusChecksRequiredCheckArgs'] required_checks: (Block Set, Min: 1) Status checks that are required. Several can be defined. (see below for nested schema)
-        :param bool strict_required_status_checks_policy: (Boolean) Whether pull requests targeting a matching branch must be tested with the latest code. This setting will not take effect unless at least one status check is enabled. Defaults to `false`.
+        :param Sequence['OrganizationRulesetRulesRequiredStatusChecksRequiredCheckArgs'] required_checks: Status checks that are required. Several can be defined.
+        :param bool strict_required_status_checks_policy: Whether pull requests targeting a matching branch must be tested with the latest code. This setting will not take effect unless at least one status check is enabled. Defaults to `false`.
         """
         pulumi.set(__self__, "required_checks", required_checks)
         if strict_required_status_checks_policy is not None:
             pulumi.set(__self__, "strict_required_status_checks_policy", strict_required_status_checks_policy)
 
     @property
     @pulumi.getter(name="requiredChecks")
     def required_checks(self) -> Sequence['outputs.OrganizationRulesetRulesRequiredStatusChecksRequiredCheck']:
         """
-        (Block Set, Min: 1) Status checks that are required. Several can be defined. (see below for nested schema)
+        Status checks that are required. Several can be defined.
         """
         return pulumi.get(self, "required_checks")
 
     @property
     @pulumi.getter(name="strictRequiredStatusChecksPolicy")
     def strict_required_status_checks_policy(self) -> Optional[bool]:
         """
-        (Boolean) Whether pull requests targeting a matching branch must be tested with the latest code. This setting will not take effect unless at least one status check is enabled. Defaults to `false`.
+        Whether pull requests targeting a matching branch must be tested with the latest code. This setting will not take effect unless at least one status check is enabled. Defaults to `false`.
         """
         return pulumi.get(self, "strict_required_status_checks_policy")
 
 
 @pulumi.output_type
 class OrganizationRulesetRulesRequiredStatusChecksRequiredCheck(dict):
     @staticmethod
@@ -1742,34 +1742,34 @@
         OrganizationRulesetRulesRequiredStatusChecksRequiredCheck.__key_warning(key)
         return super().get(key, default)
 
     def __init__(__self__, *,
                  context: str,
                  integration_id: Optional[int] = None):
         """
-        :param str context: (String) The status check context name that must be present on the commit.
-        :param int integration_id: (Number) The optional integration ID that this status check must originate from.
+        :param str context: The status check context name that must be present on the commit.
+        :param int integration_id: The optional integration ID that this status check must originate from.
         """
         pulumi.set(__self__, "context", context)
         if integration_id is not None:
             pulumi.set(__self__, "integration_id", integration_id)
 
     @property
     @pulumi.getter
     def context(self) -> str:
         """
-        (String) The status check context name that must be present on the commit.
+        The status check context name that must be present on the commit.
         """
         return pulumi.get(self, "context")
 
     @property
     @pulumi.getter(name="integrationId")
     def integration_id(self) -> Optional[int]:
         """
-        (Number) The optional integration ID that this status check must originate from.
+        The optional integration ID that this status check must originate from.
         """
         return pulumi.get(self, "integration_id")
 
 
 @pulumi.output_type
 class OrganizationRulesetRulesRequiredWorkflows(dict):
     @staticmethod
@@ -1788,23 +1788,23 @@
     def get(self, key: str, default = None) -> Any:
         OrganizationRulesetRulesRequiredWorkflows.__key_warning(key)
         return super().get(key, default)
 
     def __init__(__self__, *,
                  required_workflows: Sequence['outputs.OrganizationRulesetRulesRequiredWorkflowsRequiredWorkflow']):
         """
-        :param Sequence['OrganizationRulesetRulesRequiredWorkflowsRequiredWorkflowArgs'] required_workflows: (Block Set, Min: 1) Actions workflows that are required. Multiple can be defined. (see below for nested schema)
+        :param Sequence['OrganizationRulesetRulesRequiredWorkflowsRequiredWorkflowArgs'] required_workflows: Actions workflows that are required. Several can be defined.
         """
         pulumi.set(__self__, "required_workflows", required_workflows)
 
     @property
     @pulumi.getter(name="requiredWorkflows")
     def required_workflows(self) -> Sequence['outputs.OrganizationRulesetRulesRequiredWorkflowsRequiredWorkflow']:
         """
-        (Block Set, Min: 1) Actions workflows that are required. Multiple can be defined. (see below for nested schema)
+        Actions workflows that are required. Several can be defined.
         """
         return pulumi.get(self, "required_workflows")
 
 
 @pulumi.output_type
 class OrganizationRulesetRulesRequiredWorkflowsRequiredWorkflow(dict):
     @staticmethod
@@ -1825,81 +1825,81 @@
         return super().get(key, default)
 
     def __init__(__self__, *,
                  path: str,
                  repository_id: int,
                  ref: Optional[str] = None):
         """
-        :param str path: (String) The path to the YAML definition file of the workflow.
-        :param int repository_id: The repository IDs that the ruleset applies to. One of these IDs must match for the condition to pass. Conflicts with `repository_name`.
-        :param str ref: (String) The optional ref from which to fetch the workflow. Defaults to `master`.
+        :param str path: The path to the workflow YAML definition file.
+        :param int repository_id: The repository in which the workflow is defined.
+        :param str ref: The ref (branch or tag) of the workflow file to use.
         """
         pulumi.set(__self__, "path", path)
         pulumi.set(__self__, "repository_id", repository_id)
         if ref is not None:
             pulumi.set(__self__, "ref", ref)
 
     @property
     @pulumi.getter
     def path(self) -> str:
         """
-        (String) The path to the YAML definition file of the workflow.
+        The path to the workflow YAML definition file.
         """
         return pulumi.get(self, "path")
 
     @property
     @pulumi.getter(name="repositoryId")
     def repository_id(self) -> int:
         """
-        The repository IDs that the ruleset applies to. One of these IDs must match for the condition to pass. Conflicts with `repository_name`.
+        The repository in which the workflow is defined.
         """
         return pulumi.get(self, "repository_id")
 
     @property
     @pulumi.getter
     def ref(self) -> Optional[str]:
         """
-        (String) The optional ref from which to fetch the workflow. Defaults to `master`.
+        The ref (branch or tag) of the workflow file to use.
         """
         return pulumi.get(self, "ref")
 
 
 @pulumi.output_type
 class OrganizationRulesetRulesTagNamePattern(dict):
     def __init__(__self__, *,
                  operator: str,
                  pattern: str,
                  name: Optional[str] = None,
                  negate: Optional[bool] = None):
         """
-        :param str operator: (String) The operator to use for matching. Can be one of: `starts_with`, `ends_with`, `contains`, `regex`.
-        :param str pattern: (String) The pattern to match with.
+        :param str operator: The operator to use for matching. Can be one of: `starts_with`, `ends_with`, `contains`, `regex`.
+        :param str pattern: The pattern to match with.
         :param str name: (String) The name of the ruleset.
-        :param bool negate: (Boolean) If true, the rule will fail if the pattern matches.
+        :param bool negate: If true, the rule will fail if the pattern matches.
         """
         pulumi.set(__self__, "operator", operator)
         pulumi.set(__self__, "pattern", pattern)
         if name is not None:
             pulumi.set(__self__, "name", name)
         if negate is not None:
             pulumi.set(__self__, "negate", negate)
 
     @property
     @pulumi.getter
     def operator(self) -> str:
         """
-        (String) The operator to use for matching. Can be one of: `starts_with`, `ends_with`, `contains`, `regex`.
+        The operator to use for matching. Can be one of: `starts_with`, `ends_with`, `contains`, `regex`.
         """
         return pulumi.get(self, "operator")
 
     @property
     @pulumi.getter
     def pattern(self) -> str:
         """
-        (String) The pattern to match with.
+        The pattern to match with.
         """
         return pulumi.get(self, "pattern")
 
     @property
     @pulumi.getter
     def name(self) -> Optional[str]:
         """
@@ -1907,15 +1907,15 @@
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter
     def negate(self) -> Optional[bool]:
         """
-        (Boolean) If true, the rule will fail if the pattern matches.
+        If true, the rule will fail if the pattern matches.
         """
         return pulumi.get(self, "negate")
 
 
 @pulumi.output_type
 class OrganizationWebhookConfiguration(dict):
     @staticmethod
@@ -2184,15 +2184,15 @@
                  url: Optional[str] = None):
         """
         :param str build_type: The type of GitHub Pages site to build. Can be `legacy` or `workflow`. If you use `legacy` as build type you need to set the option `source`.
         :param str cname: The custom domain for the repository. This can only be set after the repository has been created.
         :param bool custom404: Whether the rendered GitHub Pages site has a custom 404 page.
         :param str html_url: The absolute URL (including scheme) of the rendered GitHub Pages site e.g. `https://username.github.io`.
         :param 'RepositoryPagesSourceArgs' source: The source branch and directory for the rendered Pages site. See GitHub Pages Source below for details.
-        :param str status: Set to `enabled` to enable advanced security features on the repository. Can be `enabled` or `disabled`.
+        :param str status: The GitHub Pages site's build status e.g. `building` or `built`.
         """
         if build_type is not None:
             pulumi.set(__self__, "build_type", build_type)
         if cname is not None:
             pulumi.set(__self__, "cname", cname)
         if custom404 is not None:
             pulumi.set(__self__, "custom404", custom404)
@@ -2245,15 +2245,15 @@
         """
         return pulumi.get(self, "source")
 
     @property
     @pulumi.getter
     def status(self) -> Optional[str]:
         """
-        Set to `enabled` to enable advanced security features on the repository. Can be `enabled` or `disabled`.
+        The GitHub Pages site's build status e.g. `building` or `built`.
         """
         return pulumi.get(self, "status")
 
     @property
     @pulumi.getter
     def url(self) -> Optional[str]:
         return pulumi.get(self, "url")
@@ -2391,33 +2391,33 @@
 
 @pulumi.output_type
 class RepositoryRulesetConditionsRefName(dict):
     def __init__(__self__, *,
                  excludes: Sequence[str],
                  includes: Sequence[str]):
         """
-        :param Sequence[str] excludes: (List of String) Array of ref names or patterns to exclude. The condition will not pass if any of these patterns match.
-        :param Sequence[str] includes: (List of String) Array of ref names or patterns to include. One of these patterns must match for the condition to pass. Also accepts `~DEFAULT_BRANCH` to include the default branch or `~ALL` to include all branches.
+        :param Sequence[str] excludes: Array of ref names or patterns to exclude. The condition will not pass if any of these patterns match.
+        :param Sequence[str] includes: Array of ref names or patterns to include. One of these patterns must match for the condition to pass. Also accepts `~DEFAULT_BRANCH` to include the default branch or `~ALL` to include all branches.
         """
         pulumi.set(__self__, "excludes", excludes)
         pulumi.set(__self__, "includes", includes)
 
     @property
     @pulumi.getter
     def excludes(self) -> Sequence[str]:
         """
-        (List of String) Array of ref names or patterns to exclude. The condition will not pass if any of these patterns match.
+        Array of ref names or patterns to exclude. The condition will not pass if any of these patterns match.
         """
         return pulumi.get(self, "excludes")
 
     @property
     @pulumi.getter
     def includes(self) -> Sequence[str]:
         """
-        (List of String) Array of ref names or patterns to include. One of these patterns must match for the condition to pass. Also accepts `~DEFAULT_BRANCH` to include the default branch or `~ALL` to include all branches.
+        Array of ref names or patterns to include. One of these patterns must match for the condition to pass. Also accepts `~DEFAULT_BRANCH` to include the default branch or `~ALL` to include all branches.
         """
         return pulumi.get(self, "includes")
 
 
 @pulumi.output_type
 class RepositoryRulesetRules(dict):
     @staticmethod
@@ -2648,39 +2648,39 @@
 class RepositoryRulesetRulesBranchNamePattern(dict):
     def __init__(__self__, *,
                  operator: str,
                  pattern: str,
                  name: Optional[str] = None,
                  negate: Optional[bool] = None):
         """
-        :param str operator: (String) The operator to use for matching. Can be one of: `starts_with`, `ends_with`, `contains`, `regex`.
-        :param str pattern: (String) The pattern to match with.
+        :param str operator: The operator to use for matching. Can be one of: `starts_with`, `ends_with`, `contains`, `regex`.
+        :param str pattern: The pattern to match with.
         :param str name: (String) The name of the ruleset.
-        :param bool negate: (Boolean) If true, the rule will fail if the pattern matches.
+        :param bool negate: If true, the rule will fail if the pattern matches.
         """
         pulumi.set(__self__, "operator", operator)
         pulumi.set(__self__, "pattern", pattern)
         if name is not None:
             pulumi.set(__self__, "name", name)
         if negate is not None:
             pulumi.set(__self__, "negate", negate)
 
     @property
     @pulumi.getter
     def operator(self) -> str:
         """
-        (String) The operator to use for matching. Can be one of: `starts_with`, `ends_with`, `contains`, `regex`.
+        The operator to use for matching. Can be one of: `starts_with`, `ends_with`, `contains`, `regex`.
         """
         return pulumi.get(self, "operator")
 
     @property
     @pulumi.getter
     def pattern(self) -> str:
         """
-        (String) The pattern to match with.
+        The pattern to match with.
         """
         return pulumi.get(self, "pattern")
 
     @property
     @pulumi.getter
     def name(self) -> Optional[str]:
         """
@@ -2688,52 +2688,52 @@
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter
     def negate(self) -> Optional[bool]:
         """
-        (Boolean) If true, the rule will fail if the pattern matches.
+        If true, the rule will fail if the pattern matches.
         """
         return pulumi.get(self, "negate")
 
 
 @pulumi.output_type
 class RepositoryRulesetRulesCommitAuthorEmailPattern(dict):
     def __init__(__self__, *,
                  operator: str,
                  pattern: str,
                  name: Optional[str] = None,
                  negate: Optional[bool] = None):
         """
-        :param str operator: (String) The operator to use for matching. Can be one of: `starts_with`, `ends_with`, `contains`, `regex`.
-        :param str pattern: (String) The pattern to match with.
+        :param str operator: The operator to use for matching. Can be one of: `starts_with`, `ends_with`, `contains`, `regex`.
+        :param str pattern: The pattern to match with.
         :param str name: (String) The name of the ruleset.
-        :param bool negate: (Boolean) If true, the rule will fail if the pattern matches.
+        :param bool negate: If true, the rule will fail if the pattern matches.
         """
         pulumi.set(__self__, "operator", operator)
         pulumi.set(__self__, "pattern", pattern)
         if name is not None:
             pulumi.set(__self__, "name", name)
         if negate is not None:
             pulumi.set(__self__, "negate", negate)
 
     @property
     @pulumi.getter
     def operator(self) -> str:
         """
-        (String) The operator to use for matching. Can be one of: `starts_with`, `ends_with`, `contains`, `regex`.
+        The operator to use for matching. Can be one of: `starts_with`, `ends_with`, `contains`, `regex`.
         """
         return pulumi.get(self, "operator")
 
     @property
     @pulumi.getter
     def pattern(self) -> str:
         """
-        (String) The pattern to match with.
+        The pattern to match with.
         """
         return pulumi.get(self, "pattern")
 
     @property
     @pulumi.getter
     def name(self) -> Optional[str]:
         """
@@ -2741,52 +2741,52 @@
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter
     def negate(self) -> Optional[bool]:
         """
-        (Boolean) If true, the rule will fail if the pattern matches.
+        If true, the rule will fail if the pattern matches.
         """
         return pulumi.get(self, "negate")
 
 
 @pulumi.output_type
 class RepositoryRulesetRulesCommitMessagePattern(dict):
     def __init__(__self__, *,
                  operator: str,
                  pattern: str,
                  name: Optional[str] = None,
                  negate: Optional[bool] = None):
         """
-        :param str operator: (String) The operator to use for matching. Can be one of: `starts_with`, `ends_with`, `contains`, `regex`.
-        :param str pattern: (String) The pattern to match with.
+        :param str operator: The operator to use for matching. Can be one of: `starts_with`, `ends_with`, `contains`, `regex`.
+        :param str pattern: The pattern to match with.
         :param str name: (String) The name of the ruleset.
-        :param bool negate: (Boolean) If true, the rule will fail if the pattern matches.
+        :param bool negate: If true, the rule will fail if the pattern matches.
         """
         pulumi.set(__self__, "operator", operator)
         pulumi.set(__self__, "pattern", pattern)
         if name is not None:
             pulumi.set(__self__, "name", name)
         if negate is not None:
             pulumi.set(__self__, "negate", negate)
 
     @property
     @pulumi.getter
     def operator(self) -> str:
         """
-        (String) The operator to use for matching. Can be one of: `starts_with`, `ends_with`, `contains`, `regex`.
+        The operator to use for matching. Can be one of: `starts_with`, `ends_with`, `contains`, `regex`.
         """
         return pulumi.get(self, "operator")
 
     @property
     @pulumi.getter
     def pattern(self) -> str:
         """
-        (String) The pattern to match with.
+        The pattern to match with.
         """
         return pulumi.get(self, "pattern")
 
     @property
     @pulumi.getter
     def name(self) -> Optional[str]:
         """
@@ -2794,52 +2794,52 @@
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter
     def negate(self) -> Optional[bool]:
         """
-        (Boolean) If true, the rule will fail if the pattern matches.
+        If true, the rule will fail if the pattern matches.
         """
         return pulumi.get(self, "negate")
 
 
 @pulumi.output_type
 class RepositoryRulesetRulesCommitterEmailPattern(dict):
     def __init__(__self__, *,
                  operator: str,
                  pattern: str,
                  name: Optional[str] = None,
                  negate: Optional[bool] = None):
         """
-        :param str operator: (String) The operator to use for matching. Can be one of: `starts_with`, `ends_with`, `contains`, `regex`.
-        :param str pattern: (String) The pattern to match with.
+        :param str operator: The operator to use for matching. Can be one of: `starts_with`, `ends_with`, `contains`, `regex`.
+        :param str pattern: The pattern to match with.
         :param str name: (String) The name of the ruleset.
-        :param bool negate: (Boolean) If true, the rule will fail if the pattern matches.
+        :param bool negate: If true, the rule will fail if the pattern matches.
         """
         pulumi.set(__self__, "operator", operator)
         pulumi.set(__self__, "pattern", pattern)
         if name is not None:
             pulumi.set(__self__, "name", name)
         if negate is not None:
             pulumi.set(__self__, "negate", negate)
 
     @property
     @pulumi.getter
     def operator(self) -> str:
         """
-        (String) The operator to use for matching. Can be one of: `starts_with`, `ends_with`, `contains`, `regex`.
+        The operator to use for matching. Can be one of: `starts_with`, `ends_with`, `contains`, `regex`.
         """
         return pulumi.get(self, "operator")
 
     @property
     @pulumi.getter
     def pattern(self) -> str:
         """
-        (String) The pattern to match with.
+        The pattern to match with.
         """
         return pulumi.get(self, "pattern")
 
     @property
     @pulumi.getter
     def name(self) -> Optional[str]:
         """
@@ -2847,15 +2847,15 @@
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter
     def negate(self) -> Optional[bool]:
         """
-        (Boolean) If true, the rule will fail if the pattern matches.
+        If true, the rule will fail if the pattern matches.
         """
         return pulumi.get(self, "negate")
 
 
 @pulumi.output_type
 class RepositoryRulesetRulesPullRequest(dict):
     @staticmethod
@@ -2886,19 +2886,19 @@
     def __init__(__self__, *,
                  dismiss_stale_reviews_on_push: Optional[bool] = None,
                  require_code_owner_review: Optional[bool] = None,
                  require_last_push_approval: Optional[bool] = None,
                  required_approving_review_count: Optional[int] = None,
                  required_review_thread_resolution: Optional[bool] = None):
         """
-        :param bool dismiss_stale_reviews_on_push: (Boolean) New, reviewable commits pushed will dismiss previous pull request review approvals. Defaults to `false`.
-        :param bool require_code_owner_review: (Boolean) Require an approving review in pull requests that modify files that have a designated code owner. Defaults to `false`.
-        :param bool require_last_push_approval: (Boolean) Whether the most recent reviewable push must be approved by someone other than the person who pushed it. Defaults to `false`.
-        :param int required_approving_review_count: (Number) The number of approving reviews that are required before a pull request can be merged. Defaults to `0`.
-        :param bool required_review_thread_resolution: (Boolean) All conversations on code must be resolved before a pull request can be merged. Defaults to `false`.
+        :param bool dismiss_stale_reviews_on_push: New, reviewable commits pushed will dismiss previous pull request review approvals. Defaults to `false`.
+        :param bool require_code_owner_review: Require an approving review in pull requests that modify files that have a designated code owner. Defaults to `false`.
+        :param bool require_last_push_approval: Whether the most recent reviewable push must be approved by someone other than the person who pushed it. Defaults to `false`.
+        :param int required_approving_review_count: The number of approving reviews that are required before a pull request can be merged. Defaults to `0`.
+        :param bool required_review_thread_resolution: All conversations on code must be resolved before a pull request can be merged. Defaults to `false`.
         """
         if dismiss_stale_reviews_on_push is not None:
             pulumi.set(__self__, "dismiss_stale_reviews_on_push", dismiss_stale_reviews_on_push)
         if require_code_owner_review is not None:
             pulumi.set(__self__, "require_code_owner_review", require_code_owner_review)
         if require_last_push_approval is not None:
             pulumi.set(__self__, "require_last_push_approval", require_last_push_approval)
@@ -2907,47 +2907,47 @@
         if required_review_thread_resolution is not None:
             pulumi.set(__self__, "required_review_thread_resolution", required_review_thread_resolution)
 
     @property
     @pulumi.getter(name="dismissStaleReviewsOnPush")
     def dismiss_stale_reviews_on_push(self) -> Optional[bool]:
         """
-        (Boolean) New, reviewable commits pushed will dismiss previous pull request review approvals. Defaults to `false`.
+        New, reviewable commits pushed will dismiss previous pull request review approvals. Defaults to `false`.
         """
         return pulumi.get(self, "dismiss_stale_reviews_on_push")
 
     @property
     @pulumi.getter(name="requireCodeOwnerReview")
     def require_code_owner_review(self) -> Optional[bool]:
         """
-        (Boolean) Require an approving review in pull requests that modify files that have a designated code owner. Defaults to `false`.
+        Require an approving review in pull requests that modify files that have a designated code owner. Defaults to `false`.
         """
         return pulumi.get(self, "require_code_owner_review")
 
     @property
     @pulumi.getter(name="requireLastPushApproval")
     def require_last_push_approval(self) -> Optional[bool]:
         """
-        (Boolean) Whether the most recent reviewable push must be approved by someone other than the person who pushed it. Defaults to `false`.
+        Whether the most recent reviewable push must be approved by someone other than the person who pushed it. Defaults to `false`.
         """
         return pulumi.get(self, "require_last_push_approval")
 
     @property
     @pulumi.getter(name="requiredApprovingReviewCount")
     def required_approving_review_count(self) -> Optional[int]:
         """
-        (Number) The number of approving reviews that are required before a pull request can be merged. Defaults to `0`.
+        The number of approving reviews that are required before a pull request can be merged. Defaults to `0`.
         """
         return pulumi.get(self, "required_approving_review_count")
 
     @property
     @pulumi.getter(name="requiredReviewThreadResolution")
     def required_review_thread_resolution(self) -> Optional[bool]:
         """
-        (Boolean) All conversations on code must be resolved before a pull request can be merged. Defaults to `false`.
+        All conversations on code must be resolved before a pull request can be merged. Defaults to `false`.
         """
         return pulumi.get(self, "required_review_thread_resolution")
 
 
 @pulumi.output_type
 class RepositoryRulesetRulesRequiredDeployments(dict):
     @staticmethod
@@ -2966,23 +2966,23 @@
     def get(self, key: str, default = None) -> Any:
         RepositoryRulesetRulesRequiredDeployments.__key_warning(key)
         return super().get(key, default)
 
     def __init__(__self__, *,
                  required_deployment_environments: Sequence[str]):
         """
-        :param Sequence[str] required_deployment_environments: (List of String) The environments that must be successfully deployed to before branches can be merged.
+        :param Sequence[str] required_deployment_environments: The environments that must be successfully deployed to before branches can be merged.
         """
         pulumi.set(__self__, "required_deployment_environments", required_deployment_environments)
 
     @property
     @pulumi.getter(name="requiredDeploymentEnvironments")
     def required_deployment_environments(self) -> Sequence[str]:
         """
-        (List of String) The environments that must be successfully deployed to before branches can be merged.
+        The environments that must be successfully deployed to before branches can be merged.
         """
         return pulumi.get(self, "required_deployment_environments")
 
 
 @pulumi.output_type
 class RepositoryRulesetRulesRequiredStatusChecks(dict):
     @staticmethod
@@ -3004,34 +3004,34 @@
         RepositoryRulesetRulesRequiredStatusChecks.__key_warning(key)
         return super().get(key, default)
 
     def __init__(__self__, *,
                  required_checks: Sequence['outputs.RepositoryRulesetRulesRequiredStatusChecksRequiredCheck'],
                  strict_required_status_checks_policy: Optional[bool] = None):
         """
-        :param Sequence['RepositoryRulesetRulesRequiredStatusChecksRequiredCheckArgs'] required_checks: (Block Set, Min: 1) Status checks that are required. Several can be defined. (see below for nested schema)
-        :param bool strict_required_status_checks_policy: (Boolean) Whether pull requests targeting a matching branch must be tested with the latest code. This setting will not take effect unless at least one status check is enabled. Defaults to `false`.
+        :param Sequence['RepositoryRulesetRulesRequiredStatusChecksRequiredCheckArgs'] required_checks: Status checks that are required. Several can be defined.
+        :param bool strict_required_status_checks_policy: Whether pull requests targeting a matching branch must be tested with the latest code. This setting will not take effect unless at least one status check is enabled. Defaults to `false`.
         """
         pulumi.set(__self__, "required_checks", required_checks)
         if strict_required_status_checks_policy is not None:
             pulumi.set(__self__, "strict_required_status_checks_policy", strict_required_status_checks_policy)
 
     @property
     @pulumi.getter(name="requiredChecks")
     def required_checks(self) -> Sequence['outputs.RepositoryRulesetRulesRequiredStatusChecksRequiredCheck']:
         """
-        (Block Set, Min: 1) Status checks that are required. Several can be defined. (see below for nested schema)
+        Status checks that are required. Several can be defined.
         """
         return pulumi.get(self, "required_checks")
 
     @property
     @pulumi.getter(name="strictRequiredStatusChecksPolicy")
     def strict_required_status_checks_policy(self) -> Optional[bool]:
         """
-        (Boolean) Whether pull requests targeting a matching branch must be tested with the latest code. This setting will not take effect unless at least one status check is enabled. Defaults to `false`.
+        Whether pull requests targeting a matching branch must be tested with the latest code. This setting will not take effect unless at least one status check is enabled. Defaults to `false`.
         """
         return pulumi.get(self, "strict_required_status_checks_policy")
 
 
 @pulumi.output_type
 class RepositoryRulesetRulesRequiredStatusChecksRequiredCheck(dict):
     @staticmethod
@@ -3051,71 +3051,71 @@
         RepositoryRulesetRulesRequiredStatusChecksRequiredCheck.__key_warning(key)
         return super().get(key, default)
 
     def __init__(__self__, *,
                  context: str,
                  integration_id: Optional[int] = None):
         """
-        :param str context: (String) The status check context name that must be present on the commit.
-        :param int integration_id: (Number) The optional integration ID that this status check must originate from.
+        :param str context: The status check context name that must be present on the commit.
+        :param int integration_id: The optional integration ID that this status check must originate from.
         """
         pulumi.set(__self__, "context", context)
         if integration_id is not None:
             pulumi.set(__self__, "integration_id", integration_id)
 
     @property
     @pulumi.getter
     def context(self) -> str:
         """
-        (String) The status check context name that must be present on the commit.
+        The status check context name that must be present on the commit.
         """
         return pulumi.get(self, "context")
 
     @property
     @pulumi.getter(name="integrationId")
     def integration_id(self) -> Optional[int]:
         """
-        (Number) The optional integration ID that this status check must originate from.
+        The optional integration ID that this status check must originate from.
         """
         return pulumi.get(self, "integration_id")
 
 
 @pulumi.output_type
 class RepositoryRulesetRulesTagNamePattern(dict):
     def __init__(__self__, *,
                  operator: str,
                  pattern: str,
                  name: Optional[str] = None,
                  negate: Optional[bool] = None):
         """
-        :param str operator: (String) The operator to use for matching. Can be one of: `starts_with`, `ends_with`, `contains`, `regex`.
-        :param str pattern: (String) The pattern to match with.
+        :param str operator: The operator to use for matching. Can be one of: `starts_with`, `ends_with`, `contains`, `regex`.
+        :param str pattern: The pattern to match with.
         :param str name: (String) The name of the ruleset.
-        :param bool negate: (Boolean) If true, the rule will fail if the pattern matches.
+        :param bool negate: If true, the rule will fail if the pattern matches.
         """
         pulumi.set(__self__, "operator", operator)
         pulumi.set(__self__, "pattern", pattern)
         if name is not None:
             pulumi.set(__self__, "name", name)
         if negate is not None:
             pulumi.set(__self__, "negate", negate)
 
     @property
     @pulumi.getter
     def operator(self) -> str:
         """
-        (String) The operator to use for matching. Can be one of: `starts_with`, `ends_with`, `contains`, `regex`.
+        The operator to use for matching. Can be one of: `starts_with`, `ends_with`, `contains`, `regex`.
         """
         return pulumi.get(self, "operator")
 
     @property
     @pulumi.getter
     def pattern(self) -> str:
         """
-        (String) The pattern to match with.
+        The pattern to match with.
         """
         return pulumi.get(self, "pattern")
 
     @property
     @pulumi.getter
     def name(self) -> Optional[str]:
         """
@@ -3123,15 +3123,15 @@
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter
     def negate(self) -> Optional[bool]:
         """
-        (Boolean) If true, the rule will fail if the pattern matches.
+        If true, the rule will fail if the pattern matches.
         """
         return pulumi.get(self, "negate")
 
 
 @pulumi.output_type
 class RepositorySecurityAndAnalysis(dict):
     @staticmethod
@@ -3215,41 +3215,41 @@
 
 
 @pulumi.output_type
 class RepositorySecurityAndAnalysisSecretScanning(dict):
     def __init__(__self__, *,
                  status: str):
         """
-        :param str status: Set to `enabled` to enable advanced security features on the repository. Can be `enabled` or `disabled`.
+        :param str status: The GitHub Pages site's build status e.g. `building` or `built`.
         """
         pulumi.set(__self__, "status", status)
 
     @property
     @pulumi.getter
     def status(self) -> str:
         """
-        Set to `enabled` to enable advanced security features on the repository. Can be `enabled` or `disabled`.
+        The GitHub Pages site's build status e.g. `building` or `built`.
         """
         return pulumi.get(self, "status")
 
 
 @pulumi.output_type
 class RepositorySecurityAndAnalysisSecretScanningPushProtection(dict):
     def __init__(__self__, *,
                  status: str):
         """
-        :param str status: Set to `enabled` to enable advanced security features on the repository. Can be `enabled` or `disabled`.
+        :param str status: The GitHub Pages site's build status e.g. `building` or `built`.
         """
         pulumi.set(__self__, "status", status)
 
     @property
     @pulumi.getter
     def status(self) -> str:
         """
-        Set to `enabled` to enable advanced security features on the repository. Can be `enabled` or `disabled`.
+        The GitHub Pages site's build status e.g. `building` or `built`.
         """
         return pulumi.get(self, "status")
 
 
 @pulumi.output_type
 class RepositoryTemplate(dict):
     @staticmethod
@@ -3433,46 +3433,46 @@
         return super().get(key, default)
 
     def __init__(__self__, *,
                  algorithm: Optional[str] = None,
                  member_count: Optional[int] = None,
                  notify: Optional[bool] = None):
         """
-        :param str algorithm: The algorithm to use when assigning pull requests to team members. Supported values are `ROUND_ROBIN` and `LOAD_BALANCE`. Default value is `ROUND_ROBIN`
-        :param int member_count: The number of team members to assign to a pull request
-        :param bool notify: whether to notify the entire team when at least one member is also assigned to the pull request
+        :param str algorithm: The algorithm to use when assigning pull requests to team members. Supported values are 'ROUND_ROBIN' and 'LOAD_BALANCE'.
+        :param int member_count: The number of team members to assign to a pull request.
+        :param bool notify: whether to notify the entire team when at least one member is also assigned to the pull request.
         """
         if algorithm is not None:
             pulumi.set(__self__, "algorithm", algorithm)
         if member_count is not None:
             pulumi.set(__self__, "member_count", member_count)
         if notify is not None:
             pulumi.set(__self__, "notify", notify)
 
     @property
     @pulumi.getter
     def algorithm(self) -> Optional[str]:
         """
-        The algorithm to use when assigning pull requests to team members. Supported values are `ROUND_ROBIN` and `LOAD_BALANCE`. Default value is `ROUND_ROBIN`
+        The algorithm to use when assigning pull requests to team members. Supported values are 'ROUND_ROBIN' and 'LOAD_BALANCE'.
         """
         return pulumi.get(self, "algorithm")
 
     @property
     @pulumi.getter(name="memberCount")
     def member_count(self) -> Optional[int]:
         """
-        The number of team members to assign to a pull request
+        The number of team members to assign to a pull request.
         """
         return pulumi.get(self, "member_count")
 
     @property
     @pulumi.getter
     def notify(self) -> Optional[bool]:
         """
-        whether to notify the entire team when at least one member is also assigned to the pull request
+        whether to notify the entire team when at least one member is also assigned to the pull request.
         """
         return pulumi.get(self, "notify")
 
 
 @pulumi.output_type
 class TeamSyncGroupMappingGroup(dict):
     @staticmethod
```

### Comparing `pulumi_github-6.3.0a1713561029/pulumi_github/project_card.py` & `pulumi_github-6.3.0a1713897837/pulumi_github/project_card.py`

 * *Files 2% similar despite different names*

```diff
@@ -205,34 +205,31 @@
                  note: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         This resource allows you to create and manage cards for GitHub projects.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_github as github
 
         project = github.OrganizationProject("project",
             name="An Organization Project",
             body="This is an organization project.")
         column = github.ProjectColumn("column",
             project_id=project.id,
             name="Backlog")
         card = github.ProjectCard("card",
             column_id=column.column_id,
             note="## Unaccepted 👇")
         ```
-        <!--End PulumiCodeChooser -->
 
         ### Adding An Issue To A Project
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_github as github
 
         test = github.Repository("test",
             name="myrepo",
             has_projects=True,
@@ -249,15 +246,14 @@
             project_id=test_repository_project.id,
             name="Backlog")
         test_project_card = github.ProjectCard("test",
             column_id=test_project_column.column_id,
             content_id=test_issue.issue_id,
             content_type="Issue")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         A GitHub Project Card can be imported using its [Card ID](https://developer.github.com/v3/projects/cards/#get-a-project-card):
 
         ```sh
         $ pulumi import github:index/projectCard:ProjectCard card 01234567
@@ -280,34 +276,31 @@
                  args: ProjectCardArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         This resource allows you to create and manage cards for GitHub projects.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_github as github
 
         project = github.OrganizationProject("project",
             name="An Organization Project",
             body="This is an organization project.")
         column = github.ProjectColumn("column",
             project_id=project.id,
             name="Backlog")
         card = github.ProjectCard("card",
             column_id=column.column_id,
             note="## Unaccepted 👇")
         ```
-        <!--End PulumiCodeChooser -->
 
         ### Adding An Issue To A Project
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_github as github
 
         test = github.Repository("test",
             name="myrepo",
             has_projects=True,
@@ -324,15 +317,14 @@
             project_id=test_repository_project.id,
             name="Backlog")
         test_project_card = github.ProjectCard("test",
             column_id=test_project_column.column_id,
             content_id=test_issue.issue_id,
             content_type="Issue")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         A GitHub Project Card can be imported using its [Card ID](https://developer.github.com/v3/projects/cards/#get-a-project-card):
 
         ```sh
         $ pulumi import github:index/projectCard:ProjectCard card 01234567
```

### Comparing `pulumi_github-6.3.0a1713561029/pulumi_github/project_column.py` & `pulumi_github-6.3.0a1713897837/pulumi_github/project_column.py`

 * *Files 2% similar despite different names*

```diff
@@ -127,27 +127,25 @@
                  project_id: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         This resource allows you to create and manage columns for GitHub projects.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_github as github
 
         project = github.OrganizationProject("project",
             name="A Organization Project",
             body="This is an organization project.")
         column = github.ProjectColumn("column",
             project_id=project.id,
             name="a column")
         ```
-        <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] name: The name of the column.
         :param pulumi.Input[str] project_id: The ID of an existing project that the column will be created in.
         """
         ...
@@ -157,27 +155,25 @@
                  args: ProjectColumnArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         This resource allows you to create and manage columns for GitHub projects.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_github as github
 
         project = github.OrganizationProject("project",
             name="A Organization Project",
             body="This is an organization project.")
         column = github.ProjectColumn("column",
             project_id=project.id,
             name="a column")
         ```
-        <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param ProjectColumnArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
```

### Comparing `pulumi_github-6.3.0a1713561029/pulumi_github/provider.py` & `pulumi_github-6.3.0a1713897837/pulumi_github/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-6.3.0a1713561029/pulumi_github/release.py` & `pulumi_github-6.3.0a1713897837/pulumi_github/release.py`

 * *Files 2% similar despite different names*

```diff
@@ -342,32 +342,29 @@
                  __props__=None):
         """
         This resource allows you to create and manage a release in a specific
         GitHub repository.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_github as github
 
         repo = github.Repository("repo",
             name="repo",
             description="GitHub repo managed by Terraform",
             private=False)
         example = github.Release("example",
             repository=repo.name,
             tag_name="v1.0.0")
         ```
-        <!--End PulumiCodeChooser -->
 
         ### On Non-Default Branch
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_github as github
 
         example = github.Repository("example",
             name="repo",
             auto_init=True)
@@ -378,15 +375,14 @@
         example_release = github.Release("example",
             repository=example.name,
             tag_name="v1.0.0",
             target_commitish=example_branch.branch,
             draft=False,
             prerelease=False)
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         This resource can be imported using the `name` of the repository, combined with the `id` of the release, and a `:` character for separating components, e.g.
 
         ```sh
         $ pulumi import github:index/release:Release example repo:12345678
@@ -412,32 +408,29 @@
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         This resource allows you to create and manage a release in a specific
         GitHub repository.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_github as github
 
         repo = github.Repository("repo",
             name="repo",
             description="GitHub repo managed by Terraform",
             private=False)
         example = github.Release("example",
             repository=repo.name,
             tag_name="v1.0.0")
         ```
-        <!--End PulumiCodeChooser -->
 
         ### On Non-Default Branch
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_github as github
 
         example = github.Repository("example",
             name="repo",
             auto_init=True)
@@ -448,15 +441,14 @@
         example_release = github.Release("example",
             repository=example.name,
             tag_name="v1.0.0",
             target_commitish=example_branch.branch,
             draft=False,
             prerelease=False)
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         This resource can be imported using the `name` of the repository, combined with the `id` of the release, and a `:` character for separating components, e.g.
 
         ```sh
         $ pulumi import github:index/release:Release example repo:12345678
```

### Comparing `pulumi_github-6.3.0a1713561029/pulumi_github/repository.py` & `pulumi_github-6.3.0a1713897837/pulumi_github/repository.py`

 * *Files 1% similar despite different names*

```diff
@@ -1363,34 +1363,31 @@
 
         > Note: When used with GitHub App authentication, even GET requests must have
         the `contents:write` permission or else the `allow_merge_commit`, `allow_rebase_merge`,
         and `allow_squash_merge` attributes will be ignored, causing confusing diffs.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_github as github
 
         example = github.Repository("example",
             name="example",
             description="My awesome codebase",
             visibility="public",
             template=github.RepositoryTemplateArgs(
                 owner="github",
                 repository="terraform-template-module",
                 include_all_branches=True,
             ))
         ```
-        <!--End PulumiCodeChooser -->
 
         ### With GitHub Pages Enabled
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_github as github
 
         example = github.Repository("example",
             name="example",
             description="My awesome web page",
@@ -1398,15 +1395,14 @@
             pages=github.RepositoryPagesArgs(
                 source=github.RepositoryPagesSourceArgs(
                     branch="master",
                     path="/docs",
                 ),
             ))
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Repositories can be imported using the `name`, e.g.
 
         ```sh
         $ pulumi import github:index/repository:Repository terraform terraform
@@ -1466,34 +1462,31 @@
 
         > Note: When used with GitHub App authentication, even GET requests must have
         the `contents:write` permission or else the `allow_merge_commit`, `allow_rebase_merge`,
         and `allow_squash_merge` attributes will be ignored, causing confusing diffs.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_github as github
 
         example = github.Repository("example",
             name="example",
             description="My awesome codebase",
             visibility="public",
             template=github.RepositoryTemplateArgs(
                 owner="github",
                 repository="terraform-template-module",
                 include_all_branches=True,
             ))
         ```
-        <!--End PulumiCodeChooser -->
 
         ### With GitHub Pages Enabled
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_github as github
 
         example = github.Repository("example",
             name="example",
             description="My awesome web page",
@@ -1501,15 +1494,14 @@
             pages=github.RepositoryPagesArgs(
                 source=github.RepositoryPagesSourceArgs(
                     branch="master",
                     path="/docs",
                 ),
             ))
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Repositories can be imported using the `name`, e.g.
 
         ```sh
         $ pulumi import github:index/repository:Repository terraform terraform
```

### Comparing `pulumi_github-6.3.0a1713561029/pulumi_github/repository_autolink_reference.py` & `pulumi_github-6.3.0a1713897837/pulumi_github/repository_autolink_reference.py`

 * *Files 1% similar despite different names*

```diff
@@ -179,29 +179,27 @@
                  target_url_template: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         This resource allows you to create and manage an autolink reference for a single repository.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_github as github
 
         repo = github.Repository("repo",
             name="my-repo",
             description="GitHub repo managed by Terraform",
             private=False)
         autolink = github.RepositoryAutolinkReference("autolink",
             repository=repo.name,
             key_prefix="TICKET-",
             target_url_template="https://example.com/TICKET?query=<num>")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         ### Import by key prefix
 
         ```sh
         $ pulumi import github:index/repositoryAutolinkReference:RepositoryAutolinkReference auto oof/OOF-
@@ -221,29 +219,27 @@
                  args: RepositoryAutolinkReferenceArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         This resource allows you to create and manage an autolink reference for a single repository.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_github as github
 
         repo = github.Repository("repo",
             name="my-repo",
             description="GitHub repo managed by Terraform",
             private=False)
         autolink = github.RepositoryAutolinkReference("autolink",
             repository=repo.name,
             key_prefix="TICKET-",
             target_url_template="https://example.com/TICKET?query=<num>")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         ### Import by key prefix
 
         ```sh
         $ pulumi import github:index/repositoryAutolinkReference:RepositoryAutolinkReference auto oof/OOF-
```

### Comparing `pulumi_github-6.3.0a1713561029/pulumi_github/repository_collaborator.py` & `pulumi_github-6.3.0a1713897837/pulumi_github/repository_collaborator.py`

 * *Files 2% similar despite different names*

```diff
@@ -219,26 +219,24 @@
 
         - [Adding outside collaborators to your personal repositories](https://help.github.com/en/github/setting-up-and-managing-your-github-user-account/managing-access-to-your-personal-repositories)
         - [Adding outside collaborators to repositories in your organization](https://help.github.com/articles/adding-outside-collaborators-to-repositories-in-your-organization/)
         - [Converting an organization member to an outside collaborator](https://help.github.com/articles/converting-an-organization-member-to-an-outside-collaborator/)
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_github as github
 
         # Add a collaborator to a repository
         a_repo_collaborator = github.RepositoryCollaborator("a_repo_collaborator",
             repository="our-cool-repo",
             username="SomeUser",
             permission="admin")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         GitHub Repository Collaborators can be imported using an ID made up of `repository:username`, e.g.
 
         ```sh
         $ pulumi import github:index/repositoryCollaborator:RepositoryCollaborator collaborator terraform:someuser
@@ -285,26 +283,24 @@
 
         - [Adding outside collaborators to your personal repositories](https://help.github.com/en/github/setting-up-and-managing-your-github-user-account/managing-access-to-your-personal-repositories)
         - [Adding outside collaborators to repositories in your organization](https://help.github.com/articles/adding-outside-collaborators-to-repositories-in-your-organization/)
         - [Converting an organization member to an outside collaborator](https://help.github.com/articles/converting-an-organization-member-to-an-outside-collaborator/)
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_github as github
 
         # Add a collaborator to a repository
         a_repo_collaborator = github.RepositoryCollaborator("a_repo_collaborator",
             repository="our-cool-repo",
             username="SomeUser",
             permission="admin")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         GitHub Repository Collaborators can be imported using an ID made up of `repository:username`, e.g.
 
         ```sh
         $ pulumi import github:index/repositoryCollaborator:RepositoryCollaborator collaborator terraform:someuser
```

### Comparing `pulumi_github-6.3.0a1713561029/pulumi_github/repository_collaborators.py` & `pulumi_github-6.3.0a1713897837/pulumi_github/repository_collaborators.py`

 * *Files 2% similar despite different names*

```diff
@@ -175,15 +175,14 @@
 
         - [Adding outside collaborators to your personal repositories](https://help.github.com/en/github/setting-up-and-managing-your-github-user-account/managing-access-to-your-personal-repositories)
         - [Adding outside collaborators to repositories in your organization](https://help.github.com/articles/adding-outside-collaborators-to-repositories-in-your-organization/)
         - [Converting an organization member to an outside collaborators](https://help.github.com/articles/converting-an-organization-member-to-an-outside-collaborator/)
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_github as github
 
         # Add collaborators to a repository
         some_team = github.Team("some_team",
             name="SomeTeam",
@@ -196,15 +195,14 @@
                 username="SomeUser",
             )],
             teams=[github.RepositoryCollaboratorsTeamArgs(
                 permission="pull",
                 team_id=some_team.slug,
             )])
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         GitHub Repository Collaborators can be imported using the name `name`, e.g.
 
         ```sh
         $ pulumi import github:index/repositoryCollaborators:RepositoryCollaborators collaborators terraform
@@ -246,15 +244,14 @@
 
         - [Adding outside collaborators to your personal repositories](https://help.github.com/en/github/setting-up-and-managing-your-github-user-account/managing-access-to-your-personal-repositories)
         - [Adding outside collaborators to repositories in your organization](https://help.github.com/articles/adding-outside-collaborators-to-repositories-in-your-organization/)
         - [Converting an organization member to an outside collaborators](https://help.github.com/articles/converting-an-organization-member-to-an-outside-collaborator/)
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_github as github
 
         # Add collaborators to a repository
         some_team = github.Team("some_team",
             name="SomeTeam",
@@ -267,15 +264,14 @@
                 username="SomeUser",
             )],
             teams=[github.RepositoryCollaboratorsTeamArgs(
                 permission="pull",
                 team_id=some_team.slug,
             )])
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         GitHub Repository Collaborators can be imported using the name `name`, e.g.
 
         ```sh
         $ pulumi import github:index/repositoryCollaborators:RepositoryCollaborators collaborators terraform
```

### Comparing `pulumi_github-6.3.0a1713561029/pulumi_github/repository_dependabot_security_updates.py` & `pulumi_github-6.3.0a1713897837/pulumi_github/repository_dependabot_security_updates.py`

 * *Files 1% similar despite different names*

```diff
@@ -100,29 +100,27 @@
         """
         This resource allows you to manage dependabot automated security fixes for a single repository. See the
         [documentation](https://docs.github.com/en/code-security/dependabot/dependabot-security-updates/about-dependabot-security-updates)
         for details of usage and how this will impact your repository
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_github as github
 
         repo = github.Repository("repo",
             name="my-repo",
             description="GitHub repo managed by Terraform",
             private=False,
             vulnerability_alerts=True)
         example = github.RepositoryDependabotSecurityUpdates("example",
             repository=test["id"],
             enabled=True)
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         ### Import by name
 
         ```sh
         $ pulumi import github:index/repositoryDependabotSecurityUpdates:RepositoryDependabotSecurityUpdates example my-repo
@@ -142,29 +140,27 @@
         """
         This resource allows you to manage dependabot automated security fixes for a single repository. See the
         [documentation](https://docs.github.com/en/code-security/dependabot/dependabot-security-updates/about-dependabot-security-updates)
         for details of usage and how this will impact your repository
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_github as github
 
         repo = github.Repository("repo",
             name="my-repo",
             description="GitHub repo managed by Terraform",
             private=False,
             vulnerability_alerts=True)
         example = github.RepositoryDependabotSecurityUpdates("example",
             repository=test["id"],
             enabled=True)
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         ### Import by name
 
         ```sh
         $ pulumi import github:index/repositoryDependabotSecurityUpdates:RepositoryDependabotSecurityUpdates example my-repo
```

### Comparing `pulumi_github-6.3.0a1713561029/pulumi_github/repository_deploy_key.py` & `pulumi_github-6.3.0a1713897837/pulumi_github/repository_deploy_key.py`

 * *Files 2% similar despite different names*

```diff
@@ -192,30 +192,28 @@
         This resource allows you to add/remove repository deploy keys.
 
         Further documentation on GitHub repository deploy keys:
         - [About deploy keys](https://developer.github.com/guides/managing-deploy-keys/#deploy-keys)
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_github as github
         import pulumi_tls as tls
 
         # Generate an ssh key using provider "hashicorp/tls"
         example_repository_deploy_key = tls.PrivateKey("example_repository_deploy_key", algorithm="ED25519")
         # Add the ssh key as a deploy key
         example_repository_deploy_key_repository_deploy_key = github.RepositoryDeployKey("example_repository_deploy_key",
             title="Repository test key",
             repository="test-repo",
             key=example_repository_deploy_key.public_key_openssh,
             read_only=True)
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Repository deploy keys can be imported using a colon-separated pair of repository name
         and GitHub's key id. The latter can be obtained by GitHub's SDKs and API.
 
         ```sh
@@ -247,30 +245,28 @@
         This resource allows you to add/remove repository deploy keys.
 
         Further documentation on GitHub repository deploy keys:
         - [About deploy keys](https://developer.github.com/guides/managing-deploy-keys/#deploy-keys)
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_github as github
         import pulumi_tls as tls
 
         # Generate an ssh key using provider "hashicorp/tls"
         example_repository_deploy_key = tls.PrivateKey("example_repository_deploy_key", algorithm="ED25519")
         # Add the ssh key as a deploy key
         example_repository_deploy_key_repository_deploy_key = github.RepositoryDeployKey("example_repository_deploy_key",
             title="Repository test key",
             repository="test-repo",
             key=example_repository_deploy_key.public_key_openssh,
             read_only=True)
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Repository deploy keys can be imported using a colon-separated pair of repository name
         and GitHub's key id. The latter can be obtained by GitHub's SDKs and API.
 
         ```sh
```

### Comparing `pulumi_github-6.3.0a1713561029/pulumi_github/repository_deployment_branch_policy.py` & `pulumi_github-6.3.0a1713897837/pulumi_github/repository_deployment_branch_policy.py`

 * *Files 2% similar despite different names*

```diff
@@ -147,15 +147,14 @@
                  repository: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         This resource allows you to create and manage deployment branch policies.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_github as github
 
         env = github.RepositoryEnvironment("env",
             repository="my_repo",
             environment="my_env",
@@ -165,15 +164,14 @@
             ))
         foo = github.RepositoryDeploymentBranchPolicy("foo",
             repository="my_repo",
             environment_name="my_env",
             name="foo",
             opts=pulumi.ResourceOptions(depends_on=[env]))
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         ```sh
         $ pulumi import github:index/repositoryDeploymentBranchPolicy:RepositoryDeploymentBranchPolicy foo repo:env:id
         ```
 
@@ -190,15 +188,14 @@
                  args: RepositoryDeploymentBranchPolicyArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         This resource allows you to create and manage deployment branch policies.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_github as github
 
         env = github.RepositoryEnvironment("env",
             repository="my_repo",
             environment="my_env",
@@ -208,15 +205,14 @@
             ))
         foo = github.RepositoryDeploymentBranchPolicy("foo",
             repository="my_repo",
             environment_name="my_env",
             name="foo",
             opts=pulumi.ResourceOptions(depends_on=[env]))
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         ```sh
         $ pulumi import github:index/repositoryDeploymentBranchPolicy:RepositoryDeploymentBranchPolicy foo repo:env:id
         ```
```

### Comparing `pulumi_github-6.3.0a1713561029/pulumi_github/repository_environment.py` & `pulumi_github-6.3.0a1713897837/pulumi_github/repository_environment.py`

 * *Files 2% similar despite different names*

```diff
@@ -265,15 +265,14 @@
                  wait_timer: Optional[pulumi.Input[int]] = None,
                  __props__=None):
         """
         This resource allows you to create and manage environments for a GitHub repository.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_github as github
 
         current = github.get_user(username="")
         example = github.Repository("example",
             name="A Repository Project",
@@ -286,15 +285,14 @@
                 users=[current.id],
             )],
             deployment_branch_policy=github.RepositoryEnvironmentDeploymentBranchPolicyArgs(
                 protected_branches=True,
                 custom_branch_policies=False,
             ))
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         GitHub Repository Environment can be imported using an ID made up of `name` of the repository combined with the `environment` name of the environment, separated by a `:` character, e.g.
 
         ```sh
         $ pulumi import github:index/repositoryEnvironment:RepositoryEnvironment daily terraform:daily
@@ -317,15 +315,14 @@
                  args: RepositoryEnvironmentArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         This resource allows you to create and manage environments for a GitHub repository.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_github as github
 
         current = github.get_user(username="")
         example = github.Repository("example",
             name="A Repository Project",
@@ -338,15 +335,14 @@
                 users=[current.id],
             )],
             deployment_branch_policy=github.RepositoryEnvironmentDeploymentBranchPolicyArgs(
                 protected_branches=True,
                 custom_branch_policies=False,
             ))
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         GitHub Repository Environment can be imported using an ID made up of `name` of the repository combined with the `environment` name of the environment, separated by a `:` character, e.g.
 
         ```sh
         $ pulumi import github:index/repositoryEnvironment:RepositoryEnvironment daily terraform:daily
```

### Comparing `pulumi_github-6.3.0a1713561029/pulumi_github/repository_environment_deployment_policy.py` & `pulumi_github-6.3.0a1713897837/pulumi_github/repository_environment_deployment_policy.py`

 * *Files 2% similar despite different names*

```diff
@@ -130,15 +130,14 @@
                  repository: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         This resource allows you to create and manage environment deployment branch policies for a GitHub repository.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_github as github
 
         current = github.get_user(username="")
         test = github.Repository("test", name="tf-acc-test-%s")
         test_repository_environment = github.RepositoryEnvironment("test",
@@ -153,15 +152,14 @@
                 custom_branch_policies=True,
             ))
         test_repository_environment_deployment_policy = github.RepositoryEnvironmentDeploymentPolicy("test",
             repository=test.name,
             environment=test_repository_environment.environment,
             branch_pattern="releases/*")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         GitHub Repository Environment Deployment Policy can be imported using an ID made up of `name` of the repository combined with the `environment` name of the environment with the `Id` of the deployment policy, separated by a `:` character, e.g.
 
         ```sh
         $ pulumi import github:index/repositoryEnvironmentDeploymentPolicy:RepositoryEnvironmentDeploymentPolicy daily terraform:daily:123456
@@ -180,15 +178,14 @@
                  args: RepositoryEnvironmentDeploymentPolicyArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         This resource allows you to create and manage environment deployment branch policies for a GitHub repository.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_github as github
 
         current = github.get_user(username="")
         test = github.Repository("test", name="tf-acc-test-%s")
         test_repository_environment = github.RepositoryEnvironment("test",
@@ -203,15 +200,14 @@
                 custom_branch_policies=True,
             ))
         test_repository_environment_deployment_policy = github.RepositoryEnvironmentDeploymentPolicy("test",
             repository=test.name,
             environment=test_repository_environment.environment,
             branch_pattern="releases/*")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         GitHub Repository Environment Deployment Policy can be imported using an ID made up of `name` of the repository combined with the `environment` name of the environment with the `Id` of the deployment policy, separated by a `:` character, e.g.
 
         ```sh
         $ pulumi import github:index/repositoryEnvironmentDeploymentPolicy:RepositoryEnvironmentDeploymentPolicy daily terraform:daily:123456
```

### Comparing `pulumi_github-6.3.0a1713561029/pulumi_github/repository_file.py` & `pulumi_github-6.3.0a1713897837/pulumi_github/repository_file.py`

 * *Files 1% similar despite different names*

```diff
@@ -348,15 +348,14 @@
                  __props__=None):
         """
         This resource allows you to create and manage files within a
         GitHub repository.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_github as github
 
         foo = github.Repository("foo",
             name="tf-acc-test-%s",
             auto_init=True)
@@ -366,15 +365,14 @@
             file=".gitignore",
             content="**/*.tfstate",
             commit_message="Managed by Terraform",
             commit_author="Terraform User",
             commit_email="terraform@example.com",
             overwrite_on_create=True)
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Repository files can be imported using a combination of the `repo` and `file`, e.g.
 
         ```sh
         $ pulumi import github:index/repositoryFile:RepositoryFile gitignore example/.gitignore
@@ -405,15 +403,14 @@
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         This resource allows you to create and manage files within a
         GitHub repository.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_github as github
 
         foo = github.Repository("foo",
             name="tf-acc-test-%s",
             auto_init=True)
@@ -423,15 +420,14 @@
             file=".gitignore",
             content="**/*.tfstate",
             commit_message="Managed by Terraform",
             commit_author="Terraform User",
             commit_email="terraform@example.com",
             overwrite_on_create=True)
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Repository files can be imported using a combination of the `repo` and `file`, e.g.
 
         ```sh
         $ pulumi import github:index/repositoryFile:RepositoryFile gitignore example/.gitignore
```

### Comparing `pulumi_github-6.3.0a1713561029/pulumi_github/repository_milestone.py` & `pulumi_github-6.3.0a1713897837/pulumi_github/repository_milestone.py`

 * *Files 1% similar despite different names*

```diff
@@ -247,26 +247,24 @@
         """
         Provides a GitHub repository milestone resource.
 
         This resource allows you to create and manage milestones for a GitHub Repository within an organization or user account.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_github as github
 
         # Create a milestone for a repository
         example = github.RepositoryMilestone("example",
             owner="example-owner",
             repository="example-repository",
             title="v1.1.0")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         A GitHub Repository Milestone can be imported using an ID made up of `owner/repository/number`, e.g.
 
         ```sh
         $ pulumi import github:index/repositoryMilestone:RepositoryMilestone example example-owner/example-repository/1
@@ -290,26 +288,24 @@
         """
         Provides a GitHub repository milestone resource.
 
         This resource allows you to create and manage milestones for a GitHub Repository within an organization or user account.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_github as github
 
         # Create a milestone for a repository
         example = github.RepositoryMilestone("example",
             owner="example-owner",
             repository="example-repository",
             title="v1.1.0")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         A GitHub Repository Milestone can be imported using an ID made up of `owner/repository/number`, e.g.
 
         ```sh
         $ pulumi import github:index/repositoryMilestone:RepositoryMilestone example example-owner/example-repository/1
```

### Comparing `pulumi_github-6.3.0a1713561029/pulumi_github/repository_project.py` & `pulumi_github-6.3.0a1713897837/pulumi_github/repository_project.py`

 * *Files 1% similar despite different names*

```diff
@@ -160,29 +160,27 @@
                  repository: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         This resource allows you to create and manage projects for GitHub repository.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_github as github
 
         example = github.Repository("example",
             name="example",
             description="My awesome codebase",
             has_projects=True)
         project = github.RepositoryProject("project",
             name="A Repository Project",
             repository=example.name,
             body="This is a repository project.")
         ```
-        <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] body: The body of the project.
         :param pulumi.Input[str] name: The name of the project.
         :param pulumi.Input[str] repository: The repository of the project.
         """
@@ -193,29 +191,27 @@
                  args: RepositoryProjectArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         This resource allows you to create and manage projects for GitHub repository.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_github as github
 
         example = github.Repository("example",
             name="example",
             description="My awesome codebase",
             has_projects=True)
         project = github.RepositoryProject("project",
             name="A Repository Project",
             repository=example.name,
             body="This is a repository project.")
         ```
-        <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param RepositoryProjectArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
```

### Comparing `pulumi_github-6.3.0a1713561029/pulumi_github/repository_pull_request.py` & `pulumi_github-6.3.0a1713897837/pulumi_github/repository_pull_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -405,27 +405,25 @@
                  title: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         This resource allows you to create and manage PullRequests for repositories within your GitHub organization or personal account.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_github as github
 
         example = github.RepositoryPullRequest("example",
             base_repository="example-repository",
             base_ref="main",
             head_ref="feature-branch",
             title="My newest feature",
             body="This will change everything")
         ```
-        <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] base_ref: Name of the branch serving as the base of the Pull Request.
         :param pulumi.Input[str] base_repository: Name of the base repository to retrieve the Pull Requests from.
         :param pulumi.Input[str] body: Body of the Pull Request.
         :param pulumi.Input[str] head_ref: Name of the branch serving as the head of the Pull Request.
@@ -440,27 +438,25 @@
                  args: RepositoryPullRequestArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         This resource allows you to create and manage PullRequests for repositories within your GitHub organization or personal account.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_github as github
 
         example = github.RepositoryPullRequest("example",
             base_repository="example-repository",
             base_ref="main",
             head_ref="feature-branch",
             title="My newest feature",
             body="This will change everything")
         ```
-        <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param RepositoryPullRequestArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
```

### Comparing `pulumi_github-6.3.0a1713561029/pulumi_github/repository_ruleset.py` & `pulumi_github-6.3.0a1713897837/pulumi_github/repository_ruleset.py`

 * *Files 1% similar despite different names*

```diff
@@ -314,15 +314,14 @@
         """
         Creates a GitHub repository ruleset.
 
         This resource allows you to create and manage rulesets on the repository level. When applied, a new ruleset will be created. When destroyed, that ruleset will be removed.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_github as github
 
         example = github.Repository("example",
             name="example",
             description="Example repository")
@@ -349,15 +348,14 @@
                 required_linear_history=True,
                 required_signatures=True,
                 required_deployments=github.RepositoryRulesetRulesRequiredDeploymentsArgs(
                     required_deployment_environments=["test"],
                 ),
             ))
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         GitHub Repository Rulesets can be imported using the GitHub repository name and ruleset ID e.g.
 
         ```sh
         $ pulumi import github:index/repositoryRuleset:RepositoryRuleset example example:12345`
@@ -382,15 +380,14 @@
         """
         Creates a GitHub repository ruleset.
 
         This resource allows you to create and manage rulesets on the repository level. When applied, a new ruleset will be created. When destroyed, that ruleset will be removed.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_github as github
 
         example = github.Repository("example",
             name="example",
             description="Example repository")
@@ -417,15 +414,14 @@
                 required_linear_history=True,
                 required_signatures=True,
                 required_deployments=github.RepositoryRulesetRulesRequiredDeploymentsArgs(
                     required_deployment_environments=["test"],
                 ),
             ))
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         GitHub Repository Rulesets can be imported using the GitHub repository name and ruleset ID e.g.
 
         ```sh
         $ pulumi import github:index/repositoryRuleset:RepositoryRuleset example example:12345`
```

### Comparing `pulumi_github-6.3.0a1713561029/pulumi_github/repository_tag_protection.py` & `pulumi_github-6.3.0a1713897837/pulumi_github/repository_tag_protection.py`

 * *Files 2% similar despite different names*

```diff
@@ -114,24 +114,22 @@
                  repository: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         This resource allows you to create and manage a repository tag protection for repositories within your GitHub organization or personal account.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_github as github
 
         example = github.RepositoryTagProtection("example",
             repository="example-repository",
             pattern="v*")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Repository tag protections can be imported using the `name` of the repository, combined with the `id` of the tag protection, separated by a `/` character.
         The `id` of the tag protection can be found using the [GitHub API](https://docs.github.com/en/rest/repos/tags#list-tag-protection-states-for-a-repository).
 
         Importing uses the name of the repository, as well as the ID of the tag protection, e.g.
@@ -152,24 +150,22 @@
                  args: RepositoryTagProtectionArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         This resource allows you to create and manage a repository tag protection for repositories within your GitHub organization or personal account.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_github as github
 
         example = github.RepositoryTagProtection("example",
             repository="example-repository",
             pattern="v*")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Repository tag protections can be imported using the `name` of the repository, combined with the `id` of the tag protection, separated by a `/` character.
         The `id` of the tag protection can be found using the [GitHub API](https://docs.github.com/en/rest/repos/tags#list-tag-protection-states-for-a-repository).
 
         Importing uses the name of the repository, as well as the ID of the tag protection, e.g.
```

### Comparing `pulumi_github-6.3.0a1713561029/pulumi_github/repository_topics.py` & `pulumi_github-6.3.0a1713897837/pulumi_github/repository_topics.py`

 * *Files 1% similar despite different names*

```diff
@@ -96,28 +96,26 @@
                  opts: Optional[pulumi.ResourceOptions] = None,
                  repository: Optional[pulumi.Input[str]] = None,
                  topics: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  __props__=None):
         """
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_github as github
 
         test = github.get_repository(name="test")
         test_repository_topics = github.RepositoryTopics("test",
             repository=test_github_repository["name"],
             topics=[
                 "topic-1",
                 "topic-2",
             ])
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Repository topics can be imported using the `name` of the repository.
 
         ```sh
         $ pulumi import github:index/repositoryTopics:RepositoryTopics terraform terraform
@@ -133,28 +131,26 @@
     def __init__(__self__,
                  resource_name: str,
                  args: RepositoryTopicsArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_github as github
 
         test = github.get_repository(name="test")
         test_repository_topics = github.RepositoryTopics("test",
             repository=test_github_repository["name"],
             topics=[
                 "topic-1",
                 "topic-2",
             ])
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Repository topics can be imported using the `name` of the repository.
 
         ```sh
         $ pulumi import github:index/repositoryTopics:RepositoryTopics terraform terraform
```

### Comparing `pulumi_github-6.3.0a1713561029/pulumi_github/repository_webhook.py` & `pulumi_github-6.3.0a1713897837/pulumi_github/repository_webhook.py`

 * *Files 2% similar despite different names*

```diff
@@ -94,15 +94,15 @@
                  url: Optional[pulumi.Input[str]] = None):
         """
         Input properties used for looking up and filtering RepositoryWebhook resources.
         :param pulumi.Input[bool] active: Indicate if the webhook should receive events. Defaults to `true`.
         :param pulumi.Input['RepositoryWebhookConfigurationArgs'] configuration: Configuration block for the webhook. Detailed below.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] events: A list of events which should trigger the webhook. See a list of [available events](https://developer.github.com/v3/activity/events/types/).
         :param pulumi.Input[str] repository: The repository of the webhook.
-        :param pulumi.Input[str] url: The URL of the webhook.
+        :param pulumi.Input[str] url: URL of the webhook.  This is a sensitive attribute because it may include basic auth credentials.
         """
         if active is not None:
             pulumi.set(__self__, "active", active)
         if configuration is not None:
             pulumi.set(__self__, "configuration", configuration)
         if etag is not None:
             pulumi.set(__self__, "etag", etag)
@@ -170,15 +170,15 @@
     def repository(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "repository", value)
 
     @property
     @pulumi.getter
     def url(self) -> Optional[pulumi.Input[str]]:
         """
-        The URL of the webhook.
+        URL of the webhook.  This is a sensitive attribute because it may include basic auth credentials.
         """
         return pulumi.get(self, "url")
 
     @url.setter
     def url(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "url", value)
 
@@ -195,15 +195,14 @@
                  __props__=None):
         """
         This resource allows you to create and manage webhooks for repositories within your
         GitHub organization or personal account.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_github as github
 
         repo = github.Repository("repo",
             name="foo",
             description="Terraform acceptance tests",
@@ -215,15 +214,14 @@
                 url="https://google.de/",
                 content_type="form",
                 insecure_ssl=False,
             ),
             active=False,
             events=["issues"])
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Repository webhooks can be imported using the `name` of the repository, combined with the `id` of the webhook, separated by a `/` character.
         The `id` of the webhook can be found in the URL of the webhook. For example: `"https://github.com/foo-org/foo-repo/settings/hooks/14711452"`.
 
         Importing uses the name of the repository, as well as the ID of the webhook, e.g.
@@ -248,15 +246,14 @@
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         This resource allows you to create and manage webhooks for repositories within your
         GitHub organization or personal account.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_github as github
 
         repo = github.Repository("repo",
             name="foo",
             description="Terraform acceptance tests",
@@ -268,15 +265,14 @@
                 url="https://google.de/",
                 content_type="form",
                 insecure_ssl=False,
             ),
             active=False,
             events=["issues"])
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Repository webhooks can be imported using the `name` of the repository, combined with the `id` of the webhook, separated by a `/` character.
         The `id` of the webhook can be found in the URL of the webhook. For example: `"https://github.com/foo-org/foo-repo/settings/hooks/14711452"`.
 
         Importing uses the name of the repository, as well as the ID of the webhook, e.g.
@@ -347,15 +343,15 @@
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[bool] active: Indicate if the webhook should receive events. Defaults to `true`.
         :param pulumi.Input[pulumi.InputType['RepositoryWebhookConfigurationArgs']] configuration: Configuration block for the webhook. Detailed below.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] events: A list of events which should trigger the webhook. See a list of [available events](https://developer.github.com/v3/activity/events/types/).
         :param pulumi.Input[str] repository: The repository of the webhook.
-        :param pulumi.Input[str] url: The URL of the webhook.
+        :param pulumi.Input[str] url: URL of the webhook.  This is a sensitive attribute because it may include basic auth credentials.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _RepositoryWebhookState.__new__(_RepositoryWebhookState)
 
         __props__.__dict__["active"] = active
         __props__.__dict__["configuration"] = configuration
@@ -402,11 +398,11 @@
         """
         return pulumi.get(self, "repository")
 
     @property
     @pulumi.getter
     def url(self) -> pulumi.Output[str]:
         """
-        The URL of the webhook.
+        URL of the webhook.  This is a sensitive attribute because it may include basic auth credentials.
         """
         return pulumi.get(self, "url")
```

### Comparing `pulumi_github-6.3.0a1713561029/pulumi_github/team.py` & `pulumi_github-6.3.0a1713897837/pulumi_github/team.py`

 * *Files 1% similar despite different names*

```diff
@@ -365,26 +365,24 @@
         Provides a GitHub team resource.
 
         This resource allows you to add/remove teams from your organization. When applied,
         a new team will be created. When destroyed, that team will be removed.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_github as github
 
         # Add a team to the organization
         some_team = github.Team("some_team",
             name="some-team",
             description="Some cool team",
             privacy="closed")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         GitHub Teams can be imported using the GitHub team ID or name e.g.
 
         ```sh
         $ pulumi import github:index/team:Team core 1234567
@@ -416,26 +414,24 @@
         Provides a GitHub team resource.
 
         This resource allows you to add/remove teams from your organization. When applied,
         a new team will be created. When destroyed, that team will be removed.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_github as github
 
         # Add a team to the organization
         some_team = github.Team("some_team",
             name="some-team",
             description="Some cool team",
             privacy="closed")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         GitHub Teams can be imported using the GitHub team ID or name e.g.
 
         ```sh
         $ pulumi import github:index/team:Team core 1234567
```

### Comparing `pulumi_github-6.3.0a1713561029/pulumi_github/team_members.py` & `pulumi_github-6.3.0a1713897837/pulumi_github/team_members.py`

 * *Files 2% similar despite different names*

```diff
@@ -106,15 +106,14 @@
                  opts: Optional[pulumi.ResourceOptions] = None,
                  members: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['TeamMembersMemberArgs']]]]] = None,
                  team_id: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_github as github
 
         # Add a user to the organization
         membership_for_some_user = github.Membership("membership_for_some_user",
             username="SomeUser",
@@ -134,15 +133,14 @@
                 ),
                 github.TeamMembersMemberArgs(
                     username="AnotherUser",
                     role="member",
                 ),
             ])
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         ~> **Note** Although the team id or team slug can be used it is recommended to use the team id.  Using the team slug will result in terraform doing conversions between the team slug and team id.  This will cause team members associations to the team to be destroyed and recreated on import.
 
         GitHub Team Membership can be imported using the team ID team id or team slug, e.g.
 
@@ -166,15 +164,14 @@
     def __init__(__self__,
                  resource_name: str,
                  args: TeamMembersArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_github as github
 
         # Add a user to the organization
         membership_for_some_user = github.Membership("membership_for_some_user",
             username="SomeUser",
@@ -194,15 +191,14 @@
                 ),
                 github.TeamMembersMemberArgs(
                     username="AnotherUser",
                     role="member",
                 ),
             ])
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         ~> **Note** Although the team id or team slug can be used it is recommended to use the team id.  Using the team slug will result in terraform doing conversions between the team slug and team id.  This will cause team members associations to the team to be destroyed and recreated on import.
 
         GitHub Team Membership can be imported using the team ID team id or team slug, e.g.
```

### Comparing `pulumi_github-6.3.0a1713561029/pulumi_github/team_membership.py` & `pulumi_github-6.3.0a1713897837/pulumi_github/team_membership.py`

 * *Files 5% similar despite different names*

```diff
@@ -156,15 +156,14 @@
 
         > **Note** This resource is not compatible with `TeamMembers`. Use either `TeamMembers` or `TeamMembership`.
 
         > **Note** Organization owners may not be set as "members" of a team; they may only be set as "maintainers". Attempting to set organization an owner to "member" of a may result in a `pulumi preview` diff that changes their status back to "maintainer".
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_github as github
 
         # Add a user to the organization
         membership_for_some_user = github.Membership("membership_for_some_user",
             username="SomeUser",
@@ -173,15 +172,14 @@
             name="SomeTeam",
             description="Some cool team")
         some_team_membership = github.TeamMembership("some_team_membership",
             team_id=some_team.id,
             username="SomeUser",
             role="member")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         GitHub Team Membership can be imported using an ID made up of `teamid:username` or `teamname:username`, e.g.
 
         ```sh
         $ pulumi import github:index/teamMembership:TeamMembership member 1234567:someuser
@@ -214,15 +212,14 @@
 
         > **Note** This resource is not compatible with `TeamMembers`. Use either `TeamMembers` or `TeamMembership`.
 
         > **Note** Organization owners may not be set as "members" of a team; they may only be set as "maintainers". Attempting to set organization an owner to "member" of a may result in a `pulumi preview` diff that changes their status back to "maintainer".
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_github as github
 
         # Add a user to the organization
         membership_for_some_user = github.Membership("membership_for_some_user",
             username="SomeUser",
@@ -231,15 +228,14 @@
             name="SomeTeam",
             description="Some cool team")
         some_team_membership = github.TeamMembership("some_team_membership",
             team_id=some_team.id,
             username="SomeUser",
             role="member")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         GitHub Team Membership can be imported using an ID made up of `teamid:username` or `teamname:username`, e.g.
 
         ```sh
         $ pulumi import github:index/teamMembership:TeamMembership member 1234567:someuser
```

### Comparing `pulumi_github-6.3.0a1713561029/pulumi_github/team_repository.py` & `pulumi_github-6.3.0a1713897837/pulumi_github/team_repository.py`

 * *Files 2% similar despite different names*

```diff
@@ -161,30 +161,28 @@
         to do that, see `Repository`.
 
         This resource is non-authoritative, for managing ALL collaborators of a repo, use RepositoryCollaborators
         instead.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_github as github
 
         # Add a repository to the team
         some_team = github.Team("some_team",
             name="SomeTeam",
             description="Some cool team")
         some_repo = github.Repository("some_repo", name="some-repo")
         some_team_repo = github.TeamRepository("some_team_repo",
             team_id=some_team.id,
             repository=some_repo.name,
             permission="pull")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         GitHub Team Repository can be imported using an ID made up of `team_id:repository` or `team_name:repository`, e.g.
 
         ```sh
         $ pulumi import github:index/teamRepository:TeamRepository terraform_repo 1234567:terraform
@@ -222,30 +220,28 @@
         to do that, see `Repository`.
 
         This resource is non-authoritative, for managing ALL collaborators of a repo, use RepositoryCollaborators
         instead.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_github as github
 
         # Add a repository to the team
         some_team = github.Team("some_team",
             name="SomeTeam",
             description="Some cool team")
         some_repo = github.Repository("some_repo", name="some-repo")
         some_team_repo = github.TeamRepository("some_team_repo",
             team_id=some_team.id,
             repository=some_repo.name,
             permission="pull")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         GitHub Team Repository can be imported using an ID made up of `team_id:repository` or `team_name:repository`, e.g.
 
         ```sh
         $ pulumi import github:index/teamRepository:TeamRepository terraform_repo 1234567:terraform
```

### Comparing `pulumi_github-6.3.0a1713561029/pulumi_github/team_settings.py` & `pulumi_github-6.3.0a1713897837/pulumi_github/team_settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -139,15 +139,14 @@
 
         The team must both belong to the same organization configured in the provider on GitHub.
 
         > **Note**: This resource relies on the v4 GraphQl GitHub API. If this API is not available, or the Stone Crop schema preview is not available, then this resource will not work as intended.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_github as github
 
         # Add a repository to the team
         some_team = github.Team("some_team",
             name="SomeTeam",
@@ -156,15 +155,14 @@
             team_id=some_team.id,
             review_request_delegation=github.TeamSettingsReviewRequestDelegationArgs(
                 algorithm="ROUND_ROBIN",
                 member_count=1,
                 notify=True,
             ))
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         GitHub Teams can be imported using the GitHub team ID, or the team slug e.g.
 
         ```sh
         $ pulumi import github:index/teamSettings:TeamSettings code_review_settings 1234567
@@ -193,15 +191,14 @@
 
         The team must both belong to the same organization configured in the provider on GitHub.
 
         > **Note**: This resource relies on the v4 GraphQl GitHub API. If this API is not available, or the Stone Crop schema preview is not available, then this resource will not work as intended.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_github as github
 
         # Add a repository to the team
         some_team = github.Team("some_team",
             name="SomeTeam",
@@ -210,15 +207,14 @@
             team_id=some_team.id,
             review_request_delegation=github.TeamSettingsReviewRequestDelegationArgs(
                 algorithm="ROUND_ROBIN",
                 member_count=1,
                 notify=True,
             ))
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         GitHub Teams can be imported using the GitHub team ID, or the team slug e.g.
 
         ```sh
         $ pulumi import github:index/teamSettings:TeamSettings code_review_settings 1234567
```

### Comparing `pulumi_github-6.3.0a1713561029/pulumi_github/team_sync_group_mapping.py` & `pulumi_github-6.3.0a1713897837/pulumi_github/team_sync_group_mapping.py`

 * *Files 5% similar despite different names*

```diff
@@ -129,29 +129,27 @@
         You must have team synchronization enabled for organizations owned by enterprise accounts.
 
         To learn more about team synchronization between IdPs and GitHub, please refer to:
         https://help.github.com/en/github/setting-up-and-managing-organizations-and-teams/synchronizing-teams-between-your-identity-provider-and-github
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_github as github
 
         example_groups = github.get_organization_team_sync_groups()
         example_group_mapping = github.TeamSyncGroupMapping("example_group_mapping",
             groups=[github.TeamSyncGroupMappingGroupArgs(
                 group_id=entry["value"],
                 group_name=entry["value"],
                 group_description=entry["value"],
             ) for entry in [{"key": k, "value": v} for k, v in [g for g in example_groups.groups if g.group_name == "some_team_group"]]],
             team_slug="example")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         GitHub Team Sync Group Mappings can be imported using the GitHub team `slug` e.g.
 
         ```sh
         $ pulumi import github:index/teamSyncGroupMapping:TeamSyncGroupMapping example some_team
@@ -176,29 +174,27 @@
         You must have team synchronization enabled for organizations owned by enterprise accounts.
 
         To learn more about team synchronization between IdPs and GitHub, please refer to:
         https://help.github.com/en/github/setting-up-and-managing-organizations-and-teams/synchronizing-teams-between-your-identity-provider-and-github
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_github as github
 
         example_groups = github.get_organization_team_sync_groups()
         example_group_mapping = github.TeamSyncGroupMapping("example_group_mapping",
             groups=[github.TeamSyncGroupMappingGroupArgs(
                 group_id=entry["value"],
                 group_name=entry["value"],
                 group_description=entry["value"],
             ) for entry in [{"key": k, "value": v} for k, v in [g for g in example_groups.groups if g.group_name == "some_team_group"]]],
             team_slug="example")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         GitHub Team Sync Group Mappings can be imported using the GitHub team `slug` e.g.
 
         ```sh
         $ pulumi import github:index/teamSyncGroupMapping:TeamSyncGroupMapping example some_team
```

### Comparing `pulumi_github-6.3.0a1713561029/pulumi_github/user_gpg_key.py` & `pulumi_github-6.3.0a1713897837/pulumi_github/user_gpg_key.py`

 * *Files 5% similar despite different names*

```diff
@@ -100,24 +100,22 @@
         """
         Provides a GitHub user's GPG key resource.
 
         This resource allows you to add/remove GPG keys from your user account.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_github as github
 
         example = github.UserGpgKey("example", armored_public_key=\"\"\"-----BEGIN PGP PUBLIC KEY BLOCK-----
         ...
         -----END PGP PUBLIC KEY BLOCK-----\"\"\")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         GPG keys are not importable due to the fact that [API](https://developer.github.com/v3/users/gpg_keys/#gpg-keys)
 
         does not return previously uploaded GPG key.
 
@@ -135,24 +133,22 @@
         """
         Provides a GitHub user's GPG key resource.
 
         This resource allows you to add/remove GPG keys from your user account.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_github as github
 
         example = github.UserGpgKey("example", armored_public_key=\"\"\"-----BEGIN PGP PUBLIC KEY BLOCK-----
         ...
         -----END PGP PUBLIC KEY BLOCK-----\"\"\")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         GPG keys are not importable due to the fact that [API](https://developer.github.com/v3/users/gpg_keys/#gpg-keys)
 
         does not return previously uploaded GPG key.
```

### Comparing `pulumi_github-6.3.0a1713561029/pulumi_github/user_invitation_accepter.py` & `pulumi_github-6.3.0a1713897837/pulumi_github/user_invitation_accepter.py`

 * *Files 2% similar despite different names*

```diff
@@ -100,27 +100,25 @@
                  invitation_id: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         Provides a resource to manage GitHub repository collaborator invitations.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_github as github
 
         example = github.Repository("example", name="example-repo")
         example_repository_collaborator = github.RepositoryCollaborator("example",
             repository=example.name,
             username="example-username",
             permission="push")
         example_user_invitation_accepter = github.UserInvitationAccepter("example", invitation_id=example_repository_collaborator.invitation_id)
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Allowing empty invitation IDs
 
         Set `allow_empty_id` when using `for_each` over a list of `github_repository_collaborator.invitation_id`'s.
 
         This allows applying a module again when a new `RepositoryCollaborator` resource is added to the `for_each` loop.
         This is needed as the `github_repository_collaborator.invitation_id` will be empty after a state refresh when the invitation has been accepted.
@@ -142,27 +140,25 @@
                  args: Optional[UserInvitationAccepterArgs] = None,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         Provides a resource to manage GitHub repository collaborator invitations.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_github as github
 
         example = github.Repository("example", name="example-repo")
         example_repository_collaborator = github.RepositoryCollaborator("example",
             repository=example.name,
             username="example-username",
             permission="push")
         example_user_invitation_accepter = github.UserInvitationAccepter("example", invitation_id=example_repository_collaborator.invitation_id)
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Allowing empty invitation IDs
 
         Set `allow_empty_id` when using `for_each` over a list of `github_repository_collaborator.invitation_id`'s.
 
         This allows applying a module again when a new `RepositoryCollaborator` resource is added to the `for_each` loop.
         This is needed as the `github_repository_collaborator.invitation_id` will be empty after a state refresh when the invitation has been accepted.
```

### Comparing `pulumi_github-6.3.0a1713561029/pulumi_github/user_ssh_key.py` & `pulumi_github-6.3.0a1713897837/pulumi_github/user_ssh_key.py`

 * *Files 3% similar despite different names*

```diff
@@ -128,25 +128,23 @@
         """
         Provides a GitHub user's SSH key resource.
 
         This resource allows you to add/remove SSH keys from your user account.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_github as github
         import pulumi_std as std
 
         example = github.UserSshKey("example",
             title="example title",
             key=std.file(input="~/.ssh/id_rsa.pub").result)
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         SSH keys can be imported using their ID e.g.
 
         ```sh
         $ pulumi import github:index/userSshKey:UserSshKey example 1234567
@@ -166,25 +164,23 @@
         """
         Provides a GitHub user's SSH key resource.
 
         This resource allows you to add/remove SSH keys from your user account.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_github as github
         import pulumi_std as std
 
         example = github.UserSshKey("example",
             title="example title",
             key=std.file(input="~/.ssh/id_rsa.pub").result)
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         SSH keys can be imported using their ID e.g.
 
         ```sh
         $ pulumi import github:index/userSshKey:UserSshKey example 1234567
```

### Comparing `pulumi_github-6.3.0a1713561029/pulumi_github.egg-info/PKG-INFO` & `pulumi_github-6.3.0a1713897837/pulumi_github.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_github
-Version: 6.3.0a1713561029
+Version: 6.3.0a1713897837
 Summary: A Pulumi package for creating and managing github cloud resources.
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.io
 Project-URL: Repository, https://github.com/pulumi/pulumi-github
 Keywords: pulumi,github
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_github-6.3.0a1713561029/pulumi_github.egg-info/SOURCES.txt` & `pulumi_github-6.3.0a1713897837/pulumi_github.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_github-6.3.0a1713561029/pyproject.toml` & `pulumi_github-6.3.0a1713897837/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [project]
   name = "pulumi_github"
   description = "A Pulumi package for creating and managing github cloud resources."
   dependencies = ["parver>=0.2.1", "pulumi>=3.0.0,<4.0.0", "semver>=2.8.1"]
   keywords = ["pulumi", "github"]
   readme = "README.md"
   requires-python = ">=3.8"
-  version = "6.3.0a1713561029"
+  version = "6.3.0a1713897837"
   [project.license]
     text = "Apache-2.0"
   [project.urls]
     Homepage = "https://pulumi.io"
     Repository = "https://github.com/pulumi/pulumi-github"
 
 [build-system]
```

