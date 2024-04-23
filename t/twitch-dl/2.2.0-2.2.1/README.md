# Comparing `tmp/twitch-dl-2.2.0.tar.gz` & `tmp/twitch_dl-2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "twitch-dl-2.2.0.tar", last modified: Wed Apr 10 06:32:59 2024, max compression
+gzip compressed data, was "twitch_dl-2.2.1.tar", last modified: Tue Apr 23 15:26:10 2024, max compression
```

## Comparing `twitch-dl-2.2.0.tar` & `twitch_dl-2.2.1.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxr-xr-x   0 ihabunek  (1000) ihabunek  (1000)        0 2024-04-10 06:32:59.236628 twitch-dl-2.2.0/
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)       41 2022-08-04 08:32:39.000000 twitch-dl-2.2.0/.flake8
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      166 2022-08-27 09:42:13.000000 twitch-dl-2.2.0/.gitignore
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)       65 2024-03-29 07:50:11.000000 twitch-dl-2.2.0/.vermin
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     9663 2024-04-10 06:31:46.000000 twitch-dl-2.2.0/CHANGELOG.md
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)    35147 2022-08-04 08:32:39.000000 twitch-dl-2.2.0/LICENSE
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      951 2024-03-25 07:34:51.000000 twitch-dl-2.2.0/Makefile
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)    43171 2024-04-10 06:32:59.235628 twitch-dl-2.2.0/PKG-INFO
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     1627 2024-03-29 07:50:11.000000 twitch-dl-2.2.0/README.md
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      343 2022-11-13 13:02:23.000000 twitch-dl-2.2.0/TODO.md
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      481 2022-08-27 09:42:13.000000 twitch-dl-2.2.0/book.css
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      223 2022-08-27 09:42:13.000000 twitch-dl-2.2.0/book.toml
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     8103 2024-04-10 06:31:31.000000 twitch-dl-2.2.0/changelog.yaml
-drwxr-xr-x   0 ihabunek  (1000) ihabunek  (1000)        0 2024-04-10 06:32:59.229628 twitch-dl-2.2.0/docs/
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      484 2024-03-29 07:50:11.000000 twitch-dl-2.2.0/docs/SUMMARY.md
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      282 2022-08-27 09:42:13.000000 twitch-dl-2.2.0/docs/advanced.md
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     9663 2024-04-10 06:31:46.000000 twitch-dl-2.2.0/docs/changelog.md
-drwxr-xr-x   0 ihabunek  (1000) ihabunek  (1000)        0 2024-04-10 06:32:59.230628 twitch-dl-2.2.0/docs/commands/
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)    69599 2022-08-27 09:42:13.000000 twitch-dl-2.2.0/docs/commands/auth_token.png
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     2499 2024-04-10 06:31:46.000000 twitch-dl-2.2.0/docs/commands/clips.md
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     6159 2024-04-10 06:31:46.000000 twitch-dl-2.2.0/docs/commands/download.md
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      722 2024-04-10 06:31:46.000000 twitch-dl-2.2.0/docs/commands/env.md
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      670 2024-04-10 06:31:46.000000 twitch-dl-2.2.0/docs/commands/info.md
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     2030 2024-04-10 06:31:46.000000 twitch-dl-2.2.0/docs/commands/videos.md
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      420 2024-03-29 07:50:11.000000 twitch-dl-2.2.0/docs/environment_variables.md
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     1653 2024-03-29 07:50:11.000000 twitch-dl-2.2.0/docs/installation.md
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     1169 2022-08-27 09:42:13.000000 twitch-dl-2.2.0/docs/introduction.md
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)    34916 2022-08-27 09:42:13.000000 twitch-dl-2.2.0/docs/license.md
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      664 2024-03-29 07:50:11.000000 twitch-dl-2.2.0/docs/shell_completion.md
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      690 2022-08-27 09:42:13.000000 twitch-dl-2.2.0/docs/usage.md
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     1269 2024-04-04 06:27:17.000000 twitch-dl-2.2.0/pyproject.toml
-drwxr-xr-x   0 ihabunek  (1000) ihabunek  (1000)        0 2024-04-10 06:32:59.231628 twitch-dl-2.2.0/scripts/
--rwxr-xr-x   0 ihabunek  (1000) ihabunek  (1000)     1026 2022-11-13 13:02:23.000000 twitch-dl-2.2.0/scripts/generate_changelog
--rwxr-xr-x   0 ihabunek  (1000) ihabunek  (1000)     3686 2024-03-29 07:50:11.000000 twitch-dl-2.2.0/scripts/generate_docs
--rwxr-xr-x   0 ihabunek  (1000) ihabunek  (1000)     1587 2024-04-10 06:26:52.000000 twitch-dl-2.2.0/scripts/tag_version
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)       38 2024-04-10 06:32:59.236628 twitch-dl-2.2.0/setup.cfg
-drwxr-xr-x   0 ihabunek  (1000) ihabunek  (1000)        0 2024-04-10 06:32:59.231628 twitch-dl-2.2.0/tests/
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     1578 2024-04-10 06:03:56.000000 twitch-dl-2.2.0/tests/test_api.py
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     2020 2022-08-04 08:32:39.000000 twitch-dl-2.2.0/tests/test_patterns.py
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     2605 2022-11-13 13:02:23.000000 twitch-dl-2.2.0/tests/test_progress.py
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      456 2022-08-04 08:32:39.000000 twitch-dl-2.2.0/tests/test_utils.py
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     1350 2022-08-04 08:32:39.000000 twitch-dl-2.2.0/twitch-dl.1.scd
-drwxr-xr-x   0 ihabunek  (1000) ihabunek  (1000)        0 2024-04-10 06:32:59.235628 twitch-dl-2.2.0/twitch_dl.egg-info/
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)    43171 2024-04-10 06:32:59.000000 twitch-dl-2.2.0/twitch_dl.egg-info/PKG-INFO
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     1195 2024-04-10 06:32:59.000000 twitch-dl-2.2.0/twitch_dl.egg-info/SOURCES.txt
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)        1 2024-04-10 06:32:59.000000 twitch-dl-2.2.0/twitch_dl.egg-info/dependency_links.txt
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)       47 2024-04-10 06:32:59.000000 twitch-dl-2.2.0/twitch_dl.egg-info/entry_points.txt
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      111 2024-04-10 06:32:59.000000 twitch-dl-2.2.0/twitch_dl.egg-info/requires.txt
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)        9 2024-04-10 06:32:59.000000 twitch-dl-2.2.0/twitch_dl.egg-info/top_level.txt
-drwxr-xr-x   0 ihabunek  (1000) ihabunek  (1000)        0 2024-04-10 06:32:59.234628 twitch-dl-2.2.0/twitchdl/
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      196 2024-03-29 07:50:11.000000 twitch-dl-2.2.0/twitchdl/__init__.py
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)       36 2024-03-29 07:50:11.000000 twitch-dl-2.2.0/twitchdl/__main__.py
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     9521 2024-04-10 06:24:49.000000 twitch-dl-2.2.0/twitchdl/cli.py
-drwxr-xr-x   0 ihabunek  (1000) ihabunek  (1000)        0 2024-04-10 06:32:59.235628 twitch-dl-2.2.0/twitchdl/commands/
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)        0 2024-03-29 07:50:11.000000 twitch-dl-2.2.0/twitchdl/commands/__init__.py
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     2539 2024-04-06 08:39:48.000000 twitch-dl-2.2.0/twitchdl/commands/clips.py
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)    11573 2024-04-05 06:57:32.000000 twitch-dl-2.2.0/twitchdl/commands/download.py
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     2929 2024-04-04 06:27:17.000000 twitch-dl-2.2.0/twitchdl/commands/info.py
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     2049 2024-04-04 06:27:17.000000 twitch-dl-2.2.0/twitchdl/commands/videos.py
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      931 2024-03-29 07:50:11.000000 twitch-dl-2.2.0/twitchdl/download.py
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      482 2024-04-04 08:48:56.000000 twitch-dl-2.2.0/twitchdl/entities.py
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      139 2024-04-04 06:27:17.000000 twitch-dl-2.2.0/twitchdl/exceptions.py
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     4138 2024-04-06 08:15:38.000000 twitch-dl-2.2.0/twitchdl/http.py
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     4558 2024-04-06 08:40:29.000000 twitch-dl-2.2.0/twitchdl/output.py
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     3630 2024-04-10 05:59:56.000000 twitch-dl-2.2.0/twitchdl/playlists.py
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     4627 2024-04-04 06:27:17.000000 twitch-dl-2.2.0/twitchdl/progress.py
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)    11118 2024-04-04 06:57:51.000000 twitch-dl-2.2.0/twitchdl/twitch.py
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     3037 2024-04-04 06:27:17.000000 twitch-dl-2.2.0/twitchdl/utils.py
+drwxr-xr-x   0 ihabunek  (1000) ihabunek  (1000)        0 2024-04-23 15:26:10.520835 twitch_dl-2.2.1/
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)       41 2023-08-11 10:29:42.000000 twitch_dl-2.2.1/.flake8
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      166 2023-08-11 10:29:32.000000 twitch_dl-2.2.1/.gitignore
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)       65 2024-04-23 15:07:42.000000 twitch_dl-2.2.1/.vermin
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     9873 2024-04-23 15:25:40.000000 twitch_dl-2.2.1/CHANGELOG.md
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)    35147 2023-08-11 10:29:42.000000 twitch_dl-2.2.1/LICENSE
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      951 2024-03-23 06:29:27.000000 twitch_dl-2.2.1/Makefile
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)    43171 2024-04-23 15:26:10.520835 twitch_dl-2.2.1/PKG-INFO
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     1627 2024-04-23 15:07:42.000000 twitch_dl-2.2.1/README.md
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      343 2023-08-11 10:29:32.000000 twitch_dl-2.2.1/TODO.md
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      481 2023-08-11 10:29:32.000000 twitch_dl-2.2.1/book.css
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      223 2023-08-11 10:29:32.000000 twitch_dl-2.2.1/book.toml
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     8276 2024-04-23 15:25:30.000000 twitch_dl-2.2.1/changelog.yaml
+drwxr-xr-x   0 ihabunek  (1000) ihabunek  (1000)        0 2024-04-23 15:26:10.516835 twitch_dl-2.2.1/docs/
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      484 2024-04-23 15:07:42.000000 twitch_dl-2.2.1/docs/SUMMARY.md
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      282 2023-08-11 10:29:47.000000 twitch_dl-2.2.1/docs/advanced.md
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     9873 2024-04-23 15:25:40.000000 twitch_dl-2.2.1/docs/changelog.md
+drwxr-xr-x   0 ihabunek  (1000) ihabunek  (1000)        0 2024-04-23 15:26:10.517835 twitch_dl-2.2.1/docs/commands/
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)    69599 2023-08-11 10:29:47.000000 twitch_dl-2.2.1/docs/commands/auth_token.png
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     2499 2024-04-23 15:25:40.000000 twitch_dl-2.2.1/docs/commands/clips.md
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     6159 2024-04-23 15:25:40.000000 twitch_dl-2.2.1/docs/commands/download.md
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      722 2024-04-23 15:25:40.000000 twitch_dl-2.2.1/docs/commands/env.md
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      670 2024-04-23 15:25:40.000000 twitch_dl-2.2.1/docs/commands/info.md
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     2030 2024-04-23 15:25:40.000000 twitch_dl-2.2.1/docs/commands/videos.md
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      420 2024-04-23 15:07:42.000000 twitch_dl-2.2.1/docs/environment_variables.md
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     1653 2024-04-23 15:07:42.000000 twitch_dl-2.2.1/docs/installation.md
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     1169 2023-08-11 10:29:47.000000 twitch_dl-2.2.1/docs/introduction.md
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)    34916 2023-08-11 10:29:47.000000 twitch_dl-2.2.1/docs/license.md
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      664 2024-04-23 15:07:42.000000 twitch_dl-2.2.1/docs/shell_completion.md
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      690 2023-08-11 10:29:47.000000 twitch_dl-2.2.1/docs/usage.md
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     1269 2024-04-23 15:07:42.000000 twitch_dl-2.2.1/pyproject.toml
+drwxr-xr-x   0 ihabunek  (1000) ihabunek  (1000)        0 2024-04-23 15:26:10.517835 twitch_dl-2.2.1/scripts/
+-rwxr-xr-x   0 ihabunek  (1000) ihabunek  (1000)     1026 2023-10-08 19:39:41.000000 twitch_dl-2.2.1/scripts/generate_changelog
+-rwxr-xr-x   0 ihabunek  (1000) ihabunek  (1000)     3686 2024-04-23 15:07:42.000000 twitch_dl-2.2.1/scripts/generate_docs
+-rwxr-xr-x   0 ihabunek  (1000) ihabunek  (1000)     1587 2024-04-23 15:07:42.000000 twitch_dl-2.2.1/scripts/tag_version
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)       38 2024-04-23 15:26:10.520835 twitch_dl-2.2.1/setup.cfg
+drwxr-xr-x   0 ihabunek  (1000) ihabunek  (1000)        0 2024-04-23 15:26:10.518835 twitch_dl-2.2.1/tests/
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     1578 2024-04-23 15:07:42.000000 twitch_dl-2.2.1/tests/test_api.py
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     2020 2023-08-11 10:29:32.000000 twitch_dl-2.2.1/tests/test_patterns.py
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     2605 2023-08-11 10:29:32.000000 twitch_dl-2.2.1/tests/test_progress.py
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      456 2023-08-11 10:29:32.000000 twitch_dl-2.2.1/tests/test_utils.py
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     1350 2023-08-11 10:29:42.000000 twitch_dl-2.2.1/twitch-dl.1.scd
+drwxr-xr-x   0 ihabunek  (1000) ihabunek  (1000)        0 2024-04-23 15:26:10.519835 twitch_dl-2.2.1/twitch_dl.egg-info/
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)    43171 2024-04-23 15:26:10.000000 twitch_dl-2.2.1/twitch_dl.egg-info/PKG-INFO
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     1195 2024-04-23 15:26:10.000000 twitch_dl-2.2.1/twitch_dl.egg-info/SOURCES.txt
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)        1 2024-04-23 15:26:10.000000 twitch_dl-2.2.1/twitch_dl.egg-info/dependency_links.txt
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)       47 2024-04-23 15:26:10.000000 twitch_dl-2.2.1/twitch_dl.egg-info/entry_points.txt
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      111 2024-04-23 15:26:10.000000 twitch_dl-2.2.1/twitch_dl.egg-info/requires.txt
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)        9 2024-04-23 15:26:10.000000 twitch_dl-2.2.1/twitch_dl.egg-info/top_level.txt
+drwxr-xr-x   0 ihabunek  (1000) ihabunek  (1000)        0 2024-04-23 15:26:10.519835 twitch_dl-2.2.1/twitchdl/
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      196 2024-04-23 15:07:42.000000 twitch_dl-2.2.1/twitchdl/__init__.py
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)       36 2024-04-23 15:07:42.000000 twitch_dl-2.2.1/twitchdl/__main__.py
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     9588 2024-04-23 15:10:23.000000 twitch_dl-2.2.1/twitchdl/cli.py
+drwxr-xr-x   0 ihabunek  (1000) ihabunek  (1000)        0 2024-04-23 15:26:10.519835 twitch_dl-2.2.1/twitchdl/commands/
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)        0 2024-04-23 15:07:42.000000 twitch_dl-2.2.1/twitchdl/commands/__init__.py
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     2561 2024-04-23 15:09:23.000000 twitch_dl-2.2.1/twitchdl/commands/clips.py
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)    11571 2024-04-23 15:07:42.000000 twitch_dl-2.2.1/twitchdl/commands/download.py
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     2929 2024-04-23 15:07:42.000000 twitch_dl-2.2.1/twitchdl/commands/info.py
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     2083 2024-04-23 15:09:38.000000 twitch_dl-2.2.1/twitchdl/commands/videos.py
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      931 2024-04-23 15:07:42.000000 twitch_dl-2.2.1/twitchdl/download.py
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      510 2024-04-23 15:08:18.000000 twitch_dl-2.2.1/twitchdl/entities.py
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      139 2024-04-23 15:07:42.000000 twitch_dl-2.2.1/twitchdl/exceptions.py
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     4138 2024-04-23 15:07:42.000000 twitch_dl-2.2.1/twitchdl/http.py
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     4571 2024-04-23 15:10:46.000000 twitch_dl-2.2.1/twitchdl/output.py
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     3652 2024-04-23 15:11:10.000000 twitch_dl-2.2.1/twitchdl/playlists.py
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     4722 2024-04-23 15:07:42.000000 twitch_dl-2.2.1/twitchdl/progress.py
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)    11149 2024-04-23 15:12:20.000000 twitch_dl-2.2.1/twitchdl/twitch.py
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     3099 2024-04-23 15:13:11.000000 twitch_dl-2.2.1/twitchdl/utils.py
```

### Comparing `twitch-dl-2.2.0/CHANGELOG.md` & `twitch_dl-2.2.1/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,18 @@
 twitch-dl changelog
 ===================
 
 <!-- Do not edit. This file is automatically generated from changelog.yaml.-->
 
