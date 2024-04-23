# Comparing `tmp/python_semantic_release-9.4.2.tar.gz` & `tmp/python_semantic_release-9.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_semantic_release-9.4.2.tar", last modified: Sun Apr 14 01:45:40 2024, max compression
+gzip compressed data, was "python_semantic_release-9.5.0.tar", last modified: Tue Apr 23 02:38:39 2024, max compression
```

## Comparing `python_semantic_release-9.4.2.tar` & `python_semantic_release-9.5.0.tar`

### file list

```diff
@@ -1,173 +1,173 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-14 01:45:40.381688 python_semantic_release-9.4.2/
--rw-r--r--   0 root         (0) root         (0)      230 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/AUTHORS.rst
--rw-r--r--   0 root         (0) root         (0)     1083 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)      225 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     5281 2024-04-14 01:45:40.381688 python_semantic_release-9.4.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2673 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-14 01:45:40.353688 python_semantic_release-9.4.2/docs/
--rw-r--r--   0 root         (0) root         (0)     6984 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/docs/Makefile
--rw-r--r--   0 root         (0) root         (0)     9656 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/docs/algorithm.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-14 01:45:40.353688 python_semantic_release-9.4.2/docs/automatic-releases/
--rw-r--r--   0 root         (0) root         (0)     1284 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/docs/automatic-releases/cronjobs.rst
--rw-r--r--   0 root         (0) root         (0)     4046 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/docs/automatic-releases/github-actions.rst
--rw-r--r--   0 root         (0) root         (0)      738 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/docs/automatic-releases/index.rst
--rw-r--r--   0 root         (0) root         (0)     2268 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/docs/automatic-releases/travis.rst
--rw-r--r--   0 root         (0) root         (0)    15332 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/docs/changelog_templates.rst
--rw-r--r--   0 root         (0) root         (0)    13289 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/docs/commands.rst
--rw-r--r--   0 root         (0) root         (0)    15380 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/docs/commit-parsing.rst
--rw-r--r--   0 root         (0) root         (0)     2288 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/docs/conf.py
--rw-r--r--   0 root         (0) root         (0)    28291 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/docs/configuration.rst
--rw-r--r--   0 root         (0) root         (0)       33 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/docs/contributing.rst
--rw-r--r--   0 root         (0) root         (0)       28 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/docs/contributors.rst
--rw-r--r--   0 root         (0) root         (0)     3501 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/docs/github-action.rst
--rw-r--r--   0 root         (0) root         (0)     6814 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/docs/index.rst
--rw-r--r--   0 root         (0) root         (0)     6735 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/docs/make.bat
--rw-r--r--   0 root         (0) root         (0)    21218 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/docs/migrating_from_v7.rst
--rw-r--r--   0 root         (0) root         (0)     8866 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/docs/multibranch_releases.rst
--rw-r--r--   0 root         (0) root         (0)     2403 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/docs/strict_mode.rst
--rw-r--r--   0 root         (0) root         (0)     1452 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/docs/troubleshooting.rst
--rw-r--r--   0 root         (0) root         (0)     9689 2024-04-14 01:45:34.000000 python_semantic_release-9.4.2/pyproject.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-14 01:45:40.381688 python_semantic_release-9.4.2/python_semantic_release.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5281 2024-04-14 01:45:40.000000 python_semantic_release-9.4.2/python_semantic_release.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5538 2024-04-14 01:45:40.000000 python_semantic_release-9.4.2/python_semantic_release.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-14 01:45:40.000000 python_semantic_release-9.4.2/python_semantic_release.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       95 2024-04-14 01:45:40.000000 python_semantic_release-9.4.2/python_semantic_release.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      613 2024-04-14 01:45:40.000000 python_semantic_release-9.4.2/python_semantic_release.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       17 2024-04-14 01:45:40.000000 python_semantic_release-9.4.2/python_semantic_release.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-14 01:45:40.357688 python_semantic_release-9.4.2/semantic_release/
--rw-r--r--   0 root         (0) root         (0)      870 2024-04-14 01:45:34.000000 python_semantic_release-9.4.2/semantic_release/__init__.py
--rw-r--r--   0 root         (0) root         (0)      106 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/semantic_release/__main__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-14 01:45:40.357688 python_semantic_release-9.4.2/semantic_release/changelog/
--rw-r--r--   0 root         (0) root         (0)      262 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/semantic_release/changelog/__init__.py
--rw-r--r--   0 root         (0) root         (0)      986 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/semantic_release/changelog/context.py
--rw-r--r--   0 root         (0) root         (0)     6675 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/semantic_release/changelog/release_history.py
--rw-r--r--   0 root         (0) root         (0)     4640 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/semantic_release/changelog/template.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-14 01:45:40.361688 python_semantic_release-9.4.2/semantic_release/cli/
--rw-r--r--   0 root         (0) root         (0)      419 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/semantic_release/cli/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-14 01:45:40.361688 python_semantic_release-9.4.2/semantic_release/cli/commands/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/semantic_release/cli/commands/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4087 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/semantic_release/cli/commands/changelog.py
--rw-r--r--   0 root         (0) root         (0)     3443 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/semantic_release/cli/commands/cli_context.py
--rw-r--r--   0 root         (0) root         (0)     1699 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/semantic_release/cli/commands/generate_config.py
--rw-r--r--   0 root         (0) root         (0)     2900 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/semantic_release/cli/commands/main.py
--rw-r--r--   0 root         (0) root         (0)     1703 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/semantic_release/cli/commands/publish.py
--rw-r--r--   0 root         (0) root         (0)    23015 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/semantic_release/cli/commands/version.py
--rw-r--r--   0 root         (0) root         (0)     1439 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/semantic_release/cli/common.py
--rw-r--r--   0 root         (0) root         (0)    17574 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/semantic_release/cli/config.py
--rw-r--r--   0 root         (0) root         (0)       39 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/semantic_release/cli/const.py
--rw-r--r--   0 root         (0) root         (0)     2110 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/semantic_release/cli/github_actions_output.py
--rw-r--r--   0 root         (0) root         (0)     3071 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/semantic_release/cli/masking_filter.py
--rw-r--r--   0 root         (0) root         (0)     3755 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/semantic_release/cli/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-14 01:45:40.361688 python_semantic_release-9.4.2/semantic_release/commit_parser/
--rw-r--r--   0 root         (0) root         (0)      615 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/semantic_release/commit_parser/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2609 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/semantic_release/commit_parser/_base.py
--rw-r--r--   0 root         (0) root         (0)     4393 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/semantic_release/commit_parser/angular.py
--rw-r--r--   0 root         (0) root         (0)     3289 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/semantic_release/commit_parser/emoji.py
--rw-r--r--   0 root         (0) root         (0)     5777 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/semantic_release/commit_parser/scipy.py
--rw-r--r--   0 root         (0) root         (0)     3194 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/semantic_release/commit_parser/tag.py
--rw-r--r--   0 root         (0) root         (0)     1505 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/semantic_release/commit_parser/token.py
--rw-r--r--   0 root         (0) root         (0)      730 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/semantic_release/commit_parser/util.py
--rw-r--r--   0 root         (0) root         (0)      831 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/semantic_release/const.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-14 01:45:40.345687 python_semantic_release-9.4.2/semantic_release/data/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-14 01:45:40.361688 python_semantic_release-9.4.2/semantic_release/data/templates/
--rw-r--r--   0 root         (0) root         (0)     1066 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/semantic_release/data/templates/CHANGELOG.md.j2
--rw-r--r--   0 root         (0) root         (0)      465 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/semantic_release/data/templates/release_notes.md.j2
--rw-r--r--   0 root         (0) root         (0)     1020 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/semantic_release/enums.py
--rw-r--r--   0 root         (0) root         (0)     1159 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/semantic_release/errors.py
--rw-r--r--   0 root         (0) root         (0)     5581 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/semantic_release/helpers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-14 01:45:40.365688 python_semantic_release-9.4.2/semantic_release/hvcs/
--rw-r--r--   0 root         (0) root         (0)      379 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/semantic_release/hvcs/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5232 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/semantic_release/hvcs/_base.py
--rw-r--r--   0 root         (0) root         (0)    11004 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/semantic_release/hvcs/bitbucket.py
--rw-r--r--   0 root         (0) root         (0)    11450 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/semantic_release/hvcs/gitea.py
--rw-r--r--   0 root         (0) root         (0)    16297 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/semantic_release/hvcs/github.py
--rw-r--r--   0 root         (0) root         (0)     7409 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/semantic_release/hvcs/gitlab.py
--rw-r--r--   0 root         (0) root         (0)      663 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/semantic_release/hvcs/token_auth.py
--rw-r--r--   0 root         (0) root         (0)     2886 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/semantic_release/hvcs/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-14 01:45:40.365688 python_semantic_release-9.4.2/semantic_release/version/
--rw-r--r--   0 root         (0) root         (0)      270 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/semantic_release/version/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16854 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/semantic_release/version/algorithm.py
--rw-r--r--   0 root         (0) root         (0)     7357 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/semantic_release/version/declaration.py
--rw-r--r--   0 root         (0) root         (0)     3050 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/semantic_release/version/translator.py
--rw-r--r--   0 root         (0) root         (0)    14175 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/semantic_release/version/version.py
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-14 01:45:40.381688 python_semantic_release-9.4.2/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-14 01:45:40.365688 python_semantic_release-9.4.2/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-14 01:45:40.369688 python_semantic_release-9.4.2/tests/command_line/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/tests/command_line/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2983 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/tests/command_line/conftest.py
--rw-r--r--   0 root         (0) root         (0)    11528 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/tests/command_line/test_changelog.py
--rw-r--r--   0 root         (0) root         (0)     1759 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/tests/command_line/test_generate_config.py
--rw-r--r--   0 root         (0) root         (0)     6566 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/tests/command_line/test_help.py
--rw-r--r--   0 root         (0) root         (0)     5255 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/tests/command_line/test_main.py
--rw-r--r--   0 root         (0) root         (0)     1425 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/tests/command_line/test_publish.py
--rw-r--r--   0 root         (0) root         (0)    28853 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/tests/command_line/test_version.py
--rw-r--r--   0 root         (0) root         (0)     2535 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/tests/conftest.py
--rw-r--r--   0 root         (0) root         (0)     8953 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/tests/const.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-14 01:45:40.369688 python_semantic_release-9.4.2/tests/fixtures/
--rw-r--r--   0 root         (0) root         (0)      197 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/tests/fixtures/__init__.py
--rw-r--r--   0 root         (0) root         (0)      912 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/tests/fixtures/commit_parsers.py
--rw-r--r--   0 root         (0) root         (0)    11562 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/tests/fixtures/example_project.py
--rw-r--r--   0 root         (0) root         (0)    13292 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/tests/fixtures/git_repo.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-14 01:45:40.369688 python_semantic_release-9.4.2/tests/fixtures/repos/
--rw-r--r--   0 root         (0) root         (0)      142 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/tests/fixtures/repos/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-14 01:45:40.369688 python_semantic_release-9.4.2/tests/fixtures/repos/git_flow/
--rw-r--r--   0 root         (0) root         (0)      140 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/tests/fixtures/repos/git_flow/__init__.py
--rw-r--r--   0 root         (0) root         (0)    21042 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/tests/fixtures/repos/git_flow/repo_w_2_release_channels.py
--rw-r--r--   0 root         (0) root         (0)    21711 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/tests/fixtures/repos/git_flow/repo_w_3_release_channels.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-14 01:45:40.369688 python_semantic_release-9.4.2/tests/fixtures/repos/github_flow/
--rw-r--r--   0 root         (0) root         (0)       71 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/tests/fixtures/repos/github_flow/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15712 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/tests/fixtures/repos/github_flow/repo_w_release_channels.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-14 01:45:40.373688 python_semantic_release-9.4.2/tests/fixtures/repos/trunk_based_dev/
--rw-r--r--   0 root         (0) root         (0)      199 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/tests/fixtures/repos/trunk_based_dev/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10463 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/tests/fixtures/repos/trunk_based_dev/repo_w_no_tags.py
--rw-r--r--   0 root         (0) root         (0)    13604 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/tests/fixtures/repos/trunk_based_dev/repo_w_prereleases.py
--rw-r--r--   0 root         (0) root         (0)    10698 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/tests/fixtures/repos/trunk_based_dev/repo_w_tags.py
--rw-r--r--   0 root         (0) root         (0)     4494 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/tests/fixtures/scipy.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-14 01:45:40.373688 python_semantic_release-9.4.2/tests/scenario/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/tests/scenario/__init__.py
--rw-r--r--   0 root         (0) root         (0)   127286 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/tests/scenario/test_next_version.py
--rw-r--r--   0 root         (0) root         (0)    12845 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/tests/scenario/test_release_history.py
--rw-r--r--   0 root         (0) root         (0)     5074 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/tests/scenario/test_template_render.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-14 01:45:40.373688 python_semantic_release-9.4.2/tests/unit/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/tests/unit/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-14 01:45:40.373688 python_semantic_release-9.4.2/tests/unit/semantic_release/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/tests/unit/semantic_release/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-14 01:45:40.373688 python_semantic_release-9.4.2/tests/unit/semantic_release/changelog/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/tests/unit/semantic_release/changelog/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6222 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/tests/unit/semantic_release/changelog/test_default_changelog.py
--rw-r--r--   0 root         (0) root         (0)     3560 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/tests/unit/semantic_release/changelog/test_release_notes.py
--rw-r--r--   0 root         (0) root         (0)     2116 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/tests/unit/semantic_release/changelog/test_template.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-14 01:45:40.377688 python_semantic_release-9.4.2/tests/unit/semantic_release/cli/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/tests/unit/semantic_release/cli/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5840 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/tests/unit/semantic_release/cli/test_config.py
--rw-r--r--   0 root         (0) root         (0)     2129 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/tests/unit/semantic_release/cli/test_github_actions_output.py
--rw-r--r--   0 root         (0) root         (0)     6361 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/tests/unit/semantic_release/cli/test_masking_filter.py
--rw-r--r--   0 root         (0) root         (0)     4219 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/tests/unit/semantic_release/cli/test_util.py
--rw-r--r--   0 root         (0) root         (0)      799 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/tests/unit/semantic_release/cli/test_version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-14 01:45:40.377688 python_semantic_release-9.4.2/tests/unit/semantic_release/commit_parser/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/tests/unit/semantic_release/commit_parser/__init__.py
--rw-r--r--   0 root         (0) root         (0)      140 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/tests/unit/semantic_release/commit_parser/helper.py
--rw-r--r--   0 root         (0) root         (0)     5952 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/tests/unit/semantic_release/commit_parser/test_angular.py
--rw-r--r--   0 root         (0) root         (0)     2483 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/tests/unit/semantic_release/commit_parser/test_emoji.py
--rw-r--r--   0 root         (0) root         (0)      500 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/tests/unit/semantic_release/commit_parser/test_scipy.py
--rw-r--r--   0 root         (0) root         (0)     2096 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/tests/unit/semantic_release/commit_parser/test_tag.py
--rw-r--r--   0 root         (0) root         (0)      648 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/tests/unit/semantic_release/commit_parser/test_token.py
--rw-r--r--   0 root         (0) root         (0)      836 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/tests/unit/semantic_release/commit_parser/test_util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-14 01:45:40.377688 python_semantic_release-9.4.2/tests/unit/semantic_release/hvcs/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/tests/unit/semantic_release/hvcs/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1357 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/tests/unit/semantic_release/hvcs/test__base.py
--rw-r--r--   0 root         (0) root         (0)    10521 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/tests/unit/semantic_release/hvcs/test_bitbucket.py
--rw-r--r--   0 root         (0) root         (0)    27246 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/tests/unit/semantic_release/hvcs/test_gitea.py
--rw-r--r--   0 root         (0) root         (0)    34206 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/tests/unit/semantic_release/hvcs/test_github.py
--rw-r--r--   0 root         (0) root         (0)    15576 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/tests/unit/semantic_release/hvcs/test_gitlab.py
--rw-r--r--   0 root         (0) root         (0)      966 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/tests/unit/semantic_release/hvcs/test_token_auth.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/tests/unit/semantic_release/hvcs/test_util.py
--rw-r--r--   0 root         (0) root         (0)     4507 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/tests/unit/semantic_release/test_helpers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-14 01:45:40.381688 python_semantic_release-9.4.2/tests/unit/semantic_release/version/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/tests/unit/semantic_release/version/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9605 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/tests/unit/semantic_release/version/test_algorithm.py
--rw-r--r--   0 root         (0) root         (0)     3874 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/tests/unit/semantic_release/version/test_declaration.py
--rw-r--r--   0 root         (0) root         (0)     2951 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/tests/unit/semantic_release/version/test_translator.py
--rw-r--r--   0 root         (0) root         (0)     9714 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/tests/unit/semantic_release/version/test_version.py
--rw-r--r--   0 root         (0) root         (0)     5551 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/tests/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 02:38:39.163867 python_semantic_release-9.5.0/
+-rw-r--r--   0 root         (0) root         (0)      230 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/AUTHORS.rst
+-rw-r--r--   0 root         (0) root         (0)     1083 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      225 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     5281 2024-04-23 02:38:39.163867 python_semantic_release-9.5.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2673 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 02:38:39.131866 python_semantic_release-9.5.0/docs/
+-rw-r--r--   0 root         (0) root         (0)     6984 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/docs/Makefile
+-rw-r--r--   0 root         (0) root         (0)     9656 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/docs/algorithm.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 02:38:39.131866 python_semantic_release-9.5.0/docs/automatic-releases/
+-rw-r--r--   0 root         (0) root         (0)     1284 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/docs/automatic-releases/cronjobs.rst
+-rw-r--r--   0 root         (0) root         (0)     4046 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/docs/automatic-releases/github-actions.rst
+-rw-r--r--   0 root         (0) root         (0)      738 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/docs/automatic-releases/index.rst
+-rw-r--r--   0 root         (0) root         (0)     2268 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/docs/automatic-releases/travis.rst
+-rw-r--r--   0 root         (0) root         (0)    15332 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/docs/changelog_templates.rst
+-rw-r--r--   0 root         (0) root         (0)    13289 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/docs/commands.rst
+-rw-r--r--   0 root         (0) root         (0)    15380 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/docs/commit-parsing.rst
+-rw-r--r--   0 root         (0) root         (0)     2288 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/docs/conf.py
+-rw-r--r--   0 root         (0) root         (0)    28291 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/docs/configuration.rst
+-rw-r--r--   0 root         (0) root         (0)       33 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/docs/contributing.rst
+-rw-r--r--   0 root         (0) root         (0)       28 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/docs/contributors.rst
+-rw-r--r--   0 root         (0) root         (0)     3501 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/docs/github-action.rst
+-rw-r--r--   0 root         (0) root         (0)     6814 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/docs/index.rst
+-rw-r--r--   0 root         (0) root         (0)     6735 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/docs/make.bat
+-rw-r--r--   0 root         (0) root         (0)    21218 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/docs/migrating_from_v7.rst
+-rw-r--r--   0 root         (0) root         (0)     8866 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/docs/multibranch_releases.rst
+-rw-r--r--   0 root         (0) root         (0)     2403 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/docs/strict_mode.rst
+-rw-r--r--   0 root         (0) root         (0)     1452 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/docs/troubleshooting.rst
+-rw-r--r--   0 root         (0) root         (0)     9146 2024-04-23 02:38:33.000000 python_semantic_release-9.5.0/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 02:38:39.159867 python_semantic_release-9.5.0/python_semantic_release.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5281 2024-04-23 02:38:39.000000 python_semantic_release-9.5.0/python_semantic_release.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5538 2024-04-23 02:38:39.000000 python_semantic_release-9.5.0/python_semantic_release.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-23 02:38:39.000000 python_semantic_release-9.5.0/python_semantic_release.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       95 2024-04-23 02:38:39.000000 python_semantic_release-9.5.0/python_semantic_release.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      613 2024-04-23 02:38:39.000000 python_semantic_release-9.5.0/python_semantic_release.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2024-04-23 02:38:39.000000 python_semantic_release-9.5.0/python_semantic_release.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 02:38:39.135866 python_semantic_release-9.5.0/semantic_release/
+-rw-r--r--   0 root         (0) root         (0)      870 2024-04-23 02:38:33.000000 python_semantic_release-9.5.0/semantic_release/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      106 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/semantic_release/__main__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 02:38:39.135866 python_semantic_release-9.5.0/semantic_release/changelog/
+-rw-r--r--   0 root         (0) root         (0)      262 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/semantic_release/changelog/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      986 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/semantic_release/changelog/context.py
+-rw-r--r--   0 root         (0) root         (0)     6675 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/semantic_release/changelog/release_history.py
+-rw-r--r--   0 root         (0) root         (0)     4640 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/semantic_release/changelog/template.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 02:38:39.139866 python_semantic_release-9.5.0/semantic_release/cli/
+-rw-r--r--   0 root         (0) root         (0)      419 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/semantic_release/cli/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 02:38:39.139866 python_semantic_release-9.5.0/semantic_release/cli/commands/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/semantic_release/cli/commands/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4087 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/semantic_release/cli/commands/changelog.py
+-rw-r--r--   0 root         (0) root         (0)     3443 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/semantic_release/cli/commands/cli_context.py
+-rw-r--r--   0 root         (0) root         (0)     1699 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/semantic_release/cli/commands/generate_config.py
+-rw-r--r--   0 root         (0) root         (0)     2900 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/semantic_release/cli/commands/main.py
+-rw-r--r--   0 root         (0) root         (0)     1703 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/semantic_release/cli/commands/publish.py
+-rw-r--r--   0 root         (0) root         (0)    23015 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/semantic_release/cli/commands/version.py
+-rw-r--r--   0 root         (0) root         (0)     1439 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/semantic_release/cli/common.py
+-rw-r--r--   0 root         (0) root         (0)    17574 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/semantic_release/cli/config.py
+-rw-r--r--   0 root         (0) root         (0)       39 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/semantic_release/cli/const.py
+-rw-r--r--   0 root         (0) root         (0)     2110 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/semantic_release/cli/github_actions_output.py
+-rw-r--r--   0 root         (0) root         (0)     3071 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/semantic_release/cli/masking_filter.py
+-rw-r--r--   0 root         (0) root         (0)     3755 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/semantic_release/cli/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 02:38:39.139866 python_semantic_release-9.5.0/semantic_release/commit_parser/
+-rw-r--r--   0 root         (0) root         (0)      615 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/semantic_release/commit_parser/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2609 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/semantic_release/commit_parser/_base.py
+-rw-r--r--   0 root         (0) root         (0)     4393 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/semantic_release/commit_parser/angular.py
+-rw-r--r--   0 root         (0) root         (0)     3289 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/semantic_release/commit_parser/emoji.py
+-rw-r--r--   0 root         (0) root         (0)     5777 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/semantic_release/commit_parser/scipy.py
+-rw-r--r--   0 root         (0) root         (0)     3194 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/semantic_release/commit_parser/tag.py
+-rw-r--r--   0 root         (0) root         (0)     1505 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/semantic_release/commit_parser/token.py
+-rw-r--r--   0 root         (0) root         (0)      730 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/semantic_release/commit_parser/util.py
+-rw-r--r--   0 root         (0) root         (0)      831 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/semantic_release/const.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 02:38:39.123866 python_semantic_release-9.5.0/semantic_release/data/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 02:38:39.139866 python_semantic_release-9.5.0/semantic_release/data/templates/
+-rw-r--r--   0 root         (0) root         (0)     1066 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/semantic_release/data/templates/CHANGELOG.md.j2
+-rw-r--r--   0 root         (0) root         (0)      465 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/semantic_release/data/templates/release_notes.md.j2
+-rw-r--r--   0 root         (0) root         (0)     1020 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/semantic_release/enums.py
+-rw-r--r--   0 root         (0) root         (0)     1159 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/semantic_release/errors.py
+-rw-r--r--   0 root         (0) root         (0)     5581 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/semantic_release/helpers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 02:38:39.143866 python_semantic_release-9.5.0/semantic_release/hvcs/
+-rw-r--r--   0 root         (0) root         (0)      379 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/semantic_release/hvcs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5232 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/semantic_release/hvcs/_base.py
+-rw-r--r--   0 root         (0) root         (0)    11004 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/semantic_release/hvcs/bitbucket.py
+-rw-r--r--   0 root         (0) root         (0)    11450 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/semantic_release/hvcs/gitea.py
+-rw-r--r--   0 root         (0) root         (0)    19965 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/semantic_release/hvcs/github.py
+-rw-r--r--   0 root         (0) root         (0)     7409 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/semantic_release/hvcs/gitlab.py
+-rw-r--r--   0 root         (0) root         (0)      663 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/semantic_release/hvcs/token_auth.py
+-rw-r--r--   0 root         (0) root         (0)     2886 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/semantic_release/hvcs/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 02:38:39.143866 python_semantic_release-9.5.0/semantic_release/version/
+-rw-r--r--   0 root         (0) root         (0)      270 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/semantic_release/version/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16854 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/semantic_release/version/algorithm.py
+-rw-r--r--   0 root         (0) root         (0)     7357 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/semantic_release/version/declaration.py
+-rw-r--r--   0 root         (0) root         (0)     3050 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/semantic_release/version/translator.py
+-rw-r--r--   0 root         (0) root         (0)    14175 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/semantic_release/version/version.py
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-23 02:38:39.163867 python_semantic_release-9.5.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 02:38:39.143866 python_semantic_release-9.5.0/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 02:38:39.147867 python_semantic_release-9.5.0/tests/command_line/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/tests/command_line/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2983 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/tests/command_line/conftest.py
+-rw-r--r--   0 root         (0) root         (0)    11360 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/tests/command_line/test_changelog.py
+-rw-r--r--   0 root         (0) root         (0)     1759 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/tests/command_line/test_generate_config.py
+-rw-r--r--   0 root         (0) root         (0)     6566 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/tests/command_line/test_help.py
+-rw-r--r--   0 root         (0) root         (0)     5255 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/tests/command_line/test_main.py
+-rw-r--r--   0 root         (0) root         (0)     1425 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/tests/command_line/test_publish.py
+-rw-r--r--   0 root         (0) root         (0)    28853 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/tests/command_line/test_version.py
+-rw-r--r--   0 root         (0) root         (0)     2535 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/tests/conftest.py
+-rw-r--r--   0 root         (0) root         (0)     8953 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/tests/const.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 02:38:39.147867 python_semantic_release-9.5.0/tests/fixtures/
+-rw-r--r--   0 root         (0) root         (0)      197 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/tests/fixtures/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      912 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/tests/fixtures/commit_parsers.py
+-rw-r--r--   0 root         (0) root         (0)    11562 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/tests/fixtures/example_project.py
+-rw-r--r--   0 root         (0) root         (0)    13292 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/tests/fixtures/git_repo.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 02:38:39.147867 python_semantic_release-9.5.0/tests/fixtures/repos/
+-rw-r--r--   0 root         (0) root         (0)      142 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/tests/fixtures/repos/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 02:38:39.147867 python_semantic_release-9.5.0/tests/fixtures/repos/git_flow/
+-rw-r--r--   0 root         (0) root         (0)      140 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/tests/fixtures/repos/git_flow/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    21042 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/tests/fixtures/repos/git_flow/repo_w_2_release_channels.py
+-rw-r--r--   0 root         (0) root         (0)    21711 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/tests/fixtures/repos/git_flow/repo_w_3_release_channels.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 02:38:39.147867 python_semantic_release-9.5.0/tests/fixtures/repos/github_flow/
+-rw-r--r--   0 root         (0) root         (0)       71 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/tests/fixtures/repos/github_flow/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15712 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/tests/fixtures/repos/github_flow/repo_w_release_channels.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 02:38:39.151867 python_semantic_release-9.5.0/tests/fixtures/repos/trunk_based_dev/
+-rw-r--r--   0 root         (0) root         (0)      199 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/tests/fixtures/repos/trunk_based_dev/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10463 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/tests/fixtures/repos/trunk_based_dev/repo_w_no_tags.py
+-rw-r--r--   0 root         (0) root         (0)    13604 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/tests/fixtures/repos/trunk_based_dev/repo_w_prereleases.py
+-rw-r--r--   0 root         (0) root         (0)    10698 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/tests/fixtures/repos/trunk_based_dev/repo_w_tags.py
+-rw-r--r--   0 root         (0) root         (0)     4494 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/tests/fixtures/scipy.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 02:38:39.151867 python_semantic_release-9.5.0/tests/scenario/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/tests/scenario/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   127286 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/tests/scenario/test_next_version.py
+-rw-r--r--   0 root         (0) root         (0)    12845 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/tests/scenario/test_release_history.py
+-rw-r--r--   0 root         (0) root         (0)     5074 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/tests/scenario/test_template_render.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 02:38:39.151867 python_semantic_release-9.5.0/tests/unit/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/tests/unit/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 02:38:39.151867 python_semantic_release-9.5.0/tests/unit/semantic_release/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/tests/unit/semantic_release/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 02:38:39.151867 python_semantic_release-9.5.0/tests/unit/semantic_release/changelog/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/tests/unit/semantic_release/changelog/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6222 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/tests/unit/semantic_release/changelog/test_default_changelog.py
+-rw-r--r--   0 root         (0) root         (0)     3560 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/tests/unit/semantic_release/changelog/test_release_notes.py
+-rw-r--r--   0 root         (0) root         (0)     2116 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/tests/unit/semantic_release/changelog/test_template.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 02:38:39.155866 python_semantic_release-9.5.0/tests/unit/semantic_release/cli/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/tests/unit/semantic_release/cli/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5840 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/tests/unit/semantic_release/cli/test_config.py
+-rw-r--r--   0 root         (0) root         (0)     2129 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/tests/unit/semantic_release/cli/test_github_actions_output.py
+-rw-r--r--   0 root         (0) root         (0)     6361 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/tests/unit/semantic_release/cli/test_masking_filter.py
+-rw-r--r--   0 root         (0) root         (0)     4219 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/tests/unit/semantic_release/cli/test_util.py
+-rw-r--r--   0 root         (0) root         (0)      799 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/tests/unit/semantic_release/cli/test_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 02:38:39.155866 python_semantic_release-9.5.0/tests/unit/semantic_release/commit_parser/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/tests/unit/semantic_release/commit_parser/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      140 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/tests/unit/semantic_release/commit_parser/helper.py
+-rw-r--r--   0 root         (0) root         (0)     5952 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/tests/unit/semantic_release/commit_parser/test_angular.py
+-rw-r--r--   0 root         (0) root         (0)     2483 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/tests/unit/semantic_release/commit_parser/test_emoji.py
+-rw-r--r--   0 root         (0) root         (0)      500 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/tests/unit/semantic_release/commit_parser/test_scipy.py
+-rw-r--r--   0 root         (0) root         (0)     2096 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/tests/unit/semantic_release/commit_parser/test_tag.py
+-rw-r--r--   0 root         (0) root         (0)      648 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/tests/unit/semantic_release/commit_parser/test_token.py
+-rw-r--r--   0 root         (0) root         (0)      836 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/tests/unit/semantic_release/commit_parser/test_util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 02:38:39.159867 python_semantic_release-9.5.0/tests/unit/semantic_release/hvcs/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/tests/unit/semantic_release/hvcs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1357 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/tests/unit/semantic_release/hvcs/test__base.py
+-rw-r--r--   0 root         (0) root         (0)    10521 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/tests/unit/semantic_release/hvcs/test_bitbucket.py
+-rw-r--r--   0 root         (0) root         (0)    27246 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/tests/unit/semantic_release/hvcs/test_gitea.py
+-rw-r--r--   0 root         (0) root         (0)    35951 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/tests/unit/semantic_release/hvcs/test_github.py
+-rw-r--r--   0 root         (0) root         (0)    15576 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/tests/unit/semantic_release/hvcs/test_gitlab.py
+-rw-r--r--   0 root         (0) root         (0)      966 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/tests/unit/semantic_release/hvcs/test_token_auth.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/tests/unit/semantic_release/hvcs/test_util.py
+-rw-r--r--   0 root         (0) root         (0)     4507 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/tests/unit/semantic_release/test_helpers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 02:38:39.159867 python_semantic_release-9.5.0/tests/unit/semantic_release/version/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/tests/unit/semantic_release/version/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9605 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/tests/unit/semantic_release/version/test_algorithm.py
+-rw-r--r--   0 root         (0) root         (0)     3874 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/tests/unit/semantic_release/version/test_declaration.py
+-rw-r--r--   0 root         (0) root         (0)     2951 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/tests/unit/semantic_release/version/test_translator.py
+-rw-r--r--   0 root         (0) root         (0)     9714 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/tests/unit/semantic_release/version/test_version.py
+-rw-r--r--   0 root         (0) root         (0)     5551 2024-04-23 02:37:22.000000 python_semantic_release-9.5.0/tests/util.py
```

### Comparing `python_semantic_release-9.4.2/LICENSE` & `python_semantic_release-9.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.4.2/PKG-INFO` & `python_semantic_release-9.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-semantic-release
-Version: 9.4.2
+Version: 9.5.0
 Summary: Automatic Semantic Versioning for Python projects
 Author-email: Rolf Erik Lekang <me@rolflekang.com>
 License: MIT
 Project-URL: changelog, https://github.com/python-semantic-release/python-semantic-release/blob/master/CHANGELOG.md
 Project-URL: documentation, https://python-semantic-release.readthedocs.io
 Project-URL: homepage, https://python-semantic-release.readthedocs.io
 Project-URL: issues, https://github.com/python-semantic-release/python-semantic-release/issues
