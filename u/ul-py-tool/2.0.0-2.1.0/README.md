# Comparing `tmp/ul-py-tool-2.0.0.tar.gz` & `tmp/ul-py-tool-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ul-py-tool-2.0.0.tar", last modified: Thu Apr  4 07:32:57 2024, max compression
+gzip compressed data, was "ul-py-tool-2.1.0.tar", last modified: Fri Apr 12 08:45:40 2024, max compression
```

## Comparing `ul-py-tool-2.0.0.tar` & `ul-py-tool-2.1.0.tar`

### file list

```diff
@@ -1,70 +1,70 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 07:32:57.359489 ul-py-tool-2.0.0/
--rw-r--r--   0 root         (0) root         (0)     3120 2024-04-04 07:32:57.359489 ul-py-tool-2.0.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2468 2023-04-27 10:19:15.000000 ul-py-tool-2.0.0/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-04 07:32:57.359489 ul-py-tool-2.0.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     2154 2024-04-04 07:32:56.000000 ul-py-tool-2.0.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 07:32:57.299486 ul-py-tool-2.0.0/ul_py_tool/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-04 07:32:56.000000 ul-py-tool-2.0.0/ul_py_tool/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 07:32:57.299486 ul-py-tool-2.0.0/ul_py_tool/__tests__/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-04 07:32:56.000000 ul-py-tool-2.0.0/ul_py_tool/__tests__/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       54 2022-08-06 16:21:13.000000 ul-py-tool-2.0.0/ul_py_tool/__tests__/conftest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 07:32:57.319487 ul-py-tool-2.0.0/ul_py_tool/commands/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-04 07:32:56.000000 ul-py-tool-2.0.0/ul_py_tool/commands/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2515 2023-04-27 10:19:15.000000 ul-py-tool-2.0.0/ul_py_tool/commands/cmd.py
--rw-rw-rw-   0 root         (0) root         (0)     5321 2023-06-14 11:47:43.000000 ul-py-tool-2.0.0/ul_py_tool/commands/cmd_build_images.py
--rw-rw-rw-   0 root         (0) root         (0)      826 2023-04-27 10:19:15.000000 ul-py-tool-2.0.0/ul_py_tool/commands/cmd_cleanup.py
--rw-rw-rw-   0 root         (0) root         (0)      267 2023-04-27 10:19:15.000000 ul-py-tool-2.0.0/ul_py_tool/commands/cmd_fix_own.py
--rw-rw-rw-   0 root         (0) root         (0)     2463 2023-04-27 10:19:15.000000 ul-py-tool-2.0.0/ul_py_tool/commands/cmd_fmt.py
--rw-rw-rw-   0 root         (0) root         (0)     2856 2022-08-10 16:15:33.000000 ul-py-tool-2.0.0/ul_py_tool/commands/cmd_install.py
--rw-rw-rw-   0 root         (0) root         (0)    33467 2024-02-13 13:05:21.000000 ul-py-tool-2.0.0/ul_py_tool/commands/cmd_lint.py
--rw-rw-rw-   0 root         (0) root         (0)    11939 2023-09-06 08:11:08.000000 ul-py-tool-2.0.0/ul_py_tool/commands/cmd_release.py
--rw-rw-rw-   0 root         (0) root         (0)     7296 2024-02-13 13:05:21.000000 ul-py-tool-2.0.0/ul_py_tool/commands/cmd_release_dcf.py
--rw-rw-rw-   0 root         (0) root         (0)     1133 2024-02-13 13:05:21.000000 ul-py-tool-2.0.0/ul_py_tool/commands/cmd_release_dcf_dev.py
--rw-rw-rw-   0 root         (0) root         (0)     5342 2024-04-04 07:32:56.000000 ul-py-tool-2.0.0/ul_py_tool/commands/cmd_service_version.py
--rw-rw-rw-   0 root         (0) root         (0)     3098 2022-08-05 16:32:51.000000 ul-py-tool-2.0.0/ul_py_tool/commands/cmd_stats.py
--rw-rw-rw-   0 root         (0) root         (0)     3597 2023-04-27 10:19:15.000000 ul-py-tool-2.0.0/ul_py_tool/commands/cmd_test.py
--rw-rw-rw-   0 root         (0) root         (0)     5475 2023-04-27 10:19:15.000000 ul-py-tool-2.0.0/ul_py_tool/commands/cmd_test_secrets.py
--rw-rw-rw-   0 root         (0) root         (0)     6001 2023-04-27 10:19:15.000000 ul-py-tool-2.0.0/ul_py_tool/commands/cmd_version.py
--rw-rw-rw-   0 root         (0) root         (0)     2025 2022-08-10 16:15:33.000000 ul-py-tool-2.0.0/ul_py_tool/commands/cmp_outdated.py
--rw-rw-rw-   0 root         (0) root         (0)     1194 2024-02-21 10:56:17.000000 ul-py-tool-2.0.0/ul_py_tool/commands/conf.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 07:32:57.327487 ul-py-tool-2.0.0/ul_py_tool/conf/
--rw-rw-rw-   0 root         (0) root         (0)      458 2022-02-08 11:33:41.000000 ul-py-tool-2.0.0/ul_py_tool/conf/editorconfig
--rw-rw-rw-   0 root         (0) root         (0)      284 2022-02-08 11:33:41.000000 ul-py-tool-2.0.0/ul_py_tool/conf/git.hook.pre-commit.sh
--rw-rw-rw-   0 root         (0) root         (0)      298 2022-02-08 11:33:41.000000 ul-py-tool-2.0.0/ul_py_tool/conf/git.hook.pre-push.sh
--rw-rw-rw-   0 root         (0) root         (0)       37 2022-02-08 11:33:41.000000 ul-py-tool-2.0.0/ul_py_tool/conf/gitattributes
--rw-rw-rw-   0 root         (0) root         (0)     1788 2022-02-08 11:33:41.000000 ul-py-tool-2.0.0/ul_py_tool/conf/gitignore
--rw-rw-rw-   0 root         (0) root         (0)       24 2022-08-04 17:20:57.000000 ul-py-tool-2.0.0/ul_py_tool/conf/isort.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1036 2022-08-05 12:16:56.000000 ul-py-tool-2.0.0/ul_py_tool/conf/mypy.ini
--rw-rw-rw-   0 root         (0) root         (0)      384 2022-07-26 16:44:23.000000 ul-py-tool-2.0.0/ul_py_tool/conf/pytest.ini
--rw-rw-rw-   0 root         (0) root         (0)        7 2022-08-04 17:20:57.000000 ul-py-tool-2.0.0/ul_py_tool/conf/python-version
--rw-rw-rw-   0 root         (0) root         (0)      532 2022-08-05 16:32:51.000000 ul-py-tool-2.0.0/ul_py_tool/conf/yamlint.yml
--rw-rw-rw-   0 root         (0) root         (0)     1597 2024-02-13 13:05:21.000000 ul-py-tool-2.0.0/ul_py_tool/main.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-04 07:32:56.000000 ul-py-tool-2.0.0/ul_py_tool/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 07:32:57.355488 ul-py-tool-2.0.0/ul_py_tool/utils/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-04 07:32:56.000000 ul-py-tool-2.0.0/ul_py_tool/utils/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 07:32:57.355488 ul-py-tool-2.0.0/ul_py_tool/utils/__tests__/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-04 07:32:56.000000 ul-py-tool-2.0.0/ul_py_tool/utils/__tests__/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      607 2023-04-27 10:19:15.000000 ul-py-tool-2.0.0/ul_py_tool/utils/__tests__/pipfile.py
--rw-rw-rw-   0 root         (0) root         (0)      310 2022-07-25 04:24:22.000000 ul-py-tool-2.0.0/ul_py_tool/utils/arg_file_exists.py
--rw-rw-rw-   0 root         (0) root         (0)     2877 2023-04-27 10:19:15.000000 ul-py-tool-2.0.0/ul_py_tool/utils/arg_files_glob.py
--rw-rw-rw-   0 root         (0) root         (0)      374 2022-08-04 17:20:57.000000 ul-py-tool-2.0.0/ul_py_tool/utils/arg_str2bool.py
--rw-rw-rw-   0 root         (0) root         (0)      837 2023-04-27 10:19:15.000000 ul-py-tool-2.0.0/ul_py_tool/utils/arg_str2list.py
--rw-rw-rw-   0 root         (0) root         (0)      603 2022-08-04 17:20:57.000000 ul-py-tool-2.0.0/ul_py_tool/utils/arg_str2yaml.py
--rw-rw-rw-   0 root         (0) root         (0)      523 2023-09-06 07:50:08.000000 ul-py-tool-2.0.0/ul_py_tool/utils/aseembly.py
--rw-rw-rw-   0 root         (0) root         (0)      179 2022-07-25 04:24:22.000000 ul-py-tool-2.0.0/ul_py_tool/utils/colors.py
--rw-rw-rw-   0 root         (0) root         (0)     4670 2023-09-06 07:50:08.000000 ul-py-tool-2.0.0/ul_py_tool/utils/docker_compose.py
--rw-rw-rw-   0 root         (0) root         (0)     1852 2023-04-27 10:19:15.000000 ul-py-tool-2.0.0/ul_py_tool/utils/docker_file.py
--rw-rw-rw-   0 root         (0) root         (0)      467 2022-02-08 11:33:41.000000 ul-py-tool-2.0.0/ul_py_tool/utils/fs.py
--rw-rw-rw-   0 root         (0) root         (0)      324 2022-08-04 17:20:57.000000 ul-py-tool-2.0.0/ul_py_tool/utils/input_lines.py
--rw-rw-rw-   0 root         (0) root         (0)     9717 2023-04-27 10:19:15.000000 ul-py-tool-2.0.0/ul_py_tool/utils/pipfile.py
--rw-rw-rw-   0 root         (0) root         (0)     3671 2022-08-04 17:20:57.000000 ul-py-tool-2.0.0/ul_py_tool/utils/run_command.py
--rw-rw-rw-   0 root         (0) root         (0)     5622 2022-08-06 16:21:13.000000 ul-py-tool-2.0.0/ul_py_tool/utils/semver.py
--rw-rw-rw-   0 root         (0) root         (0)     5927 2023-04-27 10:19:15.000000 ul-py-tool-2.0.0/ul_py_tool/utils/step.py
--rw-rw-rw-   0 root         (0) root         (0)      113 2022-02-08 11:33:41.000000 ul-py-tool-2.0.0/ul_py_tool/utils/write_stdout.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 07:32:57.299486 ul-py-tool-2.0.0/ul_py_tool.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3120 2024-04-04 07:32:57.000000 ul-py-tool-2.0.0/ul_py_tool.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1880 2024-04-04 07:32:57.000000 ul-py-tool-2.0.0/ul_py_tool.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-04 07:32:57.000000 ul-py-tool-2.0.0/ul_py_tool.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       50 2024-04-04 07:32:57.000000 ul-py-tool-2.0.0/ul_py_tool.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      531 2024-04-04 07:32:57.000000 ul-py-tool-2.0.0/ul_py_tool.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2024-04-04 07:32:57.000000 ul-py-tool-2.0.0/ul_py_tool.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 08:45:40.620926 ul-py-tool-2.1.0/
+-rw-r--r--   0 root         (0) root         (0)     3120 2024-04-12 08:45:40.620926 ul-py-tool-2.1.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2468 2023-04-27 11:37:13.000000 ul-py-tool-2.1.0/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-12 08:45:40.620926 ul-py-tool-2.1.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     2203 2024-04-12 08:45:37.000000 ul-py-tool-2.1.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 08:45:40.484921 ul-py-tool-2.1.0/ul_py_tool/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-12 08:45:37.000000 ul-py-tool-2.1.0/ul_py_tool/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 08:45:40.484921 ul-py-tool-2.1.0/ul_py_tool/__tests__/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-12 08:45:37.000000 ul-py-tool-2.1.0/ul_py_tool/__tests__/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       54 2022-08-06 11:46:30.000000 ul-py-tool-2.1.0/ul_py_tool/__tests__/conftest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 08:45:40.528923 ul-py-tool-2.1.0/ul_py_tool/commands/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-12 08:45:37.000000 ul-py-tool-2.1.0/ul_py_tool/commands/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2515 2022-11-05 23:11:45.000000 ul-py-tool-2.1.0/ul_py_tool/commands/cmd.py
+-rw-rw-rw-   0 root         (0) root         (0)     5321 2023-06-14 09:15:20.000000 ul-py-tool-2.1.0/ul_py_tool/commands/cmd_build_images.py
+-rw-rw-rw-   0 root         (0) root         (0)      826 2023-04-27 11:37:13.000000 ul-py-tool-2.1.0/ul_py_tool/commands/cmd_cleanup.py
+-rw-rw-rw-   0 root         (0) root         (0)      267 2023-04-27 11:37:13.000000 ul-py-tool-2.1.0/ul_py_tool/commands/cmd_fix_own.py
+-rw-rw-rw-   0 root         (0) root         (0)     2463 2022-10-10 12:04:09.000000 ul-py-tool-2.1.0/ul_py_tool/commands/cmd_fmt.py
+-rw-rw-rw-   0 root         (0) root         (0)     2856 2022-08-09 14:16:36.000000 ul-py-tool-2.1.0/ul_py_tool/commands/cmd_install.py
+-rw-rw-rw-   0 root         (0) root         (0)    32763 2024-04-12 08:45:37.000000 ul-py-tool-2.1.0/ul_py_tool/commands/cmd_lint.py
+-rw-rw-rw-   0 root         (0) root         (0)    11939 2023-09-11 07:39:21.000000 ul-py-tool-2.1.0/ul_py_tool/commands/cmd_release.py
+-rw-rw-rw-   0 root         (0) root         (0)     7296 2024-04-12 08:45:37.000000 ul-py-tool-2.1.0/ul_py_tool/commands/cmd_release_dcf.py
+-rw-rw-rw-   0 root         (0) root         (0)     1133 2024-04-12 08:45:37.000000 ul-py-tool-2.1.0/ul_py_tool/commands/cmd_release_dcf_dev.py
+-rw-rw-rw-   0 root         (0) root         (0)     5342 2024-04-12 08:45:37.000000 ul-py-tool-2.1.0/ul_py_tool/commands/cmd_service_version.py
+-rw-rw-rw-   0 root         (0) root         (0)     3098 2022-08-06 11:46:30.000000 ul-py-tool-2.1.0/ul_py_tool/commands/cmd_stats.py
+-rw-rw-rw-   0 root         (0) root         (0)     3597 2022-11-05 23:04:32.000000 ul-py-tool-2.1.0/ul_py_tool/commands/cmd_test.py
+-rw-rw-rw-   0 root         (0) root         (0)     5475 2023-04-27 11:37:13.000000 ul-py-tool-2.1.0/ul_py_tool/commands/cmd_test_secrets.py
+-rw-rw-rw-   0 root         (0) root         (0)     6001 2022-11-05 23:04:32.000000 ul-py-tool-2.1.0/ul_py_tool/commands/cmd_version.py
+-rw-rw-rw-   0 root         (0) root         (0)     2025 2022-10-10 12:04:09.000000 ul-py-tool-2.1.0/ul_py_tool/commands/cmp_outdated.py
+-rw-rw-rw-   0 root         (0) root         (0)     1194 2024-04-12 08:45:37.000000 ul-py-tool-2.1.0/ul_py_tool/commands/conf.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 08:45:40.560924 ul-py-tool-2.1.0/ul_py_tool/conf/
+-rw-rw-rw-   0 root         (0) root         (0)      458 2022-01-28 10:47:35.000000 ul-py-tool-2.1.0/ul_py_tool/conf/editorconfig
+-rw-rw-rw-   0 root         (0) root         (0)      284 2022-01-28 10:47:35.000000 ul-py-tool-2.1.0/ul_py_tool/conf/git.hook.pre-commit.sh
+-rw-rw-rw-   0 root         (0) root         (0)      298 2022-01-28 10:47:35.000000 ul-py-tool-2.1.0/ul_py_tool/conf/git.hook.pre-push.sh
+-rw-rw-rw-   0 root         (0) root         (0)       37 2022-01-28 10:47:35.000000 ul-py-tool-2.1.0/ul_py_tool/conf/gitattributes
+-rw-rw-rw-   0 root         (0) root         (0)     1788 2022-01-28 10:47:35.000000 ul-py-tool-2.1.0/ul_py_tool/conf/gitignore
+-rw-rw-rw-   0 root         (0) root         (0)       24 2022-08-02 21:07:57.000000 ul-py-tool-2.1.0/ul_py_tool/conf/isort.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1036 2022-08-05 13:02:41.000000 ul-py-tool-2.1.0/ul_py_tool/conf/mypy.ini
+-rw-rw-rw-   0 root         (0) root         (0)      384 2022-07-27 08:23:16.000000 ul-py-tool-2.1.0/ul_py_tool/conf/pytest.ini
+-rw-rw-rw-   0 root         (0) root         (0)        7 2022-08-04 17:28:35.000000 ul-py-tool-2.1.0/ul_py_tool/conf/python-version
+-rw-rw-rw-   0 root         (0) root         (0)      532 2022-08-06 11:46:30.000000 ul-py-tool-2.1.0/ul_py_tool/conf/yamlint.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1597 2024-04-12 08:45:37.000000 ul-py-tool-2.1.0/ul_py_tool/main.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-12 08:45:37.000000 ul-py-tool-2.1.0/ul_py_tool/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 08:45:40.612926 ul-py-tool-2.1.0/ul_py_tool/utils/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-12 08:45:37.000000 ul-py-tool-2.1.0/ul_py_tool/utils/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 08:45:40.616926 ul-py-tool-2.1.0/ul_py_tool/utils/__tests__/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-12 08:45:37.000000 ul-py-tool-2.1.0/ul_py_tool/utils/__tests__/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      607 2023-04-27 11:37:13.000000 ul-py-tool-2.1.0/ul_py_tool/utils/__tests__/pipfile.py
+-rw-rw-rw-   0 root         (0) root         (0)      310 2022-07-22 16:25:14.000000 ul-py-tool-2.1.0/ul_py_tool/utils/arg_file_exists.py
+-rw-rw-rw-   0 root         (0) root         (0)     2877 2022-10-10 12:04:09.000000 ul-py-tool-2.1.0/ul_py_tool/utils/arg_files_glob.py
+-rw-rw-rw-   0 root         (0) root         (0)      374 2022-08-02 21:07:57.000000 ul-py-tool-2.1.0/ul_py_tool/utils/arg_str2bool.py
+-rw-rw-rw-   0 root         (0) root         (0)      837 2022-10-10 12:04:09.000000 ul-py-tool-2.1.0/ul_py_tool/utils/arg_str2list.py
+-rw-rw-rw-   0 root         (0) root         (0)      603 2022-08-02 21:07:57.000000 ul-py-tool-2.1.0/ul_py_tool/utils/arg_str2yaml.py
+-rw-rw-rw-   0 root         (0) root         (0)      523 2023-09-11 07:39:21.000000 ul-py-tool-2.1.0/ul_py_tool/utils/aseembly.py
+-rw-rw-rw-   0 root         (0) root         (0)      179 2022-08-04 17:28:35.000000 ul-py-tool-2.1.0/ul_py_tool/utils/colors.py
+-rw-rw-rw-   0 root         (0) root         (0)     4670 2023-09-11 07:39:21.000000 ul-py-tool-2.1.0/ul_py_tool/utils/docker_compose.py
+-rw-rw-rw-   0 root         (0) root         (0)     1852 2022-10-10 12:04:09.000000 ul-py-tool-2.1.0/ul_py_tool/utils/docker_file.py
+-rw-rw-rw-   0 root         (0) root         (0)      467 2022-01-28 10:47:35.000000 ul-py-tool-2.1.0/ul_py_tool/utils/fs.py
+-rw-rw-rw-   0 root         (0) root         (0)      324 2022-08-04 11:32:36.000000 ul-py-tool-2.1.0/ul_py_tool/utils/input_lines.py
+-rw-rw-rw-   0 root         (0) root         (0)     9735 2024-04-12 08:45:37.000000 ul-py-tool-2.1.0/ul_py_tool/utils/pipfile.py
+-rw-rw-rw-   0 root         (0) root         (0)     3671 2022-08-02 21:07:57.000000 ul-py-tool-2.1.0/ul_py_tool/utils/run_command.py
+-rw-rw-rw-   0 root         (0) root         (0)     5622 2022-08-06 11:46:30.000000 ul-py-tool-2.1.0/ul_py_tool/utils/semver.py
+-rw-rw-rw-   0 root         (0) root         (0)     5927 2023-04-27 11:37:13.000000 ul-py-tool-2.1.0/ul_py_tool/utils/step.py
+-rw-rw-rw-   0 root         (0) root         (0)      113 2022-01-28 10:47:35.000000 ul-py-tool-2.1.0/ul_py_tool/utils/write_stdout.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 08:45:40.484921 ul-py-tool-2.1.0/ul_py_tool.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3120 2024-04-12 08:45:40.000000 ul-py-tool-2.1.0/ul_py_tool.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1880 2024-04-12 08:45:40.000000 ul-py-tool-2.1.0/ul_py_tool.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-12 08:45:40.000000 ul-py-tool-2.1.0/ul_py_tool.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       50 2024-04-12 08:45:40.000000 ul-py-tool-2.1.0/ul_py_tool.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      558 2024-04-12 08:45:40.000000 ul-py-tool-2.1.0/ul_py_tool.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2024-04-12 08:45:40.000000 ul-py-tool-2.1.0/ul_py_tool.egg-info/top_level.txt
```

### Comparing `ul-py-tool-2.0.0/PKG-INFO` & `ul-py-tool-2.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ul-py-tool
-Version: 2.0.0
+Version: 2.1.0
 Summary: Python ul py tool
 Home-page: https://gitlab.neroelectronics.by/unic-lab/libraries/common-python-utils/ul-py-tool.git
 Author: Unic-lab
 Author-email: 
 Platform: any
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ul-py-tool-2.0.0/README.md` & `ul-py-tool-2.1.0/README.md`

 * *Files identical despite different names*

### Comparing `ul-py-tool-2.0.0/setup.py` & `ul-py-tool-2.1.0/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 with open(path.join(HERE, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 
 setup(
     name='ul-py-tool',
-    version='2.0.0',
+    version='2.1.0',
     description='Python ul py tool',
     author='Unic-lab',
     author_email='',
     url='https://gitlab.neroelectronics.by/unic-lab/libraries/common-python-utils/ul-py-tool.git',
     packages=find_packages(include=['ul_py_tool*']),
     platforms='any',
     package_data={
@@ -39,41 +39,43 @@
     entry_points={
         "console_scripts": [
             'ulpytool=ul_py_tool.main:main',
         ],
     },
     include_package_data=True,
     install_requires=[
-        "numpy==1.23.3",
-        "pandas==2.2.1",
-        "pydantic[mypy]==2.6.4",
+        "numpy==1.26.4",
+        "pandas==2.2.2",
+        "pydantic==2.7.0",
         "PyYAML==6.0",
         "colored==2.2.4",
-        "rich==12.6.0",
+        "rich==13.7.1",
         "tomli==2.0.1",
         "requests==2.31.0",
-        "deepdiff==6.7.1",
+        "deepdiff==7.0.1",
 
         "mypy==1.9.0",
         "types-pytz==2024.1.0.20240203",
         "types-pyyaml==6.0.11",
         "types-requests==2.31.0.4",
         "types-setuptools==69.2.0.20240317",
         "types-python-dateutil==2.9.0.20240316",
-        "typing-extensions==4.3.0",
         "data-science-types==0.2.23",
+        "typing-extensions==4.11.0",
 
+        "ruff==0.3.7",
         "black==24.3.0",
-        "ruff==0.3.4",
         "isort[colors]==5.10.1",
         "yamllint==1.35.1",
+        "pre-commit==3.7.0",
 
         "pytest==8.1.1",
         "pytest-cov==5.0.0",
+        "faker==24.8.0",
         "python-gitlab==4.4.0",
         "kubernetes==29.0.0",
 
-        "wheel==0.37.1",
+        "wheel==0.43.0",
         "twine==5.0.0",
-        "setuptools==63.4.2",
+        "setuptools==69.2.0",
     ],
 )
```

### Comparing `ul-py-tool-2.0.0/ul_py_tool/commands/cmd.py` & `ul-py-tool-2.1.0/ul_py_tool/commands/cmd.py`

 * *Files identical despite different names*

### Comparing `ul-py-tool-2.0.0/ul_py_tool/commands/cmd_build_images.py` & `ul-py-tool-2.1.0/ul_py_tool/commands/cmd_build_images.py`

 * *Files identical despite different names*

### Comparing `ul-py-tool-2.0.0/ul_py_tool/commands/cmd_cleanup.py` & `ul-py-tool-2.1.0/ul_py_tool/commands/cmd_cleanup.py`

 * *Files identical despite different names*

### Comparing `ul-py-tool-2.0.0/ul_py_tool/commands/cmd_fmt.py` & `ul-py-tool-2.1.0/ul_py_tool/commands/cmd_fmt.py`

 * *Files identical despite different names*

### Comparing `ul-py-tool-2.0.0/ul_py_tool/commands/cmd_install.py` & `ul-py-tool-2.1.0/ul_py_tool/commands/cmd_install.py`

 * *Files identical despite different names*

### Comparing `ul-py-tool-2.0.0/ul_py_tool/commands/cmd_lint.py` & `ul-py-tool-2.1.0/ul_py_tool/commands/cmd_lint.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,26 +41,24 @@
     check_imports: bool
     exclude_libs: List[str]
     packages_ignored: List[str]
     py_init_dir_ignore_lists: List[List[str]]
     packages_ignored_in_setup: List[str]
     check_hooks: bool
     check_setup_packages: bool
-    check_nero_packages_is_fresh: bool
     check_packages: bool
 
     @staticmethod
     def add_parser_args(parser: argparse.ArgumentParser) -> None:
         parser.add_argument('--fix', dest='fix', type=arg_str2bool, default=False)
         parser.add_argument('--check-env', dest='check_environment', type=arg_str2bool, default=False)
         parser.add_argument('--check-hooks', dest='check_hooks', type=arg_str2bool, required=False, default=not UNDER_CI_JOB)
         parser.add_argument('--check-imports', dest='check_imports', type=arg_str2bool, default=True, required=False)
         parser.add_argument('--check-packages', dest='check_packages', type=arg_str2bool, default=not UNDER_CI_JOB, required=False)
         parser.add_argument('--check-setup-packages', dest='check_setup_packages', type=arg_str2bool, default=not UNDER_CI_JOB, required=False)
-        parser.add_argument('--check-nero-packages-is-fresh', dest='check_nero_packages_is_fresh', type=arg_str2bool, default=not UNDER_CI_JOB, required=False)
         parser.add_argument('--ignore-setup-packages', dest='packages_ignored_in_setup', type=str, default=[], nargs='+', required=False)
         parser.add_argument('--ignore-packages', dest='packages_ignored', type=str, default=[], nargs='+', required=False)
 
         parser.add_argument('--exclude-import', dest='exclude_libs', type=str, default=[], nargs='+', required=False)
 
         parser.add_argument('--print-files', dest='print_files', type=int, required=False, default=10)
 
@@ -654,35 +652,22 @@
 
         with stepper.step('LINTING RUFF') as stp:
             if not len(py_files):
                 stp.skip()
             else:
                 stp.run_cmd([
                     'ruff',
+                    'check',
                     *(('--fix', ) if self.fix else tuple()),
                     '--cache-dir',
                     os.path.join(os.getcwd(), ".tmp", "ruff_cache"),
                     f'--line-length={MAX_LINE_LEN}',
                     *py_files,
                 ], ignore_error=True)
 
-        with stepper.step('LINTING FLAKE8') as stp:
-            if not len(py_files):
-                stp.skip()
-            else:
-                stp.run_cmd([
-                    'flake8',
-                    '--indent-size=4',
-                    '--count',
-                    '--statistics',
-                    f'--max-line-length={MAX_LINE_LEN}',
-                    '--ignore=D100,D101,D102,D103,D104,D107,D105,D106,D200,D400,D413,E501,SF01,T484,W503,E402,N815,N805,NQA102',
-                    *py_files,
-                ])
-
         with stepper.step('LINT IMPORTS') as stp:
             if not len(py_files):
                 stp.skip()
             else:
                 if not self.check_imports:
                     stp.skip()
                 elif not self._check_imports(py_files):
```

### Comparing `ul-py-tool-2.0.0/ul_py_tool/commands/cmd_release.py` & `ul-py-tool-2.1.0/ul_py_tool/commands/cmd_release.py`

 * *Files identical despite different names*

### Comparing `ul-py-tool-2.0.0/ul_py_tool/commands/cmd_release_dcf.py` & `ul-py-tool-2.1.0/ul_py_tool/commands/cmd_release_dcf.py`

 * *Files identical despite different names*

### Comparing `ul-py-tool-2.0.0/ul_py_tool/commands/cmd_release_dcf_dev.py` & `ul-py-tool-2.1.0/ul_py_tool/commands/cmd_release_dcf_dev.py`

 * *Files identical despite different names*

### Comparing `ul-py-tool-2.0.0/ul_py_tool/commands/cmd_service_version.py` & `ul-py-tool-2.1.0/ul_py_tool/commands/cmd_service_version.py`

 * *Files identical despite different names*

### Comparing `ul-py-tool-2.0.0/ul_py_tool/commands/cmd_stats.py` & `ul-py-tool-2.1.0/ul_py_tool/commands/cmd_stats.py`

 * *Files identical despite different names*

### Comparing `ul-py-tool-2.0.0/ul_py_tool/commands/cmd_test.py` & `ul-py-tool-2.1.0/ul_py_tool/commands/cmd_test.py`

 * *Files identical despite different names*

### Comparing `ul-py-tool-2.0.0/ul_py_tool/commands/cmd_test_secrets.py` & `ul-py-tool-2.1.0/ul_py_tool/commands/cmd_test_secrets.py`

 * *Files identical despite different names*

### Comparing `ul-py-tool-2.0.0/ul_py_tool/commands/cmd_version.py` & `ul-py-tool-2.1.0/ul_py_tool/commands/cmd_version.py`

 * *Files identical despite different names*

### Comparing `ul-py-tool-2.0.0/ul_py_tool/commands/cmp_outdated.py` & `ul-py-tool-2.1.0/ul_py_tool/commands/cmp_outdated.py`

 * *Files identical despite different names*

### Comparing `ul-py-tool-2.0.0/ul_py_tool/commands/conf.py` & `ul-py-tool-2.1.0/ul_py_tool/commands/conf.py`

 * *Files identical despite different names*

### Comparing `ul-py-tool-2.0.0/ul_py_tool/conf/gitignore` & `ul-py-tool-2.1.0/ul_py_tool/conf/gitignore`

 * *Files identical despite different names*

### Comparing `ul-py-tool-2.0.0/ul_py_tool/conf/mypy.ini` & `ul-py-tool-2.1.0/ul_py_tool/conf/mypy.ini`

 * *Files identical despite different names*

### Comparing `ul-py-tool-2.0.0/ul_py_tool/conf/yamlint.yml` & `ul-py-tool-2.1.0/ul_py_tool/conf/yamlint.yml`

 * *Files identical despite different names*

### Comparing `ul-py-tool-2.0.0/ul_py_tool/main.py` & `ul-py-tool-2.1.0/ul_py_tool/main.py`

 * *Files identical despite different names*

### Comparing `ul-py-tool-2.0.0/ul_py_tool/utils/__tests__/pipfile.py` & `ul-py-tool-2.1.0/ul_py_tool/utils/__tests__/pipfile.py`

 * *Files identical despite different names*

### Comparing `ul-py-tool-2.0.0/ul_py_tool/utils/arg_files_glob.py` & `ul-py-tool-2.1.0/ul_py_tool/utils/arg_files_glob.py`

 * *Files identical despite different names*

### Comparing `ul-py-tool-2.0.0/ul_py_tool/utils/arg_str2list.py` & `ul-py-tool-2.1.0/ul_py_tool/utils/arg_str2list.py`

 * *Files identical despite different names*

### Comparing `ul-py-tool-2.0.0/ul_py_tool/utils/arg_str2yaml.py` & `ul-py-tool-2.1.0/ul_py_tool/utils/arg_str2yaml.py`

 * *Files identical despite different names*

### Comparing `ul-py-tool-2.0.0/ul_py_tool/utils/aseembly.py` & `ul-py-tool-2.1.0/ul_py_tool/utils/aseembly.py`

 * *Files identical despite different names*

### Comparing `ul-py-tool-2.0.0/ul_py_tool/utils/docker_compose.py` & `ul-py-tool-2.1.0/ul_py_tool/utils/docker_compose.py`

 * *Files identical despite different names*

### Comparing `ul-py-tool-2.0.0/ul_py_tool/utils/docker_file.py` & `ul-py-tool-2.1.0/ul_py_tool/utils/docker_file.py`

 * *Files identical despite different names*

### Comparing `ul-py-tool-2.0.0/ul_py_tool/utils/pipfile.py` & `ul-py-tool-2.1.0/ul_py_tool/utils/pipfile.py`

 * *Files 0% similar despite different names*

```diff
@@ -108,15 +108,15 @@
         for ps in freeze_result.split('\n'):
             psl = ps.strip().split('==')
             if len(psl) == 2:
                 name, version = psl
 
                 ver = SemVer.from_string_wop(version)
 
-                name = name.strip().lower()
+                name = name.strip().lower().replace('_', '-')
 
                 res[name] = PipfilePackage(
                     name=name,
                     version=version,
                     version_operator='' if ver is None else ver[0] or '',
                     extras=[],
                     semver=None if ver is None else ver[1],
```

### Comparing `ul-py-tool-2.0.0/ul_py_tool/utils/run_command.py` & `ul-py-tool-2.1.0/ul_py_tool/utils/run_command.py`

 * *Files identical despite different names*

### Comparing `ul-py-tool-2.0.0/ul_py_tool/utils/semver.py` & `ul-py-tool-2.1.0/ul_py_tool/utils/semver.py`

 * *Files identical despite different names*

### Comparing `ul-py-tool-2.0.0/ul_py_tool/utils/step.py` & `ul-py-tool-2.1.0/ul_py_tool/utils/step.py`

 * *Files identical despite different names*

### Comparing `ul-py-tool-2.0.0/ul_py_tool.egg-info/PKG-INFO` & `ul-py-tool-2.1.0/ul_py_tool.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ul-py-tool
-Version: 2.0.0
+Version: 2.1.0
 Summary: Python ul py tool
 Home-page: https://gitlab.neroelectronics.by/unic-lab/libraries/common-python-utils/ul-py-tool.git
 Author: Unic-lab
 Author-email: 
 Platform: any
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ul-py-tool-2.0.0/ul_py_tool.egg-info/SOURCES.txt` & `ul-py-tool-2.1.0/ul_py_tool.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ul-py-tool-2.0.0/ul_py_tool.egg-info/requires.txt` & `ul-py-tool-2.1.0/ul_py_tool.egg-info/requires.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,28 +1,30 @@
-numpy==1.23.3
-pandas==2.2.1
-pydantic[mypy]==2.6.4
+numpy==1.26.4
+pandas==2.2.2
+pydantic==2.7.0
 PyYAML==6.0
 colored==2.2.4
-rich==12.6.0
+rich==13.7.1
 tomli==2.0.1
 requests==2.31.0
-deepdiff==6.7.1
+deepdiff==7.0.1
 mypy==1.9.0
 types-pytz==2024.1.0.20240203
 types-pyyaml==6.0.11
 types-requests==2.31.0.4
 types-setuptools==69.2.0.20240317
 types-python-dateutil==2.9.0.20240316
-typing-extensions==4.3.0
 data-science-types==0.2.23
+typing-extensions==4.11.0
+ruff==0.3.7
 black==24.3.0
-ruff==0.3.4
 isort[colors]==5.10.1
 yamllint==1.35.1
+pre-commit==3.7.0
 pytest==8.1.1
 pytest-cov==5.0.0
+faker==24.8.0
 python-gitlab==4.4.0
 kubernetes==29.0.0
-wheel==0.37.1
+wheel==0.43.0
 twine==5.0.0
-setuptools==63.4.2
+setuptools==69.2.0
```