+### [2.2.1 (2024-04-23)](https://github.com/ihabunek/twitch-dl/releases/tag/2.2.1)
+
+* Fix compat with < Python 3.10 (#152)
+* Fix division by zero in progress calculation when video duration is reported
+  as 0
+
 ### [2.2.0 (2024-04-10)](https://github.com/ihabunek/twitch-dl/releases/tag/2.2.0)
 
 * **Requires Python 3.8+**
 * Migrated to Click library for generating the commandline interface
 * Add shell auto completion, see 'Shell completion' in docs.
 * Add setting defaults via environment variables, see 'Environment variables' in
   docs
```

### Comparing `twitch-dl-2.2.0/LICENSE` & `twitch_dl-2.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `twitch-dl-2.2.0/Makefile` & `twitch_dl-2.2.1/Makefile`

 * *Files identical despite different names*

### Comparing `twitch-dl-2.2.0/PKG-INFO` & `twitch_dl-2.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twitch-dl
-Version: 2.2.0
+Version: 2.2.1
 Summary: Quickly download videos from twitch.tv from the comort of your terminal emulator
 Author-email: Ivan Habunek <ivan@habunek.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `twitch-dl-2.2.0/README.md` & `twitch_dl-2.2.1/README.md`

 * *Files identical despite different names*

### Comparing `twitch-dl-2.2.0/changelog.yaml` & `twitch_dl-2.2.1/changelog.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+2.2.1:
+  date: 2024-04-23
+  changes:
+    - "Fix compat with < Python 3.10 (#152)"
+    - "Fix division by zero in progress calculation when video duration is reported as 0"
+
 2.2.0:
   date: 2024-04-10
   changes:
     - "**Requires Python 3.8+**"
     - "Migrated to Click library for generating the commandline interface"
     - "Add shell auto completion, see 'Shell completion' in docs."
     - "Add setting defaults via environment variables, see 'Environment variables' in docs"
```

### Comparing `twitch-dl-2.2.0/docs/changelog.md` & `twitch_dl-2.2.1/docs/changelog.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,18 @@
 twitch-dl changelog
 ===================
 
 <!-- Do not edit. This file is automatically generated from changelog.yaml.-->
 
+### [2.2.1 (2024-04-23)](https://github.com/ihabunek/twitch-dl/releases/tag/2.2.1)
+
+* Fix compat with < Python 3.10 (#152)
+* Fix division by zero in progress calculation when video duration is reported
+  as 0
+
 ### [2.2.0 (2024-04-10)](https://github.com/ihabunek/twitch-dl/releases/tag/2.2.0)
 
 * **Requires Python 3.8+**
 * Migrated to Click library for generating the commandline interface
 * Add shell auto completion, see 'Shell completion' in docs.
 * Add setting defaults via environment variables, see 'Environment variables' in
   docs
```

### Comparing `twitch-dl-2.2.0/docs/commands/auth_token.png` & `twitch_dl-2.2.1/docs/commands/auth_token.png`

 * *Files identical despite different names*

### Comparing `twitch-dl-2.2.0/docs/commands/clips.md` & `twitch_dl-2.2.1/docs/commands/clips.md`

 * *Files identical despite different names*

### Comparing `twitch-dl-2.2.0/docs/commands/download.md` & `twitch_dl-2.2.1/docs/commands/download.md`

 * *Files identical despite different names*

### Comparing `twitch-dl-2.2.0/docs/commands/env.md` & `twitch_dl-2.2.1/docs/commands/env.md`

 * *Files identical despite different names*

### Comparing `twitch-dl-2.2.0/docs/commands/info.md` & `twitch_dl-2.2.1/docs/commands/info.md`

 * *Files identical despite different names*

### Comparing `twitch-dl-2.2.0/docs/commands/videos.md` & `twitch_dl-2.2.1/docs/commands/videos.md`

 * *Files identical despite different names*

### Comparing `twitch-dl-2.2.0/docs/installation.md` & `twitch_dl-2.2.1/docs/installation.md`

 * *Files identical despite different names*

### Comparing `twitch-dl-2.2.0/docs/introduction.md` & `twitch_dl-2.2.1/docs/introduction.md`

 * *Files identical despite different names*

### Comparing `twitch-dl-2.2.0/docs/license.md` & `twitch_dl-2.2.1/docs/license.md`

 * *Files identical despite different names*

### Comparing `twitch-dl-2.2.0/docs/shell_completion.md` & `twitch_dl-2.2.1/docs/shell_completion.md`

 * *Files identical despite different names*

### Comparing `twitch-dl-2.2.0/docs/usage.md` & `twitch_dl-2.2.1/docs/usage.md`

 * *Files identical despite different names*

### Comparing `twitch-dl-2.2.0/pyproject.toml` & `twitch_dl-2.2.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `twitch-dl-2.2.0/scripts/generate_changelog` & `twitch_dl-2.2.1/scripts/generate_changelog`

 * *Files identical despite different names*

### Comparing `twitch-dl-2.2.0/scripts/generate_docs` & `twitch_dl-2.2.1/scripts/generate_docs`

 * *Files identical despite different names*

### Comparing `twitch-dl-2.2.0/scripts/tag_version` & `twitch_dl-2.2.1/scripts/tag_version`

 * *Files identical despite different names*

### Comparing `twitch-dl-2.2.0/tests/test_api.py` & `twitch_dl-2.2.1/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `twitch-dl-2.2.0/tests/test_patterns.py` & `twitch_dl-2.2.1/tests/test_patterns.py`

 * *Files identical despite different names*

### Comparing `twitch-dl-2.2.0/tests/test_progress.py` & `twitch_dl-2.2.1/tests/test_progress.py`

 * *Files identical despite different names*

### Comparing `twitch-dl-2.2.0/twitch-dl.1.scd` & `twitch_dl-2.2.1/twitch-dl.1.scd`

 * *Files identical despite different names*

### Comparing `twitch-dl-2.2.0/twitch_dl.egg-info/PKG-INFO` & `twitch_dl-2.2.1/twitch_dl.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twitch-dl
-Version: 2.2.0
+Version: 2.2.1
 Summary: Quickly download videos from twitch.tv from the comort of your terminal emulator
 Author-email: Ivan Habunek <ivan@habunek.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `twitch-dl-2.2.0/twitch_dl.egg-info/SOURCES.txt` & `twitch_dl-2.2.1/twitch_dl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `twitch-dl-2.2.0/twitchdl/cli.py` & `twitch_dl-2.2.1/twitchdl/cli.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import logging
 import platform
 import re
 import sys
+from typing import Optional
 
 import click
 
 from twitchdl import __version__
 from twitchdl.entities import DownloadOptions
 from twitchdl.twitch import ClipsPeriod, VideosSort, VideosType
 
@@ -26,21 +27,21 @@
     "--json",
     is_flag=True,
     default=False,
     help="Print data as JSON rather than human readable text",
 )
 
 
-def validate_positive(_ctx: click.Context, _param: click.Parameter, value: int | None):
+def validate_positive(_ctx: click.Context, _param: click.Parameter, value: Optional[int]):
     if value is not None and value <= 0:
         raise click.BadParameter("must be greater than 0")
     return value
 
 
-def validate_time(_ctx: click.Context, _param: click.Parameter, value: str) -> int | None:
+def validate_time(_ctx: click.Context, _param: click.Parameter, value: str) -> Optional[int]:
     """Parse a time string (hh:mm or hh:mm:ss) to number of seconds."""
     if not value:
         return None
 
     parts = [int(p) for p in value.split(":")]
 
     if not 2 <= len(parts) <= 3:
@@ -52,15 +53,15 @@
 
     if hours < 0 or not (0 <= minutes <= 59) or not (0 <= seconds <= 59):
         raise click.BadParameter("invalid time")
 
     return hours * 3600 + minutes * 60 + seconds
 
 
-def validate_rate(_ctx: click.Context, _param: click.Parameter, value: str) -> int | None:
+def validate_rate(_ctx: click.Context, _param: click.Parameter, value: str) -> Optional[int]:
     if not value:
         return None
 
     match = re.search(r"^([0-9]+)(k|m|)$", value, flags=re.IGNORECASE)
 
     if not match:
         raise click.BadParameter("must be an integer, followed by an optional 'k' or 'm'")
@@ -139,16 +140,16 @@
 @json_option
 def clips(
     channel_name: str,
     all: bool,
     compact: bool,
     download: bool,
     json: bool,
-    limit: int | None,
-    pager: int | None,
+    limit: Optional[int],
+    pager: Optional[int],
     period: ClipsPeriod,
 ):
     """List or download clips for given CHANNEL_NAME."""
     from twitchdl.commands.clips import clips
 
     clips(
         channel_name,
@@ -251,27 +252,27 @@
     "--max-workers",
     help="Number of workers for downloading vods concurrently",
     type=int,
     default=5,
 )
 def download(
     ids: tuple[str, ...],
-    auth_token: str | None,
-    chapter: int | None,
+    auth_token: Optional[str],
+    chapter: Optional[int],
     concat: bool,
     dry_run: bool,
-    end: int | None,
+    end: Optional[int],
     format: str,
     keep: bool,
     no_join: bool,
     overwrite: bool,
     output: str,
-    quality: str | None,
-    rate_limit: int | None,
-    start: int | None,
+    quality: Optional[str],
+    rate_limit: Optional[int],
+    start: Optional[int],
     max_workers: int,
 ):
     """Download videos or clips.
 
     Pass one or more video ID, clip slug or Twitch URL to download.
     """
     from twitchdl.commands.download import download
@@ -371,16 +372,16 @@
 @json_option
 def videos(
     channel_name: str,
     all: bool,
     compact: bool,
     games_tuple: tuple[str, ...],
     json: bool,
-    limit: int | None,
-    pager: int | None,
+    limit: Optional[int],
+    pager: Optional[int],
     sort: VideosSort,
     type: VideosType,
 ):
     """List or download clips for given CHANNEL_NAME."""
     from twitchdl.commands.videos import videos
 
     # Click provides a tuple, make it a list instead
```

### Comparing `twitch-dl-2.2.0/twitchdl/commands/clips.py` & `twitch_dl-2.2.1/twitchdl/commands/clips.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 import re
 import sys
 from os import path
-from typing import Callable, Generator
+from typing import Callable, Generator, Optional
 
 import click
 
 from twitchdl import twitch, utils
 from twitchdl.commands.download import get_clip_authenticated_url
 from twitchdl.download import download_file
 from twitchdl.output import green, print_clip, print_clip_compact, print_json, print_paged, yellow
-from twitchdl.twitch import Clip
+from twitchdl.twitch import Clip, ClipsPeriod
 
 
 def clips(
     channel_name: str,
     *,
     all: bool = False,
     compact: bool = False,
     download: bool = False,
     json: bool = False,
-    limit: int | None = None,
-    pager: int | None = None,
-    period: twitch.ClipsPeriod = "all_time",
+    limit: Optional[int] = None,
+    pager: Optional[int] = None,
+    period: ClipsPeriod = "all_time",
 ):
     # Set different defaults for limit for compact display
     default_limit = 40 if compact else 10
 
     # Ignore --limit if --pager or --all are given
     limit = sys.maxsize if all or pager else (limit or default_limit)
```

### Comparing `twitch-dl-2.2.0/twitchdl/commands/download.py` & `twitch_dl-2.2.1/twitchdl/commands/download.py`

 * *Files 0% similar despite different names*

```diff
@@ -247,15 +247,15 @@
 
     click.echo(f"Found: {blue(video['title'])} by {yellow(video['creator']['displayName'])}")
 
     target = _video_target_filename(video, args)
     click.echo(f"Output: {blue(target)}")
 
     if not args.overwrite and path.exists(target):
-        response = click.prompt("File exists. Overwrite? [Y/n]: ", default="Y", show_default=False)
+        response = click.prompt("File exists. Overwrite? [Y/n]", default="Y", show_default=False)
         if response.lower().strip() != "y":
             raise click.Abort()
         args.overwrite = True
 
     # Chapter select or manual offset
     start, end = _determine_time_range(video_id, args)
```

### Comparing `twitch-dl-2.2.0/twitchdl/commands/info.py` & `twitch_dl-2.2.1/twitchdl/commands/info.py`

 * *Files identical despite different names*

### Comparing `twitch-dl-2.2.0/twitchdl/commands/videos.py` & `twitch_dl-2.2.1/twitchdl/commands/videos.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import sys
+from typing import Optional
 
 import click
 
 from twitchdl import twitch
 from twitchdl.exceptions import ConsoleError
 from twitchdl.output import print_json, print_log, print_paged, print_video, print_video_compact
 
@@ -10,16 +11,16 @@
 def videos(
     channel_name: str,
     *,
     all: bool,
     compact: bool,
     games: list[str],
     json: bool,
-    limit: int | None,
-    pager: int | None,
+    limit: Optional[int],
+    pager: Optional[int],
     sort: twitch.VideosSort,
     type: twitch.VideosType,
 ):
     game_ids = _get_game_ids(games)
 
     # Set different defaults for limit for compact display
     limit = limit or (40 if compact else 10)
```

### Comparing `twitch-dl-2.2.0/twitchdl/download.py` & `twitch_dl-2.2.1/twitchdl/download.py`

 * *Files identical despite different names*

### Comparing `twitch-dl-2.2.0/twitchdl/http.py` & `twitch_dl-2.2.1/twitchdl/http.py`

 * *Files identical despite different names*

### Comparing `twitch-dl-2.2.0/twitchdl/output.py` & `twitch_dl-2.2.1/twitchdl/output.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import json
 from itertools import islice
-from typing import Any, Callable, Generator, TypeVar
+from typing import Any, Callable, Generator, Optional, TypeVar
 
 import click
 
 from twitchdl import utils
 from twitchdl.twitch import Clip, Video
 
 T = TypeVar("T")
@@ -45,15 +45,15 @@
 
 
 def print_paged(
     label: str,
     generator: Generator[T, Any, Any],
     print_fn: Callable[[T], None],
     page_size: int,
-    total_count: int | None = None,
+    total_count: Optional[int] = None,
 ):
     iterator = iter(generator)
     page = list(islice(iterator, page_size))
 
     first = 1
     last = first + len(page) - 1
```

### Comparing `twitch-dl-2.2.0/twitchdl/playlists.py` & `twitch_dl-2.2.1/twitchdl/playlists.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 """
 Parse and manipulate m3u8 playlists.
 """
 
 from dataclasses import dataclass
-from typing import Generator, OrderedDict
+from typing import Generator, Optional, OrderedDict
 
 import click
 import m3u8
 
 from twitchdl import utils
 from twitchdl.output import bold, dim
 
 
 @dataclass
 class Playlist:
     name: str
-    resolution: str | None
+    resolution: Optional[str]
     url: str
 
 
 @dataclass
 class Vod:
     index: int
     """Ordinal number of the VOD in the playlist"""
@@ -49,16 +49,16 @@
 
 def load_m3u8(playlist_m3u8: str) -> m3u8.M3U8:
     return m3u8.loads(playlist_m3u8)
 
 
 def enumerate_vods(
     document: m3u8.M3U8,
-    start: int | None = None,
-    end: int | None = None,
+    start: Optional[int] = None,
+    end: Optional[int] = None,
 ) -> list[Vod]:
     """Extract VODs for download from document."""
     vods = []
     vod_start = 0
 
     for index, segment in enumerate(document.segments):
         vod_end = vod_start + segment.duration
@@ -93,15 +93,15 @@
         if segment.uri in path_map:
             segment.uri = path_map[segment.uri]
             playlist.segments.append(segment)
 
     return playlist
 
 
-def select_playlist(playlists: list[Playlist], quality: str | None) -> Playlist:
+def select_playlist(playlists: list[Playlist], quality: Optional[str]) -> Playlist:
     return (
         select_playlist_by_name(playlists, quality)
         if quality is not None
         else select_playlist_interactive(playlists)
     )
```

### Comparing `twitch-dl-2.2.0/twitchdl/progress.py` & `twitch_dl-2.2.1/twitchdl/progress.py`

 * *Files 20% similar despite different names*

```diff
@@ -123,30 +123,33 @@
 
         first_sample = self.samples[0]
         last_sample = self.samples[-1]
 
         size = last_sample.downloaded - first_sample.downloaded
         duration = last_sample.timestamp - first_sample.timestamp
 
-        return size / duration
+        return size / duration if duration > 0 else None
 
     def print(self):
         now = time.time()
 
         # Don't print more often than 10 times per second
         if now - self.last_printed < 0.1:
             return
 
-        progress = " ".join(
-            [
-                f"Downloaded {self.vod_downloaded_count}/{self.vod_count} VODs",
-                f"{blue(self.progress_perc)}%",
-                f"of ~{blue(format_size(self.estimated_total))}" if self.estimated_total else "",
-                f"at {blue(format_size(self.speed))}/s" if self.speed else "",
-                f"ETA {blue(format_time(self.remaining_time))}"
-                if self.remaining_time is not None
-                else "",
-            ]
-        )
+        click.echo(f"\rDownloaded {self.vod_downloaded_count}/{self.vod_count} VODs", nl=False)
+        click.secho(f" {self.progress_perc}%", fg="blue", nl=False)
+
+        if self.estimated_total is not None:
+            total = f"~{format_size(self.estimated_total)}"
+            click.echo(f" of {blue(total)}", nl=False)
+
+        if self.speed is not None:
+            speed = f"{format_size(self.speed)}/s"
+            click.echo(f" at {blue(speed)}", nl=False)
+
+        if self.remaining_time is not None:
+            click.echo(f" ETA {blue(format_time(self.remaining_time))}", nl=False)
+
+        click.echo("    ", nl=False)
 
-        click.echo(f"\r{progress}     ", nl=False)
         self.last_printed = now
```

### Comparing `twitch-dl-2.2.0/twitchdl/twitch.py` & `twitch_dl-2.2.1/twitchdl/twitch.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 Twitch API access.
 """
 
 import json
-from typing import Dict, Generator, Literal, TypedDict
+from typing import Dict, Generator, Literal, TypedDict, Optional
 
 import click
 import httpx
 
 from twitchdl import CLIENT_ID
 from twitchdl.entities import Data
 from twitchdl.exceptions import ConsoleError
@@ -159,28 +159,28 @@
     broadcaster {
         displayName
         login
     }
 """
 
 
-def get_video(video_id: str) -> Video | None:
+def get_video(video_id: str) -> Optional[Video]:
     query = f"""
     {{
         video(id: "{video_id}") {{
             {VIDEO_FIELDS}
         }}
     }}
     """
 
     response = gql_query(query)
     return response["data"]["video"]
 
 
-def get_clip(slug: str) -> Clip | None:
+def get_clip(slug: str) -> Optional[Clip]:
     query = f"""
     {{
         clip(slug: "{slug}") {{
             {CLIP_FIELDS}
         }}
     }}
     """
@@ -205,15 +205,15 @@
     }}
     """
 
     response = gql_post(query.strip())
     return response["data"]["clip"]
 
 
-def get_channel_clips(channel_id: str, period: ClipsPeriod, limit: int, after: str | None = None):
+def get_channel_clips(channel_id: str, period: ClipsPeriod, limit: int, after: Optional[str] = None):
     """
     List channel clips.
 
     At the time of writing this:
     * filtering by game name returns an error
     * sorting by anything but VIEWS_DESC or TRENDING returns an error
     * sorting by VIEWS_DESC and TRENDING returns the same results