@@ -49,15 +49,15 @@
 Requires-Dist: pytest-clarity~=1.0; extra == "test"
 Requires-Dist: responses~=0.25.0; extra == "test"
 Requires-Dist: requests-mock~=1.10; extra == "test"
 Requires-Dist: types-pytest-lazy-fixture~=0.6.3; extra == "test"
 Provides-Extra: dev
 Requires-Dist: pre-commit~=3.5; extra == "dev"
 Requires-Dist: tox~=4.11; extra == "dev"
-Requires-Dist: ruff==0.3.5; extra == "dev"
+Requires-Dist: ruff==0.4.1; extra == "dev"
 Provides-Extra: mypy
 Requires-Dist: mypy==1.9.0; extra == "mypy"
 Requires-Dist: types-requests~=2.31.0; extra == "mypy"
 
 Python Semantic Release
 ***********************
```

### Comparing `python_semantic_release-9.4.2/README.rst` & `python_semantic_release-9.5.0/README.rst`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.4.2/docs/Makefile` & `python_semantic_release-9.5.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.4.2/docs/algorithm.rst` & `python_semantic_release-9.5.0/docs/algorithm.rst`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.4.2/docs/automatic-releases/cronjobs.rst` & `python_semantic_release-9.5.0/docs/automatic-releases/cronjobs.rst`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.4.2/docs/automatic-releases/github-actions.rst` & `python_semantic_release-9.5.0/docs/automatic-releases/github-actions.rst`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.4.2/docs/automatic-releases/index.rst` & `python_semantic_release-9.5.0/docs/automatic-releases/index.rst`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.4.2/docs/automatic-releases/travis.rst` & `python_semantic_release-9.5.0/docs/automatic-releases/travis.rst`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.4.2/docs/changelog_templates.rst` & `python_semantic_release-9.5.0/docs/changelog_templates.rst`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.4.2/docs/commands.rst` & `python_semantic_release-9.5.0/docs/commands.rst`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.4.2/docs/commit-parsing.rst` & `python_semantic_release-9.5.0/docs/commit-parsing.rst`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.4.2/docs/conf.py` & `python_semantic_release-9.5.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.4.2/docs/configuration.rst` & `python_semantic_release-9.5.0/docs/configuration.rst`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.4.2/docs/github-action.rst` & `python_semantic_release-9.5.0/docs/github-action.rst`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.4.2/docs/index.rst` & `python_semantic_release-9.5.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.4.2/docs/make.bat` & `python_semantic_release-9.5.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.4.2/docs/migrating_from_v7.rst` & `python_semantic_release-9.5.0/docs/migrating_from_v7.rst`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.4.2/docs/multibranch_releases.rst` & `python_semantic_release-9.5.0/docs/multibranch_releases.rst`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.4.2/docs/strict_mode.rst` & `python_semantic_release-9.5.0/docs/strict_mode.rst`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.4.2/docs/troubleshooting.rst` & `python_semantic_release-9.5.0/docs/troubleshooting.rst`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.4.2/pyproject.toml` & `python_semantic_release-9.5.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # and https://setuptools.pypa.io/en/latest/userguide/pyproject_config.html
 [build-system]
 requires = ["setuptools ~= 69.0", "wheel ~= 0.42"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "python-semantic-release"
-version = "9.4.2"
+version = "9.5.0"
 description = "Automatic Semantic Versioning for Python projects"
 requires-python = ">=3.8"
 license = { text = "MIT" }
 classifiers = [
   "Programming Language :: Python",
   "Programming Language :: Python :: 3",
   "Programming Language :: Python :: 3.8",
@@ -67,15 +67,15 @@
   "responses ~= 0.25.0",
   "requests-mock ~= 1.10",
   "types-pytest-lazy-fixture ~= 0.6.3",
 ]
 dev = [
   "pre-commit ~= 3.5",
   "tox ~= 4.11",
-  "ruff == 0.3.5"
+  "ruff == 0.4.1"
 ]
 mypy = [
   "mypy == 1.9.0",
   "types-requests ~= 2.31.0"
 ]
 
 [tool.pytest.ini_options]
@@ -359,74 +359,46 @@
 sections = { "tests" = ["tests"] }
 
 [tool.vulture]
 ignore_names = ["change_to_ex_proj_dir", "init_example_project"]
 
 [tool.semantic_release]
 logging_use_named_masks = true
-tag_format = "v{version}"
 commit_parser = "angular"
-commit_author = "semantic-release <semantic-release>"
-commit_message = "{version}\n\nAutomatically generated by python-semantic-release"
 build_command = """
     python -m pip install build~=0.10.0
     python -m build .
 """
 major_on_zero = true
-assets = []
 version_variables = ["semantic_release/__init__.py:__version__"]
 version_toml = ["pyproject.toml:project.version"]
 
-[tool.semantic_release.commit_parser_options]
-allowed_tags = [
-  "build",
-  "chore",
-  "ci",
-  "docs",
-  "feat",
-  "fix",
-  "perf",
-  "style",
-  "refactor",
-  "test",
-]
-minor_tags = ["feat"]
-patch_tags = ["fix", "perf"]
-
 [tool.semantic_release.changelog]
-template_dir = "templates"
-changelog_file = "CHANGELOG.md"
-exclude_commit_patterns = []
-
-[tool.semantic_release.changelog.environment]
-block_start_string = "{%"
-block_end_string = "%}"
-variable_start_string = "{{"
-variable_end_string = "}}"
-comment_start_string = "{#"
-comment_end_string = "#}"
-trim_blocks = false
-lstrip_blocks = false
-newline_sequence = "\n"
-keep_trailing_newline = false
-extensions = []
-autoescape = true
+exclude_commit_patterns = [
+  '''chore(?:\([^)]*?\))?: .+''',
+  '''ci(?:\([^)]*?\))?: .+''',
+  '''refactor(?:\([^)]*?\))?: .+''',
+  '''style(?:\([^)]*?\))?: .+''',
+  '''test(?:\([^)]*?\))?: .+''',
+  '''build\((?!deps\): .+)''',
+  '''Merged? .*''',
+  '''Initial Commit.*''',
+  # Old semantic-release version commits
+  '''^\d+\.\d+\.\d+''',
+]
 
 [tool.semantic_release.branches.main]
 match = "(main|master)"
 prerelease = false
 prerelease_token = "rc"
 
-[tool.semantic_release.branches."8.0.x"]
-match = "8.0.x"
+[tool.semantic_release.branches.alpha]
+match = "^(feat|fix|perf)/.+"
 prerelease = true
-prerelease_token = "rc"
+prerelease_token = "alpha"
 
 [tool.semantic_release.remote]
-name = "origin"
 type = "github"
-ignore_token_for_push = false
 token = { env = "GH_TOKEN" }
 
 [tool.semantic_release.publish]
-dist_glob_patterns = ["dist/*"]
 upload_to_vcs_release = true
```