@@ -290,16 +290,16 @@
 
 
 def get_channel_videos(
     channel_id: str,
     limit: int,
     sort: str,
     type: str = "archive",
-    game_ids: list[str] | None = None,
-    after: str | None = None,
+    game_ids: Optional[list[str]] = None,
+    after: Optional[str] = None,
 ):
     game_ids = game_ids or []
 
     query = f"""
     {{
         user(login: "{channel_id}") {{
             videos(
@@ -335,15 +335,15 @@
 
 
 def channel_videos_generator(
     channel_id: str,
     max_videos: int,
     sort: VideosSort,
     type: VideosType,
-    game_ids: list[str] | None = None,
+    game_ids: Optional[list[str]] = None,
 ) -> tuple[int, Generator[Video, None, None]]:
     game_ids = game_ids or []
 
     def _generator(videos: Data, max_videos: int) -> Generator[Video, None, None]:
         for video in videos["edges"]:
             if max_videos < 1:
                 return
@@ -360,15 +360,15 @@
         yield from _generator(videos, max_videos)
 
     limit = min(max_videos, 100)
     videos = get_channel_videos(channel_id, limit, sort, type, game_ids)
     return videos["totalCount"], _generator(videos, max_videos)
 
 
-def get_access_token(video_id: str, auth_token: str | None = None) -> AccessToken:
+def get_access_token(video_id: str, auth_token: Optional[str] = None) -> AccessToken:
     query = f"""
     {{
         videoPlaybackAccessToken(
             id: {video_id},
             params: {{
                 platform: "web",
                 playerBackend: "mediaplayer",
```

### Comparing `twitch-dl-2.2.0/twitchdl/utils.py` & `twitch_dl-2.2.1/twitchdl/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,36 +1,37 @@
 import re
+from typing import Optional, Union
 import unicodedata
 
 import click
 
 
 def _format_size(value: float, digits: int, unit: str):
     if digits > 0:
         return f"{{:.{digits}f}}{unit}".format(value)
     else:
         return f"{int(value)}{unit}"
 
 
-def format_size(bytes_: int | float, digits: int = 1):
+def format_size(bytes_: Union[int, float], digits: int = 1):
     if bytes_ < 1024:
         return _format_size(bytes_, digits, "B")
 
     kilo = bytes_ / 1024
     if kilo < 1024:
         return _format_size(kilo, digits, "kB")
 
     mega = kilo / 1024
     if mega < 1024:
         return _format_size(mega, digits, "MB")
 
     return _format_size(mega / 1024, digits, "GB")
 
 
-def format_duration(total_seconds: int | float) -> str:
+def format_duration(total_seconds: Union[int, float]) -> str:
     total_seconds = int(total_seconds)
     hours = total_seconds // 3600
     remainder = total_seconds % 3600
     minutes = remainder // 60
     seconds = total_seconds % 60
 
     if hours:
@@ -38,28 +39,28 @@
 
     if minutes:
         return f"{minutes} min {seconds} sec"
 
     return f"{seconds} sec"
 
 
-def format_time(total_seconds: int | float, force_hours: bool = False) -> str:
+def format_time(total_seconds: Union[int, float], force_hours: bool = False) -> str:
     total_seconds = int(total_seconds)
     hours = total_seconds // 3600
     remainder = total_seconds % 3600
     minutes = remainder // 60
     seconds = total_seconds % 60
 
     if hours or force_hours:
         return f"{hours:02}:{minutes:02}:{seconds:02}"
 
     return f"{minutes:02}:{seconds:02}"
 
 
-def read_int(msg: str, min: int, max: int, default: int | None = None) -> int:
+def read_int(msg: str, min: int, max: int, default: Optional[int] = None) -> int:
     while True:
         try:
             val = click.prompt(msg, default=default, type=int)
             if default and not val:
                 return default
             if min <= int(val) <= max:
                 return int(val)
@@ -89,21 +90,21 @@
 CLIP_PATTERNS = [
     r"^(?P<slug>[A-Za-z0-9]+(?:-[A-Za-z0-9_-]{16})?)$",
     r"^https://(www.)?twitch.tv/\w+/clip/(?P<slug>[A-Za-z0-9]+(?:-[A-Za-z0-9_-]{16})?)(\?.+)?$",
     r"^https://clips.twitch.tv/(?P<slug>[A-Za-z0-9]+(?:-[A-Za-z0-9_-]{16})?)(\?.+)?$",
 ]
 
 
-def parse_video_identifier(identifier: str) -> str | None:
+def parse_video_identifier(identifier: str) -> Optional[str]:
     """Given a video ID or URL returns the video ID, or null if not matched"""
     for pattern in VIDEO_PATTERNS:
         match = re.match(pattern, identifier)
         if match:
             return match.group("id")
 
 
-def parse_clip_identifier(identifier: str) -> str | None:
+def parse_clip_identifier(identifier: str) -> Optional[str]:
     """Given a clip slug or URL returns the clip slug, or null if not matched"""
     for pattern in CLIP_PATTERNS:
         match = re.match(pattern, identifier)
         if match:
             return match.group("slug")
```