### Comparing `python_semantic_release-9.4.2/python_semantic_release.egg-info/PKG-INFO` & `python_semantic_release-9.5.0/python_semantic_release.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-semantic-release
-Version: 9.4.2
+Version: 9.5.0
 Summary: Automatic Semantic Versioning for Python projects
 Author-email: Rolf Erik Lekang <me@rolflekang.com>
 License: MIT
 Project-URL: changelog, https://github.com/python-semantic-release/python-semantic-release/blob/master/CHANGELOG.md
 Project-URL: documentation, https://python-semantic-release.readthedocs.io
 Project-URL: homepage, https://python-semantic-release.readthedocs.io
 Project-URL: issues, https://github.com/python-semantic-release/python-semantic-release/issues
@@ -49,15 +49,15 @@
 Requires-Dist: pytest-clarity~=1.0; extra == "test"
 Requires-Dist: responses~=0.25.0; extra == "test"
 Requires-Dist: requests-mock~=1.10; extra == "test"
 Requires-Dist: types-pytest-lazy-fixture~=0.6.3; extra == "test"
 Provides-Extra: dev
 Requires-Dist: pre-commit~=3.5; extra == "dev"
 Requires-Dist: tox~=4.11; extra == "dev"
-Requires-Dist: ruff==0.3.5; extra == "dev"
+Requires-Dist: ruff==0.4.1; extra == "dev"
 Provides-Extra: mypy
 Requires-Dist: mypy==1.9.0; extra == "mypy"
 Requires-Dist: types-requests~=2.31.0; extra == "mypy"
 
 Python Semantic Release
 ***********************
```

### Comparing `python_semantic_release-9.4.2/python_semantic_release.egg-info/SOURCES.txt` & `python_semantic_release-9.5.0/python_semantic_release.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.4.2/python_semantic_release.egg-info/requires.txt` & `python_semantic_release-9.5.0/python_semantic_release.egg-info/requires.txt`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 pydantic~=2.0
 rich~=13.0
 shellingham~=1.5
 
 [dev]
 pre-commit~=3.5
 tox~=4.11
-ruff==0.3.5
+ruff==0.4.1
 
 [docs]
 Sphinx~=6.0
 sphinxcontrib-apidoc==0.5.0
 sphinx-autobuild==2024.2.4
 furo~=2024.1
```

### Comparing `python_semantic_release-9.4.2/semantic_release/__init__.py` & `python_semantic_release-9.5.0/semantic_release/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 from semantic_release.version import (
     Version,
     VersionTranslator,
     next_version,
     tags_and_versions,
 )
 
-__version__ = "9.4.2"
+__version__ = "9.5.0"
 
 
 def setup_hook(argv: list[str]) -> None:
     """
     A hook to be used in setup.py to enable `python setup.py publish`.
 
     :param argv: sys.argv
```

### Comparing `python_semantic_release-9.4.2/semantic_release/changelog/context.py` & `python_semantic_release-9.5.0/semantic_release/changelog/context.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.4.2/semantic_release/changelog/release_history.py` & `python_semantic_release-9.5.0/semantic_release/changelog/release_history.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.4.2/semantic_release/changelog/template.py` & `python_semantic_release-9.5.0/semantic_release/changelog/template.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.4.2/semantic_release/cli/commands/changelog.py` & `python_semantic_release-9.5.0/semantic_release/cli/commands/changelog.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.4.2/semantic_release/cli/commands/cli_context.py` & `python_semantic_release-9.5.0/semantic_release/cli/commands/cli_context.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.4.2/semantic_release/cli/commands/generate_config.py` & `python_semantic_release-9.5.0/semantic_release/cli/commands/generate_config.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.4.2/semantic_release/cli/commands/main.py` & `python_semantic_release-9.5.0/semantic_release/cli/commands/main.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.4.2/semantic_release/cli/commands/publish.py` & `python_semantic_release-9.5.0/semantic_release/cli/commands/publish.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.4.2/semantic_release/cli/commands/version.py` & `python_semantic_release-9.5.0/semantic_release/cli/commands/version.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.4.2/semantic_release/cli/common.py` & `python_semantic_release-9.5.0/semantic_release/cli/common.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.4.2/semantic_release/cli/config.py` & `python_semantic_release-9.5.0/semantic_release/cli/config.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.4.2/semantic_release/cli/github_actions_output.py` & `python_semantic_release-9.5.0/semantic_release/cli/github_actions_output.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.4.2/semantic_release/cli/masking_filter.py` & `python_semantic_release-9.5.0/semantic_release/cli/masking_filter.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.4.2/semantic_release/cli/util.py` & `python_semantic_release-9.5.0/semantic_release/cli/util.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.4.2/semantic_release/commit_parser/__init__.py` & `python_semantic_release-9.5.0/semantic_release/commit_parser/__init__.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.4.2/semantic_release/commit_parser/_base.py` & `python_semantic_release-9.5.0/semantic_release/commit_parser/_base.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.4.2/semantic_release/commit_parser/angular.py` & `python_semantic_release-9.5.0/semantic_release/commit_parser/angular.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.4.2/semantic_release/commit_parser/emoji.py` & `python_semantic_release-9.5.0/semantic_release/commit_parser/emoji.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.4.2/semantic_release/commit_parser/scipy.py` & `python_semantic_release-9.5.0/semantic_release/commit_parser/scipy.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.4.2/semantic_release/commit_parser/tag.py` & `python_semantic_release-9.5.0/semantic_release/commit_parser/tag.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.4.2/semantic_release/commit_parser/token.py` & `python_semantic_release-9.5.0/semantic_release/commit_parser/token.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.4.2/semantic_release/commit_parser/util.py` & `python_semantic_release-9.5.0/semantic_release/commit_parser/util.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.4.2/semantic_release/const.py` & `python_semantic_release-9.5.0/semantic_release/const.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.4.2/semantic_release/data/templates/CHANGELOG.md.j2` & `python_semantic_release-9.5.0/semantic_release/data/templates/CHANGELOG.md.j2`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.4.2/semantic_release/enums.py` & `python_semantic_release-9.5.0/semantic_release/enums.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.4.2/semantic_release/errors.py` & `python_semantic_release-9.5.0/semantic_release/errors.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.4.2/semantic_release/helpers.py` & `python_semantic_release-9.5.0/semantic_release/helpers.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.4.2/semantic_release/hvcs/_base.py` & `python_semantic_release-9.5.0/semantic_release/hvcs/_base.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.4.2/semantic_release/hvcs/bitbucket.py` & `python_semantic_release-9.5.0/semantic_release/hvcs/bitbucket.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.4.2/semantic_release/hvcs/gitea.py` & `python_semantic_release-9.5.0/semantic_release/hvcs/gitea.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.4.2/semantic_release/hvcs/github.py` & `python_semantic_release-9.5.0/semantic_release/hvcs/github.py`

 * *Files 11% similar despite different names*

```diff
@@ -46,26 +46,36 @@
 
 
 class Github(HvcsBase):
     """
     GitHub HVCS interface for interacting with GitHub repositories
 
     This class supports the following products:
+
         - GitHub Free, Pro, & Team
         - GitHub Enterprise Cloud
-
-    This class does not support the following products:
         - GitHub Enterprise Server (on-premises installations)
+
+    This interface does its best to detect which product is configured based
+    on the provided domain. If it is the official `github.com`, the default
+    domain, then it is considered as GitHub Enterprise Cloud which uses the
+    subdomain `api.github.com` for api communication.
+
+    If the provided domain is anything else, than it is assumed to be communicating
+    with an on-premise or 3rd-party maintained GitHub instance which matches with
+    the GitHub Enterprise Server product. The on-prem server product uses a
+    path prefix for handling api requests which is configured to be
+    `server.domain/api/v3` based on the documentation in April 2024.
     """
 
-    # TODO: Add support for GitHub Enterprise Server (on-premises installations)
-    #       DEFAULT_ONPREM_API_PATH = "/api/v3"
     DEFAULT_DOMAIN = "github.com"
     DEFAULT_API_SUBDOMAIN_PREFIX = "api"
     DEFAULT_API_DOMAIN = f"{DEFAULT_API_SUBDOMAIN_PREFIX}.{DEFAULT_DOMAIN}"
+    DEFAULT_API_PATH_CLOUD = "/"  # no path prefix!
+    DEFAULT_API_PATH_ONPREM = "/api/v3"
     DEFAULT_ENV_TOKEN_NAME = "GH_TOKEN"  # noqa: S105
 
     def __init__(
         self,
         remote_url: str,
         *,
         hvcs_domain: str | None = None,
@@ -113,18 +123,23 @@
         api_domain_parts = parse_url(
             hvcs_api_domain
             or os.getenv("GITHUB_API_URL", "")
             or Url(
                 # infer from Domain url and prepend the default api subdomain
                 **{
                     **self.hvcs_domain._asdict(),
-                    "host": f"{self.DEFAULT_API_SUBDOMAIN_PREFIX}.{self.hvcs_domain.host}",
-                    "path": "",
+                    "host": self.hvcs_domain.host,
+                    "path": str(
+                        PurePosixPath(
+                            str.lstrip(self.hvcs_domain.path or "", "/") or "/",
+                            self.DEFAULT_API_PATH_ONPREM.lstrip("/"),
+                        )
+                    ),
                 }
-            ).url
+            ).url.rstrip("/")
         )
 
         if api_domain_parts.scheme == "http" and not allow_insecure:
             raise ValueError("Insecure connections are currently disabled.")
 
         if not api_domain_parts.scheme:
             new_scheme = "http" if allow_insecure else "https"
@@ -134,24 +149,74 @@
 
         if api_domain_parts.scheme not in ["http", "https"]:
             raise ValueError(
                 f"Invalid scheme {api_domain_parts.scheme} for api domain {api_domain_parts.host}. "
                 "Only http and https are supported."
             )
 
-        # Strip any auth, query or fragment from the domain
-        self.api_url = parse_url(
+        # As GitHub Enterprise Cloud and GitHub Enterprise Server (on-prem) have different api locations
+        # lets check what we have been given and set the api url accordingly
+        #   NOTE: Github Server (on premise) uses a path prefix '/api/v3' for the api
+        #         while GitHub Enterprise Cloud uses a separate subdomain as the base
+        is_github_cloud = bool(self.hvcs_domain.url == f"https://{self.DEFAULT_DOMAIN}")
+
+        # Calculate out the api url that we expect for GitHub Cloud
+        default_cloud_api_url = parse_url(
             Url(
-                scheme=api_domain_parts.scheme,
-                host=api_domain_parts.host,
-                port=api_domain_parts.port,
-                path=str(PurePosixPath(api_domain_parts.path or "/")),
+                # set api domain and append the default api path
+                **{
+                    **self.hvcs_domain._asdict(),
+                    "host": f"{self.DEFAULT_API_DOMAIN}",
+                    "path": self.DEFAULT_API_PATH_CLOUD,
+                }
             ).url.rstrip("/")
         )
 
+        if (
+            is_github_cloud
+            and hvcs_api_domain
+            and api_domain_parts.url not in default_cloud_api_url.url
+        ):
+            # Api was provied but is not a subset of the expected one, raise an error
+            # we check for a subset because the user may not have provided the full api path
+            # but the correct domain.  If they didn't, then we are erroring out here.
+            raise ValueError(
+                f"Invalid api domain {api_domain_parts.url} for GitHub Enterprise Cloud. "
+                f"Expected {default_cloud_api_url.url}."
+            )
+
+        # Set the api url to the default cloud one if we are on cloud, otherwise
+        # use the verified api domain for a on-prem server
+        self.api_url = (
+            default_cloud_api_url
+            if is_github_cloud
+            else parse_url(
+                # Strip any auth, query or fragment from the domain
+                Url(
+                    scheme=api_domain_parts.scheme,
+                    host=api_domain_parts.host,
+                    port=api_domain_parts.port,
+                    path=str(
+                        PurePosixPath(
+                            # pass any custom server prefix path but ensure we don't
+                            # double up the api path in the case the user provided it
+                            str.replace(
+                                api_domain_parts.path or "",
+                                self.DEFAULT_API_PATH_ONPREM,
+                                "",
+                            ).lstrip("/")
+                            or "/",
+                            # apply the on-prem api path
+                            self.DEFAULT_API_PATH_ONPREM.lstrip("/"),
+                        )
+                    ),
+                ).url.rstrip("/")
+            )
+        )
+
     @lru_cache(maxsize=1)
     def _get_repository_owner_and_name(self) -> tuple[str, str]:
         # Github actions context
         if "GITHUB_REPOSITORY" in os.environ:
             log.debug("getting repository owner and name from environment variables")
             owner, name = os.environ["GITHUB_REPOSITORY"].rsplit("/", 1)
             return owner, name
@@ -415,15 +480,15 @@
         fragment: str | None = None,
     ) -> str:
         overrides = dict(
             filter(
                 lambda x: x[1] is not None,
                 {
                     "auth": auth,
-                    "path": str(PurePosixPath("/", path)),
+                    "path": str(PurePosixPath("/", path.lstrip("/"))),
                     "query": query,
                     "fragment": fragment,
                 }.items(),
             )
         )
         return Url(
             **{
@@ -435,17 +500,31 @@
     def create_server_url(
         self,
         path: str,
         auth: str | None = None,
         query: str | None = None,
         fragment: str | None = None,
     ) -> str:
-        return self._derive_url(self.hvcs_domain, path, auth, query, fragment)
+        # Ensure any path prefix is transfered but not doubled up on the derived url
+        return self._derive_url(
+            self.hvcs_domain,
+            path=f"{self.hvcs_domain.path or ''}/{path.lstrip(self.hvcs_domain.path)}",
+            auth=auth,
+            query=query,
+            fragment=fragment,
+        )
 
     def create_api_url(
         self,
         endpoint: str,
         auth: str | None = None,
         query: str | None = None,
         fragment: str | None = None,
     ) -> str:
-        return self._derive_url(self.api_url, endpoint, auth, query, fragment)
+        # Ensure any api path prefix is transfered but not doubled up on the derived api url
+        return self._derive_url(
+            self.api_url,
+            path=f"{self.api_url.path or ''}/{endpoint.lstrip(self.api_url.path)}",
+            auth=auth,
+            query=query,
+            fragment=fragment,
+        )
```

### Comparing `python_semantic_release-9.4.2/semantic_release/hvcs/gitlab.py` & `python_semantic_release-9.5.0/semantic_release/hvcs/gitlab.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.4.2/semantic_release/hvcs/token_auth.py` & `python_semantic_release-9.5.0/semantic_release/hvcs/token_auth.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.4.2/semantic_release/hvcs/util.py` & `python_semantic_release-9.5.0/semantic_release/hvcs/util.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.4.2/semantic_release/version/algorithm.py` & `python_semantic_release-9.5.0/semantic_release/version/algorithm.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.4.2/semantic_release/version/declaration.py` & `python_semantic_release-9.5.0/semantic_release/version/declaration.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.4.2/semantic_release/version/translator.py` & `python_semantic_release-9.5.0/semantic_release/version/translator.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.4.2/semantic_release/version/version.py` & `python_semantic_release-9.5.0/semantic_release/version/version.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.4.2/tests/command_line/conftest.py` & `python_semantic_release-9.5.0/tests/command_line/conftest.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.4.2/tests/command_line/test_changelog.py` & `python_semantic_release-9.5.0/tests/command_line/test_changelog.py`

 * *Files 2% similar despite different names*

```diff
@@ -238,17 +238,15 @@
     mock_adapter.register_uri(
         method=requests_mock.ANY, url=requests_mock.ANY, json={"id": 10001}
     )
     session.mount("http://", mock_adapter)
     session.mount("https://", mock_adapter)
 
     expected_request_url = "{api_url}/repos/{owner}/{repo_name}/releases".format(
-        # TODO: Fix as this is likely not correct given a custom domain and the
-        # use of GitHub which would be GitHub Enterprise Server which we don't yet support
-        api_url=f"https://api.{EXAMPLE_HVCS_DOMAIN}",  # GitHub API URL
+        api_url=f"https://{EXAMPLE_HVCS_DOMAIN}/api/v3",  # GitHub API URL
         owner=EXAMPLE_REPO_OWNER,
         repo_name=EXAMPLE_REPO_NAME,
     )
 
     # Patch out env vars that affect changelog URLs but only get set in e.g.
     # Github actions
     with mock.patch(
```

### Comparing `python_semantic_release-9.4.2/tests/command_line/test_generate_config.py` & `python_semantic_release-9.5.0/tests/command_line/test_generate_config.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.4.2/tests/command_line/test_help.py` & `python_semantic_release-9.5.0/tests/command_line/test_help.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.4.2/tests/command_line/test_main.py` & `python_semantic_release-9.5.0/tests/command_line/test_main.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.4.2/tests/command_line/test_publish.py` & `python_semantic_release-9.5.0/tests/command_line/test_publish.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.4.2/tests/command_line/test_version.py` & `python_semantic_release-9.5.0/tests/command_line/test_version.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.4.2/tests/conftest.py` & `python_semantic_release-9.5.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.4.2/tests/const.py` & `python_semantic_release-9.5.0/tests/const.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.4.2/tests/fixtures/commit_parsers.py` & `python_semantic_release-9.5.0/tests/fixtures/commit_parsers.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.4.2/tests/fixtures/example_project.py` & `python_semantic_release-9.5.0/tests/fixtures/example_project.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.4.2/tests/fixtures/git_repo.py` & `python_semantic_release-9.5.0/tests/fixtures/git_repo.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.4.2/tests/fixtures/repos/git_flow/repo_w_2_release_channels.py` & `python_semantic_release-9.5.0/tests/fixtures/repos/git_flow/repo_w_2_release_channels.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.4.2/tests/fixtures/repos/git_flow/repo_w_3_release_channels.py` & `python_semantic_release-9.5.0/tests/fixtures/repos/git_flow/repo_w_3_release_channels.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.4.2/tests/fixtures/repos/github_flow/repo_w_release_channels.py` & `python_semantic_release-9.5.0/tests/fixtures/repos/github_flow/repo_w_release_channels.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.4.2/tests/fixtures/repos/trunk_based_dev/repo_w_no_tags.py` & `python_semantic_release-9.5.0/tests/fixtures/repos/trunk_based_dev/repo_w_no_tags.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.4.2/tests/fixtures/repos/trunk_based_dev/repo_w_prereleases.py` & `python_semantic_release-9.5.0/tests/fixtures/repos/trunk_based_dev/repo_w_prereleases.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.4.2/tests/fixtures/repos/trunk_based_dev/repo_w_tags.py` & `python_semantic_release-9.5.0/tests/fixtures/repos/trunk_based_dev/repo_w_tags.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.4.2/tests/fixtures/scipy.py` & `python_semantic_release-9.5.0/tests/fixtures/scipy.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.4.2/tests/scenario/test_next_version.py` & `python_semantic_release-9.5.0/tests/scenario/test_next_version.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.4.2/tests/scenario/test_release_history.py` & `python_semantic_release-9.5.0/tests/scenario/test_release_history.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.4.2/tests/scenario/test_template_render.py` & `python_semantic_release-9.5.0/tests/scenario/test_template_render.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.4.2/tests/unit/semantic_release/changelog/test_default_changelog.py` & `python_semantic_release-9.5.0/tests/unit/semantic_release/changelog/test_default_changelog.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.4.2/tests/unit/semantic_release/changelog/test_release_notes.py` & `python_semantic_release-9.5.0/tests/unit/semantic_release/changelog/test_release_notes.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.4.2/tests/unit/semantic_release/changelog/test_template.py` & `python_semantic_release-9.5.0/tests/unit/semantic_release/changelog/test_template.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.4.2/tests/unit/semantic_release/cli/test_config.py` & `python_semantic_release-9.5.0/tests/unit/semantic_release/cli/test_config.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.4.2/tests/unit/semantic_release/cli/test_github_actions_output.py` & `python_semantic_release-9.5.0/tests/unit/semantic_release/cli/test_github_actions_output.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.4.2/tests/unit/semantic_release/cli/test_masking_filter.py` & `python_semantic_release-9.5.0/tests/unit/semantic_release/cli/test_masking_filter.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.4.2/tests/unit/semantic_release/cli/test_util.py` & `python_semantic_release-9.5.0/tests/unit/semantic_release/cli/test_util.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.4.2/tests/unit/semantic_release/cli/test_version.py` & `python_semantic_release-9.5.0/tests/unit/semantic_release/cli/test_version.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.4.2/tests/unit/semantic_release/commit_parser/test_angular.py` & `python_semantic_release-9.5.0/tests/unit/semantic_release/commit_parser/test_angular.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.4.2/tests/unit/semantic_release/commit_parser/test_emoji.py` & `python_semantic_release-9.5.0/tests/unit/semantic_release/commit_parser/test_emoji.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.4.2/tests/unit/semantic_release/commit_parser/test_tag.py` & `python_semantic_release-9.5.0/tests/unit/semantic_release/commit_parser/test_tag.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.4.2/tests/unit/semantic_release/commit_parser/test_token.py` & `python_semantic_release-9.5.0/tests/unit/semantic_release/commit_parser/test_token.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.4.2/tests/unit/semantic_release/commit_parser/test_util.py` & `python_semantic_release-9.5.0/tests/unit/semantic_release/commit_parser/test_util.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.4.2/tests/unit/semantic_release/hvcs/test__base.py` & `python_semantic_release-9.5.0/tests/unit/semantic_release/hvcs/test__base.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.4.2/tests/unit/semantic_release/hvcs/test_bitbucket.py` & `python_semantic_release-9.5.0/tests/unit/semantic_release/hvcs/test_bitbucket.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.4.2/tests/unit/semantic_release/hvcs/test_gitea.py` & `python_semantic_release-9.5.0/tests/unit/semantic_release/hvcs/test_gitea.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.4.2/tests/unit/semantic_release/hvcs/test_github.py` & `python_semantic_release-9.5.0/tests/unit/semantic_release/hvcs/test_github.py`

 * *Files 6% similar despite different names*

```diff
@@ -51,96 +51,145 @@
             "expected_hvcs_domain",
             "expected_hvcs_api_url",
             "insecure",
         ],
     ),
     [
         (
-            # Default values
+            # Default values (GitHub Enterprise Cloud)
             {},
             None,
             None,
-            f"https://{Github.DEFAULT_DOMAIN}",
-            f"https://{Github.DEFAULT_API_DOMAIN}",
+            "https://github.com",
+            "https://api.github.com",
+            False,
+        ),
+        (
+            # Explicitly set default values (GitHub Enterprise Cloud)
+            {},
+            Github.DEFAULT_DOMAIN,
+            Github.DEFAULT_API_DOMAIN,
+            "https://github.com",
+            "https://api.github.com",
+            False,
+        ),
+        (
+            # Pull both locations from environment (GitHub Actions on Cloud)
+            {
+                "GITHUB_SERVER_URL": f"https://{Github.DEFAULT_DOMAIN}",
+                "GITHUB_API_URL": f"https://{Github.DEFAULT_API_DOMAIN}",
+            },
+            None,
+            None,
+            "https://github.com",
+            "https://api.github.com",
+            False,
+        ),
+        (
+            # Explicitly set custom values with full api path
+            {},
+            EXAMPLE_HVCS_DOMAIN,
+            f"{EXAMPLE_HVCS_DOMAIN}{Github.DEFAULT_API_PATH_ONPREM}",
+            f"https://{EXAMPLE_HVCS_DOMAIN}",
+            f"https://{EXAMPLE_HVCS_DOMAIN}{Github.DEFAULT_API_PATH_ONPREM}",
+            False,
+        ),
+        (
+            # Explicitly defined api as subdomain
+            # POSSIBLY WRONG ASSUMPTION of Api path for GitHub Enterprise Server (On Prem)
+            {},
+            f"https://{EXAMPLE_HVCS_DOMAIN}",
+            f"https://api.{EXAMPLE_HVCS_DOMAIN}",
+            f"https://{EXAMPLE_HVCS_DOMAIN}",
+            f"https://api.{EXAMPLE_HVCS_DOMAIN}{Github.DEFAULT_API_PATH_ONPREM}",
+            False,
+        ),
+        (
+            # Custom domain with path prefix
+            {},
+            "special.custom.server/vcs",
+            None,
+            "https://special.custom.server/vcs",
+            "https://special.custom.server/vcs/api/v3",
             False,
         ),
         (
             # Gather domain from environment & imply api domain from server domain
             {"GITHUB_SERVER_URL": "https://special.custom.server/"},
             None,
             None,
             "https://special.custom.server",
-            "https://api.special.custom.server",
+            "https://special.custom.server/api/v3",
             False,
         ),
         (
-            # Pull both locations from environment
+            # Pull both locations from environment (On-prem Actions Env)
             {
                 "GITHUB_SERVER_URL": "https://special.custom.server/",
-                "GITHUB_API_URL": "https://api2.special.custom.server/",
+                "GITHUB_API_URL": "https://special.custom.server/api/v3",
             },
             None,
             None,
             "https://special.custom.server",
-            "https://api2.special.custom.server",
+            "https://special.custom.server/api/v3",
             False,
         ),
         (
             # Ignore environment & use provided parameter value (ie from user config)
             # then infer api domain from the parameter value based on default GitHub configurations
             {"GITHUB_SERVER_URL": "https://special.custom.server/vcs/"},
             f"https://{EXAMPLE_HVCS_DOMAIN}",
             None,
             f"https://{EXAMPLE_HVCS_DOMAIN}",
-            f"https://api.{EXAMPLE_HVCS_DOMAIN}",
+            f"https://{EXAMPLE_HVCS_DOMAIN}/api/v3",
             False,
         ),
         (
             # Ignore environment & use provided parameter value (ie from user config)
             {"GITHUB_API_URL": "https://api.special.custom.server/"},
             f"https://{EXAMPLE_HVCS_DOMAIN}",
-            f"https://api.{EXAMPLE_HVCS_DOMAIN}",
+            f"https://{EXAMPLE_HVCS_DOMAIN}/api/v3",
             f"https://{EXAMPLE_HVCS_DOMAIN}",
-            f"https://api.{EXAMPLE_HVCS_DOMAIN}",
+            f"https://{EXAMPLE_HVCS_DOMAIN}/api/v3",
             False,
         ),
         (
             # Allow insecure http connections explicitly
             {},
             f"http://{EXAMPLE_HVCS_DOMAIN}",
-            f"http://api.{EXAMPLE_HVCS_DOMAIN}",
+            f"http://{EXAMPLE_HVCS_DOMAIN}/api/v3",
             f"http://{EXAMPLE_HVCS_DOMAIN}",
-            f"http://api.{EXAMPLE_HVCS_DOMAIN}",
+            f"http://{EXAMPLE_HVCS_DOMAIN}/api/v3",
             True,
         ),
         (
             # Allow insecure http connections explicitly & imply insecure api domain
             {},
             f"http://{EXAMPLE_HVCS_DOMAIN}",
             None,
             f"http://{EXAMPLE_HVCS_DOMAIN}",
-            f"http://api.{EXAMPLE_HVCS_DOMAIN}",
+            f"http://{EXAMPLE_HVCS_DOMAIN}/api/v3",
             True,
         ),
         (
             # Infer insecure connection from user configuration
             {},
             EXAMPLE_HVCS_DOMAIN,
-            f"api.{EXAMPLE_HVCS_DOMAIN}",
+            EXAMPLE_HVCS_DOMAIN,
             f"http://{EXAMPLE_HVCS_DOMAIN}",
-            f"http://api.{EXAMPLE_HVCS_DOMAIN}",
+            f"http://{EXAMPLE_HVCS_DOMAIN}/api/v3",
             True,
         ),
         (
             # Infer insecure connection from user configuration & imply insecure api domain
             {},
             EXAMPLE_HVCS_DOMAIN,
             None,
             f"http://{EXAMPLE_HVCS_DOMAIN}",
-            f"http://api.{EXAMPLE_HVCS_DOMAIN}",
+            f"http://{EXAMPLE_HVCS_DOMAIN}/api/v3",
             True,
         ),
     ],
 )
 @pytest.mark.parametrize(
     "remote_url",
     [
```

### Comparing `python_semantic_release-9.4.2/tests/unit/semantic_release/hvcs/test_gitlab.py` & `python_semantic_release-9.5.0/tests/unit/semantic_release/hvcs/test_gitlab.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.4.2/tests/unit/semantic_release/hvcs/test_token_auth.py` & `python_semantic_release-9.5.0/tests/unit/semantic_release/hvcs/test_token_auth.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.4.2/tests/unit/semantic_release/test_helpers.py` & `python_semantic_release-9.5.0/tests/unit/semantic_release/test_helpers.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.4.2/tests/unit/semantic_release/version/test_algorithm.py` & `python_semantic_release-9.5.0/tests/unit/semantic_release/version/test_algorithm.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.4.2/tests/unit/semantic_release/version/test_declaration.py` & `python_semantic_release-9.5.0/tests/unit/semantic_release/version/test_declaration.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.4.2/tests/unit/semantic_release/version/test_translator.py` & `python_semantic_release-9.5.0/tests/unit/semantic_release/version/test_translator.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.4.2/tests/unit/semantic_release/version/test_version.py` & `python_semantic_release-9.5.0/tests/unit/semantic_release/version/test_version.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.4.2/tests/util.py` & `python_semantic_release-9.5.0/tests/util.py`

 * *Files identical despite different names*

